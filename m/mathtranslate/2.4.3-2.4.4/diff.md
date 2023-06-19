# Comparing `tmp/mathtranslate-2.4.3.tar.gz` & `tmp/mathtranslate-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathtranslate-2.4.3.tar", last modified: Sat Jun 17 03:55:32 2023, max compression
+gzip compressed data, was "mathtranslate-2.4.4.tar", last modified: Mon Jun 19 04:45:41 2023, max compression
```

## Comparing `mathtranslate-2.4.3.tar` & `mathtranslate-2.4.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/process_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/tencentcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/translate_arxiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/translate_tex.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/upload_overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-17 03:55:32.000000 mathtranslate-2.4.3/mathtranslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-17 03:55:32.000000 mathtranslate-2.4.3/mathtranslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 03:55:32.000000 mathtranslate-2.4.3/mathtranslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-17 03:55:32.000000 mathtranslate-2.4.3/mathtranslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-17 03:55:32.000000 mathtranslate-2.4.3/mathtranslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-17 03:55:32.000000 mathtranslate-2.4.3/mathtranslate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.055761 mathtranslate-2.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-19 04:45:41.055761 mathtranslate-2.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.051761 mathtranslate-2.4.4/mathtranslate/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17599 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/process_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.051761 mathtranslate-2.4.4/mathtranslate/tencentcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.051761 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.051761 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.051761 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.051761 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.055761 mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.055761 mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/translate_arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/translate_tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/upload_overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.051761 mathtranslate-2.4.4/mathtranslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-19 04:45:41.000000 mathtranslate-2.4.4/mathtranslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-19 04:45:41.000000 mathtranslate-2.4.4/mathtranslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 04:45:41.000000 mathtranslate-2.4.4/mathtranslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-19 04:45:41.000000 mathtranslate-2.4.4/mathtranslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 04:45:41.000000 mathtranslate-2.4.4/mathtranslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 04:45:41.000000 mathtranslate-2.4.4/mathtranslate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 04:45:41.055761 mathtranslate-2.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/setup.py
```

### Comparing `mathtranslate-2.4.3/LICENSE` & `mathtranslate-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/PKG-INFO` & `mathtranslate-2.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.4.3
+Version: 2.4.4
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.4.3 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.4.4 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.4.3/README.md` & `mathtranslate-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/cache.py` & `mathtranslate-2.4.4/mathtranslate/cache.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/config.py` & `mathtranslate-2.4.4/mathtranslate/config.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/encoding.py` & `mathtranslate-2.4.4/mathtranslate/encoding.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/process_file.py` & `mathtranslate-2.4.4/mathtranslate/process_file.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/process_latex.py` & `mathtranslate-2.4.4/mathtranslate/process_latex.py`

 * *Files 2% similar despite different names*

```diff
@@ -476,7 +476,19 @@
         latex = latex.replace(match.group(), f'{math_code}_REPLACE{count}_NEWCOMMAND')
         full_newcommands.append(match.group(0))
         latex = replace_newcommand((name, n_arguments, content), latex)
         count += 1
     for i in range(count):
         latex = latex.replace(f'{math_code}_REPLACE{i}_NEWCOMMAND', full_newcommands[i])
     return latex
+
+
+def remove_bibnote(latex):
+    pattern = regex.compile(get_pattern_command_full('bibinfo', 2), regex.DOTALL)
+
+    def replace_function(match):
+        assert match.group(1) == 'bibinfo'
+        if match.group(3) == 'note':
+            return ''
+        else:
+            return match.group(0)
+    return pattern.sub(replace_function, latex)
```

### Comparing `mathtranslate-2.4.3/mathtranslate/process_text.py` & `mathtranslate-2.4.4/mathtranslate/process_text.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencent.py` & `mathtranslate-2.4.4/mathtranslate/tencent.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/__init__.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/__init__.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/abstract_client.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/abstract_model.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/common_client.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/credential.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/exception/__init__.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/http/__init__.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/http/request.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/profile/__init__.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/profile/client_profile.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/profile/http_profile.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/sign.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/__init__.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/__init__.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/models.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py` & `mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/translate.py` & `mathtranslate-2.4.4/mathtranslate/translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,16 @@
             cache.create_cache(hash_key)
 
         self.nbad = 0
         self.ntotal = 0
 
         latex_original = process_latex.remove_tex_comments(latex_original)
         latex_original = latex_original.replace(r'\mathbf', r'\boldsymbol')
+        # \bibinfo {note} is not working in xelatex
+        latex_original = process_latex.remove_bibnote(latex_original)
         latex_original = process_latex.process_newcommands(latex_original)
 
         latex_original = process_latex.replace_accent(latex_original)
         latex_original = process_latex.replace_special(latex_original)
 
         self.complete = process_latex.is_complete(latex_original)
         self.theorems = process_latex.get_theorems(latex_original)
```

### Comparing `mathtranslate-2.4.3/mathtranslate/translate_arxiv.py` & `mathtranslate-2.4.4/mathtranslate/translate_arxiv.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,14 +108,15 @@
     '''
     utils.check_update(require_updated=require_updated)
 
     import argparse
     parser = argparse.ArgumentParser()
     parser.add_argument("number", nargs='?', type=str, help='arxiv number')
     parser.add_argument("-o", type=str, help='output path')
+    parser.add_argument("--from_dir", action='store_true')
     parser.add_argument("--notranslate", action='store_true')  # debug option
     utils.add_arguments(parser)
     options = parser.parse_args(args)
     utils.process_options(options)
 
     if options.number is None:
         parser.print_help()
@@ -130,39 +131,44 @@
     else:
         output_path = options.o
 
     success = True
     cwd = os.getcwd()
     with tempfile.TemporaryDirectory() as temp_dir:
         print('temporary directory', temp_dir)
+        if options.from_dir:
+            shutil.copytree(number, temp_dir, dirs_exist_ok=True)
         os.chdir(temp_dir)
         # must os.chdir(cwd) whenever released!
         try:
-            try:
-                download_source_with_cache(number, download_path)
-            except BaseException:
-                print('Cannot download source, maybe network issue or wrong link')
-                os.chdir(cwd)
-                return False
-            if is_pdf(download_path):
-                # case 1
-                success = False
-            else:
-                content = gzip.decompress(open(download_path, "rb").read())
-                with open(download_path, "wb") as f:
-                    f.write(content)
+            if not options.from_dir:
                 try:
-                    # case 4
-                    with tarfile.open(download_path, mode='r') as f:
-                        f.extractall()
-                    os.remove(download_path)
-                except tarfile.ReadError:
-                    # case 2 or 3
-                    print('This is a pure text file')
-                    shutil.move(download_path, 'main.tex')
+                    download_source_with_cache(number, download_path)
+                except BaseException:
+                    print('Cannot download source, maybe network issue or wrong link')
+                    os.chdir(cwd)
+                    return False
+                if is_pdf(download_path):
+                    # case 1
+                    success = False
+                else:
+                    content = gzip.decompress(open(download_path, "rb").read())
+                    with open(download_path, "wb") as f:
+                        f.write(content)
+                    try:
+                        # case 4
+                        with tarfile.open(download_path, mode='r') as f:
+                            f.extractall()
+                        os.remove(download_path)
+                    except tarfile.ReadError:
+                        # case 2 or 3
+                        print('This is a pure text file')
+                        shutil.move(download_path, 'main.tex')
+                    success = translate_dir('.', options)
+            else:
                 success = translate_dir('.', options)
             os.chdir(cwd)
             if success:
                 # case 3 or 4
                 zipdir(temp_dir, output_path)
         except BaseException as e:
             # first go back otherwise tempfile trying to delete the current directory that python is running in
```

### Comparing `mathtranslate-2.4.3/mathtranslate/translate_tex.py` & `mathtranslate-2.4.4/mathtranslate/translate_tex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/upload_overleaf.py` & `mathtranslate-2.4.4/mathtranslate/upload_overleaf.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate/utils.py` & `mathtranslate-2.4.4/mathtranslate/utils.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/mathtranslate.egg-info/PKG-INFO` & `mathtranslate-2.4.4/mathtranslate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.4.3
+Version: 2.4.4
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.4.3 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.4.4 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.4.3/mathtranslate.egg-info/SOURCES.txt` & `mathtranslate-2.4.4/mathtranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.3/setup.py` & `mathtranslate-2.4.4/setup.py`

 * *Files identical despite different names*

