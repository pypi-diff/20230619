# Comparing `tmp/codedjson-1.1.0.tar.gz` & `tmp/codedjson-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedjson-1.1.0.tar", last modified: Thu Jun 15 11:15:14 2023, max compression
+gzip compressed data, was "codedjson-1.1.1.tar", last modified: Mon Jun 19 16:54:15 2023, max compression
```

## Comparing `codedjson-1.1.0.tar` & `codedjson-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 11:15:14.134882 codedjson-1.1.0/
--rw-rw-rw-   0        0        0     1093 2023-06-10 13:01:00.000000 codedjson-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     3112 2023-06-15 11:15:14.134882 codedjson-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2363 2023-06-15 09:17:08.000000 codedjson-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 11:15:14.094494 codedjson-1.1.0/cjson/
-drwxrwxrwx   0        0        0        0 2023-06-15 11:15:14.116555 codedjson-1.1.0/cjson/src/
--rw-rw-rw-   0        0        0     4032 2023-06-15 05:28:04.000000 codedjson-1.1.0/cjson/src/cjson.py
-drwxrwxrwx   0        0        0        0 2023-06-15 11:15:14.108537 codedjson-1.1.0/cjson/src/codedjson.egg-info/
--rw-rw-rw-   0        0        0     3112 2023-06-15 11:15:14.000000 codedjson-1.1.0/cjson/src/codedjson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-06-15 11:15:14.000000 codedjson-1.1.0/cjson/src/codedjson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 11:15:14.000000 codedjson-1.1.0/cjson/src/codedjson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-15 11:15:14.000000 codedjson-1.1.0/cjson/src/codedjson.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 11:15:14.125987 codedjson-1.1.0/cjson/src/utils/
--rw-rw-rw-   0        0        0        0 2023-06-10 13:01:00.000000 codedjson-1.1.0/cjson/src/utils/__init__.py
--rw-rw-rw-   0        0        0      907 2023-06-10 13:01:00.000000 codedjson-1.1.0/cjson/src/utils/_is.py
--rw-rw-rw-   0        0        0     4454 2023-06-14 15:25:54.000000 codedjson-1.1.0/cjson/src/utils/_json.py
--rw-rw-rw-   0        0        0      204 2023-06-10 13:01:00.000000 codedjson-1.1.0/cjson/src/utils/file.py
--rw-rw-rw-   0        0        0      255 2023-06-14 12:28:54.000000 codedjson-1.1.0/cjson/src/utils/keywords.py
--rw-rw-rw-   0        0        0       42 2023-06-15 11:15:14.134882 codedjson-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1014 2023-06-15 11:15:11.000000 codedjson-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:54:15.475267 codedjson-1.1.1/
+-rw-rw-rw-   0        0        0     1093 2023-06-10 13:01:00.000000 codedjson-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3084 2023-06-19 16:54:15.475267 codedjson-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2335 2023-06-19 16:39:42.000000 codedjson-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 16:54:15.438513 codedjson-1.1.1/cjson/
+drwxrwxrwx   0        0        0        0 2023-06-19 16:54:15.459249 codedjson-1.1.1/cjson/src/
+-rw-rw-rw-   0        0        0     4032 2023-06-16 12:20:54.000000 codedjson-1.1.1/cjson/src/cjson.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:54:15.450548 codedjson-1.1.1/cjson/src/codedjson.egg-info/
+-rw-rw-rw-   0        0        0     3084 2023-06-19 16:54:15.000000 codedjson-1.1.1/cjson/src/codedjson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-06-19 16:54:15.000000 codedjson-1.1.1/cjson/src/codedjson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 16:54:15.000000 codedjson-1.1.1/cjson/src/codedjson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-19 16:54:15.000000 codedjson-1.1.1/cjson/src/codedjson.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 16:54:15.475267 codedjson-1.1.1/cjson/src/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-10 13:01:00.000000 codedjson-1.1.1/cjson/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-06-10 13:01:00.000000 codedjson-1.1.1/cjson/src/utils/_is.py
+-rw-rw-rw-   0        0        0     4454 2023-06-16 12:20:54.000000 codedjson-1.1.1/cjson/src/utils/_json.py
+-rw-rw-rw-   0        0        0      204 2023-06-10 13:01:00.000000 codedjson-1.1.1/cjson/src/utils/file.py
+-rw-rw-rw-   0        0        0      255 2023-06-16 12:20:54.000000 codedjson-1.1.1/cjson/src/utils/keywords.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 16:54:15.475267 codedjson-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1014 2023-06-19 16:54:07.000000 codedjson-1.1.1/setup.py
```

### Comparing `codedjson-1.1.0/LICENSE` & `codedjson-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codedjson-1.1.0/PKG-INFO` & `codedjson-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedjson
-Version: 1.1.0
+Version: 1.1.1
 Summary: Coded JSON files. Save your files with .cjson extension to unlock these features
 Home-page: UNKNOWN
 Author: Shubhendu Shekhar Gupta
 Author-email: subhendushekhargupta@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -23,21 +23,19 @@
     <br/>
     <br/>
     <h3> Coded Javascript Object Notation </h3>
     <br/>
     <h4> Why static JSON if you can utilize CJSON </h4>
     <br/>
     <br/>
-    <!-- <img src="https://github.com/SubhenduShekhar/cjson/actions/workflows/npm-publish.yml/badge.svg"/> -->
+    <img src="https://github.com/SubhenduShekhar/cjson/actions/workflows/tests.yml/badge.svg"/>
 </center>
 
 <br/>
 
-## NodeJS
-
 ### Your first CJSON code
 
 - Create file with `.cjson` extension
 - Write below code to decode the json:
 
 ```
     from cjson import Cjson
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: codedjson Version: 1.1.0 Summary: Coded JSON files.
+Metadata-Version: 2.1 Name: codedjson Version: 1.1.1 Summary: Coded JSON files.
 Save your files with .cjson extension to unlock these features Home-page:
 UNKNOWN Author: Shubhendu Shekhar Gupta Author-email:
 subhendushekhargupta@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.4 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6 Classifier: License :: OSI
@@ -11,24 +11,26 @@
  [https://github.com/SubhenduShekhar/cjson/blob/main/docs/logo.png?raw=true]
 
                   **** Coded Javascript Object Notation ****
 
                *** Why static JSON if you can utilize CJSON ***
 
 
+    [https://github.com/SubhenduShekhar/cjson/actions/workflows/tests.yml/
+                                  badge.svg]
 
-## NodeJS ### Your first CJSON code - Create file with `.cjson` extension -
-Write below code to decode the json: ``` from cjson import Cjson cjson = Cjson
-(file/path/to/file.cjson); var b = cjson.deserialize(); ``` #### Output: ```
-{ "source": { // Source JSON content }, "target": { "fruit": "Apple", "size":
-"Large", "color": "Red" } } ``` ### Features - [Import multiple JSON files]
-(#Import-multiple-JSON-files) - [Single/ Multiple line comments](#Single-
-Multiple-line-comments) - [Calling relative keys using JPATH](#Calling-
-relative-keys-using-JPATH) #### Import multiple JSON files You can use
-`$import` keyword for importing other JSON files.
+### Your first CJSON code - Create file with `.cjson` extension - Write below
+code to decode the json: ``` from cjson import Cjson cjson = Cjson(file/path/
+to/file.cjson); var b = cjson.deserialize(); ``` #### Output: ``` { "source":
+{ // Source JSON content }, "target": { "fruit": "Apple", "size": "Large",
+"color": "Red" } } ``` ### Features - [Import multiple JSON files](#Import-
+multiple-JSON-files) - [Single/ Multiple line comments](#Single-Multiple-line-
+comments) - [Calling relative keys using JPATH](#Calling-relative-keys-using-
+JPATH) #### Import multiple JSON files You can use `$import` keyword for
+importing other JSON files.
 You can also import multiple JSON files. ``` { "source": $import "./
 source.json", "target": { "fruit": "Apple", "size": "Large", "color": "Red" } }
 ``` #### Single/ Multiple line comments For single line comments, use `//` For
 multi line comments, use like below: ``` // This is first line comment // This
 is the second one ``` #### Calling relative keys using JPATH You can also refer
 to other variables using `$.` followed by jpath.
 Please note, the current version is only decoding using top to down approach ##
```

### Comparing `codedjson-1.1.0/README.md` & `codedjson-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,19 @@
     <br/>
     <br/>
     <h3> Coded Javascript Object Notation </h3>
     <br/>
     <h4> Why static JSON if you can utilize CJSON </h4>
     <br/>
     <br/>
-    <!-- <img src="https://github.com/SubhenduShekhar/cjson/actions/workflows/npm-publish.yml/badge.svg"/> -->
+    <img src="https://github.com/SubhenduShekhar/cjson/actions/workflows/tests.yml/badge.svg"/>
 </center>
 
 <br/>
 
-## NodeJS
-
 ### Your first CJSON code
 
 - Create file with `.cjson` extension
 - Write below code to decode the json:
 
 ```
     from cjson import Cjson
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
  [https://github.com/SubhenduShekhar/cjson/blob/main/docs/logo.png?raw=true]
 
                   **** Coded Javascript Object Notation ****
 
                *** Why static JSON if you can utilize CJSON ***
 
 
+    [https://github.com/SubhenduShekhar/cjson/actions/workflows/tests.yml/
+                                  badge.svg]
 
-## NodeJS ### Your first CJSON code - Create file with `.cjson` extension -
-Write below code to decode the json: ``` from cjson import Cjson cjson = Cjson
-(file/path/to/file.cjson); var b = cjson.deserialize(); ``` #### Output: ```
-{ "source": { // Source JSON content }, "target": { "fruit": "Apple", "size":
-"Large", "color": "Red" } } ``` ### Features - [Import multiple JSON files]
-(#Import-multiple-JSON-files) - [Single/ Multiple line comments](#Single-
-Multiple-line-comments) - [Calling relative keys using JPATH](#Calling-
-relative-keys-using-JPATH) #### Import multiple JSON files You can use
-`$import` keyword for importing other JSON files.
+### Your first CJSON code - Create file with `.cjson` extension - Write below
+code to decode the json: ``` from cjson import Cjson cjson = Cjson(file/path/
+to/file.cjson); var b = cjson.deserialize(); ``` #### Output: ``` { "source":
+{ // Source JSON content }, "target": { "fruit": "Apple", "size": "Large",
+"color": "Red" } } ``` ### Features - [Import multiple JSON files](#Import-
+multiple-JSON-files) - [Single/ Multiple line comments](#Single-Multiple-line-
+comments) - [Calling relative keys using JPATH](#Calling-relative-keys-using-
+JPATH) #### Import multiple JSON files You can use `$import` keyword for
+importing other JSON files.
 You can also import multiple JSON files. ``` { "source": $import "./
 source.json", "target": { "fruit": "Apple", "size": "Large", "color": "Red" } }
 ``` #### Single/ Multiple line comments For single line comments, use `//` For
 multi line comments, use like below: ``` // This is first line comment // This
 is the second one ``` #### Calling relative keys using JPATH You can also refer
 to other variables using `$.` followed by jpath.
 Please note, the current version is only decoding using top to down approach ##
```

### Comparing `codedjson-1.1.0/cjson/src/cjson.py` & `codedjson-1.1.1/cjson/src/cjson.py`

 * *Files identical despite different names*

### Comparing `codedjson-1.1.0/cjson/src/codedjson.egg-info/PKG-INFO` & `codedjson-1.1.1/cjson/src/codedjson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedjson
-Version: 1.1.0
+Version: 1.1.1
 Summary: Coded JSON files. Save your files with .cjson extension to unlock these features
 Home-page: UNKNOWN
 Author: Shubhendu Shekhar Gupta
 Author-email: subhendushekhargupta@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -23,21 +23,19 @@
     <br/>
     <br/>
     <h3> Coded Javascript Object Notation </h3>
     <br/>
     <h4> Why static JSON if you can utilize CJSON </h4>
     <br/>
     <br/>
-    <!-- <img src="https://github.com/SubhenduShekhar/cjson/actions/workflows/npm-publish.yml/badge.svg"/> -->
+    <img src="https://github.com/SubhenduShekhar/cjson/actions/workflows/tests.yml/badge.svg"/>
 </center>
 
 <br/>
 
-## NodeJS
-
 ### Your first CJSON code
 
 - Create file with `.cjson` extension
 - Write below code to decode the json:
 
 ```
     from cjson import Cjson
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: codedjson Version: 1.1.0 Summary: Coded JSON files.
+Metadata-Version: 2.1 Name: codedjson Version: 1.1.1 Summary: Coded JSON files.
 Save your files with .cjson extension to unlock these features Home-page:
 UNKNOWN Author: Shubhendu Shekhar Gupta Author-email:
 subhendushekhargupta@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.4 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6 Classifier: License :: OSI
@@ -11,24 +11,26 @@
  [https://github.com/SubhenduShekhar/cjson/blob/main/docs/logo.png?raw=true]
 
                   **** Coded Javascript Object Notation ****
 
                *** Why static JSON if you can utilize CJSON ***
 
 
+    [https://github.com/SubhenduShekhar/cjson/actions/workflows/tests.yml/
+                                  badge.svg]
 
-## NodeJS ### Your first CJSON code - Create file with `.cjson` extension -
-Write below code to decode the json: ``` from cjson import Cjson cjson = Cjson
-(file/path/to/file.cjson); var b = cjson.deserialize(); ``` #### Output: ```
-{ "source": { // Source JSON content }, "target": { "fruit": "Apple", "size":
-"Large", "color": "Red" } } ``` ### Features - [Import multiple JSON files]
-(#Import-multiple-JSON-files) - [Single/ Multiple line comments](#Single-
-Multiple-line-comments) - [Calling relative keys using JPATH](#Calling-
-relative-keys-using-JPATH) #### Import multiple JSON files You can use
-`$import` keyword for importing other JSON files.
+### Your first CJSON code - Create file with `.cjson` extension - Write below
+code to decode the json: ``` from cjson import Cjson cjson = Cjson(file/path/
+to/file.cjson); var b = cjson.deserialize(); ``` #### Output: ``` { "source":
+{ // Source JSON content }, "target": { "fruit": "Apple", "size": "Large",
+"color": "Red" } } ``` ### Features - [Import multiple JSON files](#Import-
+multiple-JSON-files) - [Single/ Multiple line comments](#Single-Multiple-line-
+comments) - [Calling relative keys using JPATH](#Calling-relative-keys-using-
+JPATH) #### Import multiple JSON files You can use `$import` keyword for
+importing other JSON files.
 You can also import multiple JSON files. ``` { "source": $import "./
 source.json", "target": { "fruit": "Apple", "size": "Large", "color": "Red" } }
 ``` #### Single/ Multiple line comments For single line comments, use `//` For
 multi line comments, use like below: ``` // This is first line comment // This
 is the second one ``` #### Calling relative keys using JPATH You can also refer
 to other variables using `$.` followed by jpath.
 Please note, the current version is only decoding using top to down approach ##
```

### Comparing `codedjson-1.1.0/cjson/src/codedjson.egg-info/SOURCES.txt` & `codedjson-1.1.1/cjson/src/codedjson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codedjson-1.1.0/cjson/src/utils/_is.py` & `codedjson-1.1.1/cjson/src/utils/_is.py`

 * *Files identical despite different names*

### Comparing `codedjson-1.1.0/cjson/src/utils/_json.py` & `codedjson-1.1.1/cjson/src/utils/_json.py`

 * *Files identical despite different names*

### Comparing `codedjson-1.1.0/setup.py` & `codedjson-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 __readme_file = open("README.md")
 __description = __readme_file.read()
 
 setuptools.setup(
     name="codedjson",
-    version="1.1.0",
+    version="1.1.1",
     description="Coded JSON files. Save your files with .cjson extension to unlock these features",
     long_description=__description,
     long_description_content_type="text/markdown",
     author="Shubhendu Shekhar Gupta",
     author_email="subhendushekhargupta@gmail.com",
     packages= [".", "utils/"],
     classifiers=[
```

