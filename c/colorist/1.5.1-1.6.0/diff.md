# Comparing `tmp/colorist-1.5.1.tar.gz` & `tmp/colorist-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorist-1.5.1.tar", last modified: Sat Apr 22 10:28:26 2023, max compression
+gzip compressed data, was "colorist-1.6.0.tar", last modified: Mon Jun 19 14:50:19 2023, max compression
```

## Comparing `colorist-1.5.1.tar` & `colorist-1.6.0.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.357324 colorist-1.5.1/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1759 2023-04-22 10:25:29.000000 colorist-1.5.1/INSTALLATION.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1503 2023-04-02 09:11:33.000000 colorist-1.5.1/LICENSE.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      217 2023-04-02 10:14:25.000000 colorist-1.5.1/MANIFEST.in
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    24114 2023-04-22 10:28:26.357447 colorist-1.5.1/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    19992 2023-04-22 10:25:30.000000 colorist-1.5.1/README.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      109 2023-01-25 13:58:40.000000 colorist-1.5.1/pyproject.toml
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1475 2023-04-22 10:28:26.357783 colorist-1.5.1/setup.cfg
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.344629 colorist-1.5.1/src/
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.346742 colorist-1.5.1/src/colorist/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2666 2023-04-22 08:37:25.000000 colorist-1.5.1/src/colorist/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.348273 colorist-1.5.1/src/colorist/constants/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      149 2023-04-09 23:12:39.000000 colorist-1.5.1/src/colorist/constants/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2181 2023-04-11 11:49:16.000000 colorist-1.5.1/src/colorist/constants/ansi.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      502 2023-04-09 23:12:39.000000 colorist-1.5.1/src/colorist/constants/ascii.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.350350 colorist-1.5.1/src/colorist/helper/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)   110592 2023-04-09 21:09:53.000000 colorist-1.5.1/src/colorist/helper/.coverage
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.351033 colorist-1.5.1/src/colorist/helper/.pytest_cache/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       37 2023-04-02 09:52:54.000000 colorist-1.5.1/src/colorist/helper/.pytest_cache/.gitignore
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      191 2023-04-02 09:52:54.000000 colorist-1.5.1/src/colorist/helper/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      302 2023-04-02 09:52:54.000000 colorist-1.5.1/src/colorist/helper/.pytest_cache/README.md
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.344910 colorist-1.5.1/src/colorist/helper/.pytest_cache/v/
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.351449 colorist-1.5.1/src/colorist/helper/.pytest_cache/v/cache/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.5.1/src/colorist/helper/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.5.1/src/colorist/helper/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      215 2023-04-09 23:12:39.000000 colorist-1.5.1/src/colorist/helper/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1973 2023-04-22 10:25:27.000000 colorist-1.5.1/src/colorist/helper/convert.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      733 2023-04-22 10:25:27.000000 colorist-1.5.1/src/colorist/helper/error.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1222 2023-04-09 23:12:39.000000 colorist-1.5.1/src/colorist/helper/generate.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1220 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/helper/print.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      492 2023-04-21 23:37:48.000000 colorist-1.5.1/src/colorist/helper/validate.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.351890 colorist-1.5.1/src/colorist/model/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1789 2023-04-22 08:37:25.000000 colorist-1.5.1/src/colorist/model/README.MD
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.353402 colorist-1.5.1/src/colorist/model/abc/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      572 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/abc/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      426 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/abc/effect.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1329 2023-04-22 10:25:27.000000 colorist-1.5.1/src/colorist/model/abc/hex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1915 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/abc/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1326 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/abc/rgb.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.354374 colorist-1.5.1/src/colorist/model/background/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1410 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/background/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1306 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/background/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      428 2023-04-22 10:25:27.000000 colorist-1.5.1/src/colorist/model/background/hex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      417 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/background/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      412 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/background/rgb.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1516 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/effect.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.355101 colorist-1.5.1/src/colorist/model/foreground/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1402 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/foreground/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1298 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/foreground/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      431 2023-04-22 10:25:27.000000 colorist-1.5.1/src/colorist/model/foreground/hex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      420 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/foreground/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      415 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/foreground/rgb.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.355239 colorist-1.5.1/src/colorist/print/
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.356133 colorist-1.5.1/src/colorist/print/background/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2509 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/background/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1320 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/background/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      418 2023-04-22 10:25:27.000000 colorist-1.5.1/src/colorist/print/background/hex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      518 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/background/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      355 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/background/rgb.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1395 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/effect.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.357181 colorist-1.5.1/src/colorist/print/foreground/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2331 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/foreground/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1142 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/foreground/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      382 2023-04-22 10:25:27.000000 colorist-1.5.1/src/colorist/print/foreground/hex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      498 2023-04-21 23:04:21.000000 colorist-1.5.1/src/colorist/print/foreground/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      335 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/foreground/rgb.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-01-25 13:58:40.000000 colorist-1.5.1/src/colorist/py.typed
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      174 2023-04-22 10:25:30.000000 colorist-1.5.1/src/colorist/version.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.347634 colorist-1.5.1/src/colorist.egg-info/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    24114 2023-04-22 10:28:26.000000 colorist-1.5.1/src/colorist.egg-info/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1934 2023-04-22 10:28:26.000000 colorist-1.5.1/src/colorist.egg-info/SOURCES.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-04-22 10:28:26.000000 colorist-1.5.1/src/colorist.egg-info/dependency_links.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-26 21:13:43.000000 colorist-1.5.1/src/colorist.egg-info/not-zip-safe
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       97 2023-04-22 10:28:26.000000 colorist-1.5.1/src/colorist.egg-info/requires.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        9 2023-04-22 10:28:26.000000 colorist-1.5.1/src/colorist.egg-info/top_level.txt
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.275304 colorist-1.6.0/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1827 2023-06-19 14:42:06.000000 colorist-1.6.0/INSTALLATION.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1503 2023-04-02 09:11:33.000000 colorist-1.6.0/LICENSE.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      217 2023-04-02 10:14:25.000000 colorist-1.6.0/MANIFEST.in
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    24217 2023-06-19 14:50:19.275415 colorist-1.6.0/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    20077 2023-06-19 14:42:06.000000 colorist-1.6.0/README.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      109 2023-01-25 13:58:40.000000 colorist-1.6.0/pyproject.toml
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1429 2023-06-19 14:50:19.275739 colorist-1.6.0/setup.cfg
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.262969 colorist-1.6.0/src/
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.264702 colorist-1.6.0/src/colorist/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2724 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.266555 colorist-1.6.0/src/colorist/constants/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      149 2023-04-09 23:12:39.000000 colorist-1.6.0/src/colorist/constants/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2181 2023-04-11 11:49:16.000000 colorist-1.6.0/src/colorist/constants/ansi.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      502 2023-04-09 23:12:39.000000 colorist-1.6.0/src/colorist/constants/ascii.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.268506 colorist-1.6.0/src/colorist/helper/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)   110592 2023-04-09 21:09:53.000000 colorist-1.6.0/src/colorist/helper/.coverage
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.269227 colorist-1.6.0/src/colorist/helper/.pytest_cache/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       37 2023-04-02 09:52:54.000000 colorist-1.6.0/src/colorist/helper/.pytest_cache/.gitignore
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      191 2023-04-02 09:52:54.000000 colorist-1.6.0/src/colorist/helper/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      302 2023-04-02 09:52:54.000000 colorist-1.6.0/src/colorist/helper/.pytest_cache/README.md
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.263243 colorist-1.6.0/src/colorist/helper/.pytest_cache/v/
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.269622 colorist-1.6.0/src/colorist/helper/.pytest_cache/v/cache/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.6.0/src/colorist/helper/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.6.0/src/colorist/helper/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      215 2023-04-23 10:26:22.000000 colorist-1.6.0/src/colorist/helper/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1973 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/helper/convert.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      733 2023-04-22 10:25:27.000000 colorist-1.6.0/src/colorist/helper/error.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1222 2023-04-09 23:12:39.000000 colorist-1.6.0/src/colorist/helper/generate.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1181 2023-04-25 04:39:14.000000 colorist-1.6.0/src/colorist/helper/print.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      493 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/helper/validate.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.270026 colorist-1.6.0/src/colorist/model/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1789 2023-04-22 08:37:25.000000 colorist-1.6.0/src/colorist/model/README.MD
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.271053 colorist-1.6.0/src/colorist/model/abc/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      572 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/abc/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      426 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/abc/effect.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1329 2023-04-22 10:25:27.000000 colorist-1.6.0/src/colorist/model/abc/hex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1915 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/abc/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1326 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/abc/rgb.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.272151 colorist-1.6.0/src/colorist/model/background/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1410 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/background/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1306 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/background/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      504 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/model/background/hex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      541 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/model/background/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      466 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/model/background/rgb.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1516 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/effect.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.272993 colorist-1.6.0/src/colorist/model/foreground/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1402 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/foreground/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1298 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/foreground/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      507 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/model/foreground/hex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      544 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/model/foreground/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      469 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/model/foreground/rgb.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.273322 colorist-1.6.0/src/colorist/print/
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.274194 colorist-1.6.0/src/colorist/print/background/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2509 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/print/background/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1320 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/print/background/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      461 2023-04-23 22:57:28.000000 colorist-1.6.0/src/colorist/print/background/hex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      561 2023-04-23 22:57:28.000000 colorist-1.6.0/src/colorist/print/background/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      465 2023-04-23 22:57:28.000000 colorist-1.6.0/src/colorist/print/background/rgb.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1395 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/print/effect.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.275134 colorist-1.6.0/src/colorist/print/foreground/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2331 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/print/foreground/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1142 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/print/foreground/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      415 2023-04-23 22:57:28.000000 colorist-1.6.0/src/colorist/print/foreground/hex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      531 2023-04-23 22:57:28.000000 colorist-1.6.0/src/colorist/print/foreground/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      435 2023-04-23 22:57:28.000000 colorist-1.6.0/src/colorist/print/foreground/rgb.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1318 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/print/general.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-01-25 13:58:40.000000 colorist-1.6.0/src/colorist/py.typed
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      174 2023-06-19 14:42:06.000000 colorist-1.6.0/src/colorist/version.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.265798 colorist-1.6.0/src/colorist.egg-info/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    24217 2023-06-19 14:50:19.000000 colorist-1.6.0/src/colorist.egg-info/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1964 2023-06-19 14:50:19.000000 colorist-1.6.0/src/colorist.egg-info/SOURCES.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-06-19 14:50:19.000000 colorist-1.6.0/src/colorist.egg-info/dependency_links.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-26 21:13:43.000000 colorist-1.6.0/src/colorist.egg-info/not-zip-safe
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       96 2023-06-19 14:50:19.000000 colorist-1.6.0/src/colorist.egg-info/requires.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        9 2023-06-19 14:50:19.000000 colorist-1.6.0/src/colorist.egg-info/top_level.txt
```

### Comparing `colorist-1.5.1/INSTALLATION.md` & `colorist-1.6.0/INSTALLATION.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
-![Python 2.7 | 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=2.7%20|%203.10%20|%203.11%2B&color=blueviolet)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.6.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
-[![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
+[![Codecov](https://codecov.io/gh/jakob-bagterp/colorist-for-python/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
+[![Downloads](https://static.pepy.tech/badge/colorist)](https://pepy.tech/project/colorist)
 
 # 🌈 How to Install Colorist for Python 🌈
 ## Prerequisites
-* Python version:
-    * 2.7
-    * 3.10, 3.11 or higher
+* Python version 3.10, 3.11 or higher
 * Terminal that supports color (i.e. [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code))
 
 ## Installation
 ### PyPI
 Assuming that Python is installed already, execute this command in the terminal:
 
 ```shell
```

### Comparing `colorist-1.5.1/LICENSE.md` & `colorist-1.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/PKG-INFO` & `colorist-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: colorist
-Version: 1.5.1
+Version: 1.6.0
 Summary: Colorist for Python
 Home-page: https://github.com/jakob-bagterp/colorist-for-python
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
 License: 3-Clause BSD License
 Project-URL: Bug Tracker, https://github.com/jakob-bagterp/colorist-for-python/issues
 Keywords: python,colors,terminal
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
-![Python 2.7 | 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=2.7%20|%203.10%20|%203.11%2B&color=blueviolet)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.6.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
-[![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
+[![Codecov](https://codecov.io/gh/jakob-bagterp/colorist-for-python/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
+[![Downloads](https://static.pepy.tech/badge/colorist)](https://pepy.tech/project/colorist)
 
 # 🌈 Colorist for Python 🌈
 Lightweight Python package that makes it easy and fast to print colored text in the terminal.
 
 Ready to try? [Learn how to install](https://github.com/jakob-bagterp/colorist-for-python/blob/master/INSTALLATION.md).
 
 ## Getting Started
@@ -351,25 +351,24 @@
 
 ## Contribute
 If you have suggestions or changes to the module, feel free to add to the code and create a [pull request](https://github.com/jakob-bagterp/colorist-for-python/pulls).
 
 ## Report Bugs
 Report bugs and issues [here](https://github.com/jakob-bagterp/colorist-for-python/issues).
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
-![Python 2.7 | 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=2.7%20|%203.10%20|%203.11%2B&color=blueviolet)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.6.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
-[![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
+[![Codecov](https://codecov.io/gh/jakob-bagterp/colorist-for-python/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
+[![Downloads](https://static.pepy.tech/badge/colorist)](https://pepy.tech/project/colorist)
 
 # 🌈 How to Install Colorist for Python 🌈
 ## Prerequisites
-* Python version:
-    * 2.7
-    * 3.10, 3.11 or higher
+* Python version 3.10, 3.11 or higher
 * Terminal that supports color (i.e. [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code))
 
 ## Installation
 ### PyPI
 Assuming that Python is installed already, execute this command in the terminal:
 
 ```shell
```

### Comparing `colorist-1.5.1/README.md` & `colorist-1.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
-![Python 2.7 | 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=2.7%20|%203.10%20|%203.11%2B&color=blueviolet)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.6.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
-[![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
+[![Codecov](https://codecov.io/gh/jakob-bagterp/colorist-for-python/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
+[![Downloads](https://static.pepy.tech/badge/colorist)](https://pepy.tech/project/colorist)
 
 # 🌈 Colorist for Python 🌈
 Lightweight Python package that makes it easy and fast to print colored text in the terminal.
 
 Ready to try? [Learn how to install](https://github.com/jakob-bagterp/colorist-for-python/blob/master/INSTALLATION.md).
 
 ## Getting Started
```

### Comparing `colorist-1.5.1/setup.cfg` & `colorist-1.6.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 	python
 	colors
 	terminal
 url = https://github.com/jakob-bagterp/colorist-for-python
 project_urls = 
 	Bug Tracker = https://github.com/jakob-bagterp/colorist-for-python/issues
 classifiers = 
-	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 license = 3-Clause BSD License
 license_files = LICENSE.md
@@ -31,20 +30,20 @@
 packages = find:
 python_requires = >=3.10
 zip_safe = no
 include_package_data = True
 
 [options.extras_require]
 testing = 
-	coverage ==7.2.3
-	flake8 ==6.0.0
-	mypy ==1.2.0
-	pytest ==7.3.1
-	pytest-cov ==4.0.0
-	tox ==4.4.12
+	coverage==7.2.7
+	flake8==6.0.0
+	mypy==1.3.0
+	pytest==7.3.2
+	pytest-cov==4.1.0
+	tox==4.6.0
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 colorist = py.typed
```

### Comparing `colorist-1.5.1/src/colorist/__init__.py` & `colorist-1.6.0/src/colorist/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright 2022 – present, Jakob Bagterp. BSD 3-Clause license and refer to LICENSE file.
 
 __all__ = [
     "Color", "BrightColor", "BgColor", "BgBrightColor", "ColorHex", "BgColorHex", "ColorRGB", "BgColorRGB", "ColorHSL", "BgColorHSL", "Effect",
+    "print_color",
     "black", "red", "green", "yellow", "blue", "magenta", "cyan", "white",
     "bright_black", "bright_red", "bright_green", "bright_yellow", "bright_blue", "bright_magenta", "bright_cyan", "bright_white",
     "bg_black", "bg_red", "bg_green", "bg_yellow", "bg_blue", "bg_magenta", "bg_cyan", "bg_white",
     "bg_bright_black", "bg_bright_red", "bg_bright_green", "bg_bright_yellow", "bg_bright_blue", "bg_bright_magenta", "bg_bright_cyan", "bg_bright_white",
     "effect_bold", "effect_dim", "effect_underline", "effect_blink", "effect_reverse", "effect_hide",
     "hex", "rgb", "hsl",
     "bg_hex", "bg_rgb", "bg_hsl"
@@ -38,8 +39,9 @@
                                             bright_magenta, bright_red,
                                             bright_white, bright_yellow)
 from .print.foreground.color import (black, blue, cyan, green, magenta, red,
                                      white, yellow)
 from .print.foreground.hex import hex
 from .print.foreground.hsl import hsl
 from .print.foreground.rgb import rgb
+from .print.general import print_color
 from .version import __version__  # noqa
```

### Comparing `colorist-1.5.1/src/colorist/constants/ansi.py` & `colorist-1.6.0/src/colorist/constants/ansi.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/helper/.coverage` & `colorist-1.6.0/src/colorist/helper/.coverage`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/helper/convert.py` & `colorist-1.6.0/src/colorist/helper/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # Copyright 2022 – present, Jakob Bagterp. BSD 3-Clause license and refer to LICENSE file.
 
 import colorsys
 
 from ..helper.error import message_for_hex_value_error
 
 
-def normalise_colorsys_rgb_to_real_rgb(rgb_colorsys: tuple[float, float, float]) -> tuple[int, int, int]:
-    """Since Colorsys outputs RGB values as floats between 0.0 an 1.0, we need to normalise this to a standard RGB scale from 0 to 255."""
+def normalize_colorsys_rgb_to_real_rgb(rgb_colorsys: tuple[float, float, float]) -> tuple[int, int, int]:
+    """Since Colorsys outputs RGB values as floats between 0.0 an 1.0, we need to normalize this to a standard RGB scale from 0 to 255."""
 
     red, green, blue = tuple(int(color * 255) for color in rgb_colorsys)
     return red, green, blue
 
 
-def normalise_hue_degrees_to_colorsys_hue(hue: float) -> float:
+def normalize_hue_degrees_to_colorsys_hue(hue: float) -> float:
     """When converting HLS or HSV with Colorsys, we need to prepare hue between 0 and 360 degrees to a float between 0.0 and 1.0."""
 
     return hue / 360.0
 
 
-def normalise_percentage_to_colorsys_value(value: float) -> float:
+def normalize_percentage_to_colorsys_value(value: float) -> float:
     """When converting HLS or HSV with Colorsys, we need to prepare lightness, saturation, etc. percentages between 0% and 100% to a float between 0.0 and 1.0."""
 
     return value / 100.0
 
 
 def hsl_to_rgb(hue: float, saturation: float, lightness: float) -> tuple[int, int, int]:
-    hue_colorsys = normalise_hue_degrees_to_colorsys_hue(hue)
-    saturation_colorsys = normalise_percentage_to_colorsys_value(saturation)
-    lightness_colorsys = normalise_percentage_to_colorsys_value(lightness)
+    hue_colorsys = normalize_hue_degrees_to_colorsys_hue(hue)
+    saturation_colorsys = normalize_percentage_to_colorsys_value(saturation)
+    lightness_colorsys = normalize_percentage_to_colorsys_value(lightness)
     rgb_colorsys = colorsys.hls_to_rgb(hue_colorsys, lightness_colorsys, saturation_colorsys)
-    return normalise_colorsys_rgb_to_real_rgb(rgb_colorsys)
+    return normalize_colorsys_rgb_to_real_rgb(rgb_colorsys)
 
 
 def hex_to_rgb(hex: str) -> tuple[int, int, int]:
     """Convert Hex color to RGB. Expects valid Hex color value, for instance #B4FBB8 or B4FBB8, #B4F or B4F."""
 
     hex = hex.lstrip("#")
     if len(hex) == 3:
```

### Comparing `colorist-1.5.1/src/colorist/helper/error.py` & `colorist-1.6.0/src/colorist/helper/error.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/helper/generate.py` & `colorist-1.6.0/src/colorist/helper/generate.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/model/README.MD` & `colorist-1.6.0/src/colorist/model/README.MD`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/model/abc/color.py` & `colorist-1.6.0/src/colorist/model/abc/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/model/abc/hex.py` & `colorist-1.6.0/src/colorist/model/abc/hex.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/model/abc/hsl.py` & `colorist-1.6.0/src/colorist/model/abc/hsl.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/model/abc/rgb.py` & `colorist-1.6.0/src/colorist/model/abc/rgb.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/model/background/bright_color.py` & `colorist-1.6.0/src/colorist/model/background/bright_color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/model/background/color.py` & `colorist-1.6.0/src/colorist/model/background/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/model/effect.py` & `colorist-1.6.0/src/colorist/model/effect.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/model/foreground/bright_color.py` & `colorist-1.6.0/src/colorist/model/foreground/bright_color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/model/foreground/color.py` & `colorist-1.6.0/src/colorist/model/foreground/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/print/background/bright_color.py` & `colorist-1.6.0/src/colorist/print/background/bright_color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/print/background/color.py` & `colorist-1.6.0/src/colorist/print/background/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/print/background/hsl.py` & `colorist-1.6.0/src/colorist/print/background/hsl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright 2022 – present, Jakob Bagterp. BSD 3-Clause license and refer to LICENSE file.
 
-from ... import helper
+from ...model.background.hsl import BgColorHSL
+from ...print.general import print_color
 
 
 def bg_hsl(text: str, hue: float, saturation: float, lightness: float) -> None:
     """Prints full line of text on custom HSL-colored background. Value for hue can be between 0 and 360 degrees, while saturation and lightness can be a percentage between 0(%) and 100(%)."""
 
-    red, green, blue = helper.convert.hsl_to_rgb(hue, lightness, saturation)
-    helper.print.bg_rgb(text, red, green, blue)
+    bg_color_hsl = BgColorHSL(hue, lightness, saturation)
+    print_color(text, bg_color=bg_color_hsl)
```

### Comparing `colorist-1.5.1/src/colorist/print/effect.py` & `colorist-1.6.0/src/colorist/print/effect.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/print/foreground/bright_color.py` & `colorist-1.6.0/src/colorist/print/foreground/bright_color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist/print/foreground/color.py` & `colorist-1.6.0/src/colorist/print/foreground/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.5.1/src/colorist.egg-info/PKG-INFO` & `colorist-1.6.0/src/colorist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: colorist
-Version: 1.5.1
+Version: 1.6.0
 Summary: Colorist for Python
 Home-page: https://github.com/jakob-bagterp/colorist-for-python
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
 License: 3-Clause BSD License
 Project-URL: Bug Tracker, https://github.com/jakob-bagterp/colorist-for-python/issues
 Keywords: python,colors,terminal
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
-![Python 2.7 | 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=2.7%20|%203.10%20|%203.11%2B&color=blueviolet)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.6.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
-[![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
+[![Codecov](https://codecov.io/gh/jakob-bagterp/colorist-for-python/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
+[![Downloads](https://static.pepy.tech/badge/colorist)](https://pepy.tech/project/colorist)
 
 # 🌈 Colorist for Python 🌈
 Lightweight Python package that makes it easy and fast to print colored text in the terminal.
 
 Ready to try? [Learn how to install](https://github.com/jakob-bagterp/colorist-for-python/blob/master/INSTALLATION.md).
 
 ## Getting Started
@@ -351,25 +351,24 @@
 
 ## Contribute
 If you have suggestions or changes to the module, feel free to add to the code and create a [pull request](https://github.com/jakob-bagterp/colorist-for-python/pulls).
 
 ## Report Bugs
 Report bugs and issues [here](https://github.com/jakob-bagterp/colorist-for-python/issues).
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
-![Python 2.7 | 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=2.7%20|%203.10%20|%203.11%2B&color=blueviolet)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.6.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
-[![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
+[![Codecov](https://codecov.io/gh/jakob-bagterp/colorist-for-python/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
+[![Downloads](https://static.pepy.tech/badge/colorist)](https://pepy.tech/project/colorist)
 
 # 🌈 How to Install Colorist for Python 🌈
 ## Prerequisites
-* Python version:
-    * 2.7
-    * 3.10, 3.11 or higher
+* Python version 3.10, 3.11 or higher
 * Terminal that supports color (i.e. [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code))
 
 ## Installation
 ### PyPI
 Assuming that Python is installed already, execute this command in the terminal:
 
 ```shell
```

### Comparing `colorist-1.5.1/src/colorist.egg-info/SOURCES.txt` & `colorist-1.6.0/src/colorist.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 src/colorist/model/background/rgb.py
 src/colorist/model/foreground/bright_color.py
 src/colorist/model/foreground/color.py
 src/colorist/model/foreground/hex.py
 src/colorist/model/foreground/hsl.py
 src/colorist/model/foreground/rgb.py
 src/colorist/print/effect.py
+src/colorist/print/general.py
 src/colorist/print/background/bright_color.py
 src/colorist/print/background/color.py
 src/colorist/print/background/hex.py
 src/colorist/print/background/hsl.py
 src/colorist/print/background/rgb.py
 src/colorist/print/foreground/bright_color.py
 src/colorist/print/foreground/color.py
```

