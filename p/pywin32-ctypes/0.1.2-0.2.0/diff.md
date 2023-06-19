# Comparing `tmp/pywin32-ctypes-0.1.2.tar.gz` & `tmp/pywin32-ctypes-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pywin32-ctypes-0.1.2.tar", last modified: Mon Jun 26 08:01:18 2017, max compression
+gzip compressed data, was "dist\pywin32-ctypes-0.2.0.tar", last modified: Fri Aug 17 12:32:42 2018, max compression
```

## Comparing `pywin32-ctypes-0.1.2.tar` & `pywin32-ctypes-0.2.0.tar`

### file list

```diff
@@ -1,60 +1,70 @@
-drwxrwxrwx   0        0        0        0 2017-06-26 08:01:18.000000 pywin32-ctypes-0.1.2/
--rw-rw-rw-   0        0        0     1297 2017-06-26 07:55:38.000000 pywin32-ctypes-0.1.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0       38 2016-03-02 22:21:55.000000 pywin32-ctypes-0.1.2/dev_requirements.txt
--rw-rw-rw-   0        0        0       72 2017-06-23 07:00:18.000000 pywin32-ctypes-0.1.2/doc-requirements.txt
-drwxrwxrwx   0        0        0        0 2017-06-26 08:01:18.000000 pywin32-ctypes-0.1.2/docs/
--rwxrwxrwx   0        0        0     7292 2016-03-02 22:21:55.000000 pywin32-ctypes-0.1.2/docs/make.bat
--rw-rw-rw-   0        0        0     7658 2016-03-02 22:21:55.000000 pywin32-ctypes-0.1.2/docs/Makefile
-drwxrwxrwx   0        0        0        0 2017-06-26 08:01:18.000000 pywin32-ctypes-0.1.2/docs/source/
--rw-rw-rw-   0        0        0    12194 2017-06-23 07:00:18.000000 pywin32-ctypes-0.1.2/docs/source/conf.py
--rw-rw-rw-   0        0        0      367 2016-03-02 22:21:55.000000 pywin32-ctypes-0.1.2/docs/source/index.rst
--rw-rw-rw-   0        0        0     2155 2016-03-02 22:21:55.000000 pywin32-ctypes-0.1.2/docs/source/mock_missing.py
--rw-rw-rw-   0        0        0      412 2016-03-02 22:21:55.000000 pywin32-ctypes-0.1.2/docs/source/pywin32.rst
-drwxrwxrwx   0        0        0        0 2017-06-26 08:01:18.000000 pywin32-ctypes-0.1.2/docs/source/_templates/
--rw-rw-rw-   0        0        0     1016 2016-03-02 22:21:55.000000 pywin32-ctypes-0.1.2/docs/source/_templates/module_template.rst
--rw-rw-rw-   0        0        0     1644 2016-03-02 22:21:55.000000 pywin32-ctypes-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      128 2017-06-23 07:00:18.000000 pywin32-ctypes-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      604 2017-06-26 08:01:18.000000 pywin32-ctypes-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2017-06-26 08:01:18.000000 pywin32-ctypes-0.1.2/pywin32_ctypes.egg-info/
--rw-rw-rw-   0        0        0        1 2017-06-26 08:01:17.000000 pywin32-ctypes-0.1.2/pywin32_ctypes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2017-06-26 08:01:17.000000 pywin32-ctypes-0.1.2/pywin32_ctypes.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      604 2017-06-26 08:01:17.000000 pywin32-ctypes-0.1.2/pywin32_ctypes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1284 2017-06-26 08:01:17.000000 pywin32-ctypes-0.1.2/pywin32_ctypes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2017-06-26 08:01:17.000000 pywin32-ctypes-0.1.2/pywin32_ctypes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1618 2017-06-23 07:00:09.000000 pywin32-ctypes-0.1.2/README.rst
--rw-rw-rw-   0        0        0       42 2017-06-26 08:01:18.000000 pywin32-ctypes-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1005 2017-06-23 07:00:18.000000 pywin32-ctypes-0.1.2/setup.py
--rw-rw-rw-   0        0        0      129 2016-03-02 22:21:55.000000 pywin32-ctypes-0.1.2/tox.ini
--rw-rw-rw-   0        0        0        7 2017-06-26 08:00:10.000000 pywin32-ctypes-0.1.2/VERSION
-drwxrwxrwx   0        0        0        0 2017-06-26 08:01:18.000000 pywin32-ctypes-0.1.2/win32ctypes/
-drwxrwxrwx   0        0        0        0 2017-06-26 08:01:18.000000 pywin32-ctypes-0.1.2/win32ctypes/core/
-drwxrwxrwx   0        0        0        0 2017-06-26 08:01:18.000000 pywin32-ctypes-0.1.2/win32ctypes/core/cffi/
--rw-rw-rw-   0        0        0     4981 2016-03-02 22:21:55.000000 pywin32-ctypes-0.1.2/win32ctypes/core/cffi/_advapi32.py
--rw-rw-rw-   0        0        0      554 2017-05-17 21:05:27.000000 pywin32-ctypes-0.1.2/win32ctypes/core/cffi/_common.py
--rw-rw-rw-   0        0        0     5785 2017-06-23 07:00:18.000000 pywin32-ctypes-0.1.2/win32ctypes/core/cffi/_kernel32.py
--rw-rw-rw-   0        0        0     2466 2017-06-23 07:00:09.000000 pywin32-ctypes-0.1.2/win32ctypes/core/cffi/_util.py
--rw-rw-rw-   0        0        0        0 2016-03-02 22:21:55.000000 pywin32-ctypes-0.1.2/win32ctypes/core/cffi/__init__.py
--rw-rw-rw-   0        0        0      303 2016-03-02 22:21:55.000000 pywin32-ctypes-0.1.2/win32ctypes/core/compat.py
-drwxrwxrwx   0        0        0        0 2017-06-26 08:01:18.000000 pywin32-ctypes-0.1.2/win32ctypes/core/ctypes/
--rw-rw-rw-   0        0        0     3673 2017-06-23 07:00:09.000000 pywin32-ctypes-0.1.2/win32ctypes/core/ctypes/_advapi32.py
--rw-rw-rw-   0        0        0     1298 2017-06-23 07:00:09.000000 pywin32-ctypes-0.1.2/win32ctypes/core/ctypes/_common.py
--rw-rw-rw-   0        0        0     5307 2017-06-23 07:00:09.000000 pywin32-ctypes-0.1.2/win32ctypes/core/ctypes/_kernel32.py
--rw-rw-rw-   0        0        0     1856 2017-06-23 07:00:09.000000 pywin32-ctypes-0.1.2/win32ctypes/core/ctypes/_util.py
--rw-rw-rw-   0        0        0        0 2016-03-02 22:21:55.000000 pywin32-ctypes-0.1.2/win32ctypes/core/ctypes/__init__.py
--rw-rw-rw-   0        0        0      199 2017-05-16 23:23:53.000000 pywin32-ctypes-0.1.2/win32ctypes/core/_winerrors.py
--rw-rw-rw-   0        0        0      528 2017-06-23 07:00:09.000000 pywin32-ctypes-0.1.2/win32ctypes/core/__init__.py
-drwxrwxrwx   0        0        0        0 2017-06-26 08:01:18.000000 pywin32-ctypes-0.1.2/win32ctypes/pywin32/
--rw-rw-rw-   0        0        0      954 2016-03-02 22:21:56.000000 pywin32-ctypes-0.1.2/win32ctypes/pywin32/pywintypes.py
--rw-rw-rw-   0        0        0    10826 2017-06-23 07:00:19.000000 pywin32-ctypes-0.1.2/win32ctypes/pywin32/win32api.py
--rw-rw-rw-   0        0        0     3260 2017-06-23 07:00:19.000000 pywin32-ctypes-0.1.2/win32ctypes/pywin32/win32cred.py
--rw-rw-rw-   0        0        0      396 2017-06-23 07:00:18.000000 pywin32-ctypes-0.1.2/win32ctypes/pywin32/__init__.py
--rw-rw-rw-   0        0        0      342 2017-06-26 07:46:09.000000 pywin32-ctypes-0.1.2/win32ctypes/pywintypes.py
-drwxrwxrwx   0        0        0        0 2017-06-26 08:01:18.000000 pywin32-ctypes-0.1.2/win32ctypes/tests/
--rw-rw-rw-   0        0        0     2545 2017-06-23 07:00:09.000000 pywin32-ctypes-0.1.2/win32ctypes/tests/compat.py
--rw-rw-rw-   0        0        0    11110 2017-06-23 07:00:19.000000 pywin32-ctypes-0.1.2/win32ctypes/tests/test_win32api.py
--rw-rw-rw-   0        0        0     4150 2016-03-02 22:21:56.000000 pywin32-ctypes-0.1.2/win32ctypes/tests/test_win32cred.py
--rw-rw-rw-   0        0        0      172 2016-03-02 22:21:56.000000 pywin32-ctypes-0.1.2/win32ctypes/tests/__init__.py
--rw-rw-rw-   0        0        0       21 2017-06-26 08:01:17.000000 pywin32-ctypes-0.1.2/win32ctypes/version.py
--rw-rw-rw-   0        0        0      338 2017-06-26 07:46:09.000000 pywin32-ctypes-0.1.2/win32ctypes/win32api.py
--rw-rw-rw-   0        0        0      340 2017-06-26 07:46:09.000000 pywin32-ctypes-0.1.2/win32ctypes/win32cred.py
--rw-rw-rw-   0        0        0      214 2017-06-23 07:00:18.000000 pywin32-ctypes-0.1.2/win32ctypes/__init__.py
+drwxrwxrwx   0        0        0        0 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/
+-rw-rw-rw-   0        0        0        3 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/appveyor-cache.txt
+-rw-rw-rw-   0        0        0      157 2018-08-17 11:01:58.000000 pywin32-ctypes-0.2.0/build-requirements.txt
+-rw-rw-rw-   0        0        0     1620 2018-08-17 12:29:22.000000 pywin32-ctypes-0.2.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0       72 2017-05-25 14:06:51.000000 pywin32-ctypes-0.2.0/doc-requirements.txt
+drwxrwxrwx   0        0        0        0 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/docs/
+-rwxrwxrwx   0        0        0     7292 2016-05-09 19:25:26.000000 pywin32-ctypes-0.2.0/docs/make.bat
+-rw-rw-rw-   0        0        0     7658 2016-05-09 19:25:26.000000 pywin32-ctypes-0.2.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/docs/source/
+-rw-rw-rw-   0        0        0    12194 2017-05-25 14:06:51.000000 pywin32-ctypes-0.2.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0      367 2017-05-26 09:15:47.000000 pywin32-ctypes-0.2.0/docs/source/index.rst
+-rw-rw-rw-   0        0        0     2155 2017-05-12 17:46:14.000000 pywin32-ctypes-0.2.0/docs/source/mock_missing.py
+-rw-rw-rw-   0        0        0      554 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/docs/source/pywin32.rst
+drwxrwxrwx   0        0        0        0 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/docs/source/_templates/
+-rw-rw-rw-   0        0        0     1016 2016-05-09 19:25:26.000000 pywin32-ctypes-0.2.0/docs/source/_templates/module_template.rst
+-rw-rw-rw-   0        0        0     1644 2015-03-12 23:02:48.000000 pywin32-ctypes-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      128 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      690 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/pywin32_ctypes.egg-info/
+-rw-rw-rw-   0        0        0        1 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/pywin32_ctypes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/pywin32_ctypes.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      690 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/pywin32_ctypes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1643 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/pywin32_ctypes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/pywin32_ctypes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1450 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/README.rst
+-rw-rw-rw-   0        0        0      116 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2018-08-17 12:29:22.000000 pywin32-ctypes-0.2.0/setup.py
+-rw-rw-rw-   0        0        0      193 2018-08-17 11:01:58.000000 pywin32-ctypes-0.2.0/test-requirements.txt
+-rw-rw-rw-   0        0        0      571 2018-08-17 11:02:42.000000 pywin32-ctypes-0.2.0/tox.ini
+-rw-rw-rw-   0        0        0        7 2018-08-17 12:31:33.000000 pywin32-ctypes-0.2.0/VERSION
+drwxrwxrwx   0        0        0        0 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/win32ctypes/
+drwxrwxrwx   0        0        0        0 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/win32ctypes/core/
+drwxrwxrwx   0        0        0        0 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/win32ctypes/core/cffi/
+-rw-rw-rw-   0        0        0     4964 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/cffi/_authentication.py
+-rw-rw-rw-   0        0        0      554 2015-12-10 20:00:58.000000 pywin32-ctypes-0.2.0/win32ctypes/core/cffi/_common.py
+-rw-rw-rw-   0        0        0      866 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/cffi/_dll.py
+-rw-rw-rw-   0        0        0      355 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/cffi/_nl_support.py
+-rw-rw-rw-   0        0        0     4584 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/cffi/_resource.py
+-rw-rw-rw-   0        0        0      882 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/cffi/_system_information.py
+-rw-rw-rw-   0        0        0      374 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/cffi/_time.py
+-rw-rw-rw-   0        0        0     2723 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/cffi/_util.py
+-rw-rw-rw-   0        0        0        0 2015-11-26 00:32:10.000000 pywin32-ctypes-0.2.0/win32ctypes/core/cffi/__init__.py
+-rw-rw-rw-   0        0        0      560 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/compat.py
+drwxrwxrwx   0        0        0        0 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/win32ctypes/core/ctypes/
+-rw-rw-rw-   0        0        0     3627 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/ctypes/_authentication.py
+-rw-rw-rw-   0        0        0     1502 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/ctypes/_common.py
+-rw-rw-rw-   0        0        0      594 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/ctypes/_dll.py
+-rw-rw-rw-   0        0        0      357 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/ctypes/_nl_support.py
+-rw-rw-rw-   0        0        0     4252 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/ctypes/_resource.py
+-rw-rw-rw-   0        0        0      983 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/ctypes/_system_information.py
+-rw-rw-rw-   0        0        0      384 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/ctypes/_time.py
+-rw-rw-rw-   0        0        0     2049 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/ctypes/_util.py
+-rw-rw-rw-   0        0        0        0 2015-03-12 23:02:48.000000 pywin32-ctypes-0.2.0/win32ctypes/core/ctypes/__init__.py
+-rw-rw-rw-   0        0        0      199 2015-03-12 23:02:48.000000 pywin32-ctypes-0.2.0/win32ctypes/core/_winerrors.py
+-rw-rw-rw-   0        0        0     1864 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/core/__init__.py
+drwxrwxrwx   0        0        0        0 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/win32ctypes/pywin32/
+-rw-rw-rw-   0        0        0      954 2016-05-09 19:25:26.000000 pywin32-ctypes-0.2.0/win32ctypes/pywin32/pywintypes.py
+-rw-rw-rw-   0        0        0     7768 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/pywin32/win32api.py
+-rw-rw-rw-   0        0        0     2850 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/pywin32/win32cred.py
+-rw-rw-rw-   0        0        0      396 2017-05-25 14:06:51.000000 pywin32-ctypes-0.2.0/win32ctypes/pywin32/__init__.py
+-rw-rw-rw-   0        0        0      342 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/pywintypes.py
+drwxrwxrwx   0        0        0        0 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/win32ctypes/tests/
+-rw-rw-rw-   0        0        0     2545 2017-05-23 16:50:49.000000 pywin32-ctypes-0.2.0/win32ctypes/tests/compat.py
+-rw-rw-rw-   0        0        0    11110 2017-05-25 14:06:51.000000 pywin32-ctypes-0.2.0/win32ctypes/tests/test_win32api.py
+-rw-rw-rw-   0        0        0     5710 2018-08-17 11:01:58.000000 pywin32-ctypes-0.2.0/win32ctypes/tests/test_win32cred.py
+-rw-rw-rw-   0        0        0      612 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/tests/__init__.py
+-rw-rw-rw-   0        0        0       21 2018-08-17 12:32:42.000000 pywin32-ctypes-0.2.0/win32ctypes/version.py
+-rw-rw-rw-   0        0        0      338 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/win32api.py
+-rw-rw-rw-   0        0        0      340 2018-08-10 08:40:54.000000 pywin32-ctypes-0.2.0/win32ctypes/win32cred.py
+-rw-rw-rw-   0        0        0      214 2017-05-25 14:06:51.000000 pywin32-ctypes-0.2.0/win32ctypes/__init__.py
```

### Comparing `pywin32-ctypes-0.1.2/CHANGELOG.txt` & `pywin32-ctypes-0.2.0/CHANGELOG.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Change Log
 ==========
 
+Version 0.2.0
+-------------
+
+- Fix syntax error when installing in python 3.7 (#81).
+- Support testing on python 3.7 (#82).
+- Support testing on python 3.3 and python 3.4 (#77).
+- Do not use 2to3 (#75).
+- Support lazy wrapping of win32 functions (#67).
+- Add CRED_PERSIST constants (#79 contributed by @tivnet).
+
 Version 0.1.2
 -------------
 
 (bugfix release)
 
 - Fix implementation for the deprecated api (#64).
```

### Comparing `pywin32-ctypes-0.1.2/docs/make.bat` & `pywin32-ctypes-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pywin32-ctypes-0.1.2/docs/Makefile` & `pywin32-ctypes-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pywin32-ctypes-0.1.2/docs/source/conf.py` & `pywin32-ctypes-0.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pywin32-ctypes-0.1.2/docs/source/mock_missing.py` & `pywin32-ctypes-0.2.0/docs/source/mock_missing.py`

 * *Files identical despite different names*

### Comparing `pywin32-ctypes-0.1.2/docs/source/_templates/module_template.rst` & `pywin32-ctypes-0.2.0/docs/source/_templates/module_template.rst`

 * *Files identical despite different names*

### Comparing `pywin32-ctypes-0.1.2/LICENSE.txt` & `pywin32-ctypes-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pywin32-ctypes-0.1.2/PKG-INFO` & `pywin32-ctypes-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 1.1
 Name: pywin32-ctypes
-Version: 0.1.2
+Version: 0.2.0
 Summary: UNKNOWN
 Home-page: https://github.com/enthought/pywin32-ctypes
 Author: Enthought Inc
 Author-email: info@enthought.com
 License: BSD
+Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pywin32-ctypes-0.1.2/pywin32_ctypes.egg-info/PKG-INFO` & `pywin32-ctypes-0.2.0/pywin32_ctypes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 1.1
 Name: pywin32-ctypes
-Version: 0.1.2
+Version: 0.2.0
 Summary: UNKNOWN
 Home-page: https://github.com/enthought/pywin32-ctypes
 Author: Enthought Inc
 Author-email: info@enthought.com
 License: BSD
+Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pywin32-ctypes-0.1.2/pywin32_ctypes.egg-info/SOURCES.txt` & `pywin32-ctypes-0.2.0/pywin32_ctypes.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 CHANGELOG.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
 VERSION
-dev_requirements.txt
+appveyor-cache.txt
+build-requirements.txt
 doc-requirements.txt
+setup.cfg
 setup.py
+test-requirements.txt
 tox.ini
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 docs/source/index.rst
 docs/source/mock_missing.py
 docs/source/pywin32.rst
@@ -24,22 +27,30 @@
 win32ctypes/version.py
 win32ctypes/win32api.py
 win32ctypes/win32cred.py
 win32ctypes/core/__init__.py
 win32ctypes/core/_winerrors.py
 win32ctypes/core/compat.py
 win32ctypes/core/cffi/__init__.py
-win32ctypes/core/cffi/_advapi32.py
+win32ctypes/core/cffi/_authentication.py
 win32ctypes/core/cffi/_common.py
-win32ctypes/core/cffi/_kernel32.py
+win32ctypes/core/cffi/_dll.py
+win32ctypes/core/cffi/_nl_support.py
+win32ctypes/core/cffi/_resource.py
+win32ctypes/core/cffi/_system_information.py
+win32ctypes/core/cffi/_time.py
 win32ctypes/core/cffi/_util.py
 win32ctypes/core/ctypes/__init__.py
-win32ctypes/core/ctypes/_advapi32.py
+win32ctypes/core/ctypes/_authentication.py
 win32ctypes/core/ctypes/_common.py
-win32ctypes/core/ctypes/_kernel32.py
+win32ctypes/core/ctypes/_dll.py
+win32ctypes/core/ctypes/_nl_support.py
+win32ctypes/core/ctypes/_resource.py
+win32ctypes/core/ctypes/_system_information.py
+win32ctypes/core/ctypes/_time.py
 win32ctypes/core/ctypes/_util.py
 win32ctypes/pywin32/__init__.py
 win32ctypes/pywin32/pywintypes.py
 win32ctypes/pywin32/win32api.py
 win32ctypes/pywin32/win32cred.py
 win32ctypes/tests/__init__.py
 win32ctypes/tests/compat.py
```

### Comparing `pywin32-ctypes-0.1.2/README.rst` & `pywin32-ctypes-0.2.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-.. image:: https://travis-ci.org/enthought/pywin32-ctypes.png
-  :target: https://travis-ci.org/enthought/pywin32-ctypes
-  
+
 .. image:: https://ci.appveyor.com/api/projects/status/62xqtrro26gw3l4x/branch/master?svg=true
   :target: https://ci.appveyor.com/project/EnthoughtOSS/pywin32-ctypes
 
 .. image:: https://codecov.io/github/enthought/pywin32-ctypes/coverage.svg?branch=master
    :target: https://codecov.io/github/enthought/pywin32-ctypes?branch=master
 
 .. image:: https://readthedocs.org/projects/pywin32-ctypes/badge/?version=master
@@ -39,8 +37,8 @@
 
   pip install -r dev_requirements.txt
   python install -e
 
 .. note::
 
    - While pywin32-ctypes should regularly be tested on windows, you can also
-     develop/test on unix by using wine (see travis-ci configuration to set it up).
+     develop/test on unix by using wine
```

### Comparing `pywin32-ctypes-0.1.2/setup.py` & `pywin32-ctypes-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,12 +22,12 @@
         "Programming Language :: Python :: 2.6",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.2",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
     ],
-    use_2to3=True,
     zip_safe=False,
     test_suite='win32ctypes.tests',
 )
```

### Comparing `pywin32-ctypes-0.1.2/win32ctypes/core/cffi/_advapi32.py` & `pywin32-ctypes-0.2.0/win32ctypes/core/cffi/_authentication.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 # This file is open source software distributed according to the terms in
 # LICENSE.txt
 #
 from __future__ import absolute_import
 
 from weakref import WeakKeyDictionary
 
-from win32ctypes.core.compat import is_unicode
-from ._util import ffi, check_zero
-from ._kernel32 import _GetACP
+from win32ctypes.core.compat import is_text
+from ._util import ffi, check_zero, dlls
+from ._nl_support import _GetACP
 from ._common import _PyBytes_FromStringAndSize
 
 
 ffi.cdef("""
 
 typedef struct _FILETIME {
   DWORD dwLowDateTime;
@@ -50,31 +50,30 @@
 BOOL WINAPI CredWriteW(PCREDENTIAL Credential, DWORD);
 VOID WINAPI CredFree(PVOID Buffer);
 BOOL WINAPI CredDeleteW(LPCWSTR TargetName, DWORD Type, DWORD Flags);
 
 """)
 
 _keep_alive = WeakKeyDictionary()
-advapi32 = ffi.dlopen('advapi32.dll')
 
 
 SUPPORTED_CREDKEYS = set((
     u'Type', u'TargetName', u'Persist',
     u'UserName', u'Comment', u'CredentialBlob'))
 
 
 def make_unicode(password):
     """ Convert the input string to unicode.
 
     """
-    if is_unicode(password):
+    if is_text(password):
         return password
     else:
         code_page = _GetACP()
-        return unicode(password, encoding=str(code_page), errors='strict')
+        return password.decode(encoding=str(code_page), errors='strict')
 
 
 class _CREDENTIAL(object):
 
     def __call__(self):
         return ffi.new("PCREDENTIAL")[0]
 
@@ -107,14 +106,15 @@
                     value = ffi.new('wchar_t[]', blob)
                     values.append(value)
                     setattr(c_creds, key, ffi.cast('LPTSTR', value))
         # keep values alive until c_creds goes away.
         _keep_alive[c_creds] = tuple(values)
         return c_creds
 
+
 CREDENTIAL = _CREDENTIAL()
 
 
 def PCREDENTIAL(value=None):
     return ffi.new("PCREDENTIAL", ffi.NULL if value is None else value)
 
 
@@ -139,24 +139,24 @@
         credentials[key] = data
     return credentials
 
 
 def _CredRead(TargetName, Type, Flags, ppCredential):
     target = make_unicode(TargetName)
     value = check_zero(
-        advapi32.CredReadW(target, Type, Flags, ppCredential),
+        dlls.advapi32.CredReadW(target, Type, Flags, ppCredential),
         u'CredRead')
     return value
 
 
 def _CredWrite(Credential, Flags):
     return check_zero(
-        advapi32.CredWriteW(Credential, Flags), u'CredWrite')
+        dlls.advapi32.CredWriteW(Credential, Flags), u'CredWrite')
 
 
 def _CredDelete(TargetName, Type, Flags):
     return check_zero(
-        advapi32.CredDeleteW(
+        dlls.advapi32.CredDeleteW(
             make_unicode(TargetName), Type, Flags), u'CredDelete')
 
 
-_CredFree = advapi32.CredFree
+_CredFree = dlls.advapi32.CredFree
```

### Comparing `pywin32-ctypes-0.1.2/win32ctypes/core/cffi/_common.py` & `pywin32-ctypes-0.2.0/win32ctypes/core/cffi/_common.py`

 * *Files identical despite different names*

### Comparing `pywin32-ctypes-0.1.2/win32ctypes/core/cffi/_kernel32.py` & `pywin32-ctypes-0.2.0/win32ctypes/core/cffi/_resource.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,34 +3,28 @@
 # All right reserved.
 #
 # This file is open source software distributed according to the terms in
 # LICENSE.txt
 #
 from __future__ import absolute_import
 
+
+from win32ctypes.core.compat import text_type
 from ._util import (
-    ffi, check_null, check_zero, check_false, HMODULE, PVOID, RESOURCE,
-    resource)
+    ffi, check_null, check_zero, check_false, HMODULE,
+    PVOID, RESOURCE, resource, dlls)
 
-# TODO: retrieve this value using ffi
-MAX_PATH = 260
-MAX_PATH_BUF = u'wchar_t[{0}]'.format(MAX_PATH)
 
 ffi.cdef("""
 
 typedef int WINBOOL;
 typedef WINBOOL (__stdcall *ENUMRESTYPEPROC) (HANDLE, LPTSTR, LONG_PTR);
 typedef WINBOOL (__stdcall *ENUMRESNAMEPROC) (HANDLE, LPCTSTR, LPTSTR, LONG_PTR);
 typedef WINBOOL (__stdcall *ENUMRESLANGPROC) (HANDLE, LPCTSTR, LPCTSTR, WORD, LONG_PTR);
 
-BOOL WINAPI Beep(DWORD dwFreq, DWORD dwDuration);
-UINT WINAPI GetACP(void);
-DWORD WINAPI GetTickCount(void);
-HMODULE WINAPI LoadLibraryExW(LPCTSTR lpFileName, HANDLE hFile, DWORD dwFlags);
-BOOL WINAPI FreeLibrary(HMODULE hModule);
 BOOL WINAPI EnumResourceTypesW(
     HMODULE hModule, ENUMRESTYPEPROC lpEnumFunc, LONG_PTR lParam);
 BOOL WINAPI EnumResourceNamesW(
     HMODULE hModule, LPCTSTR lpszType,
     ENUMRESNAMEPROC lpEnumFunc, LONG_PTR lParam);
 BOOL WINAPI EnumResourceLanguagesW(
     HMODULE hModule, LPCTSTR lpType,
@@ -40,21 +34,17 @@
 DWORD WINAPI SizeofResource(HMODULE hModule, HRSRC hResInfo);
 HGLOBAL WINAPI LoadResource(HMODULE hModule, HRSRC hResInfo);
 LPVOID WINAPI LockResource(HGLOBAL hResData);
 
 HANDLE WINAPI BeginUpdateResourceW(LPCTSTR pFileName, BOOL bDeleteExistingResources);
 BOOL WINAPI EndUpdateResourceW(HANDLE hUpdate, BOOL fDiscard);
 BOOL WINAPI UpdateResourceW(HANDLE hUpdate, LPCTSTR lpType, LPCTSTR lpName, WORD wLanguage, LPVOID lpData, DWORD cbData);
-UINT WINAPI GetWindowsDirectoryW(LPTSTR lpBuffer, UINT uSize);
-UINT WINAPI GetSystemDirectoryW(LPTSTR lpBuffer, UINT uSize);
 
 """)
 
-kernel32 = ffi.dlopen('kernel32.dll')
-
 
 def ENUMRESTYPEPROC(callback):
     def wrapped(hModule, lpszType, lParam):
         return callback(hModule, resource(lpszType), lParam)
     return wrapped
 
 
@@ -69,110 +59,76 @@
     def wrapped(hModule, lpszType, lpszName, wIDLanguage, lParam):
         return callback(
             hModule, resource(lpszType), resource(lpszName),
             wIDLanguage, lParam)
     return wrapped
 
 
-def _GetACP():
-    return kernel32.GetACP()
-
-
-def _GetWindowsDirectory():
-    buffer = ffi.new(MAX_PATH_BUF)
-    l = kernel32.GetWindowsDirectoryW(buffer, MAX_PATH)
-    return ffi.unpack(buffer, l)
-
-
-def _GetSystemDirectory():
-    buffer = ffi.new(MAX_PATH_BUF)
-    l = kernel32.GetSystemDirectoryW(buffer, MAX_PATH)
-    return ffi.unpack(buffer, l)
-
-
-def _GetTickCount():
-    return kernel32.GetTickCount()
-
-
-def _LoadLibraryEx(lpFilename, hFile, dwFlags):
-    result = check_null(
-        kernel32.LoadLibraryExW(
-            unicode(lpFilename), ffi.NULL, dwFlags),
-        function_name='LoadLibraryEx')
-    return HMODULE(result)
-
-
-def _FreeLibrary(hModule):
-    check_false(
-        kernel32.FreeLibrary(PVOID(hModule)),
-        function_name='FreeLibrary')
-
-
 def _EnumResourceTypes(hModule, lpEnumFunc, lParam):
     callback = ffi.callback('ENUMRESTYPEPROC', lpEnumFunc)
     check_false(
-        kernel32.EnumResourceTypesW(PVOID(hModule), callback, lParam),
+        dlls.kernel32.EnumResourceTypesW(PVOID(hModule), callback, lParam),
         function_name='EnumResourceTypes')
 
 
 def _EnumResourceNames(hModule, lpszType, lpEnumFunc, lParam):
     callback = ffi.callback('ENUMRESNAMEPROC', lpEnumFunc)
     check_false(
-        kernel32.EnumResourceNamesW(
+        dlls.kernel32.EnumResourceNamesW(
             PVOID(hModule), RESOURCE(lpszType), callback, lParam),
         function_name='EnumResourceNames')
 
 
 def _EnumResourceLanguages(hModule, lpType, lpName, lpEnumFunc, lParam):
     callback = ffi.callback('ENUMRESLANGPROC', lpEnumFunc)
     check_false(
-        kernel32.EnumResourceLanguagesW(
+        dlls.kernel32.EnumResourceLanguagesW(
             PVOID(hModule), RESOURCE(lpType),
             RESOURCE(lpName), callback, lParam),
         function_name='EnumResourceLanguages')
 
 
 def _FindResourceEx(hModule, lpType, lpName, wLanguage):
     return check_null(
-        kernel32.FindResourceExW(
+        dlls.kernel32.FindResourceExW(
             PVOID(hModule), RESOURCE(lpType), RESOURCE(lpName), wLanguage),
         function_name='FindResourceEx')
 
 
 def _SizeofResource(hModule, hResInfo):
     return check_zero(
-        kernel32.SizeofResource(PVOID(hModule), hResInfo),
+        dlls.kernel32.SizeofResource(PVOID(hModule), hResInfo),
         function_name='SizeofResource')
 
 
 def _LoadResource(hModule, hResInfo):
     return check_null(
-        kernel32.LoadResource(PVOID(hModule), hResInfo),
+        dlls.kernel32.LoadResource(PVOID(hModule), hResInfo),
         function_name='LoadResource')
 
 
 def _LockResource(hResData):
     return check_null(
-        kernel32.LockResource(hResData),
+        dlls.kernel32.LockResource(hResData),
         function_name='LockResource')
 
 
 def _BeginUpdateResource(pFileName, bDeleteExistingResources):
     result = check_null(
-        kernel32.BeginUpdateResourceW(
-            unicode(pFileName), bDeleteExistingResources))
+        dlls.kernel32.BeginUpdateResourceW(
+            text_type(pFileName), bDeleteExistingResources))
     return HMODULE(result)
 
 
 def _EndUpdateResource(hUpdate, fDiscard):
     check_false(
-        kernel32.EndUpdateResourceW(PVOID(hUpdate), fDiscard),
+        dlls.kernel32.EndUpdateResourceW(PVOID(hUpdate), fDiscard),
         function_name='EndUpdateResource')
 
 
 def _UpdateResource(hUpdate, lpType, lpName, wLanguage, cData, cbData):
     lpData = ffi.from_buffer(cData)
     check_false(
-        kernel32.UpdateResourceW(
+        dlls.kernel32.UpdateResourceW(
             PVOID(hUpdate), RESOURCE(lpType), RESOURCE(lpName),
             wLanguage, PVOID(lpData), cbData),
         function_name='UpdateResource')
```

### Comparing `pywin32-ctypes-0.1.2/win32ctypes/core/cffi/_util.py` & `pywin32-ctypes-0.2.0/win32ctypes/core/cffi/_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # LICENSE.txt
 #
 
 """ Utility functions to help with cffi wrapping.
 """
 from __future__ import absolute_import
 
+from win32ctypes.core.compat import is_bytes, is_integer, text_type
 from cffi import FFI
 
 ffi = FFI()
 ffi.set_unicode(True)
 
 
 def HMODULE(cdata):
@@ -31,18 +32,18 @@
     return int(ffi.cast("uintptr_t", x)) >> 16 == 0
 
 
 def RESOURCE(resource):
     """ Convert a resource into a compatible input for cffi.
 
     """
-    if isinstance(resource, (int, long)):
+    if is_integer(resource):
         resource = ffi.cast('wchar_t *', resource)
-    elif isinstance(resource, str):
-        resource = unicode(resource)
+    elif is_bytes(resource):
+        resource = text_type(resource)
     return resource
 
 
 def resource(lpRESOURCEID):
     """ Convert the windows RESOURCE into a python friendly object.
     """
     if IS_INTRESOURCE(lpRESOURCEID):
@@ -90,7 +91,18 @@
         exception.function = function_name
         raise exception
 
 
 check_null = ErrorWhen(ffi.NULL)
 check_zero = ErrorWhen(0)
 check_false = ErrorWhen(False)
+
+
+class Libraries(object):
+
+    def __getattr__(self, name):
+        library = ffi.dlopen('{}.dll'.format(name))
+        self.__dict__[name] = library
+        return library
+
+
+dlls = Libraries()
```

### Comparing `pywin32-ctypes-0.1.2/win32ctypes/core/ctypes/_advapi32.py` & `pywin32-ctypes-0.2.0/win32ctypes/core/ctypes/_authentication.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 #
-# (C) Copyright 2014 Enthought, Inc., Austin, TX
+# (C) Copyright 2014-18 Enthought, Inc., Austin, TX
 # All right reserved.
 #
 # This file is open source software distributed according to the terms in
 # LICENSE.txt
 #
 from __future__ import absolute_import
 
 import ctypes
 from ctypes import POINTER, Structure, c_void_p, c_wchar_p, c_char_p, cast
 from ctypes.wintypes import (
     BOOL, DWORD, FILETIME, LPCWSTR)
 
-from win32ctypes.core.compat import is_unicode
+from win32ctypes.core.compat import is_text
 from ._common import LPBYTE, _PyBytes_FromStringAndSize
-from ._util import function_factory, check_zero_factory
-from ._kernel32 import _GetACP
+from ._util import function_factory, check_zero_factory, dlls
+from ._nl_support import _GetACP
 
 
 SUPPORTED_CREDKEYS = set((
     u'Type', u'TargetName', u'Persist',
     u'UserName', u'Comment', u'CredentialBlob'))
 
-# Use a local copy of the advapi32 dll.
-advapi = ctypes.WinDLL('advapi32')
-
 
 class CREDENTIAL(Structure):
     _fields_ = [
         ("Flags", DWORD),
         ("Type", DWORD),
         ("TargetName", c_wchar_p),
         ("Comment", c_wchar_p),
@@ -66,26 +63,27 @@
                     # string we do not want that.
                     c_creds.CredentialBlobSize = \
                         ctypes.sizeof(blob_data) - \
                         ctypes.sizeof(ctypes.c_wchar)
                     c_creds.CredentialBlob = ctypes.cast(blob_data, LPBYTE)
         return c_creds
 
+
 PCREDENTIAL = POINTER(CREDENTIAL)
 
 
 def make_unicode(password):
     """ Convert the input string to unicode.
 
     """
-    if is_unicode(password):
+    if is_text(password):
         return password
     else:
         code_page = _GetACP()
-        return unicode(password, encoding=str(code_page), errors='strict')
+        return password.decode(encoding=str(code_page), errors='strict')
 
 
 def credential2dict(creds):
     credential = {}
     for key in SUPPORTED_CREDKEYS:
         if key != u'CredentialBlob':
             credential[key] = getattr(creds, key)
@@ -94,25 +92,25 @@
                 cast(creds.CredentialBlob, c_char_p),
                 creds.CredentialBlobSize)
             credential[u'CredentialBlob'] = blob
     return credential
 
 
 _CredWrite = function_factory(
-    advapi.CredWriteW,
+    dlls.advapi32.CredWriteW,
     [PCREDENTIAL, DWORD],
     BOOL,
     check_zero_factory("CredWrite"))
 
 _CredRead = function_factory(
-    advapi.CredReadW,
+    dlls.advapi32.CredReadW,
     [LPCWSTR, DWORD, DWORD, POINTER(PCREDENTIAL)],
     BOOL,
     check_zero_factory("CredRead"))
 
 _CredDelete = function_factory(
-    advapi.CredDeleteW,
+    dlls.advapi32.CredDeleteW,
     [LPCWSTR, DWORD, DWORD],
     BOOL,
     check_zero_factory("CredDelete"))
 
-_CredFree = function_factory(advapi.CredFree, [PCREDENTIAL])
+_CredFree = function_factory(dlls.advapi32.CredFree, [PCREDENTIAL])
```

### Comparing `pywin32-ctypes-0.1.2/win32ctypes/core/ctypes/_common.py` & `pywin32-ctypes-0.2.0/win32ctypes/core/ctypes/_common.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,28 @@
         return_type=py_object)
 else:
     _PyBytes_FromStringAndSize = function_factory(
         pythonapi.PyString_FromStringAndSize,
         [c_char_p, Py_ssize_t],
         return_type=py_object)
 
-IS_INTRESOURCE = lambda x: x >> 16 == 0
+
+def IS_INTRESOURCE(x):
+    return x >> 16 == 0
+
 
 byreference = ctypes.byref
 
 
 def dereference(x):
     return x.contents
+
+
+class Libraries(object):
+
+    def __getattr__(self, name):
+        library = ctypes.WinDLL(name)
+        self.__dict__[name] = library
+        return library
+
+
+dlls = Libraries()
```

### Comparing `pywin32-ctypes-0.1.2/win32ctypes/core/ctypes/_kernel32.py` & `pywin32-ctypes-0.2.0/win32ctypes/core/ctypes/_resource.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 #
-# (C) Copyright 2014 Enthought, Inc., Austin, TX
+# (C) Copyright 2018 Enthought, Inc., Austin, TX
 # All right reserved.
 #
 # This file is open source software distributed according to the terms in
 # LICENSE.txt
 #
 from __future__ import absolute_import
 
 import ctypes
 from ctypes.wintypes import (
     BOOL, DWORD, HANDLE, HMODULE, LPCWSTR, WORD, HRSRC,
-    HGLOBAL, LPVOID, UINT, LPWSTR, MAX_PATH)
+    HGLOBAL, LPVOID)
 
 from ._common import LONG_PTR, IS_INTRESOURCE
-from ._util import check_null, check_zero, check_false, function_factory
+from ._util import check_null, check_zero, check_false, function_factory, dlls
 
 _ENUMRESTYPEPROC = ctypes.WINFUNCTYPE(BOOL, HMODULE, LPVOID, LONG_PTR)
 _ENUMRESNAMEPROC = ctypes.WINFUNCTYPE(BOOL, HMODULE, LPVOID, LPVOID, LONG_PTR)
 _ENUMRESLANGPROC = ctypes.WINFUNCTYPE(
     BOOL, HMODULE, LPVOID, LPVOID, WORD, LONG_PTR)
 
-# Use a local copy of the kernel32 dll.
-kernel32 = ctypes.WinDLL('kernel32')
-
 
 def ENUMRESTYPEPROC(callback):
     def wrapped(handle, type_, param):
         if IS_INTRESOURCE(type_):
             type_ = int(type_)
         else:
             type_ = ctypes.cast(type_, LPCWSTR).value
@@ -61,134 +58,91 @@
         else:
             name = ctypes.cast(name, LPCWSTR).value
         return callback(handle, type_, name, language, param)
 
     return _ENUMRESLANGPROC(wrapped)
 
 
-_GetACP = function_factory(kernel32.GetACP, None, UINT)
+def _UpdateResource(hUpdate, lpType, lpName, wLanguage, lpData, cbData):
+    lp_type = LPCWSTR(lpType)
+    lp_name = LPCWSTR(lpName)
+    _BaseUpdateResource(hUpdate, lp_type, lp_name, wLanguage, lpData, cbData)
 
 
-_LoadLibraryEx = function_factory(
-    kernel32.LoadLibraryExW,
-    [LPCWSTR, HANDLE, DWORD],
-    HMODULE, check_null)
+def _EnumResourceNames(hModule, lpszType, lpEnumFunc, lParam):
+    resource_type = LPCWSTR(lpszType)
+    _BaseEnumResourceNames(hModule, resource_type, lpEnumFunc, lParam)
+
+
+def _EnumResourceLanguages(hModule, lpType, lpName, lpEnumFunc, lParam):
+    resource_type = LPCWSTR(lpType)
+    resource_name = LPCWSTR(lpName)
+    _BaseEnumResourceLanguages(
+        hModule, resource_type, resource_name, lpEnumFunc, lParam)
+
+
+def _FindResourceEx(hModule, lpType, lpName, wLanguage):
+    resource_type = LPCWSTR(lpType)
+    resource_name = LPCWSTR(lpName)
+    return _BaseFindResourceEx(
+        hModule, resource_type, resource_name, wLanguage)
 
-_FreeLibrary = function_factory(
-    kernel32.FreeLibrary,
-    [HMODULE],
-    BOOL,
-    check_false)
 
 _EnumResourceTypes = function_factory(
-    kernel32.EnumResourceTypesW,
+    dlls.kernel32.EnumResourceTypesW,
     [HMODULE, _ENUMRESTYPEPROC, LONG_PTR],
     BOOL,
     check_false)
 
 _LoadResource = function_factory(
-    kernel32.LoadResource,
+    dlls.kernel32.LoadResource,
     [HMODULE, HRSRC],
     HGLOBAL,
     check_null)
 
 _LockResource = function_factory(
-    kernel32.LockResource,
+    dlls.kernel32.LockResource,
     [HGLOBAL],
     LPVOID,
     check_null)
 
 _SizeofResource = function_factory(
-    kernel32.SizeofResource,
+    dlls.kernel32.SizeofResource,
     [HMODULE, HRSRC],
     DWORD,
     check_zero)
 
+_BeginUpdateResource = function_factory(
+    dlls.kernel32.BeginUpdateResourceW,
+    [LPCWSTR, BOOL],
+    HANDLE,
+    check_null)
+
+_EndUpdateResource = function_factory(
+    dlls.kernel32.EndUpdateResourceW,
+    [HANDLE, BOOL],
+    BOOL,
+    check_false)
+
 _BaseEnumResourceNames = function_factory(
-    kernel32.EnumResourceNamesW,
+    dlls.kernel32.EnumResourceNamesW,
     [HMODULE, LPCWSTR, _ENUMRESNAMEPROC, LONG_PTR],
     BOOL,
     check_false)
 
 _BaseEnumResourceLanguages = function_factory(
-    kernel32.EnumResourceLanguagesW,
+    dlls.kernel32.EnumResourceLanguagesW,
     [HMODULE, LPCWSTR, LPCWSTR, _ENUMRESLANGPROC, LONG_PTR],
     BOOL,
     check_false)
 
 _BaseFindResourceEx = function_factory(
-    kernel32.FindResourceExW,
+    dlls.kernel32.FindResourceExW,
     [HMODULE, LPCWSTR, LPCWSTR, WORD],
     HRSRC,
     check_null)
 
-_GetTickCount = function_factory(
-    kernel32.GetTickCount,
-    None,
-    DWORD)
-
-_BeginUpdateResource = function_factory(
-    kernel32.BeginUpdateResourceW,
-    [LPCWSTR, BOOL],
-    HANDLE,
-    check_null)
-
-_EndUpdateResource = function_factory(
-    kernel32.EndUpdateResourceW,
-    [HANDLE, BOOL],
-    BOOL,
-    check_false)
-
 _BaseUpdateResource = function_factory(
-    kernel32.UpdateResourceW,
+    dlls.kernel32.UpdateResourceW,
     [HANDLE, LPCWSTR, LPCWSTR, WORD, LPVOID, DWORD],
     BOOL,
     check_false)
-
-_BaseGetWindowsDirectory = function_factory(
-    kernel32.GetWindowsDirectoryW,
-    [LPWSTR, UINT],
-    UINT,
-    check_zero)
-
-_BaseGetSystemDirectory = function_factory(
-    kernel32.GetSystemDirectoryW,
-    [LPWSTR, UINT],
-    UINT,
-    check_zero)
-
-
-def _GetWindowsDirectory():
-    buffer = ctypes.create_unicode_buffer(MAX_PATH)
-    _BaseGetWindowsDirectory(buffer, MAX_PATH)
-    return ctypes.cast(buffer, LPCWSTR).value
-
-
-def _GetSystemDirectory():
-    buffer = ctypes.create_unicode_buffer(MAX_PATH)
-    _BaseGetSystemDirectory(buffer, MAX_PATH)
-    return ctypes.cast(buffer, LPCWSTR).value
-
-
-def _UpdateResource(hUpdate, lpType, lpName, wLanguage, lpData, cbData):
-    lp_type = LPCWSTR(lpType)
-    lp_name = LPCWSTR(lpName)
-    _BaseUpdateResource(hUpdate, lp_type, lp_name, wLanguage, lpData, cbData)
-
-
-def _EnumResourceNames(hModule, lpszType, lpEnumFunc, lParam):
-    resource_type = LPCWSTR(lpszType)
-    _BaseEnumResourceNames(hModule, resource_type, lpEnumFunc, lParam)
-
-
-def _EnumResourceLanguages(hModule, lpType, lpName, lpEnumFunc, lParam):
-    resource_type = LPCWSTR(lpType)
-    resource_name = LPCWSTR(lpName)
-    _BaseEnumResourceLanguages(
-        hModule, resource_type, resource_name, lpEnumFunc, lParam)
-
-
-def _FindResourceEx(hModule, lpType, lpName, wLanguage):
-    resource_type = LPCWSTR(lpType)
-    resource_name = LPCWSTR(lpName)
-    return _BaseFindResourceEx(
-        hModule, resource_type, resource_name, wLanguage)
```

### Comparing `pywin32-ctypes-0.1.2/win32ctypes/core/ctypes/_util.py` & `pywin32-ctypes-0.2.0/win32ctypes/core/ctypes/_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # LICENSE.txt
 #
 
 """ Utility functions to help with ctypes wrapping.
 """
 from __future__ import absolute_import
 
-from ctypes import GetLastError, FormatError
+from ctypes import GetLastError, FormatError, WinDLL
 
 
 def function_factory(
         function, argument_types=None,
         return_type=None, error_checking=None):
     if argument_types is not None:
         function.argtypes = argument_types
@@ -64,7 +64,18 @@
             raise make_error(function, function_name)
         else:
             return True
     return check_false
 
 
 check_false = check_false_factory()
+
+
+class Libraries(object):
+
+    def __getattr__(self, name):
+        library = WinDLL(name)
+        self.__dict__[name] = library
+        return library
+
+
+dlls = Libraries()
```

### Comparing `pywin32-ctypes-0.1.2/win32ctypes/pywin32/pywintypes.py` & `pywin32-ctypes-0.2.0/win32ctypes/pywin32/pywintypes.py`

 * *Files identical despite different names*

### Comparing `pywin32-ctypes-0.1.2/win32ctypes/pywin32/win32cred.py` & `pywin32-ctypes-0.2.0/win32ctypes/pywin32/win32cred.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,50 +5,40 @@
 # This file is open source software distributed according to the terms in
 # LICENSE.txt
 #
 """ Interface to credentials management functions. """
 
 from __future__ import absolute_import
 
-from win32ctypes.core import _advapi32, _common, _backend
+from win32ctypes.core import _authentication, _common, _backend
 from win32ctypes.pywin32.pywintypes import pywin32error as _pywin32error
 
 CRED_TYPE_GENERIC = 0x1
+CRED_PERSIST_SESSION = 0x1
+CRED_PERSIST_LOCAL_MACHINE = 0x2
 CRED_PERSIST_ENTERPRISE = 0x3
 CRED_PRESERVE_CREDENTIAL_BLOB = 0
 
 
 def CredWrite(Credential, Flags=CRED_PRESERVE_CREDENTIAL_BLOB):
     """ Creates or updates a stored credential.
 
     Parameters
     ----------
     Credential : dict
-        Parameters to be passed to win32 API CredWrite/
+        A dictionary corresponding to the PyWin32 ``PyCREDENTIAL``
+        structure.
     Flags : int
-        Always pass CRED_PRESERVE_CREDENTIAL_BLOB (i.e. 0).
-
-    Returns
-    -------
-    credentials : dict
-        A dictionary containing the following:
-
-            - Type: the type of credential (see MSDN)
-            - TargetName: the target to use (string)
-            - Persist: see MSDN
-            - UserName: the retrieved username
-            - CredentialBlob: the password (as a *string*, not an encoded
-              binary stream - this function takes care of the encoding).
-            - Comment: a string
+        Always pass ``CRED_PRESERVE_CREDENTIAL_BLOB`` (i.e. 0).
 
     """
-    c_creds = _advapi32.CREDENTIAL.fromdict(Credential, Flags)
-    c_pcreds = _advapi32.PCREDENTIAL(c_creds)
+    c_creds = _authentication.CREDENTIAL.fromdict(Credential, Flags)
+    c_pcreds = _authentication.PCREDENTIAL(c_creds)
     with _pywin32error():
-        _advapi32._CredWrite(c_pcreds, 0)
+        _authentication._CredWrite(c_pcreds, 0)
 
 
 def CredRead(TargetName, Type, Flags=0):
     """ Retrieves a stored credential.
 
     Parameters
     ----------
@@ -58,40 +48,35 @@
         One of the CRED_TYPE_* constants.
     Flags : int
         Reserved, always use 0.
 
     Returns
     -------
     credentials : dict
-        ``None`` if the target name was not found or a dictionary
-        containing the following:
-
-            - UserName: the retrieved username
-            - CredentialBlob: the password (as an utf-16 encoded 'string')
-
-
+        ``None`` if the target name was not found or A dictionary
+        corresponding to the PyWin32 ``PyCREDENTIAL`` structure.
 
     """
     if Type != CRED_TYPE_GENERIC:
         raise ValueError("Type != CRED_TYPE_GENERIC not yet supported")
 
     flag = 0
     with _pywin32error():
         if _backend == 'cffi':
-            ppcreds = _advapi32.PPCREDENTIAL()
-            _advapi32._CredRead(TargetName, Type, flag, ppcreds)
+            ppcreds = _authentication.PPCREDENTIAL()
+            _authentication._CredRead(TargetName, Type, flag, ppcreds)
             pcreds = _common.dereference(ppcreds)
         else:
-            pcreds = _advapi32.PCREDENTIAL()
-            _advapi32._CredRead(
+            pcreds = _authentication.PCREDENTIAL()
+            _authentication._CredRead(
                 TargetName, Type, flag, _common.byreference(pcreds))
     try:
-        return _advapi32.credential2dict(_common.dereference(pcreds))
+        return _authentication.credential2dict(_common.dereference(pcreds))
     finally:
-        _advapi32._CredFree(pcreds)
+        _authentication._CredFree(pcreds)
 
 
 def CredDelete(TargetName, Type, Flags=0):
     """ Remove the given target name from the stored credentials.
 
     Parameters
     ----------
@@ -102,8 +87,8 @@
     Flags : int
         Reserved, always use 0.
 
     """
     if not Type == CRED_TYPE_GENERIC:
         raise ValueError("Type != CRED_TYPE_GENERIC not yet supported.")
     with _pywin32error():
-        _advapi32._CredDelete(TargetName, Type, 0)
+        _authentication._CredDelete(TargetName, Type, 0)
```

### Comparing `pywin32-ctypes-0.1.2/win32ctypes/tests/compat.py` & `pywin32-ctypes-0.2.0/win32ctypes/tests/compat.py`

 * *Files identical despite different names*

### Comparing `pywin32-ctypes-0.1.2/win32ctypes/tests/test_win32api.py` & `pywin32-ctypes-0.2.0/win32ctypes/tests/test_win32api.py`

 * *Files identical despite different names*

### Comparing `pywin32-ctypes-0.1.2/win32ctypes/tests/test_win32cred.py` & `pywin32-ctypes-0.2.0/win32ctypes/tests/test_win32cred.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 #
 # (C) Copyright 2014 Enthought, Inc., Austin, TX
 # All right reserved.
 #
 # This file is open source software distributed according to the terms in
 # LICENSE.txt
 #
-
 from __future__ import absolute_import
-
+import os
+import sys
 import unittest
 
 import win32cred
 
 from win32ctypes.core._winerrors import ERROR_NOT_FOUND
 from win32ctypes.pywin32.pywintypes import error
 from win32ctypes.pywin32.win32cred import (
     CredDelete, CredRead, CredWrite,
     CRED_PERSIST_ENTERPRISE, CRED_TYPE_GENERIC)
 from win32ctypes.tests import compat
 
+# find the pywin32 version
+version_file = os.path.join(
+    os.path.dirname(os.path.dirname(win32cred.__file__)), 'pywin32.version.txt')
+if os.path.exists(version_file):
+    with open(version_file) as handle:
+        pywin32_build = handle.read().strip()
+else:
+    pywin32_build = None
+
 
 class TestCred(compat.TestCase):
 
-    def test_write_simple(self):
+    @unittest.skipIf(
+        pywin32_build == "223" and sys.version_info[:2] == (3,7),
+        "pywin32 version 223 bug with CredRead (mhammond/pywin32#1232)")
+    def test_write_to_pywin32(self):
         username = u"john"
         password = u"doefsajfsakfj"
         comment = u"Created by MiniPyWin32Cred test suite"
 
         target = "{0}@{1}".format(username, password)
 
         credentials = {"Type": CRED_TYPE_GENERIC,
@@ -44,15 +56,15 @@
         self.assertEqual(res["Type"], CRED_TYPE_GENERIC)
         self.assertEqual(res["UserName"], username)
         self.assertEqual(res["TargetName"], target)
         self.assertEqual(res["Comment"], comment)
         self.assertEqual(
             res["CredentialBlob"].decode('utf-16'), password)
 
-    def test_read_simple(self):
+    def test_read_from_pywin32(self):
         username = "john"
         password = "doe"
         comment = u"Created by MiniPyWin32Cred test suite"
 
         target = u"{0}@{1}".format(username, password)
 
         r_credentials = {
@@ -63,15 +75,42 @@
             u"Comment": comment,
             u"Persist": CRED_PERSIST_ENTERPRISE}
         win32cred.CredWrite(r_credentials)
 
         credentials = CredRead(target, CRED_TYPE_GENERIC)
 
         # XXX: the fact that we have to decode the password when reading, but
-        # not encode when writing is a bit insane, but that's what pywin32
+        # not encode when writing is a bit strange, but that's what pywin32
+        # seems to do as well, and we try to be backward compatible here.
+        self.assertEqual(credentials["UserName"], username)
+        self.assertEqual(credentials["TargetName"], target)
+        self.assertEqual(credentials["Comment"], comment)
+        self.assertEqual(
+            credentials["CredentialBlob"].decode("utf-16"), password)
+
+    def test_read_write(self):
+        username = "john"
+        password = "doe"
+        comment = u"Created by MiniPyWin32Cred test suite"
+
+        target = u"{0}@{1}".format(username, password)
+
+        r_credentials = {
+            u"Type": CRED_TYPE_GENERIC,
+            u"TargetName": target,
+            u"UserName": username,
+            u"CredentialBlob": password,
+            u"Comment": comment,
+            u"Persist": CRED_PERSIST_ENTERPRISE}
+        CredWrite(r_credentials)
+
+        credentials = CredRead(target, CRED_TYPE_GENERIC)
+
+        # XXX: the fact that we have to decode the password when reading, but
+        # not encode when writing is a bit strange, but that's what pywin32
         # seems to do as well, and we try to be backward compatible here.
         self.assertEqual(credentials["UserName"], username)
         self.assertEqual(credentials["TargetName"], target)
         self.assertEqual(credentials["Comment"], comment)
         self.assertEqual(
             credentials["CredentialBlob"].decode("utf-16"), password)
 
@@ -93,15 +132,15 @@
             "TargetName": target,
             "UserName": username,
             "CredentialBlob": password,
             "Comment": comment,
             "Persist": CRED_PERSIST_ENTERPRISE}
         CredWrite(r_credentials, 0)
 
-        credentials = win32cred.CredRead(target, CRED_TYPE_GENERIC)
+        credentials = CredRead(target, CRED_TYPE_GENERIC)
         self.assertTrue(credentials is not None)
 
         CredDelete(target, CRED_TYPE_GENERIC)
 
         with self.assertRaises(error) as ctx:
             CredRead(target, CRED_TYPE_GENERIC)
         self.assertEqual(ctx.exception.winerror, ERROR_NOT_FOUND)
```

