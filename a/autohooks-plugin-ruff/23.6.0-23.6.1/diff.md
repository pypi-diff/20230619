# Comparing `tmp/autohooks_plugin_ruff-23.6.0.tar.gz` & `tmp/autohooks_plugin_ruff-23.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autohooks_plugin_ruff-23.6.0.tar", max compression
+gzip compressed data, was "autohooks_plugin_ruff-23.6.1.tar", max compression
```

## Comparing `autohooks_plugin_ruff-23.6.0.tar` & `autohooks_plugin_ruff-23.6.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-06-09 11:36:55.475726 autohooks_plugin_ruff-23.6.0/LICENSE
--rw-r--r--   0        0        0     2145 2023-06-16 07:22:54.520279 autohooks_plugin_ruff-23.6.0/README.md
--rw-r--r--   0        0        0      121 2023-06-16 07:22:54.520279 autohooks_plugin_ruff-23.6.0/autohooks/plugins/ruff/__init__.py
--rw-r--r--   0        0        0      103 2023-06-16 07:27:40.543097 autohooks_plugin_ruff-23.6.0/autohooks/plugins/ruff/__version__.py
--rw-r--r--   0        0        0     2649 2023-06-16 07:27:40.543097 autohooks_plugin_ruff-23.6.0/autohooks/plugins/ruff/ruff.py
--rw-r--r--   0        0        0    62507 2023-06-16 07:22:54.524278 autohooks_plugin_ruff-23.6.0/poetry.lock
--rw-r--r--   0        0        0     2180 2023-06-16 07:27:40.547097 autohooks_plugin_ruff-23.6.0/pyproject.toml
--rw-r--r--   0        0        0     3323 1970-01-01 00:00:00.000000 autohooks_plugin_ruff-23.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-19 05:52:39.387050 autohooks_plugin_ruff-23.6.1/LICENSE
+-rw-r--r--   0        0        0     2145 2023-06-19 05:52:39.387050 autohooks_plugin_ruff-23.6.1/README.md
+-rw-r--r--   0        0        0      121 2023-06-19 05:52:39.387050 autohooks_plugin_ruff-23.6.1/autohooks/plugins/ruff/__init__.py
+-rw-r--r--   0        0        0      103 2023-06-19 05:52:39.387050 autohooks_plugin_ruff-23.6.1/autohooks/plugins/ruff/__version__.py
+-rw-r--r--   0        0        0     2622 2023-06-19 05:52:39.387050 autohooks_plugin_ruff-23.6.1/autohooks/plugins/ruff/ruff.py
+-rw-r--r--   0        0        0    62507 2023-06-19 05:52:39.391050 autohooks_plugin_ruff-23.6.1/poetry.lock
+-rw-r--r--   0        0        0     2180 2023-06-19 05:52:39.391050 autohooks_plugin_ruff-23.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3323 1970-01-01 00:00:00.000000 autohooks_plugin_ruff-23.6.1/PKG-INFO
```

### Comparing `autohooks_plugin_ruff-23.6.0/LICENSE` & `autohooks_plugin_ruff-23.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autohooks_plugin_ruff-23.6.0/README.md` & `autohooks_plugin_ruff-23.6.1/README.md`

 * *Files identical despite different names*

### Comparing `autohooks_plugin_ruff-23.6.0/autohooks/plugins/ruff/ruff.py` & `autohooks_plugin_ruff-23.6.1/autohooks/plugins/ruff/ruff.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     **kwargs,  # pylint: disable=unused-argument
 ) -> int:
     check_ruff_installed()
 
     files = [f for f in get_staged_status() if str(f.path).endswith(".py")]
 
     if not files:
-        ok("No staged files to format.")
+        ok("No staged files to lint.")
         return 0
 
     cmd = ["ruff", "check"] + get_ruff_arguments(get_ruff_config(config))
 
     if report_progress:
         report_progress.init(len(files))
 
@@ -69,15 +69,15 @@
             try:
                 subprocess.run(
                     cmd + [str(file.absolute_path())],
                     check=True,
                     capture_output=True,
                 )
                 ok(f"Linting {file.path} was successful.")
-            except subprocess.CalledProcessError as e:  # pylint: disable=C0103
+            except subprocess.CalledProcessError as e:
                 ret = e.returncode
                 format_errors = (
                     e.stdout.decode(
                         encoding=sys.getdefaultencoding(), errors="replace"
                     )
                     .rstrip()
                     .split("\n")
```

### Comparing `autohooks_plugin_ruff-23.6.0/poetry.lock` & `autohooks_plugin_ruff-23.6.1/poetry.lock`

 * *Files identical despite different names*

### Comparing `autohooks_plugin_ruff-23.6.0/pyproject.toml` & `autohooks_plugin_ruff-23.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "autohooks-plugin-ruff"
-version = "23.6.0"
+version = "23.6.1"
 description = "An autohooks plugin for python code formatting via ruff"
 license = "GPL-3.0-or-later"
 authors = ["Greenbone AG <info@greenbone.net>", "jorgegomzar <jorge.gomzar@gmail.com"]
 readme = "README.md"
 homepage = "https://github.com/greenbone/autohooks-plugin-ruff"
 repository = "https://github.com/greeenbone/autohooks-plugin-ruff"
 documentation = ""
```

### Comparing `autohooks_plugin_ruff-23.6.0/PKG-INFO` & `autohooks_plugin_ruff-23.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autohooks-plugin-ruff
-Version: 23.6.0
+Version: 23.6.1
 Summary: An autohooks plugin for python code formatting via ruff
 Home-page: https://github.com/greenbone/autohooks-plugin-ruff
 License: GPL-3.0-or-later
 Keywords: git,formatting,linting,hooks,ruff
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.7.2,<4.0.0
```

