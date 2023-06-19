# Comparing `tmp/cq23-1.9.4.tar.gz` & `tmp/cq23-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-1.9.4.tar", last modified: Sat Jun 17 07:45:55 2023, max compression
+gzip compressed data, was "cq23-2.0.0.tar", last modified: Mon Jun 19 03:23:29 2023, max compression
```

## Comparing `cq23-1.9.4.tar` & `cq23-2.0.0.tar`

### file list

```diff
@@ -1,45 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-17 07:45:55.296350 cq23-1.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-17 07:45:47.000000 cq23-1.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-17 07:45:47.000000 cq23-1.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-17 07:45:55.296350 cq23-1.9.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.292350 cq23-1.9.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-17 07:45:47.000000 cq23-1.9.4/src/admin/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-17 07:45:47.000000 cq23-1.9.4/src/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-17 07:45:47.000000 cq23-1.9.4/src/admin/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-17 07:45:47.000000 cq23-1.9.4/src/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-17 07:45:47.000000 cq23-1.9.4/src/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-17 07:45:55.000000 cq23-1.9.4/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-17 07:45:55.000000 cq23-1.9.4/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 07:45:55.000000 cq23-1.9.4/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-17 07:45:55.000000 cq23-1.9.4/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 07:45:55.000000 cq23-1.9.4/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-17 07:45:55.000000 cq23-1.9.4/src/cq23.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-17 07:45:47.000000 cq23-1.9.4/src/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-17 07:45:47.000000 cq23-1.9.4/src/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-17 07:45:47.000000 cq23-1.9.4/src/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/replay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-17 07:45:47.000000 cq23-1.9.4/src/replay/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-17 07:45:47.000000 cq23-1.9.4/src/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-17 07:45:47.000000 cq23-1.9.4/src/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-17 07:45:47.000000 cq23-1.9.4/src/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/web_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/web_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-17 07:45:47.000000 cq23-1.9.4/src/web_server/flask_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-17 07:45:47.000000 cq23-1.9.4/src/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:29.027961 cq23-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-19 03:23:29.027961 cq23-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-19 03:23:19.000000 cq23-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-19 03:23:19.000000 cq23-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-19 03:23:29.031961 cq23-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:29.019961 cq23-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:29.023961 cq23-2.0.0/src/cq23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:29.023961 cq23-2.0.0/src/cq23/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:29.023961 cq23-2.0.0/src/cq23/build_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/build_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/build_image/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/build_image/docker_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:29.027961 cq23-2.0.0/src/cq23/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:29.027961 cq23-2.0.0/src/cq23/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:29.027961 cq23-2.0.0/src/cq23/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:29.027961 cq23-2.0.0/src/cq23/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:29.027961 cq23-2.0.0/src/cq23/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/replay/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:29.027961 cq23-2.0.0/src/cq23/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:29.027961 cq23-2.0.0/src/cq23/web_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/web_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/web_server/flask_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:29.027961 cq23-2.0.0/src/cq23/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-19 03:23:19.000000 cq23-2.0.0/src/cq23/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:23:29.023961 cq23-2.0.0/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-19 03:23:29.000000 cq23-2.0.0/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-19 03:23:29.000000 cq23-2.0.0/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 03:23:29.000000 cq23-2.0.0/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-19 03:23:29.000000 cq23-2.0.0/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-19 03:23:29.000000 cq23-2.0.0/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 03:23:29.000000 cq23-2.0.0/src/cq23.egg-info/top_level.txt
```

### Comparing `cq23-1.9.4/PKG-INFO` & `cq23-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.9.4
+Version: 2.0.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.9.4/setup.cfg` & `cq23-2.0.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 1.9.4
+version = 2.0.0
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls = 
@@ -12,32 +12,36 @@
 	repository = https://github.com/CALED-Team/cq23-cli-utilities
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
+include_package_data = True
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	docker>=6.0.1
 	boto3>=1.26.143
 	colorama>=0.4.6
 	flask>=2.2.5
 	flask-cors>=3.0.10
 	requests>=2.31.0
 
+[options.package_data]
+* = *.html
+
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
-	cq23 = main.command:route_command
+	cq23 = cq23.main.command:route_command
 
 [flake8]
 max-line-length = 120
 exclude = .tox,.git,*/static/CACHE/*,docs,node_modules,venv
 
 [pycodestyle]
 max-line-length = 120
```

### Comparing `cq23-1.9.4/src/admin/aws.py` & `cq23-2.0.0/src/cq23/admin/aws.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.4/src/admin/builder.py` & `cq23-2.0.0/src/cq23/admin/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from main.utils import admin
+from cq23.main.utils import admin
 
 from .aws import create_cq_instances, terminate_instances_by_name
 
 
 def new_builders(*args):
     create_cq_instances("builder", *args)
```

### Comparing `cq23-1.9.4/src/admin/worker.py` & `cq23-2.0.0/src/cq23/admin/worker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from main.utils import admin
+from cq23.main.utils import admin
 
 from .aws import create_cq_instances, terminate_instances_by_name
 
 
 def new_workers(*args):
     create_cq_instances("worker", *args)
```

### Comparing `cq23-1.9.4/src/check/command.py` & `cq23-2.0.0/src/cq23/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.4/src/cleanup/command.py` & `cq23-2.0.0/src/cq23/cleanup/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     # Get all images
     images = client.images.list(all=True)
 
     # Delete images with names starting with 'cq_'
     for image in images:
         for tag in image.tags:
-            if tag.startswith("cq_"):
+            if tag.startswith("cq_") or tag.startswith("cq-"):
                 print("> Deleting image", tag)
                 client.images.remove(image.id, force=True)
                 break
 
     # Get the volume
     try:
         volume = client.volumes.get("cq-game-replay")
```

### Comparing `cq23-1.9.4/src/cq23.egg-info/PKG-INFO` & `cq23-2.0.0/src/cq23.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.9.4
+Version: 2.0.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.9.4/src/cq23.egg-info/SOURCES.txt` & `cq23-2.0.0/src/cq23.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 README.md
 pyproject.toml
 setup.cfg
-src/admin/__init__.py
-src/admin/aws.py
-src/admin/builder.py
-src/admin/worker.py
-src/check/__init__.py
-src/check/command.py
-src/cleanup/__init__.py
-src/cleanup/command.py
+src/cq23/__init__.py
 src/cq23.egg-info/PKG-INFO
 src/cq23.egg-info/SOURCES.txt
 src/cq23.egg-info/dependency_links.txt
 src/cq23.egg-info/entry_points.txt
 src/cq23.egg-info/requires.txt
 src/cq23.egg-info/top_level.txt
-src/main/__init__.py
-src/main/command.py
-src/main/utils.py
-src/new_client/__init__.py
-src/new_client/command.py
-src/replay/__init__.py
-src/replay/command.py
-src/run_game/__init__.py
-src/run_game/command.py
-src/run_game/docker_tools.py
-src/run_game/gcs.py
-src/web_server/__init__.py
-src/web_server/flask_api.py
-src/zip/__init__.py
-src/zip/command.py
+src/cq23/admin/__init__.py
+src/cq23/admin/aws.py
+src/cq23/admin/builder.py
+src/cq23/admin/worker.py
+src/cq23/build_image/__init__.py
+src/cq23/build_image/command.py
+src/cq23/build_image/docker_tools.py
+src/cq23/check/__init__.py
+src/cq23/check/command.py
+src/cq23/cleanup/__init__.py
+src/cq23/cleanup/command.py
+src/cq23/main/__init__.py
+src/cq23/main/command.py
+src/cq23/main/utils.py
+src/cq23/new_client/__init__.py
+src/cq23/new_client/command.py
+src/cq23/replay/__init__.py
+src/cq23/replay/command.py
+src/cq23/run_game/__init__.py
+src/cq23/run_game/command.py
+src/cq23/run_game/docker_tools.py
+src/cq23/run_game/gcs.py
+src/cq23/web_server/__init__.py
+src/cq23/web_server/flask_api.py
+src/cq23/zip/__init__.py
+src/cq23/zip/command.py
```

### Comparing `cq23-1.9.4/src/main/command.py` & `cq23-2.0.0/src/cq23/main/command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import sys
 
-from admin.builder import command as builder
-from admin.worker import command as worker
-from check.command import check
-from cleanup.command import cleanup
-from new_client.command import new_client
-from replay.command import replay
-from run_game.command import run_game
-from zip.command import zip
+from cq23.admin.builder import command as builder
+from cq23.admin.worker import command as worker
+from cq23.build_image.command import build
+from cq23.check.command import check
+from cq23.cleanup.command import cleanup
+from cq23.new_client.command import new_client
+from cq23.replay.command import replay
+from cq23.run_game.command import run_game
+from cq23.zip.command import zip
 
 from .utils import restore_cwd
 
 
 def help_message():
     message = (
         "Available commands:\n\n"
         + "> cq23 new python my_bot\n"
+        + "> cq23 build <name>\n"
         + "> cq23 run\n"
         + "> cq23 run map=<map name>\n"
         + "> cq23 replay\n"
         + "> cq23 zip\n"
         + "> cq23 check\n"
         + "> cq23 cleanup\n\n"
         + "If you need help with the competition, post a message in Discord or email us at info@codequest.club."
@@ -29,14 +31,15 @@
 
 @restore_cwd
 def route_command():
     command_args = sys.argv[1:]
 
     first_arg_mapping = {
         "new": new_client,
+        "build": build,
         "run": run_game,
         "replay": replay,
         "cleanup": cleanup,
         "zip": zip,
         "check": check,
         "worker": worker,
         "builder": builder,
```

### Comparing `cq23-1.9.4/src/main/utils.py` & `cq23-2.0.0/src/cq23/main/utils.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.4/src/new_client/command.py` & `cq23-2.0.0/src/cq23/new_client/command.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         print("You must specify the language for the client: cq23 new python my_bot")
         return
 
     language_map = {
         "raw": "https://github.com/CALED-Team/codequest23-raw-submission.git",
         "python": "https://github.com/CALED-Team/codequest23-python-submission.git",
         "cpp": "https://github.com/CALED-Team/codequest23-cpp-submission.git",
+        "java": "https://github.com/CALED-Team/codequest23-java-submission.git",
     }
     language = args[0]
 
     if language not in language_map.keys():
         return print(
             "Invalid language selected for the new bot. Language should be one of:",
             "[" + " - ".join(language_map.keys()) + "]",
```

### Comparing `cq23-1.9.4/src/replay/command.py` & `cq23-2.0.0/src/cq23/replay/command.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import time
 import webbrowser
 from multiprocessing import Process
 
 import requests
 
-from web_server import flask_api
+from cq23.web_server import flask_api
 
 
 def run_gui(replay_files_directory):
     gui_process = Process(target=flask_api.start, args=(replay_files_directory,))
     gui_process.start()
     webbrowser.open("https://watch.codequest.club/?base_url=http://127.0.0.1:2023/")
     return gui_process
```

### Comparing `cq23-1.9.4/src/run_game/docker_tools.py` & `cq23-2.0.0/src/cq23/run_game/docker_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import docker
 from docker.errors import APIError, DockerException, NotFound
 
 AWS_REGION = "ap-southeast-2"
 ECR_REGISTRY = "public.ecr.aws/z3i0q5x8"
 GAME_SERVER_ECR_REPO = "cq-game-server"
+SUBMISSIONS_ECR_REPO = "cq-submissions"
 
 DOCKER_CLIENT = None
 
 
 def ensure_docker_client_exists():
     global DOCKER_CLIENT
     try:
```

### Comparing `cq23-1.9.4/src/run_game/gcs.py` & `cq23-2.0.0/src/cq23/run_game/gcs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,76 @@
+import base64
 import json
 import os
 import subprocess
 import sys
+import time
 import webbrowser
 from multiprocessing import Process
 
 import requests
 
-from web_server import flask_api
+from cq23.web_server import flask_api
 
 from . import docker_tools
 
 MATCH_TIMEOUT_SECONDS = 12 * 60  # This should ideally match the one in game worker
 
 
+def open_waiting_page():
+    time.sleep(7)
+
+    # Open the waiting page which redirects to the GUI
+    gui_url = "https://watch.codequest.club/?base_url=http://127.0.0.1:2023/"
+    base64_gui_url = base64.b64encode(gui_url.encode("utf-8")).decode("utf-8")
+    loading_page_url = (
+        "http://127.0.0.1:2023/F/loading_screen.html?ra=" + base64_gui_url
+    )
+    webbrowser.open(loading_page_url)
+
+
 def run_gui():
     replay_files_directory = os.path.join(
         os.path.join(os.path.join(os.getcwd(), "gcs"), "src"), "live_replay_files"
     )
-    # gui_directory = os.path.join(os.getcwd(), "gui")
     gui_process = Process(target=flask_api.start, args=(replay_files_directory,))
     gui_process.start()
-    # webbrowser.open("file://" + os.path.join(gui_directory, "index.html"))
-    webbrowser.open("https://watch.codequest.club/?base_url=http://127.0.0.1:2023/")
-    return gui_process
 
+    waiting_page_process = Process(target=open_waiting_page)
+    waiting_page_process.start()
+
+    return gui_process, waiting_page_process
+
+
+def stop_gui(gui_process, waiting_page_process):
+    waiting_page_process.join(timeout=1)
+    if waiting_page_process.is_alive():
+        waiting_page_process.terminate()
 
-def stop_gui(gui_process):
     print("Requesting graceful termination of GUI server...")
     requests.request("get", "http://127.0.0.1:2023/die")
 
     gui_process.join(timeout=15)
     if gui_process.is_alive():
         print("Graceful termination failed, killing the GUI server...")
         gui_process.terminate()
 
 
-def run_gcs(gcs_folder_name, game_map=None):
+def run_gcs(gcs_folder_name, home_image, away_image, game_map=None):
     gcs_src_dir = os.path.join(gcs_folder_name, "src")
     clients_file_content = [
         {
             "id": "1",
-            "name": "Your Code - 1",
-            "image": docker_tools.get_client_image_tag(),
+            "name": "Home",
+            "image": home_image,
         },
         {
             "id": "2",
-            "name": "Your Code - 2",
-            "image": docker_tools.get_client_image_tag(),
+            "name": "Away",
+            "image": away_image,
         },
     ]
     clients_file_address = "clients.json"
 
     with open(os.path.join(gcs_src_dir, clients_file_address), "w") as f:
         f.write(json.dumps(clients_file_content))
 
@@ -63,17 +82,17 @@
     ]
 
     if game_map:
         subprocess_args.append("--server-arg")
         subprocess_args.append("-m " + str(game_map))
 
     print("Starting the game interface...")
-    gui_process = run_gui()
+    gui_process, waiting_page_process = run_gui()
 
     print("Starting the game...")
     subprocess.run(subprocess_args, timeout=MATCH_TIMEOUT_SECONDS, cwd=gcs_src_dir)
     print("Game finished.", flush=True)
 
     print("Stopping the game interface...")
-    stop_gui(gui_process)
+    stop_gui(gui_process, waiting_page_process)
 
     os.remove(os.path.join(gcs_src_dir, clients_file_address))
```

### Comparing `cq23-1.9.4/src/web_server/flask_api.py` & `cq23-2.0.0/src/cq23/web_server/flask_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import os.path
+import logging
+import os
 import time
 from threading import Thread
 
 from flask import Flask, jsonify, request, send_file
 from flask_cors import CORS
 from werkzeug.serving import make_server
 
-app = Flask(__name__)
+app = Flask(__name__, static_url_path="/F", static_folder="files")
 CORS(app)
 ROOT_DIRECTORY = None
 PORT = None
 LAST_REQUEST_TIME = time.time()
 SERVER = None
 
 
 def get_full_path_or_404(file_name):
     full_file_path = os.path.join(ROOT_DIRECTORY, file_name)
-    print(full_file_path)
     if not os.path.exists(full_file_path):
         return False, (jsonify({"message": "Replay file not found."}), 404)
 
     return True, full_file_path
 
 
 def check_death_timer():
@@ -96,18 +96,18 @@
     with open(response) as f:
         file_content = f.read()
 
     return jsonify({"message": "ok", "content": file_content})
 
 
 def start(replay_files_directory, port=2023, debug=False):
-    # This wait time here is implemented for the game server to have enough time to write a couple of the replay files
-    time.sleep(5)
+    if not debug:
+        logging.getLogger("werkzeug").setLevel(logging.ERROR)
 
     global ROOT_DIRECTORY, PORT
     ROOT_DIRECTORY = replay_files_directory
     PORT = port
 
     global SERVER
-    SERVER = make_server("127.0.0.1", port, app)
+    SERVER = make_server("0.0.0.0", port, app, threaded=True)
     SERVER.serve_forever()
     # app.run(debug=debug, port=PORT, threaded=True)
```

### Comparing `cq23-1.9.4/src/zip/command.py` & `cq23-2.0.0/src/cq23/zip/command.py`

 * *Files identical despite different names*

