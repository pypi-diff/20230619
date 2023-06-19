# Comparing `tmp/autopahe-2.3.tar.gz` & `tmp/autopahe-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopahe-2.3.tar", last modified: Mon Jun 19 20:35:16 2023, max compression
+gzip compressed data, was "autopahe-2.3.1.tar", last modified: Mon Jun 19 20:43:17 2023, max compression
```

## Comparing `autopahe-2.3.tar` & `autopahe-2.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:35:16.434912 autopahe-2.3/
--rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       62 2023-06-16 06:52:54.000000 autopahe-2.3/MANIFEST.in
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6397 2023-06-19 20:35:16.434912 autopahe-2.3/PKG-INFO
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     5746 2023-06-19 20:04:44.000000 autopahe-2.3/README.md
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:35:16.422911 autopahe-2.3/autopahe/
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:29:36.000000 autopahe-2.3/autopahe/__init__.py
--rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)    19650 2023-06-19 20:29:25.000000 autopahe-2.3/autopahe/auto_pahe.py
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     4392 2023-06-19 19:43:52.000000 autopahe-2.3/autopahe/kwikdown.py
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      248 2023-06-19 19:57:40.000000 autopahe-2.3/autopahe/test.py
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:35:16.434912 autopahe-2.3/autopahe.egg-info/
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6397 2023-06-19 20:35:16.000000 autopahe-2.3/autopahe.egg-info/PKG-INFO
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      337 2023-06-19 20:35:16.000000 autopahe-2.3/autopahe.egg-info/SOURCES.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        1 2023-06-19 20:35:16.000000 autopahe-2.3/autopahe.egg-info/dependency_links.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       53 2023-06-19 20:35:16.000000 autopahe-2.3/autopahe.egg-info/entry_points.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       95 2023-06-19 20:35:16.000000 autopahe-2.3/autopahe.egg-info/requires.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        9 2023-06-19 20:35:16.000000 autopahe-2.3/autopahe.egg-info/top_level.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       86 2023-06-16 07:47:47.000000 autopahe-2.3/pyproject.toml
--rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       98 2023-06-16 07:18:50.000000 autopahe-2.3/requirements.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       38 2023-06-19 20:35:16.434912 autopahe-2.3/setup.cfg
--rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)     1371 2023-06-19 20:34:31.000000 autopahe-2.3/setup.py
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:43:17.611632 autopahe-2.3.1/
+-rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       62 2023-06-16 06:52:54.000000 autopahe-2.3.1/MANIFEST.in
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6399 2023-06-19 20:43:17.611632 autopahe-2.3.1/PKG-INFO
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     5746 2023-06-19 20:04:44.000000 autopahe-2.3.1/README.md
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:43:17.607633 autopahe-2.3.1/autopahe/
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:29:36.000000 autopahe-2.3.1/autopahe/__init__.py
+-rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)    19663 2023-06-19 20:39:59.000000 autopahe-2.3.1/autopahe/auto_pahe.py
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     4392 2023-06-19 19:43:52.000000 autopahe-2.3.1/autopahe/kwikdown.py
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      248 2023-06-19 19:57:40.000000 autopahe-2.3.1/autopahe/test.py
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:43:17.607633 autopahe-2.3.1/autopahe.egg-info/
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6399 2023-06-19 20:43:17.000000 autopahe-2.3.1/autopahe.egg-info/PKG-INFO
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      337 2023-06-19 20:43:17.000000 autopahe-2.3.1/autopahe.egg-info/SOURCES.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        1 2023-06-19 20:43:17.000000 autopahe-2.3.1/autopahe.egg-info/dependency_links.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       53 2023-06-19 20:43:17.000000 autopahe-2.3.1/autopahe.egg-info/entry_points.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       95 2023-06-19 20:43:17.000000 autopahe-2.3.1/autopahe.egg-info/requires.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        9 2023-06-19 20:43:17.000000 autopahe-2.3.1/autopahe.egg-info/top_level.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       86 2023-06-16 07:47:47.000000 autopahe-2.3.1/pyproject.toml
+-rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       98 2023-06-16 07:18:50.000000 autopahe-2.3.1/requirements.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       38 2023-06-19 20:43:17.611632 autopahe-2.3.1/setup.cfg
+-rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)     1373 2023-06-19 20:43:08.000000 autopahe-2.3.1/setup.py
```

### Comparing `autopahe-2.3/PKG-INFO` & `autopahe-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopahe
-Version: 2.3
+Version: 2.3.1
 Summary: A python script to automate downloads from animepahe
 Home-page: https://github.com/haxsysgit/autopahe
 Author: Elenasulu Arinze
 Author-email: pentacker@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autopahe-2.3/README.md` & `autopahe-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `autopahe-2.3/autopahe/auto_pahe.py` & `autopahe-2.3.1/autopahe/auto_pahe.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,31 +480,31 @@
     index(select_index)
     
     # summary info on the selected anime
     info = about()
     Banners.i_info(info)
     
     # Handling episode to download prompt
-    download_type = input("""
+    download_type = str(input("""
     Enter the type of download facilty you want
     
     1. s or single_download for single episode download
     2. md or multi_download for multi episode download
     3. v or md_verbose for a verbose variant of the md function[SLOW]
     4. i for more in -depth info on the options above 
     
-    >> """)
+    >> """))
     print("\n")
     ep_to_download = (input("    Enter episode(s) to download >> "))
     
     switch = {
-        1:download,
-        2:multi_download_optimized,
-        3:multi_download_verbose,
-        4:info,
+        "1":download,
+        "2":multi_download_optimized,
+        "3":multi_download_verbose,
+        "4":info,
         's':download,
         'md':multi_download_optimized,
         'v':multi_download_verbose,
         'i':info,
         'single_download':download,
         'multi_download':multi_download_optimized,
         'md_verbose':multi_download_verbose,
```

### Comparing `autopahe-2.3/autopahe/kwikdown.py` & `autopahe-2.3.1/autopahe/kwikdown.py`

 * *Files identical despite different names*

### Comparing `autopahe-2.3/autopahe.egg-info/PKG-INFO` & `autopahe-2.3.1/autopahe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopahe
-Version: 2.3
+Version: 2.3.1
 Summary: A python script to automate downloads from animepahe
 Home-page: https://github.com/haxsysgit/autopahe
 Author: Elenasulu Arinze
 Author-email: pentacker@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autopahe-2.3/setup.py` & `autopahe-2.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = 'autopahe',
-    version = '2.3',
+    version = '2.3.1',
     author_email="pentacker@gmail.com",
     description = "A python script to automate downloads from animepahe",
     url = "https://github.com/haxsysgit/autopahe",
     author = "Elenasulu Arinze",
     license = "MIT",
     py_modules = [
         'autopahe',
```

