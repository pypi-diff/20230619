# Comparing `tmp/pythclient-0.1.5.tar.gz` & `tmp/pythclient-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythclient-0.1.5.tar", last modified: Wed Jun 14 14:59:39 2023, max compression
+gzip compressed data, was "pythclient-0.1.6.tar", last modified: Mon Jun 19 11:36:51 2023, max compression
```

## Comparing `pythclient-0.1.5.tar` & `pythclient-0.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:59:39.454985 pythclient-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (122)    11354 2023-06-14 14:59:24.000000 pythclient-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-14 14:59:39.454985 pythclient-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-06-14 14:59:24.000000 pythclient-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-14 14:59:24.000000 pythclient-0.1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:59:39.446985 pythclient-0.1.5/pythclient/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-14 14:59:24.000000 pythclient-0.1.5/pythclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4136 2023-06-14 14:59:24.000000 pythclient-0.1.5/pythclient/calendar.py
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-06-14 14:59:24.000000 pythclient-0.1.5/pythclient/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      574 2023-06-14 14:59:24.000000 pythclient-0.1.5/pythclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    24180 2023-06-14 14:59:24.000000 pythclient-0.1.5/pythclient/pythaccounts.py
--rw-r--r--   0 runner    (1001) docker     (122)    18523 2023-06-14 14:59:24.000000 pythclient-0.1.5/pythclient/pythclient.py
--rw-r--r--   0 runner    (1001) docker     (122)     6338 2023-06-14 14:59:24.000000 pythclient-0.1.5/pythclient/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (122)    15635 2023-06-14 14:59:24.000000 pythclient-0.1.5/pythclient/solana.py
--rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-06-14 14:59:24.000000 pythclient-0.1.5/pythclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:59:39.450985 pythclient-0.1.5/pythclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-14 14:59:39.000000 pythclient-0.1.5/pythclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-14 14:59:39.000000 pythclient-0.1.5/pythclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 14:59:39.000000 pythclient-0.1.5/pythclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-14 14:59:39.000000 pythclient-0.1.5/pythclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-14 14:59:39.000000 pythclient-0.1.5/pythclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 14:59:39.454985 pythclient-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-06-14 14:59:24.000000 pythclient-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:59:39.450985 pythclient-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-14 14:59:24.000000 pythclient-0.1.5/tests/test_mapping_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     8640 2023-06-14 14:59:24.000000 pythclient-0.1.5/tests/test_price_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-06-14 14:59:24.000000 pythclient-0.1.5/tests/test_price_account_header.py
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-06-14 14:59:24.000000 pythclient-0.1.5/tests/test_price_component.py
--rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-06-14 14:59:24.000000 pythclient-0.1.5/tests/test_price_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     3992 2023-06-14 14:59:24.000000 pythclient-0.1.5/tests/test_product_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-06-14 14:59:24.000000 pythclient-0.1.5/tests/test_pyth_account.py
--rw-r--r--   0 runner    (1001) docker     (122)    17146 2023-06-14 14:59:24.000000 pythclient-0.1.5/tests/test_pyth_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-06-14 14:59:24.000000 pythclient-0.1.5/tests/test_solana_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-06-14 14:59:24.000000 pythclient-0.1.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 11:36:51.621892 pythclient-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (122)    11354 2023-06-19 11:36:33.000000 pythclient-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-19 11:36:51.617892 pythclient-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-06-19 11:36:33.000000 pythclient-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-19 11:36:33.000000 pythclient-0.1.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 11:36:51.613892 pythclient-0.1.6/pythclient/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24180 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/pythaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18523 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/pythclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6338 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15635 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/solana.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 11:36:51.613892 pythclient-0.1.6/pythclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-19 11:36:51.000000 pythclient-0.1.6/pythclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-19 11:36:51.000000 pythclient-0.1.6/pythclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 11:36:51.000000 pythclient-0.1.6/pythclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-19 11:36:51.000000 pythclient-0.1.6/pythclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-19 11:36:51.000000 pythclient-0.1.6/pythclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-19 11:36:51.621892 pythclient-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-06-19 11:36:33.000000 pythclient-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 11:36:51.617892 pythclient-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_mapping_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8640 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_price_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_price_account_header.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_price_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_price_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3992 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_product_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_pyth_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17146 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_pyth_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_solana_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_utils.py
```

### Comparing `pythclient-0.1.5/LICENSE` & `pythclient-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/PKG-INFO` & `pythclient-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythclient
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library to retrieve Pyth account structures off the Solana blockchain.
 Home-page: https://github.com/pyth-network/pyth-client-py
 Author: Pyth Developers
 Author-email: contact@pyth.network
 Project-URL: Bug Tracker, https://github.com/pyth-network/pyth-client-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pythclient-0.1.5/README.md` & `pythclient-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/pythclient/exceptions.py` & `pythclient-0.1.6/pythclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/pythclient/pythaccounts.py` & `pythclient-0.1.6/pythclient/pythaccounts.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/pythclient/pythclient.py` & `pythclient-0.1.6/pythclient/pythclient.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/pythclient/ratelimit.py` & `pythclient-0.1.6/pythclient/ratelimit.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/pythclient/solana.py` & `pythclient-0.1.6/pythclient/solana.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/pythclient/utils.py` & `pythclient-0.1.6/pythclient/utils.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/pythclient.egg-info/PKG-INFO` & `pythclient-0.1.6/pythclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythclient
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library to retrieve Pyth account structures off the Solana blockchain.
 Home-page: https://github.com/pyth-network/pyth-client-py
 Author: Pyth Developers
 Author-email: contact@pyth.network
 Project-URL: Bug Tracker, https://github.com/pyth-network/pyth-client-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pythclient-0.1.5/pythclient.egg-info/SOURCES.txt` & `pythclient-0.1.6/pythclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/setup.py` & `pythclient-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiodns', 'aiohttp>=3.7.4', 'backoff', 'base58', 'dnspython', 'flake8', 'loguru', 'typing-extensions', 'pytz']
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='pythclient',
-    version='0.1.5',
+    version='0.1.6',
     packages=['pythclient'],
     author='Pyth Developers',
     author_email='contact@pyth.network',
     description='A library to retrieve Pyth account structures off the Solana blockchain.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/pyth-network/pyth-client-py',
```

### Comparing `pythclient-0.1.5/tests/test_mapping_account.py` & `pythclient-0.1.6/tests/test_mapping_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/tests/test_price_account.py` & `pythclient-0.1.6/tests/test_price_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/tests/test_price_account_header.py` & `pythclient-0.1.6/tests/test_price_account_header.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/tests/test_price_component.py` & `pythclient-0.1.6/tests/test_price_component.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/tests/test_price_info.py` & `pythclient-0.1.6/tests/test_price_info.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/tests/test_product_account.py` & `pythclient-0.1.6/tests/test_product_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/tests/test_pyth_account.py` & `pythclient-0.1.6/tests/test_pyth_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/tests/test_pyth_client.py` & `pythclient-0.1.6/tests/test_pyth_client.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/tests/test_solana_account.py` & `pythclient-0.1.6/tests/test_solana_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.5/tests/test_utils.py` & `pythclient-0.1.6/tests/test_utils.py`

 * *Files identical despite different names*

