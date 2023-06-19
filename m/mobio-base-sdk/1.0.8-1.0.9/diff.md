# Comparing `tmp/mobio-base-sdk-1.0.8.tar.gz` & `tmp/mobio-base-sdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-base-sdk-1.0.8.tar", last modified: Tue Aug  2 17:35:40 2022, max compression
+gzip compressed data, was "mobio-base-sdk-1.0.9.tar", last modified: Tue Aug  2 17:52:24 2022, max compression
```

## Comparing `mobio-base-sdk-1.0.8.tar` & `mobio-base-sdk-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:35:40.850207 mobio-base-sdk-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      264 2022-08-02 17:35:40.849207 mobio-base-sdk-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:35:40.839207 mobio-base-sdk-1.0.8/mobio/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.8/mobio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:35:40.839207 mobio-base-sdk-1.0.8/mobio/sdks/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.8/mobio/sdks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:35:40.840207 mobio-base-sdk-1.0.8/mobio/sdks/base/
--rw-r--r--   0 root         (0) root         (0)      198 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.8/mobio/sdks/base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:35:40.841207 mobio-base-sdk-1.0.8/mobio/sdks/base/apis/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.8/mobio/sdks/base/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      328 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.8/mobio/sdks/base/apis/check_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:35:40.843207 mobio-base-sdk-1.0.8/mobio/sdks/base/common/
--rw-r--r--   0 root         (0) root         (0)      206 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.8/mobio/sdks/base/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7266 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.8/mobio/sdks/base/common/mobio_logging.py
--rw-r--r--   0 root         (0) root         (0)     1276 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.8/mobio/sdks/base/common/system_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:35:40.844207 mobio-base-sdk-1.0.8/mobio/sdks/base/configs/
--rw-r--r--   0 root         (0) root         (0)      461 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.8/mobio/sdks/base/configs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:35:40.845207 mobio-base-sdk-1.0.8/mobio/sdks/base/controllers/
--rw-r--r--   0 root         (0) root         (0)     1515 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.8/mobio/sdks/base/controllers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:35:40.848207 mobio-base-sdk-1.0.8/mobio_base_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      264 2022-08-02 17:35:40.000000 mobio-base-sdk-1.0.8/mobio_base_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      568 2022-08-02 17:35:40.000000 mobio-base-sdk-1.0.8/mobio_base_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-02 17:35:40.000000 mobio-base-sdk-1.0.8/mobio_base_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2022-08-02 17:35:40.000000 mobio-base-sdk-1.0.8/mobio_base_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-08-02 17:35:40.000000 mobio-base-sdk-1.0.8/mobio_base_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-02 17:35:40.850207 mobio-base-sdk-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1014 2022-08-02 17:35:40.000000 mobio-base-sdk-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:52:24.665803 mobio-base-sdk-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      264 2022-08-02 17:52:24.664803 mobio-base-sdk-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:52:24.656803 mobio-base-sdk-1.0.9/mobio/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.9/mobio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:52:24.656803 mobio-base-sdk-1.0.9/mobio/sdks/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.9/mobio/sdks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:52:24.657802 mobio-base-sdk-1.0.9/mobio/sdks/base/
+-rw-r--r--   0 root         (0) root         (0)      198 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.9/mobio/sdks/base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:52:24.658803 mobio-base-sdk-1.0.9/mobio/sdks/base/apis/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.9/mobio/sdks/base/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      328 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.9/mobio/sdks/base/apis/check_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:52:24.659803 mobio-base-sdk-1.0.9/mobio/sdks/base/common/
+-rw-r--r--   0 root         (0) root         (0)      206 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.9/mobio/sdks/base/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7266 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.9/mobio/sdks/base/common/mobio_logging.py
+-rw-r--r--   0 root         (0) root         (0)     1276 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.9/mobio/sdks/base/common/system_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:52:24.660803 mobio-base-sdk-1.0.9/mobio/sdks/base/configs/
+-rw-r--r--   0 root         (0) root         (0)      461 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.9/mobio/sdks/base/configs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:52:24.660803 mobio-base-sdk-1.0.9/mobio/sdks/base/controllers/
+-rw-r--r--   0 root         (0) root         (0)     1515 2022-08-02 17:34:15.000000 mobio-base-sdk-1.0.9/mobio/sdks/base/controllers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 17:52:24.663803 mobio-base-sdk-1.0.9/mobio_base_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      264 2022-08-02 17:52:24.000000 mobio-base-sdk-1.0.9/mobio_base_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      568 2022-08-02 17:52:24.000000 mobio-base-sdk-1.0.9/mobio_base_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-02 17:52:24.000000 mobio-base-sdk-1.0.9/mobio_base_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2022-08-02 17:52:24.000000 mobio-base-sdk-1.0.9/mobio_base_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2022-08-02 17:52:24.000000 mobio-base-sdk-1.0.9/mobio_base_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-08-02 17:52:24.665803 mobio-base-sdk-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1014 2022-08-02 17:52:24.000000 mobio-base-sdk-1.0.9/setup.py
```

### Comparing `mobio-base-sdk-1.0.8/mobio/sdks/base/common/mobio_logging.py` & `mobio-base-sdk-1.0.9/mobio/sdks/base/common/mobio_logging.py`

 * *Files identical despite different names*

### Comparing `mobio-base-sdk-1.0.8/mobio/sdks/base/common/system_config.py` & `mobio-base-sdk-1.0.9/mobio/sdks/base/common/system_config.py`

 * *Files identical despite different names*

### Comparing `mobio-base-sdk-1.0.8/mobio/sdks/base/controllers/__init__.py` & `mobio-base-sdk-1.0.9/mobio/sdks/base/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `mobio-base-sdk-1.0.8/mobio_base_sdk.egg-info/SOURCES.txt` & `mobio-base-sdk-1.0.9/mobio_base_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mobio-base-sdk-1.0.8/setup.py` & `mobio-base-sdk-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # read the contents of your README file
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 version_dev='1.0.20'
-version_prod='1.0.8'
+version_prod='1.0.9'
 
 run_mode=''
 
 setup(name='mobio-base-sdk' + run_mode,
-      version='1.0.8',
+      version='1.0.9',
       description='Mobio project SDK',
       url='',
       author='MOBIO',
       author_email='contact@mobio.vn',
       license='MIT',
       package_dir={'': './'},
       packages=find_packages('./'),
```

