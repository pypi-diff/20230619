# Comparing `tmp/consolegame-0.0.3.tar.gz` & `tmp/consolegame-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consolegame-0.0.3.tar", last modified: Mon Jun 19 15:42:28 2023, max compression
+gzip compressed data, was "consolegame-0.0.4.tar", last modified: Mon Jun 19 16:09:57 2023, max compression
```

## Comparing `consolegame-0.0.3.tar` & `consolegame-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 15:42:28.526343 consolegame-0.0.3/
--rw-rw-rw-   0        0        0     1072 2023-06-19 14:25:38.000000 consolegame-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      219 2023-06-19 15:42:28.523900 consolegame-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1411 2023-06-19 14:49:30.000000 consolegame-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 15:42:28.520714 consolegame-0.0.3/consolegame.egg-info/
--rw-rw-rw-   0        0        0      219 2023-06-19 15:42:28.000000 consolegame-0.0.3/consolegame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-19 15:42:28.000000 consolegame-0.0.3/consolegame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 15:42:28.000000 consolegame-0.0.3/consolegame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 15:42:28.000000 consolegame-0.0.3/consolegame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-19 15:32:53.000000 consolegame-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 15:42:28.526731 consolegame-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      286 2023-06-19 15:41:52.000000 consolegame-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:09:57.366618 consolegame-0.0.4/
+-rw-rw-rw-   0        0        0     1072 2023-06-19 14:25:38.000000 consolegame-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      219 2023-06-19 16:09:57.361898 consolegame-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1411 2023-06-19 14:49:30.000000 consolegame-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 16:09:57.343542 consolegame-0.0.4/consolegame.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-06-19 16:09:57.000000 consolegame-0.0.4/consolegame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-19 16:09:57.000000 consolegame-0.0.4/consolegame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 16:09:57.000000 consolegame-0.0.4/consolegame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-19 16:09:57.000000 consolegame-0.0.4/consolegame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-19 15:32:53.000000 consolegame-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 16:09:57.367531 consolegame-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      279 2023-06-19 16:09:46.000000 consolegame-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:09:57.357529 consolegame-0.0.4/src/
+-rw-rw-rw-   0        0        0       47 2023-06-19 13:36:47.000000 consolegame-0.0.4/src/__init__.py
+-rw-rw-rw-   0        0        0      701 2023-06-19 13:35:14.000000 consolegame-0.0.4/src/functions.py
+-rw-rw-rw-   0        0        0     1233 2023-06-19 13:35:41.000000 consolegame-0.0.4/src/user.py
```

### Comparing `consolegame-0.0.3/LICENSE.txt` & `consolegame-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `consolegame-0.0.3/README.md` & `consolegame-0.0.4/README.md`

 * *Files identical despite different names*

