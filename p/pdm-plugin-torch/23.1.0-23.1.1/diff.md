# Comparing `tmp/pdm-plugin-torch-23.1.0.tar.gz` & `tmp/pdm-plugin-torch-23.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-plugin-torch-23.1.0.tar", last modified: Wed Apr 19 14:11:32 2023, max compression
+gzip compressed data, was "pdm-plugin-torch-23.1.1.tar", last modified: Mon Jun 19 08:11:32 2023, max compression
```

## Comparing `pdm-plugin-torch-23.1.0.tar` & `pdm-plugin-torch-23.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      614 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    10841 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/LICENSE-APACHE
--rw-r--r--   0        0        0     1074 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/LICENSE-MIT
--rw-r--r--   0        0        0     2885 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/README.md
--rw-r--r--   0        0        0        9 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/pdm-plugin-torch/pdm_plugin_torch/__init__.py
--rw-r--r--   0        0        0     1295 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/pdm-plugin-torch/pdm_plugin_torch/config.py
--rw-r--r--   0        0        0    16668 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/pdm-plugin-torch/pdm_plugin_torch/main.py
--rw-r--r--   0        0        0     1590 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2370 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/tests/conftest.py
--rw-r--r--   0        0        0      574 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/tests/fixtures/cpu-only/pyproject.toml
--rw-r--r--   0        0        0     2018 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/tests/test_lock.py
--rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 pdm-plugin-torch-23.1.0/PKG-INFO
+-rw-r--r--   0        0        0      780 2023-06-19 08:11:04.702906 pdm-plugin-torch-23.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0    10841 2023-06-19 08:11:04.702906 pdm-plugin-torch-23.1.1/LICENSE-APACHE
+-rw-r--r--   0        0        0     1074 2023-06-19 08:11:04.702906 pdm-plugin-torch-23.1.1/LICENSE-MIT
+-rw-r--r--   0        0        0     2885 2023-06-19 08:11:04.702906 pdm-plugin-torch-23.1.1/README.md
+-rw-r--r--   0        0        0        9 2023-06-19 08:11:04.702906 pdm-plugin-torch-23.1.1/pdm-plugin-torch/pdm_plugin_torch/__init__.py
+-rw-r--r--   0        0        0     1295 2023-06-19 08:11:04.702906 pdm-plugin-torch-23.1.1/pdm-plugin-torch/pdm_plugin_torch/config.py
+-rw-r--r--   0        0        0    16736 2023-06-19 08:11:04.702906 pdm-plugin-torch-23.1.1/pdm-plugin-torch/pdm_plugin_torch/main.py
+-rw-r--r--   0        0        0     1590 2023-06-19 08:11:04.702906 pdm-plugin-torch-23.1.1/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-06-19 08:11:04.702906 pdm-plugin-torch-23.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2370 2023-06-19 08:11:04.702906 pdm-plugin-torch-23.1.1/tests/conftest.py
+-rw-r--r--   0        0        0      574 2023-06-19 08:11:04.702906 pdm-plugin-torch-23.1.1/tests/fixtures/cpu-only/pyproject.toml
+-rw-r--r--   0        0        0     2018 2023-06-19 08:11:04.702906 pdm-plugin-torch-23.1.1/tests/test_lock.py
+-rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 pdm-plugin-torch-23.1.1/PKG-INFO
```

### Comparing `pdm-plugin-torch-23.1.0/CHANGELOG.md` & `pdm-plugin-torch-23.1.1/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [23.1.1] - 2023-06-15
+
+- Fix a bug where 2.5.0 would crash with an assertion.
+
 ## [23.1.0] - 2023-04-19
 
 - Adds support for PDM 2.5.0
 
 ## [23.0.0] - 2023-03-01
 
 This is the initial release
 
-[Unreleased]: https://github.com/EmbarkStudios/pdm-plugin-torch/compare/23.1.0...HEAD
+[Unreleased]: https://github.com/EmbarkStudios/pdm-plugin-torch/compare/23.1.1...HEAD
+[23.1.1]: https://github.com/EmbarkStudios/pdm-plugin-torch/compare/23.1.0...23.1.1
 [23.1.0]: https://github.com/EmbarkStudios/pdm-plugin-torch/compare/23.0.0...23.1.0
 [23.0.0]: https://github.com/EmbarkStudios/pdm-plugin-torch/releases/tag/23.0.0
```

### Comparing `pdm-plugin-torch-23.1.0/LICENSE-APACHE` & `pdm-plugin-torch-23.1.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `pdm-plugin-torch-23.1.0/LICENSE-MIT` & `pdm-plugin-torch-23.1.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `pdm-plugin-torch-23.1.0/README.md` & `pdm-plugin-torch-23.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pdm-plugin-torch-23.1.0/pdm-plugin-torch/pdm_plugin_torch/config.py` & `pdm-plugin-torch-23.1.1/pdm-plugin-torch/pdm_plugin_torch/config.py`

 * *Files identical despite different names*

### Comparing `pdm-plugin-torch-23.1.0/pdm-plugin-torch/pdm_plugin_torch/main.py` & `pdm-plugin-torch-23.1.1/pdm-plugin-torch/pdm_plugin_torch/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,16 +384,20 @@
     if is_pdm22:
         return project.pyproject["tool"]["pdm"]["plugins"]["torch"]
 
     else:
         return project.pyproject.settings["plugins"]["torch"]
 
 
-class InstallCommand:
+class InstallCommand(BaseCommand):
     name = "install"
+    description = "Install torch packages from lockfile"
+
+    def add_arguments(self, parser):
+        parser.add_argument("api", help="the api to use, e.g. cuda version or rocm")
 
     def handle(self, project: Project, options: dict):
         plugin_config = Configuration.from_toml(get_settings(project))
 
         resolves = plugin_config.variants
         if options.api not in resolves:
             raise ValueError(
@@ -420,16 +424,24 @@
                 }
             ],
             requirements=reqs,
             lockfile=spec_for_version,
         )
 
 
-class LockCommand:
+class LockCommand(BaseCommand):
     name = "lock"
+    description = "Lock Torch and its dependencies to a specific version"
+
+    def add_arguments(self, parser):
+        parser.add_argument(
+            "--check",
+            help="validate that the lockfile is up to date",
+            action="store_true",
+        )
 
     def handle(self, project: Project, options: dict):
         plugin_config = Configuration.from_toml(get_settings(project))
 
         if options.check:
             is_updated = check_lockfile(project, plugin_config.lockfile)
             if not is_updated:
@@ -470,34 +482,25 @@
         write_lockfile(project, plugin_config.lockfile, results)
 
 
 class TorchCommand(BaseCommand):
     """Generate a lockfile for torch specifically."""
 
     name = "torch"
+    description = "Manage torch dependencies"
 
     def add_arguments(self, parser):
-        subparsers = parser.add_subparsers(help="sub-command help", dest="command")
-        subparsers.required = True
-
-        parser_install = subparsers.add_parser(
-            "install", help="install a torch variant"
-        )
-        parser_install.add_argument(
-            "api", help="the api to use, e.g. cuda version or rocm"
+        subparsers = parser.add_subparsers(
+            title="Sub commands", help="sub-command help", dest="command"
         )
-        parser_install.set_defaults(command=InstallCommand())
 
-        parser_lock = subparsers.add_parser("lock", help="update lockfile")
-        parser_lock.add_argument(
-            "--check",
-            help="validate that the lockfile is up to date",
-            action="store_true",
-        )
-        parser_lock.set_defaults(command=LockCommand())
+        LockCommand.register_to(subparsers)
+        InstallCommand.register_to(subparsers)
+
+        self.parser = parser
 
-    def handle(self, project, options):
-        options.command.handle(project, options)
+    def handle(self, project: Project, options) -> None:
+        self.parser.print_help()
 
 
 def torch_plugin(core: Core):
     core.register_command(TorchCommand, "torch")
```

### Comparing `pdm-plugin-torch-23.1.0/pyproject.toml` & `pdm-plugin-torch-23.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pdm-plugin-torch"
-version = "23.1.0"
+version = "23.1.1"
 description = "A plugin to help installing torch versions"
 authors = [
     { name = "Embark Studios", email = "python@embark-studios.com" },
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dependencies = []
```

### Comparing `pdm-plugin-torch-23.1.0/tests/conftest.py` & `pdm-plugin-torch-23.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-plugin-torch-23.1.0/tests/fixtures/cpu-only/pyproject.toml` & `pdm-plugin-torch-23.1.1/tests/fixtures/cpu-only/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-plugin-torch-23.1.0/tests/test_lock.py` & `pdm-plugin-torch-23.1.1/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `pdm-plugin-torch-23.1.0/PKG-INFO` & `pdm-plugin-torch-23.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-plugin-torch
-Version: 23.1.0
+Version: 23.1.1
 Summary: A plugin to help installing torch versions
 License: MIT
 Author-email: Embark Studios <python@embark-studios.com>
 Requires-Python: >=3.8
 Project-URL: repository, https://github.com/EmbarkStudios/pdm-plugin-torch
 Description-Content-Type: text/markdown
```

