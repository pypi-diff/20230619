# Comparing `tmp/phub-2.4.tar.gz` & `tmp/phub-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phub-2.4.tar", last modified: Sat Jun 17 18:24:15 2023, max compression
+gzip compressed data, was "phub-2.5.tar", last modified: Mon Jun 19 10:45:59 2023, max compression
```

## Comparing `phub-2.4.tar` & `phub-2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:24:15.157013 phub-2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-17 18:24:05.000000 phub-2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-17 18:24:15.157013 phub-2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-17 18:24:05.000000 phub-2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-17 18:24:05.000000 phub-2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-17 18:24:15.157013 phub-2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-17 18:24:05.000000 phub-2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:24:15.157013 phub-2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:24:15.157013 phub-2.4/src/phub/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-17 18:24:05.000000 phub-2.4/src/phub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17284 2023-06-17 18:24:05.000000 phub-2.4/src/phub/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-17 18:24:05.000000 phub-2.4/src/phub/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-17 18:24:05.000000 phub-2.4/src/phub/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-17 18:24:05.000000 phub-2.4/src/phub/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-17 18:24:05.000000 phub-2.4/src/phub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:24:15.157013 phub-2.4/src/phub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-17 18:24:15.000000 phub-2.4/src/phub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-17 18:24:15.000000 phub-2.4/src/phub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 18:24:15.000000 phub-2.4/src/phub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 18:24:15.000000 phub-2.4/src/phub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-17 18:24:15.000000 phub-2.4/src/phub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:45:59.780948 phub-2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-19 10:45:46.000000 phub-2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-19 10:45:59.780948 phub-2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-19 10:45:46.000000 phub-2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-19 10:45:46.000000 phub-2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-19 10:45:59.780948 phub-2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-19 10:45:46.000000 phub-2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:45:59.776949 phub-2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:45:59.780948 phub-2.5/src/phub/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-19 10:45:46.000000 phub-2.5/src/phub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17281 2023-06-19 10:45:46.000000 phub-2.5/src/phub/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-19 10:45:46.000000 phub-2.5/src/phub/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-19 10:45:46.000000 phub-2.5/src/phub/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-19 10:45:46.000000 phub-2.5/src/phub/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-19 10:45:46.000000 phub-2.5/src/phub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:45:59.780948 phub-2.5/src/phub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-19 10:45:59.000000 phub-2.5/src/phub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-19 10:45:59.000000 phub-2.5/src/phub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 10:45:59.000000 phub-2.5/src/phub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 10:45:59.000000 phub-2.5/src/phub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 10:45:59.000000 phub-2.5/src/phub.egg-info/top_level.txt
```

### Comparing `phub-2.4/LICENSE` & `phub-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `phub-2.4/PKG-INFO` & `phub-2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 2.4
+Version: 2.5
 Summary: An API for PornHub
 Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
```

### Comparing `phub-2.4/README.md` & `phub-2.5/README.md`

 * *Files identical despite different names*

### Comparing `phub-2.4/setup.cfg` & `phub-2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phub
-version = 2.4
+version = 2.5
 description = An API for PornHub
 author = Egsagon
 author_email = egsagon12@gmail.com
 url = https://github.com/Egsagon/PHUB/
 license = GPLv3
 license_file = LICENSE
 long_description = file: README.md
```

### Comparing `phub-2.4/src/phub/__init__.py` & `phub-2.5/src/phub/__init__.py`

 * *Files identical despite different names*

### Comparing `phub-2.4/src/phub/classes.py` & `phub-2.5/src/phub/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,25 +355,25 @@
         Positive and negative likes of the video.
         '''
         
         self._lazy()
         
         votes = {t.lower(): v for t, v in consts.regexes.video_likes(self.page)}
         return Like(votes['up'], votes['down'])
-    
+
     @cached_property
     def views(self) -> int:
         '''
         How many times the video has been watched.
         '''
-        
+
         self._lazy()
-        
+
         raw = consts.regexes.video_interactions(self.page)[0]
-        return int(json.loads(f'[{raw}]')[0]['userInteractionCount'].replace(' ', ''))
+        return int(json.loads(f'[{raw}]')[0]['userInteractionCount'].replace(' ', '').replace(',', ''))
     
     @cached_property
     def hotspots(self) -> list[int]:
         '''
         List of hotspots (in seconds) of the video.
         '''
```

### Comparing `phub-2.4/src/phub/consts.py` & `phub-2.5/src/phub/consts.py`

 * *Files identical despite different names*

### Comparing `phub-2.4/src/phub/core.py` & `phub-2.5/src/phub/core.py`

 * *Files identical despite different names*

### Comparing `phub-2.4/src/phub/parser.py` & `phub-2.5/src/phub/parser.py`

 * *Files identical despite different names*

### Comparing `phub-2.4/src/phub/utils.py` & `phub-2.5/src/phub/utils.py`

 * *Files identical despite different names*

### Comparing `phub-2.4/src/phub.egg-info/PKG-INFO` & `phub-2.5/src/phub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 2.4
+Version: 2.5
 Summary: An API for PornHub
 Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
```

