# Comparing `tmp/pyquirc-0.2.0.tar.gz` & `tmp/pyquirc-0.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquirc-0.2.0.tar", last modified: Sat Dec  3 13:41:47 2022, max compression
+gzip compressed data, was "pyquirc-0.2.0.post1.tar", last modified: Mon Jun 19 08:11:11 2023, max compression
```

## Comparing `pyquirc-0.2.0.tar` & `pyquirc-0.2.0.post1.tar`

### file list

```diff
@@ -1,22 +1,75 @@
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2022-12-03 13:41:47.088222 pyquirc-0.2.0/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2356 2022-12-03 13:41:47.088222 pyquirc-0.2.0/PKG-INFO
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1604 2022-12-03 13:35:49.000000 pyquirc-0.2.0/README.md
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      174 2022-01-30 15:35:52.000000 pyquirc-0.2.0/pyproject.toml
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      881 2022-12-03 13:41:47.088222 pyquirc-0.2.0/setup.cfg
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      236 2022-01-31 12:51:33.000000 pyquirc-0.2.0/setup.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2022-12-03 13:41:47.088222 pyquirc-0.2.0/src/
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2022-12-03 13:41:47.088222 pyquirc-0.2.0/src/pyquirc.egg-info/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2356 2022-12-03 13:41:47.000000 pyquirc-0.2.0/src/pyquirc.egg-info/PKG-INFO
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      420 2022-12-03 13:41:47.000000 pyquirc-0.2.0/src/pyquirc.egg-info/SOURCES.txt
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        1 2022-12-03 13:41:47.000000 pyquirc-0.2.0/src/pyquirc.egg-info/dependency_links.txt
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       55 2022-12-03 13:41:47.000000 pyquirc-0.2.0/src/pyquirc.egg-info/entry_points.txt
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       36 2022-12-03 13:41:47.000000 pyquirc-0.2.0/src/pyquirc.egg-info/requires.txt
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        6 2022-12-03 13:41:47.000000 pyquirc-0.2.0/src/pyquirc.egg-info/top_level.txt
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2022-12-03 13:41:47.088222 pyquirc-0.2.0/src/quirc/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2078 2022-12-03 13:06:43.000000 pyquirc-0.2.0/src/quirc/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1144 2022-12-03 13:37:14.000000 pyquirc-0.2.0/src/quirc/__main__.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2022-12-03 13:41:47.088222 pyquirc-0.2.0/src/quirc/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2022-01-31 12:51:33.000000 pyquirc-0.2.0/src/quirc/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      922 2022-12-02 19:40:31.000000 pyquirc-0.2.0/src/quirc/tests/conftest.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1312 2022-12-03 12:56:10.000000 pyquirc-0.2.0/src/quirc/tests/test_decode.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      921 2022-12-02 19:40:31.000000 pyquirc-0.2.0/src/quirc/tests/test_low_level.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.189805 pyquirc-0.2.0.post1/
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.179805 pyquirc-0.2.0.post1/.github/
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.183138 pyquirc-0.2.0.post1/.github/workflows/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1614 2023-06-19 07:54:24.000000 pyquirc-0.2.0.post1/.github/workflows/ci.yml
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2772 2022-01-31 10:06:30.000000 pyquirc-0.2.0.post1/.gitignore
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       80 2022-01-31 11:28:19.000000 pyquirc-0.2.0.post1/.gitmodules
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3161 2022-01-31 19:44:55.000000 pyquirc-0.2.0.post1/CMakeLists.txt
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2452 2023-06-19 08:11:11.189805 pyquirc-0.2.0.post1/PKG-INFO
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1694 2023-06-19 07:54:24.000000 pyquirc-0.2.0.post1/README.md
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.183138 pyquirc-0.2.0.post1/examples/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1163 2023-06-19 07:54:24.000000 pyquirc-0.2.0.post1/examples/opencv_example.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      455 2023-06-19 07:54:24.000000 pyquirc-0.2.0.post1/examples/simple.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.183138 pyquirc-0.2.0.post1/extern/
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.183138 pyquirc-0.2.0.post1/extern/quirc/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       98 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/.gitignore
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      815 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/LICENSE
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3835 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/Makefile
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7615 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/README.md
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.186472 pyquirc-0.2.0.post1/extern/quirc/demo/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    12164 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/demo/camera.c
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2589 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/demo/camera.h
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2612 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/demo/convert.c
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1455 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/demo/convert.h
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7348 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/demo/demo.c
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5811 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/demo/demo_opencv.cxx
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1936 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/demo/demoutil.c
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1402 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/demo/demoutil.h
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5523 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/demo/dthash.c
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1793 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/demo/dthash.h
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     8151 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/demo/mjpeg.c
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1931 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/demo/mjpeg.h
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4686 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/demo/scanner.c
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.186472 pyquirc-0.2.0.post1/extern/quirc/lib/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    21512 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/lib/decode.c
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    27814 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/lib/identify.c
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4510 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/lib/quirc.c
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5402 2022-02-01 09:39:21.000000 pyquirc-0.2.0.post1/extern/quirc/lib/quirc.h
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3114 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/lib/quirc_internal.h
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11779 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/lib/version_db.c
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.186472 pyquirc-0.2.0.post1/extern/quirc/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7570 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/tests/dbgutil.c
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1655 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/tests/dbgutil.h
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5916 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/tests/inspect.c
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7124 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/tests/inspect_opencv.cxx
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7281 2022-01-31 09:21:19.000000 pyquirc-0.2.0.post1/extern/quirc/tests/qrtest.c
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.183138 pyquirc-0.2.0.post1/include/
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.186472 pyquirc-0.2.0.post1/include/quirc++/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1572 2022-02-01 09:30:59.000000 pyquirc-0.2.0.post1/include/quirc++/data.h
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1240 2022-02-01 09:39:36.000000 pyquirc-0.2.0.post1/include/quirc++/decoder.h
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      174 2023-06-19 07:58:10.000000 pyquirc-0.2.0.post1/pyproject.toml
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.186472 pyquirc-0.2.0.post1/resources/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    84100 2022-01-31 09:21:18.000000 pyquirc-0.2.0.post1/resources/helloworld.dat
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      439 2022-01-31 09:21:18.000000 pyquirc-0.2.0.post1/resources/helloworld.png
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      887 2023-06-19 08:11:11.189805 pyquirc-0.2.0.post1/setup.cfg
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      236 2022-01-31 10:05:21.000000 pyquirc-0.2.0.post1/setup.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.186472 pyquirc-0.2.0.post1/src/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      597 2022-02-01 09:35:08.000000 pyquirc-0.2.0.post1/src/decode.cpp
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2122 2022-02-01 14:09:11.000000 pyquirc-0.2.0.post1/src/decoder.cpp
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      799 2022-01-31 19:44:55.000000 pyquirc-0.2.0.post1/src/main.cpp
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4743 2023-06-19 07:54:24.000000 pyquirc-0.2.0.post1/src/pyquirc.cpp
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.189805 pyquirc-0.2.0.post1/src/pyquirc.egg-info/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2452 2023-06-19 08:11:11.000000 pyquirc-0.2.0.post1/src/pyquirc.egg-info/PKG-INFO
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1460 2023-06-19 08:11:11.000000 pyquirc-0.2.0.post1/src/pyquirc.egg-info/SOURCES.txt
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        1 2023-06-19 08:11:11.000000 pyquirc-0.2.0.post1/src/pyquirc.egg-info/dependency_links.txt
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       55 2023-06-19 08:11:11.000000 pyquirc-0.2.0.post1/src/pyquirc.egg-info/entry_points.txt
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       36 2023-06-19 08:11:11.000000 pyquirc-0.2.0.post1/src/pyquirc.egg-info/requires.txt
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        6 2023-06-19 08:11:11.000000 pyquirc-0.2.0.post1/src/pyquirc.egg-info/top_level.txt
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.189805 pyquirc-0.2.0.post1/src/quirc/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2078 2023-06-19 07:54:24.000000 pyquirc-0.2.0.post1/src/quirc/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1144 2023-06-19 07:54:24.000000 pyquirc-0.2.0.post1/src/quirc/__main__.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2023-06-19 08:11:11.189805 pyquirc-0.2.0.post1/src/quirc/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2022-01-31 11:19:12.000000 pyquirc-0.2.0.post1/src/quirc/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      922 2022-02-02 07:58:53.000000 pyquirc-0.2.0.post1/src/quirc/tests/conftest.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1312 2023-06-19 07:54:24.000000 pyquirc-0.2.0.post1/src/quirc/tests/test_decode.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      921 2022-02-02 08:12:55.000000 pyquirc-0.2.0.post1/src/quirc/tests/test_low_level.py
```

### Comparing `pyquirc-0.2.0/PKG-INFO` & `pyquirc-0.2.0.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquirc
-Version: 0.2.0
+Version: 0.2.0.post1
 Summary: Python bindings for quirc, via pybind11
 Author: Maximilian Nöthe
 Author-email: maximilian.noethe@tu-dortmund.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
-# pyquirc
+# pyquirc [![PyPI version](https://badge.fury.io/py/pyquirc.svg)](https://badge.fury.io/py/pyquirc)
 
 Python and C++ bindings for the [quirc](https://github.com/dlbeer/quirc) library, created using [pybind11](https://github.com/pybind/pybind11).
 
 ## Installation
 
 The package is on pypi, just
```

### Comparing `pyquirc-0.2.0/README.md` & `pyquirc-0.2.0.post1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pyquirc
+# pyquirc [![PyPI version](https://badge.fury.io/py/pyquirc.svg)](https://badge.fury.io/py/pyquirc)
 
 Python and C++ bindings for the [quirc](https://github.com/dlbeer/quirc) library, created using [pybind11](https://github.com/pybind/pybind11).
 
 ## Installation
 
 The package is on pypi, just
```

### Comparing `pyquirc-0.2.0/setup.cfg` & `pyquirc-0.2.0.post1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyquirc
-version = 0.2.0
+version = 0.2.0.post1
 author = Maximilian Nöthe
 author_email = maximilian.noethe@tu-dortmund.de
 description = Python bindings for quirc, via pybind11
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers =
```

### Comparing `pyquirc-0.2.0/src/pyquirc.egg-info/PKG-INFO` & `pyquirc-0.2.0.post1/src/pyquirc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquirc
-Version: 0.2.0
+Version: 0.2.0.post1
 Summary: Python bindings for quirc, via pybind11
 Author: Maximilian Nöthe
 Author-email: maximilian.noethe@tu-dortmund.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
-# pyquirc
+# pyquirc [![PyPI version](https://badge.fury.io/py/pyquirc.svg)](https://badge.fury.io/py/pyquirc)
 
 Python and C++ bindings for the [quirc](https://github.com/dlbeer/quirc) library, created using [pybind11](https://github.com/pybind/pybind11).
 
 ## Installation
 
 The package is on pypi, just
```

### Comparing `pyquirc-0.2.0/src/quirc/__init__.py` & `pyquirc-0.2.0.post1/src/quirc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyquirc-0.2.0/src/quirc/__main__.py` & `pyquirc-0.2.0.post1/src/quirc/__main__.py`

 * *Files identical despite different names*

### Comparing `pyquirc-0.2.0/src/quirc/tests/conftest.py` & `pyquirc-0.2.0.post1/src/quirc/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyquirc-0.2.0/src/quirc/tests/test_decode.py` & `pyquirc-0.2.0.post1/src/quirc/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `pyquirc-0.2.0/src/quirc/tests/test_low_level.py` & `pyquirc-0.2.0.post1/src/quirc/tests/test_low_level.py`

 * *Files identical despite different names*

