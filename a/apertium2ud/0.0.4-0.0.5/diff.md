# Comparing `tmp/apertium2ud-0.0.4.tar.gz` & `tmp/apertium2ud-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apertium2ud-0.0.4.tar", last modified: Fri Jun  2 23:08:37 2023, max compression
+gzip compressed data, was "apertium2ud-0.0.5.tar", last modified: Mon Jun 19 11:39:58 2023, max compression
```

## Comparing `apertium2ud-0.0.4.tar` & `apertium2ud-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 23:08:37.397187 apertium2ud-0.0.4/
--rwxrwxrwx   0 aam       (1000) aam       (1000)    35823 2023-05-19 10:05:32.000000 apertium2ud-0.0.4/LICENSE
--rwxrwxrwx   0 aam       (1000) aam       (1000)       50 2023-05-20 12:30:15.000000 apertium2ud-0.0.4/MANIFEST.in
--rwxrwxrwx   0 aam       (1000) aam       (1000)     2608 2023-06-02 23:08:37.388741 apertium2ud-0.0.4/PKG-INFO
--rwxrwxrwx   0 aam       (1000) aam       (1000)     2095 2023-05-26 10:57:10.000000 apertium2ud-0.0.4/README.md
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 23:08:36.715796 apertium2ud-0.0.4/apertium2ud/
--rwxrwxrwx   0 aam       (1000) aam       (1000)     2529 2023-06-02 23:07:37.000000 apertium2ud-0.0.4/apertium2ud/__init__.py
--rwxrwxrwx   0 aam       (1000) aam       (1000)     1856 2023-06-02 22:12:01.000000 apertium2ud-0.0.4/apertium2ud/_map_processing.py
--rwxrwxrwx   0 aam       (1000) aam       (1000)     1816 2023-06-02 22:50:42.000000 apertium2ud-0.0.4/apertium2ud/convert.py
--rwxrwxrwx   0 aam       (1000) aam       (1000)      234 2023-06-02 23:07:37.000000 apertium2ud-0.0.4/apertium2ud/meta.py
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 23:08:37.317320 apertium2ud-0.0.4/apertium2ud/resources/
--rwxrwxrwx   0 aam       (1000) aam       (1000)       25 2023-05-20 12:26:36.000000 apertium2ud-0.0.4/apertium2ud/resources/__init__.py
--rwxrwxrwx   0 aam       (1000) aam       (1000)     4037 2023-06-01 17:05:34.000000 apertium2ud-0.0.4/apertium2ud/resources/custom.udx
--rwxrwxrwx   0 aam       (1000) aam       (1000)    20114 2023-05-25 09:30:37.000000 apertium2ud-0.0.4/apertium2ud/resources/tags_map.json
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 23:08:37.010610 apertium2ud-0.0.4/apertium2ud.egg-info/
--rwxrwxrwx   0 aam       (1000) aam       (1000)     2608 2023-06-02 23:08:35.000000 apertium2ud-0.0.4/apertium2ud.egg-info/PKG-INFO
--rwxrwxrwx   0 aam       (1000) aam       (1000)      413 2023-06-02 23:08:36.000000 apertium2ud-0.0.4/apertium2ud.egg-info/SOURCES.txt
--rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-06-02 23:08:35.000000 apertium2ud-0.0.4/apertium2ud.egg-info/dependency_links.txt
--rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-06-02 23:08:34.000000 apertium2ud-0.0.4/apertium2ud.egg-info/not-zip-safe
--rwxrwxrwx   0 aam       (1000) aam       (1000)       12 2023-06-02 23:08:35.000000 apertium2ud-0.0.4/apertium2ud.egg-info/top_level.txt
--rwxrwxrwx   0 aam       (1000) aam       (1000)       38 2023-06-02 23:08:37.402189 apertium2ud-0.0.4/setup.cfg
--rwxrwxrwx   0 aam       (1000) aam       (1000)      951 2023-06-02 23:07:37.000000 apertium2ud-0.0.4/setup.py
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-19 11:39:58.386879 apertium2ud-0.0.5/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)    35823 2023-05-19 10:05:32.000000 apertium2ud-0.0.5/LICENSE
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       50 2023-05-20 12:30:15.000000 apertium2ud-0.0.5/MANIFEST.in
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     2912 2023-06-19 11:39:58.379131 apertium2ud-0.0.5/PKG-INFO
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     2408 2023-06-10 15:34:10.000000 apertium2ud-0.0.5/README.md
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-19 11:39:57.750684 apertium2ud-0.0.5/apertium2ud/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     2564 2023-06-19 11:32:52.000000 apertium2ud-0.0.5/apertium2ud/__init__.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     1856 2023-06-02 22:12:01.000000 apertium2ud-0.0.5/apertium2ud/_map_processing.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     2852 2023-06-19 11:37:39.000000 apertium2ud-0.0.5/apertium2ud/convert.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)      234 2023-06-10 15:20:10.000000 apertium2ud-0.0.5/apertium2ud/meta.py
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-19 11:39:58.307633 apertium2ud-0.0.5/apertium2ud/resources/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       25 2023-05-20 12:26:36.000000 apertium2ud-0.0.5/apertium2ud/resources/__init__.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     4037 2023-06-01 17:05:34.000000 apertium2ud-0.0.5/apertium2ud/resources/custom.udx
+-rwxrwxrwx   0 aam       (1000) aam       (1000)    20114 2023-05-25 09:30:37.000000 apertium2ud-0.0.5/apertium2ud/resources/tags_map.json
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-19 11:39:58.037689 apertium2ud-0.0.5/apertium2ud.egg-info/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     2912 2023-06-19 11:39:56.000000 apertium2ud-0.0.5/apertium2ud.egg-info/PKG-INFO
+-rwxrwxrwx   0 aam       (1000) aam       (1000)      413 2023-06-19 11:39:57.000000 apertium2ud-0.0.5/apertium2ud.egg-info/SOURCES.txt
+-rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-06-19 11:39:56.000000 apertium2ud-0.0.5/apertium2ud.egg-info/dependency_links.txt
+-rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-06-19 11:39:55.000000 apertium2ud-0.0.5/apertium2ud.egg-info/not-zip-safe
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       12 2023-06-19 11:39:56.000000 apertium2ud-0.0.5/apertium2ud.egg-info/top_level.txt
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       38 2023-06-19 11:39:58.390201 apertium2ud-0.0.5/setup.cfg
+-rwxrwxrwx   0 aam       (1000) aam       (1000)      951 2023-06-10 15:20:10.000000 apertium2ud-0.0.5/setup.py
```

### Comparing `apertium2ud-0.0.4/LICENSE` & `apertium2ud-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apertium2ud-0.0.4/PKG-INFO` & `apertium2ud-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apertium2ud
-Version: 0.0.4
+Version: 0.0.5
 Summary: Converting universal tags to Apertium tags.
 Home-page: https://github.com/alexeyev/apertium2ud
 Author: Anton Alekseev
 Author-email: anton.m.alexeye@gmail.com
 Keywords: natural language processing,apertium,morphology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -18,14 +18,23 @@
 
 Obtaining the mapping between the two tagsets based 
 on the [information from Apertium Wiki](https://wiki.apertium.org/w/index.php?title=List_of_symbols).
 
 Loosely based on [this code](https://github.com/mr-martian/apertium-recursive-learning/blob/master/tags.py), 
 hence the GPLv3 license.
 
+To install, run
+
+```bash
+python -m pip install apertium2ud
+```
+The latest uploaded version is 0.0.4.
+
+NB! The latest version from PyPI (yes, you can install the tool via pip) is equipped with the [apertium-kir](https://github.com/apertium/apertium-kir/blob/main/apertium-kir.kir.udx) `.udx` file rules.
+
 To build the machine-readable mapping, run
 
 ```bash
 python apertium_wiki_parser.py
 ```
 ## Apertium to Universal tags
```

### Comparing `apertium2ud-0.0.4/README.md` & `apertium2ud-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 
 Obtaining the mapping between the two tagsets based 
 on the [information from Apertium Wiki](https://wiki.apertium.org/w/index.php?title=List_of_symbols).
 
 Loosely based on [this code](https://github.com/mr-martian/apertium-recursive-learning/blob/master/tags.py), 
 hence the GPLv3 license.
 
+To install, run
+
+```bash
+python -m pip install apertium2ud
+```
+The latest uploaded version is 0.0.4.
+
+NB! The latest version from PyPI (yes, you can install the tool via pip) is equipped with the [apertium-kir](https://github.com/apertium/apertium-kir/blob/main/apertium-kir.kir.udx) `.udx` file rules.
+
 To build the machine-readable mapping, run
 
 ```bash
 python apertium_wiki_parser.py
 ```
 ## Apertium to Universal tags
```

### Comparing `apertium2ud-0.0.4/apertium2ud/__init__.py` & `apertium2ud-0.0.5/apertium2ud/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 # overriding
 for k, v in default_udx_mapping.items(): APERTIUM2UD_RULES[k] = v
 
 POS_TAGS_LIST = sorted(list(set(RAW_WIKI_MAP["POS"].keys())
                             .difference({"punkt"})
                             .union(RAW_WIKI_MAP["POS"]["punkt"].keys())))
+POS_TAGS_SET = set(POS_TAGS_LIST)
 
 OTHER_TAGS_LIST = sorted(list(set([t for k, v in UD2APERTIUM_RULES for t in v if not t in POS_TAGS_LIST])))
 
 ALL_APERTIUM_TAGS_LIST = POS_TAGS_LIST + OTHER_TAGS_LIST
 ALL_APERTIUM_TAGS_MAP = {tagname: idx for idx, tagname in enumerate(ALL_APERTIUM_TAGS_LIST)}
 
 # print(f"The first {len(POS_TAGS_LIST)} tags are PoS, the next {len(OTHER_TAGS_LIST)} are not.")
```

### Comparing `apertium2ud-0.0.4/apertium2ud/_map_processing.py` & `apertium2ud-0.0.5/apertium2ud/_map_processing.py`

 * *Files identical despite different names*

### Comparing `apertium2ud-0.0.4/apertium2ud/resources/custom.udx` & `apertium2ud-0.0.5/apertium2ud/resources/custom.udx`

 * *Files identical despite different names*

### Comparing `apertium2ud-0.0.4/apertium2ud/resources/tags_map.json` & `apertium2ud-0.0.5/apertium2ud/resources/tags_map.json`

 * *Files identical despite different names*

### Comparing `apertium2ud-0.0.4/apertium2ud.egg-info/PKG-INFO` & `apertium2ud-0.0.5/apertium2ud.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apertium2ud
-Version: 0.0.4
+Version: 0.0.5
 Summary: Converting universal tags to Apertium tags.
 Home-page: https://github.com/alexeyev/apertium2ud
 Author: Anton Alekseev
 Author-email: anton.m.alexeye@gmail.com
 Keywords: natural language processing,apertium,morphology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -18,14 +18,23 @@
 
 Obtaining the mapping between the two tagsets based 
 on the [information from Apertium Wiki](https://wiki.apertium.org/w/index.php?title=List_of_symbols).
 
 Loosely based on [this code](https://github.com/mr-martian/apertium-recursive-learning/blob/master/tags.py), 
 hence the GPLv3 license.
 
+To install, run
+
+```bash
+python -m pip install apertium2ud
+```
+The latest uploaded version is 0.0.4.
+
+NB! The latest version from PyPI (yes, you can install the tool via pip) is equipped with the [apertium-kir](https://github.com/apertium/apertium-kir/blob/main/apertium-kir.kir.udx) `.udx` file rules.
+
 To build the machine-readable mapping, run
 
 ```bash
 python apertium_wiki_parser.py
 ```
 ## Apertium to Universal tags
```

### Comparing `apertium2ud-0.0.4/setup.py` & `apertium2ud-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="apertium2ud",
     packages=setuptools.find_packages(),
-    version="0.0.4",
+    version="0.0.5",
     description="Converting universal tags to Apertium tags.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Anton Alekseev",
     author_email="anton.m.alexeye@gmail.com",
     url="https://github.com/alexeyev/apertium2ud",
     keywords=["natural language processing", "apertium", "morphology"],
```

