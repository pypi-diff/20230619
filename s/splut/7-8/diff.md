# Comparing `tmp/splut-7.tar.gz` & `tmp/splut-8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/splut-7.tar", last modified: Wed May 18 18:54:51 2022, max compression
+gzip compressed data, was "dist/splut-8.tar", last modified: Thu Dec 15 16:41:53 2022, max compression
```

## Comparing `splut-7.tar` & `splut-8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-05-18 18:54:51.000000 splut-7/
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-05-18 18:54:51.000000 splut-7/splut.egg-info/
--rw-rw-r--   0 arc       (1000) arc       (1000)        1 2022-05-18 18:54:50.000000 splut-7/splut.egg-info/dependency_links.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)       20 2022-05-18 18:54:50.000000 splut-7/splut.egg-info/entry_points.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)      229 2022-05-18 18:54:50.000000 splut-7/splut.egg-info/SOURCES.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)        6 2022-05-18 18:54:50.000000 splut-7/splut.egg-info/top_level.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)     1108 2022-05-18 18:54:50.000000 splut-7/splut.egg-info/PKG-INFO
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-05-18 18:54:51.000000 splut-7/splut/
--rw-rw-r--   0 arc       (1000) arc       (1000)     2509 2020-03-21 12:32:44.000000 splut-7/splut/delay.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3898 2020-03-21 12:32:44.000000 splut-7/splut/bg.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      699 2020-12-08 21:00:47.000000 splut-7/splut/__init__.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     5906 2022-05-18 18:54:49.000000 splut-7/setup.py
--rw-rw-r--   0 arc       (1000) arc       (1000)       67 2022-05-18 18:54:51.000000 splut-7/setup.cfg
--rw-rw-r--   0 arc       (1000) arc       (1000)    35147 2019-11-03 22:03:53.000000 splut-7/COPYING
--rw-rw-r--   0 arc       (1000) arc       (1000)      848 2021-01-03 19:23:29.000000 splut-7/README.md
--rw-rw-r--   0 arc       (1000) arc       (1000)     1108 2022-05-18 18:54:51.000000 splut-7/PKG-INFO
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-12-15 16:41:53.000000 splut-8/
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-12-15 16:41:53.000000 splut-8/splut.egg-info/
+-rw-rw-r--   0 arc       (1000) arc       (1000)        1 2022-12-15 16:41:51.000000 splut-8/splut.egg-info/dependency_links.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)       20 2022-12-15 16:41:51.000000 splut-8/splut.egg-info/entry_points.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)      244 2022-12-15 16:41:51.000000 splut-8/splut.egg-info/SOURCES.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)        6 2022-12-15 16:41:51.000000 splut-8/splut.egg-info/top_level.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1108 2022-12-15 16:41:51.000000 splut-8/splut.egg-info/PKG-INFO
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-12-15 16:41:53.000000 splut-8/splut/
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2936 2022-07-16 18:52:25.000000 splut-8/splut/actor.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2509 2020-03-21 12:32:44.000000 splut-8/splut/delay.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3898 2020-03-21 12:32:44.000000 splut-8/splut/bg.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      699 2020-12-08 21:00:47.000000 splut-8/splut/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     5924 2022-12-15 16:41:49.000000 splut-8/setup.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)       67 2022-12-15 16:41:53.000000 splut-8/setup.cfg
+-rw-rw-r--   0 arc       (1000) arc       (1000)    35147 2019-11-03 22:03:53.000000 splut-8/COPYING
+-rw-rw-r--   0 arc       (1000) arc       (1000)      848 2021-01-03 19:23:29.000000 splut-8/README.md
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1108 2022-12-15 16:41:53.000000 splut-8/PKG-INFO
```

### Comparing `splut-7/splut.egg-info/PKG-INFO` & `splut-8/splut.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splut
-Version: 7
+Version: 8
 Summary: Concurrency-related Python utils
 Home-page: https://github.com/combatopera/splut
 Author: Andrzej Cichocki
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: COPYING
```

### Comparing `splut-7/splut/delay.py` & `splut-8/splut/delay.py`

 * *Files identical despite different names*

### Comparing `splut-7/splut/bg.py` & `splut-8/splut/bg.py`

 * *Files identical despite different names*

### Comparing `splut-7/splut/__init__.py` & `splut-8/splut/__init__.py`

 * *Files identical despite different names*

### Comparing `splut-7/setup.py` & `splut-8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2013, 2014, 2015, 2016, 2017, 2020 Andrzej Cichocki
+# Copyright 2013, 2014, 2015, 2016, 2017, 2020, 2022 Andrzej Cichocki
 
 # This file is part of pyven.
 #
 # pyven is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -17,15 +17,15 @@
 
 import setuptools
 
 def long_description():
     with open('README.md') as f:
         return f.read()
 
-# Copyright 2013, 2014, 2015, 2016, 2017, 2020 Andrzej Cichocki
+# Copyright 2013, 2014, 2015, 2016, 2017, 2020, 2022 Andrzej Cichocki
 
 # This file is part of pyven.
 #
 # pyven is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -78,15 +78,15 @@
             check_ignore = subprocess.Popen(['git', 'check-ignore'] + [p.path for p in extpaths], cwd = rootdir, stdout = subprocess.PIPE)
             ignoredpaths = set(check_ignore.communicate()[0].decode().splitlines())
             assert check_ignore.wait() in [0, 1]
             self.extpaths = [path for path in extpaths if path.path not in ignoredpaths]
         else:
             self.extpaths = extpaths
 
-# Copyright 2013, 2014, 2015, 2016, 2017, 2020 Andrzej Cichocki
+# Copyright 2013, 2014, 2015, 2016, 2017, 2020, 2022 Andrzej Cichocki
 
 # This file is part of pyven.
 #
 # pyven is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -132,15 +132,15 @@
 def ext_modules():
     extensions = [path.make_ext() for path in sourceinfo.extpaths]
     return dict(ext_modules = cythonize(extensions)) if extensions else {}
 
 sourceinfo = SourceInfo('.')
 setuptools.setup(
         name = 'splut',
-        version = '7',
+        version = '8',
         description = 'Concurrency-related Python utils',
         long_description = long_description(),
         long_description_content_type = 'text/markdown',
         url = 'https://github.com/combatopera/splut',
         author = 'Andrzej Cichocki',
         packages = sourceinfo.packages,
         py_modules = [],
```

### Comparing `splut-7/COPYING` & `splut-8/COPYING`

 * *Files identical despite different names*

### Comparing `splut-7/README.md` & `splut-8/README.md`

 * *Files identical despite different names*

### Comparing `splut-7/PKG-INFO` & `splut-8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splut
-Version: 7
+Version: 8
 Summary: Concurrency-related Python utils
 Home-page: https://github.com/combatopera/splut
 Author: Andrzej Cichocki
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: COPYING
```

