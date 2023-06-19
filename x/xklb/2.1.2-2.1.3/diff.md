# Comparing `tmp/xklb-2.1.2.tar.gz` & `tmp/xklb-2.1.3.tar.gz`

## Comparing `xklb-2.1.2.tar` & `xklb-2.1.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.1.2/.gitattributes
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 xklb-2.1.2/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.1.2/Windows.md
--rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-2.1.2/pdm.lock
--rw-r--r--   0        0        0    13086 2020-02-02 00:00:00.000000 xklb-2.1.2/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.1.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.1.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.1.2/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-2.1.2/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/__init__.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/books.py
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/consts.py
--rw-r--r--   0        0        0     8337 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/db.py
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/dl_config.py
--rw-r--r--   0        0        0    11904 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/dl_extract.py
--rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/fs_extract.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/gdl_extract.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/gui.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/history.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/hn_extract.py
--rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/lb.py
--rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/media.py
--rw-r--r--   0        0        0    25300 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/play_actions.py
--rw-r--r--   0        0        0    34352 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/player.py
--rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/playlists.py
--rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/praw_extract.py
--rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/search.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/subtitle.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/tabs_extract.py
--rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/tube_backend.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/tube_extract.py
--rw-r--r--   0        0        0    83144 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/usage.py
--rw-r--r--   0        0        0    38734 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.1.2/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.1.2/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.1.2/LICENSE
--rw-r--r--   0        0        0    84692 2020-02-02 00:00:00.000000 xklb-2.1.2/README.md
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-2.1.2/pyproject.toml
--rw-r--r--   0        0        0    88318 2020-02-02 00:00:00.000000 xklb-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.1.3/.gitattributes
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 xklb-2.1.3/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.1.3/Windows.md
+-rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-2.1.3/pdm.lock
+-rw-r--r--   0        0        0    13086 2020-02-02 00:00:00.000000 xklb-2.1.3/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.1.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.1.3/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-2.1.3/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/books.py
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/consts.py
+-rw-r--r--   0        0        0     8337 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/db.py
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/dl_config.py
+-rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/gui.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/history.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/hn_extract.py
+-rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/lb.py
+-rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/media.py
+-rw-r--r--   0        0        0    25300 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/play_actions.py
+-rw-r--r--   0        0        0    34425 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/player.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/playlists.py
+-rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/subtitle.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/tube_extract.py
+-rw-r--r--   0        0        0    83144 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/usage.py
+-rw-r--r--   0        0        0    38734 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.1.3/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.1.3/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.1.3/LICENSE
+-rw-r--r--   0        0        0    84692 2020-02-02 00:00:00.000000 xklb-2.1.3/README.md
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0    88318 2020-02-02 00:00:00.000000 xklb-2.1.3/PKG-INFO
```

### Comparing `xklb-2.1.2/TODO` & `xklb-2.1.3/TODO`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/Windows.md` & `xklb-2.1.3/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/pdm.lock` & `xklb-2.1.3/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/readme.py` & `xklb-2.1.3/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-2.1.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-2.1.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/.github/workflows/push.yaml` & `xklb-2.1.3/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/av.py` & `xklb-2.1.3/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/books.py` & `xklb-2.1.3/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/consts.py` & `xklb-2.1.3/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/db.py` & `xklb-2.1.3/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/dl_config.py` & `xklb-2.1.3/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/dl_extract.py` & `xklb-2.1.3/xklb/dl_extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,20 +161,21 @@
                 and COALESCE(m.time_downloaded,0) = 0
                 and COALESCE(m.time_deleted,0) = 0
                 {'and COALESCE(p.time_deleted, 0) = 0' if 'time_deleted' in pl_columns else ''}
                 and m.path like "http%"
                 {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
                 {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
                 {" ".join(args.filter_sql)}
+            GROUP BY m.playlist_id
             ORDER BY 1=1
                 , COALESCE(m.time_modified, 0) = 0 DESC
                 , m.time_modified
                 {', ' + args.sort if args.sort else ''}
                 , random()
-        {LIMIT}
+            {LIMIT}
         """
     else:
         query = f"""select
                 m.path
                 {', m.title' if 'title' in m_columns else ''}
                 {', m.duration' if 'duration' in m_columns else ''}
                 {', m.time_created' if 'time_created' in m_columns else ''}
```

### Comparing `xklb-2.1.2/xklb/fs_extract.py` & `xklb-2.1.3/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/gdl_backend.py` & `xklb-2.1.3/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/gdl_extract.py` & `xklb-2.1.3/xklb/gdl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/gui.py` & `xklb-2.1.3/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/history.py` & `xklb-2.1.3/xklb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/hn_extract.py` & `xklb-2.1.3/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/lb.py` & `xklb-2.1.3/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/media.py` & `xklb-2.1.3/xklb/media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/play_actions.py` & `xklb-2.1.3/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/player.py` & `xklb-2.1.3/xklb/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,24 +395,26 @@
             return m
 
         candidate = new_candidate
         query = f"""
             SELECT
                 {args.select_sql}
                 , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
-            FROM {'media' if args.play_in_order >= consts.SIMILAR_NO_FILTER_NO_FTS else args.table}
+            FROM {'media' if args.play_in_order >= consts.SIMILAR_NO_FILTER_NO_FTS else args.table} m
             LEFT JOIN history h on h.media_id = m.id
             WHERE 1=1
                 and path like :candidate
                 {filter_args_sql(args, m_columns)}
                 {'' if args.play_in_order >= consts.SIMILAR_NO_FILTER else (" ".join(args.filter_sql) or '')}
                 {"and path not in ({})".format(",".join([f":ignore_path{i}" for i in range(len(ignore_paths))])) if len(ignore_paths) > 0 else ''}
+            GROUP BY m.id
             ORDER BY play_count, path
             LIMIT 1000
             """
+
         ignore_path_params = {f"ignore_path{i}": value for i, value in enumerate(ignore_paths)}
         bindings = {"candidate": candidate + "%", **ignore_path_params}
         if args.play_in_order >= consts.SIMILAR_NO_FILTER:
             if args.include or args.exclude:
                 bindings = {**bindings, "query": args.filter_bindings["query"]}
         else:
             bindings = {**bindings, **args.filter_bindings}
@@ -420,15 +422,15 @@
         similar_videos = list(args.db.query(query, bindings))
         log.debug(similar_videos)
 
         TOO_MANY_SIMILAR = 99
         if len(similar_videos) > TOO_MANY_SIMILAR or len(similar_videos) == total_media:
             return m
 
-        if len(similar_videos) > 0:
+        if len(similar_videos) > 1:
             commonprefix = os.path.commonprefix([d["path"] for d in similar_videos])
             log.debug(commonprefix)
             PREFIX_LENGTH_THRESHOLD = 3
             if len(Path(commonprefix).name) < PREFIX_LENGTH_THRESHOLD:
                 log.debug("Using commonprefix")
                 return m
 
@@ -452,14 +454,15 @@
             , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
         FROM {args.table} m
         LEFT JOIN history h on h.media_id = m.id
         WHERE 1=1
             and path != :path
             {filter_args_sql(args, m_columns)}
             {'' if args.related >= consts.RELATED_NO_FILTER else (" ".join(args.filter_sql) or '')}
+        GROUP BY m.id
         ORDER BY play_count
             , m.path like "http%"
             , {'rank' if 'sort' in args.defaults else f'ntile(1000) over (order by rank), {args.sort}'}
             , path
         {"LIMIT " + str(args.limit - 1) if args.limit else ""} {args.offset_sql}
         """
     bindings = {"path": m["path"]}
@@ -495,14 +498,15 @@
             , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
         FROM {args.table} m
         LEFT JOIN history h on h.media_id = m.id
         WHERE 1=1
             {filter_args_sql(args, m_columns)}
             {filter_paths}
             {'' if args.related >= consts.DIRS_NO_FILTER else (" ".join(args.filter_sql) or '')}
+        GROUP BY m.id
         ORDER BY play_count
             , m.path LIKE "http%"
             {'' if 'sort' in args.defaults else ', ' + args.sort}
             , path
         {"LIMIT 10000" if 'limit' in args.defaults else str(args.limit)} {args.offset_sql}
     """
     subpath_params = {f"subpath{i}": value + "%" for i, value in enumerate(dirs)}
```

### Comparing `xklb-2.1.2/xklb/playlists.py` & `xklb-2.1.3/xklb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/praw_extract.py` & `xklb-2.1.3/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/search.py` & `xklb-2.1.3/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/subtitle.py` & `xklb-2.1.3/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/tabs_actions.py` & `xklb-2.1.3/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/tabs_extract.py` & `xklb-2.1.3/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/tube_backend.py` & `xklb-2.1.3/xklb/tube_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,16 +138,16 @@
                         log.info("playlists.add2 %s", t.elapsed())
 
                     media.add(args, webpath, entry)  # type: ignore
                     log.info("media.add %s", t.elapsed())
 
                     added_media_count += 1
                     if added_media_count > 1:
-                        # sys.stdout.write("\033[K\r")
-                        print(f"[{playlist_path}] Added {added_media_count} media")  # , end="\r", flush=True)
+                        # sys.stdout.write("\033[K\r")  # this does not seem to be necessary
+                        print(f"[{playlist_path}] Added {added_media_count} media", end="\r", flush=True)
 
             return [], info
 
     with yt_dlp.YoutubeDL(ydl_opts) as ydl:
         ydl.add_post_processor(AddToArchivePP(), when="pre_process")
 
         log.info("yt-dlp initialized %s", t.elapsed())
```

### Comparing `xklb-2.1.2/xklb/tube_extract.py` & `xklb-2.1.3/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/usage.py` & `xklb-2.1.3/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/utils.py` & `xklb-2.1.3/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/bigdirs.py` & `xklb-2.1.3/xklb/scripts/bigdirs.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,14 +131,15 @@
             {', time_deleted' if 'time_deleted' in m_columns else ''}
             {', time_played' if 'time_played' in h_columns else ''}
         FROM media m
         LEFT JOIN history h on h.media_id = m.id
         WHERE 1=1
             {'and time_downloaded > 0' if 'time_downloaded' in m_columns else ''}
             {" ".join(args.filter_sql)}
+        GROUP BY m.id
         ORDER BY path
         """,
             args.filter_bindings,
         ),
     )
     return media
```

### Comparing `xklb-2.1.2/xklb/scripts/block.py` & `xklb-2.1.3/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/christen.py` & `xklb-2.1.3/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/cluster_sort.py` & `xklb-2.1.3/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/copy_play_counts.py` & `xklb-2.1.3/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/dedupe.py` & `xklb-2.1.3/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/dedupe_db.py` & `xklb-2.1.3/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/download_status.py` & `xklb-2.1.3/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/history.py` & `xklb-2.1.3/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/merge_dbs.py` & `xklb-2.1.3/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/merge_online_local.py` & `xklb-2.1.3/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/move_list.py` & `xklb-2.1.3/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/optimize_db.py` & `xklb-2.1.3/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/playback_control.py` & `xklb-2.1.3/xklb/scripts/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/playlists.py` & `xklb-2.1.3/xklb/scripts/playlists.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             {', p.time_deleted' if 'time_deleted' in pl_columns else ''}
             {', count(*) FILTER(WHERE play_count>0) play_count' if 'play_count' in m_columns else ''}
             {', sum(m.duration) duration' if 'duration' in m_columns else ''}
             {', sum(m.size) size' if 'size' in m_columns else ''}
             , count(*) count
         from media m
         left join ({query}) p on p.id = m.playlist_id
-        group by coalesce(p.path, "Playlist-less media")
+        group by m.playlist_id, coalesce(p.path, "Playlist-less media")
         order by count, p.path
         """
 
     if args.aggregate:
         query = f"""
         select
             'Aggregate of playlists' path
```

### Comparing `xklb-2.1.2/xklb/scripts/redownload.py` & `xklb-2.1.3/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/relmv.py` & `xklb-2.1.3/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/scatter.py` & `xklb-2.1.3/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/streaming_tab_loader.py` & `xklb-2.1.3/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/mining/data.py` & `xklb-2.1.3/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/mining/extract_links.py` & `xklb-2.1.3/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.1.3/xklb/scripts/mining/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/mining/nouns.py` & `xklb-2.1.3/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/mining/pushshift.py` & `xklb-2.1.3/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.1.3/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/xklb/assets/kotobago.png` & `xklb-2.1.3/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/.gitignore` & `xklb-2.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/LICENSE` & `xklb-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/README.md` & `xklb-2.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.1.002)
+    xk media library subcommands (v2.1.003)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-2.1.2/pyproject.toml` & `xklb-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.1.2/PKG-INFO` & `xklb-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 2.1.2
+Version: 2.1.3
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
-    xk media library subcommands (v2.1.002)
+    xk media library subcommands (v2.1.003)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

