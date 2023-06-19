# Comparing `tmp/pyrepresent-0.1.1.tar.gz` & `tmp/pyrepresent-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.1.1.tar", last modified: Sun Jun 18 08:02:32 2023, max compression
+gzip compressed data, was "pyrepresent-0.1.2.tar", last modified: Mon Jun 19 17:06:22 2023, max compression
```

## Comparing `pyrepresent-0.1.1.tar` & `pyrepresent-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 08:02:32.227963 pyrepresent-0.1.1/
--rw-rw-rw-   0        0        0      115 2023-06-18 08:02:31.000000 pyrepresent-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5268 2023-06-18 08:02:32.227963 pyrepresent-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.1.1/README.md
--rw-rw-rw-   0        0        0    12965 2023-03-21 19:21:52.000000 pyrepresent-0.1.1/build.py
--rw-rw-rw-   0        0        0      715 2023-06-18 08:02:31.000000 pyrepresent-0.1.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-18 08:02:32.198450 pyrepresent-0.1.1/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     5268 2023-06-18 08:02:32.000000 pyrepresent-0.1.1/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-06-18 08:02:32.000000 pyrepresent-0.1.1/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 08:02:32.000000 pyrepresent-0.1.1/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-06-18 08:02:32.000000 pyrepresent-0.1.1/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-18 08:02:32.000000 pyrepresent-0.1.1/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-18 08:02:32.226963 pyrepresent-0.1.1/represent/
--rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.1.1/represent/__init__.py
--rw-rw-rw-   0        0        0     5875 2023-03-09 09:10:13.000000 pyrepresent-0.1.1/represent/base.py
--rw-rw-rw-   0        0        0      202 2023-03-09 09:18:08.000000 pyrepresent-0.1.1/represent/document.py
--rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.1.1/represent/indentation.py
--rw-rw-rw-   0        0        0    19307 2023-06-18 08:01:33.000000 pyrepresent-0.1.1/represent/object.py
--rw-rw-rw-   0        0        0    20797 2023-06-17 15:02:03.000000 pyrepresent-0.1.1/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.1.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 08:02:32.228963 pyrepresent-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-18 08:01:40.000000 pyrepresent-0.1.1/setup.py
--rw-rw-rw-   0        0        0      971 2023-06-13 13:18:42.000000 pyrepresent-0.1.1/test.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:06:22.511126 pyrepresent-0.1.2/
+-rw-rw-rw-   0        0        0      115 2023-06-19 17:06:22.000000 pyrepresent-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5268 2023-06-19 17:06:22.510676 pyrepresent-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.1.2/README.md
+-rw-rw-rw-   0        0        0    12965 2023-03-21 19:21:52.000000 pyrepresent-0.1.2/build.py
+-rw-rw-rw-   0        0        0      715 2023-06-19 17:06:22.000000 pyrepresent-0.1.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-19 17:06:22.503676 pyrepresent-0.1.2/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     5268 2023-06-19 17:06:22.000000 pyrepresent-0.1.2/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-06-19 17:06:22.000000 pyrepresent-0.1.2/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 17:06:22.000000 pyrepresent-0.1.2/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-19 17:06:22.000000 pyrepresent-0.1.2/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-19 17:06:22.000000 pyrepresent-0.1.2/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 17:06:22.509675 pyrepresent-0.1.2/represent/
+-rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.1.2/represent/__init__.py
+-rw-rw-rw-   0        0        0     5875 2023-03-09 09:10:13.000000 pyrepresent-0.1.2/represent/base.py
+-rw-rw-rw-   0        0        0      202 2023-03-09 09:18:08.000000 pyrepresent-0.1.2/represent/document.py
+-rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.1.2/represent/indentation.py
+-rw-rw-rw-   0        0        0    19303 2023-06-19 17:04:33.000000 pyrepresent-0.1.2/represent/object.py
+-rw-rw-rw-   0        0        0    20795 2023-06-19 17:05:54.000000 pyrepresent-0.1.2/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.1.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 17:06:22.511126 pyrepresent-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-19 17:06:11.000000 pyrepresent-0.1.2/setup.py
+-rw-rw-rw-   0        0        0      971 2023-06-13 13:18:42.000000 pyrepresent-0.1.2/test.py
```

### Comparing `pyrepresent-0.1.1/PKG-INFO` & `pyrepresent-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.1.1
+Version: 0.1.2
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.1.1/README.md` & `pyrepresent-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.1/build.py` & `pyrepresent-0.1.2/build.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.1/pyproject.toml` & `pyrepresent-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.1.1'
+version = '0.1.2'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.1.1/pyrepresent.egg-info/PKG-INFO` & `pyrepresent-0.1.2/pyrepresent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.1.1
+Version: 0.1.2
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.1.1/represent/base.py` & `pyrepresent-0.1.2/represent/base.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.1/represent/indentation.py` & `pyrepresent-0.1.2/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.1/represent/object.py` & `pyrepresent-0.1.2/represent/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,15 +460,15 @@
 
             return ids[data_id]
         # end if
 
         # noinspection PyTypeChecker
         ids[data_id] = (
             data if (
-                (data.__class__.__name__ in dir(builtins) + dir(dt)) or
+                (type(data).__name__ in dir(builtins) + dir(dt)) or
                 (data is None)
             )
             else (
                 (
                     repr(CircularReferenceStructure(data))
                     if legalize else (
                         StringWrapper(repr(CircularReferenceStructure(data)))
```

### Comparing `pyrepresent-0.1.1/represent/structures.py` & `pyrepresent-0.1.2/represent/structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,15 @@
 # end DataStructureMeta
 
 class DataStructure(metaclass=DataStructureMeta):
     """A class to represent a structure."""
 
     __type__ = None
     __value__ = None
-    __class__ = False
+    __base__ = False
 
     # noinspection PyBroadException
     try:
         color = is_proxy_process()
 
     except Exception:
         color = True
@@ -406,15 +406,15 @@
         """
 
         if self.__value__ is None:
             name = (
                 str(self.__type__).
                 replace("<class '", "").
                 replace("'>", "")
-            ) if not self.__class__ else self.__value__
+            ) if not self.__base__ else self.__value__
 
             return Colors.color_class(name, color=self.color)
 
         else:
             name = repr(self.__value__)
 
             return Colors.color_repr(
```

### Comparing `pyrepresent-0.1.1/setup.py` & `pyrepresent-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pyrepresent',
-        version='0.1.1',
+        version='0.1.2',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `pyrepresent-0.1.1/test.py` & `pyrepresent-0.1.2/test.py`

 * *Files identical despite different names*

