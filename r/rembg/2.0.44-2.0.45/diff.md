# Comparing `tmp/rembg-2.0.44.tar.gz` & `tmp/rembg-2.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rembg-2.0.44.tar", last modified: Mon Jun 19 20:26:06 2023, max compression
+gzip compressed data, was "rembg-2.0.45.tar", last modified: Mon Jun 19 21:03:30 2023, max compression
```

## Comparing `rembg-2.0.44.tar` & `rembg-2.0.45.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:26:06.078688 rembg-2.0.44/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-19 20:24:40.000000 rembg-2.0.44/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-19 20:24:40.000000 rembg-2.0.44/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-19 20:26:06.078688 rembg-2.0.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-06-19 20:24:40.000000 rembg-2.0.44/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-19 20:24:40.000000 rembg-2.0.44/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:26:06.082688 rembg-2.0.44/rembg/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-19 20:26:06.082688 rembg-2.0.44/rembg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/bg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:26:06.078688 rembg-2.0.44/rembg/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/commands/b_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/commands/i_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/commands/p_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/commands/s_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/session_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:26:06.078688 rembg-2.0.44/rembg/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/dis_anime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/dis_general_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/silueta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/u2net_cloth_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/u2net_human_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/u2netp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:26:06.078688 rembg-2.0.44/rembg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-19 20:26:05.000000 rembg-2.0.44/rembg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-19 20:26:06.000000 rembg-2.0.44/rembg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:26:05.000000 rembg-2.0.44/rembg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 20:26:05.000000 rembg-2.0.44/rembg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-19 20:26:05.000000 rembg-2.0.44/rembg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 20:26:05.000000 rembg-2.0.44/rembg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-19 20:26:06.082688 rembg-2.0.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-19 20:24:40.000000 rembg-2.0.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:26:06.078688 rembg-2.0.44/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-19 20:24:40.000000 rembg-2.0.44/tests/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-19 20:24:40.000000 rembg-2.0.44/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:03:30.914045 rembg-2.0.45/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-19 21:02:24.000000 rembg-2.0.45/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-19 21:02:24.000000 rembg-2.0.45/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-19 21:03:30.914045 rembg-2.0.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-06-19 21:02:24.000000 rembg-2.0.45/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-19 21:02:25.000000 rembg-2.0.45/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:03:30.914045 rembg-2.0.45/rembg/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-19 21:03:30.914045 rembg-2.0.45/rembg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:03:30.914045 rembg-2.0.45/rembg/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/commands/b_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/commands/i_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/commands/p_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/commands/s_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/session_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:03:30.914045 rembg-2.0.45/rembg/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/sessions/dis_anime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/sessions/dis_general_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/sessions/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/sessions/silueta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/sessions/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/sessions/u2net_cloth_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/sessions/u2net_human_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-19 21:02:25.000000 rembg-2.0.45/rembg/sessions/u2netp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:03:30.910045 rembg-2.0.45/rembg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-19 21:03:30.000000 rembg-2.0.45/rembg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-19 21:03:30.000000 rembg-2.0.45/rembg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:03:30.000000 rembg-2.0.45/rembg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 21:03:30.000000 rembg-2.0.45/rembg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-19 21:03:30.000000 rembg-2.0.45/rembg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 21:03:30.000000 rembg-2.0.45/rembg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-19 21:03:30.914045 rembg-2.0.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-19 21:02:25.000000 rembg-2.0.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:03:30.914045 rembg-2.0.45/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-19 21:02:25.000000 rembg-2.0.45/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-19 21:02:25.000000 rembg-2.0.45/versioneer.py
```

### Comparing `rembg-2.0.44/LICENSE.txt` & `rembg-2.0.45/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/PKG-INFO` & `rembg-2.0.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.44
+Version: 2.0.45
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 Keywords: remove,background,u2net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rembg-2.0.44/README.md` & `rembg-2.0.45/README.md`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/bg.py` & `rembg-2.0.45/rembg/bg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/cli.py` & `rembg-2.0.45/rembg/cli.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/commands/b_command.py` & `rembg-2.0.45/rembg/commands/b_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/commands/i_command.py` & `rembg-2.0.45/rembg/commands/i_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/commands/p_command.py` & `rembg-2.0.45/rembg/commands/p_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/commands/s_command.py` & `rembg-2.0.45/rembg/commands/s_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/session_factory.py` & `rembg-2.0.45/rembg/session_factory.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/sessions/__init__.py` & `rembg-2.0.45/rembg/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/sessions/base.py` & `rembg-2.0.45/rembg/sessions/base.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/sessions/dis_anime.py` & `rembg-2.0.45/rembg/sessions/dis_anime.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/sessions/dis_general_use.py` & `rembg-2.0.45/rembg/sessions/dis_general_use.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/sessions/sam.py` & `rembg-2.0.45/rembg/sessions/sam.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/sessions/silueta.py` & `rembg-2.0.45/rembg/sessions/silueta.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/sessions/u2net.py` & `rembg-2.0.45/rembg/sessions/u2net.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/sessions/u2net_cloth_seg.py` & `rembg-2.0.45/rembg/sessions/u2net_cloth_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/sessions/u2net_human_seg.py` & `rembg-2.0.45/rembg/sessions/u2net_human_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg/sessions/u2netp.py` & `rembg-2.0.45/rembg/sessions/u2netp.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/rembg.egg-info/PKG-INFO` & `rembg-2.0.45/rembg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.44
+Version: 2.0.45
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 Keywords: remove,background,u2net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rembg-2.0.44/rembg.egg-info/SOURCES.txt` & `rembg-2.0.45/rembg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/setup.py` & `rembg-2.0.45/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "onnxruntime",
     "opencv-python-headless",
     "pillow",
     "pooch",
     "pymatting",
     "scikit-image",
     "scipy",
+    "tqdm",
 ]
 
 extras_require = {
     "dev": [
         "bandit",
         "black",
         "flake8",
@@ -40,15 +41,14 @@
         "aiohttp",
         "asyncer",
         "click",
         "fastapi",
         "filetype",
         "gradio",
         "python-multipart",
-        "tqdm",
         "uvicorn",
         "watchdog",
     ],
 }
 
 entry_points = {
     "console_scripts": [
```

### Comparing `rembg-2.0.44/tests/test_remove.py` & `rembg-2.0.45/tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.44/versioneer.py` & `rembg-2.0.45/versioneer.py`

 * *Files identical despite different names*

