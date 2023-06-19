# Comparing `tmp/audiobook-tags-1.0.0.tar.gz` & `tmp/audiobook-tags-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiobook-tags-1.0.0.tar", last modified: Sat Jun 17 04:48:08 2023, max compression
+gzip compressed data, was "audiobook-tags-1.1.0.tar", last modified: Mon Jun 19 04:41:04 2023, max compression
```

## Comparing `audiobook-tags-1.0.0.tar` & `audiobook-tags-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 04:48:08.619668 audiobook-tags-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-17 04:47:59.000000 audiobook-tags-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-17 04:47:59.000000 audiobook-tags-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-17 04:48:08.619668 audiobook-tags-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-17 04:47:59.000000 audiobook-tags-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-17 04:48:08.619668 audiobook-tags-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-17 04:47:59.000000 audiobook-tags-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 04:48:08.615668 audiobook-tags-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 04:48:08.619668 audiobook-tags-1.0.0/src/audiobook_tags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-17 04:48:08.000000 audiobook-tags-1.0.0/src/audiobook_tags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-17 04:48:08.000000 audiobook-tags-1.0.0/src/audiobook_tags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 04:48:08.000000 audiobook-tags-1.0.0/src/audiobook_tags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-17 04:48:08.000000 audiobook-tags-1.0.0/src/audiobook_tags.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 04:48:08.000000 audiobook-tags-1.0.0/src/audiobook_tags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 04:48:08.000000 audiobook-tags-1.0.0/src/audiobook_tags.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:41:04.691847 audiobook-tags-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-19 04:40:52.000000 audiobook-tags-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 04:40:52.000000 audiobook-tags-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-19 04:41:04.691847 audiobook-tags-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-19 04:40:52.000000 audiobook-tags-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 04:41:04.691847 audiobook-tags-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-19 04:40:52.000000 audiobook-tags-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:41:04.691847 audiobook-tags-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:41:04.691847 audiobook-tags-1.1.0/src/audiobook_tags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-19 04:41:04.000000 audiobook-tags-1.1.0/src/audiobook_tags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-19 04:41:04.000000 audiobook-tags-1.1.0/src/audiobook_tags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 04:41:04.000000 audiobook-tags-1.1.0/src/audiobook_tags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-19 04:41:04.000000 audiobook-tags-1.1.0/src/audiobook_tags.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-19 04:41:04.000000 audiobook-tags-1.1.0/src/audiobook_tags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 04:41:04.000000 audiobook-tags-1.1.0/src/audiobook_tags.egg-info/top_level.txt
```

### Comparing `audiobook-tags-1.0.0/LICENSE.txt` & `audiobook-tags-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `audiobook-tags-1.0.0/PKG-INFO` & `audiobook-tags-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiobook-tags
-Version: 1.0.0
+Version: 1.1.0
 Summary: Fix mp3 tags to use in iTunes/iPhone audiobooks
 Home-page: https://andgineer.github.io/audiobook-tags/
 Author: Andrey Sorokin
 Author-email: andrey@sorokin.engineer
 Keywords: audiobook mp3-tags
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,37 +31,38 @@
 
 ## Usage
     audiobook-tags [-h] [--encoding ENCODING] [--extension EXTENSION] [--set-tag [SET_TAG ...]] [--track-num TRACK_NUM] [--title-prefix TITLE_PREFIX] [--dry] [folder]
 
     Fixes mp3 tags for iOS audiobooks.
 
     positional arguments:
-      folder                Folder to process, do not add file name.
+      folder                Folder to process. By default current folder.
 
     options:
       -h, --help            show this help message and exit
-      --encoding ENCODING   mp3 tags encoding. "none" if you do not need mp3 tags encoding fix.
-      --extension EXTENSION
-                            Files extension including dot, for example `.mp3`.
-      --set-tag [SET_TAG ...]
+      --mask MASK, -m MASK  Files mask. By default .mp3
+      --encoding ENCODING, -e ENCODING
+                            mp3 tags encoding. "none" if you do not need mp3 tags encoding fix. By default "cp1251".
+      --tag [SET_TAG ...], -t [SET_TAG ...]
                             Change mp3 tag to specified string. Format "tag-name/tag-value".
-      --track-num TRACK_NUM
+      --num TRACK_NUM, -n TRACK_NUM
                             Sort files and set mp3 tag `track_num`: TRACK_NUM=`name` - sort by names; TRACK_NUM=`tag-<TAG>` - sort by mp3 tag with name <TAG>.
-      --title-prefix TITLE_PREFIX
-                            Prefix each file title with the track number for the file.
-      --dry                 Dry run without changing files.
+      --prefix TITLE_PREFIX, -p TITLE_PREFIX
+                            Add prefix to title tags. By default `{track:04} - ` if `--num` and no prefix if not.
+      --dry, -d             Dry run without changing files.
 
 ## Example:
 
-    audiobook-tags --set-tag="album_artist/Юрий Заборовский (Ардис)" --track-num="name"
+    audiobook-tags --tag="album_artist/Юрий Заборовский (Ардис)" --num="name" --prefix=""
 
-- Convers all `.mp3` files in current folder and subfolders
+- converts all `.mp3` files in current folder and subfolders
 - fix encoding supposing that original encoding was `Windows 1251`
 - change tag album artist.
-- set `track_num` mp3 tag to file number as ordered by file name
+- set `track_num` mp3 tag to file number as ordered by file name.
+  But do not add the track number to the title (`--prefix="""`).
 
 # Development
 
 ### OS Dependencies
 
 #### MacOS
```

### Comparing `audiobook-tags-1.0.0/README.md` & `audiobook-tags-1.1.0/src/audiobook_tags.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: audiobook-tags
+Version: 1.1.0
+Summary: Fix mp3 tags to use in iTunes/iPhone audiobooks
+Home-page: https://andgineer.github.io/audiobook-tags/
+Author: Andrey Sorokin
+Author-email: andrey@sorokin.engineer
+Keywords: audiobook mp3-tags
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 ﻿[![Build Status](https://github.com/andgineer/itunes-audiobook-from-mp3/workflows/ci/badge.svg)](https://github.com/andgineer/itunes-audiobook-from-mp3/actions)
 # Audiobooks from mp3 with broken tags
 
 Fix mp3 files tags to convert them into iTunes/iPhone audiobooks..
 
 - Fixes sort order.
 - Supports messed encoding like cyrillic Win1251.
@@ -16,37 +31,38 @@
 
 ## Usage
     audiobook-tags [-h] [--encoding ENCODING] [--extension EXTENSION] [--set-tag [SET_TAG ...]] [--track-num TRACK_NUM] [--title-prefix TITLE_PREFIX] [--dry] [folder]
 
     Fixes mp3 tags for iOS audiobooks.
 
     positional arguments:
-      folder                Folder to process, do not add file name.
+      folder                Folder to process. By default current folder.
 
     options:
       -h, --help            show this help message and exit
-      --encoding ENCODING   mp3 tags encoding. "none" if you do not need mp3 tags encoding fix.
-      --extension EXTENSION
-                            Files extension including dot, for example `.mp3`.
-      --set-tag [SET_TAG ...]
+      --mask MASK, -m MASK  Files mask. By default .mp3
+      --encoding ENCODING, -e ENCODING
+                            mp3 tags encoding. "none" if you do not need mp3 tags encoding fix. By default "cp1251".
+      --tag [SET_TAG ...], -t [SET_TAG ...]
                             Change mp3 tag to specified string. Format "tag-name/tag-value".
-      --track-num TRACK_NUM
+      --num TRACK_NUM, -n TRACK_NUM
                             Sort files and set mp3 tag `track_num`: TRACK_NUM=`name` - sort by names; TRACK_NUM=`tag-<TAG>` - sort by mp3 tag with name <TAG>.
-      --title-prefix TITLE_PREFIX
-                            Prefix each file title with the track number for the file.
-      --dry                 Dry run without changing files.
+      --prefix TITLE_PREFIX, -p TITLE_PREFIX
+                            Add prefix to title tags. By default `{track:04} - ` if `--num` and no prefix if not.
+      --dry, -d             Dry run without changing files.
 
 ## Example:
 
-    audiobook-tags --set-tag="album_artist/Юрий Заборовский (Ардис)" --track-num="name"
+    audiobook-tags --tag="album_artist/Юрий Заборовский (Ардис)" --num="name" --prefix=""
 
-- Convers all `.mp3` files in current folder and subfolders
+- converts all `.mp3` files in current folder and subfolders
 - fix encoding supposing that original encoding was `Windows 1251`
 - change tag album artist.
-- set `track_num` mp3 tag to file number as ordered by file name
+- set `track_num` mp3 tag to file number as ordered by file name.
+  But do not add the track number to the title (`--prefix="""`).
 
 # Development
 
 ### OS Dependencies
 
 #### MacOS
```

### Comparing `audiobook-tags-1.0.0/setup.py` & `audiobook-tags-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `audiobook-tags-1.0.0/src/audiobook_tags.egg-info/PKG-INFO` & `audiobook-tags-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: audiobook-tags
-Version: 1.0.0
-Summary: Fix mp3 tags to use in iTunes/iPhone audiobooks
-Home-page: https://andgineer.github.io/audiobook-tags/
-Author: Andrey Sorokin
-Author-email: andrey@sorokin.engineer
-Keywords: audiobook mp3-tags
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 ﻿[![Build Status](https://github.com/andgineer/itunes-audiobook-from-mp3/workflows/ci/badge.svg)](https://github.com/andgineer/itunes-audiobook-from-mp3/actions)
 # Audiobooks from mp3 with broken tags
 
 Fix mp3 files tags to convert them into iTunes/iPhone audiobooks..
 
 - Fixes sort order.
 - Supports messed encoding like cyrillic Win1251.
@@ -31,37 +16,38 @@
 
 ## Usage
     audiobook-tags [-h] [--encoding ENCODING] [--extension EXTENSION] [--set-tag [SET_TAG ...]] [--track-num TRACK_NUM] [--title-prefix TITLE_PREFIX] [--dry] [folder]
 
     Fixes mp3 tags for iOS audiobooks.
 
     positional arguments:
-      folder                Folder to process, do not add file name.
+      folder                Folder to process. By default current folder.
 
     options:
       -h, --help            show this help message and exit
-      --encoding ENCODING   mp3 tags encoding. "none" if you do not need mp3 tags encoding fix.
-      --extension EXTENSION
-                            Files extension including dot, for example `.mp3`.
-      --set-tag [SET_TAG ...]
+      --mask MASK, -m MASK  Files mask. By default .mp3
+      --encoding ENCODING, -e ENCODING
+                            mp3 tags encoding. "none" if you do not need mp3 tags encoding fix. By default "cp1251".
+      --tag [SET_TAG ...], -t [SET_TAG ...]
                             Change mp3 tag to specified string. Format "tag-name/tag-value".
-      --track-num TRACK_NUM
+      --num TRACK_NUM, -n TRACK_NUM
                             Sort files and set mp3 tag `track_num`: TRACK_NUM=`name` - sort by names; TRACK_NUM=`tag-<TAG>` - sort by mp3 tag with name <TAG>.
-      --title-prefix TITLE_PREFIX
-                            Prefix each file title with the track number for the file.
-      --dry                 Dry run without changing files.
+      --prefix TITLE_PREFIX, -p TITLE_PREFIX
+                            Add prefix to title tags. By default `{track:04} - ` if `--num` and no prefix if not.
+      --dry, -d             Dry run without changing files.
 
 ## Example:
 
-    audiobook-tags --set-tag="album_artist/Юрий Заборовский (Ардис)" --track-num="name"
+    audiobook-tags --tag="album_artist/Юрий Заборовский (Ардис)" --num="name" --prefix=""
 
-- Convers all `.mp3` files in current folder and subfolders
+- converts all `.mp3` files in current folder and subfolders
 - fix encoding supposing that original encoding was `Windows 1251`
 - change tag album artist.
-- set `track_num` mp3 tag to file number as ordered by file name
+- set `track_num` mp3 tag to file number as ordered by file name.
+  But do not add the track number to the title (`--prefix="""`).
 
 # Development
 
 ### OS Dependencies
 
 #### MacOS
```

