# Comparing `tmp/scraple-0.1.0.tar.gz` & `tmp/scraple-0.1.1.tar.gz`

## Comparing `scraple-0.1.0.tar` & `scraple-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,16 @@
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 scraple-0.1.0/src/scraple/TreeCore.py
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 scraple-0.1.0/src/scraple/Tree_search_engine.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 scraple-0.1.0/src/scraple/__init__.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 scraple-0.1.0/src/scraple/error.py
--rw-r--r--   0        0        0     7869 2020-02-02 00:00:00.000000 scraple-0.1.0/src/scraple/extract.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 scraple-0.1.0/src/scraple/pipeline.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scraple-0.1.0/LICENSE
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 scraple-0.1.0/README.md
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 scraple-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 scraple-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    16192 2020-02-02 00:00:00.000000 scraple-0.1.1/doc/documentation.md
+-rw-r--r--   0        0        0    25736 2020-02-02 00:00:00.000000 scraple-0.1.1/doc/code_example/Modified quotes to scrape.html
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 scraple-0.1.1/doc/code_example/example_code.py
+-rw-r--r--   0        0        0   125943 2020-02-02 00:00:00.000000 scraple-0.1.1/doc/code_example/Modified quotes to scrape_files/bootstrap.min.css
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 scraple-0.1.1/doc/code_example/Modified quotes to scrape_files/main.css
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 scraple-0.1.1/src/scraple/TreeCore.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 scraple-0.1.1/src/scraple/Tree_search_engine.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 scraple-0.1.1/src/scraple/__init__.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 scraple-0.1.1/src/scraple/error.py
+-rw-r--r--   0        0        0     8656 2020-02-02 00:00:00.000000 scraple-0.1.1/src/scraple/extract.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 scraple-0.1.1/src/scraple/pipeline.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 scraple-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scraple-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 scraple-0.1.1/README.md
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 scraple-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 scraple-0.1.1/PKG-INFO
```

### Comparing `scraple-0.1.0/src/scraple/TreeCore.py` & `scraple-0.1.1/src/scraple/TreeCore.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Contain the core function to customize a different interpretation of tree structure
+Contain the core function of implementation for "custom tree structure"
 used in this package.
 """
 
 
 def appender(num, list_):
     if num != 1:
         list_[-1] = num
```

### Comparing `scraple-0.1.0/src/scraple/Tree_search_engine.py` & `scraple-0.1.1/src/scraple/Tree_search_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Contain the core function to search the tree of the DOM.
-"""
+"""Contain the core function to traverse the "custom tree structure"."""
 from bs4 import BeautifulSoup as Bs
 
 from typing import Sequence
 from re import search
 
 from TreeCore import appender, identity_to_branch
 from error import SearchError
```

### Comparing `scraple-0.1.0/src/scraple/__init__.py` & `scraple-0.1.1/src/scraple/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-"""
-=============================
-scraple - Simple Scraping Library
-=============================
-
-Scraple is a Python library designed to simplify the process of web scraping.
-This library provide easy scraping and easy searching for selectors.
-
-Overview
----------
-
-Simprap provides a simple way to extract data from web pages by defining simple rules
-for extraction. It also offers a convenient mechanism for automatically finding
-selectors using only string present in the page.
-
-Main Features
----------
-
-- **SimpleExtractor**: A class that enables rule-based extraction of data from web pages,
-  making the actual scraping easy.
-
-- **Rules**: A class that allows the automatic discovery of selectors using string.
-  It simplifies the process of defining and applying extraction rules.
-
-Exception
---------------
-
-Simprap includes the following error classes:
-
-- **ParsingError**: Raised when an unexpected error occurs during page parsing.
-- **SearchError**: Raised when an unexpected error occurs while searching
-  for a string in a page.
-- **ExtractError**: Raised when an unexpected error occurs during data extraction
-  from a page.
-
-Dependencies
-------------
-- **beautifulsoup4** (version 4.x.x): A library for parsing HTML and XML documents.
-
-
-For more information visit https://github.com/max-efort/.
-
-"""
-
-from extract import SimpleExtractor, Rules
-from error import *
+"""
+=============================
+scraple - Simple Scraping Library
+=============================
+
+Scraple is a Python library designed to simplify the process of web scraping.
+This library provide easy searching for selectors and easy scraping.
+
+Overview
+---------
+
+Scraple provides a simple way to extract data from web pages by defining simple rules
+for extraction. It also offers a convenient mechanism for automatically finding
+selectors using only string present in the page.
+
+Main Features
+---------
+- **SimpleExtractor**: A class that enables rule-based extraction of data from web pages,
+  making the actual scraping easy.
+
+- **Rules**: A class that allows the automatic discovery of selectors using string.
+  It simplifies the process of defining and applying extraction rules.
+
+Exception
+--------------
+Scraple includes the following error classes:
+
+- **ParsingError**: Raised when an unexpected error occurs during page parsing.
+- **SearchError**: Raised when an unexpected error occurs while searching
+  for a string in a page.
+- **ExtractError**: Raised when an unexpected error occurs during data extraction
+  from a page.
+
+Dependencies
+------------
+- **beautifulsoup4** (version 4.x.x): A library for parsing HTML and XML documents.
+
+
+For more information visit https://github.com/max-efort/.
+
+"""
+
+from extract import SimpleExtractor, Rules
+from error import *
```

### Comparing `scraple-0.1.0/src/scraple/error.py` & `scraple-0.1.1/src/scraple/error.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 flags = "parsed", "local", "html"
 
 
 class ParsingError(Exception):
-    def __init__(self):
-        message = f"Can't parse the passed reference. Make sure you pass " \
-                  f"the right argument with the right flag {flags.__str__()}."
+    def __init__(self, flag: str):
+        message = f"Can't parse the passed object. Make sure you pass " \
+                  f"the right argument with the right flag {flags.__str__()}, " \
+                  f"the flag you passed was '{flag}'."
         super().__init__(message)
 
 
 class SearchError(Exception):
     def __init__(self, string: str, nth: int):
-        rank_msg = "the"
+        rank_msg = ""
         msg2 = " "
         msg3 = "."
         if nth > 1:
             rank_msg = f"the {nth}-th string of"
             msg2 = ", "
             msg3 = f", or {rank_msg} '{string}' does not exist."
 
@@ -22,11 +23,11 @@
                   f"either there is dummy text present{msg2}or the DOM is " \
                   f"too sophisticated to parse{msg3}"
         super().__init__(message)
 
 
 class ExtractError(Exception):
     def __init__(self):
-        msg = "There is no element with selector provided from the rule, either " \
-              "the DOM change or you provide an object with body which is not " \
-              "compatible with the rule provided."
+        msg = "There is no element that match the selector provided from the rule, " \
+              "either the DOM change by sophisticated anti-scrap method or you provide an " \
+              "incompatible web page with the rule."
         super().__init__(msg)
```

### Comparing `scraple-0.1.0/src/scraple/extract.py` & `scraple-0.1.1/src/scraple/extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,71 @@
 """
 Contain the core API class of scraping and defining rules.
 """
-from typing import Union, Optional, Callable, Generator
+from typing import Union, Optional, Callable, Generator, TypeAlias
 
 from TreeCore import create_Tree, identity_to_branch
 from Tree_search_engine import find_identity_by_string, find_parent_identity, parent_elements, Bs
 from error import *
 from pipeline import text, tags, link
 
 pipelines = {"text": text, "tags": tags, "link": link}
+selector: TypeAlias = str
 
 
 def refine_body(obj, flag):
-    flag = 'parsed' if flag not in flags else flag
+    obj = open(obj, encoding="utf8") if flag.lower() == 'local' else obj
     try:
-        if flag != 'parsed':
-            obj = open(obj, encoding="utf8") if flag == 'local' else obj
-            obj = Bs(obj, features="html.parser")
+        obj = Bs(obj, features="html.parser") if flag.lower() != 'parsed' else obj
         return obj.body if obj.body is not None else obj
     except:
-        raise ParsingError()
+        raise ParsingError(flag)
 
 
 class RulIn:
     """
-    Intermediate object as an Interface between Rules object and SimpleExtractor object
+    Intermediate object as an interface between Rules and SimpleExtractor class
     """
     def __init__(self, rule):
         self.parent = rule[0]
         self.fields = rule[1]
 
     def __str__(self):
-        return f'Fields Parent Selector:\n\t\t{self.parent.__str__()},' \
-               f'\nField Rule:\n\t\t{self.fields.__str__()}\n'
+        return f'Parent Selector:\n\t{self.parent.__str__()}\n' \
+               f'Field Rule:\n\t{self.fields.__str__()}\n'
 
 
 class Rules:
-    """Define rules of how to extract a web page using SimpleExtractor class."""
+    """
+    Define rules of what to extract of a web page. Use this defined rule if you plan to use
+    SimpleExtractor class.
+
+    You can retrieve the defined rules selector if you fancy to use it in other scraping method.
+    """
     def __init__(
             self,
             reference: Union[Bs, str, bytes],
-            reference_flag: str
+            page_flag: str
     ):
         """
         :param reference: An object used as reference, either a BeautifulSoup object,
             a string of local path of html file, or a string of html code.
-        :param reference_flag: Flag of the reference, determine how the reference
+        :param page_flag: Flag of the reference, determine how the reference
             will be preprocessed.
 
         flag:
-            - "parsed": BeautifulSoup object.
-            - "local" : String of local path.
-            - "html"  : String of html code.
+            - "parsed": use it for beautifulSoup object.
+            - "local" : use it for string of local path.
+            - "html"  : use it for byte or string of html code.
+
+        :raise ParsingError: If parsing of reference encounter unexpected error.
+        :raise FileNotFoundError: If the reference_flag is "local" and the file was not found.
         """
         self._count = 0
-        self._reference = refine_body(reference, reference_flag)
+        self._reference = refine_body(reference, page_flag)
         self._tree = create_Tree(self._reference)
 
         self._fields = {}  # entry_num : ["The field name", "branch_id", pipeline]
         self._parent = None  # the value is a idx (tuple)
 
     def add_field_rule(
             self,
@@ -74,24 +81,23 @@
 
         :param string: The string used to locate an element.
         :param field_name: Name to identify the rule name or field name.
         :param re_flag: Flag to use regex in the search.
         :param climb: Number indicating to search for the parent of n-th relative
             to the lowest element containing the string.
         :param find_string_of_nth: Number indicating to find for n-th string.
-        :param pipeline: A function object to process the intended element. The function
-            must take 1 argument which is an element (the element searched using
-            this methode). This library provide 3 methode to process an element in
-            which case you must pass a string name of the function, either "text",
-            "tags" or "link" which in order do the following: extract plain text,
-            extract text in the form of tags, extract link string of the element.
+        :param pipeline: A function object to process the intended elements. The function
+            must take 1 argument which is a list of elements. This library provide three
+            generic function (in which case you must pass a string name of the function).
+            The function in question is "text", "tags" or "link" which in order do the
+            following: extract plain text, extract text in the form of tags, extract link.
 
         :return: None
 
-        :raises SearchError: If the string used to identify an element is not found.
+        :raise SearchError: If the string used to identify an element is not found.
         """
         self._count += 1
         field_name = self._count if field_name is None else field_name
 
         self._fields[self._count] = [
             field_name,
             find_identity_by_string(
@@ -114,32 +120,38 @@
                 self._fields[self._count].append(None)
         else:
             self._fields[self._count].append(None)
 
         self._parent = find_parent_identity(self._parent, self._fields[self._count][1])
 
     def get_extract_rule(self) -> RulIn:
-        """Get the RulIn object to pass to SimpleExtractor class."""
+        """
+        Get the RulIn object contain the parent selector and a dictionary of
+        field selector.
+
+        A RulIn object can be passed to the SimpleExtractor constructor instead
+        of the "raw" Rules object.
+        """
         parent = identity_to_branch(self._parent, self._tree)
         rule = [parent, {}]
         for key in self._fields:
             full_branch = identity_to_branch(self._fields[key][1], self._tree)
 
-            full_branch = full_branch.split(parent)[1]  # if self._count > 1 else full_branch
+            full_branch = full_branch.split(parent)[1]
             rule[1][self._fields[key][0]] = full_branch, self._fields[key][2]
         return RulIn(rule)
 
-    def get_parent_selector(self) -> str:
+    def get_parent_selector(self) -> selector:
         """Get the CSS selector of the lowest parent element where,
         all the referred element when adding rule, is contained.
         """
         return identity_to_branch(self._parent, self._tree)
 
-    def get_reference_soup(self):
-        """Get the BeautifulSoup object of the reference page."""
+    def get_reference_soup(self) -> Bs:
+        """Get the beautifulsoup object of the reference page."""
         return self._reference
 
     def __str__(self):
         return self.get_extract_rule().__str__()
 
 
 class SimpleExtractor:
@@ -155,46 +167,52 @@
         """
         rule = rule.get_extract_rule() if isinstance(rule, Rules) else rule
         self.parent = rule.parent
         self.fields = rule.fields
 
     def perform_extraction(
             self,
-            body: Union[Bs, str],
-            page_flag: str = "parsed",
-            return_parent_element_instead: bool = False
-    ) -> Generator[Union[dict, Bs], None, None]:
+            body: Union[Bs, str, bytes],
+            page_flag: str,
+            iterate_parent_element_instead: bool = False
+    ) -> Generator[dict, None, None]:
         """
         Perform  extraction using the rule provided.
 
         flag:
-            - "parsed": BeautifulSoup object.
-            - "local" : String of local path.
-            - "html"  : String of html code.
+            - "parsed": use it for beautifulSoup object.
+            - "local" : use it for string of local path.
+            - "html"  : use it for byte or string of html code.
 
         :param body: An object of either a BeautifulSoup object,
             a string of local path or a string of html code.
         :param page_flag: Flag of the "body" object, determine how the object
             will be preprocessed.
-        :param return_parent_element_instead: A flag, if you want to iterate the parent
+        :param iterate_parent_element_instead: A flag, if you want to iterate the parent
             element (lowest element where all the CSS selector from the rule met).
 
-        :return: Generator object.
+        :return: Generator object which iterate dictionary:
+            {
+                "field name": [element, ...] or object returned by pipeline function
+            }.
 
         :raise ExtractError: If during execution it did not find any element that match
             selector provided from the rule object.
+        :raise ParsingError: If parsing of scraping subject encounter unexpected error.
+        :raise FileNotFoundError: If the page_flag is "local" and the file was not found.
         """
         body = refine_body(body, page_flag)
         parents = parent_elements(body, self.parent)
         if len(parents) < 1:
             raise ExtractError()
+
         for item in parents:
-            if return_parent_element_instead:
+            if iterate_parent_element_instead:
                 yield item
             else:
                 extracted = {}
                 for key in self.fields:
-                    selector = self.fields[key][0]
-                    child = item.select(selector) if selector != "" else [item]
+                    selector_ = self.fields[key][0]
+                    child = item.select(selector_) if selector_ != "" else [item]
                     extracted[key] = child if self.fields[key][1] is None \
                         else self.fields[key][1](child)
                 yield extracted
```

### Comparing `scraple-0.1.0/LICENSE` & `scraple-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scraple-0.1.0/README.md` & `scraple-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,66 @@
 # Scraple
 
 Scraple is a Python library designed to simplify the process of web scraping, 
 providing easy scraping and easy searching for selectors.
 
-## Installation
-[Pypi page](https://pypi.org/project/scraple/)
+## Version 
+v0.1.1 [changelog](https://github.com/max-efort/scraple/releases)
+
 
-You can install the package using pip:
+## Installation
+The package is hosted in [Pypi](https://pypi.org/project/scraple/) and can be 
+installed using pip:
 
 ```shell
 pip install scraple
 ```
 
 ## Main API
 The package provides two main classes: Rules and SimpleExtractor.
 
 #### 1. Rules
-The Rules class allows you to define rules for extracting elements from a web page. 
-You can add field rules using the add_field_rule method, which has the capability to 
-automatically pick selectors based on a provided string. Also, support for regex 
-matching.
+The Rules class allows you to define rules of extraction. 
+You can pick selector just by knowing what string present in that page using the `add_field_rule` method. 
+This method automatically searches for selector of element which text content match the string. 
+Additionally, the `add_field_rule` method supports regular expression matching.
 
 ```python
 from scraple import Rules
 
-some_rules = Rules("reference in the form of beautifulSoup4 object, html code or string path to local html file")
+#To instantiate Rules object you need to have the reference page.
+some_rules = Rules("reference in the form of string path to local html file", "local")
 some_rules.add_field_rule("a sentence or word exist in reference page", "field name 1")
-some_rules.add_field_rule("some othe.*?sentences", "field name 2", re_flag=True)
+some_rules.add_field_rule("some othe.*?text", "field name 2", re_flag=True)
 # Add more field rules...
 
 # It automatically search for the selector, to see it you can see the rule in console
 # or by printing it
 # print(rules)
 ```
 
 #### 2. SimpleExtractor
-The SimpleExtractor class performs the actual scraping based on the defined rules. 
-You provide the Rules object to the SimpleExtractor constructor and use the 
-perform_extraction method to create a generator object that iterate dictionary of
-element or text information.
+The SimpleExtractor class performs the actual scraping based on a defined rule.
+A Rules object act as the "which to extract" and the SimpleExtractor do the "extract" or 
+scraping. First, pass a Rules object
+to SimpleExtractor constructor and use the 
+`perform_extraction` method to create a generator object that iterate dictionary of
+elements extracted.
 
 ```python
 from scraple import SimpleExtractor
 
-extractor = SimpleExtractor(some_rules)
-result = extractor.rule(
-    "web page object in the form of beautifulSoup4 object, html code or string path to local html file")
+extractor = SimpleExtractor(some_rules)  # some_rules from above code snippet
+result = extractor.perform_extraction(
+    "web page in the form of beautifulSoup4 object",
+    "parsed"
+)
 
 # print(next(result))
-# {"field name 1": element or text information (if you provide pipeline func.),
-# print(next(result))
-#  "field name 2": ..., ...}
+# {
+#   "field name 1": [element, ...],
+#   "field name 2": ...,
+#   ...
+# }
 ```
-For more detail, see the [repository](https://github.com/max-efort/scraple) 
+For more information and tutorial, see the [documentation](https://github.com/max-efort/scraple/doc) or 
+visit the main [repository](https://github.com/max-efort/scraple)
```

### Comparing `scraple-0.1.0/pyproject.toml` & `scraple-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scraple"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Jibril", email="erikfortran@gmail.com" },
 ]
 description = "Simplify web scraping"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
@@ -23,7 +23,8 @@
 
 dependencies =[
 "beautifulsoup4 >=4.0.0",
 ]
 
 [project.urls]
 repository = "https://github.com/max-efort/scraple"
+changelog = "https://github.com/max-efort/scraple/releases"
```

### Comparing `scraple-0.1.0/PKG-INFO` & `scraple-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: scraple
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simplify web scraping
 Project-URL: repository, https://github.com/max-efort/scraple
+Project-URL: changelog, https://github.com/max-efort/scraple/releases
 Author-email: Jibril <erikfortran@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jibril
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -37,57 +38,68 @@
 Description-Content-Type: text/markdown
 
 # Scraple
 
 Scraple is a Python library designed to simplify the process of web scraping, 
 providing easy scraping and easy searching for selectors.
 
-## Installation
-[Pypi page](https://pypi.org/project/scraple/)
+## Version 
+v0.1.1 [changelog](https://github.com/max-efort/scraple/releases)
+
 
-You can install the package using pip:
+## Installation
+The package is hosted in [Pypi](https://pypi.org/project/scraple/) and can be 
+installed using pip:
 
 ```shell
 pip install scraple
 ```
 
 ## Main API
 The package provides two main classes: Rules and SimpleExtractor.
 
 #### 1. Rules
-The Rules class allows you to define rules for extracting elements from a web page. 
-You can add field rules using the add_field_rule method, which has the capability to 
-automatically pick selectors based on a provided string. Also, support for regex 
-matching.
+The Rules class allows you to define rules of extraction. 
+You can pick selector just by knowing what string present in that page using the `add_field_rule` method. 
+This method automatically searches for selector of element which text content match the string. 
+Additionally, the `add_field_rule` method supports regular expression matching.
 
 ```python
 from scraple import Rules
 
-some_rules = Rules("reference in the form of beautifulSoup4 object, html code or string path to local html file")
+#To instantiate Rules object you need to have the reference page.
+some_rules = Rules("reference in the form of string path to local html file", "local")
 some_rules.add_field_rule("a sentence or word exist in reference page", "field name 1")
-some_rules.add_field_rule("some othe.*?sentences", "field name 2", re_flag=True)
+some_rules.add_field_rule("some othe.*?text", "field name 2", re_flag=True)
 # Add more field rules...
 
 # It automatically search for the selector, to see it you can see the rule in console
 # or by printing it
 # print(rules)
 ```
 
 #### 2. SimpleExtractor
-The SimpleExtractor class performs the actual scraping based on the defined rules. 
-You provide the Rules object to the SimpleExtractor constructor and use the 
-perform_extraction method to create a generator object that iterate dictionary of
-element or text information.
+The SimpleExtractor class performs the actual scraping based on a defined rule.
+A Rules object act as the "which to extract" and the SimpleExtractor do the "extract" or 
+scraping. First, pass a Rules object
+to SimpleExtractor constructor and use the 
+`perform_extraction` method to create a generator object that iterate dictionary of
+elements extracted.
 
 ```python
 from scraple import SimpleExtractor
 
-extractor = SimpleExtractor(some_rules)
-result = extractor.rule(
-    "web page object in the form of beautifulSoup4 object, html code or string path to local html file")
+extractor = SimpleExtractor(some_rules)  # some_rules from above code snippet
+result = extractor.perform_extraction(
+    "web page in the form of beautifulSoup4 object",
+    "parsed"
+)
 
 # print(next(result))
-# {"field name 1": element or text information (if you provide pipeline func.),
-# print(next(result))
-#  "field name 2": ..., ...}
+# {
+#   "field name 1": [element, ...],
+#   "field name 2": ...,
+#   ...
+# }
 ```
-For more detail, see the [repository](https://github.com/max-efort/scraple) 
+For more information and tutorial, see the [documentation](https://github.com/max-efort/scraple/doc) or 
+visit the main [repository](https://github.com/max-efort/scraple)
```

