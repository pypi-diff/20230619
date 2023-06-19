# Comparing `tmp/rembg-2.0.43.tar.gz` & `tmp/rembg-2.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rembg-2.0.43.tar", last modified: Fri Jun  2 12:28:41 2023, max compression
+gzip compressed data, was "rembg-2.0.44.tar", last modified: Mon Jun 19 20:26:06 2023, max compression
```

## Comparing `rembg-2.0.43.tar` & `rembg-2.0.44.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:28:41.536268 rembg-2.0.43/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-02 12:28:28.000000 rembg-2.0.43/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-02 12:28:28.000000 rembg-2.0.43/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-06-02 12:28:41.536268 rembg-2.0.43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-06-02 12:28:28.000000 rembg-2.0.43/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-02 12:28:28.000000 rembg-2.0.43/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:28:41.536268 rembg-2.0.43/rembg/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-02 12:28:41.536268 rembg-2.0.43/rembg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/bg.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:28:41.536268 rembg-2.0.43/rembg/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/commands/b_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/commands/i_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/commands/p_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/commands/s_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/session_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:28:41.536268 rembg-2.0.43/rembg/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/dis_anime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/dis_general_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/silueta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/u2net_cloth_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/u2net_human_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/u2netp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:28:41.532268 rembg-2.0.43/rembg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-06-02 12:28:41.000000 rembg-2.0.43/rembg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-02 12:28:41.000000 rembg-2.0.43/rembg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 12:28:41.000000 rembg-2.0.43/rembg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 12:28:41.000000 rembg-2.0.43/rembg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-02 12:28:41.000000 rembg-2.0.43/rembg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 12:28:41.000000 rembg-2.0.43/rembg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 12:28:28.000000 rembg-2.0.43/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-02 12:28:28.000000 rembg-2.0.43/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-02 12:28:41.536268 rembg-2.0.43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-02 12:28:28.000000 rembg-2.0.43/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-02 12:28:28.000000 rembg-2.0.43/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:26:06.078688 rembg-2.0.44/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-19 20:24:40.000000 rembg-2.0.44/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-19 20:24:40.000000 rembg-2.0.44/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-19 20:26:06.078688 rembg-2.0.44/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-06-19 20:24:40.000000 rembg-2.0.44/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-19 20:24:40.000000 rembg-2.0.44/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:26:06.082688 rembg-2.0.44/rembg/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-19 20:26:06.082688 rembg-2.0.44/rembg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:26:06.078688 rembg-2.0.44/rembg/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/commands/b_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/commands/i_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/commands/p_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/commands/s_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/session_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:26:06.078688 rembg-2.0.44/rembg/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/dis_anime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/dis_general_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/silueta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/u2net_cloth_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/u2net_human_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-19 20:24:40.000000 rembg-2.0.44/rembg/sessions/u2netp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:26:06.078688 rembg-2.0.44/rembg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-19 20:26:05.000000 rembg-2.0.44/rembg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-19 20:26:06.000000 rembg-2.0.44/rembg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:26:05.000000 rembg-2.0.44/rembg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 20:26:05.000000 rembg-2.0.44/rembg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-19 20:26:05.000000 rembg-2.0.44/rembg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 20:26:05.000000 rembg-2.0.44/rembg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-19 20:26:06.082688 rembg-2.0.44/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-19 20:24:40.000000 rembg-2.0.44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:26:06.078688 rembg-2.0.44/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-19 20:24:40.000000 rembg-2.0.44/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-19 20:24:40.000000 rembg-2.0.44/versioneer.py
```

### Comparing `rembg-2.0.43/LICENSE.txt` & `rembg-2.0.44/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/PKG-INFO` & `rembg-2.0.44/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.43
+Version: 2.0.44
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 Keywords: remove,background,u2net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
@@ -17,15 +17,17 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 Provides-Extra: gpu
+Provides-Extra: cli
 License-File: LICENSE.txt
 
 # Rembg
 
 [![Downloads](https://pepy.tech/badge/rembg)](https://pepy.tech/project/rembg)
 [![Downloads](https://pepy.tech/badge/rembg/month)](https://pepy.tech/project/rembg)
 [![Downloads](https://pepy.tech/badge/rembg/week)](https://pepy.tech/project/rembg)
@@ -102,15 +104,16 @@
 ```
 
 ## Installation
 
 CPU support:
 
 ```bash
-pip install rembg
+pip install rembg # for library
+pip install rembg[cli] # for library + cli
 ```
 
 GPU support:
 
 First of all, you need to check if your system supports the `onnxruntime-gpu`.
 
 Go to https://onnxruntime.ai and check the installation matrix.
@@ -118,15 +121,16 @@
 <p style="display: flex;align-items: center;justify-content: center;">
   <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/onnxruntime-installation-matrix.png" width="400" />
 </p>
 
 If yes, just run:
 
 ```bash
-pip install rembg[gpu]
+pip install rembg[gpu] # for library
+pip install rembg[gpu,cli] # for library + cli
 ```
 
 ## Usage as a cli
 
 After the installation step you can use rembg just typing `rembg` in your terminal window.
 
 The `rembg` command has 4 subcommands, one for each input type:
```

### Comparing `rembg-2.0.43/README.md` & `rembg-2.0.44/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,16 @@
 ```
 
 ## Installation
 
 CPU support:
 
 ```bash
-pip install rembg
+pip install rembg # for library
+pip install rembg[cli] # for library + cli
 ```
 
 GPU support:
 
 First of all, you need to check if your system supports the `onnxruntime-gpu`.
 
 Go to https://onnxruntime.ai and check the installation matrix.
@@ -92,15 +93,16 @@
 <p style="display: flex;align-items: center;justify-content: center;">
   <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/onnxruntime-installation-matrix.png" width="400" />
 </p>
 
 If yes, just run:
 
 ```bash
-pip install rembg[gpu]
+pip install rembg[gpu] # for library
+pip install rembg[gpu,cli] # for library + cli
 ```
 
 ## Usage as a cli
 
 After the installation step you can use rembg just typing `rembg` in your terminal window.
 
 The `rembg` command has 4 subcommands, one for each input type:
```

#### html2text {}

```diff
@@ -38,34 +38,36 @@
 girl-3.out.png]
 **If this project has helped you, please consider making a [donation](https://
 www.buymeacoffee.com/danielgatis).** ## Sponsor
                PhotoRoom Remove Background API
 [Unsplash]        https://photoroom.com/api
            Fast and accurate background remover API
 ## Requirements ``` python: >3.7, <3.12 ``` ## Installation CPU support:
-```bash pip install rembg ``` GPU support: First of all, you need to check if
-your system supports the `onnxruntime-gpu`. Go to https://onnxruntime.ai and
-check the installation matrix.
+```bash pip install rembg # for library pip install rembg[cli] # for library +
+cli ``` GPU support: First of all, you need to check if your system supports
+the `onnxruntime-gpu`. Go to https://onnxruntime.ai and check the installation
+matrix.
 [https://raw.githubusercontent.com/danielgatis/rembg/master/onnxruntime-
 installation-matrix.png]
-If yes, just run: ```bash pip install rembg[gpu] ``` ## Usage as a cli After
-the installation step you can use rembg just typing `rembg` in your terminal
-window. The `rembg` command has 4 subcommands, one for each input type: - `i`
-for files - `p` for folders - `s` for http server - `b` for RGB24 pixel binary
-stream You can get help about the main command using: ``` rembg --help ``` As
-well, about all the subcommands using: ``` rembg  --help ``` ### rembg `i` Used
-when input and output are files. Remove the background from a remote image ```
-curl -s http://input.png | rembg i > output.png ``` Remove the background from
-a local file ``` rembg i path/to/input.png path/to/output.png ``` Remove the
-background specifying a model ``` rembg i -m u2netp path/to/input.png path/to/
-output.png ``` Remove the background returning only the mask ``` rembg i -om
-path/to/input.png path/to/output.png ``` Remove the background applying an
-alpha matting ``` rembg i -a path/to/input.png path/to/output.png ``` Passing
-extras parameters ``` rembg i -m sam -x '{"input_labels": [1], "input_points":
-[[100,100]]}' path/to/input.png path/to/output.png ``` ### rembg `p` Used when
+If yes, just run: ```bash pip install rembg[gpu] # for library pip install
+rembg[gpu,cli] # for library + cli ``` ## Usage as a cli After the installation
+step you can use rembg just typing `rembg` in your terminal window. The `rembg`
+command has 4 subcommands, one for each input type: - `i` for files - `p` for
+folders - `s` for http server - `b` for RGB24 pixel binary stream You can get
+help about the main command using: ``` rembg --help ``` As well, about all the
+subcommands using: ``` rembg  --help ``` ### rembg `i` Used when input and
+output are files. Remove the background from a remote image ``` curl -s http://
+input.png | rembg i > output.png ``` Remove the background from a local file
+``` rembg i path/to/input.png path/to/output.png ``` Remove the background
+specifying a model ``` rembg i -m u2netp path/to/input.png path/to/output.png
+``` Remove the background returning only the mask ``` rembg i -om path/to/
+input.png path/to/output.png ``` Remove the background applying an alpha
+matting ``` rembg i -a path/to/input.png path/to/output.png ``` Passing extras
+parameters ``` rembg i -m sam -x '{"input_labels": [1], "input_points": [
+[100,100]]}' path/to/input.png path/to/output.png ``` ### rembg `p` Used when
 input and output are folders. Remove the background from all images in a folder
 ``` rembg p path/to/input path/to/output ``` Same as before, but watching for
 new/changed files to process ``` rembg p -w path/to/input path/to/output ```
 ### rembg `s` Used to start http server. To see the complete endpoints
 documentation, go to: `http://localhost:5000/api`. Remove the background from
 an image url ``` curl -s "http://localhost:5000/api/remove?url=http://
 input.png" -o output.png ``` Remove the background from an uploaded image ```
```

### Comparing `rembg-2.0.43/rembg/bg.py` & `rembg-2.0.44/rembg/bg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg/commands/b_command.py` & `rembg-2.0.44/rembg/commands/b_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg/commands/i_command.py` & `rembg-2.0.44/rembg/commands/i_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg/commands/p_command.py` & `rembg-2.0.44/rembg/commands/p_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg/commands/s_command.py` & `rembg-2.0.44/rembg/commands/s_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg/session_factory.py` & `rembg-2.0.44/rembg/session_factory.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg/sessions/__init__.py` & `rembg-2.0.44/rembg/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg/sessions/base.py` & `rembg-2.0.44/rembg/sessions/base.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg/sessions/dis_anime.py` & `rembg-2.0.44/rembg/sessions/dis_anime.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg/sessions/dis_general_use.py` & `rembg-2.0.44/rembg/sessions/dis_general_use.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg/sessions/sam.py` & `rembg-2.0.44/rembg/sessions/sam.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg/sessions/silueta.py` & `rembg-2.0.44/rembg/sessions/silueta.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg/sessions/u2net.py` & `rembg-2.0.44/rembg/sessions/u2net.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg/sessions/u2net_cloth_seg.py` & `rembg-2.0.44/rembg/sessions/u2net_cloth_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg/sessions/u2net_human_seg.py` & `rembg-2.0.44/rembg/sessions/u2net_human_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg/sessions/u2netp.py` & `rembg-2.0.44/rembg/sessions/u2netp.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.43/rembg.egg-info/PKG-INFO` & `rembg-2.0.44/rembg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.43
+Version: 2.0.44
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 Keywords: remove,background,u2net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
@@ -17,15 +17,17 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 Provides-Extra: gpu
+Provides-Extra: cli
 License-File: LICENSE.txt
 
 # Rembg
 
 [![Downloads](https://pepy.tech/badge/rembg)](https://pepy.tech/project/rembg)
 [![Downloads](https://pepy.tech/badge/rembg/month)](https://pepy.tech/project/rembg)
 [![Downloads](https://pepy.tech/badge/rembg/week)](https://pepy.tech/project/rembg)
@@ -102,15 +104,16 @@
 ```
 
 ## Installation
 
 CPU support:
 
 ```bash
-pip install rembg
+pip install rembg # for library
+pip install rembg[cli] # for library + cli
 ```
 
 GPU support:
 
 First of all, you need to check if your system supports the `onnxruntime-gpu`.
 
 Go to https://onnxruntime.ai and check the installation matrix.
@@ -118,15 +121,16 @@
 <p style="display: flex;align-items: center;justify-content: center;">
   <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/onnxruntime-installation-matrix.png" width="400" />
 </p>
 
 If yes, just run:
 
 ```bash
-pip install rembg[gpu]
+pip install rembg[gpu] # for library
+pip install rembg[gpu,cli] # for library + cli
 ```
 
 ## Usage as a cli
 
 After the installation step you can use rembg just typing `rembg` in your terminal window.
 
 The `rembg` command has 4 subcommands, one for each input type:
```

### Comparing `rembg-2.0.43/rembg.egg-info/SOURCES.txt` & `rembg-2.0.44/rembg.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
-requirements-gpu.txt
-requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 rembg/__init__.py
 rembg/_version.py
 rembg/bg.py
 rembg/cli.py
@@ -28,8 +26,9 @@
 rembg/sessions/dis_anime.py
 rembg/sessions/dis_general_use.py
 rembg/sessions/sam.py
 rembg/sessions/silueta.py
 rembg/sessions/u2net.py
 rembg/sessions/u2net_cloth_seg.py
 rembg/sessions/u2net_human_seg.py
-rembg/sessions/u2netp.py
+rembg/sessions/u2netp.py
+tests/test_remove.py
```

### Comparing `rembg-2.0.43/versioneer.py` & `rembg-2.0.44/versioneer.py`

 * *Files identical despite different names*

