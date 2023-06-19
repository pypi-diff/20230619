# Comparing `tmp/etm-dgraham-5.1.2.tar.gz` & `tmp/etm-dgraham-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-5.1.2.tar", last modified: Mon Jun 19 09:51:53 2023, max compression
+gzip compressed data, was "etm-dgraham-5.1.3.tar", last modified: Mon Jun 19 15:40:25 2023, max compression
```

## Comparing `etm-dgraham-5.1.2.tar` & `etm-dgraham-5.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 09:51:53.891417 etm-dgraham-5.1.2/
--rw-r--r--   0 dag        (501) staff       (20)     2495 2023-06-19 09:51:43.000000 etm-dgraham-5.1.2/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.1.2/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   132529 2023-06-19 09:51:53.891257 etm-dgraham-5.1.2/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   131617 2023-06-18 11:28:27.000000 etm-dgraham-5.1.2/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.1.2/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.1.2/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 09:51:53.883763 etm-dgraham-5.1.2/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.1.2/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.1.2/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.1.2/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 09:51:53.887358 etm-dgraham-5.1.2/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.1.2/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.1.2/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-19 09:51:43.000000 etm-dgraham-5.1.2/etm/__version__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.1.2/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.1.2/etm/ical.py
--rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.1.2/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   285036 2023-06-19 09:51:43.000000 etm-dgraham-5.1.2/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    37916 2023-06-18 11:28:27.000000 etm-dgraham-5.1.2/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.1.2/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)   100087 2023-06-19 09:51:43.000000 etm-dgraham-5.1.2/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 09:51:53.889585 etm-dgraham-5.1.2/etm_dgraham.egg-info/
--rwxrwxrwx   0 dag        (501) staff       (20)   132529 2023-06-19 09:51:53.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-19 09:51:53.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-19 09:51:53.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-19 09:51:53.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-19 09:51:53.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-19 09:51:53.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.1.2/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.1.2/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.1.2/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.1.2/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.1.2/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.1.2/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-19 09:51:53.891454 etm-dgraham-5.1.2/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.1.2/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 09:51:53.889688 etm-dgraham-5.1.2/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.1.2/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 09:51:53.890794 etm-dgraham-5.1.2/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.1.2/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.1.2/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.1.2/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.1.2/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 15:40:25.089937 etm-dgraham-5.1.3/
+-rw-r--r--   0 dag        (501) staff       (20)     2493 2023-06-19 15:40:17.000000 etm-dgraham-5.1.3/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.1.3/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   132529 2023-06-19 15:40:25.089787 etm-dgraham-5.1.3/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   131617 2023-06-18 11:28:27.000000 etm-dgraham-5.1.3/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.1.3/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.1.3/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 15:40:25.081560 etm-dgraham-5.1.3/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.1.3/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.1.3/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.1.3/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 15:40:25.085417 etm-dgraham-5.1.3/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.1.3/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.1.3/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-19 15:40:17.000000 etm-dgraham-5.1.3/etm/__version__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.1.3/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.1.3/etm/ical.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.1.3/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   285956 2023-06-19 15:40:17.000000 etm-dgraham-5.1.3/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    37916 2023-06-18 11:28:27.000000 etm-dgraham-5.1.3/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.1.3/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   100087 2023-06-19 09:51:43.000000 etm-dgraham-5.1.3/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 15:40:25.088178 etm-dgraham-5.1.3/etm_dgraham.egg-info/
+-rwxrwxrwx   0 dag        (501) staff       (20)   132529 2023-06-19 15:40:25.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-19 15:40:25.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-19 15:40:25.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-19 15:40:25.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-19 15:40:25.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-19 15:40:25.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.1.3/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.1.3/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.1.3/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.1.3/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.1.3/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.1.3/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-19 15:40:25.089971 etm-dgraham-5.1.3/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.1.3/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 15:40:25.088284 etm-dgraham-5.1.3/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.1.3/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 15:40:25.089310 etm-dgraham-5.1.3/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.1.3/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.1.3/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.1.3/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.1.3/utilities/open_in_mutt
```

### Comparing `etm-dgraham-5.1.2/CHANGES.txt` & `etm-dgraham-5.1.3/CHANGES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-Recent tagged changes as of 2023-06-19T05:51:42.133568-04:00:
-- 0 seconds ago (HEAD -> working, tag: 5.1.2) Daniel Graham
+Recent tagged changes as of 2023-06-19T11:40:16.051733-04:00:
+- 0 seconds ago (HEAD -> working, tag: 5.1.3) Daniel Graham
+    c776097 2023-06-19 11:40:16 -0400
+    Tagged version 5.1.3.
+
+- 6 hours ago (tag: 5.1.2) Daniel Graham
     3483b69 2023-06-19 05:51:42 -0400
     Tagged version 5.1.2.
 
-- 21 hours ago (tag: 5.1.1) Daniel Graham
+- 27 hours ago (tag: 5.1.1) Daniel Graham
     d0c733f 2023-06-18 08:29:16 -0400
     Tagged version 5.1.1.
 
-- 22 hours ago (tag: 5.1.0) Daniel Graham
+- 28 hours ago (tag: 5.1.0) Daniel Graham
     ece86e8 2023-06-18 07:28:25 -0400
     Tagged version 5.1.0. Added ability to display completion history
     for tasks including skipped instead of finished instances.
 
 - 2 days ago (tag: 5.0.12) Daniel Graham
     c42576c 2023-06-17 08:57:03 -0400
     Tagged version 5.0.12.
@@ -24,15 +28,15 @@
     2e1f579 2023-06-17 05:05:32 -0400
     Tagged version 5.0.10.
 
 - 4 days ago (tag: 5.0.9) Daniel Graham
     7f30e8b 2023-06-15 10:14:19 -0400
     Tagged version 5.0.9.
 
-- 5 days ago (tag: 5.0.8) Daniel Graham
+- 6 days ago (tag: 5.0.8) Daniel Graham
     1f587d1 2023-06-13 20:17:48 -0400
     Tagged version 5.0.8. Only display and allow completion of jthe
     jobs of the oldest unfinished instance of a repeating task.
 
 - 11 days ago (tag: 5.0.7) Daniel Graham
     b9eccc6 2023-06-08 08:38:27 -0400
     Tagged version 5.0.7.
@@ -73,11 +77,7 @@
 - 3 weeks ago (tag: 4.12.8) Daniel Graham
     b0316d5 2023-05-26 13:50:15 -0400
     Tagged version 4.12.8.
 
 - 4 weeks ago (tag: 4.12.7) Daniel Graham
     442ff98 2023-05-25 13:53:52 -0400
     Tagged version 4.12.7.
-
-- 4 weeks ago (tag: 4.12.6) Daniel Graham
-    3da7332 2023-05-23 14:01:37 -0400
-    Tagged version 4.12.6.
```

### Comparing `etm-dgraham-5.1.2/PKG-INFO` & `etm-dgraham-5.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.1.2
+Version: 5.1.3
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.1.2/README.md` & `etm-dgraham-5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/bump.py` & `etm-dgraham-5.1.3/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/docs/index_konnections.md` & `etm-dgraham-5.1.3/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/docs/index_usedtime.md` & `etm-dgraham-5.1.3/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/docs/multiple_timers.md` & `etm-dgraham-5.1.3/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/etm/__main__.py` & `etm-dgraham-5.1.3/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/etm/data.py` & `etm-dgraham-5.1.3/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/etm/ical.py` & `etm-dgraham-5.1.3/etm/ical.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/etm/make_examples.py` & `etm-dgraham-5.1.3/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/etm/model.py` & `etm-dgraham-5.1.3/etm/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,27 +116,29 @@
     'event':        '#90ee90',
     'available':    '#1e90ff',
     'waiting':      '#6495ed',
     'finished':     '#191970',
 })
 
 FINISHED_CHAR = '✓'
+SKIPPED_CHAR = '✗'
 UPDATE_CHAR = "𝕦"
 INBASKET_CHAR = "𝕚"
 KONNECT_CHAR = 'k'
 LINK_CHAR = 'g'
 PIN_CHAR = 'p'
 ELLIPSiS_CHAR = '…'
 LINEDOT = ' · '  # ܁ U+00B7 (middle dot)
 
 etmdir = None
 
 ETMFMT = "%Y%m%dT%H%M"
 ZERO = pendulum.duration(minutes=0)
 ONEMIN = pendulum.duration(minutes=1)
+ONESEC = pendulum.duration(seconds=1)
 DAY = pendulum.duration(days=1)
 
 
 WKDAYS_DECODE = {"{0}{1}".format(n, d): "{0}({1})".format(d, n) if n else d for d in ['MO', 'TU', 'WE', 'TH', 'FR', 'SA', 'SU'] for n in ['-4', '-3', '-2', '-1', '', '1', '2', '3', '4']}
 WKDAYS_ENCODE = {"{0}({1})".format(d, n): "{0}{1}".format(n, d) if n else d for d in ['MO', 'TU', 'WE', 'TH', 'FR', 'SA', 'SU'] for n in ['-4', '-3', '-2', '-1', '+1', '+2', '+3', '+4']}
 for wkd in ['MO', 'TU', 'WE', 'TH', 'FR', 'SA', 'SU']:
     WKDAYS_ENCODE[wkd] = wkd
@@ -1838,15 +1840,15 @@
 def format_duration(obj, short=False):
     """
     if short report only hours and minutes, else include weeks and days
     >>> td = pendulum.duration(weeks=1, days=2, hours=3, minutes=27)
     >>> format_duration(td)
     '1w2d3h27m'
     """
-    if not isinstance(obj, pendulum.Duration):
+    if not (isinstance(obj, pendulum.Duration) or isinstance(obj, pendulum.Period)):
         return None
     hours = obj.hours
     try:
         until =[]
         if obj.weeks:
             if short:
                 hours += obj.weeks * 7 * 24
@@ -1874,15 +1876,15 @@
         return None
 
 
 def status_duration(obj):
     """
     hours, minutes and tenths of minutes for display in the status bar
     """
-    if not isinstance(obj, pendulum.Duration):
+    if not (isinstance(obj, pendulum.Duration) or isinstance(obj, pendulum.Period)):
         return None
     hours = obj.hours
     try:
         until =[]
         if obj.weeks:
             hours += obj.weeks * 7 * 24
 
@@ -1911,15 +1913,15 @@
 def fmt_dur(obj):
     """
     From data.py - no rounding
     >>> td = pendulum.duration(weeks=1, days=2, hours=3, minutes=27)
     >>> format_duration(td)
     '1w2d3h27m'
     """
-    if not isinstance(obj, pendulum.Duration):
+    if not (isinstance(obj, pendulum.Duration) or isinstance(obj, pendulum.Period)):
         return None
     try:
         until =[]
         if obj.weeks:
             until.append(f"{obj.weeks}w")
         if obj.remaining_days:
             until.append(f"{obj.remaining_days}d")
@@ -1934,14 +1936,37 @@
         ret = "".join(until)
         return "".join(until)
     except Exception as e:
         print('format_duration', e)
         print(obj)
         return None
 
+def fmt_period(obj):
+    if not isinstance(obj, pendulum.Period):
+        return None
+    start = obj.start
+    end = obj.end
+    neg = end < start
+    diff = start - end if neg else end - start
+    until = []
+    days = diff.remaining_days
+    hours = diff.hours
+    minutes = diff.minutes
+    if neg:
+        until.append("-")
+    else:
+        until.append("+")
+    if days:
+        until.append(f"{days}d")
+    if hours:
+        until.append(f"{hours}h")
+    if minutes:
+        until.append(f"{minutes}m")
+    return "".join(until)
+
 
 def format_duration_list(obj_lst):
     try:
         return ", ".join([format_duration(x) for x in obj_lst])
     except Exception as e:
         logger.error(f"{obj_lst}: {e}")
 
@@ -3015,33 +3040,38 @@
         if 'h' not in item:
             return showing, "there is no history of completions"
 
         relevant = self.id2relevant.get(item_id)
         res = []
         skip = item.get('o', 'k') == 's'
         for c in item['h']:
-            if skip and c.start == c.end:
-                res.append((c.end, ' '))
+            if skip and c.start == c.end + ONEMIN:
+                res.append((c.end, "", SKIPPED_CHAR))
             else:
-                res.append((c.end, FINISHED_CHAR))
+                res.append((c.end, f" ({fmt_period(c)})", FINISHED_CHAR))
         res.sort() # pendulum.DateTime obj as first component
         if len(res) > num:
             showing = f"Completion History: last {num} of {len(res)}"
             res = res[-num:]
         else:
             showing = f"Completion History"
         relevant = res[-1][0]
         details = f"{item['itemtype']} {item['summary']}"
 
-        pairs = [f"{x[1]} {format_datetime(x[0])[1]}" for x in res]
+        pairs = [f"{x[2]} {format_datetime(x[0])[1]}{x[1]}" for x in res]
         starting = format_datetime(relevant.date())[1]
 
-        ps = f"\n\nCompleted instances are marked with {FINISHED_CHAR}" if skip else ""
+        ps = f"\n\nSkipped instances are marked with a {SKIPPED_CHAR}." if skip else "\n"
+        pss = """
+Datetimes at which an instance was due
+are listed together with the period (+/-)
+from the completion until due datetime.
+"""
 
-        return  showing, f"through {starting} for\n{details}:\n  " + "\n  ".join(pairs) + ps
+        return  showing, f"through {starting} for\n{details}:\n  " + "\n  ".join(pairs) + ps + pss
 
     def touch(self, row):
         res = self.get_row_details(row)
         if not res:
             return False
         doc_id, instance, job_id = res
         now = pendulum.now('local')
@@ -5732,15 +5762,15 @@
                 if item['itemtype'] == '-':
                     switch = item.get('o', 'k')
                     relevant = rset.after(today, inc=True)
                     if switch == 's':
                         if relevant and date_to_datetime(item['s']) < today:
                             cur = date_to_datetime(item['s'])
                             while cur < today:
-                                item.setdefault('h', []).append(pendulum.period(cur, cur))
+                                item.setdefault('h', []).append(pendulum.period(cur+ONEMIN, cur))
                                 cur = rset.after(cur, inc=False)
 
                             item['s'] = pendulum.instance(cur)
                             update_db(db, item.doc_id, item)
                     else: # k or p
                         relevant = rset.after(today, inc=True)
                         already_done = [x.end for x in item.get('h', [])]
```

### Comparing `etm-dgraham-5.1.2/etm/options.py` & `etm-dgraham-5.1.3/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/etm/report.py` & `etm-dgraham-5.1.3/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/etm/view.py` & `etm-dgraham-5.1.3/etm/view.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-5.1.3/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.1.2
+Version: 5.1.3
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.1.2/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-5.1.3/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-5.1.3/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/etmlogo.png` & `etm-dgraham-5.1.3/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/etmlogo_small.png` & `etm-dgraham-5.1.3/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/etmview_agenda.png` & `etm-dgraham-5.1.3/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/namedcolors.py` & `etm-dgraham-5.1.3/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/new.png` & `etm-dgraham-5.1.3/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/setup.py` & `etm-dgraham-5.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/test/test_parser.py` & `etm-dgraham-5.1.3/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/utilities/colons_to_slashes.py` & `etm-dgraham-5.1.3/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/utilities/etm_in` & `etm-dgraham-5.1.3/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/utilities/inbasket` & `etm-dgraham-5.1.3/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.2/utilities/open_in_mutt` & `etm-dgraham-5.1.3/utilities/open_in_mutt`

 * *Files identical despite different names*

