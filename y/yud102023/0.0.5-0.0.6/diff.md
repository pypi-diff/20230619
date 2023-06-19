# Comparing `tmp/yud102023-0.0.5.tar.gz` & `tmp/yud102023-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yud102023-0.0.5.tar", last modified: Mon Jun 19 12:05:28 2023, max compression
+gzip compressed data, was "yud102023-0.0.6.tar", last modified: Mon Jun 19 12:12:59 2023, max compression
```

## Comparing `yud102023-0.0.5.tar` & `yud102023-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 12:05:28.286959 yud102023-0.0.5/
--rw-r--r--   0 tomereliel   (501) staff       (20)     1054 2023-06-18 22:55:32.000000 yud102023-0.0.5/LICENSE
--rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 12:05:28.286798 yud102023-0.0.5/PKG-INFO
--rw-r--r--   0 tomereliel   (501) staff       (20)       49 2023-06-18 22:56:17.000000 yud102023-0.0.5/README.md
--rw-r--r--   0 tomereliel   (501) staff       (20)      633 2023-06-19 12:05:22.000000 yud102023-0.0.5/pyproject.toml
--rw-r--r--   0 tomereliel   (501) staff       (20)       38 2023-06-19 12:05:28.287005 yud102023-0.0.5/setup.cfg
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 12:05:28.284318 yud102023-0.0.5/src/
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 12:05:28.285594 yud102023-0.0.5/src/yud102023/
--rw-r--r--   0 tomereliel   (501) staff       (20)    30062 2023-06-19 12:04:41.000000 yud102023-0.0.5/src/yud102023/goodbye.py
--rw-r--r--   0 tomereliel   (501) staff       (20)        0 2023-06-14 14:29:08.000000 yud102023-0.0.5/src/yud102023/init.py
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 12:05:28.286583 yud102023-0.0.5/src/yud102023.egg-info/
--rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 12:05:28.000000 yud102023-0.0.5/src/yud102023.egg-info/PKG-INFO
--rw-r--r--   0 tomereliel   (501) staff       (20)      263 2023-06-19 12:05:28.000000 yud102023-0.0.5/src/yud102023.egg-info/SOURCES.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)        1 2023-06-19 12:05:28.000000 yud102023-0.0.5/src/yud102023.egg-info/dependency_links.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)        9 2023-06-19 12:05:28.000000 yud102023-0.0.5/src/yud102023.egg-info/requires.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)       10 2023-06-19 12:05:28.000000 yud102023-0.0.5/src/yud102023.egg-info/top_level.txt
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 12:12:59.778280 yud102023-0.0.6/
+-rw-r--r--   0 tomereliel   (501) staff       (20)     1054 2023-06-18 22:55:32.000000 yud102023-0.0.6/LICENSE
+-rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 12:12:59.778140 yud102023-0.0.6/PKG-INFO
+-rw-r--r--   0 tomereliel   (501) staff       (20)       49 2023-06-18 22:56:17.000000 yud102023-0.0.6/README.md
+-rw-r--r--   0 tomereliel   (501) staff       (20)      633 2023-06-19 12:12:50.000000 yud102023-0.0.6/pyproject.toml
+-rw-r--r--   0 tomereliel   (501) staff       (20)       38 2023-06-19 12:12:59.778329 yud102023-0.0.6/setup.cfg
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 12:12:59.775975 yud102023-0.0.6/src/
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 12:12:59.777302 yud102023-0.0.6/src/yud102023/
+-rw-r--r--   0 tomereliel   (501) staff       (20)    30324 2023-06-19 12:11:54.000000 yud102023-0.0.6/src/yud102023/goodbye.py
+-rw-r--r--   0 tomereliel   (501) staff       (20)        0 2023-06-14 14:29:08.000000 yud102023-0.0.6/src/yud102023/init.py
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 12:12:59.777936 yud102023-0.0.6/src/yud102023.egg-info/
+-rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 12:12:59.000000 yud102023-0.0.6/src/yud102023.egg-info/PKG-INFO
+-rw-r--r--   0 tomereliel   (501) staff       (20)      263 2023-06-19 12:12:59.000000 yud102023-0.0.6/src/yud102023.egg-info/SOURCES.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)        1 2023-06-19 12:12:59.000000 yud102023-0.0.6/src/yud102023.egg-info/dependency_links.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)        9 2023-06-19 12:12:59.000000 yud102023-0.0.6/src/yud102023.egg-info/requires.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)       10 2023-06-19 12:12:59.000000 yud102023-0.0.6/src/yud102023.egg-info/top_level.txt
```

### Comparing `yud102023-0.0.5/LICENSE` & `yud102023-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yud102023-0.0.5/PKG-INFO` & `yud102023-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yud102023
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small creactive goodbye project for my students
 Author-email: Tomereliel <tomereliel.dev@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yud102023-0.0.5/pyproject.toml` & `yud102023-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "yud102023"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Tomereliel", email="tomereliel.dev@gmail.com" },
 ]
 description = "A small creactive goodbye project for my students"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `yud102023-0.0.5/src/yud102023/goodbye.py` & `yud102023-0.0.6/src/yud102023/goodbye.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,19 +80,23 @@
 }
 
 IDS = {"oren":b'$\x06Z\xd4\xaa\xbd\xedG{\xaf\x8d\xe2\xfb\xee\xfbt',
        "daniel":b'\x1c\x90\x07\xb1\x19\x1fV\xca\xf9\xc8~S\x99\xf2\xae\x8e',
        "yonatan":b'$\xf18\xa3P\x17\xc5\x05+\xd1\xe1KK}\x90\xdc',
        "avi":b'\x18\xc3m\x15\xed\xa4\xc3\xa1`\x86]\x11#\x7fC\xe3',
        "ido":b'z\xe4N\xd8/\x84r\xffV\xc0\x95\x90Ga\xb2\xa8',
+       "Edo":b'z\xe4N\xd8/\x84r\xffV\xc0\x95\x90Ga\xb2\xa8',
       "yarden":b'\xb9v\xcc\xd5\x0b\x9f\x0f\xcb\xfb\x86\xf48\xf6y\xb7\xae',
       "shahar":b'H\xe9\x1c\xe5\xc94\x14rE\xfd\xe8\x8d\x92\x92|a',
+      "shachar":b'H\xe9\x1c\xe5\xc94\x14rE\xfd\xe8\x8d\x92\x92|a',
       "itai":b'\xc2\xaf}\x95\xa2\x04\xb8_*\xa7\xd6\x91W\x90\x0c\xd6',
+      "itay":b'\xc2\xaf}\x95\xa2\x04\xb8_*\xa7\xd6\x91W\x90\x0c\xd6',
       "lior":b'\xa8*\xd3{T\xbd\xff`P\xb5\xa7m;\xf2\x91 ',
       "eliya":b'2mMOY\xdf\xee\x83\xb7\x8a\xddP\x16\xc2\xad\xd6',
+      "elia":b'2mMOY\xdf\xee\x83\xb7\x8a\xddP\x16\xc2\xad\xd6',
       "ron":b'4\xe0\xecx\xd37\xfc\xcc\x1e\xef\xe0\xe8\xa5/\x86('
        }
 
 HEB_BLESS = {"oren":'''
 אורן היקר,
 היה לי כיף ללמד אותך השנה.
 אתה אדם נעים וצנוע שכיף להיות לידו.
```

### Comparing `yud102023-0.0.5/src/yud102023.egg-info/PKG-INFO` & `yud102023-0.0.6/src/yud102023.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yud102023
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small creactive goodbye project for my students
 Author-email: Tomereliel <tomereliel.dev@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

