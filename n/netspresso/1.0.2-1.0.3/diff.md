# Comparing `tmp/netspresso-1.0.2.tar.gz` & `tmp/netspresso-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netspresso-1.0.2.tar", last modified: Mon Jun 19 08:20:00 2023, max compression
+gzip compressed data, was "netspresso-1.0.3.tar", last modified: Mon Jun 19 09:42:26 2023, max compression
```

## Comparing `netspresso-1.0.2.tar` & `netspresso-1.0.3.tar`

### file list

```diff
@@ -1,85 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 08:20:00.097537 netspresso-1.0.2/
--rw-rw-rw-   0        0        0    11558 2023-06-12 20:26:38.000000 netspresso-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      100 2023-06-19 08:15:31.000000 netspresso-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6997 2023-06-19 08:20:00.096541 netspresso-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6546 2023-06-19 07:37:38.000000 netspresso-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 08:19:59.842000 netspresso-1.0.2/imgs/
-drwxrwxrwx   0        0        0        0 2023-06-19 08:19:59.882891 netspresso-1.0.2/imgs/banner/
--rw-rw-rw-   0        0        0   264662 2023-06-19 07:37:38.000000 netspresso-1.0.2/imgs/banner/pynp_main.png
-drwxrwxrwx   0        0        0        0 2023-06-19 08:19:59.955241 netspresso-1.0.2/imgs/common/
--rw-rw-rw-   0        0        0     6203 2023-06-19 07:37:38.000000 netspresso-1.0.2/imgs/common/facebook.png
--rw-rw-rw-   0        0        0    11521 2023-06-19 07:37:38.000000 netspresso-1.0.2/imgs/common/facebook_white.png
--rw-rw-rw-   0        0        0    16945 2023-06-19 07:37:38.000000 netspresso-1.0.2/imgs/common/github.png
--rw-rw-rw-   0        0        0    23987 2023-06-19 07:37:38.000000 netspresso-1.0.2/imgs/common/github_white.png
--rw-rw-rw-   0        0        0     7269 2023-06-19 07:37:38.000000 netspresso-1.0.2/imgs/common/linkedin.png
--rw-rw-rw-   0        0        0    12503 2023-06-19 07:37:38.000000 netspresso-1.0.2/imgs/common/linkedin_white.png
--rw-rw-rw-   0        0        0      163 2023-06-19 07:37:38.000000 netspresso-1.0.2/imgs/common/logo-transparent.png
--rw-rw-rw-   0        0        0    13368 2023-06-19 07:37:38.000000 netspresso-1.0.2/imgs/common/twitter.png
--rw-rw-rw-   0        0        0    19185 2023-06-19 07:37:38.000000 netspresso-1.0.2/imgs/common/twitter_white.png
--rw-rw-rw-   0        0        0     7051 2023-06-19 07:37:38.000000 netspresso-1.0.2/imgs/common/youtube.png
--rw-rw-rw-   0        0        0    12219 2023-06-19 07:37:38.000000 netspresso-1.0.2/imgs/common/youtube_white.png
-drwxrwxrwx   0        0        0        0 2023-06-19 08:19:59.956910 netspresso-1.0.2/netspresso/
--rw-rw-rw-   0        0        0       23 2023-06-19 07:53:15.000000 netspresso-1.0.2/netspresso/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:19:59.972869 netspresso-1.0.2/netspresso/__pycache__/
--rw-rw-rw-   0        0        0      178 2023-06-14 07:33:49.000000 netspresso-1.0.2/netspresso/__pycache__/__init__.cpython-38.pyc
-drwxrwxrwx   0        0        0        0 2023-06-19 08:19:59.974864 netspresso-1.0.2/netspresso/compressor/
--rw-rw-rw-   0        0        0    23619 2023-06-13 07:57:24.000000 netspresso-1.0.2/netspresso/compressor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:19:59.976859 netspresso-1.0.2/netspresso/compressor/__pycache__/
--rw-rw-rw-   0        0        0    19045 2023-06-13 08:58:47.000000 netspresso-1.0.2/netspresso/compressor/__pycache__/__init__.cpython-38.pyc
-drwxrwxrwx   0        0        0        0 2023-06-19 08:19:59.981846 netspresso-1.0.2/netspresso/compressor/client/
--rw-rw-rw-   0        0        0     8479 2023-06-19 05:43:13.000000 netspresso-1.0.2/netspresso/compressor/client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:19:59.986832 netspresso-1.0.2/netspresso/compressor/client/__pycache__/
--rw-rw-rw-   0        0        0     7679 2023-06-16 06:25:23.000000 netspresso-1.0.2/netspresso/compressor/client/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0      876 2023-06-16 05:07:28.000000 netspresso-1.0.2/netspresso/compressor/client/__pycache__/config.cpython-38.pyc
--rw-rw-rw-   0        0        0      536 2023-06-16 05:06:54.000000 netspresso-1.0.2/netspresso/compressor/client/config.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:19:59.990822 netspresso-1.0.2/netspresso/compressor/client/configs/
--rw-rw-rw-   0        0        0       41 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/client/configs/config-local.ini
--rw-rw-rw-   0        0        0       61 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/client/configs/config-prod.ini
-drwxrwxrwx   0        0        0        0 2023-06-19 08:20:00.001792 netspresso-1.0.2/netspresso/compressor/client/schemas/
--rw-rw-rw-   0        0        0        0 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/client/schemas/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:20:00.022765 netspresso-1.0.2/netspresso/compressor/client/schemas/__pycache__/
--rw-rw-rw-   0        0        0      183 2023-06-13 06:22:33.000000 netspresso-1.0.2/netspresso/compressor/client/schemas/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     2612 2023-06-13 06:22:33.000000 netspresso-1.0.2/netspresso/compressor/client/schemas/__pycache__/auth.cpython-38.pyc
--rw-rw-rw-   0        0        0      602 2023-06-13 06:22:33.000000 netspresso-1.0.2/netspresso/compressor/client/schemas/__pycache__/common.cpython-38.pyc
--rw-rw-rw-   0        0        0     5153 2023-06-13 06:22:33.000000 netspresso-1.0.2/netspresso/compressor/client/schemas/__pycache__/compression.cpython-38.pyc
--rw-rw-rw-   0        0        0     5771 2023-06-13 06:22:33.000000 netspresso-1.0.2/netspresso/compressor/client/schemas/__pycache__/model.cpython-38.pyc
--rw-rw-rw-   0        0        0     2644 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/client/schemas/auth.py
--rw-rw-rw-   0        0        0      482 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/client/schemas/common.py
--rw-rw-rw-   0        0        0     4108 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/client/schemas/compression.py
--rw-rw-rw-   0        0        0     5681 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/client/schemas/model.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:20:00.039691 netspresso-1.0.2/netspresso/compressor/client/utils/
--rw-rw-rw-   0        0        0        0 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/client/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:20:00.059639 netspresso-1.0.2/netspresso/compressor/client/utils/__pycache__/
--rw-rw-rw-   0        0        0      181 2023-06-13 06:22:33.000000 netspresso-1.0.2/netspresso/compressor/client/utils/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     1840 2023-06-16 07:49:17.000000 netspresso-1.0.2/netspresso/compressor/client/utils/__pycache__/common.cpython-38.pyc
--rw-rw-rw-   0        0        0     1543 2023-06-13 06:22:33.000000 netspresso-1.0.2/netspresso/compressor/client/utils/__pycache__/enum.cpython-38.pyc
--rw-rw-rw-   0        0        0     3780 2023-06-13 06:22:33.000000 netspresso-1.0.2/netspresso/compressor/client/utils/__pycache__/validator.cpython-38.pyc
--rw-rw-rw-   0        0        0      597 2023-06-19 05:43:13.000000 netspresso-1.0.2/netspresso/compressor/client/utils/common.py
--rw-rw-rw-   0        0        0      840 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/client/utils/enum.py
--rw-rw-rw-   0        0        0      997 2023-06-19 05:43:13.000000 netspresso-1.0.2/netspresso/compressor/client/utils/system.py
--rw-rw-rw-   0        0        0     3814 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/client/utils/validator.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:20:00.067618 netspresso-1.0.2/netspresso/compressor/core/
--rw-rw-rw-   0        0        0        0 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:20:00.077589 netspresso-1.0.2/netspresso/compressor/core/__pycache__/
--rw-rw-rw-   0        0        0      173 2023-06-13 06:22:33.000000 netspresso-1.0.2/netspresso/compressor/core/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     2332 2023-06-13 06:22:33.000000 netspresso-1.0.2/netspresso/compressor/core/__pycache__/compression.cpython-38.pyc
--rw-rw-rw-   0        0        0     3580 2023-06-13 06:22:33.000000 netspresso-1.0.2/netspresso/compressor/core/__pycache__/model.cpython-38.pyc
--rw-rw-rw-   0        0        0     1900 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/core/compression.py
--rw-rw-rw-   0        0        0     2966 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/core/model.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:20:00.086567 netspresso-1.0.2/netspresso/compressor/utils/
--rw-rw-rw-   0        0        0        0 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:20:00.093547 netspresso-1.0.2/netspresso/compressor/utils/__pycache__/
--rw-rw-rw-   0        0        0      174 2023-06-13 06:22:33.000000 netspresso-1.0.2/netspresso/compressor/utils/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     1400 2023-06-13 06:22:33.000000 netspresso-1.0.2/netspresso/compressor/utils/__pycache__/model.cpython-38.pyc
--rw-rw-rw-   0        0        0      477 2023-06-13 06:22:33.000000 netspresso-1.0.2/netspresso/compressor/utils/__pycache__/token.cpython-38.pyc
--rw-rw-rw-   0        0        0     2035 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/utils/model.py
--rw-rw-rw-   0        0        0      236 2023-06-13 06:13:37.000000 netspresso-1.0.2/netspresso/compressor/utils/token.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:19:59.970875 netspresso-1.0.2/netspresso.egg-info/
--rw-rw-rw-   0        0        0     6997 2023-06-19 08:19:59.000000 netspresso-1.0.2/netspresso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2743 2023-06-19 08:19:59.000000 netspresso-1.0.2/netspresso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 08:19:59.000000 netspresso-1.0.2/netspresso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-06-19 08:19:59.000000 netspresso-1.0.2/netspresso.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 08:19:59.000000 netspresso-1.0.2/netspresso.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      145 2023-06-13 08:34:11.000000 netspresso-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 08:20:00.098533 netspresso-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1165 2023-06-19 07:48:57.000000 netspresso-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:42:26.677549 netspresso-1.0.3/
+-rw-rw-rw-   0        0        0    11558 2023-06-12 20:26:38.000000 netspresso-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     6253 2023-06-19 09:42:26.676550 netspresso-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5802 2023-06-19 09:35:55.000000 netspresso-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 09:42:26.604743 netspresso-1.0.3/netspresso/
+-rw-rw-rw-   0        0        0       23 2023-06-19 09:36:48.000000 netspresso-1.0.3/netspresso/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:42:26.622696 netspresso-1.0.3/netspresso/compressor/
+-rw-rw-rw-   0        0        0    23619 2023-06-13 07:57:24.000000 netspresso-1.0.3/netspresso/compressor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:42:26.628678 netspresso-1.0.3/netspresso/compressor/client/
+-rw-rw-rw-   0        0        0     8479 2023-06-19 05:43:13.000000 netspresso-1.0.3/netspresso/compressor/client/__init__.py
+-rw-rw-rw-   0        0        0      536 2023-06-16 05:06:54.000000 netspresso-1.0.3/netspresso/compressor/client/config.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:42:26.633666 netspresso-1.0.3/netspresso/compressor/client/configs/
+-rw-rw-rw-   0        0        0       41 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/client/configs/config-local.ini
+-rw-rw-rw-   0        0        0       61 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/client/configs/config-prod.ini
+drwxrwxrwx   0        0        0        0 2023-06-19 09:42:26.646631 netspresso-1.0.3/netspresso/compressor/client/schemas/
+-rw-rw-rw-   0        0        0        0 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/client/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2644 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/client/schemas/auth.py
+-rw-rw-rw-   0        0        0      482 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/client/schemas/common.py
+-rw-rw-rw-   0        0        0     4108 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/client/schemas/compression.py
+-rw-rw-rw-   0        0        0     5681 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/client/schemas/model.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:42:26.659597 netspresso-1.0.3/netspresso/compressor/client/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/client/utils/__init__.py
+-rw-rw-rw-   0        0        0      597 2023-06-19 05:43:13.000000 netspresso-1.0.3/netspresso/compressor/client/utils/common.py
+-rw-rw-rw-   0        0        0      840 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/client/utils/enum.py
+-rw-rw-rw-   0        0        0      997 2023-06-19 05:43:13.000000 netspresso-1.0.3/netspresso/compressor/client/utils/system.py
+-rw-rw-rw-   0        0        0     3814 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/client/utils/validator.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:42:26.666602 netspresso-1.0.3/netspresso/compressor/core/
+-rw-rw-rw-   0        0        0        0 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/core/__init__.py
+-rw-rw-rw-   0        0        0     1900 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/core/compression.py
+-rw-rw-rw-   0        0        0     2966 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/core/model.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:42:26.673559 netspresso-1.0.3/netspresso/compressor/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/utils/__init__.py
+-rw-rw-rw-   0        0        0     2035 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/utils/model.py
+-rw-rw-rw-   0        0        0      236 2023-06-13 06:13:37.000000 netspresso-1.0.3/netspresso/compressor/utils/token.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:42:26.619702 netspresso-1.0.3/netspresso.egg-info/
+-rw-rw-rw-   0        0        0     6253 2023-06-19 09:42:26.000000 netspresso-1.0.3/netspresso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1137 2023-06-19 09:42:26.000000 netspresso-1.0.3/netspresso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:42:26.000000 netspresso-1.0.3/netspresso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-06-19 09:42:26.000000 netspresso-1.0.3/netspresso.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 09:42:26.000000 netspresso-1.0.3/netspresso.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 09:42:26.677549 netspresso-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2023-06-19 07:48:57.000000 netspresso-1.0.3/setup.py
```

### Comparing `netspresso-1.0.2/LICENSE` & `netspresso-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netspresso-1.0.2/README.md` & `netspresso-1.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,51 @@
+Metadata-Version: 2.1
+Name: netspresso
+Version: 1.0.3
+Summary: NetsPresso Python Package
+Home-page: https://github.com/Nota-NetsPresso/netspresso-python
+Author: NetsPresso
+Author-email: bmlee@nota.ai
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align=right>
   <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FNota-NetsPresso%2Fnetspresso-python&count_bg=%2323E7E7E7&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
 </div>
 
 # NetsPresso Python Package
 
 <div align="center">
-    <img src="imgs/banner/pynp_main.png"/>
+    <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/banner/pynp_main.png"/>
 </div>
 </br>
 
 <div align="center">
-    <a href="https://github.com/Nota-NetsPresso" style="text-decoration:none;">
-        <picture>
-            <source media="(prefers-color-scheme: dark)" srcset="imgs/common/github_white.png">
-            <source media="(prefers-color-scheme: light)" srcset="imgs/common/github.png">
-            <img alt="github" src="imgs/common/github.png" width="3%">
-        </picture>
+    <a href="https://github.com/Nota-NetsPresso">
+        <img alt="github" src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/github.png" width="3%">
     </a>
-    <img src="imgs/common/logo-transparent.png" width="3%" alt="" />
-    <a href="https://www.facebook.com/NotaAI" style="text-decoration:none;">
-        <picture>
-            <source media="(prefers-color-scheme: dark)" srcset="imgs/common/facebook_white.png">
-            <source media="(prefers-color-scheme: light)" srcset="imgs/common/facebook.png">
-            <img alt="facebook" src="imgs/common/facebook.png" width="3%">
-        </picture>
+    <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/logo-transparent.png" width="3%"/>
+    <a href="https://www.facebook.com/NotaAI">
+        <img alt="facebook" src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/facebook.png" width="3%">
     </a>
-    <img src="imgs/common/logo-transparent.png" width="3%" alt="" />
-    <a href="https://twitter.com/nota_ai" style="text-decoration:none;">
-        <picture>
-            <source media="(prefers-color-scheme: dark)" srcset="imgs/common/twitter_white.png">
-            <source media="(prefers-color-scheme: light)" srcset="imgs/common/twitter.png">
-            <img alt="twitter" src="imgs/common/twitter.png" width="3%">
-        </picture>
+    <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/logo-transparent.png" width="3%"/>
+    <a href="https://twitter.com/nota_ai">
+        <img alt="twitter" src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/twitter.png" width="3%">
     </a>
-    <img src="imgs/common/logo-transparent.png" width="3%" alt="" />
-    <a href="https://www.youtube.com/channel/UCeewYFAqb2EqwEXZCfH9DVQ" style="text-decoration:none;">
-        <picture>
-            <source media="(prefers-color-scheme: dark)" srcset="imgs/common/youtube_white.png">
-            <source media="(prefers-color-scheme: light)" srcset="imgs/common/youtube.png">
-            <img alt="youtube" src="imgs/common/youtube.png" width="3%">
-        </picture>
+    <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/logo-transparent.png" width="3%"/>
+    <a href="https://www.youtube.com/channel/UCeewYFAqb2EqwEXZCfH9DVQ">
+        <img alt="youtube" src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/youtube.png" width="3%">
     </a>
-    <img src="imgs/common/logo-transparent.png" width="3%" alt="" />
-    <a href="https://www.linkedin.com/company/nota-incorporated" style="text-decoration:none;">
-        <picture>
-            <source media="(prefers-color-scheme: dark)" srcset="imgs/common/linkedin_white.png">
-            <source media="(prefers-color-scheme: light)" srcset="imgs/common/linkedin.png">
-            <img alt="youtube" src="imgs/common/linkedin.png" width="3%">
-        </picture>
+    <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/logo-transparent.png" width="3%"/>
+    <a href="https://www.linkedin.com/company/nota-incorporated">
+        <img alt="youtube" src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/linkedin.png" width="3%">
     </a>
 </div>
 </br>
 
 <div align="center">
     <p align="center">
         <a href="https://www.python.org/downloads/" target="_blank"><img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue" />
```

#### html2text {}

```diff
@@ -1,13 +1,25 @@
+Metadata-Version: 2.1 Name: netspresso Version: 1.0.3 Summary: NetsPresso
+Python Package Home-page: https://github.com/Nota-NetsPresso/netspresso-python
+Author: NetsPresso Author-email: bmlee@nota.ai Classifier: Programming Language
+:: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
+Content-Type: text/markdown License-File: LICENSE
                                    [https://hits.seeyoufarm.com/api/count/incr/
          badge.svg?url=https%3A%2F%2Fgithub.com%2FNota-NetsPresso%2Fnetspresso-
 python&count_bg=%2323E7E7E7&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false]
 # NetsPresso Python Package
-                          [imgs/banner/pynp_main.png]
-   ___[github]_  ___[facebook]_  ___[twitter]_  ___[youtube]_  ___[youtube]_
+  [https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/banner/
+                                pynp_main.png]
+ [github] [https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/
+ common/logo-transparent.png] [facebook] [https://netspresso-docs-imgs.s3.ap-
+northeast-2.amazonaws.com/imgs/common/logo-transparent.png] [twitter] [https://
+    netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/logo-
+   transparent.png] [youtube] [https://netspresso-docs-imgs.s3.ap-northeast-
+          2.amazonaws.com/imgs/common/logo-transparent.png] [youtube]
 [https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue]_[https:
                //img.shields.io/badge/TensorFlow-2.3.x_~_2.5.x.-
        FF6F00?style=flat&logo=tensorflow&logoColor=#FF6F00&link=https://
 www.tensorflow.org/install/pip]_[https://img.shields.io/badge/PyTorch-1.11.x_~
            1.13.x.-EE4C2C?style=flat&logo=pytorch&logoColor=#EE4C2C]
  Use **PyNetsPresso** for a seamless model optimization process. PyNetsPresso
 resolves AI-related constraints in business use cases and enables cost-
```

### Comparing `netspresso-1.0.2/netspresso/compressor/__init__.py` & `netspresso-1.0.3/netspresso/compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.0.2/netspresso/compressor/client/__init__.py` & `netspresso-1.0.3/netspresso/compressor/client/__init__.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.0.2/netspresso/compressor/client/config.py` & `netspresso-1.0.3/netspresso/compressor/client/config.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.0.2/netspresso/compressor/client/schemas/auth.py` & `netspresso-1.0.3/netspresso/compressor/client/schemas/auth.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.0.2/netspresso/compressor/client/schemas/compression.py` & `netspresso-1.0.3/netspresso/compressor/client/schemas/compression.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.0.2/netspresso/compressor/client/schemas/model.py` & `netspresso-1.0.3/netspresso/compressor/client/schemas/model.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.0.2/netspresso/compressor/client/utils/common.py` & `netspresso-1.0.3/netspresso/compressor/client/utils/common.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.0.2/netspresso/compressor/client/utils/enum.py` & `netspresso-1.0.3/netspresso/compressor/client/utils/enum.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.0.2/netspresso/compressor/client/utils/system.py` & `netspresso-1.0.3/netspresso/compressor/client/utils/system.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.0.2/netspresso/compressor/client/utils/validator.py` & `netspresso-1.0.3/netspresso/compressor/client/utils/validator.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.0.2/netspresso/compressor/core/compression.py` & `netspresso-1.0.3/netspresso/compressor/core/compression.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.0.2/netspresso/compressor/core/model.py` & `netspresso-1.0.3/netspresso/compressor/core/model.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.0.2/netspresso/compressor/utils/model.py` & `netspresso-1.0.3/netspresso/compressor/utils/model.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.0.2/setup.py` & `netspresso-1.0.3/setup.py`

 * *Files identical despite different names*

