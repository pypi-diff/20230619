# Comparing `tmp/okx_exchange_api-1.0.2.tar.gz` & `tmp/okx_exchange_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okx_exchange_api-1.0.2.tar", last modified: Mon Jun 19 07:56:51 2023, max compression
+gzip compressed data, was "okx_exchange_api-1.0.3.tar", last modified: Mon Jun 19 08:03:50 2023, max compression
```

## Comparing `okx_exchange_api-1.0.2.tar` & `okx_exchange_api-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:51.090928 okx_exchange_api-1.0.2/
--rw-rw-rw-   0        0        0      936 2023-06-19 07:56:51.090928 okx_exchange_api-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-06-19 06:35:06.000000 okx_exchange_api-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:51.089928 okx_exchange_api-1.0.2/okx_exchange_api.egg-info/
--rw-rw-rw-   0        0        0      936 2023-06-19 07:56:51.000000 okx_exchange_api-1.0.2/okx_exchange_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-06-19 07:56:51.000000 okx_exchange_api-1.0.2/okx_exchange_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 07:56:51.000000 okx_exchange_api-1.0.2/okx_exchange_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-19 07:56:51.000000 okx_exchange_api-1.0.2/okx_exchange_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 07:56:51.000000 okx_exchange_api-1.0.2/okx_exchange_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 07:56:51.090928 okx_exchange_api-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1904 2023-06-19 07:55:44.000000 okx_exchange_api-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:03:50.901131 okx_exchange_api-1.0.3/
+-rw-rw-rw-   0        0        0      936 2023-06-19 08:03:50.900130 okx_exchange_api-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-06-19 06:35:06.000000 okx_exchange_api-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 08:03:50.892179 okx_exchange_api-1.0.3/okx_exchange_api/
+-rw-rw-rw-   0        0        0       93 2019-04-17 10:24:31.000000 okx_exchange_api-1.0.3/okx_exchange_api/__init__.py
+-rw-rw-rw-   0        0        0     3249 2019-04-17 10:24:31.000000 okx_exchange_api-1.0.3/okx_exchange_api/account_api.py
+-rw-rw-rw-   0        0        0     2616 2019-04-17 10:24:31.000000 okx_exchange_api-1.0.3/okx_exchange_api/client.py
+-rw-rw-rw-   0        0        0     4963 2019-04-17 10:24:31.000000 okx_exchange_api-1.0.3/okx_exchange_api/consts.py
+-rw-rw-rw-   0        0        0     2065 2019-04-17 10:24:31.000000 okx_exchange_api-1.0.3/okx_exchange_api/ett_api.py
+-rw-rw-rw-   0        0        0     1279 2019-10-20 08:46:56.000000 okx_exchange_api-1.0.3/okx_exchange_api/exceptions.py
+-rw-rw-rw-   0        0        0     7819 2019-04-17 10:24:31.000000 okx_exchange_api-1.0.3/okx_exchange_api/futures_api.py
+-rw-rw-rw-   0        0        0     6921 2019-04-17 10:24:31.000000 okx_exchange_api-1.0.3/okx_exchange_api/lever_api.py
+-rw-rw-rw-   0        0        0     6268 2019-04-17 10:24:31.000000 okx_exchange_api-1.0.3/okx_exchange_api/spot_api.py
+-rw-rw-rw-   0        0        0     7034 2019-04-17 10:24:31.000000 okx_exchange_api-1.0.3/okx_exchange_api/swap_api.py
+-rw-rw-rw-   0        0        0     1365 2019-04-17 10:24:31.000000 okx_exchange_api-1.0.3/okx_exchange_api/utils.py
+-rw-rw-rw-   0        0        0      768 2019-04-17 10:24:31.000000 okx_exchange_api-1.0.3/okx_exchange_api/websocket.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:03:50.900130 okx_exchange_api-1.0.3/okx_exchange_api.egg-info/
+-rw-rw-rw-   0        0        0      936 2023-06-19 08:03:50.000000 okx_exchange_api-1.0.3/okx_exchange_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2023-06-19 08:03:50.000000 okx_exchange_api-1.0.3/okx_exchange_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 08:03:50.000000 okx_exchange_api-1.0.3/okx_exchange_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-19 08:03:50.000000 okx_exchange_api-1.0.3/okx_exchange_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-19 08:03:50.000000 okx_exchange_api-1.0.3/okx_exchange_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 08:03:50.901131 okx_exchange_api-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1904 2023-06-19 08:03:33.000000 okx_exchange_api-1.0.3/setup.py
```

### Comparing `okx_exchange_api-1.0.2/PKG-INFO` & `okx_exchange_api-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okx_exchange_api
-Version: 1.0.2
+Version: 1.0.3
 Summary: okx交易所api封装
 Home-page: https://github.com/AbsoluteValentine/okx-exchange-api
 Author: AbsoluteValentine
 Author-email: spikeqiang@gamil.com
 License: Apache 2.0
 Keywords: okx-exchange-api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `okx_exchange_api-1.0.2/okx_exchange_api.egg-info/PKG-INFO` & `okx_exchange_api-1.0.3/okx_exchange_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okx-exchange-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: okx交易所api封装
 Home-page: https://github.com/AbsoluteValentine/okx-exchange-api
 Author: AbsoluteValentine
 Author-email: spikeqiang@gamil.com
 License: Apache 2.0
 Keywords: okx-exchange-api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `okx_exchange_api-1.0.2/setup.py` & `okx_exchange_api-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="okx_exchange_api",
-    version="1.0.2",
+    version="1.0.3",
     author="AbsoluteValentine",
     author_email="spikeqiang@gamil.com",
     description="okx交易所api封装",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AbsoluteValentine/okx-exchange-api",
     packages=setuptools.find_packages(),
```

