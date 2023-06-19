# Comparing `tmp/fastapienv-1.0.0.tar.gz` & `tmp/fastapienv-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fastapienv-1.0.0.tar", last modified: Mon Jun 19 19:59:27 2023, max compression
+gzip compressed data, was "dist\fastapienv-1.0.1.tar", last modified: Mon Jun 19 20:09:12 2023, max compression
```

## Comparing `fastapienv-1.0.0.tar` & `fastapienv-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 19:59:27.934546 fastapienv-1.0.0/
--rw-rw-rw-   0        0        0     1814 2023-06-19 19:59:27.932527 fastapienv-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1182 2023-06-19 19:55:23.000000 fastapienv-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 19:59:27.891533 fastapienv-1.0.0/fastapienv/
--rw-rw-rw-   0        0        0       86 2023-06-19 19:32:18.000000 fastapienv-1.0.0/fastapienv/__init__.py
--rw-rw-rw-   0        0        0     3225 2023-06-19 19:33:04.000000 fastapienv-1.0.0/fastapienv/main.py
-drwxrwxrwx   0        0        0        0 2023-06-19 19:59:27.925529 fastapienv-1.0.0/fastapienv.egg-info/
--rw-rw-rw-   0        0        0     1814 2023-06-19 19:59:27.000000 fastapienv-1.0.0/fastapienv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-06-19 19:59:27.000000 fastapienv-1.0.0/fastapienv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 19:59:27.000000 fastapienv-1.0.0/fastapienv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-19 19:59:27.000000 fastapienv-1.0.0/fastapienv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2023-06-19 19:59:27.000000 fastapienv-1.0.0/fastapienv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 19:59:27.000000 fastapienv-1.0.0/fastapienv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 19:59:27.935530 fastapienv-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-06-19 19:44:50.000000 fastapienv-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:09:12.534396 fastapienv-1.0.1/
+-rw-rw-rw-   0        0        0     1776 2023-06-19 20:09:12.532398 fastapienv-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1144 2023-06-19 20:08:53.000000 fastapienv-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 20:09:12.457522 fastapienv-1.0.1/fastapienv/
+-rw-rw-rw-   0        0        0       86 2023-06-19 19:32:18.000000 fastapienv-1.0.1/fastapienv/__init__.py
+-rw-rw-rw-   0        0        0     3225 2023-06-19 19:33:04.000000 fastapienv-1.0.1/fastapienv/main.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:09:12.528399 fastapienv-1.0.1/fastapienv.egg-info/
+-rw-rw-rw-   0        0        0     1776 2023-06-19 20:09:12.000000 fastapienv-1.0.1/fastapienv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-06-19 20:09:12.000000 fastapienv-1.0.1/fastapienv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 20:09:12.000000 fastapienv-1.0.1/fastapienv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-19 20:09:12.000000 fastapienv-1.0.1/fastapienv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2023-06-19 20:09:12.000000 fastapienv-1.0.1/fastapienv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 20:09:12.000000 fastapienv-1.0.1/fastapienv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 20:09:12.535442 fastapienv-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      698 2023-06-19 20:09:01.000000 fastapienv-1.0.1/setup.py
```

### Comparing `fastapienv-1.0.0/PKG-INFO` & `fastapienv-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapienv
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python module that creates a Python environment and generates FastAPI boilerplate code.
 Home-page: UNKNOWN
 Author: Gautam Sagar Mallela
 Author-email: gautamsagar.mallela99@gmail.com
 License: UNKNOWN
 Description: # Your Module
         
@@ -17,21 +17,21 @@
         You can install the module using pip:
         
         ## Usage
         
         To use the module, import it and call the `createFastApiEnvironment` function:
         
         ```python
-        from fastapienv import fastapienv
+        import fastapienv
         
         # for creating just python environment and fast api boiler plate code
-        fastapienv.createFastApiEnvironment('{{your_prefered_env_name}}')
+        createFastApiEnvironment('{{your_prefered_env_name}}')
         
         # here is the example for all the options provided in my module
-        fastapienv.createFastApiEnvironment("myenv", activate_env=True, start_server=True, server_host="localhost", server_port=8000, server_reload=True)
+        createFastApiEnvironment("myenv", activate_env=True, start_server=True, server_host="localhost", server_port=8000, server_reload=True)
         
         # activate_env will activate the environment after creating it.
         # start_server will start the fast api server using uvicorn.
         # server_host will be used to give the ip address or host name.
         # server_port will be used to change the port number at which your fast api server should run
         # server_reload will be used for dynamic reloading of your server if any changes happens to your files.
```

### Comparing `fastapienv-1.0.0/README.md` & `fastapienv-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 You can install the module using pip:
 
 ## Usage
 
 To use the module, import it and call the `createFastApiEnvironment` function:
 
 ```python
-from fastapienv import fastapienv
+import fastapienv
 
 # for creating just python environment and fast api boiler plate code
-fastapienv.createFastApiEnvironment('{{your_prefered_env_name}}')
+createFastApiEnvironment('{{your_prefered_env_name}}')
 
 # here is the example for all the options provided in my module
-fastapienv.createFastApiEnvironment("myenv", activate_env=True, start_server=True, server_host="localhost", server_port=8000, server_reload=True)
+createFastApiEnvironment("myenv", activate_env=True, start_server=True, server_host="localhost", server_port=8000, server_reload=True)
 
 # activate_env will activate the environment after creating it.
 # start_server will start the fast api server using uvicorn.
 # server_host will be used to give the ip address or host name.
 # server_port will be used to change the port number at which your fast api server should run
 # server_reload will be used for dynamic reloading of your server if any changes happens to your files.
```

### Comparing `fastapienv-1.0.0/fastapienv/main.py` & `fastapienv-1.0.1/fastapienv/main.py`

 * *Files identical despite different names*

### Comparing `fastapienv-1.0.0/fastapienv.egg-info/PKG-INFO` & `fastapienv-1.0.1/fastapienv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapienv
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python module that creates a Python environment and generates FastAPI boilerplate code.
 Home-page: UNKNOWN
 Author: Gautam Sagar Mallela
 Author-email: gautamsagar.mallela99@gmail.com
 License: UNKNOWN
 Description: # Your Module
         
@@ -17,21 +17,21 @@
         You can install the module using pip:
         
         ## Usage
         
         To use the module, import it and call the `createFastApiEnvironment` function:
         
         ```python
-        from fastapienv import fastapienv
+        import fastapienv
         
         # for creating just python environment and fast api boiler plate code
-        fastapienv.createFastApiEnvironment('{{your_prefered_env_name}}')
+        createFastApiEnvironment('{{your_prefered_env_name}}')
         
         # here is the example for all the options provided in my module
-        fastapienv.createFastApiEnvironment("myenv", activate_env=True, start_server=True, server_host="localhost", server_port=8000, server_reload=True)
+        createFastApiEnvironment("myenv", activate_env=True, start_server=True, server_host="localhost", server_port=8000, server_reload=True)
         
         # activate_env will activate the environment after creating it.
         # start_server will start the fast api server using uvicorn.
         # server_host will be used to give the ip address or host name.
         # server_port will be used to change the port number at which your fast api server should run
         # server_reload will be used for dynamic reloading of your server if any changes happens to your files.
```

### Comparing `fastapienv-1.0.0/setup.py` & `fastapienv-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fastapienv',
-    version='1.0.0',
+    version='1.0.1',
     description='A Python module that creates a Python environment and generates FastAPI boilerplate code.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Gautam Sagar Mallela',
     author_email='gautamsagar.mallela99@gmail.com',
     keywords='python module fastapi boilerplate',
     packages=find_packages(),
```

