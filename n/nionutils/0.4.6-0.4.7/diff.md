# Comparing `tmp/nionutils-0.4.6.tar.gz` & `tmp/nionutils-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nionutils-0.4.6.tar", last modified: Fri Nov  4 20:41:46 2022, max compression
+gzip compressed data, was "nionutils-0.4.7.tar", last modified: Mon Jun 19 21:20:46 2023, max compression
```

## Comparing `nionutils-0.4.6.tar` & `nionutils-0.4.7.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:41:46.841171 nionutils-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-11-04 20:41:35.000000 nionutils-0.4.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13209 2022-11-04 20:41:46.841171 nionutils-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7153 2022-11-04 20:41:35.000000 nionutils-0.4.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:41:46.833171 nionutils-0.4.6/nion/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:41:46.837171 nionutils-0.4.6/nion/utils/
--rw-r--r--   0 runner    (1001) docker     (121)    14637 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/Binding.py
--rw-r--r--   0 runner    (1001) docker     (121)     9024 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/Color.py
--rw-r--r--   0 runner    (1001) docker     (121)     8622 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/Converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/DateTime.py
--rw-r--r--   0 runner    (1001) docker     (121)     6994 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/Event.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    41774 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/Geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)    43211 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/ListModel.py
--rw-r--r--   0 runner    (1001) docker     (121)     6577 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/Model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2100 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/Observable.py
--rw-r--r--   0 runner    (1001) docker     (121)     3940 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/Process.py
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/Promise.py
--rw-r--r--   0 runner    (1001) docker     (121)     6717 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/Recorder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/ReferenceCounting.py
--rw-r--r--   0 runner    (1001) docker     (121)     6328 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/Registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    10117 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/Selection.py
--rw-r--r--   0 runner    (1001) docker     (121)    18500 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/Stream.py
--rw-r--r--   0 runner    (1001) docker     (121)    13540 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/StructuredModel.py
--rw-r--r--   0 runner    (1001) docker     (121)     5984 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/ThreadPool.py
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/Validator.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:41:46.841171 nionutils-0.4.6/nion/utils/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/test/Binding_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3871 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/test/Color_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/test/Converter_test.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4945 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/test/Geometry_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    19040 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/test/ListModel_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/test/Model_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/test/Observable_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/test/Process_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/test/Recorder_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/test/Registry_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/test/Selection_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2654 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/test/Stream_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    14943 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/test/StructuredModel_test.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 20:41:35.000000 nionutils-0.4.6/nion/utils/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:41:46.841171 nionutils-0.4.6/nionutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13209 2022-11-04 20:41:46.000000 nionutils-0.4.6/nionutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-11-04 20:41:46.000000 nionutils-0.4.6/nionutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 20:41:46.000000 nionutils-0.4.6/nionutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-04 20:41:46.000000 nionutils-0.4.6/nionutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-04 20:41:35.000000 nionutils-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-11-04 20:41:46.841171 nionutils-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-04 20:41:35.000000 nionutils-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:20:46.643042 nionutils-0.4.7/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5881 2023-06-19 21:20:33.000000 nionutils-0.4.7/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-19 21:20:33.000000 nionutils-0.4.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-06-19 21:20:46.643042 nionutils-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-19 21:20:33.000000 nionutils-0.4.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:20:46.631042 nionutils-0.4.7/nion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:20:46.639042 nionutils-0.4.7/nion/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/Binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/Color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/DateTime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/Event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41774 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/Geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43211 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/ListModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/Model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/Observable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/Process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/Promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/Recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/ReferenceCounting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/Registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/Selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20106 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/Stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13690 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/StructuredModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/ThreadPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/Validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:20:46.639042 nionutils-0.4.7/nion/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/test/Binding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/test/Color_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/test/Converter_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4945 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/test/Geometry_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19040 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/test/ListModel_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/test/Model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/test/Observable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/test/Process_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/test/Recorder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/test/Registry_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/test/Selection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/test/Stream_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/test/StructuredModel_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:20:33.000000 nionutils-0.4.7/nion/utils/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:20:46.643042 nionutils-0.4.7/nionutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-06-19 21:20:46.000000 nionutils-0.4.7/nionutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-19 21:20:46.000000 nionutils-0.4.7/nionutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:20:46.000000 nionutils-0.4.7/nionutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 21:20:46.000000 nionutils-0.4.7/nionutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 21:20:33.000000 nionutils-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-19 21:20:46.643042 nionutils-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-19 21:20:33.000000 nionutils-0.4.7/setup.py
```

### Comparing `nionutils-0.4.6/LICENSE.txt` & `nionutils-0.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/PKG-INFO` & `nionutils-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 Metadata-Version: 2.1
 Name: nionutils
-Version: 0.4.6
+Version: 0.4.7
 Summary: Nion utility classes.
 Home-page: https://github.com/nion-software/nionutils
 Author: Nion Software
 Author-email: swift@nion.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: ~=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 License-File: LICENSE.txt
 
 Nion Utilities
 ==============
 
 The Nion Utils library (used in Nion Swift)
 -------------------------------------------
 Nion utility classes.
 
 .. start-badges
 
 .. list-table::
     :stub-columns: 1
 
-    * - tests
-      - | |linux|
     * - package
       - |version|
 
-
-.. |linux| image:: https://img.shields.io/travis/nion-software/nionutils/master.svg?label=Linux%20build
-   :target: https://travis-ci.org/nion-software/nionutils
-   :alt: Travis CI build status (Linux)
-
 .. |version| image:: https://img.shields.io/pypi/v/nionutils.svg
    :target: https://pypi.org/project/nionutils/
    :alt: Latest PyPI version
 
 .. end-badges
 
 More Information
@@ -69,15 +62,15 @@
 This project is funded by Nion Co. as part of the `Nion
 Swift <http://nion.com/swift/>`__ imaging and analysis platform. The
 code is available under the Apache License, Version 2.0.
 
 Requirements
 ------------
 
-Requires Python 3.8 or later.
+Requires Python 3.9 or later.
 
 Getting Help and Contributing
 -----------------------------
 
 If you find a bug, please file an issue on GitHub. You can also contact
 us directly at swift@nion.com.
 
@@ -241,14 +234,22 @@
 The Structured Model classes provide a way to describe a data structure
 which can produce a modifiable and observable object to be used as a
 model for other utility classes such as binding and events.
 
 Changelog (nionutils)
 =====================
 
+0.4.7 (2023-06-19)
+------------------
+- Add explicit support for Python 3.11; drop support for Python 3.8.
+- Add an auditing capability for performance auditing.
+- Add ability to add/remove streams from CombineLatestStream.
+- Add ability to display datetime in local time and with format in DateTime converter.
+- Add ValuesToIndexConverter.
+
 0.4.6 (2022-11-04)
 ------------------
 - Minor maintenance.
 
 0.4.5 (2022-09-13)
 ------------------
 - Add minor Color method to get RGB values.
```

### Comparing `nionutils-0.4.6/README.rst` & `nionutils-0.4.7/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,17 @@
 Nion utility classes.
 
 .. start-badges
 
 .. list-table::
     :stub-columns: 1
 
-    * - tests
-      - | |linux|
     * - package
       - |version|
 
-
-.. |linux| image:: https://img.shields.io/travis/nion-software/nionutils/master.svg?label=Linux%20build
-   :target: https://travis-ci.org/nion-software/nionutils
-   :alt: Travis CI build status (Linux)
-
 .. |version| image:: https://img.shields.io/pypi/v/nionutils.svg
    :target: https://pypi.org/project/nionutils/
    :alt: Latest PyPI version
 
 .. end-badges
 
 More Information
@@ -53,15 +46,15 @@
 This project is funded by Nion Co. as part of the `Nion
 Swift <http://nion.com/swift/>`__ imaging and analysis platform. The
 code is available under the Apache License, Version 2.0.
 
 Requirements
 ------------
 
-Requires Python 3.8 or later.
+Requires Python 3.9 or later.
 
 Getting Help and Contributing
 -----------------------------
 
 If you find a bug, please file an issue on GitHub. You can also contact
 us directly at swift@nion.com.
```

### Comparing `nionutils-0.4.6/nion/utils/Binding.py` & `nionutils-0.4.7/nion/utils/Binding.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/Color.py` & `nionutils-0.4.7/nion/utils/Color.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/Converter.py` & `nionutils-0.4.7/nion/utils/Converter.py`

 * *Files 22% similar despite different names*

```diff
@@ -182,19 +182,66 @@
         return str(value) if value else None
 
     def convert_back(self, value: typing.Optional[str]) -> typing.Optional[pathlib.Path]:
         return pathlib.Path(value) if value else None
 
 
 class DatetimeToStringConverter(ConverterLike[datetime.datetime, str]):
+    """Convert between UTC datetime and str.
+
+    datetime value is always utc and is naive to timezone.
+
+    is_local can be used to _display_ the datetime in local time zone.
+
+    format can be used to specify the format but must be parseable if used to convert both forward and back.
+    """
+    def __init__(self, is_local: bool = False, timezone: typing.Optional[datetime.tzinfo] = None, format: typing.Optional[str] = None) -> None:
+        self.__is_local = is_local
+        self.__timezone = timezone
+        self.__format = format
+
     def convert(self, value: typing.Optional[datetime.datetime]) -> typing.Optional[str]:
+        if value:
+            if self.__is_local:
+                value = value.replace(tzinfo=datetime.timezone.utc).astimezone().replace(tzinfo=None)
+            elif self.__timezone:
+                value = value.replace(tzinfo=datetime.timezone.utc).astimezone(self.__timezone).replace(tzinfo=None)
+        if value and self.__format:
+            return value.strftime(self.__format)
         return value.isoformat() if value is not None else None
 
     def convert_back(self, value: typing.Optional[str]) -> typing.Optional[datetime.datetime]:
         try:
-            if value and len(value) == 26:
-                return datetime.datetime.strptime(value, "%Y-%m-%dT%H:%M:%S.%f")
+            if self.__format:
+                format_ = self.__format
+            elif value and len(value) == 26:
+                format_ = "%Y-%m-%dT%H:%M:%S.%f"
             elif value and len(value) == 19:
-                return datetime.datetime.strptime(value, "%Y-%m-%dT%H:%M:%S")
+                format_ = "%Y-%m-%dT%H:%M:%S"
+            else:
+                format_ = str()
+
+            dt = datetime.datetime.strptime(value, format_) if value else None
+
+            if dt and self.__is_local:
+                return dt.astimezone(datetime.timezone.utc).replace(tzinfo=None)
+            elif dt and self.__timezone:
+                return dt.replace(tzinfo=self.__timezone).astimezone(datetime.timezone.utc).replace(tzinfo=None)
+            else:
+                return dt.replace(tzinfo=None) if dt else None
         except ValueError as e:
+            print(e)
             pass  # fall through
         return None
+
+
+class ValuesToIndexConverter(ConverterLike[FT, int], typing.Generic[FT]):
+    """Convert between set of values of type FT and int index value."""
+
+    def __init__(self, values: typing.Sequence[FT]) -> None:
+        self.__values = list(values)
+
+    def convert(self, value: typing.Optional[FT]) -> typing.Optional[int]:
+        return self.__values.index(value) if value in self.__values else None
+
+    def convert_back(self, index: typing.Optional[int]) -> typing.Optional[FT]:
+        return self.__values[index] if index is not None and 0 <= index < len(self.__values) else None
```

### Comparing `nionutils-0.4.6/nion/utils/DateTime.py` & `nionutils-0.4.7/nion/utils/DateTime.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/Event.py` & `nionutils-0.4.7/nion/utils/Event.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/Geometry.py` & `nionutils-0.4.7/nion/utils/Geometry.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/ListModel.py` & `nionutils-0.4.7/nion/utils/ListModel.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/Model.py` & `nionutils-0.4.7/nion/utils/Model.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/Observable.py` & `nionutils-0.4.7/nion/utils/Observable.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/Promise.py` & `nionutils-0.4.7/nion/utils/Promise.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 class Promise(typing.Generic[T]):
     """A promise to provide data and metadata on request.
 
     Pass a callable to produce a value. Access the value using the value or opt_value properties.
     """
     def __init__(self, fn: typing.Callable[[], T]):
-        assert fn
         self.__lock = threading.RLock()
         self.__value : typing.Optional[T] = None
         self.__fn : typing.Optional[typing.Callable[[], T]] = fn
 
     @property
     def value(self) -> typing.Optional[T]:
         """Evaluate the value if not already evaluated and return the value."""
```

### Comparing `nionutils-0.4.6/nion/utils/Recorder.py` & `nionutils-0.4.7/nion/utils/Recorder.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,32 +14,41 @@
 
 class Accessor(abc.ABC):
     @abc.abstractmethod
     def get(self, o: Observable.Observable) -> typing.Any: ...
 
 
 class DirectAccessor(Accessor):
+    def __repr__(self) -> str:
+        return f"self"
+
     def get(self, o: Observable.Observable) -> typing.Any:
         return o
 
 
 class KeyAccessor(Accessor):
     def __init__(self, accessor: Accessor, key: str) -> None:
         self.accessor = accessor
         self.key = key
 
+    def __repr__(self) -> str:
+        return f"{self.accessor}.{self.key}"
+
     def get(self, o: Observable.Observable) -> typing.Any:
         return getattr(self.accessor.get(o), self.key)
 
 
 class IndexAccessor(Accessor):
     def __init__(self, accessor: Accessor, index: int) -> None:
         self.accessor = accessor
         self.index = index
 
+    def __repr__(self) -> str:
+        return f"{self.accessor}[{self.index}]"
+
     def get(self, o: Observable.Observable) -> typing.Any:
         return self.accessor.get(o)[self.index]
 
 
 class RecorderEntry(abc.ABC):
     @abc.abstractmethod
     def apply(self, o: Observable.Observable) -> None: ...
@@ -47,35 +56,44 @@
 
 class KeyRecorderEntry(RecorderEntry):
     def __init__(self, accessor: Accessor, key: str, item: typing.Any) -> None:
         self.accessor = accessor
         self.key = key
         self.item = item
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.accessor}, {self.key}, {self.item})"
+
     def apply(self, o: Observable.Observable) -> None:
         setattr(self.accessor.get(o), self.key, self.item)
 
 
 class InsertRecorderEntry(RecorderEntry):
     def __init__(self, accessor: Accessor, key: str, index: int, item: typing.Any) -> None:
         self.accessor = accessor
         self.key = key
         self.index = index
         self.item = item
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.accessor}, {self.key}, {self.index}, {self.item})"
+
     def apply(self, o: Observable.Observable) -> None:
         self.accessor.get(o).insert_item(self.key, self.index, self.item)
 
 
 class RemoveRecorderEntry(RecorderEntry):
     def __init__(self, accessor: Accessor, key: str, index: int) -> None:
         self.accessor = accessor
         self.key = key
         self.index = index
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.accessor}, {self.key}, {self.index})"
+
     def apply(self, o: Observable.Observable) -> None:
         self.accessor.get(o).remove_item(self.key, getattr(self.accessor.get(o), self.key)[self.index])
 
 
 class RecorderLogger:
     def __init__(self) -> None:
         self.__items: typing.List[RecorderEntry] = list()
@@ -84,48 +102,80 @@
         self.__items.append(recorder_entry)
 
     def apply(self, object: Observable.Observable) -> None:
         for logger_item in self.__items:
             logger_item.apply(object)
 
 
+class RecorderDelegateProtocol(typing.Protocol):
+    def property_changed(self, accessor: Accessor, key: str, value: typing.Any) -> None: ...
+    def set_item(self, accessor: Accessor, key: str, item: typing.Any) -> None: ...
+    def insert_item(self, accessor: Accessor, key: str, index: int, item: typing.Any) -> None: ...
+    def remove_item(self, accessor: Accessor, key: str, index: int) -> None: ...
+
+
+class RecorderDelegate(RecorderDelegateProtocol):
+    def __init__(self, logger: typing.Optional[RecorderLogger] = None) -> None:
+        self.__logger: RecorderLogger = logger if logger is not None else RecorderLogger()
+
+    def property_changed(self, accessor: Accessor, key: str, value: typing.Any) -> None:
+        self.__logger.append(KeyRecorderEntry(accessor, key, value))
+
+    def set_item(self, accessor: Accessor, key: str, item: typing.Any) -> None:
+        self.__logger.append(KeyRecorderEntry(accessor, key, copy.deepcopy(item)))
+
+    def insert_item(self, accessor: Accessor, key: str, index: int, item: typing.Any) -> None:
+        self.__logger.append(InsertRecorderEntry(accessor, key, index, copy.deepcopy(item)))
+
+    def remove_item(self, accessor: Accessor, key: str, index: int) -> None:
+        self.__logger.append(RemoveRecorderEntry(accessor, key, index))
+
+
 class Recorder:
     """Record changes to an observable object.
 
     The Accessor describe how to access the object from a root object.
 
     The RecorderEntry describes how to change the object.
     """
 
     # TODO: make changes resilient... what happens if underlying object changes and recorder can't be applied?
     # TODO: thread safety
 
-    def __init__(self, object: typing.Any, accessor: typing.Optional[Accessor] = None, logger: typing.Optional[RecorderLogger] = None) -> None:
+    def __init__(self, object: typing.Any, accessor: typing.Optional[Accessor] = None, logger: typing.Optional[RecorderLogger] = None, delegate: typing.Optional[RecorderDelegateProtocol] = None) -> None:
+        self.__weak_object = weakref.ref(object)
         self.__accessor = accessor or DirectAccessor()
-        self.__logger: RecorderLogger = logger if logger is not None else RecorderLogger()
+        self.__logger: typing.Optional[RecorderLogger] = None
+        if delegate:
+            assert logger is None
+            self.__delegate = delegate
+        else:
+            self.__logger = logger if logger is not None else RecorderLogger()
+            self.__delegate = RecorderDelegate(self.__logger)
         self.__property_changed_event_listener = object.property_changed_event.listen(weak_partial(Recorder.__property_changed, self, weakref.ref(object)))
         self.__item_set_event_listener = object.item_set_event.listen(weak_partial(Recorder.__item_set, self))
         self.__item_cleared_event_listener = object.item_cleared_event.listen(weak_partial(Recorder.__item_cleared, self))
         self.__item_inserted_event_listener = object.item_inserted_event.listen(weak_partial(Recorder.__item_inserted, self))
         self.__item_removed_event_listener = object.item_removed_event.listen(weak_partial(Recorder.__item_removed, self))
         self.__item_recorders: typing.Dict[str, Recorder] = dict()
         self.__relationship_recorders = collections.defaultdict(list)
         for key in object.item_names:
             item = getattr(object, key)
             if item:
-                self.__item_recorders[key] = Recorder(item, KeyAccessor(self.__accessor, key), self.__logger)
+                self.__item_recorders[key] = Recorder(item, KeyAccessor(self.__accessor, key), delegate=self.__delegate)
         for key in object.relationship_names:
             items = getattr(object, key)
             for index, item in enumerate(items):
-                self.__relationship_recorders[key].append(Recorder(item, IndexAccessor(KeyAccessor(self.__accessor, key), index), self.__logger))
+                self.__relationship_recorders[key].append(Recorder(item, IndexAccessor(KeyAccessor(self.__accessor, key), index), delegate=self.__delegate))
 
     def close(self) -> None:
         pass
 
     def apply(self, object: Observable.Observable) -> None:
+        assert self.__logger
         self.__logger.apply(object)
 
     @property
     def _accessor(self) -> Accessor:
         return self.__accessor
 
     @_accessor.setter
@@ -133,34 +183,40 @@
         self.__accessor = value
 
     # Python 3.9+: o_ref: weakref.ReferenceType[typing.Any]
     def __property_changed(self, o_ref: typing.Any, key: str) -> None:
         object = o_ref()
         if object:
             if not hasattr(object, "_is_persistent_property_recordable") or object._is_persistent_property_recordable(key):
-                self._append_recorder_entry(KeyRecorderEntry(self.__accessor, key, getattr(object, key)))
+                self.__delegate.property_changed(self.__accessor, key, getattr(object, key))
 
     def __item_set(self, key: str, item: typing.Any) -> None:
+        object = self.__weak_object()
+        if hasattr(object, "relationship_names") and key not in getattr(object, "item_names"):
+            return
         self.__item_recorders.pop(key)
         if item:
-            self.__item_recorders[key] = Recorder(item, KeyAccessor(self.__accessor, key), self.__logger)
-        self._append_recorder_entry(KeyRecorderEntry(self.__accessor, key, copy.deepcopy(item)))
+            self.__item_recorders[key] = Recorder(item, KeyAccessor(self.__accessor, key), delegate=self.__delegate)
+        self.__delegate.set_item(self.__accessor, key, item)
 
     def __item_cleared(self, key: str) -> None:
         self.__item_set(key, None)
 
     def __item_inserted(self, key: str, value: typing.Any, before_index: int) -> None:
+        object = self.__weak_object()
+        if hasattr(object, "relationship_names") and key not in getattr(object, "relationship_names"):
+            return
         for index, relationship_recorder in enumerate(self.__relationship_recorders[key]):
             if index >= before_index:
                 relationship_recorder._accessor = IndexAccessor(KeyAccessor(self.__accessor, key), index + 1)
-        self.__relationship_recorders[key].insert(before_index, Recorder(value, IndexAccessor(KeyAccessor(self.__accessor, key), before_index), self.__logger))
-        self._append_recorder_entry(InsertRecorderEntry(self.__accessor, key, before_index, copy.deepcopy(value)))
+        self.__relationship_recorders[key].insert(before_index, Recorder(value, IndexAccessor(KeyAccessor(self.__accessor, key), before_index), delegate=self.__delegate))
+        self.__delegate.insert_item(self.__accessor, key, before_index, value)
 
     def __item_removed(self, key: str, value: typing.Any, item_index: int) -> None:
+        object = self.__weak_object()
+        if hasattr(object, "relationship_names") and key not in getattr(object, "relationship_names"):
+            return
         for index, relationship_recorder in enumerate(self.__relationship_recorders[key]):
             if index > item_index:
                 relationship_recorder._accessor = IndexAccessor(KeyAccessor(self.__accessor, key), index - 1)
         self.__relationship_recorders[key].pop(item_index)
-        self._append_recorder_entry(RemoveRecorderEntry(self.__accessor, key, item_index))
-
-    def _append_recorder_entry(self, recorder_entry: RecorderEntry) -> None:
-        self.__logger.append(recorder_entry)
+        self.__delegate.remove_item(self.__accessor, key, item_index)
```

### Comparing `nionutils-0.4.6/nion/utils/ReferenceCounting.py` & `nionutils-0.4.7/nion/utils/ReferenceCounting.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/Registry.py` & `nionutils-0.4.7/nion/utils/Registry.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/Selection.py` & `nionutils-0.4.7/nion/utils/Selection.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/Stream.py` & `nionutils-0.4.7/nion/utils/Stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 # local libraries
 import weakref
 
 from . import Event
 from . import Observable
 from .ReferenceCounting import weak_partial
 
-T = typing.TypeVar('T')
-OT = typing.TypeVar('OT')
+T = typing.TypeVar('T', covariant=True)
+OT = typing.TypeVar('OT', covariant=True)
 EqualityOperator = typing.Callable[[typing.Any, typing.Any], bool]
 
 
 class AbstractStream(typing.Generic[T]):
     """A stream provides a value property and a value_stream event that fires when the value changes."""
 
     def __init__(self) -> None:
@@ -39,15 +39,15 @@
 
     def about_to_delete(self) -> None:
         pass
 
     def add_ref(self) -> AbstractStream[T]:
         return self
 
-    def remove_ref(self, check:bool=True) -> None:
+    def remove_ref(self, check: bool = True) -> None:
         pass
 
     class RefContextManager:
         def __init__(self, item: AbstractStream[T]) -> None:
             self.__item = item
 
         def __enter__(self) -> AbstractStream[T]:
@@ -156,31 +156,44 @@
 
     def __init__(self, stream_list: typing.Sequence[AbstractStream[T]],
                  value_fn: typing.Optional[typing.Callable[..., typing.Optional[OT]]] = None) -> None:
         super().__init__()
         # outgoing messages
         self.value_stream = Event.Event()
         # references
-        self.__stream_list = list(stream_list)
+        self.__stream_list: typing.List[AbstractStream[T]] = list()
         self.__value_fn = value_fn or (lambda *x: typing.cast(OT, tuple(x)))
         # initialize values
-        self.__values: typing.List[typing.Optional[T]] = [None] * len(stream_list)
+        self.__values: typing.List[typing.Optional[T]] = list()
         self.__value: typing.Optional[OT] = None
         # listen for display changes
-        self.__listeners = dict()  # index
-        for index, stream in enumerate(self.__stream_list):
-            # define a stub and use weak_partial to avoid holding references to self.
-            def handle_stream_value(stream: CombineLatestStream[T, OT], index: int, value: typing.Any) -> None:
-                stream.__handle_stream_value(index, value)
+        self.__listeners: typing.List[Event.EventListener] = list()
+        for stream in stream_list:
+            self.__stream_list.append(stream)
+            self.__listeners.append(stream.value_stream.listen(weak_partial(CombineLatestStream.__handle_stream_value, self, stream)))
+            self.__values.append(stream.value)
+        self.__values_changed()
+
+    def append_stream(self, stream: AbstractStream[T]) -> None:
+        self.insert_stream(len(self.__stream_list), stream)
 
-            self.__listeners[index] = stream.value_stream.listen(weak_partial(handle_stream_value, self, index))
-            self.__values[index] = stream.value
+    def insert_stream(self, index: int, stream: AbstractStream[T]) -> None:
+        self.__stream_list.insert(index, stream)
+        self.__listeners.insert(index, stream.value_stream.listen(weak_partial(CombineLatestStream.__handle_stream_value, self, stream)))
+        self.__values.insert(index, stream.value)
         self.__values_changed()
 
-    def __handle_stream_value(self, index: int, value: typing.Optional[T]) -> None:
+    def remove_stream(self, index: int) -> None:
+        self.__stream_list.pop(index)
+        self.__listeners.pop(index)
+        self.__values.pop(index)
+        self.__values_changed()
+
+    def __handle_stream_value(self, stream: AbstractStream[T], value: typing.Optional[T]) -> None:
+        index = self.__stream_list.index(stream)
         self.__values[index] = value
         self.__values_changed()
 
     def __values_changed(self) -> None:
         self.__value = self.__value_fn(*self.__values)
         self.value_stream.fire(self.__value)
 
@@ -191,15 +204,15 @@
 
 class DebounceValue(typing.Generic[T]):
     def __init__(self) -> None:
         self.value: typing.Optional[T] = None
 
 
 class DebounceStream(AbstractStream[T], typing.Generic[T]):
-    """A stream that produces latest value after a specified interval has elapsed."""
+    """A stream that produces the latest value after a specified interval has elapsed."""
 
     def __init__(self, input_stream: AbstractStream[T], period: float, event_loop: typing.Optional[asyncio.AbstractEventLoop]) -> None:
         super().__init__()
         self.value_stream = Event.Event()
         self.__input_stream = input_stream
         self.__period = period
         self.__value_holder = DebounceValue[T]()
@@ -208,18 +221,18 @@
         def value_changed(stream: DebounceStream[T], value: typing.Optional[T]) -> None:
             stream.__value_changed(value)
 
         self.__listener = input_stream.value_stream.listen(weak_partial(value_changed, self))
         self.__debounce_task = StreamTask(None, event_loop)
         self.__value_changed(input_stream.value)
 
-        def finalize(task: StreamTask, s: str) -> None:
+        def finalize(task: StreamTask) -> None:
             task.clear()
 
-        weakref.finalize(self, finalize, self.__debounce_task, str(self))
+        weakref.finalize(self, finalize, self.__debounce_task)
 
     def __value_changed(self, value: typing.Optional[T]) -> None:
         self.__value_holder.value = value
         if not self.__debounce_task.is_active:  # only trigger new task if necessary
 
             async def debounce_delay(period: float, value_stream: Event.Event, value_holder: DebounceValue[T]) -> None:
                 await asyncio.sleep(period)
@@ -265,18 +278,18 @@
                 if sample_value.is_dirty:
                     sample_value.value = sample_value.pending_value
                     sample_value.is_dirty = False
                     value_stream.fire(sample_value.value)
 
         self.__sample_task = StreamTask(sample_loop(period, self.value_stream, self.__sample_value), event_loop)
 
-        def finalize(task: StreamTask, s: str) -> None:
+        def finalize(task: StreamTask) -> None:
             task.clear()
 
-        weakref.finalize(self, finalize, self.__sample_task, str(self))
+        weakref.finalize(self, finalize, self.__sample_task)
 
     def __value_changed(self, value: typing.Optional[T]) -> None:
         self.__sample_value.set_pending_value(value)
 
     @property
     def value(self) -> typing.Optional[T]:
         return self.__sample_value.value
@@ -464,33 +477,56 @@
         self.value = ValueChange(ValueChangeType.END, self.__value_stream.value)
         self.__is_active = False
 
     def __value_changed(self, value: typing.Optional[T]) -> None:
         self.value = ValueChange(ValueChangeType.CHANGE, self.__value_stream.value)
 
 
+ValueChangeStreamReactorInterfaceT = typing.TypeVar("ValueChangeStreamReactorInterfaceT", covariant=True)
+
+
+class ValueChangeStreamReactorInterface(typing.Protocol[ValueChangeStreamReactorInterfaceT]):
+    async def begin(self) -> None: ...
+    async def next_value_change(self) -> ValueChange[ValueChangeStreamReactorInterfaceT]: ...
+
+
 class ValueChangeStreamReactor(typing.Generic[T]):
-    def __init__(self, value_change_stream: ValueChangeStream[T]) -> None:
+    def __init__(self, value_change_stream: ValueChangeStream[T], event_loop: typing.Optional[asyncio.AbstractEventLoop] = None) -> None:
         self.__value_change_stream = value_change_stream
+        self.__event_loop = event_loop or asyncio.get_running_loop()
         self.__value_changed_listener = value_change_stream.value_stream.listen(weak_partial(ValueChangeStreamReactor.__value_changed, self))
         self.__event_queue: asyncio.Queue[ValueChange[T]] = asyncio.Queue()
         self.__task: typing.Optional[asyncio.Task[None]] = None
 
-        def finalize(task: typing.Optional[asyncio.Task[None]], s: str) -> None:
-            if task:
-                task.cancel()
-
-        weakref.finalize(self, finalize, self.__task, str(self))
-
     def __value_changed(self, value_change: ValueChange[T]) -> None:
         self.__event_queue.put_nowait(value_change)
 
-    def run(self, cfn: typing.Callable[[ValueChangeStreamReactor[T]], typing.Coroutine[typing.Any, typing.Any, typing.Any]]) -> None:
+    def run(self, cfn: typing.Callable[[ValueChangeStreamReactorInterface[T]], typing.Coroutine[typing.Any, typing.Any, typing.Any]]) -> None:
         assert not self.__task
-        self.__task = asyncio.get_running_loop().create_task(cfn(self))
+
+        class AValueChangeStreamReactor(ValueChangeStreamReactorInterface[T]):
+            def __init__(self, event_queue: asyncio.Queue[ValueChange[T]]) -> None:
+                self.__event_queue = event_queue
+
+            async def begin(self) -> None:
+                while True:
+                    value_change = await self.__event_queue.get()
+                    if value_change.state == ValueChangeType.BEGIN:
+                        break
+
+            async def next_value_change(self) -> ValueChange[typing.Any]:
+                return await self.__event_queue.get()
+
+        self.__task = self.__event_loop.create_task(cfn(AValueChangeStreamReactor(self.__event_queue)))
+
+        def finalize(task: typing.Optional[asyncio.Task[None]]) -> None:
+            if task:
+                task.cancel()
+
+        weakref.finalize(self, finalize, self.__task)
 
     async def begin(self) -> None:
         while True:
             value_change = await self.__event_queue.get()
             if value_change.state == ValueChangeType.BEGIN:
                 break
```

### Comparing `nionutils-0.4.6/nion/utils/StructuredModel.py` & `nionutils-0.4.7/nion/utils/StructuredModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,17 @@
 
     def __setattr__(self, name: str, value: typing.Any) -> None:
         if self.__initialized and name in self.__field_models and isinstance(self.__field_models[name], FieldPropertyModel):
             typing.cast(typing.Any, self.__field_models[name]).value = value
         else:
             super().__setattr__(name, value)
 
+    def has_field(self, name: str) -> bool:
+        return name in self.__field_models and isinstance(self.__field_models[name], FieldPropertyModel)
+
     @property
     def field_value(self) -> RecordModel:
         return self
 
     def insert_item(self, name: str, index: int, item: typing.Any) -> None:
         items = getattr(self, name)
         items.insert(index, item)
```

### Comparing `nionutils-0.4.6/nion/utils/ThreadPool.py` & `nionutils-0.4.7/nion/utils/ThreadPool.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import typing
 import weakref
 
 # third party libraries
 # None
 
 # local libraries
-# None
+from nion.utils import Process
 
 
 _ThreadPoolTask = typing.Callable[[], None]
 _OptionalThreadPoolTask = typing.Optional[_ThreadPoolTask]
 _QueueParam = typing.Any  # Python 3.9: queue.Queue[_OptionalThreadPoolTask]
 
 class ThreadPool:
@@ -43,15 +43,16 @@
         pass
 
     def start(self, thread_count: int = 16) -> None:
         def run(q: _QueueParam, cancel: threading.Event) -> None:
             while True:
                 task = q.get()
                 if task and not cancel.is_set():
-                    task()
+                    with Process.audit(f"threadpool.{task}"):
+                        task()
                 q.task_done()
                 if not task:  # do not break for cancel; need to match the final put(None)
                     break
 
         for _ in range(thread_count):
             thread = threading.Thread(target=run, args=(self.__queue, self.__cancel_event))
             thread.start()
@@ -120,15 +121,16 @@
                             if dispatcher_info.dispatch_thread_cancel.wait(0.05):  # gather changes and helps tests run faster
                                 return
                             current_time = time.time()
                             if current_time < dispatcher_info.cached_value_time + minimum_time:
                                 if dispatcher_info.dispatch_thread_cancel.wait(dispatcher_info.cached_value_time + minimum_time - current_time):
                                     return
                             dispatcher_info.is_dispatch_pending = False  # any pending calls up to this point will be realized in the recompute
-                            fn()
+                            with Process.audit(f"dispatch.{fn}"):
+                                fn()
                             dispatcher_info.cached_value_time = time.time()
                         finally:
                             with dispatcher_info.is_dispatching_lock:
                                 # the only way the thread can end is if not pending within lock.
                                 # recompute_future can only be set within lock.
                                 if not dispatcher_info.is_dispatch_pending:
                                     dispatcher_info.dispatch_future = None
```

### Comparing `nionutils-0.4.6/nion/utils/Validator.py` & `nionutils-0.4.7/nion/utils/Validator.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/test/Binding_test.py` & `nionutils-0.4.7/nion/utils/test/Binding_test.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/test/Color_test.py` & `nionutils-0.4.7/nion/utils/test/Color_test.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/test/Geometry_test.py` & `nionutils-0.4.7/nion/utils/test/Geometry_test.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/test/ListModel_test.py` & `nionutils-0.4.7/nion/utils/test/ListModel_test.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/test/Model_test.py` & `nionutils-0.4.7/nion/utils/test/Model_test.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/test/Process_test.py` & `nionutils-0.4.7/nion/utils/test/Process_test.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/test/Recorder_test.py` & `nionutils-0.4.7/nion/utils/test/Recorder_test.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/test/Registry_test.py` & `nionutils-0.4.7/nion/utils/test/Registry_test.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/test/Selection_test.py` & `nionutils-0.4.7/nion/utils/test/Selection_test.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/test/Stream_test.py` & `nionutils-0.4.7/nion/utils/test/Stream_test.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nion/utils/test/StructuredModel_test.py` & `nionutils-0.4.7/nion/utils/test/StructuredModel_test.py`

 * *Files identical despite different names*

### Comparing `nionutils-0.4.6/nionutils.egg-info/PKG-INFO` & `nionutils-0.4.7/nionutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 Metadata-Version: 2.1
 Name: nionutils
-Version: 0.4.6
+Version: 0.4.7
 Summary: Nion utility classes.
 Home-page: https://github.com/nion-software/nionutils
 Author: Nion Software
 Author-email: swift@nion.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: ~=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 License-File: LICENSE.txt
 
 Nion Utilities
 ==============
 
 The Nion Utils library (used in Nion Swift)
 -------------------------------------------
 Nion utility classes.
 
 .. start-badges
 
 .. list-table::
     :stub-columns: 1
 
-    * - tests
-      - | |linux|
     * - package
       - |version|
 
-
-.. |linux| image:: https://img.shields.io/travis/nion-software/nionutils/master.svg?label=Linux%20build
-   :target: https://travis-ci.org/nion-software/nionutils
-   :alt: Travis CI build status (Linux)
-
 .. |version| image:: https://img.shields.io/pypi/v/nionutils.svg
    :target: https://pypi.org/project/nionutils/
    :alt: Latest PyPI version
 
 .. end-badges
 
 More Information
@@ -69,15 +62,15 @@
 This project is funded by Nion Co. as part of the `Nion
 Swift <http://nion.com/swift/>`__ imaging and analysis platform. The
 code is available under the Apache License, Version 2.0.
 
 Requirements
 ------------
 
-Requires Python 3.8 or later.
+Requires Python 3.9 or later.
 
 Getting Help and Contributing
 -----------------------------
 
 If you find a bug, please file an issue on GitHub. You can also contact
 us directly at swift@nion.com.
 
@@ -241,14 +234,22 @@
 The Structured Model classes provide a way to describe a data structure
 which can produce a modifiable and observable object to be used as a
 model for other utility classes such as binding and events.
 
 Changelog (nionutils)
 =====================
 
+0.4.7 (2023-06-19)
+------------------
+- Add explicit support for Python 3.11; drop support for Python 3.8.
+- Add an auditing capability for performance auditing.
+- Add ability to add/remove streams from CombineLatestStream.
+- Add ability to display datetime in local time and with format in DateTime converter.
+- Add ValuesToIndexConverter.
+
 0.4.6 (2022-11-04)
 ------------------
 - Minor maintenance.
 
 0.4.5 (2022-09-13)
 ------------------
 - Add minor Color method to get RGB values.
```

### Comparing `nionutils-0.4.6/nionutils.egg-info/SOURCES.txt` & `nionutils-0.4.7/nionutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CHANGES.rst
 LICENSE.txt
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 nion/utils/Binding.py
 nion/utils/Color.py
```

### Comparing `nionutils-0.4.6/setup.cfg` & `nionutils-0.4.7/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [metadata]
 name = nionutils
-version = 0.4.6
+version = 0.4.7
 author = Nion Software
 author_email = swift@nion.com
 description = Nion utility classes.
 long_description = file: README.rst, CHANGES.rst, LICENSE.rst
 url = https://github.com/nion-software/nionutils
 license = Apache-2.0
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: Apache Software License
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 packages = find_namespace:
-python_requires = ~=3.8
+python_requires = >=3.9
 
 [options.packages.find]
 include = nion, nion.utils, nion.utils.test
 
 [options.package_data]
 nion.utils = py.typed
```

