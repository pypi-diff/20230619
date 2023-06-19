# Comparing `tmp/critical_node-0.0.1.tar.gz` & `tmp/critical_node-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "critical_node-0.0.1.tar", last modified: Mon Jun 19 01:47:55 2023, max compression
+gzip compressed data, was "critical_node-0.0.2.tar", last modified: Mon Jun 19 02:10:58 2023, max compression
```

## Comparing `critical_node-0.0.1.tar` & `critical_node-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 01:47:55.064873 critical_node-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-06-19 01:42:48.000000 critical_node-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      642 2023-06-19 01:47:55.063869 critical_node-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      137 2023-06-19 01:45:57.000000 critical_node-0.0.1/README.md
--rw-rw-rw-   0        0        0      583 2023-06-19 01:43:58.000000 critical_node-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 01:47:55.064873 critical_node-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-19 01:47:55.034406 critical_node-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 01:47:55.040385 critical_node-0.0.1/src/critical_node/
--rw-rw-rw-   0        0        0       89 2023-06-19 01:42:04.000000 critical_node-0.0.1/src/critical_node/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:47:55.062880 critical_node-0.0.1/src/critical_node/model/
--rw-rw-rw-   0        0        0       41 2023-06-19 01:42:04.000000 critical_node-0.0.1/src/critical_node/model/test2.py
--rw-rw-rw-   0        0        0       78 2023-06-19 01:37:38.000000 critical_node-0.0.1/src/critical_node/test1.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:47:55.060886 critical_node-0.0.1/src/critical_node.egg-info/
--rw-rw-rw-   0        0        0      642 2023-06-19 01:47:55.000000 critical_node-0.0.1/src/critical_node.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-06-19 01:47:55.000000 critical_node-0.0.1/src/critical_node.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 01:47:55.000000 critical_node-0.0.1/src/critical_node.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-19 01:47:55.000000 critical_node-0.0.1/src/critical_node.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 02:10:58.639342 critical_node-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-06-19 01:42:48.000000 critical_node-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      642 2023-06-19 02:10:58.638430 critical_node-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      137 2023-06-19 01:45:57.000000 critical_node-0.0.2/README.md
+-rw-rw-rw-   0        0        0      583 2023-06-19 02:10:37.000000 critical_node-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 02:10:58.639342 critical_node-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 02:10:58.614927 critical_node-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 02:10:58.619910 critical_node-0.0.2/src/critical_node/
+-rw-rw-rw-   0        0        0       90 2023-06-19 02:09:35.000000 critical_node-0.0.2/src/critical_node/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:10:58.637511 critical_node-0.0.2/src/critical_node/model/
+-rw-rw-rw-   0        0        0       41 2023-06-19 01:42:04.000000 critical_node-0.0.2/src/critical_node/model/test2.py
+-rw-rw-rw-   0        0        0       78 2023-06-19 01:37:38.000000 critical_node-0.0.2/src/critical_node/test1.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:10:58.636454 critical_node-0.0.2/src/critical_node.egg-info/
+-rw-rw-rw-   0        0        0      642 2023-06-19 02:10:58.000000 critical_node-0.0.2/src/critical_node.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-06-19 02:10:58.000000 critical_node-0.0.2/src/critical_node.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 02:10:58.000000 critical_node-0.0.2/src/critical_node.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-19 02:10:58.000000 critical_node-0.0.2/src/critical_node.egg-info/top_level.txt
```

### Comparing `critical_node-0.0.1/LICENSE` & `critical_node-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `critical_node-0.0.1/PKG-INFO` & `critical_node-0.0.2/src/critical_node.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: critical_node
-Version: 0.0.1
+Name: critical-node
+Version: 0.0.2
 Summary: A small text
 Author-email: YunHengWang <1975667609@qq.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `critical_node-0.0.1/pyproject.toml` & `critical_node-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "critical_node"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="YunHengWang", email="1975667609@qq.com" },
 ]
 description = "A small text"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `critical_node-0.0.1/src/critical_node.egg-info/PKG-INFO` & `critical_node-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: critical-node
-Version: 0.0.1
+Name: critical_node
+Version: 0.0.2
 Summary: A small text
 Author-email: YunHengWang <1975667609@qq.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

