# Comparing `tmp/pytest_netdut-0.6.0.tar.gz` & `tmp/pytest_netdut-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_netdut-0.6.0.tar", last modified: Mon Jun  5 06:08:29 2023, max compression
+gzip compressed data, was "pytest_netdut-0.7.0.tar", last modified: Mon Jun 19 04:56:09 2023, max compression
```

## Comparing `pytest_netdut-0.6.0.tar` & `pytest_netdut-0.7.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:29.709213 pytest_netdut-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:29.689212 pytest_netdut-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:29.697212 pytest_netdut-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-05 06:08:29.709213 pytest_netdut-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:29.697212 pytest_netdut-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:29.689212 pytest_netdut-0.6.0/docs/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:29.701213 pytest_netdut-0.6.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   114704 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/docs/images/failed_assertion.png
--rw-r--r--   0 runner    (1001) docker     (123)    90069 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/docs/images/test_showver_results.png
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:29.701213 pytest_netdut-0.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/examples/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/examples/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/examples/test_eapi_ssh_x.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/examples/test_showver.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/examples/test_skip_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/examples/test_using_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-05 06:08:29.709213 pytest_netdut-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:29.693212 pytest_netdut-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:29.705213 pytest_netdut-0.6.0/src/pytest_netdut/
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/src/pytest_netdut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/src/pytest_netdut/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    18406 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/src/pytest_netdut/px.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/src/pytest_netdut/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/src/pytest_netdut/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:29.705213 pytest_netdut-0.6.0/src/pytest_netdut.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-05 06:08:29.000000 pytest_netdut-0.6.0/src/pytest_netdut.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-05 06:08:29.000000 pytest_netdut-0.6.0/src/pytest_netdut.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 06:08:29.000000 pytest_netdut-0.6.0/src/pytest_netdut.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-05 06:08:29.000000 pytest_netdut-0.6.0/src/pytest_netdut.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 06:08:29.000000 pytest_netdut-0.6.0/src/pytest_netdut.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:29.709213 pytest_netdut-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/tests/test_netdut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/tests/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/tests/test_wait_for.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/tests/test_xapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-05 06:08:10.000000 pytest_netdut-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.320307 pytest_netdut-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.316307 pytest_netdut-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.316307 pytest_netdut-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-19 04:56:09.320307 pytest_netdut-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.316307 pytest_netdut-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.316307 pytest_netdut-0.7.0/docs/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.316307 pytest_netdut-0.7.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   114704 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/docs/images/failed_assertion.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90069 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/docs/images/test_showver_results.png
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.320307 pytest_netdut-0.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/examples/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/examples/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/examples/test_eapi_ssh_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/examples/test_showver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/examples/test_skip_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/examples/test_using_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-19 04:56:09.320307 pytest_netdut-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.316307 pytest_netdut-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.320307 pytest_netdut-0.7.0/src/pytest_netdut/
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/src/pytest_netdut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/src/pytest_netdut/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18406 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/src/pytest_netdut/px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/src/pytest_netdut/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/src/pytest_netdut/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.320307 pytest_netdut-0.7.0/src/pytest_netdut.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-19 04:56:09.000000 pytest_netdut-0.7.0/src/pytest_netdut.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-19 04:56:09.000000 pytest_netdut-0.7.0/src/pytest_netdut.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 04:56:09.000000 pytest_netdut-0.7.0/src/pytest_netdut.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-19 04:56:09.000000 pytest_netdut-0.7.0/src/pytest_netdut.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 04:56:09.000000 pytest_netdut-0.7.0/src/pytest_netdut.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.320307 pytest_netdut-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/tests/test_netdut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/tests/test_wait_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/tests/test_xapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/tox.ini
```

### Comparing `pytest_netdut-0.6.0/.github/workflows/build.yaml` & `pytest_netdut-0.7.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/.github/workflows/release.yaml` & `pytest_netdut-0.7.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/.gitignore` & `pytest_netdut-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/Dockerfile` & `pytest_netdut-0.7.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/LICENSE` & `pytest_netdut-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/Makefile` & `pytest_netdut-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/PKG-INFO` & `pytest_netdut-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_netdut
-Version: 0.6.0
+Version: 0.7.0
 Summary: "Automated software testing for switches using pytest"
 Home-page: https://github.com/aristanetworks/pytest-netdut
 Author: "David Snowdon"
 Author-email: "daves@arista.com"
 Maintainer: "Alex Webster"
 Maintainer-email: "alexw@arista.com"
 License: "BSD 3-Clause License"
```

### Comparing `pytest_netdut-0.6.0/README.md` & `pytest_netdut-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/docs/images/failed_assertion.png` & `pytest_netdut-0.7.0/docs/images/failed_assertion.png`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/docs/images/test_showver_results.png` & `pytest_netdut-0.7.0/docs/images/test_showver_results.png`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/examples/test_daemon.py` & `pytest_netdut-0.7.0/examples/test_daemon.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/examples/test_eapi_ssh_x.py` & `pytest_netdut-0.7.0/examples/test_eapi_ssh_x.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/examples/test_skip_demo.py` & `pytest_netdut-0.7.0/examples/test_skip_demo.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/mkdocs.yml` & `pytest_netdut-0.7.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/setup.cfg` & `pytest_netdut-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/src/pytest_netdut/__init__.py` & `pytest_netdut-0.7.0/src/pytest_netdut/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/src/pytest_netdut/factories.py` & `pytest_netdut-0.7.0/src/pytest_netdut/factories.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,17 @@
 
     def sendline(self, *args, **kwargs):
         return self._cli.sendline(*args, **kwargs)
 
     def sendintr(self, *args, **kwargs):
         return self._cli.sendintr(*args, **kwargs)
 
+    def prompt(self, *args, **kwargs):
+        return self._cli.prompt(*args, **kwargs)
+
     @property
     def cli_flavor(self):
         return self._cli.cli_flavor
 
     @cli_flavor.setter
     def cli_flavor(self, value):
         self._cli.cli_flavor = value
```

### Comparing `pytest_netdut-0.6.0/src/pytest_netdut/px.py` & `pytest_netdut-0.7.0/src/pytest_netdut/px.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/src/pytest_netdut/utils.py` & `pytest_netdut-0.7.0/src/pytest_netdut/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/src/pytest_netdut/wrappers.py` & `pytest_netdut-0.7.0/src/pytest_netdut/wrappers.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/src/pytest_netdut.egg-info/PKG-INFO` & `pytest_netdut-0.7.0/src/pytest_netdut.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-netdut
-Version: 0.6.0
+Version: 0.7.0
 Summary: "Automated software testing for switches using pytest"
 Home-page: https://github.com/aristanetworks/pytest-netdut
 Author: "David Snowdon"
 Author-email: "daves@arista.com"
 Maintainer: "Alex Webster"
 Maintainer-email: "alexw@arista.com"
 License: "BSD 3-Clause License"
```

### Comparing `pytest_netdut-0.6.0/src/pytest_netdut.egg-info/SOURCES.txt` & `pytest_netdut-0.7.0/src/pytest_netdut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/tests/conftest.py` & `pytest_netdut-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/tests/test_netdut.py` & `pytest_netdut-0.7.0/tests/test_netdut.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/tests/test_translator.py` & `pytest_netdut-0.7.0/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/tests/test_wait_for.py` & `pytest_netdut-0.7.0/tests/test_wait_for.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/tests/test_xapi.py` & `pytest_netdut-0.7.0/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.6.0/tox.ini` & `pytest_netdut-0.7.0/tox.ini`

 * *Files identical despite different names*

