# Comparing `tmp/pywalc-0.1.1.tar.gz` & `tmp/pywalc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywalc-0.1.1.tar", last modified: Sun Jun 18 09:15:38 2023, max compression
+gzip compressed data, was "pywalc-0.2.1.tar", last modified: Mon Jun 19 12:15:30 2023, max compression
```

## Comparing `pywalc-0.1.1.tar` & `pywalc-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-18 09:15:38.901733 pywalc-0.1.1/
--rw-r--r--   0 png       (1000) png261    (1000)     1070 2023-06-16 14:10:31.000000 pywalc-0.1.1/LICENSE
--rw-r--r--   0 png       (1000) png261    (1000)      110 2023-06-17 14:45:01.000000 pywalc-0.1.1/MANIFEST.in
--rw-r--r--   0 png       (1000) png261    (1000)     3150 2023-06-18 09:15:38.901733 pywalc-0.1.1/PKG-INFO
--rw-r--r--   0 png       (1000) png261    (1000)     2478 2023-06-18 08:59:35.000000 pywalc-0.1.1/README.md
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-18 09:15:38.898399 pywalc-0.1.1/pywalc/
--rw-r--r--   0 png       (1000) png261    (1000)      232 2023-06-18 08:04:04.000000 pywalc-0.1.1/pywalc/__init__.py
--rw-r--r--   0 png       (1000) png261    (1000)     1035 2023-06-18 08:13:57.000000 pywalc-0.1.1/pywalc/__main__.py
--rw-r--r--   0 png       (1000) png261    (1000)      763 2023-06-18 08:04:32.000000 pywalc-0.1.1/pywalc/colors.py
--rw-r--r--   0 png       (1000) png261    (1000)     4388 2023-06-18 08:50:21.000000 pywalc-0.1.1/pywalc/server.py
--rw-r--r--   0 png       (1000) png261    (1000)      661 2023-06-18 09:13:43.000000 pywalc-0.1.1/pywalc/settings.py
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-18 09:15:38.895066 pywalc-0.1.1/pywalc/static/
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-18 09:15:38.898399 pywalc-0.1.1/pywalc/static/css/
--rw-r--r--   0 png       (1000) png261    (1000)     4575 2023-06-17 07:42:58.000000 pywalc-0.1.1/pywalc/static/css/style.css
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-18 09:15:38.901733 pywalc-0.1.1/pywalc/static/js/
--rw-r--r--   0 png       (1000) png261    (1000)      825 2023-06-18 02:17:16.000000 pywalc-0.1.1/pywalc/static/js/Actions.js
--rw-r--r--   0 png       (1000) png261    (1000)      790 2023-06-18 02:54:06.000000 pywalc-0.1.1/pywalc/static/js/Color.js
--rw-r--r--   0 png       (1000) png261    (1000)      209 2023-06-17 07:42:58.000000 pywalc-0.1.1/pywalc/static/js/Sys.js
--rw-r--r--   0 png       (1000) png261    (1000)      794 2023-06-18 02:09:23.000000 pywalc-0.1.1/pywalc/static/js/Theme.js
--rw-r--r--   0 png       (1000) png261    (1000)     1284 2023-06-18 02:54:06.000000 pywalc-0.1.1/pywalc/static/js/Wallpaper.js
--rw-r--r--   0 png       (1000) png261    (1000)      675 2023-06-18 02:54:06.000000 pywalc-0.1.1/pywalc/static/js/api.js
--rw-r--r--   0 png       (1000) png261    (1000)     1636 2023-06-18 02:09:23.000000 pywalc-0.1.1/pywalc/static/js/data.js
--rw-r--r--   0 png       (1000) png261    (1000)      352 2023-06-17 16:05:08.000000 pywalc-0.1.1/pywalc/static/js/helper.js
--rw-r--r--   0 png       (1000) png261    (1000)      537 2023-06-18 02:54:06.000000 pywalc-0.1.1/pywalc/static/js/main.js
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-18 09:15:38.901733 pywalc-0.1.1/pywalc/templates/
--rw-r--r--   0 png       (1000) png261    (1000)     3496 2023-06-18 02:05:57.000000 pywalc-0.1.1/pywalc/templates/index.html
--rw-r--r--   0 png       (1000) png261    (1000)      701 2023-06-18 08:49:52.000000 pywalc-0.1.1/pywalc/theme.py
--rw-r--r--   0 png       (1000) png261    (1000)     1944 2023-06-18 06:52:55.000000 pywalc-0.1.1/pywalc/util.py
--rw-r--r--   0 png       (1000) png261    (1000)     1299 2023-06-18 08:05:08.000000 pywalc-0.1.1/pywalc/wallpaper.py
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-18 09:15:38.898399 pywalc-0.1.1/pywalc.egg-info/
--rw-r--r--   0 png       (1000) png261    (1000)     3150 2023-06-18 09:15:38.000000 pywalc-0.1.1/pywalc.egg-info/PKG-INFO
--rw-r--r--   0 png       (1000) png261    (1000)      682 2023-06-18 09:15:38.000000 pywalc-0.1.1/pywalc.egg-info/SOURCES.txt
--rw-r--r--   0 png       (1000) png261    (1000)        1 2023-06-18 09:15:38.000000 pywalc-0.1.1/pywalc.egg-info/dependency_links.txt
--rw-r--r--   0 png       (1000) png261    (1000)       48 2023-06-18 09:15:38.000000 pywalc-0.1.1/pywalc.egg-info/entry_points.txt
--rw-r--r--   0 png       (1000) png261    (1000)        1 2023-06-18 09:15:38.000000 pywalc-0.1.1/pywalc.egg-info/not-zip-safe
--rw-r--r--   0 png       (1000) png261    (1000)      134 2023-06-18 09:15:38.000000 pywalc-0.1.1/pywalc.egg-info/requires.txt
--rw-r--r--   0 png       (1000) png261    (1000)        7 2023-06-18 09:15:38.000000 pywalc-0.1.1/pywalc.egg-info/top_level.txt
--rw-r--r--   0 png       (1000) png261    (1000)       38 2023-06-18 09:15:38.901733 pywalc-0.1.1/setup.cfg
--rw-r--r--   0 png       (1000) png261    (1000)     1270 2023-06-18 09:13:30.000000 pywalc-0.1.1/setup.py
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-19 12:15:30.660427 pywalc-0.2.1/
+-rw-r--r--   0 png       (1000) png261    (1000)     1070 2023-06-16 14:10:31.000000 pywalc-0.2.1/LICENSE
+-rw-r--r--   0 png       (1000) png261    (1000)      110 2023-06-17 14:45:01.000000 pywalc-0.2.1/MANIFEST.in
+-rw-r--r--   0 png       (1000) png261    (1000)     3150 2023-06-19 12:15:30.660427 pywalc-0.2.1/PKG-INFO
+-rw-r--r--   0 png       (1000) png261    (1000)     2478 2023-06-18 08:59:35.000000 pywalc-0.2.1/README.md
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-19 12:15:30.657094 pywalc-0.2.1/pywalc/
+-rw-r--r--   0 png       (1000) png261    (1000)      232 2023-06-19 10:30:29.000000 pywalc-0.2.1/pywalc/__init__.py
+-rw-r--r--   0 png       (1000) png261    (1000)      142 2023-06-19 10:06:29.000000 pywalc-0.2.1/pywalc/__main__.py
+-rw-r--r--   0 png       (1000) png261    (1000)     1462 2023-06-19 12:12:16.000000 pywalc-0.2.1/pywalc/app.py
+-rw-r--r--   0 png       (1000) png261    (1000)      543 2023-06-19 10:03:34.000000 pywalc-0.2.1/pywalc/colors.py
+-rw-r--r--   0 png       (1000) png261    (1000)     1436 2023-06-19 10:07:27.000000 pywalc-0.2.1/pywalc/pywal_util.py
+-rw-r--r--   0 png       (1000) png261    (1000)     4403 2023-06-19 10:25:00.000000 pywalc-0.2.1/pywalc/server.py
+-rw-r--r--   0 png       (1000) png261    (1000)      515 2023-06-19 12:14:53.000000 pywalc-0.2.1/pywalc/settings.py
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-19 12:15:30.657094 pywalc-0.2.1/pywalc/static/
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-19 12:15:30.660427 pywalc-0.2.1/pywalc/static/css/
+-rw-r--r--   0 png       (1000) png261    (1000)     4575 2023-06-17 07:42:58.000000 pywalc-0.2.1/pywalc/static/css/style.css
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-19 12:15:30.660427 pywalc-0.2.1/pywalc/static/js/
+-rw-r--r--   0 png       (1000) png261    (1000)      825 2023-06-19 09:58:09.000000 pywalc-0.2.1/pywalc/static/js/Actions.js
+-rw-r--r--   0 png       (1000) png261    (1000)      790 2023-06-18 02:54:06.000000 pywalc-0.2.1/pywalc/static/js/Color.js
+-rw-r--r--   0 png       (1000) png261    (1000)      209 2023-06-17 07:42:58.000000 pywalc-0.2.1/pywalc/static/js/Sys.js
+-rw-r--r--   0 png       (1000) png261    (1000)      794 2023-06-18 02:09:23.000000 pywalc-0.2.1/pywalc/static/js/Theme.js
+-rw-r--r--   0 png       (1000) png261    (1000)     1284 2023-06-19 09:57:09.000000 pywalc-0.2.1/pywalc/static/js/Wallpaper.js
+-rw-r--r--   0 png       (1000) png261    (1000)      675 2023-06-18 02:54:06.000000 pywalc-0.2.1/pywalc/static/js/api.js
+-rw-r--r--   0 png       (1000) png261    (1000)     1636 2023-06-19 10:00:16.000000 pywalc-0.2.1/pywalc/static/js/data.js
+-rw-r--r--   0 png       (1000) png261    (1000)      352 2023-06-17 16:05:08.000000 pywalc-0.2.1/pywalc/static/js/helper.js
+-rw-r--r--   0 png       (1000) png261    (1000)      537 2023-06-18 02:54:06.000000 pywalc-0.2.1/pywalc/static/js/main.js
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-19 12:15:30.660427 pywalc-0.2.1/pywalc/templates/
+-rw-r--r--   0 png       (1000) png261    (1000)     3496 2023-06-18 02:05:57.000000 pywalc-0.2.1/pywalc/templates/index.html
+-rw-r--r--   0 png       (1000) png261    (1000)      261 2023-06-19 10:03:29.000000 pywalc-0.2.1/pywalc/theme.py
+-rw-r--r--   0 png       (1000) png261    (1000)     1525 2023-06-19 12:12:38.000000 pywalc-0.2.1/pywalc/util.py
+-rw-r--r--   0 png       (1000) png261    (1000)     1344 2023-06-19 10:07:27.000000 pywalc-0.2.1/pywalc/wallpaper.py
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-19 12:15:30.660427 pywalc-0.2.1/pywalc.egg-info/
+-rw-r--r--   0 png       (1000) png261    (1000)     3150 2023-06-19 12:15:30.000000 pywalc-0.2.1/pywalc.egg-info/PKG-INFO
+-rw-r--r--   0 png       (1000) png261    (1000)      717 2023-06-19 12:15:30.000000 pywalc-0.2.1/pywalc.egg-info/SOURCES.txt
+-rw-r--r--   0 png       (1000) png261    (1000)        1 2023-06-19 12:15:30.000000 pywalc-0.2.1/pywalc.egg-info/dependency_links.txt
+-rw-r--r--   0 png       (1000) png261    (1000)       48 2023-06-19 12:15:30.000000 pywalc-0.2.1/pywalc.egg-info/entry_points.txt
+-rw-r--r--   0 png       (1000) png261    (1000)        1 2023-06-19 12:15:30.000000 pywalc-0.2.1/pywalc.egg-info/not-zip-safe
+-rw-r--r--   0 png       (1000) png261    (1000)      134 2023-06-19 12:15:30.000000 pywalc-0.2.1/pywalc.egg-info/requires.txt
+-rw-r--r--   0 png       (1000) png261    (1000)        7 2023-06-19 12:15:30.000000 pywalc-0.2.1/pywalc.egg-info/top_level.txt
+-rw-r--r--   0 png       (1000) png261    (1000)       38 2023-06-19 12:15:30.660427 pywalc-0.2.1/setup.cfg
+-rw-r--r--   0 png       (1000) png261    (1000)     1270 2023-06-19 12:14:38.000000 pywalc-0.2.1/setup.py
```

### Comparing `pywalc-0.1.1/LICENSE` & `pywalc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywalc-0.1.1/PKG-INFO` & `pywalc-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pywalc
-Version: 0.1.1
+Version: 0.2.1
 Summary: Change pywal color online
 Home-page: https://github.com/png261/pywalc
-Download-URL: https://github.com/png261/pywalc/archive/0.1.1.tar.gz
+Download-URL: https://github.com/png261/pywalc/archive/0.2.1.tar.gz
 Author: Phuong Nguyen
 Author-email: nhphuong.code@gmail.com
 License: MIT
 Keywords: pywalc wal colorscheme terminal-emulators changing-colorschemes
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pywalc-0.1.1/README.md` & `pywalc-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pywalc-0.1.1/pywalc/server.py` & `pywalc-0.2.1/pywalc/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,36 +87,36 @@
             return self.wallpaper.get_colors(id)
 
         @self.server.post("/wallpaper", tags=["wallpaper"])
         async def upload_wallpaper(files: List[UploadFile] = File(...)):
             return await self.wallpaper.upload(files)
 
         @self.server.get("/wallpaper/load", tags=["wallpaper"])
-        def load_wallpaper():
-            return self.wallpaper.load()
+        def apply_wallpaper():
+            return self.wallpaper.apply()
 
         @self.server.get("/color", tags=["color"])
         def get_colors():
             return self.color.get()
 
         @self.server.put("/color", tags=["color"])
         async def update_color(colors: Request):
             return await self.color.update(colors)
 
         @self.server.get("/color/load", tags=["color"])
-        def load_colors():
-            return self.color.load(self.wallpaper.get_current())
+        def apply_color():
+            return self.color.apply(self.wallpaper.get_current())
 
         @self.server.get("/theme", tags=["theme"])
         def get_themes():
             return self.theme.get()
 
         @self.server.get("/theme/{category}/{name}", tags=["theme"])
-        def set_theme(name, category):
-            return self.theme.set(name, category)
+        def get_theme_color(name, category):
+            return self.theme.get_color(name, category)
 
         @self.server.get("/sys", tags=["system"])
         def get_system_info():
             return {"os": OS, "name": socket.gethostname()}
 
         @self.server.get("/reset", tags=["system"])
         def reset():
```

### Comparing `pywalc-0.1.1/pywalc/settings.py` & `pywalc-0.2.1/pywalc/settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import pywal
 import os
-from . import util
 
-__version__ = "0.1.1"
+__version__ = "0.2.1"
 
 HOME = pywal.settings.HOME
 XDG_CACHE_DIR = os.getenv("XDG_CACHE_HOME", os.path.join(HOME, ".cache"))
 
 PYWALL_CACHE = pywal.settings.CACHE_DIR
-PYWAL_FILE_PATH = os.path.join(PYWALL_CACHE, "colors.json")
-PYWAL_DATA = pywal.colors.file(PYWAL_FILE_PATH)
-PYWAL_CURRENT_WALLPAPER = util.read_file(os.path.join(PYWALL_CACHE, "wal"))[0]
+PYWAL_DATA_FILE = os.path.join(PYWALL_CACHE, "colors.json")
 PYWAL_MODULE_DIR = pywal.settings.MODULE_DIR
 
 MODULE_DIR = os.path.dirname(__file__)
 CACHE_DIR = os.path.join(XDG_CACHE_DIR, "pywalc")
 WALLPAPER_DIR = os.path.join(CACHE_DIR, "wallpapers")
 BACKUP_FILE = os.path.join(CACHE_DIR, "backup.json")
```

### Comparing `pywalc-0.1.1/pywalc/static/css/style.css` & `pywalc-0.2.1/pywalc/static/css/style.css`

 * *Files identical despite different names*

### Comparing `pywalc-0.1.1/pywalc/static/js/Actions.js` & `pywalc-0.2.1/pywalc/static/js/Actions.js`

 * *Files identical despite different names*

### Comparing `pywalc-0.1.1/pywalc/static/js/Color.js` & `pywalc-0.2.1/pywalc/static/js/Color.js`

 * *Files identical despite different names*

### Comparing `pywalc-0.1.1/pywalc/static/js/Theme.js` & `pywalc-0.2.1/pywalc/static/js/Theme.js`

 * *Files identical despite different names*

### Comparing `pywalc-0.1.1/pywalc/static/js/Wallpaper.js` & `pywalc-0.2.1/pywalc/static/js/Wallpaper.js`

 * *Files identical despite different names*

### Comparing `pywalc-0.1.1/pywalc/static/js/api.js` & `pywalc-0.2.1/pywalc/static/js/api.js`

 * *Files identical despite different names*

### Comparing `pywalc-0.1.1/pywalc/static/js/data.js` & `pywalc-0.2.1/pywalc/static/js/data.js`

 * *Files identical despite different names*

### Comparing `pywalc-0.1.1/pywalc/static/js/main.js` & `pywalc-0.2.1/pywalc/static/js/main.js`

 * *Files identical despite different names*

### Comparing `pywalc-0.1.1/pywalc/templates/index.html` & `pywalc-0.2.1/pywalc/templates/index.html`

 * *Files identical despite different names*

### Comparing `pywalc-0.1.1/pywalc/util.py` & `pywalc-0.2.1/pywalc/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-"""
-Misc helper functions.
-"""
 import json
-import logging
 import os
 import shutil
-import sys
 import qrcode
 import io
+import uuid
 
 
 def read_file(input_file):
     """Read data from a file and trim newlines."""
     with open(input_file, "r") as file:
         return file.read().splitlines()
 
@@ -33,15 +29,15 @@
     """Write data to a file."""
     create_dir(os.path.dirname(export_file))
 
     try:
         with open(export_file, mode) as file:
             file.write(data)
     except PermissionError:
-        logging.warning("Couldn't write to %s.", export_file)
+        print("Couldn't write to %s.", export_file)
 
 
 def save_file_json(data, export_file):
     """Write data to a json file."""
     create_dir(os.path.dirname(export_file))
 
     with open(export_file, "w") as file:
@@ -49,37 +45,25 @@
 
 
 def create_dir(directory):
     """Alias to create the cache dir."""
     os.makedirs(directory, exist_ok=True)
 
 
-def setup_logging():
-    """Logging config."""
-    logging.basicConfig(
-        format=(
-            "[%(levelname)s\033[0m] " "\033[1;31m%(module)s\033[0m: " "%(message)s"
-        ),
-        level=logging.INFO,
-        stream=sys.stdout,
-    )
-    logging.addLevelName(logging.ERROR, "\033[1;31mE")
-    logging.addLevelName(logging.INFO, "\033[1;32mI")
-    logging.addLevelName(logging.WARNING, "\033[1;33mW")
-
-
 def copy_dir(source, dest):
     try:
         shutil.copyfile(source, dest)
     except shutil.SameFileError:
         pass
 
 
-def show_ascii_qrcode(
-    url,
-):
+def show_ascii_qrcode(url):
     qr = qrcode.QRCode()
     qr.add_data(url)
     f = io.StringIO()
     qr.print_ascii(out=f)
     f.seek(0)
     print(f.read())
+
+
+def get_random_id():
+    return str(uuid.uuid1().hex)
```

### Comparing `pywalc-0.1.1/pywalc.egg-info/PKG-INFO` & `pywalc-0.2.1/pywalc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pywalc
-Version: 0.1.1
+Version: 0.2.1
 Summary: Change pywal color online
 Home-page: https://github.com/png261/pywalc
-Download-URL: https://github.com/png261/pywalc/archive/0.1.1.tar.gz
+Download-URL: https://github.com/png261/pywalc/archive/0.2.1.tar.gz
 Author: Phuong Nguyen
 Author-email: nhphuong.code@gmail.com
 License: MIT
 Keywords: pywalc wal colorscheme terminal-emulators changing-colorschemes
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pywalc-0.1.1/pywalc.egg-info/SOURCES.txt` & `pywalc-0.2.1/pywalc.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 pywalc/__init__.py
 pywalc/__main__.py
+pywalc/app.py
 pywalc/colors.py
+pywalc/pywal_util.py
 pywalc/server.py
 pywalc/settings.py
 pywalc/theme.py
 pywalc/util.py
 pywalc/wallpaper.py
 pywalc.egg-info/PKG-INFO
 pywalc.egg-info/SOURCES.txt
```

### Comparing `pywalc-0.1.1/setup.py` & `pywalc-0.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 LONG_DESC = open("README.md").read()
-VERSION = '0.1.1'
+VERSION = "0.2.1"
 DOWNLOAD = "https://github.com/png261/pywalc/archive/%s.tar.gz" % VERSION
 
 setuptools.setup(
     name="pywalc",
     version=VERSION,
     author="Phuong Nguyen",
     author_email="nhphuong.code@gmail.com",
```

