# Comparing `tmp/libretrofuzz-3.2.2.tar.gz` & `tmp/libretrofuzz-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-3.2.2.tar", max compression
+gzip compressed data, was "libretrofuzz-3.2.3.tar", max compression
```

## Comparing `libretrofuzz-3.2.2.tar` & `libretrofuzz-3.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-18 23:09:50.908152 libretrofuzz-3.2.2/LICENSE
--rw-r--r--   0        0        0     7471 2023-06-18 23:09:50.908152 libretrofuzz-3.2.2/README.rst
--rw-r--r--   0        0        0       22 2023-06-18 23:09:50.908152 libretrofuzz-3.2.2/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    55163 2023-06-18 23:09:50.908152 libretrofuzz-3.2.2/libretrofuzz/__main__.py
--rw-r--r--   0        0        0     1275 2023-06-18 23:09:50.912152 libretrofuzz-3.2.2/pyproject.toml
--rw-r--r--   0        0        0     8651 2023-06-18 23:10:00.195928 libretrofuzz-3.2.2/setup.py
--rw-r--r--   0        0        0     8659 2023-06-18 23:10:00.196968 libretrofuzz-3.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-19 02:17:50.114804 libretrofuzz-3.2.3/LICENSE
+-rw-r--r--   0        0        0     7471 2023-06-19 02:17:50.114804 libretrofuzz-3.2.3/README.rst
+-rw-r--r--   0        0        0       22 2023-06-19 02:17:50.114804 libretrofuzz-3.2.3/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    54640 2023-06-19 02:17:50.114804 libretrofuzz-3.2.3/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0     1275 2023-06-19 02:17:50.114804 libretrofuzz-3.2.3/pyproject.toml
+-rw-r--r--   0        0        0     8651 2023-06-19 02:18:02.618495 libretrofuzz-3.2.3/setup.py
+-rw-r--r--   0        0        0     8659 2023-06-19 02:18:02.619518 libretrofuzz-3.2.3/PKG-INFO
```

### Comparing `libretrofuzz-3.2.2/LICENSE` & `libretrofuzz-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.2.2/README.rst` & `libretrofuzz-3.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.2.2/libretrofuzz/__main__.py` & `libretrofuzz-3.2.3/libretrofuzz/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -974,14 +974,17 @@
     # so the hack and meta matching must be disabled
     if before:
         hack = False
         nometa = True
     # no-fail is equivalent to max fuzz
     if nofail:
         score = 0
+    # filter disables no-merge since the setting deletes the old images
+    if filters:
+        nomerge = False
     # besides the explicit setting these two need to disable images,
     # one because the console is not ready to print images (or emoji)
     # the other to prevent unpleasant empty space.
     if nub_verbose or dryrun:
         noimage = True
 
     thumbs = Thumbs._make(await downloadgamenames(client, system))
@@ -1037,21 +1040,26 @@
         _, max_score, _ = result[0]
         winners = [x for x in result if x[1] == max_score and x[1] >= score]
         show = result if verbose else winners
         name_format = style((nameaux if short_names else name) + ": ", bold=True)
         # still remove the forbidden characters
         # the name will be used in the filename
         name = regex.sub(forbidden, "_", name)
+        # Delete old images in the case of --filter.
+        # this always happens, for consistency
+        if filters:
+            for dirname in Thumbs._fields:
+                Path(thumbnails_dir, destination, dirname, name + ".png").unlink(missing_ok=True)
         if winners:
             allow = True
             # these parent directories were created when reading the playlist
             # more efficient than doing it a playlist game loop
             real_thumb_dir = Path(thumbnails_dir, destination)
             down_thumb_dir = Path(tmpdir, destination)
-            if not filters and nomerge:
+            if nomerge:
                 # to implement no-merge you have to disable downloads on
                 # 'at least one' thumbnail (including user added ones)
                 missing_thumbs = 0
                 served__thumbs = False
                 for dirname in Thumbs._fields:
                     real = Path(real_thumb_dir, dirname, name + ".png")
                     if not real.exists():
@@ -1107,23 +1115,14 @@
                                     MAX_RETRIES,
                                     dryrun,
                                 ):
                                     first_wait = False
                                     downloaded_once = True
                                     urls[(dirname, winner)] = url
                                     break
-                    # Delete old images in the case of --filter.
-                    # internet not available will exit the program
-                    # so this won't happen in a loop in that case
-                    # broken/not found server links WILL get deleted
-                    # it will also skip if the user cancels
-                    # as is logical this is before image display
-                    if filters:
-                        for old, _ in downloaded_dict.values():
-                            old.unlink(missing_ok=True)
                     if not noimage and viewer and downloaded_once:
                         displayImages(downloaded_dict)
                         if wait_after is not None:
                             await printwait(wait_after, waiting_format)
                     if downloaded_once:
                         for old, new in downloaded_dict.values():
                             if new.exists():
@@ -1143,20 +1142,14 @@
                     echo(skipped_format)
         else:
             failure += 1
             if verbose:
                 name_format = name_format + ", ".join((strfy_runtime(x) for x in show))
                 failure_format = f'{style("Failure",     fg=RED, bold=True)}: {name_format}'
                 echo(failure_format)
-            # same idea as above can't be unified because
-            # the above delete needs to be after downloads
-            # but before displaying the image
-            if filters:
-                for dirname in Thumbs._fields:
-                    Path(thumbnails_dir, destination, dirname, name + ".png").unlink(missing_ok=True)
     echo(f"{success}/{len(names)} successes {failure}/{len(names)} failures")
 
 
 async def printwait(wait: Optional[float], waiting_format: str):
     count = int(wait / 0.1)
     with handleContinueDownload():
         for i in trange(count, dynamic_ncols=True, bar_format=waiting_format, leave=False):
```

### Comparing `libretrofuzz-3.2.2/pyproject.toml` & `libretrofuzz-3.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "3.2.2"
+version = "3.2.3"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-3.2.2/setup.py` & `libretrofuzz-3.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '3.2.2',
+    'version': '3.2.3',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get a adequate default that is neither too strict or lax.\n\nIf you still want more thumbnails, using ``libretro-fuzz --min 80 --delay 5 --delay 5`` works (smaller ``--min`` increases fuzz), with some delays introduced to check if you want to keep the game selected for the thumbnails. If you prefer only exact matches, use `--min 100`.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-merge --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nA common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 90 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=60]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=60]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100≃equal, 90=default. No-op with ``--no-fail``.\n                        | [default: 90; 0<=x<=100]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --dry-run             Print results only, no image download.\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-3.2.2/PKG-INFO` & `libretrofuzz-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 3.2.2
+Version: 3.2.3
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

