# Comparing `tmp/pyrosexmod-0.2.0.tar.gz` & `tmp/pyrosexmod-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrosexmod-0.2.0.tar", last modified: Mon Jun 19 07:44:47 2023, max compression
+gzip compressed data, was "pyrosexmod-0.2.1.tar", last modified: Mon Jun 19 10:16:15 2023, max compression
```

## Comparing `pyrosexmod-0.2.0.tar` & `pyrosexmod-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:47.770302 pyrosexmod-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-19 07:44:30.000000 pyrosexmod-0.2.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-19 07:44:30.000000 pyrosexmod-0.2.0/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-19 07:44:30.000000 pyrosexmod-0.2.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-19 07:44:47.770302 pyrosexmod-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-19 07:44:30.000000 pyrosexmod-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:47.770302 pyrosexmod-0.2.0/pyrosexmod/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 07:44:30.000000 pyrosexmod-0.2.0/pyrosexmod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:47.770302 pyrosexmod-0.2.0/pyrosexmod/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-19 07:44:30.000000 pyrosexmod-0.2.0/pyrosexmod/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-19 07:44:30.000000 pyrosexmod-0.2.0/pyrosexmod/filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:47.770302 pyrosexmod-0.2.0/pyrosexmod/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 07:44:30.000000 pyrosexmod-0.2.0/pyrosexmod/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-19 07:44:30.000000 pyrosexmod-0.2.0/pyrosexmod/helpers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:47.770302 pyrosexmod-0.2.0/pyrosexmod/listen/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-19 07:44:30.000000 pyrosexmod-0.2.0/pyrosexmod/listen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-19 07:44:30.000000 pyrosexmod-0.2.0/pyrosexmod/listen/listen.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-19 07:44:30.000000 pyrosexmod-0.2.0/pyrosexmod/teledl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:47.770302 pyrosexmod-0.2.0/pyrosexmod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-19 07:44:30.000000 pyrosexmod-0.2.0/pyrosexmod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-19 07:44:30.000000 pyrosexmod-0.2.0/pyrosexmod/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:47.770302 pyrosexmod-0.2.0/pyrosexmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-19 07:44:47.000000 pyrosexmod-0.2.0/pyrosexmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-19 07:44:47.000000 pyrosexmod-0.2.0/pyrosexmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:44:47.000000 pyrosexmod-0.2.0/pyrosexmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 07:44:47.000000 pyrosexmod-0.2.0/pyrosexmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 07:44:47.000000 pyrosexmod-0.2.0/pyrosexmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 07:44:47.770302 pyrosexmod-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-19 07:44:30.000000 pyrosexmod-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:16:15.570881 pyrosexmod-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-19 10:16:03.000000 pyrosexmod-0.2.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-19 10:16:03.000000 pyrosexmod-0.2.1/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-19 10:16:03.000000 pyrosexmod-0.2.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-19 10:16:15.570881 pyrosexmod-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-19 10:16:03.000000 pyrosexmod-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:16:15.562880 pyrosexmod-0.2.1/pyrosexmod/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-19 10:16:03.000000 pyrosexmod-0.2.1/pyrosexmod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:16:15.566881 pyrosexmod-0.2.1/pyrosexmod/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-19 10:16:03.000000 pyrosexmod-0.2.1/pyrosexmod/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-19 10:16:03.000000 pyrosexmod-0.2.1/pyrosexmod/filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:16:15.566881 pyrosexmod-0.2.1/pyrosexmod/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 10:16:03.000000 pyrosexmod-0.2.1/pyrosexmod/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-19 10:16:03.000000 pyrosexmod-0.2.1/pyrosexmod/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:16:15.566881 pyrosexmod-0.2.1/pyrosexmod/listen/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-19 10:16:03.000000 pyrosexmod-0.2.1/pyrosexmod/listen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-19 10:16:03.000000 pyrosexmod-0.2.1/pyrosexmod/listen/listen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-19 10:16:03.000000 pyrosexmod-0.2.1/pyrosexmod/teledl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:16:15.570881 pyrosexmod-0.2.1/pyrosexmod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-19 10:16:03.000000 pyrosexmod-0.2.1/pyrosexmod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-19 10:16:03.000000 pyrosexmod-0.2.1/pyrosexmod/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:16:15.566881 pyrosexmod-0.2.1/pyrosexmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-19 10:16:15.000000 pyrosexmod-0.2.1/pyrosexmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-19 10:16:15.000000 pyrosexmod-0.2.1/pyrosexmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 10:16:15.000000 pyrosexmod-0.2.1/pyrosexmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 10:16:15.000000 pyrosexmod-0.2.1/pyrosexmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 10:16:15.000000 pyrosexmod-0.2.1/pyrosexmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 10:16:15.570881 pyrosexmod-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-19 10:16:03.000000 pyrosexmod-0.2.1/setup.py
```

### Comparing `pyrosexmod-0.2.0/COPYING` & `pyrosexmod-0.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.2.0/COPYING.lesser` & `pyrosexmod-0.2.1/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.2.0/NOTICE` & `pyrosexmod-0.2.1/NOTICE`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.2.0/PKG-INFO` & `pyrosexmod-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyrosexmod
-Version: 0.2.0
+Version: 0.2.1
 Summary: A monkeypatcher add-on for Pyrosex
-Home-page: https://github.com/OTHFamily/pyrosexmod
+Home-page: https://github.com/OnTheHerd/pyrosexmod
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyrosexmod-0.2.0/README.md` & `pyrosexmod-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.2.0/pyrosexmod/helpers/helpers.py` & `pyrosexmod-0.2.1/pyrosexmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.2.0/pyrosexmod/listen/listen.py` & `pyrosexmod-0.2.1/pyrosexmod/listen/listen.py`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.2.0/pyrosexmod/teledl.py` & `pyrosexmod-0.2.1/pyrosexmod/teledl.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import asyncio
-from yt_dlp import YoutubeDL
+from youtube_dlc import YoutubeDL
 
 
 async def download(link: str) -> str:
     loop = asyncio.get_running_loop()
     
     def video_dl():
         ydl_optssx = {
```

### Comparing `pyrosexmod-0.2.0/pyrosexmod.egg-info/PKG-INFO` & `pyrosexmod-0.2.1/pyrosexmod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyrosexmod
-Version: 0.2.0
+Version: 0.2.1
 Summary: A monkeypatcher add-on for Pyrosex
-Home-page: https://github.com/OTHFamily/pyrosexmod
+Home-page: https://github.com/OnTheHerd/pyrosexmod
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyrosexmod-0.2.0/setup.py` & `pyrosexmod-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     version=version,
     author="OTH",
     author_email="oth@pyrosex.org",
     license="LGPLv3+",
     description="A monkeypatcher add-on for Pyrosex",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/OTHFamily/pyrosexmod",
+    url="https://github.com/OnTheHerd/pyrosexmod",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    install_requires=["pyrosex>=0.0.3", "yt-dlp==2022.10.04"],
+    install_requires=["pyrosex>=0.0.3", "youtube-dlc"],
 )
```

