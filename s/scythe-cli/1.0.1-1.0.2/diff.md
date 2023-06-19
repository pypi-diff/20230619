# Comparing `tmp/scythe_cli-1.0.1.tar.gz` & `tmp/scythe_cli-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scythe_cli-1.0.1.tar", max compression
+gzip compressed data, was "scythe_cli-1.0.2.tar", max compression
```

## Comparing `scythe_cli-1.0.1.tar` & `scythe_cli-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2022-04-01 04:53:11.923617 scythe_cli-1.0.1/README.md
--rw-r--r--   0        0        0      814 2023-06-19 01:52:41.252976 scythe_cli-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-04-01 04:53:11.926950 scythe_cli-1.0.1/scythe_cli/__init__.py
--rw-r--r--   0        0        0       32 2023-05-22 00:56:50.311829 scythe_cli-1.0.1/scythe_cli/application/__init__.py
--rw-r--r--   0        0        0     2708 2023-06-19 01:52:33.746396 scythe_cli-1.0.1/scythe_cli/application/application.py
--rw-r--r--   0        0        0     3761 2023-06-19 01:50:13.664722 scythe_cli-1.0.1/scythe_cli/application/quickstart.py
--rw-r--r--   0        0        0     1820 2023-06-17 05:39:33.414672 scythe_cli-1.0.1/scythe_cli/application/timers.py
--rw-r--r--   0        0        0       54 2023-06-17 04:43:26.019412 scythe_cli-1.0.1/scythe_cli/console.py
--rw-r--r--   0        0        0      283 2023-06-19 01:49:07.585265 scythe_cli-1.0.1/scythe_cli/constants.py
--rw-r--r--   0        0        0     9330 2023-06-19 01:35:56.348376 scythe_cli-1.0.1/scythe_cli/harvest.py
--rw-r--r--   0        0        0     3667 2023-06-19 01:42:32.798498 scythe_cli-1.0.1/scythe_cli/ui/apps.py
--rw-r--r--   0        0        0      246 2023-05-22 00:56:50.311829 scythe_cli-1.0.1/scythe_cli/ui/styles/app.css
--rw-r--r--   0        0        0      639 2023-05-22 00:56:50.311829 scythe_cli-1.0.1/scythe_cli/ui/styles/timer-container.css
--rw-r--r--   0        0        0      893 2023-06-19 01:33:10.186369 scythe_cli-1.0.1/scythe_cli/ui/styles/timer-modal.css
--rw-r--r--   0        0        0      888 2023-05-22 00:56:50.311829 scythe_cli-1.0.1/scythe_cli/ui/styles/timer.css
--rw-r--r--   0        0        0      147 2023-06-17 18:46:28.388935 scythe_cli-1.0.1/scythe_cli/ui/widgets/__init__.py
--rw-r--r--   0        0        0      228 2023-05-22 00:56:50.311829 scythe_cli-1.0.1/scythe_cli/ui/widgets/actions.py
--rw-r--r--   0        0        0     4775 2023-06-19 01:24:39.446966 scythe_cli-1.0.1/scythe_cli/ui/widgets/timer.py
--rw-r--r--   0        0        0     4513 2023-06-19 01:42:25.861888 scythe_cli-1.0.1/scythe_cli/ui/widgets/timer_container.py
--rw-r--r--   0        0        0     5877 2023-06-19 01:43:45.151241 scythe_cli-1.0.1/scythe_cli/ui/widgets/timer_modal.py
--rw-r--r--   0        0        0     2146 2023-06-18 17:17:49.220101 scythe_cli-1.0.1/scythe_cli/utils.py
--rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 scythe_cli-1.0.1/setup.py
--rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 scythe_cli-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-04-01 04:53:11.923617 scythe_cli-1.0.2/README.md
+-rw-r--r--   0        0        0      814 2023-06-19 01:53:38.042331 scythe_cli-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-04-01 04:53:11.926950 scythe_cli-1.0.2/scythe_cli/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-22 00:56:50.311829 scythe_cli-1.0.2/scythe_cli/application/__init__.py
+-rw-r--r--   0        0        0     2661 2023-06-19 01:53:39.978976 scythe_cli-1.0.2/scythe_cli/application/application.py
+-rw-r--r--   0        0        0     3761 2023-06-19 01:50:13.664722 scythe_cli-1.0.2/scythe_cli/application/quickstart.py
+-rw-r--r--   0        0        0     1820 2023-06-17 05:39:33.414672 scythe_cli-1.0.2/scythe_cli/application/timers.py
+-rw-r--r--   0        0        0       54 2023-06-17 04:43:26.019412 scythe_cli-1.0.2/scythe_cli/console.py
+-rw-r--r--   0        0        0      283 2023-06-19 01:49:07.585265 scythe_cli-1.0.2/scythe_cli/constants.py
+-rw-r--r--   0        0        0     9330 2023-06-19 01:35:56.348376 scythe_cli-1.0.2/scythe_cli/harvest.py
+-rw-r--r--   0        0        0     3667 2023-06-19 01:42:32.798498 scythe_cli-1.0.2/scythe_cli/ui/apps.py
+-rw-r--r--   0        0        0      246 2023-05-22 00:56:50.311829 scythe_cli-1.0.2/scythe_cli/ui/styles/app.css
+-rw-r--r--   0        0        0      639 2023-05-22 00:56:50.311829 scythe_cli-1.0.2/scythe_cli/ui/styles/timer-container.css
+-rw-r--r--   0        0        0      893 2023-06-19 01:33:10.186369 scythe_cli-1.0.2/scythe_cli/ui/styles/timer-modal.css
+-rw-r--r--   0        0        0      888 2023-05-22 00:56:50.311829 scythe_cli-1.0.2/scythe_cli/ui/styles/timer.css
+-rw-r--r--   0        0        0      147 2023-06-17 18:46:28.388935 scythe_cli-1.0.2/scythe_cli/ui/widgets/__init__.py
+-rw-r--r--   0        0        0      228 2023-05-22 00:56:50.311829 scythe_cli-1.0.2/scythe_cli/ui/widgets/actions.py
+-rw-r--r--   0        0        0     4775 2023-06-19 01:24:39.446966 scythe_cli-1.0.2/scythe_cli/ui/widgets/timer.py
+-rw-r--r--   0        0        0     4513 2023-06-19 01:42:25.861888 scythe_cli-1.0.2/scythe_cli/ui/widgets/timer_container.py
+-rw-r--r--   0        0        0     5877 2023-06-19 01:43:45.151241 scythe_cli-1.0.2/scythe_cli/ui/widgets/timer_modal.py
+-rw-r--r--   0        0        0     2146 2023-06-18 17:17:49.220101 scythe_cli-1.0.2/scythe_cli/utils.py
+-rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 scythe_cli-1.0.2/setup.py
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 scythe_cli-1.0.2/PKG-INFO
```

### Comparing `scythe_cli-1.0.1/pyproject.toml` & `scythe_cli-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scythe-cli"
-version = "1.0.1"
+version = "1.0.2"
 description = "A Harvest is always better with a good tool"
 authors = ["Sean Collings <seanrcollings@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/seanrcollings/scythe"
 
 [tool.poetry.dependencies]
```

### Comparing `scythe_cli-1.0.1/scythe_cli/application/application.py` & `scythe_cli-1.0.2/scythe_cli/application/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,16 @@
 import keyring
 
 from scythe_cli.harvest import AsyncHarvest, Harvest, HarvestError
 from scythe_cli.console import console
 from scythe_cli import utils
 
 arc.configure(
-    environment="development",
-    debug=True,
     present=arc.PresentConfig(color=arc.ColorConfig(accent=color.fg.hex("#fa5d00"))),
-    version="1.0.1",
+    version="1.0.2",
 )
 
 from scythe_cli.application import quickstart
 from scythe_cli.application import timers
 
 
 @arc.command("scythe")
```

### Comparing `scythe_cli-1.0.1/scythe_cli/application/quickstart.py` & `scythe_cli-1.0.2/scythe_cli/application/quickstart.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.1/scythe_cli/application/timers.py` & `scythe_cli-1.0.2/scythe_cli/application/timers.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.1/scythe_cli/harvest.py` & `scythe_cli-1.0.2/scythe_cli/harvest.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.1/scythe_cli/ui/apps.py` & `scythe_cli-1.0.2/scythe_cli/ui/apps.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.1/scythe_cli/ui/styles/timer-container.css` & `scythe_cli-1.0.2/scythe_cli/ui/styles/timer-container.css`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.1/scythe_cli/ui/styles/timer-modal.css` & `scythe_cli-1.0.2/scythe_cli/ui/styles/timer-modal.css`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.1/scythe_cli/ui/styles/timer.css` & `scythe_cli-1.0.2/scythe_cli/ui/styles/timer.css`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.1/scythe_cli/ui/widgets/timer.py` & `scythe_cli-1.0.2/scythe_cli/ui/widgets/timer.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.1/scythe_cli/ui/widgets/timer_container.py` & `scythe_cli-1.0.2/scythe_cli/ui/widgets/timer_container.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.1/scythe_cli/ui/widgets/timer_modal.py` & `scythe_cli-1.0.2/scythe_cli/ui/widgets/timer_modal.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.1/scythe_cli/utils.py` & `scythe_cli-1.0.2/scythe_cli/utils.py`

 * *Files identical despite different names*

### Comparing `scythe_cli-1.0.1/setup.py` & `scythe_cli-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'xdg>=5.1.1,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['scythe = scythe_cli.application.application:scythe']}
 
 setup_kwargs = {
     'name': 'scythe-cli',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'A Harvest is always better with a good tool',
     'long_description': '',
     'author': 'Sean Collings',
     'author_email': 'seanrcollings@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/seanrcollings/scythe',
```

### Comparing `scythe_cli-1.0.1/PKG-INFO` & `scythe_cli-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scythe-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Harvest is always better with a good tool
 Home-page: https://github.com/seanrcollings/scythe
 License: MIT
 Author: Sean Collings
 Author-email: seanrcollings@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

