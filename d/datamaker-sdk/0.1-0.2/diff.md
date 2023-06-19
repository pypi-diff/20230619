# Comparing `tmp/datamaker-sdk-0.1.tar.gz` & `tmp/datamaker-sdk-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamaker-sdk-0.1.tar", last modified: Wed Oct 12 02:46:31 2022, max compression
+gzip compressed data, was "datamaker-sdk-0.2.tar", last modified: Mon Jun 19 01:23:42 2023, max compression
```

## Comparing `datamaker-sdk-0.1.tar` & `datamaker-sdk-0.2.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxrwxr-x   0 hslee     (1000) hslee     (1000)        0 2022-10-12 02:46:31.333638 datamaker-sdk-0.1/
--rw-rw-r--   0 hslee     (1000) hslee     (1000)     1101 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/LICENSE
--rw-rw-r--   0 hslee     (1000) hslee     (1000)      870 2022-10-12 02:46:31.333638 datamaker-sdk-0.1/PKG-INFO
--rw-rw-r--   0 hslee     (1000) hslee     (1000)        0 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/README.md
-drwxrwxr-x   0 hslee     (1000) hslee     (1000)        0 2022-10-12 02:46:31.333638 datamaker-sdk-0.1/datamaker/
--rw-rw-r--   0 hslee     (1000) hslee     (1000)        0 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/__init__.py
-drwxrwxr-x   0 hslee     (1000) hslee     (1000)        0 2022-10-12 02:46:31.333638 datamaker-sdk-0.1/datamaker/client/
--rw-rw-r--   0 hslee     (1000) hslee     (1000)     3526 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/client/__init__.py
--rw-rw-r--   0 hslee     (1000) hslee     (1000)      405 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/client/exceptions.py
-drwxrwxr-x   0 hslee     (1000) hslee     (1000)        0 2022-10-12 02:46:31.333638 datamaker-sdk-0.1/datamaker/client/mixins/
--rw-rw-r--   0 hslee     (1000) hslee     (1000)        0 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/client/mixins/__init__.py
--rw-rw-r--   0 hslee     (1000) hslee     (1000)      906 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/client/mixins/annotation.py
--rw-rw-r--   0 hslee     (1000) hslee     (1000)     1783 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/client/mixins/dataset.py
--rw-rw-r--   0 hslee     (1000) hslee     (1000)      337 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/client/mixins/integration.py
--rw-rw-r--   0 hslee     (1000) hslee     (1000)      904 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/client/mixins/ml.py
--rw-rw-r--   0 hslee     (1000) hslee     (1000)      420 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/client/utils.py
-drwxrwxr-x   0 hslee     (1000) hslee     (1000)        0 2022-10-12 02:46:31.333638 datamaker-sdk-0.1/datamaker/plugins/
--rw-rw-r--   0 hslee     (1000) hslee     (1000)     1049 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/plugins/__init__.py
--rw-rw-r--   0 hslee     (1000) hslee     (1000)     1676 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/plugins/exports.py
--rw-rw-r--   0 hslee     (1000) hslee     (1000)        0 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/plugins/imports.py
--rw-rw-r--   0 hslee     (1000) hslee     (1000)     6894 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/plugins/neural_networks.py
--rw-rw-r--   0 hslee     (1000) hslee     (1000)      455 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/plugins/preprocessors.py
-drwxrwxr-x   0 hslee     (1000) hslee     (1000)        0 2022-10-12 02:46:31.333638 datamaker-sdk-0.1/datamaker/utils/
--rw-rw-r--   0 hslee     (1000) hslee     (1000)        0 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/utils/__init__.py
--rw-rw-r--   0 hslee     (1000) hslee     (1000)     1940 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/utils/file.py
--rw-rw-r--   0 hslee     (1000) hslee     (1000)     1401 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/datamaker/utils/logger.py
-drwxrwxr-x   0 hslee     (1000) hslee     (1000)        0 2022-10-12 02:46:31.333638 datamaker-sdk-0.1/datamaker_sdk.egg-info/
--rw-rw-r--   0 hslee     (1000) hslee     (1000)      870 2022-10-12 02:46:31.000000 datamaker-sdk-0.1/datamaker_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 hslee     (1000) hslee     (1000)      750 2022-10-12 02:46:31.000000 datamaker-sdk-0.1/datamaker_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 hslee     (1000) hslee     (1000)        1 2022-10-12 02:46:31.000000 datamaker-sdk-0.1/datamaker_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 hslee     (1000) hslee     (1000)      106 2022-10-12 02:46:31.000000 datamaker-sdk-0.1/datamaker_sdk.egg-info/requires.txt
--rw-rw-r--   0 hslee     (1000) hslee     (1000)       10 2022-10-12 02:46:31.000000 datamaker-sdk-0.1/datamaker_sdk.egg-info/top_level.txt
--rw-rw-r--   0 hslee     (1000) hslee     (1000)      107 2022-10-12 02:28:52.000000 datamaker-sdk-0.1/pyproject.toml
--rw-rw-r--   0 hslee     (1000) hslee     (1000)     1004 2022-10-12 02:46:31.333638 datamaker-sdk-0.1/setup.cfg
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.689411 datamaker-sdk-0.2/
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.685410 datamaker-sdk-0.2/.github/
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.685410 datamaker-sdk-0.2/.github/workflows/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1131 2023-06-19 01:23:35.000000 datamaker-sdk-0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      221 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/.gitignore
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1101 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/LICENSE
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      870 2023-06-19 01:23:42.689411 datamaker-sdk-0.2/PKG-INFO
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/README.md
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.685410 datamaker-sdk-0.2/datamaker/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/__init__.py
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.685410 datamaker-sdk-0.2/datamaker/client/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     3526 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/client/__init__.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      405 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/client/exceptions.py
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.689411 datamaker-sdk-0.2/datamaker/client/mixins/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/client/mixins/__init__.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1021 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/client/mixins/annotation.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     3922 2023-06-19 01:07:34.000000 datamaker-sdk-0.2/datamaker/client/mixins/dataset.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      337 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/client/mixins/integration.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      904 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/client/mixins/ml.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      420 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/client/utils.py
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.689411 datamaker-sdk-0.2/datamaker/plugins/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1049 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/plugins/__init__.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1676 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/plugins/exports.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/plugins/imports.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     6894 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/plugins/neural_networks.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      455 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/plugins/preprocessors.py
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.689411 datamaker-sdk-0.2/datamaker/utils/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/utils/__init__.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1940 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/utils/file.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1401 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/utils/logger.py
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.689411 datamaker-sdk-0.2/datamaker_sdk.egg-info/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      870 2023-06-19 01:23:42.000000 datamaker-sdk-0.2/datamaker_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      798 2023-06-19 01:23:42.000000 datamaker-sdk-0.2/datamaker_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)        1 2023-06-19 01:23:42.000000 datamaker-sdk-0.2/datamaker_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      106 2023-06-19 01:23:42.000000 datamaker-sdk-0.2/datamaker_sdk.egg-info/requires.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)       10 2023-06-19 01:23:42.000000 datamaker-sdk-0.2/datamaker_sdk.egg-info/top_level.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      162 2023-06-19 01:23:35.000000 datamaker-sdk-0.2/pyproject.toml
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1004 2023-06-19 01:23:42.689411 datamaker-sdk-0.2/setup.cfg
```

### Comparing `datamaker-sdk-0.1/LICENSE` & `datamaker-sdk-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.1/PKG-INFO` & `datamaker-sdk-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaker-sdk
-Version: 0.1
+Version: 0.2
 Summary: datamaker sdk
 Home-page: https://www.datamaker.io
 Author: datamaker
 Author-email: developer@datamaker.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamaker-sdk-0.1/datamaker/client/__init__.py` & `datamaker-sdk-0.2/datamaker/client/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.1/datamaker/client/mixins/annotation.py` & `datamaker-sdk-0.2/datamaker/client/mixins/annotation.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,10 +20,14 @@
         url_conversion = get_default_url_conversion(url_conversion, files_fields=['files'])
         return self._list(path, payload, url_conversion, list_all)
 
     def create_labels(self, data):
         path = 'labels/'
         return self._post(path, payload=data)
 
+    def create_label_tags(self, data):
+        path = 'label_tags/'
+        return self._post(path, payload=data)
+
     def set_tags_labels(self, data, params=None):
         path = 'labels/set_tags/'
         return self._post(path, payload=data, params=params)
```

### Comparing `datamaker-sdk-0.1/datamaker/client/mixins/ml.py` & `datamaker-sdk-0.2/datamaker/client/mixins/ml.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.1/datamaker/plugins/__init__.py` & `datamaker-sdk-0.2/datamaker/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.1/datamaker/plugins/exports.py` & `datamaker-sdk-0.2/datamaker/plugins/exports.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.1/datamaker/plugins/neural_networks.py` & `datamaker-sdk-0.2/datamaker/plugins/neural_networks.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.1/datamaker/utils/file.py` & `datamaker-sdk-0.2/datamaker/utils/file.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.1/datamaker/utils/logger.py` & `datamaker-sdk-0.2/datamaker/utils/logger.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.1/datamaker_sdk.egg-info/PKG-INFO` & `datamaker-sdk-0.2/datamaker_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaker-sdk
-Version: 0.1
+Version: 0.2
 Summary: datamaker sdk
 Home-page: https://www.datamaker.io
 Author: datamaker
 Author-email: developer@datamaker.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamaker-sdk-0.1/datamaker_sdk.egg-info/SOURCES.txt` & `datamaker-sdk-0.2/datamaker_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+.gitignore
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
+.github/workflows/python-publish.yml
 datamaker/__init__.py
 datamaker/client/__init__.py
 datamaker/client/exceptions.py
 datamaker/client/utils.py
 datamaker/client/mixins/__init__.py
 datamaker/client/mixins/annotation.py
 datamaker/client/mixins/dataset.py
```

### Comparing `datamaker-sdk-0.1/setup.cfg` & `datamaker-sdk-0.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.6
 install_requires = 
-	django==4.0.4
-	djangorestframework==3.13.1
-	django-constance[database]==2.8.0
-	requests==2.26.0
-	tqdm==4.62.3
+	django>=4.0.4
+	djangorestframework>=3.13.1
+	django-constance[database]>=2.8.0
+	requests>=2.26.0
+	tqdm>=4.62.3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

