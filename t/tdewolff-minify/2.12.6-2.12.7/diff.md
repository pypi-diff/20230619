# Comparing `tmp/tdewolff-minify-2.12.6.tar.gz` & `tmp/tdewolff-minify-2.12.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdewolff-minify-2.12.6.tar", last modified: Fri May 26 14:53:42 2023, max compression
+gzip compressed data, was "tdewolff-minify-2.12.7.tar", last modified: Mon Jun 19 19:19:54 2023, max compression
```

## Comparing `tdewolff-minify-2.12.6.tar` & `tdewolff-minify-2.12.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-05-26 14:53:42.543719 tdewolff-minify-2.12.6/
--rw-r--r--   0 taco      (1000) users      (100)       87 2022-09-24 00:44:48.000000 tdewolff-minify-2.12.6/MANIFEST.in
--rw-r--r--   0 taco      (1000) users      (100)     1741 2023-05-26 14:53:42.543719 tdewolff-minify-2.12.6/PKG-INFO
--rw-r--r--   0 taco      (1000) users      (100)     1485 2023-05-26 14:39:15.000000 tdewolff-minify-2.12.6/README.md
--rw-r--r--   0 taco      (1000) users      (100)      144 2023-05-26 14:51:39.000000 tdewolff-minify-2.12.6/go.mod
--rw-r--r--   0 taco      (1000) users      (100)     1652 2023-05-26 14:51:39.000000 tdewolff-minify-2.12.6/go.sum
--rw-r--r--   0 taco      (1000) users      (100)     4818 2022-08-30 23:02:13.000000 tdewolff-minify-2.12.6/minify.c
--rw-r--r--   0 taco      (1000) users      (100)     5088 2023-05-26 14:52:13.000000 tdewolff-minify-2.12.6/minify.go
--rw-r--r--   0 taco      (1000) users      (100)      236 2022-09-23 17:18:06.000000 tdewolff-minify-2.12.6/minify.pyi
--rw-r--r--   0 taco      (1000) users      (100)        0 2022-09-23 16:09:33.000000 tdewolff-minify-2.12.6/py.typed
--rw-r--r--   0 taco      (1000) users      (100)       38 2023-05-26 14:53:42.543719 tdewolff-minify-2.12.6/setup.cfg
--rw-r--r--   0 taco      (1000) users      (100)     1356 2022-09-24 00:44:53.000000 tdewolff-minify-2.12.6/setup.py
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-05-26 14:53:42.543719 tdewolff-minify-2.12.6/tdewolff_minify.egg-info/
--rw-r--r--   0 taco      (1000) users      (100)     1741 2023-05-26 14:53:42.000000 tdewolff-minify-2.12.6/tdewolff_minify.egg-info/PKG-INFO
--rw-r--r--   0 taco      (1000) users      (100)      277 2023-05-26 14:53:42.000000 tdewolff-minify-2.12.6/tdewolff_minify.egg-info/SOURCES.txt
--rw-r--r--   0 taco      (1000) users      (100)        1 2023-05-26 14:53:42.000000 tdewolff-minify-2.12.6/tdewolff_minify.egg-info/dependency_links.txt
--rw-r--r--   0 taco      (1000) users      (100)        1 2023-05-26 14:53:42.000000 tdewolff-minify-2.12.6/tdewolff_minify.egg-info/not-zip-safe
--rw-r--r--   0 taco      (1000) users      (100)        7 2023-05-26 14:53:42.000000 tdewolff-minify-2.12.6/tdewolff_minify.egg-info/top_level.txt
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-06-19 19:19:54.731698 tdewolff-minify-2.12.7/
+-rw-r--r--   0 taco      (1000) users      (100)       87 2022-09-24 00:44:48.000000 tdewolff-minify-2.12.7/MANIFEST.in
+-rw-r--r--   0 taco      (1000) users      (100)     1741 2023-06-19 19:19:54.731698 tdewolff-minify-2.12.7/PKG-INFO
+-rw-r--r--   0 taco      (1000) users      (100)     1485 2023-05-26 14:39:15.000000 tdewolff-minify-2.12.7/README.md
+-rw-r--r--   0 taco      (1000) users      (100)      144 2023-06-19 19:19:33.000000 tdewolff-minify-2.12.7/go.mod
+-rw-r--r--   0 taco      (1000) users      (100)     1831 2023-06-19 19:19:33.000000 tdewolff-minify-2.12.7/go.sum
+-rw-r--r--   0 taco      (1000) users      (100)     4818 2022-08-30 23:02:13.000000 tdewolff-minify-2.12.7/minify.c
+-rw-r--r--   0 taco      (1000) users      (100)     5088 2023-05-26 14:52:13.000000 tdewolff-minify-2.12.7/minify.go
+-rw-r--r--   0 taco      (1000) users      (100)      236 2022-09-23 17:18:06.000000 tdewolff-minify-2.12.7/minify.pyi
+-rw-r--r--   0 taco      (1000) users      (100)        0 2022-09-23 16:09:33.000000 tdewolff-minify-2.12.7/py.typed
+-rw-r--r--   0 taco      (1000) users      (100)       38 2023-06-19 19:19:54.731698 tdewolff-minify-2.12.7/setup.cfg
+-rw-r--r--   0 taco      (1000) users      (100)     1356 2022-09-24 00:44:53.000000 tdewolff-minify-2.12.7/setup.py
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-06-19 19:19:54.731698 tdewolff-minify-2.12.7/tdewolff_minify.egg-info/
+-rw-r--r--   0 taco      (1000) users      (100)     1741 2023-06-19 19:19:54.000000 tdewolff-minify-2.12.7/tdewolff_minify.egg-info/PKG-INFO
+-rw-r--r--   0 taco      (1000) users      (100)      277 2023-06-19 19:19:54.000000 tdewolff-minify-2.12.7/tdewolff_minify.egg-info/SOURCES.txt
+-rw-r--r--   0 taco      (1000) users      (100)        1 2023-06-19 19:19:54.000000 tdewolff-minify-2.12.7/tdewolff_minify.egg-info/dependency_links.txt
+-rw-r--r--   0 taco      (1000) users      (100)        1 2023-06-19 19:19:54.000000 tdewolff-minify-2.12.7/tdewolff_minify.egg-info/not-zip-safe
+-rw-r--r--   0 taco      (1000) users      (100)        7 2023-06-19 19:19:54.000000 tdewolff-minify-2.12.7/tdewolff_minify.egg-info/top_level.txt
```

### Comparing `tdewolff-minify-2.12.6/PKG-INFO` & `tdewolff-minify-2.12.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdewolff-minify
-Version: 2.12.6
+Version: 2.12.7
 Summary: Go minifiers for web formats
 Home-page: https://github.com/tdewolff/minify
 Author: Taco de Wolff
 Author-email: tacodewolff@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `tdewolff-minify-2.12.6/README.md` & `tdewolff-minify-2.12.7/README.md`

 * *Files identical despite different names*

### Comparing `tdewolff-minify-2.12.6/go.sum` & `tdewolff-minify-2.12.7/go.sum`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 github.com/fsnotify/fsnotify v1.6.0/go.mod h1:sl3t1tCWJFWoRz9R8WJCbQihKKwmorjAbSClcnxKAGw=
 github.com/matryer/try v0.0.0-20161228173917-9ac251b645a2/go.mod h1:0KeJpeMD6o+O4hW7qJOT7vyQPKrWmj26uf5wMc/IiIs=
 github.com/spf13/pflag v1.0.5/go.mod h1:McXfInJRrz4CZXVZOBLb0bTZqETkiAhM9Iw0y3An2Bg=
 github.com/tdewolff/minify/v2 v2.12.5 h1:s2KDBt/D/3ayE3gcqQF8VIgTmYgkx+btuLvVAeePzZM=
 github.com/tdewolff/minify/v2 v2.12.5/go.mod h1:i8QXtVyL7Ddwc4I5gqzvgBqKlTMgMNTbiXaPO4Iqg+A=
 github.com/tdewolff/minify/v2 v2.12.6 h1:kw5FU0ErJyd7fs+TMojIlBvLyEjsN93wP1n8NUOs320=
 github.com/tdewolff/minify/v2 v2.12.6/go.mod h1:ZRKTheiOGyLSK8hOZWWv+YoJAECzDivNgAlVYDHp/Ws=
+github.com/tdewolff/minify/v2 v2.12.7 h1:pBzz2tAfz5VghOXiQIsSta6srhmTeinQPjRDHWoumCA=
+github.com/tdewolff/minify/v2 v2.12.7/go.mod h1:ZRKTheiOGyLSK8hOZWWv+YoJAECzDivNgAlVYDHp/Ws=
 github.com/tdewolff/parse/v2 v2.6.5 h1:lYvWBk55GkqKl0JJenGpmrgu/cPHQQ6/Mm1hBGswoGQ=
 github.com/tdewolff/parse/v2 v2.6.5/go.mod h1:woz0cgbLwFdtbjJu8PIKxhW05KplTFQkOdX78o+Jgrs=
 github.com/tdewolff/parse/v2 v2.6.6 h1:Yld+0CrKUJaCV78DL1G2nk3C9lKrxyRTux5aaK/AkDo=
 github.com/tdewolff/parse/v2 v2.6.6/go.mod h1:woz0cgbLwFdtbjJu8PIKxhW05KplTFQkOdX78o+Jgrs=
 github.com/tdewolff/test v1.0.7/go.mod h1:6DAvZliBAAnD7rhVgwaM7DE5/d9NMOAJ09SqYqeK4QE=
 github.com/tdewolff/test v1.0.9/go.mod h1:6DAvZliBAAnD7rhVgwaM7DE5/d9NMOAJ09SqYqeK4QE=
 golang.org/x/sys v0.0.0-20220908164124-27713097b956/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
```

### Comparing `tdewolff-minify-2.12.6/minify.c` & `tdewolff-minify-2.12.7/minify.c`

 * *Files identical despite different names*

### Comparing `tdewolff-minify-2.12.6/minify.go` & `tdewolff-minify-2.12.7/minify.go`

 * *Files identical despite different names*

### Comparing `tdewolff-minify-2.12.6/setup.py` & `tdewolff-minify-2.12.7/setup.py`

 * *Files identical despite different names*

### Comparing `tdewolff-minify-2.12.6/tdewolff_minify.egg-info/PKG-INFO` & `tdewolff-minify-2.12.7/tdewolff_minify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdewolff-minify
-Version: 2.12.6
+Version: 2.12.7
 Summary: Go minifiers for web formats
 Home-page: https://github.com/tdewolff/minify
 Author: Taco de Wolff
 Author-email: tacodewolff@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

