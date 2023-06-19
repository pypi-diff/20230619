# Comparing `tmp/sys-call-0.0.1.tar.gz` & `tmp/sys-call-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sys-call-0.0.1.tar", last modified: Mon Jun 19 19:04:13 2023, max compression
+gzip compressed data, was "sys-call-0.0.2.tar", last modified: Mon Jun 19 19:53:35 2023, max compression
```

## Comparing `sys-call-0.0.1.tar` & `sys-call-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lbirch     (501) staff       (20)        0 2023-06-19 19:04:13.572569 sys-call-0.0.1/
--rw-r--r--   0 lbirch     (501) staff       (20)     1074 2023-06-19 17:13:30.000000 sys-call-0.0.1/LICENSE
--rw-r--r--   0 lbirch     (501) staff       (20)    11031 2023-06-19 19:04:13.572307 sys-call-0.0.1/PKG-INFO
--rw-r--r--   0 lbirch     (501) staff       (20)    10583 2023-06-19 19:04:05.000000 sys-call-0.0.1/README.md
--rw-r--r--   0 lbirch     (501) staff       (20)       38 2023-06-19 19:04:13.572611 sys-call-0.0.1/setup.cfg
--rw-r--r--   0 lbirch     (501) staff       (20)     1363 2023-06-19 19:03:47.000000 sys-call-0.0.1/setup.py
-drwxr-xr-x   0 lbirch     (501) staff       (20)        0 2023-06-19 19:04:13.571783 sys-call-0.0.1/sys_call.egg-info/
--rw-r--r--   0 lbirch     (501) staff       (20)    11031 2023-06-19 19:04:13.000000 sys-call-0.0.1/sys_call.egg-info/PKG-INFO
--rw-r--r--   0 lbirch     (501) staff       (20)      259 2023-06-19 19:04:13.000000 sys-call-0.0.1/sys_call.egg-info/SOURCES.txt
--rw-r--r--   0 lbirch     (501) staff       (20)        1 2023-06-19 19:04:13.000000 sys-call-0.0.1/sys_call.egg-info/dependency_links.txt
--rw-r--r--   0 lbirch     (501) staff       (20)      108 2023-06-19 19:04:13.000000 sys-call-0.0.1/sys_call.egg-info/entry_points.txt
--rw-r--r--   0 lbirch     (501) staff       (20)       12 2023-06-19 19:04:13.000000 sys-call-0.0.1/sys_call.egg-info/requires.txt
--rw-r--r--   0 lbirch     (501) staff       (20)        8 2023-06-19 19:04:13.000000 sys-call-0.0.1/sys_call.egg-info/top_level.txt
-drwxr-xr-x   0 lbirch     (501) staff       (20)        0 2023-06-19 19:04:13.571989 sys-call-0.0.1/syscall/
--rw-r--r--   0 lbirch     (501) staff       (20)       22 2023-06-19 19:04:10.000000 sys-call-0.0.1/syscall/__init__.py
--rwxr-xr-x   0 lbirch     (501) staff       (20)     6470 2023-06-19 17:44:18.000000 sys-call-0.0.1/syscall/syscall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:53:35.451347 sys-call-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-19 19:53:20.000000 sys-call-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-06-19 19:53:35.451347 sys-call-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-06-19 19:53:20.000000 sys-call-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 19:53:35.451347 sys-call-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-19 19:53:20.000000 sys-call-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:53:35.451347 sys-call-0.0.2/sys_call.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-06-19 19:53:35.000000 sys-call-0.0.2/sys_call.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-19 19:53:35.000000 sys-call-0.0.2/sys_call.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:53:35.000000 sys-call-0.0.2/sys_call.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-19 19:53:35.000000 sys-call-0.0.2/sys_call.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 19:53:35.000000 sys-call-0.0.2/sys_call.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 19:53:35.000000 sys-call-0.0.2/sys_call.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:53:35.451347 sys-call-0.0.2/syscall/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 19:53:20.000000 sys-call-0.0.2/syscall/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6470 2023-06-19 19:53:20.000000 sys-call-0.0.2/syscall/syscall.py
```

### Comparing `sys-call-0.0.1/LICENSE` & `sys-call-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sys-call-0.0.1/PKG-INFO` & `sys-call-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sys-call
-Version: 0.0.1
+Version: 0.0.2
 Summary: Linux Syscall implementations, calling conventions, and shellcode examples.
-Home-page: http://github.com/lbirchler/syscall/
+Home-page: http://github.com/lbirchler/sys-call/
 Author: Lawrence Birchler
 Author-email: bplyr@tutanota.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# syscall
+# sys-call
 
 CLI tool to display Linux Syscall implementations, calling conventions, and shellcode examples.
 
 Supported architectures: arm, arm64, x64, x86
 
 Data Sources:
 - Syscall implementations and calling conventions: [syscall.sh](https://syscall.sh)
```

### Comparing `sys-call-0.0.1/README.md` & `sys-call-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# syscall
+# sys-call
 
 CLI tool to display Linux Syscall implementations, calling conventions, and shellcode examples.
 
 Supported architectures: arm, arm64, x64, x86
 
 Data Sources:
 - Syscall implementations and calling conventions: [syscall.sh](https://syscall.sh)
```

### Comparing `sys-call-0.0.1/setup.py` & `sys-call-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     version=get_version('syscall/__init__.py'),
     description='Linux Syscall implementations, calling conventions, and shellcode examples.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(include=['syscall', 'syscall.*']),
     author='Lawrence Birchler',
     author_email='bplyr@tutanota.com',
-    url='http://github.com/lbirchler/syscall/',
+    url='http://github.com/lbirchler/sys-call/',
     install_requires=[
       'rich>13.4.0'
     ],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
```

### Comparing `sys-call-0.0.1/sys_call.egg-info/PKG-INFO` & `sys-call-0.0.2/sys_call.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sys-call
-Version: 0.0.1
+Version: 0.0.2
 Summary: Linux Syscall implementations, calling conventions, and shellcode examples.
-Home-page: http://github.com/lbirchler/syscall/
+Home-page: http://github.com/lbirchler/sys-call/
 Author: Lawrence Birchler
 Author-email: bplyr@tutanota.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# syscall
+# sys-call
 
 CLI tool to display Linux Syscall implementations, calling conventions, and shellcode examples.
 
 Supported architectures: arm, arm64, x64, x86
 
 Data Sources:
 - Syscall implementations and calling conventions: [syscall.sh](https://syscall.sh)
```

### Comparing `sys-call-0.0.1/syscall/syscall.py` & `sys-call-0.0.2/syscall/syscall.py`

 * *Files identical despite different names*

