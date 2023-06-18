# Comparing `tmp/libretrofuzz-3.2.1.tar.gz` & `tmp/libretrofuzz-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-3.2.1.tar", max compression
+gzip compressed data, was "libretrofuzz-3.2.2.tar", max compression
```

## Comparing `libretrofuzz-3.2.1.tar` & `libretrofuzz-3.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-13 16:18:57.774312 libretrofuzz-3.2.1/LICENSE
--rw-r--r--   0        0        0     7471 2023-06-13 16:18:57.774312 libretrofuzz-3.2.1/README.rst
--rw-r--r--   0        0        0       22 2023-06-13 16:18:57.774312 libretrofuzz-3.2.1/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    55734 2023-06-13 16:18:57.774312 libretrofuzz-3.2.1/libretrofuzz/__main__.py
--rw-r--r--   0        0        0     1275 2023-06-13 16:18:57.774312 libretrofuzz-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     8651 2023-06-13 16:19:09.019950 libretrofuzz-3.2.1/setup.py
--rw-r--r--   0        0        0     8659 2023-06-13 16:19:09.021023 libretrofuzz-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-18 23:09:50.908152 libretrofuzz-3.2.2/LICENSE
+-rw-r--r--   0        0        0     7471 2023-06-18 23:09:50.908152 libretrofuzz-3.2.2/README.rst
+-rw-r--r--   0        0        0       22 2023-06-18 23:09:50.908152 libretrofuzz-3.2.2/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    55163 2023-06-18 23:09:50.908152 libretrofuzz-3.2.2/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0     1275 2023-06-18 23:09:50.912152 libretrofuzz-3.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8651 2023-06-18 23:10:00.195928 libretrofuzz-3.2.2/setup.py
+-rw-r--r--   0        0        0     8659 2023-06-18 23:10:00.196968 libretrofuzz-3.2.2/PKG-INFO
```

### Comparing `libretrofuzz-3.2.1/LICENSE` & `libretrofuzz-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.2.1/README.rst` & `libretrofuzz-3.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.2.1/libretrofuzz/__main__.py` & `libretrofuzz-3.2.2/libretrofuzz/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 # have the same system.
 
 from pathlib import Path
 from typing import Optional, List
 from urllib.request import unquote, quote
 from tempfile import TemporaryDirectory
 from contextlib import asynccontextmanager, contextmanager
-from functools import partial
-from itertools import chain
+from itertools import chain, tee
 from struct import unpack
 import json
 import os
 import sys
 import io
 import zlib
 import fnmatch
@@ -46,22 +45,14 @@
 from typer.colors import YELLOW, RED, BLUE, GREEN
 from typer import style, echo, run, Exit, Argument, Option
 from prompt_toolkit.input import create_input
 import regex
 
 regex.DEFAULT_VERSION = regex.VERSION1
 
-# stop showing the variables - a library installed this behind my back
-try:
-    from rich.traceback import install
-
-    install(show_locals=False)
-except ImportError:
-    pass
-
 
 ###########################################
 ########### SCRIPT SETTINGS ###############
 ###########################################
 
 ADDRESS = "https://thumbnails.libretro.com"
 DEF_SCORE = 90
@@ -257,15 +248,15 @@
         elif (ch == close_p) and paren_level:
             paren_level -= 1
         elif not paren_level:
             result += ch
     return result
 
 
-def extractbefore(name, before):
+def extractbefore(before, name):
     if before:
         # Ignore metadata and get the string before it
         name_without_meta = regex.search(r"(^[^\[({]*)", name)
         if name_without_meta:
             before_index = name_without_meta.group(1).find(before)
             if before_index != -1:
                 return name[0:before_index]
@@ -313,46 +304,46 @@
         self.normcache2 = normcache2
         self.hack = hack
 
     def __call__(self, name, other, processor=None, score_cutoff=None):
         if name == other:
             return MAX_SCORE
         (_, name_ns, _, _, digits) = self.normcache[name]
-        (_, other_ns, other_subs, other_ns_subs, other_digits) = self.normcache2[other]
+        (_, other_ns, _, other_ns_subs, other_digits) = self.normcache2[other]
         if name_ns == other_ns:
             return MAX_SCORE
 
         remaining = MAX_SCORE - DEF_SCORE
 
         cnbrs = fuzz.ratio(digits, other_digits)  # normalized to 0-100
         # 2 heuristics (this time), however they don't both have the same weight
         increment_common_number = remaining * 0.03
         increment_common_length = remaining * 0.97
 
-        rest_of_score = increment_common_number * 0.01 * cnbrs  # 100 gives 1
-        common_prop = len(os.path.commonprefix([name_ns, other_ns])) / len(name_ns)
-        rest_of_score += increment_common_length * common_prop
         sum_ns = ""
-        for sub, sub_ns in zip(other_subs, other_ns_subs):
+        for sub_ns in other_ns_subs:
             # if you find a exact match on either a subtitle
             # or a sequence of subtitles from the start, give
             # a 'winning' score but distingish them by the rest
             # by name ratio and digits ratio
             if name_ns == (sum_ns := sum_ns + sub_ns) or name_ns == sub_ns:
                 # reset increment and rest of score
                 rest_of_score = increment_common_number * 0.01 * cnbrs
                 rest_of_score += increment_common_length * 0.01 * fuzz.WRatio(name, other)
                 return DEF_SCORE + rest_of_score
 
+        rest_of_score = increment_common_number * 0.01 * cnbrs  # 100 gives 1
+        common_prop = len(os.path.commonprefix([name_ns, other_ns])) / len(name_ns)
+        rest_of_score += increment_common_length * common_prop
         # give a penality if you got here and the name you're checking against
         # already has a perfect match in the playlist being processed. This usually
         # penalizes hack names but removes a lot of inane false positives
         # (depending on the playlist completeness). Disable it when processing hacks
         # TODO remove this when a feature to choose when waiting happens
-        if not self.hack and other_ns in self.normcache:
+        if not self.hack and other in self.normcache:
             rest_of_score -= remaining * 0.65
         return fuzz.WRatio(name, other) * (DEF_SCORE / 100) + rest_of_score
 
 
 # ---------------------------------------------------------------
 # Normalization functions, part of the functions that change both
 # local labels and remote names to be more similar to compare
@@ -384,17 +375,15 @@
     # Word-Word or Word:Word without creating new subtitle
     # and removing articles from subtitles is helpful anyway
     subtitles = t.split(" - ")
     if len(subtitles) == 1:
         subtitles = t.split(": ")
     subtitles2 = [None] * len(subtitles)
     for i, st in enumerate(subtitles):
-        # remove all symbols, except, ',' and '''
-        # this needs to be here for all the names
-        # to be operating on the same base for definite articles
+        # remove all symbols, except, ',' and ''', here for camelcase split
         st = regex.sub(almost_symbols_pattern, "", st)
         # CamelCaseNames for local labels are common when there are no spaces
         # do this to normalize for definite articles
         st = " ".join([a for s in regex.split(camelcase_pattern, st) if s and (a := s.strip())])
         # Tries to make roman numerals in the range 1-20 equivalent to normal numbers.
         # If both str tested have roman numerals little harm done if XXIV gets turned into 204.
         st = replaceRoman(st, "XVIII", "18")
@@ -510,50 +499,51 @@
     """create directories that are children of temp_dir and thumbnails_dir that have the
     subdirs needed to move files created on them from one to the other, so you don't
     need to care to create directories for every file processed.
     return a list of game names and 'db_names' (stripped of extension): [(names: str,db_names: str)]
     db_names without extension are the system directory names libretro searchs for the thumbnail.
     """
     names = []
-    dbs = set()
+    dbs = []
     try:
         with RzipReader(playlist).open() as f:
             data = json.load(f)
             for r in data["items"]:
                 assert (
                     "label" in r and r["label"].strip() != ""
                 ), f"\n{json.dumps(r,indent=4)} of playlist {playlist} has no label"
                 assert "db_name" in r and r["db_name"].endswith(
                     ".lpl"
                 ), f"\n{json.dumps(r,indent=4)} of playlist {playlist} has no valid db_name"
                 # add the label name and the db name (it's a playlist name, minus the extension '.lpl')
                 db = r["db_name"][:-4]
-                dbs.add(db)
-                names.append((r["label"], db))
+                dbs.append(db)
+                names.append(r["label"])
     except json.JSONDecodeError:
         # older version of the playlist format, this has no error correction; the extra lines after the
         # game entries can be between 0 and 5, because retroarch will ignore lines missing at the end.
         with RzipReader(playlist).open() as f:
             # make sure not to count empty lines, which might break the assumptions made here
             data = [x for x in map(str.strip, f.readlines()) if x]
             gamelineslen = len(data) - (len(data) % 6)
             for i in range(0, gamelineslen, 6):
                 name = data[i + 1]
                 db = data[i + 5][:-4]
-                dbs.add(db)
-                names.append((name, db))
+                dbs.append(db)
+                names.append(name)
     # create the directories we will 'maybe' need. This is not so problematic
     # as it seems since likely len(dbs) == 1, so 6 directories per playlist
     # versus having os.makedirs called hundred of times for larger playlists
     # this is vulnerable to ToCToU deletion but everything is with directories
+    dbs_set = set(dbs)
     for parent in [temp_dir, thumbnails_dir]:
-        for db in dbs:
+        for db in dbs_set:
             for dirname in Thumbs._fields:
                 os.makedirs(Path(parent, db, dirname), exist_ok=True)
-    return names
+    return names, dbs
 
 
 def getPath(cfg: Path, setting: str, default_value: str):
     """returns paths inside of a cfg file setting"""
     with open(cfg) as f:
         file_content = "[DUMMY]\n" + f.read()
     configParser = configparser.RawConfigParser()
@@ -760,19 +750,20 @@
         try:
             async with lock_keys(), AsyncClient() as client:
                 # temporary dir for downloads (required to prevent clobbering)
                 # parent directory of this temp dir is the same as the
                 # RA thumbnail dir to make mv the file just renaming, not cp
                 with TemporaryDirectory(prefix="libretrofuzz", dir=thumbnails_dir) as tmpdir:
                     echo(style(f"{playlist} -> {system}", bold=True))
-                    names = readPlaylistAndPrepareDirectories(
+                    names, dbs = readPlaylistAndPrepareDirectories(
                         Path(playlist_dir, playlist), tmpdir, thumbnails_dir
                     )
                     await downloader(
                         names,
+                        dbs,
                         system,
                         wait_before,
                         wait_after,
                         filters,
                         dryrun,
                         score,
                         noimage,
@@ -880,18 +871,19 @@
                     for playlist, system in notInSystems:
                         echo(
                             style("Custom playlist skipped: ", fg=RED, bold=True)
                             + style(f"{system}.lpl", bold=True)
                         )
                     for playlist, system in inSystems:
                         echo(style(f"{system}.lpl -> {system}", bold=True))
-                        names = readPlaylistAndPrepareDirectories(playlist, tmpdir, thumbnails_dir)
+                        names, dbs = readPlaylistAndPrepareDirectories(playlist, tmpdir, thumbnails_dir)
                         try:
                             await downloader(
                                 names,
+                                dbs,
                                 system,
                                 wait_before,
                                 wait_after,
                                 filters,
                                 dryrun,
                                 score,
                                 noimage,
@@ -948,15 +940,16 @@
     except (RequestError, HTTPStatusError) as err:
         error(f"Could not get the remote thumbnail game names, exiting: {err}")
         raise Exit(code=1)
     return args
 
 
 async def downloader(
-    names: [(str, str)],
+    names: [str],
+    dbs: [str],
     system: str,
     wait_before: Optional[float],
     wait_after: Optional[float],
     filters: Optional[List[str]],
     dryrun: bool,
     score: int,
     noimage: bool,
@@ -967,14 +960,17 @@
     verbose: Optional[int],
     nub_verbose: bool,
     before: Optional[str],
     tmpdir: Path,
     thumbnails_dir: Path,
     client: AsyncClient,
 ):
+    # number of success and failures to print at the end
+    failure = 0
+    success = 0
     # not a error to pass a empty playlist
     if len(names) == 0:
         return
     # before implies that the names of the playlists may be cut,
     # so the hack and meta matching must be disabled
     if before:
         hack = False
@@ -984,58 +980,52 @@
         score = 0
     # besides the explicit setting these two need to disable images,
     # one because the console is not ready to print images (or emoji)
     # the other to prevent unpleasant empty space.
     if nub_verbose or dryrun:
         noimage = True
 
-    # build the function that will be called to print data,
-    # filling in some fixed arguments
-    short_names = os.getenv("SHORT")
-    short_names = True if short_names and short_names != "0" else False
-    strfy_runtime = partial(strfy, score, short_names, nub_verbose)
-    norm = partial(normalizer, nometa, hack)
-    failure = 0
-    success = 0
-
     thumbs = Thumbs._make(await downloadgamenames(client, system))
     # we choose the highest similarity of all 3 directories,
     # since no mixed matches are allowed
     # (until you call again without --no-merge anyway
     # or if they have the same score)
     remote_names = set()
     remote_names.update(thumbs.Named_Boxarts.keys(), thumbs.Named_Titles.keys(), thumbs.Named_Snaps.keys())
     if not remote_names:
         raise StopPlaylist()
 
+    # build the function that will be called to print data
+    short_names = os.getenv("SHORT")
+    short_names = True if short_names and short_names != "0" else False
+
+    def strfy_runtime(s, urldict=None):
+        return strfy(score, short_names, nub_verbose, s, urldict)
+
     # preprocess data to build a heuristic later. Do not move
     # into the later loop because thats when the heuristic is used
-    normcache = dict()
-    # nonetheless save the normalization to not be forced to redo it
-    for name, _ in names:
-        # done before the forbidden removal because the 'before' str might have '_'
-        norm_name = extractbefore(name, before)
-        # this is the character that libretro-thumbnails uses as placeholder
-        norm_name = regex.sub(forbidden, "_", norm_name)
-        normtuple = norm(norm_name)
-        # cache normalization with all the name variants checked
-        # reason is to be able to reuse the calculation (name)
-        normcache[name] = normtuple  # original
-        # check if server names are equal to playlist normalized variants
-        normcache[normtuple[0]] = normtuple  # normalized
-        normcache[normtuple[1]] = normtuple  # normalized nospace
-    tmpdict = dict()
-    normcache2 = dict()
-    for x in remote_names:
-        normtuple = norm(x)
-        normcache2[normtuple[0]] = normtuple  # normalized only
-        tmpdict[x] = normtuple[0]
-    remote_names = tmpdict
+    def norm(n):
+        return normalizer(nometa, hack, n)
+
+    def norm_local(n):
+        return norm(regex.sub(forbidden, "_", extractbefore(before, n)))
+
+    a, b = tee(map(norm_local, names))
+    # store normalized local name as key
+    normcache = {t[0]: t for t in a}
+    # store the actual local name as key (cache)
+    normcache.update(zip(names, b))
+    # remote names normalization and cache
+    a, b = tee(map(norm, remote_names))
+    # store normalized remote name as key
+    normcache2 = {t[0]: t for t in a}
+    # remote name as key, normalized remote name as value
+    remote_names = {x: t[0] for x, t in zip(remote_names, b)}
     scorer = TitleScorer(normcache, normcache2, hack)
-    for name, destination in names:
+    for name, destination in zip(names, dbs):
         await asyncio.sleep(0)  # update key status
         checkEscape()  # check key status
         # if the user used filters, filter everything that doesn't match any of the globs
         if filters and not any(map(lambda x: fnmatch.fnmatch(name, x), filters)):
             continue
         # cached normalized name
         nameaux = normcache[name][0]
```

### Comparing `libretrofuzz-3.2.1/pyproject.toml` & `libretrofuzz-3.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "3.2.1"
+version = "3.2.2"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-3.2.1/setup.py` & `libretrofuzz-3.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '3.2.1',
+    'version': '3.2.2',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get a adequate default that is neither too strict or lax.\n\nIf you still want more thumbnails, using ``libretro-fuzz --min 80 --delay 5 --delay 5`` works (smaller ``--min`` increases fuzz), with some delays introduced to check if you want to keep the game selected for the thumbnails. If you prefer only exact matches, use `--min 100`.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-merge --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nA common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 90 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=60]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=60]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100≃equal, 90=default. No-op with ``--no-fail``.\n                        | [default: 90; 0<=x<=100]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --dry-run             Print results only, no image download.\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-3.2.1/PKG-INFO` & `libretrofuzz-3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 3.2.1
+Version: 3.2.2
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

