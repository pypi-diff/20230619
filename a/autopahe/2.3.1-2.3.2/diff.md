# Comparing `tmp/autopahe-2.3.1.tar.gz` & `tmp/autopahe-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopahe-2.3.1.tar", last modified: Mon Jun 19 20:43:17 2023, max compression
+gzip compressed data, was "autopahe-2.3.2.tar", last modified: Mon Jun 19 20:48:07 2023, max compression
```

## Comparing `autopahe-2.3.1.tar` & `autopahe-2.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:43:17.611632 autopahe-2.3.1/
--rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       62 2023-06-16 06:52:54.000000 autopahe-2.3.1/MANIFEST.in
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6399 2023-06-19 20:43:17.611632 autopahe-2.3.1/PKG-INFO
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     5746 2023-06-19 20:04:44.000000 autopahe-2.3.1/README.md
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:43:17.607633 autopahe-2.3.1/autopahe/
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:29:36.000000 autopahe-2.3.1/autopahe/__init__.py
--rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)    19663 2023-06-19 20:39:59.000000 autopahe-2.3.1/autopahe/auto_pahe.py
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     4392 2023-06-19 19:43:52.000000 autopahe-2.3.1/autopahe/kwikdown.py
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      248 2023-06-19 19:57:40.000000 autopahe-2.3.1/autopahe/test.py
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:43:17.607633 autopahe-2.3.1/autopahe.egg-info/
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6399 2023-06-19 20:43:17.000000 autopahe-2.3.1/autopahe.egg-info/PKG-INFO
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      337 2023-06-19 20:43:17.000000 autopahe-2.3.1/autopahe.egg-info/SOURCES.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        1 2023-06-19 20:43:17.000000 autopahe-2.3.1/autopahe.egg-info/dependency_links.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       53 2023-06-19 20:43:17.000000 autopahe-2.3.1/autopahe.egg-info/entry_points.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       95 2023-06-19 20:43:17.000000 autopahe-2.3.1/autopahe.egg-info/requires.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        9 2023-06-19 20:43:17.000000 autopahe-2.3.1/autopahe.egg-info/top_level.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       86 2023-06-16 07:47:47.000000 autopahe-2.3.1/pyproject.toml
--rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       98 2023-06-16 07:18:50.000000 autopahe-2.3.1/requirements.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       38 2023-06-19 20:43:17.611632 autopahe-2.3.1/setup.cfg
--rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)     1373 2023-06-19 20:43:08.000000 autopahe-2.3.1/setup.py
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:48:07.449403 autopahe-2.3.2/
+-rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       62 2023-06-16 06:52:54.000000 autopahe-2.3.2/MANIFEST.in
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6399 2023-06-19 20:48:07.449403 autopahe-2.3.2/PKG-INFO
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     5746 2023-06-19 20:04:44.000000 autopahe-2.3.2/README.md
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:48:07.449403 autopahe-2.3.2/autopahe/
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:29:36.000000 autopahe-2.3.2/autopahe/__init__.py
+-rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)    19696 2023-06-19 20:47:52.000000 autopahe-2.3.2/autopahe/auto_pahe.py
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     4392 2023-06-19 19:43:52.000000 autopahe-2.3.2/autopahe/kwikdown.py
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      248 2023-06-19 19:57:40.000000 autopahe-2.3.2/autopahe/test.py
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:48:07.449403 autopahe-2.3.2/autopahe.egg-info/
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6399 2023-06-19 20:48:07.000000 autopahe-2.3.2/autopahe.egg-info/PKG-INFO
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      337 2023-06-19 20:48:07.000000 autopahe-2.3.2/autopahe.egg-info/SOURCES.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        1 2023-06-19 20:48:07.000000 autopahe-2.3.2/autopahe.egg-info/dependency_links.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       53 2023-06-19 20:48:07.000000 autopahe-2.3.2/autopahe.egg-info/entry_points.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       95 2023-06-19 20:48:07.000000 autopahe-2.3.2/autopahe.egg-info/requires.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        9 2023-06-19 20:48:07.000000 autopahe-2.3.2/autopahe.egg-info/top_level.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       86 2023-06-16 07:47:47.000000 autopahe-2.3.2/pyproject.toml
+-rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       98 2023-06-16 07:18:50.000000 autopahe-2.3.2/requirements.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       38 2023-06-19 20:48:07.453403 autopahe-2.3.2/setup.cfg
+-rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)     1373 2023-06-19 20:48:05.000000 autopahe-2.3.2/setup.py
```

### Comparing `autopahe-2.3.1/PKG-INFO` & `autopahe-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopahe
-Version: 2.3.1
+Version: 2.3.2
 Summary: A python script to automate downloads from animepahe
 Home-page: https://github.com/haxsysgit/autopahe
 Author: Elenasulu Arinze
 Author-email: pentacker@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autopahe-2.3.1/README.md` & `autopahe-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `autopahe-2.3.1/autopahe/auto_pahe.py` & `autopahe-2.3.2/autopahe/auto_pahe.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         abt = soup.select('.anime-synopsis')
         return abt[0].text.strip()
 
 
 def download(arg = 1,barg:str = "firefox"):
     # using return value of the search function to get the page
     # using the json data from the page url to get page where the episodes to watch are
-
+    arg = int(arg)
     print()
 
     #session string of the stream episode
     episode_session = jsonpage_dict['data'][arg-1]['session']
     
     #stream page url format
     stream_page_url = f'https://animepahe.com/play/{session_id}/{episode_session}'
@@ -441,15 +441,16 @@
         
         
 
 
     
 
             
-def multi_download_verbose(eps: str):
+def multi_download_verbose(eps):
+    eps = str(eps)
     # given arg specifies '-' for range
     # New format for list comprehension  
     episodes = [
         num
         for segment in eps.split(",")
         for num in (
             range(int(segment.split("-")[0]), int(segment.split("-")[1]) + 1)
```

### Comparing `autopahe-2.3.1/autopahe/kwikdown.py` & `autopahe-2.3.2/autopahe/kwikdown.py`

 * *Files identical despite different names*

### Comparing `autopahe-2.3.1/autopahe.egg-info/PKG-INFO` & `autopahe-2.3.2/autopahe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopahe
-Version: 2.3.1
+Version: 2.3.2
 Summary: A python script to automate downloads from animepahe
 Home-page: https://github.com/haxsysgit/autopahe
 Author: Elenasulu Arinze
 Author-email: pentacker@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autopahe-2.3.1/setup.py` & `autopahe-2.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = 'autopahe',
-    version = '2.3.1',
+    version = '2.3.2',
     author_email="pentacker@gmail.com",
     description = "A python script to automate downloads from animepahe",
     url = "https://github.com/haxsysgit/autopahe",
     author = "Elenasulu Arinze",
     license = "MIT",
     py_modules = [
         'autopahe',
```

