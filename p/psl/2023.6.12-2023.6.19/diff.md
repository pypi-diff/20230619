# Comparing `tmp/psl-2023.6.12.tar.gz` & `tmp/psl-2023.6.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psl-2023.6.12.tar", last modified: Mon Jun 12 13:05:37 2023, max compression
+gzip compressed data, was "psl-2023.6.19.tar", last modified: Mon Jun 19 13:06:30 2023, max compression
```

## Comparing `psl-2023.6.12.tar` & `psl-2023.6.19.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:05:37.263585 psl-2023.6.12/
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-06-12 13:05:02.000000 psl-2023.6.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 13:05:02.000000 psl-2023.6.12/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-12 13:05:37.263585 psl-2023.6.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-12 13:05:02.000000 psl-2023.6.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:05:37.263585 psl-2023.6.12/psl/
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-12 13:05:12.000000 psl-2023.6.12/psl/__init__.py
--rw-------   0 runner    (1001) docker     (123)   109019 2023-06-12 13:05:12.000000 psl-2023.6.12/psl/psl.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:05:02.000000 psl-2023.6.12/psl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:05:37.263585 psl-2023.6.12/psl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-12 13:05:37.000000 psl-2023.6.12/psl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-12 13:05:37.000000 psl-2023.6.12/psl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:05:37.000000 psl-2023.6.12/psl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:05:25.000000 psl-2023.6.12/psl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-12 13:05:37.000000 psl-2023.6.12/psl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:05:37.263585 psl-2023.6.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-12 13:05:02.000000 psl-2023.6.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:06:30.439833 psl-2023.6.19/
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-06-19 13:05:57.000000 psl-2023.6.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-19 13:05:57.000000 psl-2023.6.19/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-19 13:06:30.439833 psl-2023.6.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-19 13:05:57.000000 psl-2023.6.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:06:30.439833 psl-2023.6.19/psl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-19 13:06:05.000000 psl-2023.6.19/psl/__init__.py
+-rw-------   0 runner    (1001) docker     (123)   109723 2023-06-19 13:06:05.000000 psl-2023.6.19/psl/psl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:05:57.000000 psl-2023.6.19/psl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:06:30.439833 psl-2023.6.19/psl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-19 13:06:30.000000 psl-2023.6.19/psl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-19 13:06:30.000000 psl-2023.6.19/psl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:06:30.000000 psl-2023.6.19/psl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:06:18.000000 psl-2023.6.19/psl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-19 13:06:30.000000 psl-2023.6.19/psl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 13:06:30.439833 psl-2023.6.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-19 13:05:57.000000 psl-2023.6.19/setup.py
```

### Comparing `psl-2023.6.12/LICENSE` & `psl-2023.6.19/LICENSE`

 * *Files identical despite different names*

### Comparing `psl-2023.6.12/PKG-INFO` & `psl-2023.6.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.6.12
+Version: 2023.6.19
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.6.12/README.md` & `psl-2023.6.19/README.md`

 * *Files identical despite different names*

### Comparing `psl-2023.6.12/psl/__init__.py` & `psl-2023.6.19/psl/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import pathlib
 import typing
 
-__version__ = "2023.6.12"
-__checksum__ = "5c35aaf6e7583a27a11d266425d198d0d92ddca6"
+__version__ = "2023.6.19"
+__checksum__ = "e59b87a5d8e71edb2dee3d57fc35c9a6a5fb3806"
 __all__ = ["PUBLIC_SUFFIX_URL", "domain_suffixes", "Suffixes", "domain_can_set_cookie"]
 
 
 PUBLIC_SUFFIX_URL = "https://publicsuffix.org/list/public_suffix_list.dat"
 _PUBLIC_SUFFIX_PATH = pathlib.Path(__file__).parent / "psl.txt"
```

### Comparing `psl-2023.6.12/psl/psl.txt` & `psl-2023.6.19/psl/psl.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5533,26 +5533,92 @@
 vi
 co.vi
 com.vi
 k12.vi
 net.vi
 org.vi
 vn
+ac.vn
+ai.vn
+biz.vn
 com.vn
-net.vn
-org.vn
 edu.vn
 gov.vn
-int.vn
-ac.vn
-biz.vn
+health.vn
+id.vn
 info.vn
+int.vn
+io.vn
 name.vn
+net.vn
+org.vn
 pro.vn
-health.vn
+angiang.vn
+bacgiang.vn
+backan.vn
+baclieu.vn
+bacninh.vn
+baria-vungtau.vn
+bentre.vn
+binhdinh.vn
+binhduong.vn
+binhphuoc.vn
+binhthuan.vn
+camau.vn
+cantho.vn
+caobang.vn
+daklak.vn
+daknong.vn
+danang.vn
+dienbien.vn
+dongnai.vn
+dongthap.vn
+gialai.vn
+hagiang.vn
+haiduong.vn
+haiphong.vn
+hanam.vn
+hanoi.vn
+hatinh.vn
+haugiang.vn
+hoabinh.vn
+hungyen.vn
+khanhhoa.vn
+kiengiang.vn
+kontum.vn
+laichau.vn
+lamdong.vn
+langson.vn
+laocai.vn
+longan.vn
+namdinh.vn
+nghean.vn
+ninhbinh.vn
+ninhthuan.vn
+phutho.vn
+phuyen.vn
+quangbinh.vn
+quangnam.vn
+quangngai.vn
+quangninh.vn
+quangtri.vn
+soctrang.vn
+sonla.vn
+tayninh.vn
+thaibinh.vn
+thainguyen.vn
+thanhhoa.vn
+thanhphohochiminh.vn
+thuathienhue.vn
+tiengiang.vn
+travinh.vn
+tuyenquang.vn
+vinhlong.vn
+vinhphuc.vn
+yenbai.vn
 vu
 com.vu
 edu.vu
 net.vu
 org.vu
 wf
 ws
@@ -5912,15 +5978,14 @@
 comsec
 condos
 construction
 consulting
 contact
 contractors
 cooking
-cookingchannel
 cool
 corsica
 country
 coupon
 coupons
 courses
 cpa
@@ -6042,15 +6107,14 @@
 flights
 flir
 florist
 flowers
 fly
 foo
 food
-foodnetwork
 football
 ford
 forex
 forsale
 forum
 foundation
 fox
@@ -6127,15 +6191,14 @@
 hdfcbank
 health
 healthcare
 help
 helsinki
 here
 hermes
-hgtv
 hiphop
 hisamitsu
 hitachi
 hiv
 hkt
 hockey
 holdings
@@ -6640,15 +6703,14 @@
 town
 toyota
 toys
 trade
 trading
 training
 travel
-travelchannel
 travelers
 travelersinsurance
 trust
 trv
 tube
 tui
 tunes
```

### Comparing `psl-2023.6.12/psl.egg-info/PKG-INFO` & `psl-2023.6.19/psl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.6.12
+Version: 2023.6.19
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.6.12/setup.py` & `psl-2023.6.19/setup.py`

 * *Files identical despite different names*

