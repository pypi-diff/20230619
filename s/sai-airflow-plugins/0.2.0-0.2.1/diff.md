# Comparing `tmp/sai-airflow-plugins-0.2.0.tar.gz` & `tmp/sai-airflow-plugins-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sai-airflow-plugins-0.2.0.tar", last modified: Mon Jun 19 13:17:34 2023, max compression
+gzip compressed data, was "sai-airflow-plugins-0.2.1.tar", last modified: Mon Jun 19 13:39:07 2023, max compression
```

## Comparing `sai-airflow-plugins-0.2.0.tar` & `sai-airflow-plugins-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:34.777865 sai-airflow-plugins-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-19 13:17:34.777865 sai-airflow-plugins-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:34.773865 sai-airflow-plugins-0.2.0/sai_airflow_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:34.773865 sai-airflow-plugins-0.2.0/sai_airflow_plugins/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/hooks/fabric_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/hooks/mattermost_webhook_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:34.777865 sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/conditional_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/conditional_skip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/fabric_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/mattermost_webhook_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:34.777865 sai-airflow-plugins-0.2.0/sai_airflow_plugins/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/sensors/conditional_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/sensors/fabric_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:34.773865 sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-19 13:17:34.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-19 13:17:34.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:17:34.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-19 13:17:34.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 13:17:34.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-19 13:17:34.777865 sai-airflow-plugins-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:34.777865 sai-airflow-plugins-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/mocked_fabric_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/test_conditional_skip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/test_fabric_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/test_fabric_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/test_fabric_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/test_mattermost_webhook_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/test_mattermost_webhook_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:07.427754 sai-airflow-plugins-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-19 13:39:07.427754 sai-airflow-plugins-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:07.419754 sai-airflow-plugins-0.2.1/sai_airflow_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:07.423754 sai-airflow-plugins-0.2.1/sai_airflow_plugins/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins/hooks/fabric_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins/hooks/mattermost_webhook_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:07.423754 sai-airflow-plugins-0.2.1/sai_airflow_plugins/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins/operators/conditional_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins/operators/conditional_skip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins/operators/fabric_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins/operators/mattermost_webhook_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:07.423754 sai-airflow-plugins-0.2.1/sai_airflow_plugins/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins/sensors/conditional_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins/sensors/fabric_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:07.419754 sai-airflow-plugins-0.2.1/sai_airflow_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-19 13:39:07.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-19 13:39:07.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:39:07.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-19 13:39:07.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 13:39:07.000000 sai-airflow-plugins-0.2.1/sai_airflow_plugins.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-19 13:39:07.427754 sai-airflow-plugins-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:07.427754 sai-airflow-plugins-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/tests/mocked_fabric_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/tests/test_conditional_skip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/tests/test_fabric_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/tests/test_fabric_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/tests/test_fabric_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/tests/test_mattermost_webhook_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-19 13:38:56.000000 sai-airflow-plugins-0.2.1/tests/test_mattermost_webhook_operator.py
```

### Comparing `sai-airflow-plugins-0.2.0/LICENSE` & `sai-airflow-plugins-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/PKG-INFO` & `sai-airflow-plugins-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sai-airflow-plugins
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package with various operators, hooks and utilities for Apache Airflow
 Home-page: https://github.com/Slimmer-AI/sai-airflow-plugins
 Author: Slimmer.AI
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `sai-airflow-plugins-0.2.0/README.rst` & `sai-airflow-plugins-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/sai_airflow_plugins/hooks/fabric_hook.py` & `sai-airflow-plugins-0.2.1/sai_airflow_plugins/hooks/fabric_hook.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/sai_airflow_plugins/hooks/mattermost_webhook_hook.py` & `sai-airflow-plugins-0.2.1/sai_airflow_plugins/hooks/mattermost_webhook_hook.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/conditional_operators.py` & `sai-airflow-plugins-0.2.1/sai_airflow_plugins/operators/conditional_operators.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/conditional_skip_mixin.py` & `sai-airflow-plugins-0.2.1/sai_airflow_plugins/operators/conditional_skip_mixin.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/fabric_operator.py` & `sai-airflow-plugins-0.2.1/sai_airflow_plugins/operators/fabric_operator.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/mattermost_webhook_operator.py` & `sai-airflow-plugins-0.2.1/sai_airflow_plugins/operators/mattermost_webhook_operator.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/sai_airflow_plugins/sensors/conditional_sensors.py` & `sai-airflow-plugins-0.2.1/sai_airflow_plugins/sensors/conditional_sensors.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/sai_airflow_plugins/sensors/fabric_sensor.py` & `sai-airflow-plugins-0.2.1/sai_airflow_plugins/sensors/fabric_sensor.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/PKG-INFO` & `sai-airflow-plugins-0.2.1/sai_airflow_plugins.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sai-airflow-plugins
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package with various operators, hooks and utilities for Apache Airflow
 Home-page: https://github.com/Slimmer-AI/sai-airflow-plugins
 Author: Slimmer.AI
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/SOURCES.txt` & `sai-airflow-plugins-0.2.1/sai_airflow_plugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/setup.py` & `sai-airflow-plugins-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/tests/mocked_fabric_hook.py` & `sai-airflow-plugins-0.2.1/tests/mocked_fabric_hook.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/tests/test_conditional_skip_mixin.py` & `sai-airflow-plugins-0.2.1/tests/test_conditional_skip_mixin.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/tests/test_fabric_hook.py` & `sai-airflow-plugins-0.2.1/tests/test_fabric_hook.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/tests/test_fabric_operator.py` & `sai-airflow-plugins-0.2.1/tests/test_fabric_operator.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/tests/test_fabric_sensor.py` & `sai-airflow-plugins-0.2.1/tests/test_fabric_sensor.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/tests/test_mattermost_webhook_hook.py` & `sai-airflow-plugins-0.2.1/tests/test_mattermost_webhook_hook.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.2.0/tests/test_mattermost_webhook_operator.py` & `sai-airflow-plugins-0.2.1/tests/test_mattermost_webhook_operator.py`

 * *Files identical despite different names*

