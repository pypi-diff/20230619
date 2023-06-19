# Comparing `tmp/web_ext_helper-1.0.7.tar.gz` & `tmp/web_ext_helper-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_ext_helper-1.0.7.tar", max compression
+gzip compressed data, was "web_ext_helper-1.0.8.tar", max compression
```

## Comparing `web_ext_helper-1.0.7.tar` & `web_ext_helper-1.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.0.7/LICENSE
--rw-r--r--   0        0        0      654 2023-06-18 17:37:12.434008 web_ext_helper-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     1754 2023-06-17 20:34:00.666577 web_ext_helper-1.0.7/README.md
--rw-r--r--   0        0        0      237 2023-06-18 17:20:13.515316 web_ext_helper-1.0.7/web_ext_helper/classes.py
--rw-r--r--   0        0        0      547 2023-06-18 17:36:56.873136 web_ext_helper-1.0.7/web_ext_helper/functions.py
--rw-r--r--   0        0        0    17958 2023-06-18 17:37:01.118273 web_ext_helper-1.0.7/web_ext_helper/web_ext_helper.py
--rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 web_ext_helper-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.0.8/LICENSE
+-rw-r--r--   0        0        0      654 2023-06-19 16:21:17.751282 web_ext_helper-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1754 2023-06-17 20:34:00.666577 web_ext_helper-1.0.8/README.md
+-rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.0.8/web_ext_helper/classes.py
+-rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.0.8/web_ext_helper/functions.py
+-rw-r--r--   0        0        0    18142 2023-06-19 16:21:10.777540 web_ext_helper-1.0.8/web_ext_helper/web_ext_helper.py
+-rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 web_ext_helper-1.0.8/PKG-INFO
```

### Comparing `web_ext_helper-1.0.7/LICENSE` & `web_ext_helper-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.0.7/pyproject.toml` & `web_ext_helper-1.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web-ext-helper"
-version = "1.0.7"
+version = "1.0.8"
 description = "A simple cli tool that helps you building your web extensions."
 authors = ["AppSolves <appsolves@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "web_ext_helper"}]
 
 [tool.poetry.dependencies]
```

### Comparing `web_ext_helper-1.0.7/README.md` & `web_ext_helper-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.0.7/web_ext_helper/functions.py` & `web_ext_helper-1.0.8/web_ext_helper/functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import time
 import jwt
 import typer
-from .classes import bcolors
+
+try:
+    from .classes import bcolors
+except ImportError:
+    from classes import bcolors
 
 
 def error(message: str):
     typer.echo(f"{bcolors.FAIL}Error: {message}{bcolors.ENDC}", err=True)
     raise typer.Exit(1)
```

### Comparing `web_ext_helper-1.0.7/web_ext_helper/web_ext_helper.py` & `web_ext_helper-1.0.8/web_ext_helper/web_ext_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import os
 import json
-import time
 import shutil
 import typer
 import zipfile
 import rich.progress
 import requests as req
 import subprocess as sp
 from PIL import Image
 from dotenv import load_dotenv
 from appdirs import user_cache_dir
-from .functions import error, generate_jwt
-from .classes import bcolors
 
-cached_app_build_dir = f"{user_cache_dir('web-ext-helper', False)}/build"
-cached_app_data_env_dir = f"{user_cache_dir('web-ext-helper', False)}/data/.env"
+try:
+    from .functions import error, generate_jwt
+    from .classes import bcolors
+except ImportError:
+    from functions import error, generate_jwt
+    from classes import bcolors
+
+cached_app_build_dir = os.path.join(user_cache_dir("web-ext-helper", False), "build")
+cached_app_data_env_dir = os.path.join(
+    user_cache_dir("web-ext-helper", False), "data", ".env"
+)
 cached_app_dir = os.path.dirname(os.path.dirname(cached_app_build_dir))
 os.makedirs(cached_app_build_dir, exist_ok=True)
 os.makedirs(os.path.dirname(cached_app_data_env_dir), exist_ok=True)
 
 load_dotenv(cached_app_data_env_dir)
 
-
 app = typer.Typer()
 typer.clear()
 
 try:
     with open("src/manifest.json", "r") as manifest_file:
         manifest_data = json.load(manifest_file)
 
@@ -83,15 +88,15 @@
                             task,
                             advance=progress_percentage
                             - progress.tasks[task].completed,
                             description=description,
                         )
 
     typer.echo(
-        f"\n{bcolors.OKGREEN}Extension built successfully in {bcolors.OKCYAN}{progress.tasks[task].finished_time:.2f}{bcolors.OKGREEN} seconds.{bcolors.ENDC}"
+        f"\n{bcolors.OKGREEN}Extension built successfully in {bcolors.PURPLE}{progress.tasks[task].finished_time:.2f}{bcolors.OKGREEN} seconds.{bcolors.ENDC}"
     )
 
 
 @app.command(help="Validate the extension", name="validate")
 def __validate__():
     if not os.path.exists("src/manifest.json"):
         error("src/manifest.json not found")
@@ -141,103 +146,98 @@
         )
         raise typer.Exit(1)
     except sp.CalledProcessError as e:
         typer.echo(f"{bcolors.FAIL}{e.stderr.decode()}{bcolors.ENDC}", err=True)
         raise typer.Exit(1)
 
 
-@app.command(help="Sign the extension for mozilla addons", name="sign")
+@app.command(help="Sign the extension for self-hosting the extension", name="sign")
 def __sign__():
     if not os.path.exists("src/manifest.json"):
         error("src/manifest.json not found")
         raise typer.Exit(1)
 
-    typer.echo(f"{bcolors.OKCYAN}Signing extension...{bcolors.ENDC}")
+    with rich.progress.Progress(
+        "[progress.description]{task.description}",
+        "[progress.percentage]{task.percentage:>3.0f}%",
+        rich.progress.BarColumn(),
+        rich.progress.TimeRemainingColumn(),
+    ) as progress:
+        task = progress.add_task("[green]Signing extension...", total=100)
 
-    try:
-        sp.run(
-            [
-                r"C:\Program Files\nodejs\web-ext.cmd",
-                "sign",
-                "--source-dir",
-                "src",
-            ],
-        )
-    except FileNotFoundError:
-        error(
-            "web-ext not found. Please install it globally using 'npm install -g web-ext'"
-        )
-        raise typer.Exit(1)
-    except sp.CalledProcessError as e:
-        typer.echo(f"{bcolors.FAIL}{e.stderr.decode()}{bcolors.ENDC}", err=True)
-        raise typer.Exit(1)
+        try:
+            api_key, api_secret = os.environ.get("AMO_API_KEY", None), os.environ.get(
+                "AMO_API_SECRET", None
+            )
+
+            if api_key is None or api_secret is None:
+                error(
+                    "AMO_API_KEY and AMO_API_SECRET environment variables not found.\nPlease set them using the set-amo-credentials command before publishing the extension"
+                )
+                raise typer.Exit(1)
+
+            sp.run(
+                [
+                    r"C:\Program Files\nodejs\web-ext.cmd",
+                    "sign",
+                    "--channel=unlisted",
+                    "--source-dir",
+                    "src",
+                    f"--api-key={api_key}",
+                    f"--api-secret={api_secret}",
+                ],
+            )
+            progress.update(task, advance=100, description="Signing extension...")
+        except FileNotFoundError:
+            error(
+                "web-ext not found. Please install it globally using 'npm install -g web-ext'"
+            )
+            raise typer.Exit(1)
+        except sp.CalledProcessError as e:
+            typer.echo(f"{bcolors.FAIL}{e.stderr.decode()}{bcolors.ENDC}", err=True)
+            raise typer.Exit(1)
 
 
 @app.command(help="Publish the extension to the Mozilla Addons Store", name="publish")
-def __publish__(
-    build: bool = typer.Option(
-        False, "--build", "-b", help="Build the extension before publishing"
-    ),
-):
+def __publish__():
     if not os.path.exists("src/manifest.json"):
         error("src/manifest.json not found")
         raise typer.Exit(1)
 
-    if build:
-        __build__()
-        time.sleep(1)
-        typer.clear()
-    else:
-        if not os.path.exists(
-            f"{cached_app_build_dir}/{manifest_name_lower}-{manifest_version}.zip"
-        ):
-            error("Build not found. Please build the extension first")
-            raise typer.Exit(1)
-
     typer.echo(f"{bcolors.OKCYAN}Publishing extension...{bcolors.ENDC}")
 
     try:
-        with open("src/manifest.json", "r") as manifest_file:
-            manifest_data = json.load(manifest_file)
-            guid = manifest_data["browser_specific_settings"]["gecko"]["id"]
-
         api_key, api_secret = os.environ.get("AMO_API_KEY", None), os.environ.get(
             "AMO_API_SECRET", None
         )
 
         if api_key is None or api_secret is None:
             error(
                 "AMO_API_KEY and AMO_API_SECRET environment variables not found.\nPlease set them using the set-amo-credentials command before publishing the extension"
             )
             raise typer.Exit(1)
 
-        jwt_token = generate_jwt(api_key, api_secret)
-
-        req.put(
-            f"https://addons.mozilla.org/api/v5/addons/addon/{guid}",
-            headers={
-                "Authorization": f"JWT {jwt_token}",
-            },
-            files={
-                "upload": (
-                    f"{manifest_name_lower}-{manifest_version}.zip",
-                    open(
-                        f"{cached_app_build_dir}/{manifest_name_lower}-{manifest_version}.zip",
-                        "rb",
-                    ),
-                    "application/zip",
-                )
-            },
+        sp.run(
+            [
+                r"C:\Program Files\nodejs\web-ext.cmd",
+                "sign",
+                "--channel=listed",
+                "--source-dir",
+                "src",
+                f"--api-key={api_key}",
+                f"--api-secret={api_secret}",
+            ],
         )
-
-        typer.echo(
-            f"{bcolors.OKGREEN}Successfully published extension to the Mozilla Addons Store: {bcolors.OKCYAN}{manifest_name} v{manifest_version}{bcolors.ENDC}"
+    except FileNotFoundError:
+        error(
+            "web-ext not found. Please install it globally using 'npm install -g web-ext'"
         )
-    except req.exceptions.HTTPError as e:
-        typer.echo(f"{bcolors.FAIL}{e.response.text}{bcolors.ENDC}", err=True)
+        raise typer.Exit(1)
+    except sp.CalledProcessError as e:
+        typer.echo(f"{bcolors.FAIL}{e.stderr.decode()}{bcolors.ENDC}", err=True)
         raise typer.Exit(1)
 
 
 @app.command(help="Delete the extension from the Mozilla Addons Store", name="delete")
 def __delete__(confirm: bool = typer.Option(False, "--confirm", "-c")):
     if not os.path.exists("src/manifest.json"):
         error("src/manifest.json not found")
```

### Comparing `web_ext_helper-1.0.7/PKG-INFO` & `web_ext_helper-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ext-helper
-Version: 1.0.7
+Version: 1.0.8
 Summary: A simple cli tool that helps you building your web extensions.
 License: GPL-3.0-or-later
 Author: AppSolves
 Author-email: appsolves@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

