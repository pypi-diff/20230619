# Comparing `tmp/etm-dgraham-5.1.3.tar.gz` & `tmp/etm-dgraham-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-5.1.3.tar", last modified: Mon Jun 19 15:40:25 2023, max compression
+gzip compressed data, was "etm-dgraham-5.1.4.tar", last modified: Mon Jun 19 17:40:24 2023, max compression
```

## Comparing `etm-dgraham-5.1.3.tar` & `etm-dgraham-5.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 15:40:25.089937 etm-dgraham-5.1.3/
--rw-r--r--   0 dag        (501) staff       (20)     2493 2023-06-19 15:40:17.000000 etm-dgraham-5.1.3/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.1.3/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   132529 2023-06-19 15:40:25.089787 etm-dgraham-5.1.3/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   131617 2023-06-18 11:28:27.000000 etm-dgraham-5.1.3/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.1.3/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.1.3/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 15:40:25.081560 etm-dgraham-5.1.3/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.1.3/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.1.3/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.1.3/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 15:40:25.085417 etm-dgraham-5.1.3/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.1.3/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.1.3/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-19 15:40:17.000000 etm-dgraham-5.1.3/etm/__version__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.1.3/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.1.3/etm/ical.py
--rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.1.3/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   285956 2023-06-19 15:40:17.000000 etm-dgraham-5.1.3/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    37916 2023-06-18 11:28:27.000000 etm-dgraham-5.1.3/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.1.3/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)   100087 2023-06-19 09:51:43.000000 etm-dgraham-5.1.3/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 15:40:25.088178 etm-dgraham-5.1.3/etm_dgraham.egg-info/
--rwxrwxrwx   0 dag        (501) staff       (20)   132529 2023-06-19 15:40:25.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-19 15:40:25.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-19 15:40:25.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-19 15:40:25.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-19 15:40:25.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-19 15:40:25.000000 etm-dgraham-5.1.3/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.1.3/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.1.3/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.1.3/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.1.3/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.1.3/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.1.3/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-19 15:40:25.089971 etm-dgraham-5.1.3/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.1.3/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 15:40:25.088284 etm-dgraham-5.1.3/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.1.3/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 15:40:25.089310 etm-dgraham-5.1.3/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.1.3/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.1.3/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.1.3/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.1.3/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 17:40:24.970517 etm-dgraham-5.1.4/
+-rw-r--r--   0 dag        (501) staff       (20)     2491 2023-06-19 17:40:17.000000 etm-dgraham-5.1.4/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.1.4/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   132529 2023-06-19 17:40:24.970365 etm-dgraham-5.1.4/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   131617 2023-06-18 11:28:27.000000 etm-dgraham-5.1.4/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.1.4/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.1.4/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 17:40:24.962495 etm-dgraham-5.1.4/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.1.4/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.1.4/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.1.4/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 17:40:24.966120 etm-dgraham-5.1.4/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.1.4/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.1.4/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-19 17:40:17.000000 etm-dgraham-5.1.4/etm/__version__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.1.4/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.1.4/etm/ical.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.1.4/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   285975 2023-06-19 17:40:17.000000 etm-dgraham-5.1.4/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    37916 2023-06-18 11:28:27.000000 etm-dgraham-5.1.4/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.1.4/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   100087 2023-06-19 09:51:43.000000 etm-dgraham-5.1.4/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 17:40:24.968675 etm-dgraham-5.1.4/etm_dgraham.egg-info/
+-rwxrwxrwx   0 dag        (501) staff       (20)   132529 2023-06-19 17:40:24.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-19 17:40:24.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-19 17:40:24.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-19 17:40:24.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-19 17:40:24.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-19 17:40:24.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.1.4/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.1.4/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.1.4/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.1.4/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.1.4/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.1.4/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-19 17:40:24.970552 etm-dgraham-5.1.4/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.1.4/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 17:40:24.968784 etm-dgraham-5.1.4/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.1.4/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 17:40:24.969838 etm-dgraham-5.1.4/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.1.4/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.1.4/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.1.4/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.1.4/utilities/open_in_mutt
```

### Comparing `etm-dgraham-5.1.3/CHANGES.txt` & `etm-dgraham-5.1.4/CHANGES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-Recent tagged changes as of 2023-06-19T11:40:16.051733-04:00:
-- 0 seconds ago (HEAD -> working, tag: 5.1.3) Daniel Graham
+Recent tagged changes as of 2023-06-19T13:40:16.377730-04:00:
+- 0 seconds ago (HEAD -> working, tag: 5.1.4) Daniel Graham
+    84421ec 2023-06-19 13:40:16 -0400
+    Tagged version 5.1.4.
+
+- 2 hours ago (tag: 5.1.3) Daniel Graham
     c776097 2023-06-19 11:40:16 -0400
     Tagged version 5.1.3.
 
-- 6 hours ago (tag: 5.1.2) Daniel Graham
+- 8 hours ago (tag: 5.1.2) Daniel Graham
     3483b69 2023-06-19 05:51:42 -0400
     Tagged version 5.1.2.
 
-- 27 hours ago (tag: 5.1.1) Daniel Graham
+- 29 hours ago (tag: 5.1.1) Daniel Graham
     d0c733f 2023-06-18 08:29:16 -0400
     Tagged version 5.1.1.
 
-- 28 hours ago (tag: 5.1.0) Daniel Graham
+- 30 hours ago (tag: 5.1.0) Daniel Graham
     ece86e8 2023-06-18 07:28:25 -0400
     Tagged version 5.1.0. Added ability to display completion history
     for tasks including skipped instead of finished instances.
 
 - 2 days ago (tag: 5.0.12) Daniel Graham
     c42576c 2023-06-17 08:57:03 -0400
     Tagged version 5.0.12.
@@ -73,11 +77,7 @@
 - 3 weeks ago (tag: 4.12.9) Daniel Graham
     b8fbc47 2023-05-27 13:45:19 -0400
     Tagged version 4.12.9.
 
 - 3 weeks ago (tag: 4.12.8) Daniel Graham
     b0316d5 2023-05-26 13:50:15 -0400
     Tagged version 4.12.8.
-
-- 4 weeks ago (tag: 4.12.7) Daniel Graham
-    442ff98 2023-05-25 13:53:52 -0400
-    Tagged version 4.12.7.
```

### Comparing `etm-dgraham-5.1.3/PKG-INFO` & `etm-dgraham-5.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.1.3
+Version: 5.1.4
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.1.3/README.md` & `etm-dgraham-5.1.4/README.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/bump.py` & `etm-dgraham-5.1.4/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/docs/index_konnections.md` & `etm-dgraham-5.1.4/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/docs/index_usedtime.md` & `etm-dgraham-5.1.4/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/docs/multiple_timers.md` & `etm-dgraham-5.1.4/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/etm/__main__.py` & `etm-dgraham-5.1.4/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/etm/data.py` & `etm-dgraham-5.1.4/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/etm/ical.py` & `etm-dgraham-5.1.4/etm/ical.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/etm/make_examples.py` & `etm-dgraham-5.1.4/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/etm/model.py` & `etm-dgraham-5.1.4/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -3058,17 +3058,18 @@
         details = f"{item['itemtype']} {item['summary']}"
 
         pairs = [f"{x[2]} {format_datetime(x[0])[1]}{x[1]}" for x in res]
         starting = format_datetime(relevant.date())[1]
 
         ps = f"\n\nSkipped instances are marked with a {SKIPPED_CHAR}." if skip else "\n"
         pss = """
-Datetimes at which an instance was due
-are listed together with the period (+/-)
-from the completion until due datetime.
+Datetimes at which an instance was due are
+listed together with the period (+/-) from
+the completion until the due datetime in
+parentheses.
 """
 
         return  showing, f"through {starting} for\n{details}:\n  " + "\n  ".join(pairs) + ps + pss
 
     def touch(self, row):
         res = self.get_row_details(row)
         if not res:
```

### Comparing `etm-dgraham-5.1.3/etm/options.py` & `etm-dgraham-5.1.4/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/etm/report.py` & `etm-dgraham-5.1.4/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/etm/view.py` & `etm-dgraham-5.1.4/etm/view.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-5.1.4/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.1.3
+Version: 5.1.4
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.1.3/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-5.1.4/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-5.1.4/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/etmlogo.png` & `etm-dgraham-5.1.4/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/etmlogo_small.png` & `etm-dgraham-5.1.4/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/etmview_agenda.png` & `etm-dgraham-5.1.4/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/namedcolors.py` & `etm-dgraham-5.1.4/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/new.png` & `etm-dgraham-5.1.4/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/setup.py` & `etm-dgraham-5.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/test/test_parser.py` & `etm-dgraham-5.1.4/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/utilities/colons_to_slashes.py` & `etm-dgraham-5.1.4/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/utilities/etm_in` & `etm-dgraham-5.1.4/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/utilities/inbasket` & `etm-dgraham-5.1.4/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.3/utilities/open_in_mutt` & `etm-dgraham-5.1.4/utilities/open_in_mutt`

 * *Files identical despite different names*

