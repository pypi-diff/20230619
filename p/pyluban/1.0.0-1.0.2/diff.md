# Comparing `tmp/pyluban-1.0.0.tar.gz` & `tmp/pyluban-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyluban-1.0.0.tar", last modified: Sun Jun 18 13:00:09 2023, max compression
+gzip compressed data, was "pyluban-1.0.2.tar", last modified: Mon Jun 19 00:44:06 2023, max compression
```

## Comparing `pyluban-1.0.0.tar` & `pyluban-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:00:09.397592 pyluban-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-06-18 12:59:29.000000 pyluban-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-18 13:00:09.397592 pyluban-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-18 12:59:29.000000 pyluban-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:00:09.393592 pyluban-1.0.0/pyluban.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-18 13:00:09.000000 pyluban-1.0.0/pyluban.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-18 13:00:09.000000 pyluban-1.0.0/pyluban.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:00:09.000000 pyluban-1.0.0/pyluban.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-18 13:00:09.000000 pyluban-1.0.0/pyluban.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-18 13:00:09.000000 pyluban-1.0.0/pyluban.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-18 13:00:09.000000 pyluban-1.0.0/pyluban.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-06-18 12:59:29.000000 pyluban-1.0.0/pyluban.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-18 12:59:29.000000 pyluban-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:00:09.393592 pyluban-1.0.0/script/
--rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-06-18 12:59:29.000000 pyluban-1.0.0/script/luban_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-06-18 12:59:29.000000 pyluban-1.0.0/script/operatordef.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-18 12:59:29.000000 pyluban-1.0.0/script/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 13:00:09.397592 pyluban-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-18 12:59:29.000000 pyluban-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:00:09.397592 pyluban-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-06-18 12:59:29.000000 pyluban-1.0.0/src/MurmurHash3.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-06-18 12:59:29.000000 pyluban-1.0.0/src/base64.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    87039 2023-06-18 12:59:57.000000 pyluban-1.0.0/src/feature.pb.cc
--rw-r--r--   0 runner    (1001) docker     (123)   167132 2023-06-18 12:59:29.000000 pyluban-1.0.0/src/luban_wrap.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-18 12:59:29.000000 pyluban-1.0.0/src/pyluban.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:00:09.397592 pyluban-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-06-18 12:59:29.000000 pyluban-1.0.0/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:44:06.277986 pyluban-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-06-19 00:43:42.000000 pyluban-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-19 00:44:06.277986 pyluban-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-19 00:43:42.000000 pyluban-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:44:06.277986 pyluban-1.0.2/pyluban.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-19 00:44:06.000000 pyluban-1.0.2/pyluban.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-19 00:44:06.000000 pyluban-1.0.2/pyluban.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 00:44:06.000000 pyluban-1.0.2/pyluban.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-19 00:44:06.000000 pyluban-1.0.2/pyluban.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 00:44:06.000000 pyluban-1.0.2/pyluban.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-19 00:44:06.000000 pyluban-1.0.2/pyluban.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-06-19 00:43:42.000000 pyluban-1.0.2/pyluban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-19 00:43:42.000000 pyluban-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:44:06.277986 pyluban-1.0.2/script/
+-rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-06-19 00:43:42.000000 pyluban-1.0.2/script/luban_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-06-19 00:43:42.000000 pyluban-1.0.2/script/operatordef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-19 00:43:42.000000 pyluban-1.0.2/script/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 00:44:06.277986 pyluban-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-19 00:43:42.000000 pyluban-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:44:06.277986 pyluban-1.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-06-19 00:43:42.000000 pyluban-1.0.2/src/MurmurHash3.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-06-19 00:43:42.000000 pyluban-1.0.2/src/base64.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    87039 2023-06-19 00:43:57.000000 pyluban-1.0.2/src/feature.pb.cc
+-rw-r--r--   0 runner    (1001) docker     (123)   167132 2023-06-19 00:43:42.000000 pyluban-1.0.2/src/luban_wrap.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-19 00:43:42.000000 pyluban-1.0.2/src/pyluban.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:44:06.277986 pyluban-1.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-06-19 00:43:42.000000 pyluban-1.0.2/test/test.py
```

### Comparing `pyluban-1.0.0/LICENSE` & `pyluban-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyluban-1.0.0/PKG-INFO` & `pyluban-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyluban
-Version: 1.0.0
+Version: 1.0.2
 Summary: Python wrapper for luban.
 Home-page: https://github.com/uopensail/luban
 Author: uopensail
 Author-email: 
 License: License :: AGLP 3
 Keywords: feature operator and hasher
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # luban
-[中文文档](README_ZN.md)
+[中文文档](https://github.com/uopensail/luban/blob/main/README_ZN.md)
 ## Why Need?
 
 The feature-processing module is used in different scenarios, such as: model training and model inference. Usually, we use Python to train models, and feature-processing is also done in Python. However, in model inference, the shorter the inference run time, the better. So we usually use C++/java/golang or other languages to do model inference.
 
 If feature-process module is written in many different languages, they may be inconsistencies. So, we decide to develop such a module in C++, which can be used by other different languages. In addition, we use a yaml configuration for feature processing, so that it will be easier to use.
 
 ## Supported libraries and tools
@@ -87,66 +87,24 @@
     1. step1: Configure the JSON file
     2. use `luban_parser` to process JSON configuration files and generate configuration files in TOML format
     3. Use the configuration file in TOML format as a configuration input for C/C++/Golang/Python
 
 
 ## Install
 
-### install protobuf 
-The installation script under CentOS 7 is below, other systems is similar.
+### install On MacOS ARM
 
 ```shell
-#!/bin/shell
-
-yum install -y git wget
-yum install -y openssl openssl-devel gcc-c++
-yum install -y snappy snappy-devel autoconf automake libtool
-yum install -y bzip2 bzip2-devel lz4-devel libzstd-devel
-yum install -y epel-release gflags gflags-devel which 
-
-# install cmake
-# use cmake to compile this project for c/c++ lib
-cd /tmp 
-wget https://github.com/Kitware/CMake/releases/download/v3.18.2/cmake-3.18.2.tar.gz
-tar -xvf cmake-3.18.2.tar.gz
-cd cmake-3.18.2
-./bootstrap
-gmake && gmake install
-
-# instal libunwind
-cd /tmp
-wget http://download.savannah.gnu.org/releases/libunwind/libunwind-1.5.0.tar.gz
-tar -xvf libunwind-1.5.0.tar.gz
-cd libunwind-1.5.0
-CFLAGS=-fPIC ./configure
-make CFLAGS=-fPIC && make CFLAGS=-fPIC install 
-
-# install gperftools and tcmalloc
-cd /tmp
-wget https://github.com/gperftools/gperftools/releases/download/gperftools-2.7/gperftools-2.7.tar.gz
-tar -xvf gperftools-2.7.tar.gz 
-cd gperftools-2.7
-./configure
-make -j6 && make install 
-
-# install protobuf
-cd /tmp
-git clone https://github.com/protocolbuffers/protobuf.git
-cd protobuf 
-git checkout v3.8.0 && git submodule update --init --recursive
-./autogen.sh
-./configure 
-make && make install
-ldconfig
-
-rm -rf /tmp/*
+brew install protobuf
+pip install pyluba
 ```
 
-### install pyluban
+### Unix Like
+
 ```shell
-python setup.py install --install-scripts=/usr/local/bin
+pip install pyluba
 ```
 
 ## Q&A
 
 `Fatal Python error: type_traverse() called for non-heap type 'Entity'`
 this is python's bug, please upgrade python to python3.8 or higher
```

### Comparing `pyluban-1.0.0/README.md` & `pyluban-1.0.2/pyluban.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,29 @@
+Metadata-Version: 2.1
+Name: pyluban
+Version: 1.0.2
+Summary: Python wrapper for luban.
+Home-page: https://github.com/uopensail/luban
+Author: uopensail
+Author-email: 
+License: License :: AGLP 3
+Keywords: feature operator and hasher
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # luban
-[中文文档](README_ZN.md)
+[中文文档](https://github.com/uopensail/luban/blob/main/README_ZN.md)
 ## Why Need?
 
 The feature-processing module is used in different scenarios, such as: model training and model inference. Usually, we use Python to train models, and feature-processing is also done in Python. However, in model inference, the shorter the inference run time, the better. So we usually use C++/java/golang or other languages to do model inference.
 
 If feature-process module is written in many different languages, they may be inconsistencies. So, we decide to develop such a module in C++, which can be used by other different languages. In addition, we use a yaml configuration for feature processing, so that it will be easier to use.
 
 ## Supported libraries and tools
@@ -67,66 +87,24 @@
     1. step1: Configure the JSON file
     2. use `luban_parser` to process JSON configuration files and generate configuration files in TOML format
     3. Use the configuration file in TOML format as a configuration input for C/C++/Golang/Python
 
 
 ## Install
 
-### install protobuf 
-The installation script under CentOS 7 is below, other systems is similar.
+### install On MacOS ARM
 
 ```shell
-#!/bin/shell
-
-yum install -y git wget
-yum install -y openssl openssl-devel gcc-c++
-yum install -y snappy snappy-devel autoconf automake libtool
-yum install -y bzip2 bzip2-devel lz4-devel libzstd-devel
-yum install -y epel-release gflags gflags-devel which 
-
-# install cmake
-# use cmake to compile this project for c/c++ lib
-cd /tmp 
-wget https://github.com/Kitware/CMake/releases/download/v3.18.2/cmake-3.18.2.tar.gz
-tar -xvf cmake-3.18.2.tar.gz
-cd cmake-3.18.2
-./bootstrap
-gmake && gmake install
-
-# instal libunwind
-cd /tmp
-wget http://download.savannah.gnu.org/releases/libunwind/libunwind-1.5.0.tar.gz
-tar -xvf libunwind-1.5.0.tar.gz
-cd libunwind-1.5.0
-CFLAGS=-fPIC ./configure
-make CFLAGS=-fPIC && make CFLAGS=-fPIC install 
-
-# install gperftools and tcmalloc
-cd /tmp
-wget https://github.com/gperftools/gperftools/releases/download/gperftools-2.7/gperftools-2.7.tar.gz
-tar -xvf gperftools-2.7.tar.gz 
-cd gperftools-2.7
-./configure
-make -j6 && make install 
-
-# install protobuf
-cd /tmp
-git clone https://github.com/protocolbuffers/protobuf.git
-cd protobuf 
-git checkout v3.8.0 && git submodule update --init --recursive
-./autogen.sh
-./configure 
-make && make install
-ldconfig
-
-rm -rf /tmp/*
+brew install protobuf
+pip install pyluba
 ```
 
-### install pyluban
+### Unix Like
+
 ```shell
-python setup.py install --install-scripts=/usr/local/bin
+pip install pyluba
 ```
 
 ## Q&A
 
 `Fatal Python error: type_traverse() called for non-heap type 'Entity'`
-this is python's bug, please upgrade python to python3.8 or higher
+this is python's bug, please upgrade python to python3.8 or higher
```

### Comparing `pyluban-1.0.0/pyluban.py` & `pyluban-1.0.2/pyluban.py`

 * *Files identical despite different names*

### Comparing `pyluban-1.0.0/pyproject.toml` & `pyluban-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyluban-1.0.0/script/luban_parser.py` & `pyluban-1.0.2/script/luban_parser.py`

 * *Files identical despite different names*

### Comparing `pyluban-1.0.0/script/operatordef.py` & `pyluban-1.0.2/script/operatordef.py`

 * *Files identical despite different names*

### Comparing `pyluban-1.0.0/script/typedef.py` & `pyluban-1.0.2/script/typedef.py`

 * *Files identical despite different names*

### Comparing `pyluban-1.0.0/setup.py` & `pyluban-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     extra_compile_args=COMPILE_OPTIONS,
     extra_link_args=LINK_OPTIONS,
 )
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 setup(
     name="pyluban",
-    version="1.0.0",
+    version="1.0.2",
     description="Python wrapper for luban.",
     license="License :: AGLP 3",
     author="uopensail",
     author_email="",
     url="https://github.com/uopensail/luban",
     packages=find_packages(),
     py_modules=["pyluban"],
```

### Comparing `pyluban-1.0.0/src/MurmurHash3.cc` & `pyluban-1.0.2/src/MurmurHash3.cc`

 * *Files identical despite different names*

### Comparing `pyluban-1.0.0/src/base64.cpp` & `pyluban-1.0.2/src/base64.cpp`

 * *Files identical despite different names*

### Comparing `pyluban-1.0.0/src/feature.pb.cc` & `pyluban-1.0.2/src/feature.pb.cc`

 * *Files identical despite different names*

### Comparing `pyluban-1.0.0/src/luban_wrap.cxx` & `pyluban-1.0.2/src/luban_wrap.cxx`

 * *Files identical despite different names*

### Comparing `pyluban-1.0.0/src/pyluban.cpp` & `pyluban-1.0.2/src/pyluban.cpp`

 * *Files identical despite different names*

### Comparing `pyluban-1.0.0/test/test.py` & `pyluban-1.0.2/test/test.py`

 * *Files identical despite different names*

