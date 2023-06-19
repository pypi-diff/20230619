# Comparing `tmp/python-automation-framework-0.1.0.tar.gz` & `tmp/python-automation-framework-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-automation-framework-0.1.0.tar", last modified: Thu Jun  1 15:09:08 2023, max compression
+gzip compressed data, was "python-automation-framework-0.1.1.tar", last modified: Mon Jun 19 07:28:33 2023, max compression
```

## Comparing `python-automation-framework-0.1.0.tar` & `python-automation-framework-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-06-01 15:09:08.655600 python-automation-framework-0.1.0/
--rw-r--r--   0 mikereiche   (502) staff       (20)     5387 2023-06-01 15:09:08.655463 python-automation-framework-0.1.0/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)     5137 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/README.md
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-06-01 15:09:08.652944 python-automation-framework-0.1.0/paf/
--rw-r--r--   0 mikereiche   (502) staff       (20)     7037 2023-06-01 14:56:14.000000 python-automation-framework-0.1.0/paf/assertion.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     3319 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/paf/common.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2138 2023-06-01 15:07:19.000000 python-automation-framework-0.1.0/paf/component.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      497 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/paf/config.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2473 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/paf/control.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.1.0/paf/dom.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.1.0/paf/javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2502 2023-06-01 15:07:19.000000 python-automation-framework-0.1.0/paf/listener.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2649 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/paf/locator.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     4345 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/paf/manager.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     3131 2023-06-01 15:07:19.000000 python-automation-framework-0.1.0/paf/page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2346 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/paf/request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      302 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/paf/types.py
--rw-r--r--   0 mikereiche   (502) staff       (20)    14599 2023-06-01 15:07:19.000000 python-automation-framework-0.1.0/paf/uielement.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     6689 2023-05-02 17:26:39.000000 python-automation-framework-0.1.0/paf/xpath.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-06-01 15:09:08.653998 python-automation-framework-0.1.0/python_automation_framework.egg-info/
--rw-r--r--   0 mikereiche   (502) staff       (20)     5387 2023-06-01 15:09:08.000000 python-automation-framework-0.1.0/python_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)      668 2023-06-01 15:09:08.000000 python-automation-framework-0.1.0/python_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-06-01 15:09:08.000000 python-automation-framework-0.1.0/python_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       46 2023-06-01 15:09:08.000000 python-automation-framework-0.1.0/python_automation_framework.egg-info/requires.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        4 2023-06-01 15:09:08.000000 python-automation-framework-0.1.0/python_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-06-01 15:09:08.655645 python-automation-framework-0.1.0/setup.cfg
--rw-r--r--   0 mikereiche   (502) staff       (20)      587 2023-06-01 15:08:41.000000 python-automation-framework-0.1.0/setup.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-06-01 15:09:08.655263 python-automation-framework-0.1.0/test/
--rw-r--r--   0 mikereiche   (502) staff       (20)     2021 2023-05-09 19:15:59.000000 python-automation-framework-0.1.0/test/test_component.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2049 2023-06-01 15:07:19.000000 python-automation-framework-0.1.0/test/test_demo_mode.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      524 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/test/test_javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     3291 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/test/test_locator.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     3274 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/test/test_manager.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1563 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/test/test_page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1124 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/test/test_request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     9791 2023-06-01 15:07:19.000000 python-automation-framework-0.1.0/test/test_uielement.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-06-19 07:28:33.377688 python-automation-framework-0.1.1/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5387 2023-06-19 07:28:33.376814 python-automation-framework-0.1.1/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5137 2023-05-09 19:33:48.000000 python-automation-framework-0.1.1/README.md
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-06-19 07:28:33.329887 python-automation-framework-0.1.1/paf/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6983 2023-06-05 10:36:16.000000 python-automation-framework-0.1.1/paf/assertion.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3319 2023-05-09 19:33:48.000000 python-automation-framework-0.1.1/paf/common.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2138 2023-06-01 15:07:19.000000 python-automation-framework-0.1.1/paf/component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      451 2023-06-05 10:36:16.000000 python-automation-framework-0.1.1/paf/config.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2384 2023-06-05 10:36:16.000000 python-automation-framework-0.1.1/paf/control.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.1.1/paf/dom.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.1.1/paf/javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2502 2023-06-01 15:07:19.000000 python-automation-framework-0.1.1/paf/listener.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2649 2023-05-09 19:33:48.000000 python-automation-framework-0.1.1/paf/locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4345 2023-05-09 19:33:48.000000 python-automation-framework-0.1.1/paf/manager.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3131 2023-06-01 15:07:19.000000 python-automation-framework-0.1.1/paf/page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2346 2023-05-09 19:33:48.000000 python-automation-framework-0.1.1/paf/request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      302 2023-05-09 19:33:48.000000 python-automation-framework-0.1.1/paf/types.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)    14485 2023-06-05 10:36:16.000000 python-automation-framework-0.1.1/paf/uielement.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6689 2023-05-02 17:26:39.000000 python-automation-framework-0.1.1/paf/xpath.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-06-19 07:28:33.341692 python-automation-framework-0.1.1/python_automation_framework.egg-info/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5387 2023-06-19 07:28:33.000000 python-automation-framework-0.1.1/python_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)      689 2023-06-19 07:28:33.000000 python-automation-framework-0.1.1/python_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-06-19 07:28:33.000000 python-automation-framework-0.1.1/python_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       46 2023-06-19 07:28:33.000000 python-automation-framework-0.1.1/python_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        4 2023-06-19 07:28:33.000000 python-automation-framework-0.1.1/python_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-06-19 07:28:33.377755 python-automation-framework-0.1.1/setup.cfg
+-rw-r--r--   0 mikereiche   (502) staff       (20)      587 2023-06-19 07:28:24.000000 python-automation-framework-0.1.1/setup.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-06-19 07:28:33.376181 python-automation-framework-0.1.1/test/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2021 2023-05-09 19:15:59.000000 python-automation-framework-0.1.1/test/test_component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      546 2023-06-05 10:36:16.000000 python-automation-framework-0.1.1/test/test_control.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2049 2023-06-01 15:07:19.000000 python-automation-framework-0.1.1/test/test_demo_mode.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      524 2023-05-09 19:33:48.000000 python-automation-framework-0.1.1/test/test_javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3291 2023-05-09 19:33:48.000000 python-automation-framework-0.1.1/test/test_locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3274 2023-05-09 19:33:48.000000 python-automation-framework-0.1.1/test/test_manager.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1563 2023-05-09 19:33:48.000000 python-automation-framework-0.1.1/test/test_page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1124 2023-05-09 19:33:48.000000 python-automation-framework-0.1.1/test/test_request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     9718 2023-06-05 10:36:16.000000 python-automation-framework-0.1.1/test/test_uielement.py
```

### Comparing `python-automation-framework-0.1.0/PKG-INFO` & `python-automation-framework-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-automation-framework
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automation framework for the WebDriver API
 Home-page: https://github.com/mreiche/python-automation-framework
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 
 ![Tests Status](https://github.com/mreiche/python-automation-framework/actions/workflows/tests.yml/badge.svg)
 [![Code Coverage Status](https://codecov.io/github/mreiche/python-automation-framework/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-automation-framework)
```

### Comparing `python-automation-framework-0.1.0/README.md` & `python-automation-framework-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/paf/assertion.py` & `python-automation-framework-0.1.1/paf/assertion.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from abc import ABC
 from typing import Generic, TypeVar
 
 import inject
 
 from paf.common import Rect, HasParent, HasName
-from paf.control import Control, RetryException
+from paf.control import RetryException, retry
 from paf.types import Supplier, Predicate, Number, ACTUAL_TYPE, Mapper
 
 
 class Format:
     @staticmethod
     def param(value: any):
         if value is None:
@@ -61,23 +61,21 @@
 
     def _test_sequence(
         self,
         test: Predicate[ACTUAL_TYPE],
         additional_subject: Supplier = None,
     ) -> bool:
         from paf.listener import Listener
-
-        control = inject.instance(Control)
         listener = inject.instance(Listener)
 
         try:
             def perform_test():
                 assert test(self.actual)
 
-            control.retry(perform_test, lambda e: listener.assertion_failed(self, self._find_closest_ui_element(), e))
+            retry(perform_test, lambda e: listener.assertion_failed(self, self._find_closest_ui_element(), e))
             listener.assertion_passed(self, self._find_closest_ui_element())
             return True
 
         except RetryException as e:
             listener.assertion_failed_finally(self, self._find_closest_ui_element(), e)
 
             if self._raise:
```

### Comparing `python-automation-framework-0.1.0/paf/common.py` & `python-automation-framework-0.1.1/paf/common.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/paf/component.py` & `python-automation-framework-0.1.1/paf/component.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/paf/javascript.py` & `python-automation-framework-0.1.1/paf/javascript.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/paf/listener.py` & `python-automation-framework-0.1.1/paf/listener.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/paf/locator.py` & `python-automation-framework-0.1.1/paf/locator.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/paf/manager.py` & `python-automation-framework-0.1.1/paf/manager.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/paf/page.py` & `python-automation-framework-0.1.1/paf/page.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/paf/request.py` & `python-automation-framework-0.1.1/paf/request.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/paf/uielement.py` & `python-automation-framework-0.1.1/paf/uielement.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.color import Color
 
 import paf.javascript as script
 from paf.assertion import StringAssertion, Format, BinaryAssertion, QuantityAssertion, RectAssertion, ASSERTION
 from paf.common import HasParent, Locator, Point, Rect, Property, Formatter, NotFoundException, NotUniqueException
-from paf.control import Control
+from paf.control import retry
 from paf.dom import Attribute
 from paf.listener import Listener
 from paf.locator import By
 from paf.types import Mapper, Consumer, R
 from paf.xpath import XPath
 
 
@@ -202,21 +202,17 @@
                 return mapper(web_element)
             else:
                 raise NotFoundException(f"Not found")
 
         return self._find_web_elements(_handle)
 
     def _action_sequence(self, consumer: Consumer[WebElement], action_name: str):
-        control = inject.instance(Control)
         listener = inject.instance(Listener)
         try:
-            control.retry(
-                action=lambda: self.find_web_element(consumer),
-                on_fail=lambda e: listener.action_failed(action_name, self, e)
-            )
+            retry(lambda: self.find_web_element(consumer), lambda e: listener.action_failed(action_name, self, e))
             listener.action_passed(action_name, self)
         except Exception as exception:
             listener.action_failed_finally(action_name, self, exception)
             raise Exception(f"{self.name_path}: {exception}")
 
     def click(self):
         self._action_sequence(lambda web_element: web_element.click(), __name__)
```

### Comparing `python-automation-framework-0.1.0/paf/xpath.py` & `python-automation-framework-0.1.1/paf/xpath.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/python_automation_framework.egg-info/PKG-INFO` & `python-automation-framework-0.1.1/python_automation_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-automation-framework
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automation framework for the WebDriver API
 Home-page: https://github.com/mreiche/python-automation-framework
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 
 ![Tests Status](https://github.com/mreiche/python-automation-framework/actions/workflows/tests.yml/badge.svg)
 [![Code Coverage Status](https://codecov.io/github/mreiche/python-automation-framework/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-automation-framework)
```

### Comparing `python-automation-framework-0.1.0/python_automation_framework.egg-info/SOURCES.txt` & `python-automation-framework-0.1.1/python_automation_framework.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 paf/xpath.py
 python_automation_framework.egg-info/PKG-INFO
 python_automation_framework.egg-info/SOURCES.txt
 python_automation_framework.egg-info/dependency_links.txt
 python_automation_framework.egg-info/requires.txt
 python_automation_framework.egg-info/top_level.txt
 test/test_component.py
+test/test_control.py
 test/test_demo_mode.py
 test/test_javascript.py
 test/test_locator.py
 test/test_manager.py
 test/test_page.py
 test/test_request.py
 test/test_uielement.py
```

### Comparing `python-automation-framework-0.1.0/setup.py` & `python-automation-framework-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="python-automation-framework",
     description="Automation framework for the WebDriver API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.1.0",
+    version="0.1.1",
     url="https://github.com/mreiche/python-automation-framework",
     author="Mike Reiche",
     packages=["paf"],
     install_requires=["inject>=4.3.1", "selenium>=4.8.3", "is-empty>=1.0.1"],
 )
```

### Comparing `python-automation-framework-0.1.0/test/test_component.py` & `python-automation-framework-0.1.1/test/test_component.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/test/test_demo_mode.py` & `python-automation-framework-0.1.1/test/test_demo_mode.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/test/test_javascript.py` & `python-automation-framework-0.1.1/test/test_javascript.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/test/test_locator.py` & `python-automation-framework-0.1.1/test/test_locator.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/test/test_manager.py` & `python-automation-framework-0.1.1/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/test/test_page.py` & `python-automation-framework-0.1.1/test/test_page.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/test/test_request.py` & `python-automation-framework-0.1.1/test/test_request.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.1.0/test/test_uielement.py` & `python-automation-framework-0.1.1/test/test_uielement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inject
 import pytest
 from selenium.webdriver.support.color import Color
 
-from paf.control import Control
+from paf.control import change, retry
 from paf.locator import By
 from paf.manager import WebDriverManager
 from paf.page import PageFactory, FinderPage
 from paf.uielement import UiElement
 from paf.xpath import XPath
 from test import create_webdriver
 
@@ -186,23 +186,18 @@
     assert path
 
 
 def test_retry(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/key-click-display-test.html")
     btn = finder.find(By.id("button").unique)
     clicks = finder.find(XPath.at("div").id("events").select("p"))
-
-    control = inject.instance(Control)
     btn.click()
-    control.retry(
-        action=lambda: clicks.expect.count.be(3),
-        on_fail=lambda e: btn.click(),
-        wait_after_fail=0,
-        count=3
-    )
+
+    with change(count=3, wait_after_fail=0):
+        retry(lambda: clicks.expect.count.be(3), lambda e: btn.click())
 
 
 def test_actions(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/events/javascript-events.html")
 
     click_btn = finder.find("#onclick")
     click_status = finder.find("#onclickstatus")
```

