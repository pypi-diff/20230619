# Comparing `tmp/etm-dgraham-5.1.1.tar.gz` & `tmp/etm-dgraham-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-5.1.1.tar", last modified: Sun Jun 18 12:29:26 2023, max compression
+gzip compressed data, was "etm-dgraham-5.1.2.tar", last modified: Mon Jun 19 09:51:53 2023, max compression
```

## Comparing `etm-dgraham-5.1.1.tar` & `etm-dgraham-5.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 12:29:26.467400 etm-dgraham-5.1.1/
--rw-r--r--   0 dag        (501) staff       (20)     2504 2023-06-18 12:29:18.000000 etm-dgraham-5.1.1/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.1.1/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   132529 2023-06-18 12:29:26.467184 etm-dgraham-5.1.1/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   131617 2023-06-18 11:28:27.000000 etm-dgraham-5.1.1/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.1.1/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.1.1/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 12:29:26.461023 etm-dgraham-5.1.1/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.1.1/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.1.1/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.1.1/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 12:29:26.463292 etm-dgraham-5.1.1/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.1.1/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.1.1/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-18 12:29:18.000000 etm-dgraham-5.1.1/etm/__version__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.1.1/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.1.1/etm/ical.py
--rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.1.1/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   284740 2023-06-18 12:29:18.000000 etm-dgraham-5.1.1/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    37916 2023-06-18 11:28:27.000000 etm-dgraham-5.1.1/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.1.1/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)   100088 2023-06-18 11:28:27.000000 etm-dgraham-5.1.1/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 12:29:26.465454 etm-dgraham-5.1.1/etm_dgraham.egg-info/
--rwxrwxrwx   0 dag        (501) staff       (20)   132529 2023-06-18 12:29:26.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-18 12:29:26.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-18 12:29:26.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-18 12:29:26.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-18 12:29:26.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-18 12:29:26.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.1.1/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.1.1/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.1.1/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.1.1/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.1.1/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.1.1/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-18 12:29:26.467451 etm-dgraham-5.1.1/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.1.1/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 12:29:26.465565 etm-dgraham-5.1.1/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.1.1/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 12:29:26.466617 etm-dgraham-5.1.1/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.1.1/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.1.1/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.1.1/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.1.1/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 09:51:53.891417 etm-dgraham-5.1.2/
+-rw-r--r--   0 dag        (501) staff       (20)     2495 2023-06-19 09:51:43.000000 etm-dgraham-5.1.2/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.1.2/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   132529 2023-06-19 09:51:53.891257 etm-dgraham-5.1.2/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   131617 2023-06-18 11:28:27.000000 etm-dgraham-5.1.2/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.1.2/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.1.2/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 09:51:53.883763 etm-dgraham-5.1.2/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.1.2/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.1.2/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.1.2/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 09:51:53.887358 etm-dgraham-5.1.2/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.1.2/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.1.2/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-19 09:51:43.000000 etm-dgraham-5.1.2/etm/__version__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.1.2/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.1.2/etm/ical.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.1.2/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   285036 2023-06-19 09:51:43.000000 etm-dgraham-5.1.2/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    37916 2023-06-18 11:28:27.000000 etm-dgraham-5.1.2/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.1.2/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   100087 2023-06-19 09:51:43.000000 etm-dgraham-5.1.2/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 09:51:53.889585 etm-dgraham-5.1.2/etm_dgraham.egg-info/
+-rwxrwxrwx   0 dag        (501) staff       (20)   132529 2023-06-19 09:51:53.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-19 09:51:53.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-19 09:51:53.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-19 09:51:53.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-19 09:51:53.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-19 09:51:53.000000 etm-dgraham-5.1.2/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.1.2/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.1.2/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.1.2/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.1.2/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.1.2/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.1.2/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-19 09:51:53.891454 etm-dgraham-5.1.2/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.1.2/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 09:51:53.889688 etm-dgraham-5.1.2/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.1.2/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 09:51:53.890794 etm-dgraham-5.1.2/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.1.2/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.1.2/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.1.2/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.1.2/utilities/open_in_mutt
```

### Comparing `etm-dgraham-5.1.1/CHANGES.txt` & `etm-dgraham-5.1.2/CHANGES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,55 @@
-Recent tagged changes as of 2023-06-18T08:29:16.450280-04:00:
-- 0 seconds ago (HEAD -> working, tag: 5.1.1) Daniel Graham
+Recent tagged changes as of 2023-06-19T05:51:42.133568-04:00:
+- 0 seconds ago (HEAD -> working, tag: 5.1.2) Daniel Graham
+    3483b69 2023-06-19 05:51:42 -0400
+    Tagged version 5.1.2.
+
+- 21 hours ago (tag: 5.1.1) Daniel Graham
     d0c733f 2023-06-18 08:29:16 -0400
     Tagged version 5.1.1.
 
-- 61 minutes ago (tag: 5.1.0) Daniel Graham
+- 22 hours ago (tag: 5.1.0) Daniel Graham
     ece86e8 2023-06-18 07:28:25 -0400
     Tagged version 5.1.0. Added ability to display completion history
     for tasks including skipped instead of finished instances.
 
-- 24 hours ago (tag: 5.0.12) Daniel Graham
+- 2 days ago (tag: 5.0.12) Daniel Graham
     c42576c 2023-06-17 08:57:03 -0400
     Tagged version 5.0.12.
 
-- 27 hours ago (tag: 5.0.11) Daniel Graham
+- 2 days ago (tag: 5.0.11) Daniel Graham
     e9228d2 2023-06-17 05:19:31 -0400
     Tagged version 5.0.11.
 
-- 27 hours ago (tag: 5.0.10) Daniel Graham
+- 2 days ago (tag: 5.0.10) Daniel Graham
     2e1f579 2023-06-17 05:05:32 -0400
     Tagged version 5.0.10.
 
-- 3 days ago (tag: 5.0.9) Daniel Graham
+- 4 days ago (tag: 5.0.9) Daniel Graham
     7f30e8b 2023-06-15 10:14:19 -0400
     Tagged version 5.0.9.
 
 - 5 days ago (tag: 5.0.8) Daniel Graham
     1f587d1 2023-06-13 20:17:48 -0400
     Tagged version 5.0.8. Only display and allow completion of jthe
     jobs of the oldest unfinished instance of a repeating task.
 
-- 10 days ago (tag: 5.0.7) Daniel Graham
+- 11 days ago (tag: 5.0.7) Daniel Graham
     b9eccc6 2023-06-08 08:38:27 -0400
     Tagged version 5.0.7.
 
-- 13 days ago (tag: 5.0.6) Daniel Graham
+- 2 weeks ago (tag: 5.0.6) Daniel Graham
     345ca4e 2023-06-05 12:41:31 -0400
     Tagged version 5.0.6.
 
-- 13 days ago (tag: 5.0.5) Daniel Graham
+- 2 weeks ago (tag: 5.0.5) Daniel Graham
     9273685 2023-06-05 06:28:25 -0400
     Tagged version 5.0.5.
 
-- 13 days ago (tag: 5.0.4) Daniel Graham
+- 2 weeks ago (tag: 5.0.4) Daniel Graham
     ea199ac 2023-06-05 06:02:56 -0400
     Tagged version 5.0.4.
 
 - 2 weeks ago (tag: 5.0.3) Daniel Graham
     e0a0d9e 2023-06-04 16:44:49 -0400
     Tagged version 5.0.3.
 
@@ -66,18 +70,14 @@
     b8fbc47 2023-05-27 13:45:19 -0400
     Tagged version 4.12.9.
 
 - 3 weeks ago (tag: 4.12.8) Daniel Graham
     b0316d5 2023-05-26 13:50:15 -0400
     Tagged version 4.12.8.
 
-- 3 weeks ago (tag: 4.12.7) Daniel Graham
+- 4 weeks ago (tag: 4.12.7) Daniel Graham
     442ff98 2023-05-25 13:53:52 -0400
     Tagged version 4.12.7.
 
 - 4 weeks ago (tag: 4.12.6) Daniel Graham
     3da7332 2023-05-23 14:01:37 -0400
     Tagged version 4.12.6.
-
-- 4 weeks ago (tag: 4.12.5) Daniel Graham
-    f0c24d8 2023-05-21 15:08:06 -0400
-    Tagged version 4.12.5.
```

### Comparing `etm-dgraham-5.1.1/PKG-INFO` & `etm-dgraham-5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.1.1
+Version: 5.1.2
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.1.1/README.md` & `etm-dgraham-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/bump.py` & `etm-dgraham-5.1.2/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/docs/index_konnections.md` & `etm-dgraham-5.1.2/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/docs/index_usedtime.md` & `etm-dgraham-5.1.2/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/docs/multiple_timers.md` & `etm-dgraham-5.1.2/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/etm/__main__.py` & `etm-dgraham-5.1.2/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/etm/data.py` & `etm-dgraham-5.1.2/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/etm/ical.py` & `etm-dgraham-5.1.2/etm/ical.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/etm/make_examples.py` & `etm-dgraham-5.1.2/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/etm/model.py` & `etm-dgraham-5.1.2/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -595,22 +595,23 @@
         self.update_item_hsh()
         goto = self.item_hsh.get('g')
         if goto:
             return True, goto
         else:
             return False, "does not have an @g goto entry"
 
-    def get_repetitions(self, num=5):
+    def get_repetitions(self):
         """
         Called with a row, we should have an doc_id and can use relevant
         as aft_dt.
         Called while editing, we won't have a row or doc_id and can use '@s'
         as aft_dt
         """
-        # self.update_item_hsh()
+        num = self.settings['num_repetitions']
+        self.update_item_hsh()
         item = self.item_hsh
         showing =  "Repetitions"
         if not ('s' in item and ('r' in item or '+' in item)):
             return showing, "not a repeating item"
         relevant = date_to_datetime(item['s'])
 
         pairs = [format_datetime(x[0])[1] for x in item_instances(item, relevant, num+1, False)]
@@ -1007,14 +1008,15 @@
         self.item_hsh = {'created': created}
         cur_hsh = {}
         cur_key = None
         msg = []
         for pos, (k, v) in self.pos_hsh.items():
             obj = self.object_hsh.get((k, v))
             if obj is None:
+                logger.debug(f"got None for {k}, {v}")
                 msg.append(f"bad entry for {k}: {v}")
                 return msg
                 # continue
             elif k in ['a', 'u', 'n', 't', 'k']:
                 self.item_hsh.setdefault(k, []).append(obj)
             elif k in ['rr', 'jj']:
                 if cur_hsh:
@@ -1053,27 +1055,31 @@
                     #FIXME
                     self.item_hsh['f'] = last
             else:
                 msg.extend(res)
         if self.item_hsh.get('z', None) not in [None, 'float']:
             del self.item_hsh['z']
         if msg:
+            msg = "\n".join(msg)
             logger.debug(f"{msg}")
 
         return msg
 
 
     def update_item_hsh(self):
         msg = self.check_item_hsh()
+        if msg:
+            logger.error(msg)
 
         links = self.item_hsh.get('k', [])
         if links:
             # make sure the doc_id refers to an actual document
             self.item_hsh['k'] = [x for x in links if self.db.contains(doc_id=x)]
 
+
         if self.is_modified and not msg:
             now = pendulum.now('local')
             if self.is_new:
                 # creating a new item or editing a copy of an existing item
                 self.item_hsh['created'] = now
                 if self.doc_id is None:
                     self.doc_id = self.db.insert(self.item_hsh)
@@ -1322,15 +1328,15 @@
         bad_lst = []
         completions = []
         # arg_lst will be a list of pendulum periods
         for arg in args:
             if not arg:
                 continue
             obj, rep  = self.do_completion(arg)
-            if obj:
+            if isinstance(obj, pendulum.Period):
                 obj_lst.append(obj)
                 rep_lst.append(rep)
             else:
                 all_ok = False
                 bad_lst.append(arg)
 
 
@@ -3025,15 +3031,17 @@
             showing = f"Completion History"
         relevant = res[-1][0]
         details = f"{item['itemtype']} {item['summary']}"
 
         pairs = [f"{x[1]} {format_datetime(x[0])[1]}" for x in res]
         starting = format_datetime(relevant.date())[1]
 
-        return  showing, f"through {starting} for\n{details}:\n  " + "\n  ".join(pairs)
+        ps = f"\n\nCompleted instances are marked with {FINISHED_CHAR}" if skip else ""
+
+        return  showing, f"through {starting} for\n{details}:\n  " + "\n  ".join(pairs) + ps
 
     def touch(self, row):
         res = self.get_row_details(row)
         if not res:
             return False
         doc_id, instance, job_id = res
         now = pendulum.now('local')
```

### Comparing `etm-dgraham-5.1.1/etm/options.py` & `etm-dgraham-5.1.2/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/etm/report.py` & `etm-dgraham-5.1.2/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/etm/view.py` & `etm-dgraham-5.1.2/etm/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -2403,15 +2403,15 @@
     if not res:
         return
     showing, reps = res
     show_message(showing, reps, 24)
 
 @bindings.add('c-r', filter=is_editing)
 def is_editing_reps(*event):
-    res = item.get_repetitions(5)
+    res = item.get_repetitions()
     if not res:
         return
     showing, reps = res
     show_message(showing, reps, 24)
 
 @bindings.add('P', filter=is_viewing_or_details & is_item_view & is_items_table)
 def toggle_pinned(*event):
```

### Comparing `etm-dgraham-5.1.1/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-5.1.2/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.1.1
+Version: 5.1.2
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.1.1/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-5.1.2/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-5.1.2/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/etmlogo.png` & `etm-dgraham-5.1.2/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/etmlogo_small.png` & `etm-dgraham-5.1.2/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/etmview_agenda.png` & `etm-dgraham-5.1.2/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/namedcolors.py` & `etm-dgraham-5.1.2/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/new.png` & `etm-dgraham-5.1.2/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/setup.py` & `etm-dgraham-5.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/test/test_parser.py` & `etm-dgraham-5.1.2/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/utilities/colons_to_slashes.py` & `etm-dgraham-5.1.2/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/utilities/etm_in` & `etm-dgraham-5.1.2/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/utilities/inbasket` & `etm-dgraham-5.1.2/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.1/utilities/open_in_mutt` & `etm-dgraham-5.1.2/utilities/open_in_mutt`

 * *Files identical despite different names*

