# Comparing `tmp/xklb-1.31.9.tar.gz` & `tmp/xklb-2.1.2.tar.gz`

## Comparing `xklb-1.31.9.tar` & `xklb-2.1.2.tar`

### file list

```diff
@@ -1,68 +1,70 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.31.9/.gitattributes
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 xklb-1.31.9/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.31.9/Windows.md
--rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-1.31.9/pdm.lock
--rw-r--r--   0        0        0    19420 2020-02-02 00:00:00.000000 xklb-1.31.9/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.31.9/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.31.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.31.9/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-1.31.9/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-1.31.9/.github/workflows/push.yaml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/__init__.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/books.py
--rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/consts.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/dl_config.py
--rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/dl_extract.py
--rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/fs_extract.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/gdl_extract.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/gui.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/hn_extract.py
--rw-r--r--   0        0        0    11781 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/lb.py
--rw-r--r--   0        0        0     7649 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/media.py
--rw-r--r--   0        0        0    25369 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/play_actions.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/playback.py
--rw-r--r--   0        0        0    35233 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/player.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/playlists.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/praw_extract.py
--rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/search.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/subtitle.py
--rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/tabs_extract.py
--rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/tube_backend.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/tube_extract.py
--rw-r--r--   0        0        0    76102 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/usage.py
--rw-r--r--   0        0        0    37860 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/relmv.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.31.9/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.31.9/LICENSE
--rw-r--r--   0        0        0    98892 2020-02-02 00:00:00.000000 xklb-1.31.9/README.md
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-1.31.9/pyproject.toml
--rw-r--r--   0        0        0   102519 2020-02-02 00:00:00.000000 xklb-1.31.9/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.1.2/.gitattributes
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 xklb-2.1.2/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.1.2/Windows.md
+-rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-2.1.2/pdm.lock
+-rw-r--r--   0        0        0    13086 2020-02-02 00:00:00.000000 xklb-2.1.2/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.1.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.1.2/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-2.1.2/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/books.py
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/consts.py
+-rw-r--r--   0        0        0     8337 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/db.py
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/dl_config.py
+-rw-r--r--   0        0        0    11904 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/gui.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/history.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/hn_extract.py
+-rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/lb.py
+-rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/media.py
+-rw-r--r--   0        0        0    25300 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/play_actions.py
+-rw-r--r--   0        0        0    34352 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/player.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/playlists.py
+-rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/subtitle.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/tube_extract.py
+-rw-r--r--   0        0        0    83144 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/usage.py
+-rw-r--r--   0        0        0    38734 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.1.2/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.1.2/LICENSE
+-rw-r--r--   0        0        0    84692 2020-02-02 00:00:00.000000 xklb-2.1.2/README.md
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0    88318 2020-02-02 00:00:00.000000 xklb-2.1.2/PKG-INFO
```

### Comparing `xklb-1.31.9/TODO` & `xklb-2.1.2/TODO`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,31 @@
-
-lb bigdirs ~/lb/video.db
-
-/mnt/d/75_MovieQueue/unsorted/NRMwalkthroughHD/ should be 200GB
-
-
-- move mpv specific playhead code to a script subcommand
-
-option to delete mpv watch_later file if media file does not exist
-
-- dlstatus print errors also:
-
-sqlite lb/fs/blogspot.db 'select error, count(*) from media group by 1 order by 2'
-[{"error": "NoExtractorError", "count(*)": 21},
- {"error": null, "count(*)": 46},
- {"error": "HTTPError", "count(*)": 112},
- {"error": "HTTPNotFoundError", "count(*)": 118}]
-
-- if limit is less than 120, check up to 120 files to see if they exist
-
 - use socket-play as default playback -- accurately get playhead
 
-- move time_played, playhead, and other sparse or ephemeral data to its own table
-
-add time_first_played, time_last_played; remove time_played instead use play_count
-
-- scatter -- flatten to new directories
-
-default 16000 files, flat subdirectory
-
 - POIs CLI -- save your trip plans and see places to go with automated day trip itineraries, geopandas buffer
 
 - wt/lt/search join and use fts on both tables, threading ?
 
 - improve playlists subcommand
 
 - upscale command -- download higher quality videos; use webpath, PURL, comment to get URL
 
 - make generic printer. support --json or --csv for most subcommands
 
 - improve dlstatus subcommand tests
 
-- scan bpm and key sig  https://github.com/aubio/aubio https://github.com/tyiannak/pyAudioAnalysis
+- scan bpm and key sig
+
+    https://github.com/aubio/aubio
+    https://github.com/tyiannak/pyAudioAnalysis
 
 - cluster images
 
-https://github.com/HughKu/Im2txt
-https://github.com/immich-app/immich/tree/main/machine-learning/app
+    https://github.com/rhsimplex/image-match/blob/master/image_match/goldberg.py
+    https://github.com/HughKu/Im2txt
+    https://github.com/immich-app/immich/tree/main/machine-learning/app
 
 - CLI EDA tool
 
 - CLI incremental diff (SQLITE, NDJSON, CSV)
 
     compare 100 rows at a time using primary key
```

### Comparing `xklb-1.31.9/Windows.md` & `xklb-2.1.2/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/pdm.lock` & `xklb-2.1.2/pdm.lock`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,15 @@
 name = "future"
 version = "0.18.3"
 requires_python = ">=2.6, !=3.0.*, !=3.1.*, !=3.2.*"
 summary = "Clean single-source support for Python 3 and 2"
 
 [[package]]
 name = "gallery-dl"
-version = "1.25.5"
+version = "1.25.6"
 requires_python = ">=3.4"
 summary = "Command-line program to download image galleries and collections from several image hosting sites"
 dependencies = [
     "requests>=2.11.0",
 ]
 
 [[package]]
@@ -376,15 +376,15 @@
 summary = "Easy-to-use, Pythonic and complete IMAP client library"
 dependencies = [
     "six",
 ]
 
 [[package]]
 name = "importlib-metadata"
-version = "6.6.0"
+version = "6.7.0"
 requires_python = ">=3.7"
 summary = "Read metadata from Python packages"
 dependencies = [
     "zipp>=0.5",
 ]
 
 [[package]]
@@ -641,15 +641,15 @@
 name = "pillow"
 version = "9.5.0"
 requires_python = ">=3.7"
 summary = "Python Imaging Library (Fork)"
 
 [[package]]
 name = "platformdirs"
-version = "3.5.3"
+version = "3.6.0"
 requires_python = ">=3.7"
 summary = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 
 [[package]]
 name = "pluggy"
 version = "1.0.0"
 requires_python = ">=3.6"
@@ -1194,15 +1194,15 @@
 [[package]]
 name = "wcwidth"
 version = "0.2.6"
 summary = "Measures the displayed width of unicode strings in a terminal"
 
 [[package]]
 name = "websocket-client"
-version = "1.5.3"
+version = "1.6.0"
 requires_python = ">=3.7"
 summary = "WebSocket client for Python with low level API options"
 
 [[package]]
 name = "websockets"
 version = "11.0.3"
 requires_python = ">=3.7"
@@ -1257,15 +1257,15 @@
     "mutagen",
     "pycryptodomex",
     "websockets",
 ]
 
 [[package]]
 name = "zeroconf"
-version = "0.66.0"
+version = "0.69.0"
 requires_python = ">=3.7,<4.0"
 summary = "A pure python implementation of multicast DNS service discovery"
 dependencies = [
     "async-timeout>=3.0.0; python_version < \"3.11\"",
     "ifaddr>=0.1.7",
 ]
 
@@ -1982,17 +1982,17 @@
 "ftfy 6.1.1" = [
     {url = "https://files.pythonhosted.org/packages/97/16/79c6e17bd3465f6498282dd23813846c68cd0989fe60bfef68bb1918d041/ftfy-6.1.1.tar.gz", hash = "sha256:bfc2019f84fcd851419152320a6375604a0f1459c281b5b199b2cd0d2e727f8f"},
     {url = "https://files.pythonhosted.org/packages/e1/1e/bf736f9576a8979752b826b75cbd83663ff86634ea3055a766e2d8ad3ee5/ftfy-6.1.1-py3-none-any.whl", hash = "sha256:0ffd33fce16b54cccaec78d6ec73d95ad370e5df5a25255c8966a6147bd667ca"},
 ]
 "future 0.18.3" = [
     {url = "https://files.pythonhosted.org/packages/8f/2e/cf6accf7415237d6faeeebdc7832023c90e0282aa16fd3263db0eb4715ec/future-0.18.3.tar.gz", hash = "sha256:34a17436ed1e96697a86f9de3d15a3b0be01d8bc8de9c1dffd59fb8234ed5307"},
 ]
-"gallery-dl 1.25.5" = [
-    {url = "https://files.pythonhosted.org/packages/77/f6/f62a94277168fd5f2adbed55f2358250b0aa3eb9508847fedb73090e842d/gallery_dl-1.25.5.tar.gz", hash = "sha256:205cca54722e659d962e4db766acb1bf0c57178e5fd8efd502a43f8fdf31e1a8"},
-    {url = "https://files.pythonhosted.org/packages/aa/d9/f9e4e2f7722c2b4c27fab9431c85b2e7f40c870d0537955073e548ea2ddf/gallery_dl-1.25.5-py3-none-any.whl", hash = "sha256:9b2c7f16954eeceeb8ede1f88f5e7b6bd13ebc680d54b5e8fee8e997d587e930"},
+"gallery-dl 1.25.6" = [
+    {url = "https://files.pythonhosted.org/packages/45/f6/e87f5b13503dff408c202d79d1bdd1c0ff348d92fc463452c02b9f1ae1a3/gallery_dl-1.25.6-py3-none-any.whl", hash = "sha256:a2ae6a06610d905dc86f9ebd091a3619586b9671c70b0c5d3ac9536e4b4cdd80"},
+    {url = "https://files.pythonhosted.org/packages/60/78/176e7c4310a6c200372871a005da8ee5447c0e62cd3533172e009b71a94a/gallery_dl-1.25.6.tar.gz", hash = "sha256:0824ceff5b7a9482b69d02adaa05aad07026efad2de6d3a183cbfdf7352463f5"},
 ]
 "guessit 3.7.1" = [
     {url = "https://files.pythonhosted.org/packages/96/5f/64304acee35bac703cee51656a5caf37bd18c9490561fbff225922f41d39/guessit-3.7.1.tar.gz", hash = "sha256:2c18d982ee6db30db5d59557add0324a2b49bf3940a752947510632a2b58a3c1"},
     {url = "https://files.pythonhosted.org/packages/db/5e/eec6416047845a745b1d2aee181244b380e59158e29d814021d2e511b267/guessit-3.7.1-py3-none-any.whl", hash = "sha256:c3be280ee8ec581a45ca6a654a92e317bf89567fdc55e7167452226f4f5b8b38"},
 ]
 "humanize 4.6.0" = [
     {url = "https://files.pythonhosted.org/packages/06/b1/9e491df2ee1c919d67ee328d8bc9f17b7a9af68e4077f3f5fac83a4488c9/humanize-4.6.0.tar.gz", hash = "sha256:5f1f22bc65911eb1a6ffe7659bd6598e33dcfeeb904eb16ee1e705a09bf75916"},
@@ -2006,17 +2006,17 @@
     {url = "https://files.pythonhosted.org/packages/9c/1f/19ebc343cc71a7ffa78f17018535adc5cbdd87afb31d7c34874680148b32/ifaddr-0.2.0-py3-none-any.whl", hash = "sha256:085e0305cfe6f16ab12d72e2024030f5d52674afad6911bb1eee207177b8a748"},
     {url = "https://files.pythonhosted.org/packages/e8/ac/fb4c578f4a3256561548cd825646680edcadb9440f3f68add95ade1eb791/ifaddr-0.2.0.tar.gz", hash = "sha256:cc0cbfcaabf765d44595825fb96a99bb12c79716b73b44330ea38ee2b0c4aed4"},
 ]
 "imapclient 2.1.0" = [
     {url = "https://files.pythonhosted.org/packages/dc/39/e1c2c2c6e2356ab6ea81fcfc0a74b044b311d6a91a45300811d9a6077ef7/IMAPClient-2.1.0-py2.py3-none-any.whl", hash = "sha256:3eeb97b9aa8faab0caa5024d74bfde59408fbd542781246f6960873c7bf0dd01"},
     {url = "https://files.pythonhosted.org/packages/ea/31/883f78210ed7578f6dd41e4dbc3ad5e7c6127a51e56513b8b7bb7efdf9b3/IMAPClient-2.1.0.zip", hash = "sha256:60ba79758cc9f13ec910d7a3df9acaaf2bb6c458720d9a02ec33a41352fd1b99"},
 ]
-"importlib-metadata 6.6.0" = [
-    {url = "https://files.pythonhosted.org/packages/0b/1f/9de392c2b939384e08812ef93adf37684ec170b5b6e7ea302d9f163c2ea0/importlib_metadata-6.6.0.tar.gz", hash = "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"},
-    {url = "https://files.pythonhosted.org/packages/30/bb/bf2944b8b88c65b797acc2c6a2cb0fb817f7364debf0675792e034013858/importlib_metadata-6.6.0-py3-none-any.whl", hash = "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed"},
+"importlib-metadata 6.7.0" = [
+    {url = "https://files.pythonhosted.org/packages/a3/82/f6e29c8d5c098b6be61460371c2c5591f4a335923639edec43b3830650a4/importlib_metadata-6.7.0.tar.gz", hash = "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4"},
+    {url = "https://files.pythonhosted.org/packages/ff/94/64287b38c7de4c90683630338cf28f129decbba0a44f0c6db35a873c73c4/importlib_metadata-6.7.0-py3-none-any.whl", hash = "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"},
 ]
 "importlib-resources 5.12.0" = [
     {url = "https://files.pythonhosted.org/packages/38/71/c13ea695a4393639830bf96baea956538ba7a9d06fcce7cef10bfff20f72/importlib_resources-5.12.0-py3-none-any.whl", hash = "sha256:7b1deeebbf351c7578e09bf2f63fa2ce8b5ffec296e0d349139d43cca061a81a"},
     {url = "https://files.pythonhosted.org/packages/4e/a2/3cab1de83f95dd15297c15bdc04d50902391d707247cada1f021bbfe2149/importlib_resources-5.12.0.tar.gz", hash = "sha256:4be82589bf5c1d7999aedf2a45159d10cb3ca4f19b2271f8792bc8e6da7b22f6"},
 ]
 "iniconfig 2.0.0" = [
     {url = "https://files.pythonhosted.org/packages/d7/4b/cbd8e699e64a6f16ca3a8220661b5f83792b3017d0f79807cb8708d33913/iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
@@ -2519,17 +2519,17 @@
     {url = "https://files.pythonhosted.org/packages/d9/0e/7c6f054022235830dc2c37ec83e947d9ca09b0b0361e1e5e29983da92294/Pillow-9.5.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:cb841572862f629b99725ebaec3287fc6d275be9b14443ea746c1dd325053cbd"},
     {url = "https://files.pythonhosted.org/packages/db/5c/ba9e291850f594f89436cdca93d36c6f8610d4fb7833a6c257f4481d4174/Pillow-9.5.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:662da1f3f89a302cc22faa9f14a262c2e3951f9dbc9617609a47521c69dd9f8f"},
     {url = "https://files.pythonhosted.org/packages/e7/2a/f3ed578595f8486ee2cc07434460097d89aedd406a3db849b890ca8ec416/Pillow-9.5.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:a127ae76092974abfbfa38ca2d12cbeddcdeac0fb71f9627cc1135bedaf9d51a"},
     {url = "https://files.pythonhosted.org/packages/ec/7d/01404982db598f271ac7c0d0207860f60ab9288cfacce9872eb567cfbfe3/Pillow-9.5.0-cp37-cp37m-macosx_10_10_x86_64.whl", hash = "sha256:5d4ebf8e1db4441a55c509c4baa7a0587a0210f7cd25fcfe74dbbce7a4bd1906"},
     {url = "https://files.pythonhosted.org/packages/f2/43/0892913d499c8df2c88dee69d59e77de19e0c51754a9be82023880641c09/Pillow-9.5.0-cp39-cp39-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:8aca1152d93dcc27dc55395604dcfc55bed5f25ef4c98716a928bacba90d33a3"},
     {url = "https://files.pythonhosted.org/packages/ff/fc/48a51c0fe2a00d5def57b9981a1e0f8339b516351da7a51500383d833bc8/Pillow-9.5.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:608488bdcbdb4ba7837461442b90ea6f3079397ddc968c31265c1e056964f1ef"},
 ]
-"platformdirs 3.5.3" = [
-    {url = "https://files.pythonhosted.org/packages/6d/1a/96efea7b36835ce89911d7813fe68f5b1db7ecae4023bf209a7aeba93017/platformdirs-3.5.3-py3-none-any.whl", hash = "sha256:0ade98a4895e87dc51d47151f7d2ec290365a585151d97b4d8d6312ed6132fed"},
-    {url = "https://files.pythonhosted.org/packages/d2/5d/29eed8861e07378ef46e956650615a9677f8f48df7911674f923236ced2b/platformdirs-3.5.3.tar.gz", hash = "sha256:e48fabd87db8f3a7df7150a4a5ea22c546ee8bc39bc2473244730d4b56d2cc4e"},
+"platformdirs 3.6.0" = [
+    {url = "https://files.pythonhosted.org/packages/05/31/793923615e85deef0c25abf5d044b3f99f1348b620122ab184b7d3f70f21/platformdirs-3.6.0.tar.gz", hash = "sha256:57e28820ca8094678b807ff529196506d7a21e17156cb1cddb3e74cebce54640"},
+    {url = "https://files.pythonhosted.org/packages/a7/4d/00f9fe4bbb3459da0d6c790b1526e5edebaeff2a80166eabb0a42f9e0a05/platformdirs-3.6.0-py3-none-any.whl", hash = "sha256:ffa199e3fbab8365778c4a10e1fbf1b9cd50707de826eb304b50e57ec0cc8d38"},
 ]
 "pluggy 1.0.0" = [
     {url = "https://files.pythonhosted.org/packages/9e/01/f38e2ff29715251cf25532b9082a1589ab7e4f571ced434f98d0139336dc/pluggy-1.0.0-py2.py3-none-any.whl", hash = "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"},
     {url = "https://files.pythonhosted.org/packages/a1/16/db2d7de3474b6e37cbb9c008965ee63835bba517e22cdb8c35b5116b5ce1/pluggy-1.0.0.tar.gz", hash = "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159"},
 ]
 "praw 7.7.0" = [
     {url = "https://files.pythonhosted.org/packages/b3/93/55ae62910b94b46ecdd0ee8765289304f8df8deeaa1df7a96b0831c637ff/praw-7.7.0-py3-none-any.whl", hash = "sha256:22155c4b3006733a5ab0754136cf2226917747b61ec037ee335246fe0db5420e"},
@@ -3143,17 +3143,17 @@
     {url = "https://files.pythonhosted.org/packages/3e/09/bbd7e880b56e825d5859a58adb1bd1feb45b604218706057ca1e3278fa62/wasabi-1.1.2.tar.gz", hash = "sha256:1aaef3aceaa32edb9c91330d29d3936c0c39fdb965743549c173cb54b16c30b5"},
     {url = "https://files.pythonhosted.org/packages/8f/69/26cbf0bad11703241cb84d5324d868097f7a8faf2f1888354dac8883f3fc/wasabi-1.1.2-py3-none-any.whl", hash = "sha256:0a3f933c4bf0ed3f93071132c1b87549733256d6c8de6473c5f7ed2e171b5cf9"},
 ]
 "wcwidth 0.2.6" = [
     {url = "https://files.pythonhosted.org/packages/20/f4/c0584a25144ce20bfcf1aecd041768b8c762c1eb0aa77502a3f0baa83f11/wcwidth-0.2.6-py2.py3-none-any.whl", hash = "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e"},
     {url = "https://files.pythonhosted.org/packages/5e/5f/1e4bd82a9cc1f17b2c2361a2d876d4c38973a997003ba5eb400e8a932b6c/wcwidth-0.2.6.tar.gz", hash = "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"},
 ]
-"websocket-client 1.5.3" = [
-    {url = "https://files.pythonhosted.org/packages/98/be/1aa255e5b937e62ca81b6d990e372bc013e355bd8048b8579eefe24ad57d/websocket-client-1.5.3.tar.gz", hash = "sha256:b96f3bce3e54e3486ebe6504bc22bd4c140392bd2eb71764db29be8f2639aa65"},
-    {url = "https://files.pythonhosted.org/packages/c6/12/76e939a8b7757eb7675d5b8996e07733a180161397ed0904c16128721e40/websocket_client-1.5.3-py3-none-any.whl", hash = "sha256:3566f8467cd350874c4913816355642a4942f6c1ed1e9406e3d42fae6d6c072a"},
+"websocket-client 1.6.0" = [
+    {url = "https://files.pythonhosted.org/packages/31/4e/aa6ab8f8812b5766350ed2beb5bc6f3a007c448dd9c178ef5db2d163dac3/websocket-client-1.6.0.tar.gz", hash = "sha256:e84c7eafc66aade6d1967a51dfd219aabdf81d15b9705196e11fd81f48666b78"},
+    {url = "https://files.pythonhosted.org/packages/cd/b9/cf588fc9e8cdfe2cdb22360c608a9337918ee63ded9b232fe9c1c46e1d8a/websocket_client-1.6.0-py3-none-any.whl", hash = "sha256:72d7802608745b0a212f79b478642473bd825777d8637b6c8c421bf167790d4f"},
 ]
 "websockets 11.0.3" = [
     {url = "https://files.pythonhosted.org/packages/03/28/3a51ffcf51ac45746639f83128908bbb1cd212aa631e42d15a7acebce5cb/websockets-11.0.3-pp37-pypy37_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e052b8467dd07d4943936009f46ae5ce7b908ddcac3fda581656b1b19c083d9b"},
     {url = "https://files.pythonhosted.org/packages/0a/84/68b848a373493b58615d6c10e9e8ccbaadfd540f84905421739a807704f8/websockets-11.0.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:aa5003845cdd21ac0dc6c9bf661c5beddd01116f6eb9eb3c8e272353d45b3288"},
     {url = "https://files.pythonhosted.org/packages/0f/d8/a997d3546aef9cc995a1126f7d7ade96c0e16c1a0efb9d2d430aee57c925/websockets-11.0.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:619d9f06372b3a42bc29d0cd0354c9bb9fb39c2cbc1a9c5025b4538738dbffaf"},
     {url = "https://files.pythonhosted.org/packages/14/fc/5cbbf439c925e1e184a0392ec477a30cee2fabc0e63807c1d4b6d570fb52/websockets-11.0.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:b30c6590146e53149f04e85a6e4fcae068df4289e31e4aee1fdf56a0dead8f97"},
     {url = "https://files.pythonhosted.org/packages/16/49/ae616bd221efba84a3d78737b417f704af1ffa36f40dcaba5eb954dd4753/websockets-11.0.3-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:e848f46a58b9fcf3d06061d17be388caf70ea5b8cc3466251963c8345e13f7eb"},
@@ -3315,62 +3315,62 @@
     {url = "https://files.pythonhosted.org/packages/fb/2d/060ab740f64ea6ea2088e375c3046839faaf4bbba2b65a5364668bd765e7/yarl-1.9.2-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:84e0b1599334b1e1478db01b756e55937d4614f8654311eb26012091be109d59"},
     {url = "https://files.pythonhosted.org/packages/fe/7d/9d85f658b6f7c041ca3ba371d133040c4dc41eb922aef0a6ba917291d187/yarl-1.9.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:aff634b15beff8902d1f918012fc2a42e0dbae6f469fce134c8a0dc51ca423bb"},
 ]
 "yt-dlp 2023.3.4" = [
     {url = "https://files.pythonhosted.org/packages/a7/df/498c57f641e9993376cf52489047158e6d660e8bab06b72c470ad5cce2bd/yt_dlp-2023.3.4-py2.py3-none-any.whl", hash = "sha256:40ca421407ce07c8fd700854fd978d58526ec6fff3468caa34ff1c7333b8dc34"},
     {url = "https://files.pythonhosted.org/packages/e8/4a/1e01f24fcb49191626e2b17d00e13a093315d03a9da09fccb1c75913e420/yt-dlp-2023.3.4.tar.gz", hash = "sha256:265d5da97a76c15d7d9a4088a67b78acd5dcf6f8cfd8257c52f581ff996ff515"},
 ]
-"zeroconf 0.66.0" = [
-    {url = "https://files.pythonhosted.org/packages/01/8d/21b7888f9ff1ba9636b20b04047ad0ed3adc50412c23583955dd17022533/zeroconf-0.66.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9a24696415df8fab6c588ab42cde5d90ede8e5b2f491f1bf430f345993697648"},
-    {url = "https://files.pythonhosted.org/packages/05/8b/4e33d4cd95f3ce0305d033eebc5dfbc5355c54a3fa9a010749a18756858f/zeroconf-0.66.0-cp310-cp310-manylinux_2_31_x86_64.whl", hash = "sha256:7d525441081ece62a08caf39d5fbfcd63d0f4207534c48847339a467abcb3ebf"},
-    {url = "https://files.pythonhosted.org/packages/06/06/3fb05d32ab98779fa749164eae148a652ded2ff567afe88d86e3bcc19044/zeroconf-0.66.0-pp37-pypy37_pp73-macosx_11_0_x86_64.whl", hash = "sha256:414581e7cd3074132c9ce55cde9dcd8b1dfb95c69d4d7a9d61f206915f5b3be6"},
-    {url = "https://files.pythonhosted.org/packages/07/22/c38d8501f829fe3287cac4765b63a1876180e9848562ecf2c81fb5ff3b38/zeroconf-0.66.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:0844743c5bc5ca57310a5939d388f72b3973f32d75bc2c5d9b475104e09c66ef"},
-    {url = "https://files.pythonhosted.org/packages/09/ba/1176554e377100f1f1d963397dc33fd27e33166774423846732e2f8aa497/zeroconf-0.66.0-cp38-cp38-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:19b70f63950a60d3729de9f7a45cd01704d796dab01e8246a79f3420c527878e"},
-    {url = "https://files.pythonhosted.org/packages/09/c1/cae76f0b9580ff1d116f2f61659e7c74f950d6e4ea433ceba697711fd76e/zeroconf-0.66.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:a6a857dcb71ed5c6a5a3b8668effbdfe09a2383bf33fe659c6bcd034f1263467"},
-    {url = "https://files.pythonhosted.org/packages/0c/1f/28b1099f31751f9cfa4d4071082022509d55726f92b097d398b3db587af6/zeroconf-0.66.0-cp37-cp37m-win32.whl", hash = "sha256:c632a04b2d314b52a2e29dcc453d3fa3d1133b0da94e6025410a21b8323be08b"},
-    {url = "https://files.pythonhosted.org/packages/21/18/fcd54add5cea152355fe99ddfde28f74a4d359cda7bf6e90c4a9ef90f529/zeroconf-0.66.0-cp39-cp39-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:20887b20f26453c41660184895dff387a8155e61f89206ae223b8262b44ae2c8"},
-    {url = "https://files.pythonhosted.org/packages/2a/9c/c1a4bb6f8a073f422b7d264b857ee19f42ba97192e57ef5afe1927a5bf97/zeroconf-0.66.0-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:0356fcbe7073fab997c1e8a475255de64a1f5d891f550c008b68017409373d77"},
-    {url = "https://files.pythonhosted.org/packages/3f/1b/4bcc4b9cd61516ff80fdabdd3344f37081b32cd799fb1a8cd9cd1611417a/zeroconf-0.66.0-cp310-cp310-win32.whl", hash = "sha256:1214f2291f2ee96efeaebc604137cba1408b0054f433af3502321603e218a4b7"},
-    {url = "https://files.pythonhosted.org/packages/42/53/65bc5f9239f52701b1b9cd155a3184bd635a39e10fad8caf3d50c492ea1e/zeroconf-0.66.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:9dca4aafee95c92bea2e68791bad7db1d34cb1b792c3f5d348c5f3dbc26ab58e"},
-    {url = "https://files.pythonhosted.org/packages/42/5d/28572cca42b3dab479f705f38684a618b00d8bbd6495ff0dfdd446b6a212/zeroconf-0.66.0-cp37-cp37m-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:45d98c460a9bb51e85e15be95b7d33c01f73ce8302489d67fe961da5d7662139"},
-    {url = "https://files.pythonhosted.org/packages/53/9c/abeefab0652d2ebe78fe8f4bcd6a8c38fbd212c066a2b85a48022327de84/zeroconf-0.66.0-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:1545d10f20152c28e9e73b1f9918bac0174a421ab4d86c1badb1078d89fb0574"},
-    {url = "https://files.pythonhosted.org/packages/56/04/5433a0465e828b2c0fdb844c882a20cb50d6d3abafd7ae44737a23da38cd/zeroconf-0.66.0-cp39-cp39-win32.whl", hash = "sha256:5edc86847ce23c86db6fcef91a162f5a9974928115f158d9e347042fae27663d"},
-    {url = "https://files.pythonhosted.org/packages/5f/15/effb9ac7fabfa95b963bec892da85012014774099928548d47bf096a8ea1/zeroconf-0.66.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:886c665b42df65b35d092e502180f475495d919db0c8b51b462afb8a8c7763c4"},
-    {url = "https://files.pythonhosted.org/packages/5f/45/940e523d7576db80660589c9d7207ce0b38d19332e116eb7bd46404eddcd/zeroconf-0.66.0-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:455daec7b7e9095fc81a2973a0be92187c26d60bdc0009230662e233acc02289"},
-    {url = "https://files.pythonhosted.org/packages/5f/a4/7ce118203229f63bd3c7f29a21568d03c5c6a76db35d07d814cd000118fa/zeroconf-0.66.0-cp310-cp310-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:bbced1ba8013fb9c8e8384e77bded79d8d4ed87195935ccfc9254ffab9f5372f"},
-    {url = "https://files.pythonhosted.org/packages/61/e6/c82b1c39df5b8ff7979272e641b7561b62994845a4d805f9ecdd1447ced6/zeroconf-0.66.0-cp37-cp37m-macosx_11_0_x86_64.whl", hash = "sha256:d560798fd9cffebfc1b22c28e385cb3068cb3511b53fe93334813bb7fa100759"},
-    {url = "https://files.pythonhosted.org/packages/6d/97/e273c09740f12688ed1d00bcb65424e42c6489e3182c00d9e74b44f8fa22/zeroconf-0.66.0.tar.gz", hash = "sha256:1af7dc50d6c26d174e4cd79bc9b390cf42d5ed2dd1ee91c1b113201888143c0d"},
-    {url = "https://files.pythonhosted.org/packages/75/d3/e1118c8f4870f891ca00d098d13826f5d63363dbac307116d8e920dd4596/zeroconf-0.66.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:44c4990e9e766b23cab86dc7fa0c2191604290b09c07b8cd9326d2ef3abe9415"},
-    {url = "https://files.pythonhosted.org/packages/80/54/59812395d7caa08235b1a47673f4e504b90d3e465be2ebf4a100a7671363/zeroconf-0.66.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:54a6aeec0c0ca680ddc7b3367cd6b070de3c87082f052f16a5cae91be3ecaab1"},
-    {url = "https://files.pythonhosted.org/packages/80/f6/0538e24d8eceb80c53bb8cbe9fa046afca2924e6b9bc9696ac4b35941d48/zeroconf-0.66.0-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:776be3098fc1e361288905a4ea05379c51dad166f049327b524d5cb98bace0c0"},
-    {url = "https://files.pythonhosted.org/packages/90/48/582ae01ea5ab8ece075d1c01acc2bcff06ff9d5fd8274f1b95ca489c1ec3/zeroconf-0.66.0-cp311-cp311-win_amd64.whl", hash = "sha256:1fec47c1d8dd84aa61196d081b32752a42d19bd78ed3b3cced5478305fa5bcb6"},
-    {url = "https://files.pythonhosted.org/packages/90/a6/fd0d52ac6fed8434157659d6c61db508e8f0c2bd1054c61434166f535a2b/zeroconf-0.66.0-cp311-cp311-win32.whl", hash = "sha256:04d12703423aea6546511bce9747cad2e3eaec7a47a4f7188ce6c67f204098ce"},
-    {url = "https://files.pythonhosted.org/packages/97/27/d0362dba626c6abe9f767a6c7e68722b383b5dc6ac04f08202fac7ef8290/zeroconf-0.66.0-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:4b211886b0a5cbef7c7f9d15d1492e9f323de0fb7e8c750cd86224002a2efc55"},
-    {url = "https://files.pythonhosted.org/packages/a6/08/59a7af0c3527d070b060c71624089c4bb0f2b6c0def24aed912be572d584/zeroconf-0.66.0-cp38-cp38-win_amd64.whl", hash = "sha256:5fe741398486564b5c457c77d9167591e59034cdee85dd7a40531e80b97cb7ee"},
-    {url = "https://files.pythonhosted.org/packages/a6/8c/fcbbb3558425d84e240ea79bdde28d0fd5cc755cd6820654691082d728ef/zeroconf-0.66.0-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:2c55b7acd4a23133484eeb9814de1e281981b0389f7268ba6fcdedf199362820"},
-    {url = "https://files.pythonhosted.org/packages/ae/8e/af12216a116049091b4348d3a60980be498af81d31e59bb9d9eb872b5794/zeroconf-0.66.0-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:b15ff89c605da12c245cd89fe8b0b7db7b054566b97c58eceaa13bafcc18ad96"},
-    {url = "https://files.pythonhosted.org/packages/af/7d/50704d3a4558b70c101382e776627d77bee4e8c62d49574b600137563795/zeroconf-0.66.0-pp38-pypy38_pp73-macosx_11_0_x86_64.whl", hash = "sha256:ca6520bd128f7fdb043f909b50fcdc2666ac8968ef22ef9f5f77d326ebeab3ad"},
-    {url = "https://files.pythonhosted.org/packages/b0/bf/c8a0b0f970bd704a764874a644f12d75923e2433b2f4abbff2e020cdae1a/zeroconf-0.66.0-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:ce399141063a517ffef3c6504d36ae203828e26c35e39a3bc2948c9230fd1b71"},
-    {url = "https://files.pythonhosted.org/packages/b3/dd/34e5a4271e7ce5ab03b77e97ecbaf7c7aa184f40471340b19cc4557b37b6/zeroconf-0.66.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:2d42cd53da6cfa5a4c89ed89621c0faa6b28718db6f290464ac83ee9f33a49ea"},
-    {url = "https://files.pythonhosted.org/packages/b6/62/e66769e70ab3f46e8a803632bdffe613bc9cd0e2a645b5f98dfbf5d81e1c/zeroconf-0.66.0-cp39-cp39-win_amd64.whl", hash = "sha256:eaddcd38486b47137257ee80bd943d66f2ce6c36a431ff229e3d3bcc12dd2d62"},
-    {url = "https://files.pythonhosted.org/packages/be/b5/cb7238b69aed8b40d0963d767adce50c1c0d053b947dd174246aae69ce37/zeroconf-0.66.0-cp310-cp310-win_amd64.whl", hash = "sha256:64cdce0750a6d18b8dde9ee1401724e3165f31a3a58d898e06dea8e618edd67f"},
-    {url = "https://files.pythonhosted.org/packages/c1/4c/a2cd16cc98456df8684f00e8780640bd923bcc35e37a27123716704431be/zeroconf-0.66.0-cp311-cp311-macosx_11_0_x86_64.whl", hash = "sha256:91e3e0264b040578e4895fe090fed3782f2a7f67857548b82ad9fdf2c8e59fed"},
-    {url = "https://files.pythonhosted.org/packages/c6/17/e2e852ad98eb69f1477e6795b003994b4cccd99fafcf349119716545ab8e/zeroconf-0.66.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8eaea03f9ee65a69035716070644d40548f66dfc333403f92c4e4fd43b5704c6"},
-    {url = "https://files.pythonhosted.org/packages/cb/a7/f0fcb5112326846649e6a64a39799a6ab238f180989996674889a069d41e/zeroconf-0.66.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:1396389b9fd2cc7da570eae1068dfbbeb93508c1e913b6b09096eccbc4dafa44"},
-    {url = "https://files.pythonhosted.org/packages/cc/04/fd4ee7486bffb82ea0797845658ed88b5631d94456c9dd914deabc386369/zeroconf-0.66.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:2c27c45486de5094925d9a8a48e647854396995e74e9819513b0e2159f71de1b"},
-    {url = "https://files.pythonhosted.org/packages/cd/d7/49f2bd9326a14c0c63675753674c88578f2a68b3bb9d5ac40632f3b79e29/zeroconf-0.66.0-pp39-pypy39_pp73-macosx_11_0_x86_64.whl", hash = "sha256:cfe90abdd093b859ee344a94866f1b3c2c9dc054f7473745fb190b14083a70b1"},
-    {url = "https://files.pythonhosted.org/packages/ce/8a/bc01e9856ba197453c54c26e4dae851cfbccd4e574b1395118af25bc3552/zeroconf-0.66.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:56962db72a9439645c956979e9fcf00fd391ee8b769180284a87be3e906fef20"},
-    {url = "https://files.pythonhosted.org/packages/d2/49/e5158404daf23899e99d72c4a1ec88879b3af467a9f616c946443778c91d/zeroconf-0.66.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8f4d43cdbf4a108e1e0727f12bf7a2222dec0ab0566197bbeb504d0f1e53447f"},
-    {url = "https://files.pythonhosted.org/packages/db/d6/6a17c10fd09de8a45747cb0dd85ef04d76e948d9454c0ddb58e7fb72fddb/zeroconf-0.66.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:be5687c8a4834b8b343676793ba269831d34f69cbaae0adcacc881559d940e5a"},
-    {url = "https://files.pythonhosted.org/packages/e2/77/1bde47d1d9dd0dddc64cc5a7ec7e299f0e203d6ec478c058735a98b635c1/zeroconf-0.66.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c182cac6633d517a11c06ab3b04b5d3d2bea356de81d5f57273d78cfa1aa04b9"},
-    {url = "https://files.pythonhosted.org/packages/e3/01/0f04de804ae2469b1a165cdf01e40fe099158869d6defd8a699d1bb4d81e/zeroconf-0.66.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:829478a8dee2fea754e2c8fd54b28462d61b016945aba94c3b51b984d18209dc"},
-    {url = "https://files.pythonhosted.org/packages/e5/ac/7f6fb7143b04014f0f6ca5a99b35a4bdc189e5514e5221f2a904acdd3431/zeroconf-0.66.0-cp311-cp311-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:c12e38b2ccfaaebfe4a1516a1e97647872e7b5193d3711be014c982da5768121"},
-    {url = "https://files.pythonhosted.org/packages/e9/95/4593816ab58f8a90dee06f96c32c2cd7d1b5d71d9511d3a86cac6e77de94/zeroconf-0.66.0-cp37-cp37m-win_amd64.whl", hash = "sha256:b65dceae6fcaeb95f1fd7b3e348a6b795a85fc2d15a16b72104e366915b062e1"},
-    {url = "https://files.pythonhosted.org/packages/e9/e1/b278980b921f98cdb7072c522e9f030b6801ca279fbf16089c69fe9d894b/zeroconf-0.66.0-cp38-cp38-macosx_11_0_x86_64.whl", hash = "sha256:555660a7dc720ae92c0f409447200cb751e90353bfe7717aedf8114ec19b053e"},
-    {url = "https://files.pythonhosted.org/packages/ee/ed/b2e08281b95e008e288216bb4a13d5a9c4321dd1d5d7a13cadb7d9a3ea61/zeroconf-0.66.0-cp38-cp38-win32.whl", hash = "sha256:57a1c0c2681bb86e2be3200480149429545df5d477c5b702ecc0b140cdc01a8e"},
-    {url = "https://files.pythonhosted.org/packages/ef/a9/d952f9805084d504f8ada522bdb6535a17b06e667cb3923623686ed4f59a/zeroconf-0.66.0-pp37-pypy37_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:10ad59230f826cc37500dffb54aba82a70d22afa6f25b2ff7a44e9e020517eca"},
-    {url = "https://files.pythonhosted.org/packages/f5/24/7b37c243ad7b6bd83f74c6e9efe8db915a80abcc50926792337d0c3c6960/zeroconf-0.66.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:9939600589a9fbfb00e5a90bdf8b3ece45029147e2e99eafe641d5f1d83fb0d9"},
+"zeroconf 0.69.0" = [
+    {url = "https://files.pythonhosted.org/packages/04/f9/b89ba913563eca7ad5cf80d066d14df68c8a1614731b07a5cc238c7680cb/zeroconf-0.69.0-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:9e2cfe4baa6540e21cbb74d820a1bf8f3258449bee92be1cba289033fe77f0c9"},
+    {url = "https://files.pythonhosted.org/packages/0b/30/0d5cb2bf0a29e844748c039d7ceb13008a376e2af95c6b51f4a8754ed494/zeroconf-0.69.0-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:ff92c07ff69156cb496d001700afd06959c37b80731c78c5ce896f4f3aebfe21"},
+    {url = "https://files.pythonhosted.org/packages/0b/31/516fd6b8512190e94896ece6c37f9be244611ea2c64877a3ea0227ef532d/zeroconf-0.69.0-cp311-cp311-macosx_11_0_x86_64.whl", hash = "sha256:1dea30128d618a46d489809a55a932a5797c353b5d9a3dc5ed63d5d5887a7e97"},
+    {url = "https://files.pythonhosted.org/packages/0b/5a/03a16379942dd478099eddc92316e4b1be37928797fa12ed592353360482/zeroconf-0.69.0-cp39-cp39-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:0a7a34989a88eacd4948e8a04c5b9ed5757df8684a09fb85e8f3d374b57903e5"},
+    {url = "https://files.pythonhosted.org/packages/15/72/34dbc01948cf279175f4d042405caefeb90e720cfcb9988b370ca8dee052/zeroconf-0.69.0-cp37-cp37m-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:d1d543bc558e526ae217848c508c737d74be678712ebd226fc3d8335762b807f"},
+    {url = "https://files.pythonhosted.org/packages/1b/00/7caa74735c5458ae4c8c3c8b25e49b35ba66fbbafaf6087a6b09bd6a99fb/zeroconf-0.69.0-cp310-cp310-win_amd64.whl", hash = "sha256:2f139ee88d6c1d874546d042cc024b9db4a58658c856edd2c5685adb9a7b19d2"},
+    {url = "https://files.pythonhosted.org/packages/1e/42/f98be8565e895f12a3dfb69c158f80098aae179aae734e9d57a7606f799d/zeroconf-0.69.0-cp38-cp38-macosx_11_0_x86_64.whl", hash = "sha256:95d6896d7b90acd209be6f57cbabfa66893bb7a2dcd94de64b7e9933f26bba67"},
+    {url = "https://files.pythonhosted.org/packages/23/e1/fea9a99847a3a1ad96ce32906694682edbed85e600f2a103fd0f24f294fb/zeroconf-0.69.0-cp39-cp39-win32.whl", hash = "sha256:c9fd5f6c76b98fc822824a0e5b25b120a240a9382174002bca1224ff70b474dc"},
+    {url = "https://files.pythonhosted.org/packages/2a/11/4b2d14fe946ee5013d458295cf8f0983b3f1b6f593ada58f121959af3037/zeroconf-0.69.0-cp37-cp37m-win_amd64.whl", hash = "sha256:efb9ad9b6bf4681ea600bfa6dbd8f1ffea849c61238deeb9baacf8fee5c3226e"},
+    {url = "https://files.pythonhosted.org/packages/2a/90/3e742b51e64eaeef88eac47b75e33dbb320da12493b0ef9a8ee6dca8fa1e/zeroconf-0.69.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:33725a8b22f6e4ac93083168da4954aae9d84dfbb0e2675ae4db8e3d477b0d30"},
+    {url = "https://files.pythonhosted.org/packages/2c/aa/574ba28275cbcca990f3e8ef0017dc07a815770fda10303c71b6729fe6aa/zeroconf-0.69.0-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:9e4ec38105bcf61da91e4f8bbd0eac7175ea158f3d4aad7d72da5fd577aeda1a"},
+    {url = "https://files.pythonhosted.org/packages/2f/ea/42731cefb800697e57e2021990cecff77d3fc942e5900fb2a382fe1e78a1/zeroconf-0.69.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:4b24c3b19c8170f75b7280c0f3297d1afbe3fb66dc0f9ca1217eb05147472ff6"},
+    {url = "https://files.pythonhosted.org/packages/30/cb/da2dbd380684c8a15457bfc7a4012c54de86cd0dcda4e23fb59effe7ca0c/zeroconf-0.69.0-cp38-cp38-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:78ab98603a38f77dd1925163d75dabb201db9ccd01be2505bfedf9f31bdcd137"},
+    {url = "https://files.pythonhosted.org/packages/3b/b7/d046c27d8d8c3877c67ddac9cc6a3d702a9b9495ab0acfd84d9a3b0d0de1/zeroconf-0.69.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3ff3dfc001a0873bf5b7a671efe79f8d251ad8ca0ab6189870cba0f6d2ecba9c"},
+    {url = "https://files.pythonhosted.org/packages/3d/b3/0f0a08f0c176b9ffa0359c7a8682dc0b2f766cd2dbb237d4ade84daa4439/zeroconf-0.69.0-cp310-cp310-manylinux_2_31_x86_64.whl", hash = "sha256:9df3f88e71588f28ab5410e574621b4eb3f4bf63876f6382ed4a966accb76e0c"},
+    {url = "https://files.pythonhosted.org/packages/3f/9b/8426c230ecdb0f88e92d19b7f2d724d918e87d049ffd02a580a57dd67567/zeroconf-0.69.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:a010ffaa4f318466b194c5bf97d857d48fd17fe09ccaa2c8eb48227f0e09592c"},
+    {url = "https://files.pythonhosted.org/packages/3f/be/fa304116a29c6645a33e74a77cefa2b126bce9d95666b5a03eb9cdf49c87/zeroconf-0.69.0-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e477cd1b71327293f2eb32db128f90e636f6ce27d37ca871bdfa4ab65a793347"},
+    {url = "https://files.pythonhosted.org/packages/41/3e/4c2c7b5df82181c42851534a9fd849738f770b95284ad26cf9c4fb9d8a4d/zeroconf-0.69.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d2d99b115f00dd8217ee7b233d66a90697c941dd5ab240917a778b97edf3e68c"},
+    {url = "https://files.pythonhosted.org/packages/46/78/d26a6794e4486f84721d03a0193f3fcb0fa77cb18e8a6271ade574f562f7/zeroconf-0.69.0-pp37-pypy37_pp73-macosx_11_0_x86_64.whl", hash = "sha256:921d4a1c5ad5745acd51bb87ecdcf2e0c7e1174876d688e44512a4631674ea1b"},
+    {url = "https://files.pythonhosted.org/packages/4a/82/5a08900b2c80b8f00c72bc1669694ea0eeb0dbb61ca97dd72ee46c9f312d/zeroconf-0.69.0-cp37-cp37m-win32.whl", hash = "sha256:a63501b614dd426ef7d7249d26517369f6094bb9e928ee3f75a623fa663569c4"},
+    {url = "https://files.pythonhosted.org/packages/4e/42/9478ee1b25e0f7971042d92428113278cee43da8de4fb7b20c47be417f8e/zeroconf-0.69.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:5097cbb812bf488cda700c1ceaa91bcb9d7d9098fccbc9f60f19b64d52fccd35"},
+    {url = "https://files.pythonhosted.org/packages/4f/15/c363f449810b2eed14f4bb2020af589ccb089f21952bf8c81a6d41b9b099/zeroconf-0.69.0-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:ae7dfe470eaf38c3df6daf3a508fcf3a7daa445e6ebedc569320f05bdb7e08f1"},
+    {url = "https://files.pythonhosted.org/packages/50/63/54b069bb874dfcaa5c523671b474dc899c13167e8a6f86ea670fb92d0a76/zeroconf-0.69.0-pp37-pypy37_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:1ab65dcd3aea834ddac1ba27806983ca3cab9f8db87ea6923130d30bdbfbcd68"},
+    {url = "https://files.pythonhosted.org/packages/5b/b9/c2042c7ed9927a2de5d9f3dbd637eeff73a490cb7ad7a9d6dfd434ee8244/zeroconf-0.69.0-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:5df7d15461859dcec0bfca9e8f120ae46e284fe2071d8f654d65635a03a04542"},
+    {url = "https://files.pythonhosted.org/packages/5c/8c/9153299f2abaf3348f258de3bd4a83f854e0432456ec8de4a45b7ac9bad9/zeroconf-0.69.0-pp39-pypy39_pp73-macosx_11_0_x86_64.whl", hash = "sha256:bd60de9c364d5ecd2182b35432d50fe243f6de392fd52126855e06310217c676"},
+    {url = "https://files.pythonhosted.org/packages/68/70/accdd21e9730df1fd5e05805580ee0d65b901d04644f8f16b05ef5c11bad/zeroconf-0.69.0-cp37-cp37m-macosx_11_0_x86_64.whl", hash = "sha256:6b165bc4d101a5369c56cf31e07241a991a08432ebc235e662ee105acf814a59"},
+    {url = "https://files.pythonhosted.org/packages/6d/b3/1288ce4c7069e344cc6825dd896b4c0fe5e7950aff9ea98415275a302d15/zeroconf-0.69.0.tar.gz", hash = "sha256:c6520f39f718e6bd16a87e0a7711ff65acfbb11bbc9fabb6283506833e0c3c0f"},
+    {url = "https://files.pythonhosted.org/packages/6f/69/392b364c8ef243b7efc29c12b7b51df5bdae80de204e66fe0d561416f849/zeroconf-0.69.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ffd1c97a7f479717af6880b5684582eab4f38a1a69a6a6b89803eaac3d0baecb"},
+    {url = "https://files.pythonhosted.org/packages/74/3f/a9087e451ca85b361851042616958aff1da69c31a878ae525a866422b51b/zeroconf-0.69.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:55951cd11cd34b3dda2d24589bbf7f53c51ce5c5be0769ebbdd00eca5f73a6d2"},
+    {url = "https://files.pythonhosted.org/packages/75/b5/a60a895f60e1ca19968ad8c2b102c189741050de53b624927d74fd4b9c79/zeroconf-0.69.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:a3cd0163e166dad9b000f84f319eccfd801ef75f0a3594dfb29078f672dfe14f"},
+    {url = "https://files.pythonhosted.org/packages/76/51/1fe35c29b5b002a8a58d16084fcbde7fb747a4e109c46bc79a551f491cb4/zeroconf-0.69.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:356f60aa84c8ce22104f986ee72953e9a133d0de4096db4a2d96e9409ff6e9bb"},
+    {url = "https://files.pythonhosted.org/packages/94/a2/646555f9847c83f2cf36cbc56e715812cff4da7bd11bbf2ff8d3da96a96c/zeroconf-0.69.0-cp39-cp39-win_amd64.whl", hash = "sha256:8df09bf5236cf8719d9204f81865d1d0783a0b735f325a766a2d18be81a58102"},
+    {url = "https://files.pythonhosted.org/packages/a7/d2/257a10be23d6f7a7264a561f9929768300c74ed16d347018ccd3255256ab/zeroconf-0.69.0-cp311-cp311-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:d38a85219f79b548c4bb0ee80576e64852a01e0070cfb8c80d3dcb9e952caa1d"},
+    {url = "https://files.pythonhosted.org/packages/af/a2/fcc4cb25dd8ea83f2103e559835377d10683166c073f85fbf65a03db14e2/zeroconf-0.69.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:13003192f4f862de250f1cd2ffc558cd0d01b087933ed2800a3d39f3229e0aba"},
+    {url = "https://files.pythonhosted.org/packages/b2/9e/d84945cfdd63cd4a61a323c75485462f77de6dd6a830126d4112d9b4ba1c/zeroconf-0.69.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:6d3fe233ea66cbb5c41cc5a63e6a6427b2dfc272d1b503fb92619ceaa0ceb6f1"},
+    {url = "https://files.pythonhosted.org/packages/b5/76/483634d98980980ce70eb38217700adeec90be7a92499c96407aa6a3d3db/zeroconf-0.69.0-pp38-pypy38_pp73-macosx_11_0_x86_64.whl", hash = "sha256:3d2080eaed841e20007790742ba0d6cb4c1b6f4499afdca889c2bfb562f4da98"},
+    {url = "https://files.pythonhosted.org/packages/c6/9b/61c47925f3ca395765d411b46f4ccd8d9a6c7304dad48e99554f33d4a241/zeroconf-0.69.0-cp311-cp311-win_amd64.whl", hash = "sha256:4b8c148db654937bb3991e507a8c1337d624e95681124de201bf15737f308809"},
+    {url = "https://files.pythonhosted.org/packages/c6/f9/1ad7c8af17df8dd6058890643c2fbd92c51bda206b9edfd16fdafc5ccedc/zeroconf-0.69.0-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:1687e0e6d176d7c0ce9780697393bf0e093182a15f4743f4315267fb751af5d2"},
+    {url = "https://files.pythonhosted.org/packages/cd/5d/b83da029c490ce9ad4d4b9dafec19d045f5759b636f3aaeb084acd0830c1/zeroconf-0.69.0-cp310-cp310-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:c05eb8a137a6d0b4fefdb3784677c3d430a77c9a3b43f286e788eaff24347ec4"},
+    {url = "https://files.pythonhosted.org/packages/d2/17/e4da18a6d3869308ec67c6256015d7df896fa5a758fe30f27cd657b48712/zeroconf-0.69.0-cp38-cp38-win_amd64.whl", hash = "sha256:9c723f1903a995568d0a930687dce15985d17cda4932d97102f302653f7262f3"},
+    {url = "https://files.pythonhosted.org/packages/d4/4c/58ae63c8f41f2087d52f267e394ed893c64409c428a2e8f8f4664b0daa1a/zeroconf-0.69.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:f1d2b4518bf1cc6c62e8a1d005ecc310fe949b68ec2b16376d75e5f1502de5de"},
+    {url = "https://files.pythonhosted.org/packages/da/d6/e41181c4eafaf2b65eae2ed14792ed209de229c5969a500abbaa243515be/zeroconf-0.69.0-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:73a3aba23ee947b0b217c8abec448cc53a55a845b9c68c7699d8f3e0ee090f72"},
+    {url = "https://files.pythonhosted.org/packages/e2/12/6f75a8672d359dc30b6bff66eb2c173a7a17942fbaa890859862275fb138/zeroconf-0.69.0-cp38-cp38-win32.whl", hash = "sha256:4321ffd7de54eed4be5c8a36d460b566717c4a5600fe9133eb72bae18b2d3a2c"},
+    {url = "https://files.pythonhosted.org/packages/e8/8b/25e5241a66f6081fe6f236a58d5dc2c7bc56066e7e6d1c07c659101bc5b8/zeroconf-0.69.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:77cb728f2a88b217ac423b83d05ff9a0b452148cf9779453188d9ef31f6fcafb"},
+    {url = "https://files.pythonhosted.org/packages/eb/13/9ca288f0fe10f1c8e9fa21b47d99c43fc862eef4216830e05e6b253d744a/zeroconf-0.69.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ae80834676c9c77b9043e0f3572b1f480bf265d4f63b96e5cefaba07cb35f947"},
+    {url = "https://files.pythonhosted.org/packages/eb/5f/93d9a48d8c7362b0367608a3ea04917ff574a95fda690e38cbcc0a7c11f2/zeroconf-0.69.0-cp310-cp310-win32.whl", hash = "sha256:6560b1f1dc595f799a5ffb68c54d71f9dbe76cc5bc01e66cb2de4b4a9f898fe3"},
+    {url = "https://files.pythonhosted.org/packages/f0/0d/de0e72d870e89307993fcba8d0da9fc05373c958ef03c75da5cb5b20d0db/zeroconf-0.69.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:85b927548b636683144b9696a81961c1109b7dc66f6fc473564be3ca831df13a"},
+    {url = "https://files.pythonhosted.org/packages/f0/eb/a18c82cdc00b5a1ea9b22fb49f396576f21a2fbf18873eaa413e815e463a/zeroconf-0.69.0-cp311-cp311-win32.whl", hash = "sha256:7773814b57846996d8a660dd180ff5c1fcf9da00a710f16f6429aa77fe5b14a4"},
+    {url = "https://files.pythonhosted.org/packages/fd/0b/0db30dde1573132a308a992db412c2ed232b3ede90affc6f7f99f75073d2/zeroconf-0.69.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:822235895234fe0bdbad8264989e200fdb4200b806be4cd699797630dee166e7"},
 ]
 "zipp 3.15.0" = [
     {url = "https://files.pythonhosted.org/packages/00/27/f0ac6b846684cecce1ee93d32450c45ab607f65c2e0255f0092032d91f07/zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
     {url = "https://files.pythonhosted.org/packages/5b/fa/c9e82bbe1af6266adf08afb563905eb87cab83fde00a0a08963510621047/zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
 ]
```

### Comparing `xklb-1.31.9/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-2.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-2.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/.github/workflows/push.yaml` & `xklb-2.1.2/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/av.py` & `xklb-2.1.2/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/books.py` & `xklb-2.1.2/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/consts.py` & `xklb-2.1.2/xklb/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,16 @@
     "time_scanned",
     "time_downloaded",
     "time_deleted",
     "time_modified",
     "time_created",
     "time_played",
     "time_valid",
-    "time_partial_first",
-    "time_partial_last",
+    "time_first_played",
+    "time_last_played",
     "playhead",
 )
 
 
 class DBType:
     audio = "audio"
     video = "video"
@@ -170,26 +170,26 @@
     if speech_recognition:
         extensions.extend(SPEECH_RECOGNITION_EXTENSIONS)
 
     return get_files(path, extensions)
 
 
 time_facets = [
-    "all",
     "watching",
     "watched",
     "deleted",
     "created",
     "modified",
     "downloaded",
 ]
 
 frequency = ["daily", "weekly", "monthly", "quarterly", "yearly"]
 
 PLAYLIST_KNOWN_KEYS = (
+    "description",
     "url",
     "duration",
     "view_count",
     "webpage_url",
     "original_url",
 )
```

### Comparing `xklb-1.31.9/xklb/db.py` & `xklb-2.1.2/xklb/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,27 +65,31 @@
         db.conn.execute("PRAGMA main.cache_size = 8000")  # type: ignore
 
     db.enable_wal()
     return db
 
 
 def columns(args, table_name):
-    return args.db[table_name].columns_dict
+    try:
+        return args.db[table_name].columns_dict
+    except Exception:
+        return {}
 
 
 config = {
     "playlists": {
         "column_order": ["path", "extractor_key"],
         "ignore_columns": ["id", "extractor_playlist_id"],
     },
     "media": {
         "search_columns": ["path", "title", "mood", "genre", "description", "artist", "album"],
         "column_order": ["path", "webpath", "extractor_id"],
         "ignore_columns": ["id", "extractor_id"],
     },
+    "history": {"ignore_columns": ["id"]},
     "captions": {"search_columns": ["text"]},
     "reddit_posts": {
         "search_columns": ["title", "selftext"],
         "column_order": ["path"],
     },
     "reddit_comments": {
         "search_columns": ["body"],
```

### Comparing `xklb-1.31.9/xklb/dl_config.py` & `xklb-2.1.2/xklb/dl_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 .*Origin Error
 .*API is not granting access
 .*Did not get any data blocks
 .*Too Many Requests
 .*Postprocessing
 .*Premieres in
 .*user.*not allowed
+.*Upgrade now
 .*read operation timed out
 .*Could not connect
 .*restricted
 .*Internal Server Error
 .*Internal error encountered
 .*not currently available
 .*currently unavailable
```

### Comparing `xklb-1.31.9/xklb/dl_extract.py` & `xklb-2.1.2/xklb/dl_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,15 @@
                 {', m.duration' if 'duration' in m_columns else ''}
                 {', m.time_created' if 'time_created' in m_columns else ''}
                 {', m.size' if 'size' in m_columns else ''}
                 {', m.time_modified' if 'time_modified' in m_columns else ''}
                 {', m.time_downloaded' if 'time_downloaded' in m_columns else ''}
                 {', m.time_deleted' if 'time_deleted' in m_columns else ''}
                 {', m.error' if 'error' in m_columns else ''}
+                , 'Playlist-less media' as extractor_key
             FROM media m
             WHERE 1=1
                 {'and COALESCE(m.time_downloaded,0) = 0' if 'time_downloaded' in m_columns else ''}
                 {'and COALESCE(m.time_deleted,0) = 0' if 'time_deleted' in m_columns else ''}
                 and m.path like "http%"
                 {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
                 {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
@@ -200,20 +201,20 @@
         """
 
     return query, args.filter_bindings
 
 
 def process_downloadqueue(args) -> List[dict]:
     if args.playlist_files:
-        known_playlists = set()
-        if not args.force:
-            known_playlists = get_paths(args)
-
         Path(args.database).touch()
         playlist_files_data = set(utils.flatten(Path(p).read_text().splitlines() for p in args.playlists))
+
+        known_playlists = set()
+        if not args.force and len(playlist_files_data) > 9:
+            known_playlists = get_paths(args)
         playlists = list(playlist_files_data - known_playlists)
         log.warning(
             "%s new - %s known = %s to download",
             len(playlist_files_data),
             len(known_playlists),
             len(playlists),
         )
```

### Comparing `xklb-1.31.9/xklb/fs_extract.py` & `xklb-2.1.2/xklb/fs_extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,23 +117,14 @@
     if args.profile in (DBType.audio, DBType.video) and not which("ffprobe"):
         log.error("ffmpeg is not installed. Install it with your package manager.")
         raise SystemExit(3)
 
     return args
 
 
-def calculate_sparseness(stat) -> int:
-    if stat.st_size == 0:
-        sparseness = 0
-    else:
-        blocks_allocated = stat.st_blocks * 512
-        sparseness = blocks_allocated / stat.st_size
-    return sparseness
-
-
 def extract_metadata(mp_args, path) -> Optional[Dict[str, int]]:
     log.debug(path)
 
     try:
         stat = Path(path).stat()
     except FileNotFoundError:
         return None
@@ -142,27 +133,21 @@
         return None
     except Exception as e:
         log.error(f"[{path}] %s", e)
         return None
 
     media = {
         "path": path,
-        "play_count": 0,
-        "time_played": 0,
-        "playhead": 0,
         "size": stat.st_size,
         "time_created": int(stat.st_ctime),
         "time_modified": int(stat.st_mtime) or consts.now(),
         "time_downloaded": consts.APPLICATION_START,
         "time_deleted": 0,
     }
 
-    if hasattr(stat, "st_blocks"):
-        media = {**media, "sparseness": calculate_sparseness(stat)}
-
     if mp_args.profile == DBType.filesystem:
         media = {**media, "is_dir": Path(path).is_dir()}
 
     if mp_args.profile in (DBType.audio, DBType.video):
         media = av.munge_av_tags(mp_args, media, path)
 
     if mp_args.profile == DBType.text:
@@ -326,15 +311,15 @@
     threadsafe = [DBType.audio, DBType.video, DBType.filesystem]
 
     info = {
         "extractor_key": "Local",
         "extractor_config": utils.filter_namespace(args, ["ocr", "speech_recognition", "scan_subtitles"]),
         "time_deleted": 0,
     }
-    args.playlist_id = playlists.add(args, str(path), info)
+    args.playlist_id = playlists.add(args, str(path), info, check_subpath=True)
 
     print(f"[{path}] Building file list...")
     new_files = find_new_files(args, path)
     if new_files:
         print(f"[{path}] Adding {len(new_files)} new media")
         log.debug(new_files)
 
@@ -403,13 +388,13 @@
                 length(path)-length(REPLACE(path, '/', '')) desc
                 , path
             """,
         ),
     )
 
     for playlist in fs_playlists:
-        extractor_config = json.loads((playlist.get("extractor_config") or "{}"))
+        extractor_config = json.loads(playlist.get("extractor_config") or "{}")
         args_env = argparse.Namespace(
             **{**extractor_config, **args.__dict__, "profile": playlist["profile"]},
         )
 
         extractor(args_env, [playlist["path"]])
```

### Comparing `xklb-1.31.9/xklb/gdl_backend.py` & `xklb-2.1.2/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/gdl_extract.py` & `xklb-2.1.2/xklb/gdl_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         default={},
         metavar="KEY=VALUE",
         help="Add key/value pairs to override or extend default downloader configuration",
     )
     parser.add_argument("--download-archive", default="~/.local/share/gallerydl.sqlite3")
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
     parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
-    parser.add_argument("--playlist-files", action="store_true", help="Read playlists from text files")
     parser.add_argument(
         "--force",
         "-f",
         action="store_true",
         help="Fetch metadata for paths even if they are already in the media table",
     )
     parser.add_argument("--extra-media-data", default={}, nargs=1, action=utils.ArgparseDict, metavar="KEY=VALUE")
@@ -38,14 +37,15 @@
 
     parser.add_argument("--timeout", "-T", help="Quit after x minutes")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
     if action == SC.galleryadd:
+        parser.add_argument("--playlist-files", action="store_true", help="Read playlists from text files")
         parser.add_argument("playlists", nargs="+", help=argparse.SUPPRESS)
 
     args = parser.parse_args()
     args.action = action
 
     if args.db:
         args.database = args.db
@@ -71,15 +71,15 @@
         sys.argv = ["galleryadd", *args]
 
     args = parse_args(SC.galleryadd, usage=usage.galleryadd)
     if args.playlist_files:
         args.playlists = list(utils.flatten([Path(p).read_text().splitlines() for p in args.playlists]))
 
     known_playlists = set()
-    if not args.force:
+    if not args.force and len(args.playlists) > 9:
         known_playlists = media.get_paths(args)
 
     added_media_count = 0
     for path in args.playlists:
         if path in known_playlists:
             log.info("[%s]: Already added. Skipping!", path)
             continue
```

### Comparing `xklb-1.31.9/xklb/gui.py` & `xklb-2.1.2/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/hn_extract.py` & `xklb-2.1.2/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/lb.py` & `xklb-2.1.2/xklb/lb.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,33 +3,34 @@
 from xklb import __version__, utils
 from xklb.consts import SC
 from xklb.dl_extract import dl_download
 from xklb.fs_extract import fs_add, fs_update
 from xklb.gdl_extract import gallery_add, gallery_update
 from xklb.hn_extract import hacker_news_add
 from xklb.play_actions import filesystem, listen, read, view, watch
-from xklb.playback import playback_next, playback_now, playback_pause, playback_stop
 from xklb.praw_extract import reddit_add, reddit_update
 from xklb.scripts.bigdirs import bigdirs
 from xklb.scripts.block import block
 from xklb.scripts.christen import christen
 from xklb.scripts.cluster_sort import cluster_sort
 from xklb.scripts.copy_play_counts import copy_play_counts
 from xklb.scripts.dedupe import dedupe
 from xklb.scripts.dedupe_db import dedupe_db
 from xklb.scripts.download_status import download_status
 from xklb.scripts.history import history
 from xklb.scripts.merge_dbs import merge_dbs
 from xklb.scripts.merge_online_local import merge_online_local
 from xklb.scripts.mining.extract_links import extract_links
+from xklb.scripts.mining.mpv_watchlater import mpv_watchlater
 from xklb.scripts.mining.nouns import nouns
 from xklb.scripts.mining.pushshift import pushshift_extract
 from xklb.scripts.mining.reddit_selftext import reddit_selftext
 from xklb.scripts.move_list import move_list
 from xklb.scripts.optimize_db import optimize_db
+from xklb.scripts.playback_control import playback_next, playback_now, playback_pause, playback_stop
 from xklb.scripts.playlists import playlists
 from xklb.scripts.redownload import redownload
 from xklb.scripts.relmv import relmv
 from xklb.scripts.scatter import scatter
 from xklb.scripts.streaming_tab_loader import streaming_tab_loader
 from xklb.search import search
 from xklb.tabs_actions import tabs
@@ -99,14 +100,16 @@
     mining:
       lb reddit-selftext       db selftext external links -> db media table
       lb pushshift             Convert Pushshift jsonl.zstd -> reddit.db format (stdin)
       lb hnadd                 Create a hackernews database (this takes a few days)
 
       lb extract-links         Extract links from lists of web pages
 
+      lb mpv-watchlater        Import timestamps from mpv watchlater to history table
+
       lb cluster-sort          Lines -> sorted by sentence similarity groups (stdin)
       lb nouns                 Unstructured text -> compound nouns (stdin)
     """
 
 
 def print_help(parser) -> None:
     print(usage())
@@ -238,14 +241,17 @@
     subp_surf.set_defaults(func=streaming_tab_loader)
 
     subp_nouns = add_parser(subparsers, "nouns")
     subp_nouns.set_defaults(func=nouns)
     subp_cluster_sort = add_parser(subparsers, "cluster-sort", ["cs", "clustersort", "cluster_sort"])
     subp_cluster_sort.set_defaults(func=cluster_sort)
 
+    subp_mpv_watchlater = add_parser(subparsers, "mpv-watchlater")
+    subp_mpv_watchlater.set_defaults(func=mpv_watchlater)
+
     subp_reddit_selftext = add_parser(subparsers, "reddit-selftext")
     subp_reddit_selftext.set_defaults(func=reddit_selftext)
     subp_nfb_directors = add_parser(subparsers, "extract-links", ["links"])
     subp_nfb_directors.set_defaults(func=extract_links)
 
     parser.add_argument("--version", "-V", action="store_true")
     return parser
```

### Comparing `xklb-1.31.9/xklb/media.py` & `xklb-2.1.2/xklb/media.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,34 +27,35 @@
 
 def get(args, path):
     return args.db.pop_dict("select * from media where path = ?", path)
 
 
 def get_paths(args):
     tables = args.db.table_names()
+
     known_playlists = set()
     if "media" in tables:
         known_playlists.update(d["path"] for d in args.db.query("SELECT path from media"))
+
+        m_columns = db.columns(args, "media")
+        if "webpath" in m_columns:
+            known_playlists.update(d["webpath"] for d in args.db.query("SELECT webpath from media"))
+
     if "playlists" in tables:
         known_playlists.update(d["path"] for d in args.db.query("SELECT path from playlists"))
+
     return known_playlists
 
 
 def consolidate(v: dict) -> Optional[dict]:
-    v = {
-        **(v.pop("photo", None) or {}),
-        **(v.pop("blog", None) or {}),
-        **(v.pop("location", None) or {}),
-        **(v.pop("post", None) or {}),
-        **v,
-    }
-
     if v.get("title") in ("[Deleted video]", "[Private video]"):
         return None
 
+    v = utils.flatten_dict(v, passthrough_keys=["automatic_captions", "http_headers", "subtitles"])
+
     upload_date = safe_unpack(
         v.pop("upload_date", None),
         v.pop("release_date", None),
         v.pop("date", None),
         v.pop("created_at", None),
         v.pop("published", None),
         v.pop("updated", None),
@@ -84,17 +85,14 @@
     duration = v.pop("duration", None)
     cv["duration"] = 0 if not duration else int(duration)
     cv["time_uploaded"] = upload_date
     cv["time_created"] = consts.APPLICATION_START
     cv["time_modified"] = 0  # this should be 0 if the file has never been downloaded
     cv["time_deleted"] = 0
     cv["time_downloaded"] = 0
-    cv["play_count"] = 0
-    cv["time_played"] = 0
-    cv["playhead"] = 0
     language = v.pop("language", None)
     cv["tags"] = combine(
         "language:" + language if language else None,
         v.pop("description", None),
         v.pop("caption", None),
         v.pop("content", None),
         v.pop("categories", None),
@@ -179,19 +177,14 @@
 
 def _add(args, entry):
     tags = entry.pop("tags", None) or ""
     media_id = args.db.pop("select id from media where path = ?", [entry["path"]])
     if media_id:
         entry["id"] = media_id
 
-        # remove default 0s to not overwrite existing value during upsert
-        entry.pop("play_count", None)
-        entry.pop("time_played", None)
-        entry.pop("playhead", None)
-
         args.db["media"].upsert(utils.dict_filter_bool(entry), pk="id", alter=True)
     else:
         args.db["media"].insert(utils.dict_filter_bool(entry), pk="id", alter=True)
         media_id = args.db.pop("select id from media where path = ?", [entry["path"]])
     if tags:
         args.db["captions"].insert({"media_id": media_id, "time": 0, "text": tags}, alter=True)
```

### Comparing `xklb-1.31.9/xklb/play_actions.py` & `xklb-2.1.2/xklb/play_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import argparse, os, shlex, shutil, sys, time
 from collections import deque
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 from random import random
 from typing import Dict, Tuple
 
-from xklb import consts, db, player, subtitle, tube_backend, usage, utils
+from xklb import consts, db, history, player, subtitle, tube_backend, usage, utils
 from xklb.consts import SC
-from xklb.playback import now_playing
 from xklb.player import mark_media_deleted, override_sort
 from xklb.scripts.bigdirs import process_bigdirs
+from xklb.scripts.playback_control import now_playing
 from xklb.utils import cmd_interactive, log, random_filename, safe_unpack
 
 
 def parse_args_sort(args) -> None:
     if args.sort:
         args.sort = " ".join(args.sort)
     elif not args.sort and hasattr(args, "defaults"):
@@ -45,19 +45,18 @@
                 args.limit != consts.DEFAULT_PLAY_QUEUE,
             ],
         )
         else None,
         args.sort,
         "duration desc" if args.action in (SC.listen, SC.watch) and args.include else None,
         "size desc" if args.action in (SC.listen, SC.watch) and args.include else None,
-        "play_count" if args.action in (SC.listen, SC.watch) and "play_count" in m_columns else None,
+        "play_count" if args.action in (SC.listen, SC.watch) else None,
         "size desc, duration"
         if args.action in (SC.listen, SC.watch) and "size" in m_columns and "duration" in m_columns
         else None,
-        "sparseness" if args.action == SC.filesystem else None,
         "size" if args.action == SC.filesystem else None,
         "m.path",
         "random",
     ]
 
     sort = list(filter(bool, sorts))
     sort = [override_sort(s) for s in sort]
@@ -261,14 +260,16 @@
 
     args.sock = None
     return args
 
 
 def construct_query(args) -> Tuple[str, dict]:
     m_columns = db.columns(args, "media")
+    h_columns = db.columns(args, "history")
+
     args.filter_sql = []
     args.filter_bindings = {}
 
     if args.duration:
         args.filter_sql.append(" and duration IS NOT NULL " + args.duration)
     if args.size:
         args.filter_sql.append(" and size IS NOT NULL " + args.size)
@@ -364,17 +365,23 @@
     query = f"""WITH m as (
     SELECT rowid, * FROM {args.table}
     WHERE 1=1
         {player.filter_args_sql(args, m_columns)}
     )
     SELECT
         {args.select_sql}
+        , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
+        , MIN(h.time_played) time_first_played
+        , MAX(h.time_played) time_last_played
+        , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
     FROM m
+    LEFT JOIN history h on h.media_id = m.id
     WHERE 1=1
         {" ".join(args.filter_sql)}
+    GROUP BY m.id, m.path -- for time_played aggregates
     ORDER BY 1=1
         , {args.sort}
     {args.limit_sql} {args.offset_sql}
     """
 
     args.filter_sql = [
         s for s in args.filter_sql if "rowid" not in s
@@ -493,15 +500,15 @@
             args,
             m["original_path"],
             start_time,
             existing_playhead=m.get("playhead"),
             media_duration=m.get("duration"),
         )
         if playhead:
-            player.set_playhead(args, m["original_path"], playhead)
+            history.add(args, [m["original_path"]], playhead=playhead)
 
 
 def play(args, m) -> None:
     t = utils.Timer()
     print(m["now_playing"])
     log.debug("now_playing: %s", t.elapsed())
 
@@ -538,14 +545,16 @@
                 else:
                     raise SystemExit(r.returncode)
     finally:
         save_playhead(args, m, start_time)
 
 
 def process_playqueue(args) -> None:
+    history.create(args)
+
     t = utils.Timer()
     query, bindings = construct_query(args)
     log.debug("construct_query: %s", t.elapsed())
 
     if args.print and not any(
         [
             args.partial,
@@ -560,39 +569,25 @@
     ):
         player.printer(args, query, bindings)
         return
 
     media = list(args.db.query(query, bindings))
     log.debug("query: %s", t.elapsed())
 
-    if args.partial and Path(args.watch_later_directory).exists():
-        media = utils.mpv_enrich2(args, media)
-        log.debug("utils.mpv_enrich2: %s", t.elapsed())
+    if args.partial:
+        media = utils.history_sort(args, media)
+        log.debug("utils.history_sort: %s", t.elapsed())
 
     if args.lower is not None or args.upper is not None:
         media = utils.filter_episodic(args, media)
         log.debug("utils.filter_episodic: %s", t.elapsed())
 
     if not media:
         utils.no_media_found()
 
-    if all(
-        [
-            Path(args.watch_later_directory).exists(),
-            args.play_in_order == 0,
-            args.related == 0,
-            not args.cluster,
-            "sort" in args.defaults,
-            not args.partial,
-            not args.random,
-        ],
-    ):
-        media = utils.mpv_enrich(args, media)
-        log.debug("utils.mpv_enrich: %s", t.elapsed())
-
     if args.safe:
         media = [d for d in media if tube_backend.is_supported(d["path"]) or Path(d["path"]).exists()]
         log.debug("tube_backend.is_supported: %s", t.elapsed())
 
     if args.big_dirs:
         media_keyed = {d["path"]: d for d in media}
         dirs = process_bigdirs(args, media)
```

### Comparing `xklb-1.31.9/xklb/playback.py` & `xklb-2.1.2/xklb/scripts/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/player.py` & `xklb-2.1.2/xklb/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from shlex import join, quote, split
 from shutil import which
 from time import sleep
 from typing import Dict, List, Optional, Tuple, Union
 
 from tabulate import tabulate
 
-from xklb import consts, db, media, utils
+from xklb import consts, db, history, media, utils
 from xklb.consts import SC
 from xklb.utils import cmd, cmd_interactive, human_time, log
 
 try:
     import tkinter  # noqa
 
     from xklb import gui
@@ -126,16 +126,14 @@
                     player.extend([f"--end={end}"])
 
         if args.action == SC.watch and m and m.get("subtitle_count") is not None:
             if m["subtitle_count"] > 0:
                 player.extend(args.player_args_sub)
             elif m["size"] > 500 * 1000000:  # 500 MB
                 log.debug("Skipping subs player_args: size")
-            elif m.get("time_partial_first"):
-                log.debug("Skipping subs player_args: partially watched")
             else:
                 player.extend(args.player_args_no_sub)
 
     elif system() == "Linux":
         player_path = find_xdg_application(m["path"])
         if player_path:
             args.player_need_sleep = False
@@ -180,48 +178,14 @@
                     (*chunk_paths,),
                 )
                 modified_row_count += cursor.rowcount
 
     return modified_row_count
 
 
-def set_playhead(args, path: str, playhead: int) -> int:
-    with args.db.conn:
-        cursor = args.db.conn.execute(
-            f"""UPDATE media
-            SET playhead = :playhead
-                , time_played = {consts.now()}
-            WHERE path = :path
-            """,
-            {"playhead": playhead, "path": path},
-        )
-    return cursor.rowcount
-
-
-def mark_media_watched(args, paths, time_watched=consts.now()) -> int:
-    paths = utils.conform(paths)
-    modified_row_count = 0
-    if paths:
-        df_chunked = utils.chunks(paths, consts.SQLITE_PARAM_LIMIT)
-        for chunk_paths in df_chunked:
-            with args.db.conn:
-                cursor = args.db.conn.execute(
-                    f"""UPDATE media
-                    SET play_count = play_count + 1
-                        , time_played = {time_watched}
-                    WHERE path in ("""
-                    + ",".join(["?"] * len(chunk_paths))
-                    + ")",
-                    (*chunk_paths,),
-                )
-                modified_row_count += cursor.rowcount
-
-    return modified_row_count
-
-
 def mark_media_deleted(args, paths, time_deleted=consts.APPLICATION_START) -> int:
     paths = utils.conform(paths)
 
     modified_row_count = 0
     if paths:
         df_chunked = utils.chunks(paths, consts.SQLITE_PARAM_LIMIT)
         for chunk_paths in df_chunked:
@@ -312,15 +276,15 @@
     ASK_MOVE = (Action.MOVE, Action.KEEP)
     ASK_DELETE = (Action.DELETE, Action.KEEP)
     ASK_SOFTDELETE = (Action.SOFTDELETE, Action.KEEP)
     ASK_MOVE_OR_DELETE = (Action.MOVE, Action.DELETE)
 
 
 def post_act(args, media_file: str, action: Optional[str] = None, geom_data=None, media=None) -> None:
-    mark_media_watched(args, [media_file])
+    history.add(args, [media_file], mark_done=True)
 
     def handle_delete_action():
         if media_file.startswith("http"):
             mark_media_deleted(args, media_file)
         else:
             delete_media(args, media_file)
 
@@ -430,15 +394,17 @@
         if candidate in ("" or new_candidate):
             return m
 
         candidate = new_candidate
         query = f"""
             SELECT
                 {args.select_sql}
+                , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
             FROM {'media' if args.play_in_order >= consts.SIMILAR_NO_FILTER_NO_FTS else args.table}
+            LEFT JOIN history h on h.media_id = m.id
             WHERE 1=1
                 and path like :candidate
                 {filter_args_sql(args, m_columns)}
                 {'' if args.play_in_order >= consts.SIMILAR_NO_FILTER else (" ".join(args.filter_sql) or '')}
                 {"and path not in ({})".format(",".join([f":ignore_path{i}" for i in range(len(ignore_paths))])) if len(ignore_paths) > 0 else ''}
             ORDER BY play_count, path
             LIMIT 1000
@@ -479,15 +445,17 @@
     )
     args.include = sorted(words, key=len, reverse=True)[:100]
     args.table = db.fts_flexible_search(args)
 
     query = f"""
         SELECT
             {args.select_sql}, rank
+            , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
         FROM {args.table} m
+        LEFT JOIN history h on h.media_id = m.id
         WHERE 1=1
             and path != :path
             {filter_args_sql(args, m_columns)}
             {'' if args.related >= consts.RELATED_NO_FILTER else (" ".join(args.filter_sql) or '')}
         ORDER BY play_count
             , m.path like "http%"
             , {'rank' if 'sort' in args.defaults else f'ntile(1000) over (order by rank), {args.sort}'}
@@ -520,15 +488,17 @@
             + " OR ".join([f"(path LIKE :subpath{i} and path not like :subpath{i} || '/%')" for i in range(len(dirs))])
             + ")"
         )
 
     query = f"""
         SELECT
             {args.select_sql}
+            , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
         FROM {args.table} m
+        LEFT JOIN history h on h.media_id = m.id
         WHERE 1=1
             {filter_args_sql(args, m_columns)}
             {filter_paths}
             {'' if args.related >= consts.DIRS_NO_FILTER else (" ".join(args.filter_sql) or '')}
         ORDER BY play_count
             , m.path LIKE "http%"
             {'' if 'sort' in args.defaults else ', ' + args.sort}
@@ -875,15 +845,16 @@
     query = f"""
     SELECT
         {time_period} AS time_period
         , SUM(duration) AS duration_sum
         , AVG(duration) AS duration_avg
         , SUM(size) AS size_sum
         , AVG(size) AS size_avg
-    FROM media
+    FROM media m
+    LEFT JOIN history h on h.media_id = m.id
     WHERE coalesce(time_period, 0)>0 and {time_column}>0 {where}
     GROUP BY time_period
     """
     return list(args.db.query(query))
 
 
 def cadence_adjusted_duration(args, duration):
@@ -910,17 +881,14 @@
         D = {"path": "Aggregate", "count": len(media)}
 
         if "duration" in media[0]:
             D["duration"] = duration
             D["avg_duration"] = duration / len(media)
             D["cadence_adj_duration"] = cadence_adjusted_duration(args, duration)
 
-        if "sparseness" in media[0]:
-            D["sparseness"] = None
-
         if "size" in media[0]:
             D["size"] = sum((d["size"] or 0) for d in media)
             D["avg_size"] = sum((d["size"] or 0) for d in media) / len(media)
 
         if args.cols:
             for c in args.cols:
                 if isinstance(media[0][c], Number):
@@ -929,15 +897,15 @@
         media = [D]
 
     else:
         if "d" in args.print:
             marked = mark_media_deleted(args, [d["path"] for d in media])
             log.warning(f"Marked {marked} metadata records as deleted")
         if "w" in args.print:
-            marked = mark_media_watched(args, [d["path"] for d in media])
+            marked = history.add(args, [d["path"] for d in media])
             log.warning(f"Marked {marked} metadata records as watched")
 
     if "f" in args.print:
         if args.limit == 1:
             path = media[0]["path"]
             if not Path(path).exists():
                 mark_media_deleted(args, path)
```

### Comparing `xklb-1.31.9/xklb/playlists.py` & `xklb-2.1.2/xklb/playlists.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sqlite3
 from copy import deepcopy
 from datetime import datetime, timezone
-from typing import List
+from typing import List, Optional
 
 from xklb import consts, db, utils
 from xklb.utils import log, safe_unpack
 
 """
 playlists table
     extractor_key = Name of the Extractor -- "Local", "Imgur", "YouTube"
@@ -73,44 +73,49 @@
     playlists_id = get_id(args, entry["path"])
     if playlists_id:
         entry["id"] = playlists_id
         args.db["playlists"].upsert(entry, pk="id", alter=True)
     else:
         args.db["playlists"].insert(entry, pk="id", alter=True)
         playlists_id = get_id(args, entry["path"])
+    return playlists_id
 
 
 def exists(args, playlist_path) -> bool:
     try:
         known = args.db.pop("select 1 from playlists where path=?", [str(playlist_path)])
     except sqlite3.OperationalError as e:
         log.debug(e)
         return False
     if known is None:
         return False
     return True
 
 
-def is_playlist_subpath(args, playlist_path) -> bool:
+def get_subpath_playlist_id(args, playlist_path) -> Optional[int]:
     try:
-        known = args.db.pop("select path from playlists where ? like path || '%'", [str(playlist_path)])
+        known = args.db.pop(
+            "select path from playlists where ? like path || '%' and path != ?",
+            [str(playlist_path), str(playlist_path)],
+        )
     except sqlite3.OperationalError as e:
         log.debug(e)
-        return False
-    if known is None:
-        return False
-    return True
+        return None
+    return known
 
 
-def add(args, playlist_path: str, info: dict) -> int:
-    if exists(args, playlist_path) or not is_playlist_subpath(args, playlist_path):
-        pl = consolidate(args, deepcopy(info))
-        playlist = {**pl, "path": playlist_path, **args.extra_playlist_data}
-        _add(args, utils.dict_filter_bool(playlist))
-    return get_id(args, playlist_path)
+def add(args, playlist_path: str, info: dict, check_subpath=False) -> int:
+    if check_subpath:
+        subpath_playlist_id = get_subpath_playlist_id(args, playlist_path)
+        if subpath_playlist_id:
+            return subpath_playlist_id
+
+    pl = consolidate(args, deepcopy(info))
+    playlist = {**pl, "path": playlist_path, **args.extra_playlist_data}
+    return _add(args, utils.dict_filter_bool(playlist))
 
 
 def media_exists(args, playlist_path, path) -> bool:
     m_columns = db.columns(args, "media")
     try:
         known = args.db.execute(
             f"select 1 from media where playlist_id in (select id from playlists where path = ?) and (path=? or {'web' if 'webpath' in m_columns else ''}path=?)",
```

### Comparing `xklb-1.31.9/xklb/praw_extract.py` & `xklb-2.1.2/xklb/praw_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,27 +193,18 @@
             "SELECT path FROM media WHERE webpath =?",
             [slim_dict["path"]],
             ignore_errors=["no such column", "no such table"],
         )
         if already_downloaded_path:
             slim_dict["path"] = already_downloaded_path
 
-        existing_meta = args.db.pop_dict(
-            "SELECT play_count, time_played, time_downloaded, time_deleted FROM media WHERE path =?",
-            [slim_dict["path"]],
-            ignore_errors=["no such column", "no such table"],
-        )
         slim_dict = {
             **slim_dict,
-            "play_count": 0,
-            "time_played": 0,
-            "playhead": 0,
             "time_downloaded": 0,
             "time_deleted": 0,
-            **(existing_meta or {}),
         }
 
         if post_dict.get("author_is_blocked") == 1:
             pass
         elif "selftext" in slim_dict:
             args.db["reddit_posts"].upsert(slim_dict, pk=["path", "subreddit"], alter=True)
         else:
```

### Comparing `xklb-1.31.9/xklb/search.py` & `xklb-2.1.2/xklb/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,14 +179,16 @@
     args = parse_args()
     query, bindings = construct_query(args)
     captions = list(args.db.query(query, bindings))
     merged_captions = merge_captions(args, captions)
 
     if args.open:
         for d in merged_captions:
+            print(d["text"])
+
             args.start = str(d["time"] - 2)
             args.end = str(int(d["end"] + 1.5))
             m = args.db.pop_dict("select * from media where path = ?", [d["path"]])
             args.player = player.parse(args, m)
             r = player.local_player(args, m)
             if r.returncode != 0:
                 log.warning("Player exited with code %s", r.returncode)
```

### Comparing `xklb-1.31.9/xklb/subtitle.py` & `xklb-2.1.2/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/tabs_actions.py` & `xklb-2.1.2/xklb/tabs_actions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 from pathlib import Path
 from time import sleep
 from typing import Dict, List, Tuple
 
-from xklb import db, usage, utils
+from xklb import db, history, usage, utils
 from xklb.consts import SC
-from xklb.player import generic_player, mark_media_watched, override_sort, printer
+from xklb.player import generic_player, override_sort, printer
 from xklb.utils import cmd, flatten, log
 
 
 def parse_args(action) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library tabs",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
@@ -87,25 +87,38 @@
     for idx, exc in enumerate(args.exclude):
         args.filter_sql.append(tabs_exclude_sql(idx))
         args.filter_bindings[f"exclude{idx}"] = "%" + exc.replace(" ", "%").replace("%%", " ") + "%"
 
     LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
     OFFSET = f"OFFSET {args.skip}" if args.skip else ""
 
-    query = f"""SELECT path
+    query = f"""WITH m as (
+            SELECT
+                path
+                , frequency
+                , COALESCE(MAX(time_played), 0) time_played
+                , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
+                , time_deleted
+                , hostname
+                , category
+            FROM media
+            LEFT JOIN history h on h.media_id = media.id
+            GROUP BY media.id
+        )
+        SELECT path
         , frequency
         , CASE
             WHEN frequency = 'daily' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+1 Day' )) as int)
             WHEN frequency = 'weekly' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+7 Days' )) as int)
             WHEN frequency = 'monthly' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+1 Month' )) as int)
             WHEN frequency = 'quarterly' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+3 Months' )) as int)
             WHEN frequency = 'yearly' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+1 Year' )) as int)
         END time_valid
         {', ' + ', '.join(args.cols) if args.cols else ''}
-    FROM media
+    FROM m
     WHERE 1=1
         and COALESCE(time_deleted,0) = 0
         {" ".join(args.filter_sql)}
         {"and time_valid < cast(STRFTIME('%s', datetime()) as int)" if not args.print else ''}
     ORDER BY 1=1
         {', ' + args.sort if args.sort else ''}
         {', time_played, time_valid, path' if args.print else ''}
@@ -128,15 +141,15 @@
     return query, args.filter_bindings
 
 
 def play(args, m: Dict) -> None:
     media_file = m["path"]
 
     cmd(*generic_player(args), media_file, strict=False)
-    mark_media_watched(args, [media_file])
+    history.add(args, [media_file], mark_done=True)
 
 
 def frequency_filter(args, media: List[Dict]) -> List[dict]:
     mapper = {
         "daily": 1,
         "weekly": 7,
         "monthly": 30,
@@ -178,8 +191,9 @@
         if len(media) >= MANY_TABS:
             sleep(0.3)
     return None
 
 
 def tabs() -> None:
     args = parse_args(SC.tabs)
+    history.create(args)
     process_tabs_actions(args)
```

### Comparing `xklb-1.31.9/xklb/tabs_extract.py` & `xklb-2.1.2/xklb/tabs_extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,16 +76,14 @@
 
     return {
         "path": path,
         "hostname": hostname,
         "frequency": args.frequency,
         "category": args.category or "Uncategorized",
         "time_created": consts.APPLICATION_START,
-        "time_played": 0,
-        "play_count": 0,
         "time_deleted": 0,
     }
 
 
 def tabs_add(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
```

### Comparing `xklb-1.31.9/xklb/tube_backend.py` & `xklb-2.1.2/xklb/tube_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 
 playlists_of_playlists = []
 added_media_count = 0
 
 
 def get_playlist_metadata(args, playlist_path, ydl_opts, playlist_root=True) -> None:
     yt_dlp = load_module_level_yt_dlp()
+    t = utils.Timer()
 
     class ExistingPlaylistVideoReached(yt_dlp.DownloadCancelled):
         pass
 
     class AddToArchivePP(yt_dlp.postprocessor.PostProcessor):
         def run(self, info) -> Tuple[list, dict]:  # pylint: disable=arguments-renamed
             global added_media_count
@@ -104,51 +105,60 @@
             if info:
                 webpath = safe_unpack(info.get("webpage_url"), info.get("url"), info.get("original_url"))
                 if webpath != playlist_path and info.get("webpage_url_basename") == "playlist":
                     if playlist_root:
                         if not info.get("playlist_id") or webpath == playlist_path:
                             log.warning("Importing playlist-less media %s", playlist_path)
                         playlists.add(args, playlist_path, info)
+                        log.info("playlists.add %s", t.elapsed())
 
                     if args.ignore_errors:
                         if webpath in playlists_of_playlists and not playlist_root:
                             raise ExistingPlaylistVideoReached  # prevent infinite bug
                     else:
                         if webpath in playlists_of_playlists:
                             raise ExistingPlaylistVideoReached  # prevent infinite bug
 
                     get_playlist_metadata(args, webpath, ydl_opts, playlist_root=False)
+                    log.info("get_playlist_metadata %s", t.elapsed())
                     playlists_of_playlists.append(webpath)
                     return [], info
 
                 entry = deepcopy(info)
                 if entry:
-                    if not info.get("playlist_id") or webpath == playlist_path:
-                        log.warning("Importing playlist-less media %s", playlist_path)
-                    playlist_id = playlists.add(args, playlist_path, info)
-
                     if playlists.media_exists(args, playlist_path, webpath) and not args.ignore_errors:
                         raise ExistingPlaylistVideoReached
 
-                    entry = {**entry, "playlist_id": playlist_id, **args.extra_media_data}
+                    entry = {**entry, **args.extra_media_data}
+
+                    if not info.get("playlist_id") or webpath == playlist_path:
+                        log.warning("Importing playlist-less media %s", playlist_path)
+                    else:
+                        playlist_id = playlists.add(args, playlist_path, info)  # add sub-playlist
+                        entry["playlist_id"] = playlist_id
+                        log.info("playlists.add2 %s", t.elapsed())
+
                     media.add(args, webpath, entry)  # type: ignore
+                    log.info("media.add %s", t.elapsed())
 
                     added_media_count += 1
                     if added_media_count > 1:
-                        sys.stdout.write("\033[K\r")
-                        print(f"[{playlist_path}] Added {added_media_count} media", end="\r", flush=True)
+                        # sys.stdout.write("\033[K\r")
+                        print(f"[{playlist_path}] Added {added_media_count} media")  # , end="\r", flush=True)
 
             return [], info
 
     with yt_dlp.YoutubeDL(ydl_opts) as ydl:
         ydl.add_post_processor(AddToArchivePP(), when="pre_process")
 
+        log.info("yt-dlp initialized %s", t.elapsed())
         count_before_extract = added_media_count
         try:
             pl = ydl.extract_info(playlist_path, download=False, process=True)
+            log.info("ydl.extract_info done %s", t.elapsed())
         except yt_dlp.DownloadError:
             log.error("[%s] DownloadError skipping", playlist_path)
         except ExistingPlaylistVideoReached:
             if added_media_count > count_before_extract:
                 sys.stdout.write("\n")
             playlists.log_problem(args, playlist_path)
         else:
@@ -213,29 +223,26 @@
     ) as ydl:
         videos = args.db.execute(
             f"""
             SELECT
               id
             , path
             , playlist_id
-            , play_count
-            , time_played
-            , playhead
             FROM media
             WHERE 1=1
                 {'and width is null' if 'width' in m_columns else ''}
                 and path not like '%playlist%'
                 and playlist_id = (select id from playlists where path = ?)
             ORDER by random()
             """,
             [playlist_path],
         ).fetchall()
 
         current_video_count = 0
-        for id, path, playlist_id, play_count, time_played, playhead in videos:
+        for id, path, playlist_id in videos:
             entry = ydl.extract_info(path)
             if entry is None:
                 continue
 
             chapters = getattr(entry, "chapters", [])
             chapter_count = len(chapters)
             if chapter_count > 0:
@@ -259,18 +266,15 @@
                     else:
                         captions.extend([{"media_id": id, **d} for d in file_captions])
                 if len(captions) > 0:
                     args.db["captions"].insert_all(captions, alter=True)
 
             entry["id"] = id
             entry["playlist_id"] = playlist_id
-            entry["play_count"] = play_count
             entry["chapter_count"] = chapter_count
-            entry["time_played"] = time_played
-            entry["playhead"] = playhead
 
             media.add(args, path, entry)
 
             current_video_count += 1
             sys.stdout.write("\033[K\r")
             print(
                 f"[{playlist_path}] {current_video_count} of {len(videos)} extra metadata fetched",
```

### Comparing `xklb-1.31.9/xklb/tube_extract.py` & `xklb-2.1.2/xklb/tube_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         sys.argv = ["tubeadd", *args]
 
     args = parse_args(SC.tubeadd, usage=usage.tubeadd)
     if args.playlist_files:
         args.playlists = list(utils.flatten([Path(p).read_text().splitlines() for p in args.playlists]))
 
     known_playlists = set()
-    if not args.force:
+    if not args.force and len(args.playlists) > 9:
         known_playlists = media.get_paths(args)
 
     for path in args.playlists:
         if args.safe and not tube_backend.is_supported(path):
             log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
             continue
```

### Comparing `xklb-1.31.9/xklb/usage.py` & `xklb-2.1.2/xklb/usage.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     Create a video database and read internal/external subtitle files into a searchable database:
         library fsadd --scan-subtitles tv.search.db ./tv/ ./movies/
 
     Decode media to check for corruption (slow):
         library fsadd --check-corrupt 100 tv.db ./tv/  # scan through 100 percent of each file to evaluate how corrupt it is (very slow)
         library fsadd --check-corrupt   1 tv.db ./tv/  # scan through 1 percent of each file to evaluate how corrupt it is (takes about one second per file)
-        library fsadd --check-corrupt   5 tv.db ./tv/  # scan through 1 percent of each file to evaluate how corrupt it is (takes about ten seconds per file)
+        library fsadd --check-corrupt   5 tv.db ./tv/  # scan through 5 percent of each file to evaluate how corrupt it is (takes about ten seconds per file)
 
         library fsadd --check-corrupt   5 --delete-corrupt 30 tv.db ./tv/  # scan 5 percent of each file to evaluate how corrupt it is, if 30 percent or more of those checks fail then the file is deleted
 
         nb: the behavior of delete-corrupt changes between full and partial scan
         library fsadd --check-corrupt  99 --delete-corrupt  1 tv.db ./tv/  # partial scan 99 percent of each file to evaluate how corrupt it is, if 1 percent or more of those checks fail then the file is deleted
         library fsadd --check-corrupt 100 --delete-corrupt  1 tv.db ./tv/  # full scan each file to evaluate how corrupt it is, if there is _any_ corruption then the file is deleted
 
@@ -742,16 +742,27 @@
 
         By default tubeupdate will quickly add media.
         You can run with --extra to fetch more details: (best resolution width, height, subtitle tags, etc)
 
         library tubeupdate educational.db --extra https://www.youtube.com/channel/UCBsEUcR-ezAuxB2WlfeENvA/videos
 """
 
-galleryadd = None
-galleryupdate = None
+galleryadd = """library galleryadd DATABASE URLS
+
+Add gallery_dl URLs to download later or periodically update
+
+Passing the `--playlist-files` flag will treat each URL as a local file to read URLs from
+
+    library galleryadd my.db ./my-favorite-manhwa.txt
+"""
+
+galleryupdate = """library galleryupdate DATABASE URLS
+
+Check previously saved gallery_dl URLs for new content
+"""
 
 bigdirs = """library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by deleted | played] [--size=+5MB]
 
     See what folders take up space
 
         library bigdirs video.db
         library bigdirs audio.db
@@ -770,17 +781,46 @@
 
         library christen audio.db --run
 
     You can optionally replace all the spaces in your filenames with dots
 
         library christen --dot-space video.db
 """
+
 cluster_sort = """library cluster-sort [input_path | stdin] [output_path | stdout]
 
     Group lines of text into sorted output
+
+    $ echo 'red apple
+    broccoli
+    yellow
+    green
+    orange apple
+    red apple' | library cluster-sort
+
+    orange apple
+    red apple
+    red apple
+    broccoli
+    green
+    yellow
+
+    $ echo 'red apple
+    broccoli
+    yellow
+    green
+    orange apple
+    red apple' | library cluster-sort --groups
+
+    [
+        {'common_prefix': '',
+        'grouped_paths': ['orange apple\n', 'red apple\n', 'red apple\n']},
+        {'common_prefix': '',
+        'grouped_paths': ['broccoli\n', 'green\n', 'yellow\n']}
+    ]
 """
 
 copy_play_counts = """library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
 
     Copy play count information between databases
 
         library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
@@ -892,17 +932,89 @@
 
         # move new music for this week
         library relmv (
             library listen ~/lb/audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
         ) /mnt/d/80_Now_Listening/
 """
 
+mv_list = """library mv-list [--limit LIMIT] [--lower LOWER] [--upper UPPER] MOUNT_POINT DATABASE
+
+Free up space on a specific disk. Find candidates for moving data to a different mount point
+
+
+The program takes a mount point and a xklb database file. If you don't have a database file you can create one like this:
+
+    $ library fsadd --filesystem d.db ~/d/
+
+But this should definitely also work with xklb audio and video databases:
+
+    $ library mv-list /mnt/d/ video.db
+
+The program will print a table with a sorted list of folders which are good candidates for moving.
+Candidates are determined by how many files are in the folder (so you don't spend hours waiting for folders with millions of tiny files to copy over).
+The default is 4 to 4000--but it can be adjusted via the --lower and --upper flags.
+
+    ...
+    ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
+    │ 4.0 GB   │       7 │ /mnt/d/71_Mealtime_Videos/unsorted/Miguel_4K/                                                                 │
+    ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
+    │ 5.7 GB   │      10 │ /mnt/d/71_Mealtime_Videos/unsorted/Bollywood_Premium/                                                         │
+    ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
+    │ 2.3 GB   │       4 │ /mnt/d/71_Mealtime_Videos/chief_wiggum/                                                                       │
+    ╘══════════╧═════════╧═══════════════════════════════════════════════════════════════════════════════════════════════════════════════╛
+    6702 other folders not shown
+
+    ██╗███╗░░██╗░██████╗████████╗██████╗░██╗░░░██╗░█████╗░████████╗██╗░█████╗░███╗░░██╗░██████╗
+    ██║████╗░██║██╔════╝╚══██╔══╝██╔══██╗██║░░░██║██╔══██╗╚══██╔══╝██║██╔══██╗████╗░██║██╔════╝
+    ██║██╔██╗██║╚█████╗░░░░██║░░░██████╔╝██║░░░██║██║░░╚═╝░░░██║░░░██║██║░░██║██╔██╗██║╚█████╗░
+    ██║██║╚████║░╚═══██╗░░░██║░░░██╔══██╗██║░░░██║██║░░██╗░░░██║░░░██║██║░░██║██║╚████║░╚═══██╗
+    ██║██║░╚███║██████╔╝░░░██║░░░██║░░██║╚██████╔╝╚█████╔╝░░░██║░░░██║╚█████╔╝██║░╚███║██████╔╝
+    ╚═╝╚═╝░░╚══╝╚═════╝░░░░╚═╝░░░╚═╝░░╚═╝░╚═════╝░░╚════╝░░░░╚═╝░░░╚═╝░╚════╝░╚═╝░░╚══╝╚═════╝░
+
+    Type "done" when finished
+    Type "more" to see more files
+    Paste a folder (and press enter) to toggle selection
+    Type "*" to select all files in the most recently printed table
+
+Then it will give you a prompt:
+
+    Paste a path:
+
+Wherein you can copy and paste paths you want to move from the table and the program will keep track for you.
+
+    Paste a path: /mnt/d/75_MovieQueue/720p/s11/
+    26 selected paths: 162.1 GB ; future free space: 486.9 GB
+
+You can also press the up arrow or paste it again to remove it from the list:
+
+    Paste a path: /mnt/d/75_MovieQueue/720p/s11/
+    25 selected paths: 159.9 GB ; future free space: 484.7 GB
+
+After you are done selecting folders you can press ctrl-d and it will save the list to a tmp file:
+
+    Paste a path: done
+
+        Folder list saved to /tmp/tmpa7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
+
+            rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmpa7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
+"""
+
 scatter = """library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --srcmounts SRCMOUNTS DATABASE RELATIVE_PATHS ...
 
-    Balance size
+Balance files across filesystem folder trees or multiple devices (mostly useful for mergerfs)
+
+    Scatter filesystem folder trees (without mountpoints; limited functionality; good for balancing fs inodes)
+
+        $ library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
+
+    Reduce number of files per folder (creates more folders)
+
+        $ library scatter scatter.db --max-files-per-folder 16000 /test/{0,1,2,3,4,5,6,7,8,9}
+
+    Multi-device re-bin: balance by size
 
         $ library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 ~/lb/fs/scatter.db subfolder/of/mergerfs/mnt
         Current path distribution:
         ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
         │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
         ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
         │ /mnt/d1 │        12793 │ 169.5 GB     │ 4.5 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
@@ -941,25 +1053,21 @@
         ### Move 1146 files to /mnt/d5 with this command: ###
         rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpfrj141jj / /mnt/d5
         ### Move 1185 files to /mnt/d3 with this command: ###
         rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpqh2euc8n / /mnt/d3
         ### Move 1134 files to /mnt/d4 with this command: ###
         rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmphzb0gj92 / /mnt/d4
 
-    Balance device inodes for specific subfolder
+    Multi-device re-bin: balance device inodes for specific subfolder
 
         $ library scatter -m /mnt/d1:/mnt/d2 ~/lb/fs/scatter.db subfolder --group count --sort 'size desc'
 
-    Scatter the most recent 100 files
+    Multi-device re-bin: only consider the most recent 100 files
 
         $ library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' ~/lb/fs/scatter.db /
-
-    Scatter without mountpoints (limited functionality; only good for balancing fs inodes)
-
-        $ library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
 """
 surf = """library surf [--count COUNT] [--target-hosts TARGET_HOSTS] < stdin
 
     Streaming tab loader: press ctrl+c to stop.
 
     Open tabs from a line-delimited file:
 
@@ -990,7 +1098,12 @@
         end | parallel -j5
 """
 
 reddit_selftext = """library reddit-selftext DATABASE
 
     Extract URLs from reddit selftext from the reddit_posts table to the media table
 """
+
+mpv_watchlater = """library mpv-watchlater DATABASE [--watch-later-directory ~/.config/mpv/watch_later/]
+
+    Extract timestamps from MPV to the history table
+"""
```

### Comparing `xklb-1.31.9/xklb/utils.py` & `xklb-2.1.2/xklb/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse, csv, functools, hashlib, logging, math, multiprocessing, os, platform, random, re, shlex, shutil, signal, string, subprocess, sys, tempfile, time
 from ast import literal_eval
+from collections import Counter
 from collections.abc import Iterable
 from copy import deepcopy
 from datetime import datetime, timedelta, timezone
 from functools import wraps
 from pathlib import Path
 from random import shuffle
 from shutil import which
@@ -45,15 +46,15 @@
     parser = argparse.ArgumentParser(add_help=False)
     parser.add_argument("-v", "--verbose", action="count", default=0)
     args, _unknown = parser.parse_known_args()
 
     try:
         if args.verbose > 0 and os.getpgrp() == os.tcgetpgrp(sys.stdout.fileno()):
             sys.excepthook = ultratb.FormattedTB(
-                mode="Context",
+                mode="Verbose" if args.verbose > 1 else "Context",
                 color_scheme="Neutral",
                 call_pdb=True,
                 debugger_cls=TerminalPdb,
             )
     except Exception:
         pass
 
@@ -126,14 +127,27 @@
             yield from flatten(x)
         elif isinstance(x, bytes):
             yield x.decode("utf-8")
         else:
             yield x
 
 
+def flatten_dict(nested_dict, parent_key="", sep="_", passthrough_keys=None):
+    if passthrough_keys is None:
+        passthrough_keys = []
+    flattened_dict = {}
+    for key, value in nested_dict.items():
+        new_key = f"{parent_key}{sep}{key}" if parent_key else key
+        if isinstance(value, dict) and key not in passthrough_keys:
+            flattened_dict.update(flatten_dict(value, new_key, sep, passthrough_keys))
+        else:
+            flattened_dict[new_key] = value
+    return flattened_dict
+
+
 def conform(list_: Union[str, Iterable]) -> List:
     if not list_:
         return []
     if not isinstance(list_, list):
         list_ = [list_]
     list_ = flatten(list_)
     list_ = list(filter(bool, list_))
@@ -456,36 +470,14 @@
     return cast_infos[0].host
 
 
 def path_to_mpv_watchlater_md5(path: str) -> str:
     return hashlib.md5(path.encode("utf-8")).hexdigest().upper()
 
 
-def mpv_enrich(args, media) -> List[Dict]:
-    for m in media:
-        md5 = path_to_mpv_watchlater_md5(m["path"])
-        metadata_path = Path(args.watch_later_directory, md5)
-        if metadata_path.exists():
-            m["time_partial_first"] = int(metadata_path.stat().st_ctime)
-            m["time_partial_last"] = int(metadata_path.stat().st_mtime)
-        else:
-            m["time_partial_first"] = 0
-            m["time_partial_last"] = 0
-
-    return sorted(media, key=lambda m: m.get("time_partial_first") or 0, reverse=True)
-
-
-def mpv_watchlater_value(path, key) -> Optional[str]:
-    data = Path(path).read_text().splitlines()
-    for s in data:
-        if s.startswith(key + "="):
-            return s.split("=")[1]
-    return None
-
-
 def filter_episodic(args, media: List[Dict]) -> List[Dict]:
     parent_dict = {}
     for m in media:
         path = Path(m["path"])
         parent_path = path.parent
         parent_dict.setdefault(parent_path, 0)
         parent_dict[parent_path] += 1
@@ -503,30 +495,25 @@
             continue
         else:
             filtered_media.append(m)
 
     return filtered_media
 
 
-def mpv_enrich2(args, media) -> List[Dict]:
-    md5s = {path_to_mpv_watchlater_md5(m["path"]): m for m in media}
-    paths = set(Path(args.watch_later_directory).glob("*"))
-
-    previously_watched = [
-        {
-            **(md5s.get(p.stem) or {}),
-            "time_partial_first": int(p.stat().st_ctime),
-            "time_partial_last": int(p.stat().st_mtime),
-            "playhead": safe_int(mpv_watchlater_value(p, "start")),
-        }
-        for p in paths
-        if md5s.get(p.stem)
-    ]
+def mpv_watchlater_value(path, key) -> Optional[str]:
+    data = Path(path).read_text().splitlines()
+    for s in data:
+        if s.startswith(key + "="):
+            return s.split("=")[1]
+    return None
+
+
+def history_sort(args, media) -> List[Dict]:
     if "s" in args.partial:  # skip; only play unseen
-        previously_watched_paths = [m["path"] for m in previously_watched]
+        previously_watched_paths = [m["path"] for m in media if m["time_first_played"]]
         return [m for m in media if m["path"] not in previously_watched_paths]
 
     def mpv_progress(m):
         playhead = m.get("playhead")
         duration = m.get("duration")
         if not playhead:
             return float("-inf")
@@ -538,30 +525,30 @@
         elif "t" in args.partial:
             return -(duration - playhead)  # time remaining
         else:
             return playhead / duration  # percent remaining
 
     def sorting_hat():
         if "f" in args.partial:  # first-viewed
-            return lambda m: m.get("time_partial_first") or 0
+            return lambda m: m.get("time_first_played") or 0
         elif "p" in args.partial or "t" in args.partial:  # sort by remaining duration
             return mpv_progress
 
-        return lambda m: m.get("time_partial_last") or m.get("time_partial_first") or 0
+        return lambda m: m.get("time_last_played") or m.get("time_first_played") or 0
 
     reverse_chronology = True
     if "o" in args.partial:  # oldest first
         reverse_chronology = False
 
     key = sorting_hat()
     if args.print:
         reverse_chronology = not reverse_chronology
 
     media = sorted(
-        previously_watched,
+        media,
         key=key,
         reverse=reverse_chronology,
     )
 
     if args.skip:
         media = media[int(args.skip) :]
 
@@ -1273,7 +1260,45 @@
 
         if all(len(segment) % 2 == 0 for segment in segments):
             for i in range(len(segments)):
                 segments[i] = segments[i][:-1]
 
     segments[-1] += extension
     return str(Path(*segments))
+
+
+def rebin_folders(paths, max_files_per_folder=16000):
+    parent_counts = Counter(Path(p).parent for p in paths)
+    rebinned_tuples = []
+    untouched = []
+    parent_index = {}
+    parent_current_count = {}
+
+    for p in paths:
+        path = Path(p)
+        parent = path.parent
+        if parent_counts[parent] > max_files_per_folder:
+            if parent not in parent_index:
+                parent_index[parent] = 1
+                parent_current_count[parent] = 0
+
+            min_len = math.floor(parent_counts[parent] / max_files_per_folder)
+            rebinned_tuples.append((p, str(parent / str(parent_index[parent]).zfill(len(str(min_len))) / path.name)))
+            parent_current_count[parent] += 1
+
+            _quotient, remainder = divmod(parent_current_count[parent], max_files_per_folder)
+            if remainder == 0:
+                parent_index[parent] += 1
+        else:
+            untouched.append(p)
+
+    return untouched, rebinned_tuples
+
+
+def move_files(file_list):
+    for existing_path, new_path in file_list:
+        parent_dir = os.path.dirname(new_path)
+        os.makedirs(parent_dir, exist_ok=True)
+        try:
+            shutil.move(existing_path, new_path)
+        except Exception:
+            log.exception("Could not move %s", existing_path)
```

### Comparing `xklb-1.31.9/xklb/scripts/bigdirs.py` & `xklb-2.1.2/xklb/scripts/bigdirs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import argparse
+import argparse, os
 from pathlib import Path
 from typing import Dict, List
 
 from tabulate import tabulate
 
-from xklb import db, usage, utils
+from xklb import db, history, usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library bigdirs",
         usage=usage.bigdirs,
@@ -51,18 +51,18 @@
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
 
 
 def group_files_by_folder(args, media) -> List[Dict]:
     d = {}
     for m in media:
-        p = m["path"].split("/")
+        p = m["path"].split(os.sep)
         while len(p) >= 2:
             p.pop()
-            parent = "/".join(p) + "/"
+            parent = os.sep.join(p) + os.sep
 
             file_deleted = bool(m.get("time_deleted", 0))
             file_played = bool(m.get("time_played", 0))
             if parent not in d:
                 d[parent] = {"size": 0, "count": 0, "deleted": 0, "played": 0}
             if not file_deleted:
                 d[parent]["size"] += m.get("size", 0)
@@ -83,19 +83,19 @@
 
     return [{**v, "path": k} for k, v in d.items()]
 
 
 def folder_depth(args, folders) -> List[Dict]:
     d = {}
     for f in folders:
-        p = f["path"].split("/")
+        p = f["path"].split(os.sep)
         p.pop()
 
         depth = 1 + args.depth
-        parent = "/".join(p[:depth]) + "/"
+        parent = os.sep.join(p[:depth]) + os.sep
         if len(p) < depth:
             continue
 
         if d.get(parent):
             d[parent]["size"] += f["size"]
             d[parent]["count"] += f["count"]
             d[parent]["deleted"] += f["deleted"]
@@ -110,34 +110,36 @@
             d.pop(path)
 
     return [{**v, "path": k} for k, v in d.items()]
 
 
 def get_table(args) -> List[dict]:
     m_columns = db.columns(args, "media")
+    h_columns = db.columns(args, "history")
     args.filter_sql = []
     args.filter_bindings = {}
 
     if args.size:
         args.filter_sql.append(" and size IS NOT NULL " + args.size)
     db.construct_search_bindings(args, m_columns)
 
     media = list(
         args.db.query(
             f"""
-        select
+        SELECT
             path
             , size
             {', time_deleted' if 'time_deleted' in m_columns else ''}
-            {', time_played' if 'time_played' in m_columns else ''}
-        from media m
-        where 1=1
+            {', time_played' if 'time_played' in h_columns else ''}
+        FROM media m
+        LEFT JOIN history h on h.media_id = m.id
+        WHERE 1=1
             {'and time_downloaded > 0' if 'time_downloaded' in m_columns else ''}
             {" ".join(args.filter_sql)}
-        order by path
+        ORDER BY path
         """,
             args.filter_bindings,
         ),
     )
     return media
 
 
@@ -161,14 +163,16 @@
         args.folder_size = utils.parse_human_to_lambda(utils.human_to_bytes, args.folder_size)
         folders = [d for d in folders if args.folder_size(d["size"])]
     return sorted(folders, key=sort_by(args))
 
 
 def bigdirs() -> None:
     args = parse_args()
+    history.create(args)
+
     tbl = get_table(args)
     tbl = process_bigdirs(args, tbl)
 
     if args.limit:
         tbl = tbl[-int(args.limit) :]
 
     tbl = utils.list_dict_filter_bool(tbl, keep_0=False)
```

### Comparing `xklb-1.31.9/xklb/scripts/block.py` & `xklb-2.1.2/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/scripts/christen.py` & `xklb-2.1.2/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/scripts/cluster_sort.py` & `xklb-2.1.2/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/scripts/copy_play_counts.py` & `xklb-2.1.2/xklb/scripts/copy_play_counts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 from pathlib import Path
 
-from xklb import db, usage, utils
+from xklb import db, history, usage, utils
+from xklb.scripts.dedupe_db import dedupe_rows
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library copy-play-counts", usage=usage.copy_play_counts)
     parser.add_argument("database")
     parser.add_argument("source_dbs", nargs="+")
@@ -23,50 +24,75 @@
 
     return args
 
 
 def copy_play_count(args, source_db) -> None:
     args.db.attach("src", Path(source_db).resolve())
 
-    copy_counts = args.db.query(
-        """
-        SELECT
-            *
-        FROM
-            src.media
-        WHERE
-            src.media.play_count > 0
-            or
-            src.media.playhead > 0
-        """,
-    )
-
-    modified_row_count = 0
-    with args.db.conn:
-        for d in copy_counts:
-            renamed_path = d["path"].replace(args.source_prefix, args.target_prefix, 1)
-            log.debug(renamed_path)
-
-            sql = """
-            UPDATE
-                main.media
-            SET
-                play_count = :play_count
-                , time_played = :time_played
-                , playhead = :playhead
-            WHERE
-                main.media.path = :renamed_path
-            """
-            cursor = args.db.conn.execute(sql, {**d, "renamed_path": renamed_path})
-            modified_row_count += cursor.rowcount
-
-    log.info("Updated %s rows", modified_row_count)
+    copy_counts = []
+    try:
+        # TODO delete after 2024-06-01
+        old_schema = list(
+            args.db.query(
+                """
+                SELECT
+                    path, play_count, time_played, playhead
+                FROM
+                    src.media
+                WHERE
+                    src.media.play_count > 0
+                    OR
+                    src.media.playhead > 0
+                """,
+            ),
+        )
+
+        new_schema = []
+        for d in old_schema:
+            if d["playhead"] is None or d["playhead"] == 0:
+                new_schema.append(
+                    {"path": d["path"], "time_played": d["time_played"], "playhead": d["playhead"], "done": False},
+                )
+            else:
+                for _ in range(d["playhead"]):
+                    new_schema.append(
+                        {"path": d["path"], "time_played": d["time_played"], "playhead": d["playhead"], "done": True},
+                    )
+        copy_counts.extend(new_schema)
+    except:
+        log.info("Old schema playhead could not be read")
+
+    try:
+        copy_counts.extend(
+            list(
+                args.db.query(
+                    """
+                SELECT
+                    path, time_played, playhead, done
+                FROM
+                    src.media m
+                JOIN src.history h on h.media_id = m.id
+                WHERE
+                    h.time_played > 0
+                    OR
+                    h.playhead > 0
+                """,
+                ),
+            ),
+        )
+    except:
+        log.info("New schema playhead could not be read")
+
+    for d in copy_counts:
+        renamed_path = d["path"].replace(args.source_prefix, args.target_prefix, 1)
+        history.add(args, [renamed_path], time_played=d["time_played"], playhead=d["playhead"], mark_done=d["done"])
 
 
 def copy_play_counts() -> None:
     args = parse_args()
     for s_db in args.source_dbs:
         copy_play_count(args, s_db)
+    dedupe_rows(args, "history", ["id"], ["media_id", "time_played"])
 
 
 if __name__ == "__main__":
     copy_play_counts()
```

### Comparing `xklb-1.31.9/xklb/scripts/dedupe.py` & `xklb-2.1.2/xklb/scripts/dedupe.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,15 +89,14 @@
         and m1.duration <= m2.duration + 4
         and m1.title = m2.title
         and m1.artist = m2.artist
         and m1.album = m2.album
     WHERE 1=1
         and m1.time_deleted = 0 and m2.time_deleted = 0
         and m1.audio_count > 0 and m2.audio_count > 0
-        and abs(m1.sparseness - 1) < 0.1
         and m1.title != ''
         and m1.artist != ''
         and m1.album != ''
     ORDER BY 1=1
         , length(m1.path)-length(REPLACE(m1.path, '/', '')) DESC
         , length(m1.path)-length(REPLACE(m1.path, '.', ''))
         , length(m1.path)
@@ -130,15 +129,14 @@
         and m1.extractor_id = m2.extractor_id
         and m1.duration >= m2.duration - 4
         and m1.duration <= m2.duration + 4
         and p1.extractor_key in (p2.extractor_key, 'Local')
         and m2.path != m1.path
     WHERE 1=1
         and m1.time_deleted = 0 and m2.time_deleted = 0
-        and abs(m1.sparseness - 1) < 0.1
         and m1.extractor_id != '' and p1.extractor_key != ''
     ORDER BY 1=1
         , m1.video_count > 0 DESC
         , m1.subtitle_count > 0 DESC
         , m1.audio_count DESC
         , length(m1.path)-length(REPLACE(m1.path, '/', '')) DESC
         , length(m1.path)-length(REPLACE(m1.path, '.', ''))
@@ -168,15 +166,14 @@
         media m1
     JOIN media m2 on 1=1
         and m2.path != m1.path
         and m1.duration >= m2.duration - 4
         and m1.duration <= m2.duration + 4
     WHERE 1=1
         and m1.time_deleted = 0 and m2.time_deleted = 0
-        and abs(m1.sparseness - 1) < 0.1
         and m1.title != '' and m1.uploader != ''
         and m1.title = m2.title and m1.uploader = m2.uploader
     ORDER BY 1=1
         , m1.video_count > 0 DESC
         , m1.subtitle_count > 0 DESC
         , m1.audio_count DESC
         , length(m1.path)-length(REPLACE(m1.path, '/', '')) DESC
```

### Comparing `xklb-1.31.9/xklb/scripts/dedupe_db.py` & `xklb-2.1.2/xklb/scripts/dedupe_db.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library dedupe-dbs", usage=usage.dedupe_db)
     parser.add_argument("--skip-upsert", action="store_true")
     parser.add_argument("--skip-0", action="store_true")
     parser.add_argument("--only-columns", action=utils.ArgparseList, help="Comma separated column names to upsert")
     parser.add_argument("--primary-keys", "--pk", action=utils.ArgparseList, help="Comma separated primary keys")
     parser.add_argument(
-        "--business-keys", "--bk", action=utils.ArgparseList, required=True, help="Comma separated business keys"
+        "--business-keys",
+        "--bk",
+        action=utils.ArgparseList,
+        required=True,
+        help="Comma separated business keys",
     )
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
     parser.add_argument("--verbose", "-v", action="count", default=0)
 
     parser.add_argument("database")
     parser.add_argument("table")
     args = parser.parse_intermixed_args()
@@ -27,14 +31,28 @@
     args.db = db.connect(args)
 
     log.info(utils.dict_filter_bool(args.__dict__))
 
     return args
 
 
+def dedupe_rows(args, tablename, primary_keys, business_keys):
+    with args.db.conn:
+        args.db.conn.execute(
+            f"""
+            DELETE FROM {tablename}
+            WHERE ({','.join(primary_keys)}) NOT IN (
+                SELECT {','.join(f"MIN({col}) AS {col}" for col in primary_keys)}
+                FROM {tablename}
+                GROUP BY {','.join(business_keys)}
+            )
+            """,
+        )
+
+
 def dedupe_db() -> None:
     args = parse_args()
 
     upsert_columns = args.only_columns
     target_columns = args.db[args.table].columns_dict
     if not args.primary_keys:
         args.primary_keys = list(o.name for o in args.db[args.table].columns if o.is_pk)
@@ -55,45 +73,36 @@
     if not args.skip_upsert:
         log.info("Upserting data in %s", ",".join(upsert_columns))
 
         for col in upsert_columns:
             data = list(
                 args.db.query(
                     f"""
-                    SELECT {','.join(args.business_keys + [col])}
+                    SELECT {','.join([*args.business_keys, col])}
                     FROM {args.table}
                     WHERE {f'NULLIF({col}, 0)' if args.skip_0 else col} IS NOT NULL
                     AND ({','.join(args.business_keys)}) IN (
                         SELECT {','.join(args.business_keys)}
                         FROM {args.table}
                         WHERE {col} IS NULL
                     )
                     ORDER BY {','.join(args.primary_keys)}
-                    """
-                )
+                    """,
+                ),
             )
             log.info("%s (%s rows)", col, len(data))
 
             with args.db.conn:
-                gen_where_sql = lambda row: " AND ".join(
-                    [f"{key} = {args.db.quote(row[key])}" for key in args.business_keys]
-                )
-                gen_update_sql = (
-                    lambda row: f"UPDATE {args.table} SET {col} = {args.db.quote(row[col])} WHERE {gen_where_sql(row)};"
-                )
+
+                def gen_where_sql(row):
+                    return " AND ".join([f"{key} = {args.db.quote(row[key])}" for key in args.business_keys])
+
+                def gen_update_sql(row):
+                    return f"UPDATE {args.table} SET {col} = {args.db.quote(row[col])} WHERE {gen_where_sql(row)};"
+
                 args.db.conn.executescript("\n".join([gen_update_sql(row) for row in data]))
 
-    with args.db.conn:
-        args.db.conn.execute(
-            f"""
-            DELETE FROM {args.table}
-            WHERE ({','.join(args.primary_keys)}) NOT IN (
-                SELECT {','.join(f"MIN({col}) AS {col}" for col in args.primary_keys)}
-                FROM {args.table}
-                GROUP BY {','.join(args.business_keys)}
-            )
-            """
-        )
+    dedupe_rows(args, args.table, primary_keys=args.primary_keys, business_keys=args.business_keys)
 
 
 if __name__ == "__main__":
     dedupe_db()
```

### Comparing `xklb-1.31.9/xklb/scripts/download_status.py` & `xklb-2.1.2/xklb/scripts/download_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,36 +84,56 @@
 
 
 def download_status() -> None:
     args = parse_args()
     play_actions.parse_args_sort(args)
 
     if args.delete:
-        return delete_playlists(args, args.delete)
+        delete_playlists(args, args.delete)
+        return
 
     query, bindings = dl_extract.construct_query(args)
 
     count_paths = ""
     if "time_modified" in query:
         if args.safe:
             args.db.register_function(tube_backend.is_supported, deterministic=True)
-            count_paths = (
-                "count(*) FILTER(WHERE COALESCE(m.time_modified,0) = 0 and is_supported(path)) never_downloaded"
-            )
+            count_paths = "count(*) FILTER(WHERE COALESCE(time_modified,0) = 0 and is_supported(path)) never_downloaded"
         else:
-            count_paths = "count(*) FILTER(WHERE COALESCE(m.time_modified,0) = 0) never_downloaded"
+            count_paths = "count(*) FILTER(WHERE COALESCE(time_modified,0) = 0) never_downloaded"
 
     query = f"""select
         {count_paths}
         , extractor_key
         {', sum(duration) duration' if 'duration' in query else ''}
-        {', count(*) FILTER(WHERE COALESCE(m.time_modified,0) > 0 AND error IS NOT NULL) errors' if 'error' in query else ''}
+        {', count(*) FILTER(WHERE COALESCE(time_modified,0) > 0 AND error IS NOT NULL) errors' if 'error' in query else ''}
         {', group_concat(distinct error) error_descriptions' if 'error' in query and args.verbose >= 1 else ''}
-    from ({query}) m
+    from ({query})
     where 1=1
         and COALESCE(time_downloaded,0) = 0
         and COALESCE(time_deleted,0) = 0
     group by extractor_key
     order by never_downloaded"""
 
     printer(args, query, bindings)
-    return None
+
+    if "error" in db.columns(args, "media"):
+        query = """
+        select error, count(*) count
+        from media
+        where error is not null
+        group by 1
+        order by 2
+        """
+        errors = list(args.db.query(query))
+
+        common_errors = []
+        other_errors = []
+        for error in errors:
+            if error["count"] == 1:
+                other_errors.append(error)
+            else:
+                common_errors.append(error)
+
+        common_errors.append({"error": "Other", "count": len(other_errors)})
+        common_errors.append({"error": "Total", "count": sum(d["count"] for d in errors)})
+        print(tabulate(common_errors, tablefmt="fancy_grid", headers="keys", showindex=False))
```

### Comparing `xklb-1.31.9/xklb/scripts/history.py` & `xklb-2.1.2/xklb/scripts/history.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 
 from tabulate import tabulate
 
 from xklb import consts, db, player, usage, utils
+from xklb.history import create
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         "library history",
         usage=usage.history,
@@ -35,16 +36,16 @@
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
     parser.add_argument(
         "facet",
         metavar="facet",
         type=str.lower,
-        default="all",
-        const="all",
+        default="watching",
+        const="watching",
         nargs="?",
         help="One of: %(choices)s (default: %(default)s)",
     )
 
     args = parser.parse_args()
 
     args.facet = utils.partial_startswith(args.facet, consts.time_facets)
@@ -97,50 +98,57 @@
     LIMIT {args.limit or 5}
     """
     return list(args.db.query(query))
 
 
 def history() -> None:
     args = parse_args()
+    create(args)
 
     m_columns = args.db["media"].columns_dict
 
-    if args.facet.startswith(("all", "watching")):
+    if args.facet.startswith("watching"):
         print("Partially watched:")
         tbl = player.historical_usage(args, args.frequency, "time_played", "and coalesce(play_count, 0)=0")
         print_history(tbl)
         query = f"""SELECT
                 path
                 {', title' if 'title' in m_columns else ''}
                 {', duration' if 'duration' in m_columns else ''}
                 {', subtitle_count' if 'subtitle_count' in m_columns else ''}
-                {', time_played' if 'time_played' in m_columns else ''}
-                {', playhead' if 'playhead' in m_columns else ''}
-            FROM media
+                , MAX(h.time_played) time_played
+                , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
+                , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
+            FROM media m
+            LEFT JOIN history h on h.media_id = m.id
             WHERE coalesce(time_deleted, 0) = 0
                 and coalesce(playhead, 0) > 60
                 and coalesce(play_count, 0) = 0
+            GROUP BY m.id
             ORDER BY time_played desc, playhead desc
             LIMIT {args.limit or 5}
         """
         tbl = list(args.db.query(query))
         print_recent(tbl, "time_played")
 
-    elif args.facet.startswith(("all", "watched")):
+    elif args.facet.startswith("watched"):
         print("Finished watching:")
         tbl = player.historical_usage(args, args.frequency, "time_played", "and coalesce(play_count, 0)>0")
         print_history(tbl)
         query = f"""SELECT
                 path
                 {', title' if 'title' in m_columns else ''}
                 {', duration' if 'duration' in m_columns else ''}
                 {', subtitle_count' if 'subtitle_count' in m_columns else ''}
-                {', time_played' if 'time_played' in m_columns else ''}
-            FROM media
+                , MAX(h.time_played) time_played
+                , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
+            FROM media m
+            LEFT JOIN history h on h.media_id = m.id
             WHERE coalesce(play_count, 0)>0
+            GROUP BY m.id
             ORDER BY time_played desc, path
             LIMIT {args.limit or 5}
         """
         tbl = list(args.db.query(query))
         print_recent(tbl, "time_played")
 
     else:
```

### Comparing `xklb-1.31.9/xklb/scripts/merge_dbs.py` & `xklb-2.1.2/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/scripts/merge_online_local.py` & `xklb-2.1.2/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/scripts/move_list.py` & `xklb-2.1.2/xklb/scripts/move_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from copy import deepcopy
 from pathlib import Path
 from typing import Dict, List, Tuple
 
 import humanize
 from tabulate import tabulate
 
-from xklb import db, player, utils
+from xklb import db, player, usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library mv-list",
+        usage=usage.mv_list,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default="25")
     parser.add_argument("--lower", default=4, type=int, help="Number of files per folder lower limit")
     parser.add_argument("--upper", default=4000, type=int, help="Number of files per folder upper limit")
     parser.add_argument("--verbose", "-v", action="count", default=0)
```

### Comparing `xklb-1.31.9/xklb/scripts/optimize_db.py` & `xklb-2.1.2/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/scripts/playlists.py` & `xklb-2.1.2/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/scripts/redownload.py` & `xklb-2.1.2/xklb/scripts/redownload.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,14 @@
     print(f"Showing most recent {args.limit} deletions. Use -l to change this limit")
 
 
 def print_deleted(args, deleted_media) -> None:
     tbl = deepcopy(deleted_media)
     tbl = utils.list_dict_filter_bool(tbl, keep_0=False)
     tbl = utils.list_dict_filter_unique(tbl)
-    tbl = utils.list_dict_filter_keys(tbl, ["sparseness"])
     tbl = tbl[: int(args.limit)]
     tbl = utils.col_resize(tbl, "path", 25)
     tbl = utils.col_duration(tbl, "duration")
     tbl = utils.col_naturalsize(tbl, "size")
     for t in consts.TIME_COLUMNS:
         utils.col_naturaldate(tbl, t)
     print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
```

### Comparing `xklb-1.31.9/xklb/scripts/relmv.py` & `xklb-2.1.2/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/scripts/scatter.py` & `xklb-2.1.2/xklb/scripts/scatter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import argparse, random, tempfile
+import argparse, random, sys, tempfile
 from pathlib import Path
 from statistics import median
 from typing import Dict, List, Tuple, Union
 
 from humanize import naturalsize
 from tabulate import tabulate
 
@@ -13,25 +13,26 @@
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library scatter",
         usage=usage.scatter,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue")
+    parser.add_argument("--max-files-per-folder", "--max-files-per-directory", type=int)
     parser.add_argument("--policy", "-p")
     parser.add_argument("--group", "-g")
     parser.add_argument("--sort", "-s", default="random()", help="Sort files before moving")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--srcmounts", "-m", help="/mnt/d1:/mnt/d2")
 
     parser.add_argument("database")
     parser.add_argument(
         "relative_paths",
         nargs="+",
-        help="Paths to scatter, relative to the root of your mergerfs mount if using -m, any path substring is valid",
+        help="Paths to scatter; if using -m any path substring is valid (relative to the root of your mergerfs mount)",
     )
     args = parser.parse_args()
     args.db = db.connect(args)
 
     if args.srcmounts:
         args.srcmounts = [m.rstrip("\\/") for m in args.srcmounts.split(":")]
         if args.group is None:
@@ -40,14 +41,24 @@
             args.policy = "pfrd"
     else:
         if args.group is None:
             args.group = "count"
         if args.policy is None:
             args.policy = "rand"
 
+    if args.srcmounts and args.max_files_per_folder:
+        msg = (
+            "--max-files-per-folder has no affect during multi-device re-bin operation. Run as an independent operation"
+        )
+        raise ValueError(msg)
+
+    if args.srcmounts is None and args.policy not in ("rand", "used"):
+        msg = "Without srcmounts defined the only meaningful policies are: `rand` or `used`"
+        raise ValueError(msg)
+
     args.relative_paths = [p.lstrip(".") for p in args.relative_paths]
 
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
 
 
 def get_table(args) -> List[dict]:
@@ -137,15 +148,15 @@
 
         if len(disk_rebin) > 0:
             full_disks.append(disk_stat["mount"])
         to_rebin.extend(disk_rebin)
 
     if len(disk_stats) == len(full_disks):
         log.warning(
-            "No valid targets. You have selected an ideal state which is significantly different from the current path distribution.",
+            "No valid targets. You have selected an ideal state which is too similar or too different from the current path distribution.",
         )
         log.warning(
             'For this run, "full" source disks will be treated as valid targets. Otherwise, there is nothing to do.',
         )
         full_disks = []
 
     rebinned = []
@@ -184,22 +195,43 @@
 
 
 def scatter() -> None:
     args = parse_args()
 
     files = get_table(args)
 
+    if args.max_files_per_folder:
+        paths = [d["path"] for d in files]
+        untouched, rebinned = utils.rebin_folders(paths, args.max_files_per_folder)
+
+        tbl = []
+        for existing_path, new_path in rebinned:
+            tbl.append({"existing_path": existing_path, "new_path": new_path})
+            if len(tbl) > 10:
+                break
+        tbl = utils.col_resize(tbl, "existing_path", 20)
+        tbl = utils.col_resize(tbl, "new_path", 20)
+        print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+        print(len(rebinned), "files would be moved (only 10 shown)")
+        print(len(untouched), "files would not be moved")
+
+        if utils.confirm("Move files ?"):
+            utils.move_files(rebinned)
+        sys.exit(0)
+
     if args.srcmounts:
         disk_stats = utils.get_mount_stats(args.srcmounts)
+        assert all(p.exists() for p in args.srcmounts)
     else:
         log.warning(
             "srcmounts was not provided (-m) so provided paths will only be compared with each other. This might not be what you want!!",
         )
-        log.warning("In this setting paths should be absolute!--and the only valid policies are: `rand`, `used`.")
-        args.srcmounts = [str(Path(p).resolve()) for p in args.relative_paths]
+        paths = [Path(p).resolve() for p in args.relative_paths]
+        assert all(p.exists() for p in paths)
+        args.srcmounts = [str(p) for p in paths]
         disk_stats = get_rel_stats(args.srcmounts, files)
 
     if len(disk_stats) < 2:
         log.error(
             "\nThis tool does not make sense to use for only one path."
             " Define more paths or use the -m flag to define mountpoints which share the same subfolder (eg. mergerfs)",
         )
```

### Comparing `xklb-1.31.9/xklb/scripts/streaming_tab_loader.py` & `xklb-2.1.2/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/scripts/mining/data.py` & `xklb-2.1.2/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/scripts/mining/extract_links.py` & `xklb-2.1.2/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/scripts/mining/nouns.py` & `xklb-2.1.2/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/scripts/mining/pushshift.py` & `xklb-2.1.2/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.1.2/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/xklb/assets/kotobago.png` & `xklb-2.1.2/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/.gitignore` & `xklb-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/LICENSE` & `xklb-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/README.md` & `xklb-2.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.31.009)
+    xk media library subcommands (v2.1.002)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -203,14 +203,16 @@
     mining:
       lb reddit-selftext       db selftext external links -> db media table
       lb pushshift             Convert Pushshift jsonl.zstd -> reddit.db format (stdin)
       lb hnadd                 Create a hackernews database (this takes a few days)
 
       lb extract-links         Extract links from lists of web pages
 
+      lb mpv-watchlater        Import timestamps from mpv watchlater to history table
+
       lb cluster-sort          Lines -> sorted by sentence similarity groups (stdin)
       lb nouns                 Unstructured text -> compound nouns (stdin)
     
 
 </details>
 
 ## Examples
@@ -257,187 +259,43 @@
 Recently, this functionality has also been integrated into watch/listen subcommands so you could just do this:
 
     $ library watch --big-dirs ./my.db
     $ lb wt -B  # shorthand equivalent
 
 </details>
 
-
-### library mv-list: free up space
-
-<details><summary>Find candidates for moving to a different mount point</summary>
-
-The program takes a mount point and a xklb database file. If you don't have a database file you can create one like this:
-
-    $ library fsadd --filesystem d.db ~/d/
-
-But this should definitely also work with xklb audio and video databases:
-
-    $ library mv-list /mnt/d/ video.db
-
-The program will print a table with a sorted list of folders which are good candidates for moving.
-Candidates are determined by how many files are in the folder (so you don't spend hours waiting for folders with millions of tiny files to copy over).
-The default is 4 to 4000--but it can be adjusted via the --lower and --upper flags.
-
-    ...
-    ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
-    │ 4.0 GB   │       7 │ /mnt/d/71_Mealtime_Videos/unsorted/Miguel_4K/                                                                 │
-    ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
-    │ 5.7 GB   │      10 │ /mnt/d/71_Mealtime_Videos/unsorted/Bollywood_Premium/                                                         │
-    ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
-    │ 2.3 GB   │       4 │ /mnt/d/71_Mealtime_Videos/chief_wiggum/                                                                       │
-    ╘══════════╧═════════╧═══════════════════════════════════════════════════════════════════════════════════════════════════════════════╛
-    6702 other folders not shown
-
-    ██╗███╗░░██╗░██████╗████████╗██████╗░██╗░░░██╗░█████╗░████████╗██╗░█████╗░███╗░░██╗░██████╗
-    ██║████╗░██║██╔════╝╚══██╔══╝██╔══██╗██║░░░██║██╔══██╗╚══██╔══╝██║██╔══██╗████╗░██║██╔════╝
-    ██║██╔██╗██║╚█████╗░░░░██║░░░██████╔╝██║░░░██║██║░░╚═╝░░░██║░░░██║██║░░██║██╔██╗██║╚█████╗░
-    ██║██║╚████║░╚═══██╗░░░██║░░░██╔══██╗██║░░░██║██║░░██╗░░░██║░░░██║██║░░██║██║╚████║░╚═══██╗
-    ██║██║░╚███║██████╔╝░░░██║░░░██║░░██║╚██████╔╝╚█████╔╝░░░██║░░░██║╚█████╔╝██║░╚███║██████╔╝
-    ╚═╝╚═╝░░╚══╝╚═════╝░░░░╚═╝░░░╚═╝░░╚═╝░╚═════╝░░╚════╝░░░░╚═╝░░░╚═╝░╚════╝░╚═╝░░╚══╝╚═════╝░
-
-    Type "done" when finished
-    Type "more" to see more files
-    Paste a folder (and press enter) to toggle selection
-    Type "*" to select all files in the most recently printed table
-
-Then it will give you a prompt:
-
-    Paste a path:
-
-Wherein you can copy and paste paths you want to move from the table and the program will keep track for you.
-
-    Paste a path: /mnt/d/75_MovieQueue/720p/s11/
-    26 selected paths: 162.1 GB ; future free space: 486.9 GB
-
-You can also press the up arrow or paste it again to remove it from the list:
-
-    Paste a path: /mnt/d/75_MovieQueue/720p/s11/
-    25 selected paths: 159.9 GB ; future free space: 484.7 GB
-
-After you are done selecting folders you can press ctrl-d and it will save the list to a tmp file:
-
-    Paste a path: done
-
-        Folder list saved to /tmp/tmpa7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
-
-            rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmpa7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
-
-</details>
-
-
-### Scatter your data across disks (for [mergerfs](https://github.com/trapexit/mergerfs))
-
-<details><summary>Balance files across devices or filesystems</summary>
-
-    library scatter -h
-    usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --srcmounts SRCMOUNTS DATABASE RELATIVE_PATHS ...
-
-    Balance size
-
-        $ library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 ~/lb/fs/scatter.db subfolder/of/mergerfs/mnt
-        Current path distribution:
-        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
-        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
-        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
-        │ /mnt/d1 │        12793 │ 169.5 GB     │ 4.5 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d2 │        13226 │ 177.9 GB     │ 4.7 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d3 │            1 │ 717.6 kB     │ 717.6 kB      │ Jan 31         │ Jul 18 2022     │ yesterday      │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d4 │           82 │ 1.5 GB       │ 12.5 MB       │ Jan 31         │ Apr 22 2022     │ yesterday      │
-        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
-
-        Simulated path distribution:
-        5845 files should be moved
-        20257 files should not be moved
-        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
-        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
-        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
-        │ /mnt/d1 │         9989 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d2 │        10185 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d3 │         1186 │ 53.6 GB      │ 30.8 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d4 │         1216 │ 49.5 GB      │ 29.5 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d5 │         1146 │ 53.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d6 │         1198 │ 48.8 GB      │ 30.6 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d7 │         1182 │ 52.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
-        ### Move 1182 files to /mnt/d7 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpmr1628ij / /mnt/d7
-        ### Move 1198 files to /mnt/d6 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmp9yd75f6j / /mnt/d6
-        ### Move 1146 files to /mnt/d5 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpfrj141jj / /mnt/d5
-        ### Move 1185 files to /mnt/d3 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpqh2euc8n / /mnt/d3
-        ### Move 1134 files to /mnt/d4 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmphzb0gj92 / /mnt/d4
-
-    Balance device inodes for specific subfolder
-
-        $ library scatter -m /mnt/d1:/mnt/d2 ~/lb/fs/scatter.db subfolder --group count --sort 'size desc'
-
-    Scatter the most recent 100 files
-
-        $ library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' ~/lb/fs/scatter.db /
-
-    Scatter without mountpoints (limited functionality; only good for balancing fs inodes)
-
-        $ library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
-
-
-    positional arguments:
-    database
-    relative_paths        Paths to scatter, relative to the root of your mergerfs mount; any path substring is valid
-
-    options:
-    -h, --help            show this help message and exit
-    --limit LIMIT, -L LIMIT, -l LIMIT, -queue LIMIT, --queue LIMIT
-    --policy POLICY, -p POLICY
-    --group GROUP, -g GROUP
-    --sort SORT, -s SORT  Sort files before moving
-    --usage, -u           Show disk usage
-    --verbose, -v
-    --srcmounts SRCMOUNTS, -m SRCMOUNTS
-                            /mnt/d1:/mnt/d2
-
-</details>
-
 ### Pipe to [mnamer](https://github.com/jkwill87/mnamer)
 
 <details><summary>Rename poorly named files</summary>
 
     pip install mnamer
     mnamer --movie-directory ~/d/70_Now_Watching/ --episode-directory ~/d/70_Now_Watching/ \
         --no-overwrite -b (library watch -p fd -s 'path : McCloud')
     library fsadd ~/d/70_Now_Watching/
 
 </details>
 
-### Music alarm clock (via termux crontab)
+### Music alarm clock
+
+<details><summary>via termux crontab</summary>
 
 Wake up to your own music
 
     30 7 * * * library listen ./audio.db
 
 Wake up to your own music _only when you are *not* home_ (computer on local-only IP)
 
     30 7 * * * timeout 0.4 nc -z 192.168.1.12 22 || library listen --random
 
 Wake up to your own music on your Chromecast speaker group _only when you are home_
 
     30 7 * * * ssh 192.168.1.12 library listen --cast --cast-to "Bedroom pair"
 
+</details>
+
 ### Pipe to [lowcharts](https://github.com/juan-leon/lowcharts)
 
 <details><summary>$ library watch -p f -col time_created | lowcharts timehist -w 80</summary>
 
     Matches: 445183.
     Each ∎ represents a count of 1896
     [2022-04-13 03:16:05] [151689] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
@@ -552,15 +410,15 @@
 
     Create a video database and read internal/external subtitle files into a searchable database:
         library fsadd --scan-subtitles tv.search.db ./tv/ ./movies/
 
     Decode media to check for corruption (slow):
         library fsadd --check-corrupt 100 tv.db ./tv/  # scan through 100 percent of each file to evaluate how corrupt it is (very slow)
         library fsadd --check-corrupt   1 tv.db ./tv/  # scan through 1 percent of each file to evaluate how corrupt it is (takes about one second per file)
-        library fsadd --check-corrupt   5 tv.db ./tv/  # scan through 1 percent of each file to evaluate how corrupt it is (takes about ten seconds per file)
+        library fsadd --check-corrupt   5 tv.db ./tv/  # scan through 5 percent of each file to evaluate how corrupt it is (takes about ten seconds per file)
 
         library fsadd --check-corrupt   5 --delete-corrupt 30 tv.db ./tv/  # scan 5 percent of each file to evaluate how corrupt it is, if 30 percent or more of those checks fail then the file is deleted
 
         nb: the behavior of delete-corrupt changes between full and partial scan
         library fsadd --check-corrupt  99 --delete-corrupt  1 tv.db ./tv/  # partial scan 99 percent of each file to evaluate how corrupt it is, if 1 percent or more of those checks fail then the file is deleted
         library fsadd --check-corrupt 100 --delete-corrupt  1 tv.db ./tv/  # full scan each file to evaluate how corrupt it is, if there is _any_ corruption then the file is deleted
 
@@ -1532,21 +1390,55 @@
     If --primary-keys is not provided table metadata primary keys will be used
     If --only-columns is not provided all non-primary and non-business key columns will be upserted
     If your duplicate rows contain exactly the same data in all the columns you can run with --skip-upsert to save a lot of time
 
 
 </details>
 
-<details><summary>Sort lines by similarity (cluster-sort)</summary>
+<details><summary>Sort lines of text by similarity (cluster-sort)</summary>
 
     $ library cluster-sort -h
     usage: library cluster-sort [input_path | stdin] [output_path | stdout]
 
     Group lines of text into sorted output
 
+    $ echo 'red apple
+    broccoli
+    yellow
+    green
+    orange apple
+    red apple' | library cluster-sort
+
+    orange apple
+    red apple
+    red apple
+    broccoli
+    green
+    yellow
+
+    $ echo 'red apple
+    broccoli
+    yellow
+    green
+    orange apple
+    red apple' | library cluster-sort --groups
+
+    [
+        {'common_prefix': '',
+        'grouped_paths': ['orange apple
+', 'red apple
+', 'red apple
+']},
+        {'common_prefix': '',
+        'grouped_paths': ['broccoli
+', 'green
+', 'yellow
+']}
+    ]
+
 
 </details>
 
 <details><summary>Move files preserving parent folder hierarchy (relmv)</summary>
 
     $ library relmv -h
     usage: library relmv [--dry-run] SOURCE ... DEST
```

### Comparing `xklb-1.31.9/pyproject.toml` & `xklb-2.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.31.9/PKG-INFO` & `xklb-2.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.31.9
+Version: 2.1.2
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -224,15 +224,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.31.009)
+    xk media library subcommands (v2.1.002)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -288,14 +288,16 @@
     mining:
       lb reddit-selftext       db selftext external links -> db media table
       lb pushshift             Convert Pushshift jsonl.zstd -> reddit.db format (stdin)
       lb hnadd                 Create a hackernews database (this takes a few days)
 
       lb extract-links         Extract links from lists of web pages
 
+      lb mpv-watchlater        Import timestamps from mpv watchlater to history table
+
       lb cluster-sort          Lines -> sorted by sentence similarity groups (stdin)
       lb nouns                 Unstructured text -> compound nouns (stdin)
     
 
 </details>
 
 ## Examples
@@ -342,187 +344,43 @@
 Recently, this functionality has also been integrated into watch/listen subcommands so you could just do this:
 
     $ library watch --big-dirs ./my.db
     $ lb wt -B  # shorthand equivalent
 
 </details>
 
-
-### library mv-list: free up space
-
-<details><summary>Find candidates for moving to a different mount point</summary>
-
-The program takes a mount point and a xklb database file. If you don't have a database file you can create one like this:
-
-    $ library fsadd --filesystem d.db ~/d/
-
-But this should definitely also work with xklb audio and video databases:
-
-    $ library mv-list /mnt/d/ video.db
-
-The program will print a table with a sorted list of folders which are good candidates for moving.
-Candidates are determined by how many files are in the folder (so you don't spend hours waiting for folders with millions of tiny files to copy over).
-The default is 4 to 4000--but it can be adjusted via the --lower and --upper flags.
-
-    ...
-    ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
-    │ 4.0 GB   │       7 │ /mnt/d/71_Mealtime_Videos/unsorted/Miguel_4K/                                                                 │
-    ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
-    │ 5.7 GB   │      10 │ /mnt/d/71_Mealtime_Videos/unsorted/Bollywood_Premium/                                                         │
-    ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
-    │ 2.3 GB   │       4 │ /mnt/d/71_Mealtime_Videos/chief_wiggum/                                                                       │
-    ╘══════════╧═════════╧═══════════════════════════════════════════════════════════════════════════════════════════════════════════════╛
-    6702 other folders not shown
-
-    ██╗███╗░░██╗░██████╗████████╗██████╗░██╗░░░██╗░█████╗░████████╗██╗░█████╗░███╗░░██╗░██████╗
-    ██║████╗░██║██╔════╝╚══██╔══╝██╔══██╗██║░░░██║██╔══██╗╚══██╔══╝██║██╔══██╗████╗░██║██╔════╝
-    ██║██╔██╗██║╚█████╗░░░░██║░░░██████╔╝██║░░░██║██║░░╚═╝░░░██║░░░██║██║░░██║██╔██╗██║╚█████╗░
-    ██║██║╚████║░╚═══██╗░░░██║░░░██╔══██╗██║░░░██║██║░░██╗░░░██║░░░██║██║░░██║██║╚████║░╚═══██╗
-    ██║██║░╚███║██████╔╝░░░██║░░░██║░░██║╚██████╔╝╚█████╔╝░░░██║░░░██║╚█████╔╝██║░╚███║██████╔╝
-    ╚═╝╚═╝░░╚══╝╚═════╝░░░░╚═╝░░░╚═╝░░╚═╝░╚═════╝░░╚════╝░░░░╚═╝░░░╚═╝░╚════╝░╚═╝░░╚══╝╚═════╝░
-
-    Type "done" when finished
-    Type "more" to see more files
-    Paste a folder (and press enter) to toggle selection
-    Type "*" to select all files in the most recently printed table
-
-Then it will give you a prompt:
-
-    Paste a path:
-
-Wherein you can copy and paste paths you want to move from the table and the program will keep track for you.
-
-    Paste a path: /mnt/d/75_MovieQueue/720p/s11/
-    26 selected paths: 162.1 GB ; future free space: 486.9 GB
-
-You can also press the up arrow or paste it again to remove it from the list:
-
-    Paste a path: /mnt/d/75_MovieQueue/720p/s11/
-    25 selected paths: 159.9 GB ; future free space: 484.7 GB
-
-After you are done selecting folders you can press ctrl-d and it will save the list to a tmp file:
-
-    Paste a path: done
-
-        Folder list saved to /tmp/tmpa7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
-
-            rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmpa7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
-
-</details>
-
-
-### Scatter your data across disks (for [mergerfs](https://github.com/trapexit/mergerfs))
-
-<details><summary>Balance files across devices or filesystems</summary>
-
-    library scatter -h
-    usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --srcmounts SRCMOUNTS DATABASE RELATIVE_PATHS ...
-
-    Balance size
-
-        $ library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 ~/lb/fs/scatter.db subfolder/of/mergerfs/mnt
-        Current path distribution:
-        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
-        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
-        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
-        │ /mnt/d1 │        12793 │ 169.5 GB     │ 4.5 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d2 │        13226 │ 177.9 GB     │ 4.7 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d3 │            1 │ 717.6 kB     │ 717.6 kB      │ Jan 31         │ Jul 18 2022     │ yesterday      │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d4 │           82 │ 1.5 GB       │ 12.5 MB       │ Jan 31         │ Apr 22 2022     │ yesterday      │
-        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
-
-        Simulated path distribution:
-        5845 files should be moved
-        20257 files should not be moved
-        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
-        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
-        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
-        │ /mnt/d1 │         9989 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d2 │        10185 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d3 │         1186 │ 53.6 GB      │ 30.8 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d4 │         1216 │ 49.5 GB      │ 29.5 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d5 │         1146 │ 53.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d6 │         1198 │ 48.8 GB      │ 30.6 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d7 │         1182 │ 52.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
-        ### Move 1182 files to /mnt/d7 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpmr1628ij / /mnt/d7
-        ### Move 1198 files to /mnt/d6 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmp9yd75f6j / /mnt/d6
-        ### Move 1146 files to /mnt/d5 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpfrj141jj / /mnt/d5
-        ### Move 1185 files to /mnt/d3 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpqh2euc8n / /mnt/d3
-        ### Move 1134 files to /mnt/d4 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmphzb0gj92 / /mnt/d4
-
-    Balance device inodes for specific subfolder
-
-        $ library scatter -m /mnt/d1:/mnt/d2 ~/lb/fs/scatter.db subfolder --group count --sort 'size desc'
-
-    Scatter the most recent 100 files
-
-        $ library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' ~/lb/fs/scatter.db /
-
-    Scatter without mountpoints (limited functionality; only good for balancing fs inodes)
-
-        $ library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
-
-
-    positional arguments:
-    database
-    relative_paths        Paths to scatter, relative to the root of your mergerfs mount; any path substring is valid
-
-    options:
-    -h, --help            show this help message and exit
-    --limit LIMIT, -L LIMIT, -l LIMIT, -queue LIMIT, --queue LIMIT
-    --policy POLICY, -p POLICY
-    --group GROUP, -g GROUP
-    --sort SORT, -s SORT  Sort files before moving
-    --usage, -u           Show disk usage
-    --verbose, -v
-    --srcmounts SRCMOUNTS, -m SRCMOUNTS
-                            /mnt/d1:/mnt/d2
-
-</details>
-
 ### Pipe to [mnamer](https://github.com/jkwill87/mnamer)
 
 <details><summary>Rename poorly named files</summary>
 
     pip install mnamer
     mnamer --movie-directory ~/d/70_Now_Watching/ --episode-directory ~/d/70_Now_Watching/ \
         --no-overwrite -b (library watch -p fd -s 'path : McCloud')
     library fsadd ~/d/70_Now_Watching/
 
 </details>
 
-### Music alarm clock (via termux crontab)
+### Music alarm clock
+
+<details><summary>via termux crontab</summary>
 
 Wake up to your own music
 
     30 7 * * * library listen ./audio.db
 
 Wake up to your own music _only when you are *not* home_ (computer on local-only IP)
 
     30 7 * * * timeout 0.4 nc -z 192.168.1.12 22 || library listen --random
 
 Wake up to your own music on your Chromecast speaker group _only when you are home_
 
     30 7 * * * ssh 192.168.1.12 library listen --cast --cast-to "Bedroom pair"
 
+</details>
+
 ### Pipe to [lowcharts](https://github.com/juan-leon/lowcharts)
 
 <details><summary>$ library watch -p f -col time_created | lowcharts timehist -w 80</summary>
 
     Matches: 445183.
     Each ∎ represents a count of 1896
     [2022-04-13 03:16:05] [151689] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
@@ -637,15 +495,15 @@
 
     Create a video database and read internal/external subtitle files into a searchable database:
         library fsadd --scan-subtitles tv.search.db ./tv/ ./movies/
 
     Decode media to check for corruption (slow):
         library fsadd --check-corrupt 100 tv.db ./tv/  # scan through 100 percent of each file to evaluate how corrupt it is (very slow)
         library fsadd --check-corrupt   1 tv.db ./tv/  # scan through 1 percent of each file to evaluate how corrupt it is (takes about one second per file)
-        library fsadd --check-corrupt   5 tv.db ./tv/  # scan through 1 percent of each file to evaluate how corrupt it is (takes about ten seconds per file)
+        library fsadd --check-corrupt   5 tv.db ./tv/  # scan through 5 percent of each file to evaluate how corrupt it is (takes about ten seconds per file)
 
         library fsadd --check-corrupt   5 --delete-corrupt 30 tv.db ./tv/  # scan 5 percent of each file to evaluate how corrupt it is, if 30 percent or more of those checks fail then the file is deleted
 
         nb: the behavior of delete-corrupt changes between full and partial scan
         library fsadd --check-corrupt  99 --delete-corrupt  1 tv.db ./tv/  # partial scan 99 percent of each file to evaluate how corrupt it is, if 1 percent or more of those checks fail then the file is deleted
         library fsadd --check-corrupt 100 --delete-corrupt  1 tv.db ./tv/  # full scan each file to evaluate how corrupt it is, if there is _any_ corruption then the file is deleted
 
@@ -1617,21 +1475,55 @@
     If --primary-keys is not provided table metadata primary keys will be used
     If --only-columns is not provided all non-primary and non-business key columns will be upserted
     If your duplicate rows contain exactly the same data in all the columns you can run with --skip-upsert to save a lot of time
 
 
 </details>
 
-<details><summary>Sort lines by similarity (cluster-sort)</summary>
+<details><summary>Sort lines of text by similarity (cluster-sort)</summary>
 
     $ library cluster-sort -h
     usage: library cluster-sort [input_path | stdin] [output_path | stdout]
 
     Group lines of text into sorted output
 
+    $ echo 'red apple
+    broccoli
+    yellow
+    green
+    orange apple
+    red apple' | library cluster-sort
+
+    orange apple
+    red apple
+    red apple
+    broccoli
+    green
+    yellow
+
+    $ echo 'red apple
+    broccoli
+    yellow
+    green
+    orange apple
+    red apple' | library cluster-sort --groups
+
+    [
+        {'common_prefix': '',
+        'grouped_paths': ['orange apple
+', 'red apple
+', 'red apple
+']},
+        {'common_prefix': '',
+        'grouped_paths': ['broccoli
+', 'green
+', 'yellow
+']}
+    ]
+
 
 </details>
 
 <details><summary>Move files preserving parent folder hierarchy (relmv)</summary>
 
     $ library relmv -h
     usage: library relmv [--dry-run] SOURCE ... DEST
```

