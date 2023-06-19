# Comparing `tmp/scythe_cli-1.0.0.tar.gz` & `tmp/scythe_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scythe_cli-1.0.0.tar", max compression
+gzip compressed data, was "scythe_cli-1.0.1.tar", max compression
```

## Comparing `scythe_cli-1.0.0.tar` & `scythe_cli-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2022-04-01 04:53:11.923617 scythe_cli-1.0.0/README.md
--rw-r--r--   0        0        0      906 2023-06-19 01:47:29.176073 scythe_cli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-04-01 04:53:11.926950 scythe_cli-1.0.0/scythe_cli/__init__.py
--rw-r--r--   0        0        0       32 2023-05-22 00:56:50.311829 scythe_cli-1.0.0/scythe_cli/application/__init__.py
--rw-r--r--   0        0        0     2708 2023-06-17 18:30:54.415252 scythe_cli-1.0.0/scythe_cli/application/application.py
--rw-r--r--   0        0        0     3761 2023-06-17 05:39:35.404656 scythe_cli-1.0.0/scythe_cli/application/quickstart.py
--rw-r--r--   0        0        0     1820 2023-06-17 05:39:33.414672 scythe_cli-1.0.0/scythe_cli/application/timers.py
--rw-r--r--   0        0        0       54 2023-06-17 04:43:26.019412 scythe_cli-1.0.0/scythe_cli/console.py
--rw-r--r--   0        0        0      556 2023-06-17 03:59:43.092914 scythe_cli-1.0.0/scythe_cli/constants.py
--rw-r--r--   0        0        0     9330 2023-06-19 01:35:56.348376 scythe_cli-1.0.0/scythe_cli/harvest.py
--rw-r--r--   0        0        0     3667 2023-06-19 01:42:32.798498 scythe_cli-1.0.0/scythe_cli/ui/apps.py
--rw-r--r--   0        0        0      246 2023-05-22 00:56:50.311829 scythe_cli-1.0.0/scythe_cli/ui/styles/app.css
--rw-r--r--   0        0        0      639 2023-05-22 00:56:50.311829 scythe_cli-1.0.0/scythe_cli/ui/styles/timer-container.css
--rw-r--r--   0        0        0      893 2023-06-19 01:33:10.186369 scythe_cli-1.0.0/scythe_cli/ui/styles/timer-modal.css
--rw-r--r--   0        0        0      888 2023-05-22 00:56:50.311829 scythe_cli-1.0.0/scythe_cli/ui/styles/timer.css
--rw-r--r--   0        0        0      147 2023-06-17 18:46:28.388935 scythe_cli-1.0.0/scythe_cli/ui/widgets/__init__.py
--rw-r--r--   0        0        0      228 2023-05-22 00:56:50.311829 scythe_cli-1.0.0/scythe_cli/ui/widgets/actions.py
--rw-r--r--   0        0        0     4775 2023-06-19 01:24:39.446966 scythe_cli-1.0.0/scythe_cli/ui/widgets/timer.py
--rw-r--r--   0        0        0     4513 2023-06-19 01:42:25.861888 scythe_cli-1.0.0/scythe_cli/ui/widgets/timer_container.py
--rw-r--r--   0        0        0     5877 2023-06-19 01:43:45.151241 scythe_cli-1.0.0/scythe_cli/ui/widgets/timer_modal.py
--rw-r--r--   0        0        0     2146 2023-06-18 17:17:49.220101 scythe_cli-1.0.0/scythe_cli/utils.py
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 scythe_cli-1.0.0/setup.py
--rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 scythe_cli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-04-01 04:53:11.923617 scythe_cli-1.0.1/README.md
+-rw-r--r--   0        0        0      814 2023-06-19 01:52:41.252976 scythe_cli-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-04-01 04:53:11.926950 scythe_cli-1.0.1/scythe_cli/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-22 00:56:50.311829 scythe_cli-1.0.1/scythe_cli/application/__init__.py
+-rw-r--r--   0        0        0     2708 2023-06-19 01:52:33.746396 scythe_cli-1.0.1/scythe_cli/application/application.py
+-rw-r--r--   0        0        0     3761 2023-06-19 01:50:13.664722 scythe_cli-1.0.1/scythe_cli/application/quickstart.py
+-rw-r--r--   0        0        0     1820 2023-06-17 05:39:33.414672 scythe_cli-1.0.1/scythe_cli/application/timers.py
+-rw-r--r--   0        0        0       54 2023-06-17 04:43:26.019412 scythe_cli-1.0.1/scythe_cli/console.py
+-rw-r--r--   0        0        0      283 2023-06-19 01:49:07.585265 scythe_cli-1.0.1/scythe_cli/constants.py
+-rw-r--r--   0        0        0     9330 2023-06-19 01:35:56.348376 scythe_cli-1.0.1/scythe_cli/harvest.py
+-rw-r--r--   0        0        0     3667 2023-06-19 01:42:32.798498 scythe_cli-1.0.1/scythe_cli/ui/apps.py
+-rw-r--r--   0        0        0      246 2023-05-22 00:56:50.311829 scythe_cli-1.0.1/scythe_cli/ui/styles/app.css
+-rw-r--r--   0        0        0      639 2023-05-22 00:56:50.311829 scythe_cli-1.0.1/scythe_cli/ui/styles/timer-container.css
+-rw-r--r--   0        0        0      893 2023-06-19 01:33:10.186369 scythe_cli-1.0.1/scythe_cli/ui/styles/timer-modal.css
+-rw-r--r--   0        0        0      888 2023-05-22 00:56:50.311829 scythe_cli-1.0.1/scythe_cli/ui/styles/timer.css
+-rw-r--r--   0        0        0      147 2023-06-17 18:46:28.388935 scythe_cli-1.0.1/scythe_cli/ui/widgets/__init__.py
+-rw-r--r--   0        0        0      228 2023-05-22 00:56:50.311829 scythe_cli-1.0.1/scythe_cli/ui/widgets/actions.py
+-rw-r--r--   0        0        0     4775 2023-06-19 01:24:39.446966 scythe_cli-1.0.1/scythe_cli/ui/widgets/timer.py
+-rw-r--r--   0        0        0     4513 2023-06-19 01:42:25.861888 scythe_cli-1.0.1/scythe_cli/ui/widgets/timer_container.py
+-rw-r--r--   0        0        0     5877 2023-06-19 01:43:45.151241 scythe_cli-1.0.1/scythe_cli/ui/widgets/timer_modal.py
+-rw-r--r--   0        0        0     2146 2023-06-18 17:17:49.220101 scythe_cli-1.0.1/scythe_cli/utils.py
+-rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 scythe_cli-1.0.1/setup.py
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 scythe_cli-1.0.1/PKG-INFO
```

### Comparing `scythe_cli-1.0.0/pyproject.toml` & `scythe_cli-1.0.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 [tool.poetry]
 name = "scythe-cli"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Harvest is always better with a good tool"
 authors = ["Sean Collings <seanrcollings@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/seanrcollings/scythe"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.25.1"
 xdg = "^5.1.1"
-pydantic = "^1.9.0"
 arc-cli = "^8.4.0"
-oyaml = "^1.0"
-diskcache = "^5.4.0"
-textual = {extras = ["dev"], version = "^0.27.0"}
+textual = {version = "^0.27.0"}
 httpx = "^0.24.0"
-toml = "^0.10.2"
 msgspec = "^0.15.1"
 keyring = "^23.13.1"
 
-
 [tool.poetry.dev-dependencies]
 black = "^20.8b1"
 mypy = "^0.800"
 pylint = "^2.7.0"
 types-requests = "^2.27.7"
 types-PyYAML = "^6.0.3"
```

### Comparing `scythe_cli-1.0.0/scythe_cli/application/application.py` & `scythe_cli-1.0.1/scythe_cli/application/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from scythe_cli.console import console
 from scythe_cli import utils
 
 arc.configure(
     environment="development",
     debug=True,
     present=arc.PresentConfig(color=arc.ColorConfig(accent=color.fg.hex("#fa5d00"))),
-    version="1.0.0",
+    version="1.0.1",
 )
 
 from scythe_cli.application import quickstart
 from scythe_cli.application import timers
 
 
 @arc.command("scythe")
```

### Comparing `scythe_cli-1.0.0/scythe_cli/application/quickstart.py` & `scythe_cli-1.0.1/scythe_cli/application/quickstart.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.0/scythe_cli/application/timers.py` & `scythe_cli-1.0.1/scythe_cli/application/timers.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.0/scythe_cli/harvest.py` & `scythe_cli-1.0.1/scythe_cli/harvest.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.0/scythe_cli/ui/apps.py` & `scythe_cli-1.0.1/scythe_cli/ui/apps.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.0/scythe_cli/ui/styles/timer-container.css` & `scythe_cli-1.0.1/scythe_cli/ui/styles/timer-container.css`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.0/scythe_cli/ui/styles/timer-modal.css` & `scythe_cli-1.0.1/scythe_cli/ui/styles/timer-modal.css`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.0/scythe_cli/ui/styles/timer.css` & `scythe_cli-1.0.1/scythe_cli/ui/styles/timer.css`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.0/scythe_cli/ui/widgets/timer.py` & `scythe_cli-1.0.1/scythe_cli/ui/widgets/timer.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.0/scythe_cli/ui/widgets/timer_container.py` & `scythe_cli-1.0.1/scythe_cli/ui/widgets/timer_container.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.0/scythe_cli/ui/widgets/timer_modal.py` & `scythe_cli-1.0.1/scythe_cli/ui/widgets/timer_modal.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.0/scythe_cli/utils.py` & `scythe_cli-1.0.1/scythe_cli/utils.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.0/setup.py` & `scythe_cli-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,31 +8,27 @@
  'scythe_cli.ui.widgets']
 
 package_data = \
 {'': ['*'], 'scythe_cli.ui': ['styles/*']}
 
 install_requires = \
 ['arc-cli>=8.4.0,<9.0.0',
- 'diskcache>=5.4.0,<6.0.0',
  'httpx>=0.24.0,<0.25.0',
  'keyring>=23.13.1,<24.0.0',
  'msgspec>=0.15.1,<0.16.0',
- 'oyaml>=1.0,<2.0',
- 'pydantic>=1.9.0,<2.0.0',
  'requests>=2.25.1,<3.0.0',
- 'textual[dev]>=0.27.0,<0.28.0',
- 'toml>=0.10.2,<0.11.0',
+ 'textual>=0.27.0,<0.28.0',
  'xdg>=5.1.1,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['scythe = scythe_cli.application.application:scythe']}
 
 setup_kwargs = {
     'name': 'scythe-cli',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'A Harvest is always better with a good tool',
     'long_description': '',
     'author': 'Sean Collings',
     'author_email': 'seanrcollings@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/seanrcollings/scythe',
```

### Comparing `scythe_cli-1.0.0/PKG-INFO` & `scythe_cli-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: scythe-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Harvest is always better with a good tool
 Home-page: https://github.com/seanrcollings/scythe
 License: MIT
 Author: Sean Collings
 Author-email: seanrcollings@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arc-cli (>=8.4.0,<9.0.0)
-Requires-Dist: diskcache (>=5.4.0,<6.0.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: keyring (>=23.13.1,<24.0.0)
 Requires-Dist: msgspec (>=0.15.1,<0.16.0)
-Requires-Dist: oyaml (>=1.0,<2.0)
-Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
-Requires-Dist: textual[dev] (>=0.27.0,<0.28.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: textual (>=0.27.0,<0.28.0)
 Requires-Dist: xdg (>=5.1.1,<6.0.0)
 Description-Content-Type: text/markdown
```

