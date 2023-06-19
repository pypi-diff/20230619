# Comparing `tmp/aorta_sirius-0.7.tar.gz` & `tmp/aorta_sirius-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aorta_sirius-0.7.tar", last modified: Sun Jun 11 22:25:39 2023, max compression
+gzip compressed data, was "aorta_sirius-0.8.tar", last modified: Mon Jun 19 06:13:16 2023, max compression
```

## Comparing `aorta_sirius-0.7.tar` & `aorta_sirius-0.8.tar`

### file list

```diff
@@ -1,21 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:25:39.397873 aorta_sirius-0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 22:25:39.397873 aorta_sirius-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 22:25:03.000000 aorta_sirius-0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 22:25:39.397873 aorta_sirius-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-11 22:25:03.000000 aorta_sirius-0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:25:39.393874 aorta_sirius-0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:25:39.393874 aorta_sirius-0.7/src/aorta_sirius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 22:25:39.000000 aorta_sirius-0.7/src/aorta_sirius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-11 22:25:39.000000 aorta_sirius-0.7/src/aorta_sirius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 22:25:39.000000 aorta_sirius-0.7/src/aorta_sirius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 22:25:39.000000 aorta_sirius-0.7/src/aorta_sirius.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 22:25:39.000000 aorta_sirius-0.7/src/aorta_sirius.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:25:39.397873 aorta_sirius-0.7/src/sirius/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 22:25:03.000000 aorta_sirius-0.7/src/sirius/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:25:39.397873 aorta_sirius-0.7/src/sirius/application_performance_monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-11 22:25:03.000000 aorta_sirius-0.7/src/sirius/application_performance_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-11 22:25:03.000000 aorta_sirius-0.7/src/sirius/common.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-11 22:25:03.000000 aorta_sirius-0.7/src/sirius/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 22:25:03.000000 aorta_sirius-0.7/src/sirius/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:25:39.397873 aorta_sirius-0.7/src/sirius/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-11 22:25:03.000000 aorta_sirius-0.7/src/sirius/logger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.530640 aorta_sirius-0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-19 06:13:16.530640 aorta_sirius-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-19 06:12:58.000000 aorta_sirius-0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 06:13:16.530640 aorta_sirius-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-19 06:12:58.000000 aorta_sirius-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/aorta_sirius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-19 06:13:16.000000 aorta_sirius-0.8/src/aorta_sirius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-19 06:13:16.000000 aorta_sirius-0.8/src/aorta_sirius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:13:16.000000 aorta_sirius-0.8/src/aorta_sirius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 06:13:16.000000 aorta_sirius-0.8/src/aorta_sirius.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 06:13:16.000000 aorta_sirius-0.8/src/aorta_sirius.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/sirius/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/sirius/application_performance_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/application_performance_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/application_performance_monitoring/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/sirius/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/communication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/sirius/communication/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/communication/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/communication/discord/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/sirius/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/database/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/sirius/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/http_requests/exceptions.py
```

### Comparing `aorta_sirius-0.7/setup.py` & `aorta_sirius-0.8/setup.py`

 * *Files identical despite different names*

### Comparing `aorta_sirius-0.7/src/sirius/common.py` & `aorta_sirius-0.8/src/sirius/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,30 +9,42 @@
 
 class Environment(Enum):
     Production: str = "Production"
     Staging: str = "Staging"
     Development: str = "Development"
 
 
-def get_environmental_variable(key: str) -> str:
-    value: str = os.getenv(key)
+def get_environmental_variable(environmental_variable: EnvironmentVariable) -> str:
+    value: str = os.getenv(environmental_variable.value)
     if value is None:
-        raise ApplicationException(f"Environment variable with the key is not available: {key}")
+        raise ApplicationException(f"Environment variable with the key is not available: {environmental_variable.value}")
 
     return value
 
 
 def get_environment() -> Environment:
     environment: str = os.getenv(EnvironmentVariable.ENVIRONMENT.value)
     try:
         return Environment.Development if environment is None else Environment(environment)
     except ValueError:
         raise ApplicationException(f"Invalid environment variable setup: {environment}")
 
 
+def is_production_environment() -> bool:
+    return Environment.Production == get_environment()
+
+
+def is_staging_environment() -> bool:
+    return Environment.Staging == get_environment()
+
+
+def is_development_environment() -> bool:
+    return Environment.Development == get_environment()
+
+
 def threaded(func: Callable) -> Callable:
     def wrapper(*args: Any, **kwargs: Any) -> threading.Thread:
         thread: threading.Thread = threading.Thread(target=func, args=args, kwargs=kwargs)
         thread.start()
         return thread
 
     return wrapper
```

