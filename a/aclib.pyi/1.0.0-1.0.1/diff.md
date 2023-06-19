# Comparing `tmp/aclib.pyi-1.0.0.tar.gz` & `tmp/aclib.pyi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aclib.pyi-1.0.0.tar", last modified: Mon Jun 19 03:11:44 2023, max compression
+gzip compressed data, was "aclib.pyi-1.0.1.tar", last modified: Mon Jun 19 05:51:42 2023, max compression
```

## Comparing `aclib.pyi-1.0.0.tar` & `aclib.pyi-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 03:11:44.950842 aclib.pyi-1.0.0/
--rw-rw-rw-   0        0        0     1087 2023-06-14 09:24:38.000000 aclib.pyi-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1231 2023-06-19 03:11:44.948842 aclib.pyi-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-06-18 10:02:00.000000 aclib.pyi-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 03:11:44.872842 aclib.pyi-1.0.0/aclib/
-drwxrwxrwx   0        0        0        0 2023-06-19 03:11:44.921843 aclib.pyi-1.0.0/aclib/pyi/
-drwxrwxrwx   0        0        0        0 2023-06-19 03:11:44.939841 aclib.pyi-1.0.0/aclib/pyi/__API__/
--rw-rw-rw-   0        0        0      313 2023-06-19 02:29:10.000000 aclib.pyi-1.0.0/aclib/pyi/__API__/colorstr.py
--rw-rw-rw-   0        0        0     4091 2023-06-19 02:41:16.000000 aclib.pyi-1.0.0/aclib/pyi/__API__/compiler.py
--rw-rw-rw-   0        0        0      131 2023-06-17 07:36:14.000000 aclib.pyi-1.0.0/aclib/pyi/__API__/const.py
--rw-rw-rw-   0        0        0     2937 2023-06-19 02:43:03.000000 aclib.pyi-1.0.0/aclib/pyi/__API__/installer.py
--rw-rw-rw-   0        0        0       79 2023-06-18 09:23:05.000000 aclib.pyi-1.0.0/aclib/pyi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:11:44.919843 aclib.pyi-1.0.0/aclib.pyi.egg-info/
--rw-rw-rw-   0        0        0     1231 2023-06-19 03:11:44.000000 aclib.pyi-1.0.0/aclib.pyi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-06-19 03:11:44.000000 aclib.pyi-1.0.0/aclib.pyi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 03:11:44.000000 aclib.pyi-1.0.0/aclib.pyi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-19 03:11:44.000000 aclib.pyi-1.0.0/aclib.pyi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 03:11:44.000000 aclib.pyi-1.0.0/aclib.pyi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 03:11:44.950842 aclib.pyi-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1258 2023-06-18 09:54:00.000000 aclib.pyi-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:11:44.946841 aclib.pyi-1.0.0/tests/
--rw-rw-rw-   0        0        0      455 2023-06-19 03:07:50.000000 aclib.pyi-1.0.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:51:42.601544 aclib.pyi-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2023-06-14 09:24:38.000000 aclib.pyi-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1231 2023-06-19 05:51:42.600544 aclib.pyi-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-06-18 10:02:00.000000 aclib.pyi-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 05:51:42.549550 aclib.pyi-1.0.1/aclib/
+drwxrwxrwx   0        0        0        0 2023-06-19 05:51:42.581544 aclib.pyi-1.0.1/aclib/pyi/
+drwxrwxrwx   0        0        0        0 2023-06-19 05:51:42.595553 aclib.pyi-1.0.1/aclib/pyi/__API__/
+-rw-rw-rw-   0        0        0      313 2023-06-19 02:29:10.000000 aclib.pyi-1.0.1/aclib/pyi/__API__/colorstr.py
+-rw-rw-rw-   0        0        0     4063 2023-06-19 05:48:36.000000 aclib.pyi-1.0.1/aclib/pyi/__API__/compiler.py
+-rw-rw-rw-   0        0        0      131 2023-06-17 07:36:14.000000 aclib.pyi-1.0.1/aclib/pyi/__API__/const.py
+-rw-rw-rw-   0        0        0     2892 2023-06-19 05:48:36.000000 aclib.pyi-1.0.1/aclib/pyi/__API__/installer.py
+-rw-rw-rw-   0        0        0       79 2023-06-18 09:23:05.000000 aclib.pyi-1.0.1/aclib/pyi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:51:42.578546 aclib.pyi-1.0.1/aclib.pyi.egg-info/
+-rw-rw-rw-   0        0        0     1231 2023-06-19 05:51:42.000000 aclib.pyi-1.0.1/aclib.pyi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-06-19 05:51:42.000000 aclib.pyi-1.0.1/aclib.pyi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 05:51:42.000000 aclib.pyi-1.0.1/aclib.pyi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-19 05:51:42.000000 aclib.pyi-1.0.1/aclib.pyi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 05:51:42.000000 aclib.pyi-1.0.1/aclib.pyi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 05:51:42.602544 aclib.pyi-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2023-06-19 05:48:36.000000 aclib.pyi-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:51:42.598546 aclib.pyi-1.0.1/tests/
+-rw-rw-rw-   0        0        0      456 2023-06-19 05:14:59.000000 aclib.pyi-1.0.1/tests/test.py
```

### Comparing `aclib.pyi-1.0.0/LICENSE` & `aclib.pyi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aclib.pyi-1.0.0/PKG-INFO` & `aclib.pyi-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aclib.pyi
-Version: 1.0.0
+Version: 1.0.1
 Summary: compile and pack python project to exe with pyd.
 Home-page: https://github.com/AnsChaser/aclib.pyi
 Author: AnsChaser
 Author-email: anschaser@163.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `aclib.pyi-1.0.0/aclib/pyi/__API__/compiler.py` & `aclib.pyi-1.0.1/aclib/pyi/__API__/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 def compile(srcdir: str, dstdir: str = DIR_COMPILED, exclude_scripts: list[str] = None, dst_replace_confirm=True) -> str:
     """exclude_scripts is a list of glob expressions whose root equals srcdir."""
 
     dstdir = dstdir or 'compiled'
     exclude_scripts = exclude_scripts or []
     language_level = platform.python_version().split(".")[0]
     stringcode_pattern = 'f?((["\']{3})|(["\']))[\\s\\S]*?(?<!\\\\)\\1|#[\\s\\S]+?(?=\n|$)'
-    tempdir = tempfile.TemporaryDirectory(dir='', ignore_cleanup_errors=True)
+    tempdir = tempfile.TemporaryDirectory(dir='')
     copy_tree(srcdir, tempdir.name)
     all_pyfiles = matchpath('**/*.py', root=tempdir.name, onlyfile=True)
     exclude_pyfiles = matchpath(*exclude_scripts, root=tempdir.name, onlyfile=True)
     compiling_pyfiles = sorted(set(all_pyfiles) - set(exclude_pyfiles))
     builddir_content1 = matchpath('build', 'build/*', root=tempdir.name, onlydir=True)
 
     for pyfile in compiling_pyfiles:
```

### Comparing `aclib.pyi-1.0.0/aclib/pyi/__API__/installer.py` & `aclib.pyi-1.0.1/aclib/pyi/__API__/installer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
 import os, time, re, glob, tempfile, traceback, PyInstaller.__main__
-from distutils.dir_util import remove_tree
 
 from .const import *
 from .colorstr import *
 
 def makeversion(dstdir, appname) -> str:
     y, m, d = (str(i) for i in time.localtime()[:3])
     mainversion = y[-2:] + m.zfill(2) + d.zfill(2)
     subversions = ['00']
-    for fp in glob.glob('*', root_dir=dstdir):
-        subversions += re.findall(f'^{re.escape(appname)}_{mainversion}(\d\d)(?:\.exe)?$', fp)
+    for fp in glob.glob(os.path.join(dstdir, '*')):
+        subversions += re.findall(f'^{re.escape(os.path.join(dstdir, appname))}_{mainversion}(\d\d)(?:\.exe)?$', fp)
     subversions.sort(key=lambda v: int(v))
     subversion = str(int(subversions[-1]) + 1).zfill(2)
     return mainversion + subversion
 
 def pyipack(
     scriptpath: str,
     distdir: str=DIR_DIST,
@@ -25,15 +24,15 @@
     exename: str=NAME_APPNAME,
     show_console=True,
     admin_permission=False,
     one_file_mode=False,
     appfiles: list[str]=None,    # [relaglob] 相对路径起点：scriptdir
     dst_replace_confirm=True,
 ):
-    builddir = tempfile.TemporaryDirectory(dir='', ignore_cleanup_errors=True)
+    builddir = tempfile.TemporaryDirectory(dir='')
     distdir = distdir or 'dist'
     scriptdir = os.path.dirname(scriptpath)
     scriptname = os.path.basename(scriptpath)[:-3]
     appname = appname or scriptname
     appversion = appversion or makeversion(distdir, appname)
     appfullname = f'{appname}_{appversion}'
     exedir = os.path.join(distdir, appfullname)
```

### Comparing `aclib.pyi-1.0.0/aclib.pyi.egg-info/PKG-INFO` & `aclib.pyi-1.0.1/aclib.pyi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aclib.pyi
-Version: 1.0.0
+Version: 1.0.1
 Summary: compile and pack python project to exe with pyd.
 Home-page: https://github.com/AnsChaser/aclib.pyi
 Author: AnsChaser
 Author-email: anschaser@163.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `aclib.pyi-1.0.0/setup.py` & `aclib.pyi-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='aclib.pyi',
-    version='1.0.0',
+    version='1.0.1',
     author='AnsChaser',
     author_email='anschaser@163.com',
     description='compile and pack python project to exe with pyd.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AnsChaser/aclib.pyi',
     python_requires='>=3.6',
```

