# Comparing `tmp/jira2json-0.1.1-py3-none-any.whl.zip` & `tmp/jira2json-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7212 bytes, number of entries: 8
--rw-r--r--  2.0 unx     8202 b- defN 23-May-20 05:34 jira2json/__init__.py
--rw-r--r--  2.0 unx     2788 b- defN 23-May-20 05:04 jira2json/__main__.py
--rw-r--r--  2.0 unx     1066 b- defN 23-May-20 05:35 jira2json-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3278 b- defN 23-May-20 05:35 jira2json-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-20 05:35 jira2json-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-May-20 05:35 jira2json-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-May-20 05:35 jira2json-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      649 b- defN 23-May-20 05:35 jira2json-0.1.1.dist-info/RECORD
-8 files, 16140 bytes uncompressed, 6076 bytes compressed:  62.4%
+Zip file size: 7220 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     8202 b- defN 23-Jun-16 13:09 jira2json/__init__.py
+-rw-r--r--  2.0 unx     2794 b- defN 23-Jun-16 13:07 jira2json/__main__.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jun-19 12:08 jira2json-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3280 b- defN 23-Jun-19 12:08 jira2json-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 12:08 jira2json-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-19 12:08 jira2json-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-19 12:08 jira2json-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      649 b- defN 23-Jun-19 12:08 jira2json-0.1.2.dist-info/RECORD
+8 files, 16148 bytes uncompressed, 6084 bytes compressed:  62.3%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: jira2json/__init__.py
 Comment: 
 
 Filename: jira2json/__main__.py
 Comment: 
 
-Filename: jira2json-0.1.1.dist-info/LICENSE
+Filename: jira2json-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: jira2json-0.1.1.dist-info/METADATA
+Filename: jira2json-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: jira2json-0.1.1.dist-info/WHEEL
+Filename: jira2json-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: jira2json-0.1.1.dist-info/entry_points.txt
+Filename: jira2json-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: jira2json-0.1.1.dist-info/top_level.txt
+Filename: jira2json-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: jira2json-0.1.1.dist-info/RECORD
+Filename: jira2json-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jira2json/__init__.py

```diff
@@ -1,11 +1,11 @@
 """A module for converting JIRA issues to JSON lines format."""
 
 __author__ = "Bar Harel"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __license__ = "MIT License"
 __all__ = ["iterate_jira_issues", "save_jsons_to_file", "parse_issues",
            "default_parsers"]
 
 import csv as _csv
 import json as _json
 import logging as _logging
```

## jira2json/__main__.py

```diff
@@ -8,15 +8,15 @@
 
 
 def _main():
     """Entry point of the program."""
 
     try:
         import dotenv
-        dotenv.load_dotenv()
+        dotenv.load_dotenv(".env")
     except ImportError:  # pragma: no cover
         pass
 
     logging.basicConfig(level=logging.WARNING)
 
     args = _parse_args()
```

## Comparing `jira2json-0.1.1.dist-info/LICENSE` & `jira2json-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jira2json-0.1.1.dist-info/METADATA` & `jira2json-0.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira2json
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dump JIRA issues to a dictionary / JSON.
 Home-page: https://github.com/bharel/jira_to_json
 Download-URL: https://pypi.org/project/jira2json/#files
 Author: Bar Harel
 Maintainer: Bar Harel
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -44,15 +44,15 @@
 
 Supports Jira Datacenter.
 
 ## Installation
 
 Install the library with pip:
 
-`pip install jira2json[dotenv]`
+`pip install "jira2json[dotenv]"`
 
 The `dotenv` extra installs the [python-dotenv](https://pypi.org/project/python-dotenv/)
 library, which is used to load the Jira server's url and the authentication token
 from a `.env` file.
 
 ## Usage
```

## Comparing `jira2json-0.1.1.dist-info/RECORD` & `jira2json-0.1.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-jira2json/__init__.py,sha256=PB2T1PlnZufT4dsJhKznrfOj8Wmu2jQ7d2hOBRMaQYo,8202
-jira2json/__main__.py,sha256=CTKSzhLcgG9wHb9nbmrWdi0W5eBslASr36D5_WUKvcQ,2788
-jira2json-0.1.1.dist-info/LICENSE,sha256=MaPhSU7il12T3Bcg0cXr-jnboVYaLvHmE_0kLh9vVoQ,1066
-jira2json-0.1.1.dist-info/METADATA,sha256=KyG1Pa7_6bQdoW1Zr-CuzrZTHf_g2JKcaBIVq7FA3bE,3278
-jira2json-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-jira2json-0.1.1.dist-info/entry_points.txt,sha256=MCMoXzRpUJinDnVYHsgxW4FWzRbBWIsKCnUHws-8GrY,55
-jira2json-0.1.1.dist-info/top_level.txt,sha256=2ntqVDpDmn-AuGSL3GGvo6FK4FwzmW9fI_1AgRyIgmc,10
-jira2json-0.1.1.dist-info/RECORD,,
+jira2json/__init__.py,sha256=BpWcbPSBJbvfe7P9zk2S7NUWdbtqcBZHAQ050gfGh5k,8202
+jira2json/__main__.py,sha256=7hslNh2JzE22QRvZsY7fJl1SyZZHUXmk5K8xSgq-jZA,2794
+jira2json-0.1.2.dist-info/LICENSE,sha256=MaPhSU7il12T3Bcg0cXr-jnboVYaLvHmE_0kLh9vVoQ,1066
+jira2json-0.1.2.dist-info/METADATA,sha256=VJ1keZ8tZ-qjFRZx7nZ2bb5UIIuEHfK--lp0_a9zPhk,3280
+jira2json-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+jira2json-0.1.2.dist-info/entry_points.txt,sha256=MCMoXzRpUJinDnVYHsgxW4FWzRbBWIsKCnUHws-8GrY,55
+jira2json-0.1.2.dist-info/top_level.txt,sha256=2ntqVDpDmn-AuGSL3GGvo6FK4FwzmW9fI_1AgRyIgmc,10
+jira2json-0.1.2.dist-info/RECORD,,
```

