# Comparing `tmp/sliceable_dict-0.3.0.tar.gz` & `tmp/sliceable_dict-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliceable_dict-0.3.0.tar", last modified: Tue Mar 14 21:11:37 2023, max compression
+gzip compressed data, was "sliceable_dict-0.4.0.tar", last modified: Mon Jun 19 10:19:04 2023, max compression
```

## Comparing `sliceable_dict-0.3.0.tar` & `sliceable_dict-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-03-14 21:11:37.418180 sliceable_dict-0.3.0/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)    35149 2022-12-16 23:31:45.000000 sliceable_dict-0.3.0/LICENSE
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     1811 2023-03-14 21:11:37.418180 sliceable_dict-0.3.0/PKG-INFO
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     1248 2022-12-17 13:19:37.000000 sliceable_dict-0.3.0/README.md
--rw-rw-r--   0 palmb     (1000) palmb     (1000)      636 2023-03-14 21:08:48.000000 sliceable_dict-0.3.0/pyproject.toml
--rw-rw-r--   0 palmb     (1000) palmb     (1000)       38 2023-03-14 21:11:37.418180 sliceable_dict-0.3.0/setup.cfg
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-03-14 21:11:37.414180 sliceable_dict-0.3.0/sliceable_dict/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)       67 2023-02-08 13:50:27.000000 sliceable_dict-0.3.0/sliceable_dict/__init__.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     9327 2023-03-14 20:58:03.000000 sliceable_dict-0.3.0/sliceable_dict/core.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     4773 2023-03-14 20:25:45.000000 sliceable_dict-0.3.0/sliceable_dict/lib.py
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-03-14 21:11:37.414180 sliceable_dict-0.3.0/sliceable_dict.egg-info/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     1811 2023-03-14 21:11:37.000000 sliceable_dict-0.3.0/sliceable_dict.egg-info/PKG-INFO
--rw-rw-r--   0 palmb     (1000) palmb     (1000)      305 2023-03-14 21:11:37.000000 sliceable_dict-0.3.0/sliceable_dict.egg-info/SOURCES.txt
--rw-rw-r--   0 palmb     (1000) palmb     (1000)        1 2023-03-14 21:11:37.000000 sliceable_dict-0.3.0/sliceable_dict.egg-info/dependency_links.txt
--rw-rw-r--   0 palmb     (1000) palmb     (1000)       15 2023-03-14 21:11:37.000000 sliceable_dict-0.3.0/sliceable_dict.egg-info/top_level.txt
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-03-14 21:11:37.418180 sliceable_dict-0.3.0/tests/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     6211 2023-02-20 17:58:12.000000 sliceable_dict-0.3.0/tests/test_SimpleIdex.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     6122 2023-03-14 21:02:01.000000 sliceable_dict-0.3.0/tests/test_SliceDict.py
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-19 10:19:04.777467 sliceable_dict-0.4.0/
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)    35149 2022-12-16 23:31:45.000000 sliceable_dict-0.4.0/LICENSE
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     1781 2023-06-19 10:19:04.777467 sliceable_dict-0.4.0/PKG-INFO
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     1218 2023-06-19 09:54:41.000000 sliceable_dict-0.4.0/README.md
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      636 2023-06-19 10:15:39.000000 sliceable_dict-0.4.0/pyproject.toml
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)       38 2023-06-19 10:19:04.777467 sliceable_dict-0.4.0/setup.cfg
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-19 10:19:04.773467 sliceable_dict-0.4.0/sliceable_dict/
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)       67 2023-02-08 13:50:27.000000 sliceable_dict-0.4.0/sliceable_dict/__init__.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     9321 2023-06-19 10:13:49.000000 sliceable_dict-0.4.0/sliceable_dict/core.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     4773 2023-03-14 20:25:45.000000 sliceable_dict-0.4.0/sliceable_dict/lib.py
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-19 10:19:04.777467 sliceable_dict-0.4.0/sliceable_dict.egg-info/
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     1781 2023-06-19 10:19:04.000000 sliceable_dict-0.4.0/sliceable_dict.egg-info/PKG-INFO
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      326 2023-06-19 10:19:04.000000 sliceable_dict-0.4.0/sliceable_dict.egg-info/SOURCES.txt
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)        1 2023-06-19 10:19:04.000000 sliceable_dict-0.4.0/sliceable_dict.egg-info/dependency_links.txt
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)       15 2023-06-19 10:19:04.000000 sliceable_dict-0.4.0/sliceable_dict.egg-info/top_level.txt
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-19 10:19:04.777467 sliceable_dict-0.4.0/tests/
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     6211 2023-02-20 17:58:12.000000 sliceable_dict-0.4.0/tests/test_SimpleIdex.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     6090 2023-06-19 09:55:38.000000 sliceable_dict-0.4.0/tests/test_SliceDict.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      683 2023-06-19 10:14:01.000000 sliceable_dict-0.4.0/tests/test_pickle.py
```

### Comparing `sliceable_dict-0.3.0/LICENSE` & `sliceable_dict-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sliceable_dict-0.3.0/PKG-INFO` & `sliceable_dict-0.4.0/sliceable_dict.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sliceable_dict
-Version: 0.3.0
+Name: sliceable-dict
+Version: 0.4.0
 Summary: Dictionary that support slicing and multiple key selection
 Author-email: Bert Palm <bert.palm.home@gmail.com>
 Project-URL: Homepage, https://github.com/palmb/slice-dict
 Project-URL: Bug Tracker, https://github.com/palmb/slice-dict/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -32,17 +32,14 @@
 An example usage:
 ```pycon
 >>> from sliceable_dict import SliceDict
 >>> d = SliceDict(zero=0, one=1)
 >>> d
 {'zero': 0, 'one': 1,}
 
->>> isinstance(d, dict)
-True
-
 # multi-key support 
 >>> d[['two', 'three']] = 2, 3
 >>> d[['one', 'three']]
 {'one': 1, 'three': 3}
 
 # slicing
 >>> d[:]
```

### Comparing `sliceable_dict-0.3.0/README.md` & `sliceable_dict-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -18,17 +18,14 @@
 An example usage:
 ```pycon
 >>> from sliceable_dict import SliceDict
 >>> d = SliceDict(zero=0, one=1)
 >>> d
 {'zero': 0, 'one': 1,}
 
->>> isinstance(d, dict)
-True
-
 # multi-key support 
 >>> d[['two', 'three']] = 2, 3
 >>> d[['one', 'three']]
 {'one': 1, 'three': 3}
 
 # slicing
 >>> d[:]
```

### Comparing `sliceable_dict-0.3.0/pyproject.toml` & `sliceable_dict-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sliceable_dict"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="Bert Palm", email="bert.palm.home@gmail.com" },
 ]
 description = "Dictionary that support slicing and multiple key selection"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sliceable_dict-0.3.0/sliceable_dict/core.py` & `sliceable_dict-0.4.0/sliceable_dict/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from . import lib
 
 SliceDictT = TypeVar("SliceDictT", bound="SliceDict")
 DictLike = Union[SliceDictT, dict]
 
 
-class SliceDict(UserDict, dict):
+class SliceDict(UserDict):
     """
     A dict like container that support slicing, boolean selection
     and passing multiple keys at once.
     """
 
     # =====================================================
     # __get/set/del-item__
```

### Comparing `sliceable_dict-0.3.0/sliceable_dict/lib.py` & `sliceable_dict-0.4.0/sliceable_dict/lib.py`

 * *Files identical despite different names*

### Comparing `sliceable_dict-0.3.0/sliceable_dict.egg-info/PKG-INFO` & `sliceable_dict-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sliceable-dict
-Version: 0.3.0
+Name: sliceable_dict
+Version: 0.4.0
 Summary: Dictionary that support slicing and multiple key selection
 Author-email: Bert Palm <bert.palm.home@gmail.com>
 Project-URL: Homepage, https://github.com/palmb/slice-dict
 Project-URL: Bug Tracker, https://github.com/palmb/slice-dict/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -32,17 +32,14 @@
 An example usage:
 ```pycon
 >>> from sliceable_dict import SliceDict
 >>> d = SliceDict(zero=0, one=1)
 >>> d
 {'zero': 0, 'one': 1,}
 
->>> isinstance(d, dict)
-True
-
 # multi-key support 
 >>> d[['two', 'three']] = 2, 3
 >>> d[['one', 'three']]
 {'one': 1, 'three': 3}
 
 # slicing
 >>> d[:]
```

### Comparing `sliceable_dict-0.3.0/tests/test_SimpleIdex.py` & `sliceable_dict-0.4.0/tests/test_SimpleIdex.py`

 * *Files identical despite different names*

### Comparing `sliceable_dict-0.3.0/tests/test_SliceDict.py` & `sliceable_dict-0.4.0/tests/test_SliceDict.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 @pytest.mark.parametrize("kwargs", [dict(), dict(a=99), dict(x=99)])
 @pytest.mark.parametrize("args", [(), ([[1, 2]],), (dict(a="a", b="b"),)])
 def test_creation(container_or_child, args, kwargs):
     bc = container_or_child(*args, **kwargs)
     assert isinstance(bc, container_or_child)
     assert isinstance(bc, SliceDict)
-    assert isinstance(bc, dict)
 
 
 @pytest.mark.parametrize("attr", dir(dict))
 def test_attrs(container_or_child, attr):
     assert hasattr(container_or_child, attr)
```

