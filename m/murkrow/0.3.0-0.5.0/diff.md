# Comparing `tmp/murkrow-0.3.0.tar.gz` & `tmp/murkrow-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murkrow-0.3.0.tar", max compression
+gzip compressed data, was "murkrow-0.5.0.tar", max compression
```

## Comparing `murkrow-0.3.0.tar` & `murkrow-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1504 2023-04-06 23:40:21.685931 murkrow-0.3.0/LICENSE
--rw-r--r--   0        0        0     1536 2023-04-06 23:55:12.092008 murkrow-0.3.0/README.md
--rw-r--r--   0        0        0      374 2023-04-07 19:34:52.211320 murkrow-0.3.0/murkrow/__init__.py
--rw-r--r--   0        0        0     3419 2023-04-07 18:17:08.297847 murkrow-0.3.0/murkrow/display.py
--rw-r--r--   0        0        0     1657 2023-04-07 18:40:38.406623 murkrow-0.3.0/murkrow/messaging.py
--rw-r--r--   0        0        0     2390 2023-04-07 18:58:56.825050 murkrow-0.3.0/murkrow/murkrow.py
--rw-r--r--   0        0        0     2849 2023-04-07 19:34:52.211116 murkrow-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-04-06 23:40:21.688686 murkrow-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      624 2023-04-07 00:08:40.215618 murkrow-0.3.0/tests/test_murkrow.py
--rw-r--r--   0        0        0     2518 1970-01-01 00:00:00.000000 murkrow-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-04-06 23:40:21.685931 murkrow-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1536 2023-04-06 23:55:12.092008 murkrow-0.5.0/README.md
+-rw-r--r--   0        0        0      814 2023-06-19 13:00:13.140204 murkrow-0.5.0/murkrow/__init__.py
+-rw-r--r--   0        0        0     3419 2023-04-07 18:17:08.297847 murkrow-0.5.0/murkrow/display.py
+-rw-r--r--   0        0        0     4771 2023-06-19 07:19:48.311394 murkrow-0.5.0/murkrow/messaging.py
+-rw-r--r--   0        0        0     6529 2023-06-19 07:19:48.311746 murkrow-0.5.0/murkrow/murkrow.py
+-rw-r--r--   0        0        0     1789 2023-06-19 07:19:48.311936 murkrow-0.5.0/murkrow/registry.py
+-rw-r--r--   0        0        0     2342 2023-06-19 13:00:13.140482 murkrow-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-04-06 23:40:21.688686 murkrow-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      624 2023-04-07 20:27:18.344406 murkrow-0.5.0/tests/test_murkrow.py
+-rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 murkrow-0.5.0/PKG-INFO
```

### Comparing `murkrow-0.3.0/LICENSE` & `murkrow-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `murkrow-0.3.0/README.md` & `murkrow-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `murkrow-0.3.0/murkrow/display.py` & `murkrow-0.5.0/murkrow/display.py`

 * *Files identical despite different names*

### Comparing `murkrow-0.3.0/tests/test_murkrow.py` & `murkrow-0.5.0/tests/test_murkrow.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 """Tests for `murkrow` package."""
 
-from murkrow import assistant, human, narrate, system, user, ai
+from murkrow import ai, assistant, human, narrate, system, user
 
 
 def test_messaging():
     """Test the messaging helpers for OpenAI role-based chat."""
     assert assistant('hello') == {'role': 'assistant', 'content': 'hello'}
     assert human('hello') == {'role': 'user', 'content': 'hello'}
     assert narrate('hello') == {'role': 'system', 'content': 'hello'}
```

### Comparing `murkrow-0.3.0/PKG-INFO` & `murkrow-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 Metadata-Version: 2.1
 Name: murkrow
-Version: 0.3.0
+Version: 0.5.0
 Summary: Markdown for LLMs.
 Home-page: https://github.com/rgbkrk/murkrow
 License: BSD-3-Clause
 Author: Kyle Kelley
 Author-email: rgbkrk@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.11.0,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
-Requires-Dist: ipython (>=7,<9)
+Requires-Dist: ipython (>=8.12.0,<9.0.0)
 Requires-Dist: openai (>=0.27.4,<0.28.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Murkrow
 
 ![Murkrow](https://archives.bulbagarden.net/media/upload/thumb/e/e7/0198Murkrow.png/250px-0198Murkrow.png)
 
 ```
```

