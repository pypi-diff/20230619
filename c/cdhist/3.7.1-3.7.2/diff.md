# Comparing `tmp/cdhist-3.7.1.tar.gz` & `tmp/cdhist-3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdhist-3.7.1.tar", last modified: Mon Jun 19 04:02:01 2023, max compression
+gzip compressed data, was "cdhist-3.7.2.tar", last modified: Mon Jun 19 04:05:01 2023, max compression
```

## Comparing `cdhist-3.7.1.tar` & `cdhist-3.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-19 04:02:01.494346 cdhist-3.7.1/
--rw-r--r--   0 mark      (1000) mark      (1000)       74 2023-06-19 03:15:16.000000 cdhist-3.7.1/.flake8
--rw-r--r--   0 mark      (1000) mark      (1000)       72 2023-03-30 00:30:45.000000 cdhist-3.7.1/.gitignore
--rw-r--r--   0 mark      (1000) mark      (1000)      343 2023-06-19 03:26:25.000000 cdhist-3.7.1/Makefile
--rw-r--r--   0 mark      (1000) mark      (1000)    15978 2023-06-19 04:02:01.494346 cdhist-3.7.1/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)    15576 2023-06-19 03:27:42.000000 cdhist-3.7.1/README.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-19 04:02:01.491013 cdhist-3.7.1/cdhist/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-09-20 03:37:27.000000 cdhist-3.7.1/cdhist/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)       93 2023-06-19 03:59:43.000000 cdhist-3.7.1/cdhist/__main__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     9425 2023-06-19 03:43:27.000000 cdhist-3.7.1/cdhist/cdhist.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4474 2023-06-19 03:24:01.000000 cdhist-3.7.1/cdhist/git_worktree.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2834 2023-06-19 03:43:27.000000 cdhist-3.7.1/cdhist/utils.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-19 04:02:01.494346 cdhist-3.7.1/cdhist.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)    15978 2023-06-19 04:02:01.000000 cdhist-3.7.1/cdhist.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      328 2023-06-19 04:02:01.000000 cdhist-3.7.1/cdhist.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-06-19 04:02:01.000000 cdhist-3.7.1/cdhist.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       46 2023-06-19 04:02:01.000000 cdhist-3.7.1/cdhist.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       51 2023-06-19 04:02:01.000000 cdhist-3.7.1/cdhist.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        7 2023-06-19 04:02:01.000000 cdhist-3.7.1/cdhist.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)     1016 2023-06-19 04:00:25.000000 cdhist-3.7.1/pyproject.toml
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2023-06-19 04:02:01.494346 cdhist-3.7.1/setup.cfg
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-19 04:05:01.124770 cdhist-3.7.2/
+-rw-r--r--   0 mark      (1000) mark      (1000)       74 2023-06-19 03:15:16.000000 cdhist-3.7.2/.flake8
+-rw-r--r--   0 mark      (1000) mark      (1000)       72 2023-03-30 00:30:45.000000 cdhist-3.7.2/.gitignore
+-rw-r--r--   0 mark      (1000) mark      (1000)      343 2023-06-19 03:26:25.000000 cdhist-3.7.2/Makefile
+-rw-r--r--   0 mark      (1000) mark      (1000)    15978 2023-06-19 04:05:01.124770 cdhist-3.7.2/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)    15576 2023-06-19 03:27:42.000000 cdhist-3.7.2/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-19 04:05:01.121437 cdhist-3.7.2/cdhist/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-09-20 03:37:27.000000 cdhist-3.7.2/cdhist/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       93 2023-06-19 03:59:43.000000 cdhist-3.7.2/cdhist/__main__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     9410 2023-06-19 04:04:15.000000 cdhist-3.7.2/cdhist/cdhist.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4474 2023-06-19 03:24:01.000000 cdhist-3.7.2/cdhist/git_worktree.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2834 2023-06-19 03:43:27.000000 cdhist-3.7.2/cdhist/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-19 04:05:01.124770 cdhist-3.7.2/cdhist.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)    15978 2023-06-19 04:05:01.000000 cdhist-3.7.2/cdhist.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      328 2023-06-19 04:05:01.000000 cdhist-3.7.2/cdhist.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-06-19 04:05:01.000000 cdhist-3.7.2/cdhist.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       46 2023-06-19 04:05:01.000000 cdhist-3.7.2/cdhist.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       51 2023-06-19 04:05:01.000000 cdhist-3.7.2/cdhist.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        7 2023-06-19 04:05:01.000000 cdhist-3.7.2/cdhist.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)     1016 2023-06-19 04:00:25.000000 cdhist-3.7.2/pyproject.toml
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2023-06-19 04:05:01.124770 cdhist-3.7.2/setup.cfg
```

### Comparing `cdhist-3.7.1/PKG-INFO` & `cdhist-3.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdhist
-Version: 3.7.1
+Version: 3.7.2
 Summary: Program to provide a Linux cd history directory stack
 Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/bulletmark/cdhist
 Keywords: bash,zsh,cd,fzf,git,worktree
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `cdhist-3.7.1/README.md` & `cdhist-3.7.2/README.md`

 * *Files identical despite different names*

### Comparing `cdhist-3.7.1/cdhist/cdhist.py` & `cdhist-3.7.2/cdhist/cdhist.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,16 +208,15 @@
 
         pkg = Path(sys.argv[0]).stem.replace('-', '_')
         try:
             version = metadata.version(pkg)
         except Exception:
             version = '?'
 
-        print(version)
-        return
+        return version
 
     # Just output shell init code if asked
     if args.init:
         print(init_code(args))
         return
 
     # This is temporary back-compatibility code until the previously
```

### Comparing `cdhist-3.7.1/cdhist/git_worktree.py` & `cdhist-3.7.2/cdhist/git_worktree.py`

 * *Files identical despite different names*

### Comparing `cdhist-3.7.1/cdhist/utils.py` & `cdhist-3.7.2/cdhist/utils.py`

 * *Files identical despite different names*

### Comparing `cdhist-3.7.1/cdhist.egg-info/PKG-INFO` & `cdhist-3.7.2/cdhist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdhist
-Version: 3.7.1
+Version: 3.7.2
 Summary: Program to provide a Linux cd history directory stack
 Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/bulletmark/cdhist
 Keywords: bash,zsh,cd,fzf,git,worktree
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `cdhist-3.7.1/pyproject.toml` & `cdhist-3.7.2/pyproject.toml`

 * *Files identical despite different names*

