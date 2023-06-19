# Comparing `tmp/pbcmd-5.1.tar.gz` & `tmp/pbcmd-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbcmd-5.1.tar", last modified: Wed May 24 14:31:23 2023, max compression
+gzip compressed data, was "pbcmd-6.0.tar", last modified: Mon Jun 19 13:43:11 2023, max compression
```

## Comparing `pbcmd-5.1.tar` & `pbcmd-6.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-05-24 14:31:23.171124 pbcmd-5.1/
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     2035 2020-12-15 02:52:07.000000 pbcmd-5.1/.gitignore
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      667 2023-05-24 14:31:23.171124 pbcmd-5.1/PKG-INFO
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      245 2021-08-03 13:23:21.000000 pbcmd-5.1/README.rst
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      729 2023-05-24 14:31:18.000000 pbcmd-5.1/pyproject.toml
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       38 2023-05-24 14:31:23.171124 pbcmd-5.1/setup.cfg
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       37 2022-12-06 02:55:21.000000 pbcmd-5.1/setup.py
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-05-24 14:31:23.167791 pbcmd-5.1/src/
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-05-24 14:31:23.171124 pbcmd-5.1/src/pbcmd/
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)        0 2021-07-29 14:48:36.000000 pbcmd-5.1/src/pbcmd/__init__.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      284 2022-12-06 02:39:31.000000 pbcmd-5.1/src/pbcmd/calc.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      766 2021-09-02 20:09:18.000000 pbcmd-5.1/src/pbcmd/cli.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     5649 2022-09-30 15:21:25.000000 pbcmd-5.1/src/pbcmd/cpush.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     3030 2023-05-24 14:27:43.000000 pbcmd-5.1/src/pbcmd/csplit.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     6585 2022-12-06 02:43:49.000000 pbcmd-5.1/src/pbcmd/git.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      208 2021-07-29 15:09:35.000000 pbcmd-5.1/src/pbcmd/hello.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1783 2022-12-06 02:43:54.000000 pbcmd-5.1/src/pbcmd/mail.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1773 2022-12-06 02:45:17.000000 pbcmd-5.1/src/pbcmd/obscure.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1069 2021-09-07 16:30:06.000000 pbcmd-5.1/src/pbcmd/proxy.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1688 2022-12-06 02:47:02.000000 pbcmd-5.1/src/pbcmd/pyon2json.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1891 2021-07-29 15:15:52.000000 pbcmd-5.1/src/pbcmd/rm_timestamped.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      746 2022-12-06 02:47:15.000000 pbcmd-5.1/src/pbcmd/timefmt.py
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-05-24 14:31:23.171124 pbcmd-5.1/src/pbcmd.egg-info/
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      667 2023-05-24 14:31:23.000000 pbcmd-5.1/src/pbcmd.egg-info/PKG-INFO
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      507 2023-05-24 14:31:23.000000 pbcmd-5.1/src/pbcmd.egg-info/SOURCES.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)        1 2023-05-24 14:31:23.000000 pbcmd-5.1/src/pbcmd.egg-info/dependency_links.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       37 2023-05-24 14:31:23.000000 pbcmd-5.1/src/pbcmd.egg-info/entry_points.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       49 2023-05-24 14:31:23.000000 pbcmd-5.1/src/pbcmd.egg-info/requires.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)        6 2023-05-24 14:31:23.000000 pbcmd-5.1/src/pbcmd.egg-info/top_level.txt
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-19 13:43:11.991117 pbcmd-6.0/
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     2035 2020-12-15 02:52:07.000000 pbcmd-6.0/.gitignore
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      667 2023-06-19 13:43:11.991117 pbcmd-6.0/PKG-INFO
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      245 2021-08-03 13:23:21.000000 pbcmd-6.0/README.rst
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      758 2023-06-19 13:42:46.000000 pbcmd-6.0/pyproject.toml
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       38 2023-06-19 13:43:11.991117 pbcmd-6.0/setup.cfg
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       37 2023-06-19 13:37:37.000000 pbcmd-6.0/setup.py
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-19 13:43:11.987784 pbcmd-6.0/src/
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-19 13:43:11.991117 pbcmd-6.0/src/pbcmd/
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)        0 2021-07-29 14:48:36.000000 pbcmd-6.0/src/pbcmd/__init__.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      469 2023-06-06 00:18:27.000000 pbcmd-6.0/src/pbcmd/calc.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      814 2023-06-19 13:38:07.000000 pbcmd-6.0/src/pbcmd/cli.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     5710 2023-06-19 13:30:53.000000 pbcmd-6.0/src/pbcmd/cpush.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     3030 2023-05-24 14:27:43.000000 pbcmd-6.0/src/pbcmd/csplit.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     6585 2022-12-06 02:43:49.000000 pbcmd-6.0/src/pbcmd/git.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      208 2021-07-29 15:09:35.000000 pbcmd-6.0/src/pbcmd/hello.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1783 2022-12-06 02:43:54.000000 pbcmd-6.0/src/pbcmd/mail.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1773 2022-12-06 02:45:17.000000 pbcmd-6.0/src/pbcmd/obscure.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      416 2023-06-19 13:37:48.000000 pbcmd-6.0/src/pbcmd/pqcat.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1069 2021-09-07 16:30:06.000000 pbcmd-6.0/src/pbcmd/proxy.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1688 2022-12-06 02:47:02.000000 pbcmd-6.0/src/pbcmd/pyon2json.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1891 2021-07-29 15:15:52.000000 pbcmd-6.0/src/pbcmd/rm_timestamped.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      746 2022-12-06 02:47:15.000000 pbcmd-6.0/src/pbcmd/timefmt.py
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-19 13:43:11.991117 pbcmd-6.0/src/pbcmd.egg-info/
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      667 2023-06-19 13:43:11.000000 pbcmd-6.0/src/pbcmd.egg-info/PKG-INFO
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      526 2023-06-19 13:43:11.000000 pbcmd-6.0/src/pbcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)        1 2023-06-19 13:43:11.000000 pbcmd-6.0/src/pbcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       37 2023-06-19 13:43:11.000000 pbcmd-6.0/src/pbcmd.egg-info/entry_points.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       64 2023-06-19 13:43:11.000000 pbcmd-6.0/src/pbcmd.egg-info/requires.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)        6 2023-06-19 13:43:11.000000 pbcmd-6.0/src/pbcmd.egg-info/top_level.txt
```

### Comparing `pbcmd-5.1/.gitignore` & `pbcmd-6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pbcmd-5.1/PKG-INFO` & `pbcmd-6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbcmd
-Version: 5.1
+Version: 6.0
 Summary: PB's miscellaneous command line tools.
 Author-email: Parantapa Bhattacharya <pb+pypi@parantapa.net>
 Project-URL: Homepage, https://github.com/parantapa/pbcmd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `pbcmd-5.1/pyproject.toml` & `pbcmd-6.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pbcmd"
-version = "5.1"
+version = "6.0"
 authors = [
   { name="Parantapa Bhattacharya", email="pb+pypi@parantapa.net" },
 ]
 description = "PB's miscellaneous command line tools."
 readme = "README.rst"
 requires-python = ">=3.10"
 classifiers = [
@@ -19,15 +19,17 @@
 
 dependencies = [
     "click",
     "python-dateutil",
     "wasabi",
     "tqdm",
     "pydantic",
-    "json5"
+    "json5",
+    "pandas",
+    "pyarrow"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/parantapa/pbcmd"
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `pbcmd-5.1/src/pbcmd/cli.py` & `pbcmd-6.0/src/pbcmd/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .calc import calc
 from .proxy import proxy
 from .timefmt import timefmt
 from .git import git
 from .pyon2json import pyon2json
 from .csplit import csplit
 from .cpush import cpush
+from .pqcat import pqcat
 
 # from .rm_timestamped import rm_timestamped
 from .obscure import obscure, unobscure
 from .mail import mail
 
 
 @click.group()
@@ -29,10 +30,11 @@
 cli.add_command(pyon2json)
 cli.add_command(csplit)
 cli.add_command(cpush)
 # cli.add_command(rm_timestamped)
 cli.add_command(obscure)
 cli.add_command(unobscure)
 cli.add_command(mail)
+cli.add_command(pqcat)
 
 if __name__ == "__main__":
     cli(prog_name="pb")
```

### Comparing `pbcmd-5.1/src/pbcmd/cpush.py` & `pbcmd-6.0/src/pbcmd/cpush.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 
     cmd = f"""
         rsync
             --archive
             --verbose
             --compress
             --delete
+            --exclude 'core.*'
             '{remote_dir_es}'
             '{local_dir_es}'
         """
     run_(cmd, errormsg="Failed to pull from remote directory")
 
 
 def rsync_push(remote_dir: RemotePath, local_dir: Path):
@@ -99,14 +100,15 @@
 
     cmd = f"""
         rsync
             --archive
             --verbose
             --compress
             --delete
+            --exclude '.git/'
             '{local_dir_es}'
             '{remote_dir_es}'
         """
     run_(cmd, errormsg="Failed to push to remote directory")
 
 
 def find_config(cwd: Path) -> Path:
```

### Comparing `pbcmd-5.1/src/pbcmd/csplit.py` & `pbcmd-6.0/src/pbcmd/csplit.py`

 * *Files identical despite different names*

### Comparing `pbcmd-5.1/src/pbcmd/git.py` & `pbcmd-6.0/src/pbcmd/git.py`

 * *Files identical despite different names*

### Comparing `pbcmd-5.1/src/pbcmd/mail.py` & `pbcmd-6.0/src/pbcmd/mail.py`

 * *Files identical despite different names*

### Comparing `pbcmd-5.1/src/pbcmd/obscure.py` & `pbcmd-6.0/src/pbcmd/obscure.py`

 * *Files identical despite different names*

### Comparing `pbcmd-5.1/src/pbcmd/proxy.py` & `pbcmd-6.0/src/pbcmd/proxy.py`

 * *Files identical despite different names*

### Comparing `pbcmd-5.1/src/pbcmd/pyon2json.py` & `pbcmd-6.0/src/pbcmd/pyon2json.py`

 * *Files identical despite different names*

### Comparing `pbcmd-5.1/src/pbcmd/rm_timestamped.py` & `pbcmd-6.0/src/pbcmd/rm_timestamped.py`

 * *Files identical despite different names*

### Comparing `pbcmd-5.1/src/pbcmd/timefmt.py` & `pbcmd-6.0/src/pbcmd/timefmt.py`

 * *Files identical despite different names*

### Comparing `pbcmd-5.1/src/pbcmd.egg-info/PKG-INFO` & `pbcmd-6.0/src/pbcmd.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbcmd
-Version: 5.1
+Version: 6.0
 Summary: PB's miscellaneous command line tools.
 Author-email: Parantapa Bhattacharya <pb+pypi@parantapa.net>
 Project-URL: Homepage, https://github.com/parantapa/pbcmd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

