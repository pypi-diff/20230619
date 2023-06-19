# Comparing `tmp/mtmtool-1.2.7.tar.gz` & `tmp/mtmtool-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtmtool-1.2.7.tar", last modified: Fri Jun 16 11:28:45 2023, max compression
+gzip compressed data, was "mtmtool-1.2.8.tar", last modified: Mon Jun 19 12:48:09 2023, max compression
```

## Comparing `mtmtool-1.2.7.tar` & `mtmtool-1.2.8.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 11:28:45.459439 mtmtool-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-06-16 11:28:37.000000 mtmtool-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-06-16 11:28:37.000000 mtmtool-1.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-16 11:28:45.459439 mtmtool-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-06-16 11:28:37.000000 mtmtool-1.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 11:28:45.459439 mtmtool-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2026 2023-06-16 11:28:37.000000 mtmtool-1.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 11:28:45.451439 mtmtool-1.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 11:28:45.455439 mtmtool-1.2.7/src/mtmtool/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/functool.py
--rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/io.py
--rw-r--r--   0 runner    (1001) docker     (122)      436 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/itertools.py
--rw-r--r--   0 runner    (1001) docker     (122)     2097 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     2438 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/projection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 11:28:45.455439 mtmtool-1.2.7/src/mtmtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-16 11:28:45.000000 mtmtool-1.2.7/src/mtmtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-06-16 11:28:45.000000 mtmtool-1.2.7/src/mtmtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 11:28:45.000000 mtmtool-1.2.7/src/mtmtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 11:28:45.000000 mtmtool-1.2.7/src/mtmtool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-16 11:28:45.000000 mtmtool-1.2.7/src/mtmtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-16 11:28:45.000000 mtmtool-1.2.7/src/mtmtool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 11:28:45.459439 mtmtool-1.2.7/test/
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-06-16 11:28:37.000000 mtmtool-1.2.7/test/test_args2kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 12:48:09.105533 mtmtool-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-06-19 12:48:00.000000 mtmtool-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-06-19 12:48:00.000000 mtmtool-1.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-19 12:48:09.101533 mtmtool-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-06-19 12:48:00.000000 mtmtool-1.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-19 12:48:09.105533 mtmtool-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-06-19 12:48:00.000000 mtmtool-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 12:48:09.101533 mtmtool-1.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 12:48:09.101533 mtmtool-1.2.8/src/mtmtool/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/functool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5583 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/projection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 12:48:09.101533 mtmtool-1.2.8/src/mtmtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-19 12:48:09.000000 mtmtool-1.2.8/src/mtmtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-19 12:48:09.000000 mtmtool-1.2.8/src/mtmtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 12:48:09.000000 mtmtool-1.2.8/src/mtmtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 12:48:08.000000 mtmtool-1.2.8/src/mtmtool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-19 12:48:09.000000 mtmtool-1.2.8/src/mtmtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-19 12:48:09.000000 mtmtool-1.2.8/src/mtmtool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 12:48:09.101533 mtmtool-1.2.8/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-06-19 12:48:00.000000 mtmtool-1.2.8/test/test_args2kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1584 2023-06-19 12:48:00.000000 mtmtool-1.2.8/test/test_map_pool.py
```

### Comparing `mtmtool-1.2.7/LICENSE` & `mtmtool-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.7/PKG-INFO` & `mtmtool-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmtool
-Version: 1.2.7
+Version: 1.2.8
 Summary:  A Personal Python Tool Library.
 Home-page: https://github.com/imutum/imutum_python_tool
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
```

### Comparing `mtmtool-1.2.7/setup.py` & `mtmtool-1.2.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os, shutil, sys, glob
 
 package_name = "imutum_python_tool"
 abbreviation_name = "mtmtool"
 description = " A Personal Python Tool Library."
-version = "1.2.7"
+version = "1.2.8"
 
 
 def check_requires(requires: list):
     pip_file = "pip.exe" if "win" in sys.platform else "pip"
     pip_paths = [
         os.path.join(os.path.dirname(sys.executable), "Scripts", pip_file),
         os.path.join(os.path.dirname(sys.executable), pip_file),
@@ -47,15 +47,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/imutum/{package_name}",
     packages=setuptools.find_packages("src"),  #包括在安装包内的Python包
     package_dir={"": "src"},
     zip_safe=False,
     include_package_data=True,  #启用清单文件MANIFEST.in,包含数据文件
-    install_requires=["requests", "pyyaml"],
+    install_requires=["requests", "pyyaml", "dill"],
     # ext_modules=ext_modules,
     python_requires='>=3.8',
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3.8",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `mtmtool-1.2.7/src/mtmtool/functool.py` & `mtmtool-1.2.8/src/mtmtool/functool.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.7/src/mtmtool/io.py` & `mtmtool-1.2.8/src/mtmtool/io.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.7/src/mtmtool/log.py` & `mtmtool-1.2.8/src/mtmtool/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     "INFO": logging.INFO,
     "WARNING": logging.WARNING,
     "ERROR": logging.ERROR,
     "CRITICAL": logging.CRITICAL,
 }
 
 # 默认的日志格式
-datefmt_classic = "%Y-%m-%d %H:%M:%S"
-fmt_classic = '%(asctime)s.%(msecs)03d UTC %(levelname)s %(name)s: %(message)s'
+datefmt_classic = "%Y-%m-%d %H:%M:%S %z"
+fmt_classic = '%(asctime)s %(levelname)s %(name)s: %(message)s'
 
 
 # 装饰器，自动获取函数的name参数，如果是文件路径，则自动提取文件名作为logger的name
 def auto_logger_name(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         kwargs_new = func_args2kwargs(func, *args, **kwargs)
```

### Comparing `mtmtool-1.2.7/src/mtmtool/projection.py` & `mtmtool-1.2.8/src/mtmtool/projection.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.7/src/mtmtool/time.py` & `mtmtool-1.2.8/src/mtmtool/time.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.7/src/mtmtool/webhook.py` & `mtmtool-1.2.8/src/mtmtool/webhook.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.7/src/mtmtool.egg-info/PKG-INFO` & `mtmtool-1.2.8/src/mtmtool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmtool
-Version: 1.2.7
+Version: 1.2.8
 Summary:  A Personal Python Tool Library.
 Home-page: https://github.com/imutum/imutum_python_tool
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
```

### Comparing `mtmtool-1.2.7/test/test_args2kwargs.py` & `mtmtool-1.2.8/test/test_args2kwargs.py`

 * *Files identical despite different names*

