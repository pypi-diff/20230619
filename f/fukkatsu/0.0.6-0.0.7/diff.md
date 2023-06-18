# Comparing `tmp/fukkatsu-0.0.6.tar.gz` & `tmp/fukkatsu-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fukkatsu-0.0.6.tar", last modified: Sun Jun 18 20:19:23 2023, max compression
+gzip compressed data, was "fukkatsu-0.0.7.tar", last modified: Sun Jun 18 22:32:09 2023, max compression
```

## Comparing `fukkatsu-0.0.6.tar` & `fukkatsu-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 20:19:23.956079 fukkatsu-0.0.6/
--rw-rw-rw-   0        0        0     1319 2023-06-18 20:16:23.000000 fukkatsu-0.0.6/CHANGELOG.md
--rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0    12171 2023-06-18 20:19:23.949512 fukkatsu-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    11530 2023-06-13 23:47:46.000000 fukkatsu-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 20:19:23.855746 fukkatsu-0.0.6/fukkatsu/
--rw-rw-rw-   0        0        0    10417 2023-06-18 19:57:30.000000 fukkatsu-0.0.6/fukkatsu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 20:19:23.905830 fukkatsu-0.0.6/fukkatsu/memory/
--rw-rw-rw-   0        0        0       75 2023-05-20 04:07:03.000000 fukkatsu-0.0.6/fukkatsu/memory/__init__.py
--rw-rw-rw-   0        0        0      663 2023-05-20 04:07:01.000000 fukkatsu-0.0.6/fukkatsu/memory/manage.py
--rw-rw-rw-   0        0        0       23 2023-05-20 04:07:01.000000 fukkatsu-0.0.6/fukkatsu/memory/short.py
-drwxrwxrwx   0        0        0        0 2023-06-18 20:19:23.917845 fukkatsu-0.0.6/fukkatsu/observer/
--rw-rw-rw-   0        0        0       40 2023-06-15 23:48:34.000000 fukkatsu-0.0.6/fukkatsu/observer/__init__.py
--rw-rw-rw-   0        0        0     1062 2023-06-18 20:00:23.000000 fukkatsu-0.0.6/fukkatsu/observer/tracker.py
-drwxrwxrwx   0        0        0        0 2023-06-18 20:19:23.938999 fukkatsu-0.0.6/fukkatsu/utils/
--rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.6/fukkatsu/utils/__init__.py
--rw-rw-rw-   0        0        0     4082 2023-06-12 22:53:43.000000 fukkatsu-0.0.6/fukkatsu/utils/helper.py
--rw-rw-rw-   0        0        0     3242 2023-06-18 19:57:30.000000 fukkatsu-0.0.6/fukkatsu/utils/medic.py
--rw-rw-rw-   0        0        0     2779 2023-06-14 23:23:55.000000 fukkatsu-0.0.6/fukkatsu/utils/prompt.py
-drwxrwxrwx   0        0        0        0 2023-06-18 20:19:23.888836 fukkatsu-0.0.6/fukkatsu.egg-info/
--rw-rw-rw-   0        0        0    12171 2023-06-18 20:19:23.000000 fukkatsu-0.0.6/fukkatsu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-06-18 20:19:23.000000 fukkatsu-0.0.6/fukkatsu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 20:19:23.000000 fukkatsu-0.0.6/fukkatsu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-18 20:19:23.000000 fukkatsu-0.0.6/fukkatsu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-18 20:19:23.000000 fukkatsu-0.0.6/fukkatsu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 20:19:23.956079 fukkatsu-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1086 2023-06-17 23:20:33.000000 fukkatsu-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:32:09.152033 fukkatsu-0.0.7/
+-rw-rw-rw-   0        0        0     1387 2023-06-18 20:59:20.000000 fukkatsu-0.0.7/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    12171 2023-06-18 22:32:09.137523 fukkatsu-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    11530 2023-06-13 23:47:46.000000 fukkatsu-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 22:32:09.063719 fukkatsu-0.0.7/fukkatsu/
+-rw-rw-rw-   0        0        0    10373 2023-06-18 22:31:09.000000 fukkatsu-0.0.7/fukkatsu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:32:09.104277 fukkatsu-0.0.7/fukkatsu/memory/
+-rw-rw-rw-   0        0        0       75 2023-05-20 04:07:03.000000 fukkatsu-0.0.7/fukkatsu/memory/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-05-20 04:07:01.000000 fukkatsu-0.0.7/fukkatsu/memory/manage.py
+-rw-rw-rw-   0        0        0       23 2023-05-20 04:07:01.000000 fukkatsu-0.0.7/fukkatsu/memory/short.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:32:09.120327 fukkatsu-0.0.7/fukkatsu/observer/
+-rw-rw-rw-   0        0        0       40 2023-06-15 23:48:34.000000 fukkatsu-0.0.7/fukkatsu/observer/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-06-18 20:00:23.000000 fukkatsu-0.0.7/fukkatsu/observer/tracker.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:32:09.137523 fukkatsu-0.0.7/fukkatsu/utils/
+-rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.7/fukkatsu/utils/__init__.py
+-rw-rw-rw-   0        0        0     4082 2023-06-12 22:53:43.000000 fukkatsu-0.0.7/fukkatsu/utils/helper.py
+-rw-rw-rw-   0        0        0     3242 2023-06-18 22:31:09.000000 fukkatsu-0.0.7/fukkatsu/utils/medic.py
+-rw-rw-rw-   0        0        0     2779 2023-06-14 23:23:55.000000 fukkatsu-0.0.7/fukkatsu/utils/prompt.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:32:09.094939 fukkatsu-0.0.7/fukkatsu.egg-info/
+-rw-rw-rw-   0        0        0    12171 2023-06-18 22:32:08.000000 fukkatsu-0.0.7/fukkatsu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-06-18 22:32:08.000000 fukkatsu-0.0.7/fukkatsu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 22:32:08.000000 fukkatsu-0.0.7/fukkatsu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-18 22:32:08.000000 fukkatsu-0.0.7/fukkatsu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-18 22:32:08.000000 fukkatsu-0.0.7/fukkatsu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 22:32:09.152033 fukkatsu-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2023-06-18 20:55:47.000000 fukkatsu-0.0.7/setup.py
```

### Comparing `fukkatsu-0.0.6/CHANGELOG.md` & `fukkatsu-0.0.7/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -32,8 +32,12 @@
 
 ### 0.0.6
 
 - short-term-memory fix
     - short-term-memory will now only save functions that executed successfully
 - live counter fix
     - removed unintended extra live
-- logging formatting enhanced + api call logging added
+- logging formatting enhanced + api call logging added
+
+### 0.0.7
+
+- fix of "Attempt `x` to reanimate" logging message
```

### Comparing `fukkatsu-0.0.6/LICENSE` & `fukkatsu-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.6/PKG-INFO` & `fukkatsu-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fukkatsu
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python library for runtime LLM supported code corrections.
 Home-page: https://github.com/maxmekiska/fukkatsu
 Author: Maximilian Mekiska
 Author-email: maxmekiska@gmail.com
 Keywords: machinelearning,llm,runtime,codecorrection
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fukkatsu-0.0.6/README.md` & `fukkatsu-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.6/fukkatsu/__init__.py` & `fukkatsu-0.0.7/fukkatsu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 
 import copy
 import functools
 import traceback
 
 from fukkatsu.memory import SHORT_TERM_MEMORY
 from fukkatsu.observer.tracker import track
@@ -88,16 +88,15 @@
                     )
                     track.warning(
                         f"Import block added to suggested code:\n {suggested_code}\n"
                     )
 
                 for i in range(lives):
 
-                    if i != lives - 1:
-                        track.warning(f"Attempt {i+2} to reanimate\n")
+                    track.warning(f"Attempt {i+1} to reanimate\n")
 
                     try:
                         global_dict = globals()
                         local_dict = locals()
 
                         compiled_code = compile(suggested_code, "<string>", "exec")
```

### Comparing `fukkatsu-0.0.6/fukkatsu/memory/manage.py` & `fukkatsu-0.0.7/fukkatsu/memory/manage.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.6/fukkatsu/observer/tracker.py` & `fukkatsu-0.0.7/fukkatsu/observer/tracker.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.6/fukkatsu/utils/helper.py` & `fukkatsu-0.0.7/fukkatsu/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.6/fukkatsu/utils/medic.py` & `fukkatsu-0.0.7/fukkatsu/utils/medic.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.6/fukkatsu/utils/prompt.py` & `fukkatsu-0.0.7/fukkatsu/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.6/fukkatsu.egg-info/PKG-INFO` & `fukkatsu-0.0.7/fukkatsu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fukkatsu
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python library for runtime LLM supported code corrections.
 Home-page: https://github.com/maxmekiska/fukkatsu
 Author: Maximilian Mekiska
 Author-email: maxmekiska@gmail.com
 Keywords: machinelearning,llm,runtime,codecorrection
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fukkatsu-0.0.6/setup.py` & `fukkatsu-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     author="Maximilian Mekiska",
     author_email="maxmekiska@gmail.com",
     url="https://github.com/maxmekiska/fukkatsu",
     description="A python library for runtime LLM supported code corrections.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="fukkatsu",
-    version="0.0.6",
+    version="0.0.7",
     packages=find_packages(include=["fukkatsu", "fukkatsu.*"]),
     install_requires=[
         "setuptools >= 41.0.0",
         "openai >= 0.27.5, <= 0.28",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
```

