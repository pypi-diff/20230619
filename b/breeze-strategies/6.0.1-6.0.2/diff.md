# Comparing `tmp/breeze_strategies-6.0.1.tar.gz` & `tmp/breeze_strategies-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-6.0.1.tar", last modified: Mon Jun 19 08:00:15 2023, max compression
+gzip compressed data, was "breeze_strategies-6.0.2.tar", last modified: Mon Jun 19 08:38:13 2023, max compression
```

## Comparing `breeze_strategies-6.0.1.tar` & `breeze_strategies-6.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 08:00:15.241980 breeze_strategies-6.0.1/
--rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-6.0.1/LICENSE
--rw-rw-rw-   0        0        0     1135 2023-06-19 08:00:15.239978 breeze_strategies-6.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-06-19 07:58:59.000000 breeze_strategies-6.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 08:00:15.171666 breeze_strategies-6.0.1/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0.1/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    18069 2023-06-19 07:58:03.000000 breeze_strategies-6.0.1/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:00:15.235990 breeze_strategies-6.0.1/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1135 2023-06-19 08:00:15.000000 breeze_strategies-6.0.1/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-19 08:00:15.000000 breeze_strategies-6.0.1/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 08:00:15.000000 breeze_strategies-6.0.1/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-19 08:00:15.000000 breeze_strategies-6.0.1/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-19 08:00:15.000000 breeze_strategies-6.0.1/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 08:00:15.241980 breeze_strategies-6.0.1/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-06-19 07:59:05.000000 breeze_strategies-6.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:38:13.112002 breeze_strategies-6.0.2/
+-rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-6.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1135 2023-06-19 08:38:13.111005 breeze_strategies-6.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-06-19 08:37:30.000000 breeze_strategies-6.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 08:38:13.056948 breeze_strategies-6.0.2/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0.2/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    18070 2023-06-19 08:36:51.000000 breeze_strategies-6.0.2/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:38:13.109002 breeze_strategies-6.0.2/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1135 2023-06-19 08:38:12.000000 breeze_strategies-6.0.2/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-19 08:38:12.000000 breeze_strategies-6.0.2/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 08:38:12.000000 breeze_strategies-6.0.2/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-19 08:38:12.000000 breeze_strategies-6.0.2/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-19 08:38:12.000000 breeze_strategies-6.0.2/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 08:38:13.113004 breeze_strategies-6.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-06-19 08:37:27.000000 breeze_strategies-6.0.2/setup.py
```

### Comparing `breeze_strategies-6.0.1/LICENSE` & `breeze_strategies-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-6.0.1/PKG-INFO` & `breeze_strategies-6.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze_strategies
-Version: 6.0.1
+Version: 6.0.2
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.1
+pip install breeze_strategies==6.0.2
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.1/README.md` & `breeze_strategies-6.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.1
+pip install breeze_strategies==6.0.2
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.1/breeze_strategies/breeze_strategies.py` & `breeze_strategies-6.0.2/breeze_strategies/breeze_strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         self.stock_code = stock_code
         self.product_type = product_type 
         self.expiry_date = expiry_date  
         self.strike_price = strike_price
         self.order_type = order_type
         self.validity = validity
         self.stoploss = stoploss
-        self.quantity = quantity
+        #self.quantity = quantity
         self.validity_date = validity_date
 
         def place_order_method(stock_code,exchange_code,product,action,order_type,stoploss,quantity,price,validity,validity_date,expiry_date,right,strike_price,res_queue):
          
             data =  self.client.place_order(stock_code=stock_code,
                     exchange_code=exchange_code,
                     product="options",
```

### Comparing `breeze_strategies-6.0.1/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-6.0.2/breeze_strategies.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze-strategies
-Version: 6.0.1
+Version: 6.0.2
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.1
+pip install breeze_strategies==6.0.2
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.1/setup.py` & `breeze_strategies-6.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="6.0.1",
+    version="6.0.2",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

