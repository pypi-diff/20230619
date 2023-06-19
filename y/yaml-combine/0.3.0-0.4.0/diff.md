# Comparing `tmp/yaml-combine-0.3.0.tar.gz` & `tmp/yaml-combine-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\knoxg\workspace-2022-03-randomnoun\git\yaml-combine-py\dist\tmpxtw21h83\yaml-combine-0.3.0.tar", last modified: Tue Apr 19 05:43:21 2022, max compression
+gzip compressed data, was "yaml-combine-0.4.0.tar", last modified: Mon Jun 19 00:32:37 2023, max compression
```

## Comparing `yaml-combine-0.3.0.tar` & `yaml-combine-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-04-19 05:43:21.000000 yaml-combine-0.3.0/
--rw-rw-rw-   0        0        0     1340 2022-04-10 07:21:25.000000 yaml-combine-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1844 2022-04-19 05:43:21.000000 yaml-combine-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      235 2022-04-10 07:21:25.000000 yaml-combine-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0      672 2022-04-10 07:21:25.000000 yaml-combine-0.3.0/README.md
--rw-rw-rw-   0        0        0       85 2022-04-19 05:43:21.000000 yaml-combine-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2009 2022-04-19 05:42:13.000000 yaml-combine-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-19 05:43:21.000000 yaml-combine-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2022-04-19 05:43:21.000000 yaml-combine-0.3.0/src/randomnoun/
-drwxrwxrwx   0        0        0        0 2022-04-19 05:43:21.000000 yaml-combine-0.3.0/src/randomnoun/yaml_combine/
--rw-rw-rw-   0        0        0     9776 2022-04-19 05:19:05.000000 yaml-combine-0.3.0/src/randomnoun/yaml_combine/yaml_combiner.py
--rw-rw-rw-   0        0        0       23 2022-04-10 07:21:25.000000 yaml-combine-0.3.0/src/randomnoun/yaml_combine/__init__.py
--rw-rw-rw-   0        0        0      877 2022-04-10 07:21:25.000000 yaml-combine-0.3.0/src/randomnoun/yaml_combine/__main__.py
-drwxrwxrwx   0        0        0        0 2022-04-19 05:43:21.000000 yaml-combine-0.3.0/src/yaml_combine.egg-info/
--rw-rw-rw-   0        0        0        1 2022-04-19 05:43:21.000000 yaml-combine-0.3.0/src/yaml_combine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2022-04-19 05:43:21.000000 yaml-combine-0.3.0/src/yaml_combine.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2022-04-19 05:43:21.000000 yaml-combine-0.3.0/src/yaml_combine.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0     1844 2022-04-19 05:43:21.000000 yaml-combine-0.3.0/src/yaml_combine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       46 2022-04-19 05:43:21.000000 yaml-combine-0.3.0/src/yaml_combine.egg-info/requires.txt
--rw-rw-rw-   0        0        0      471 2022-04-19 05:43:21.000000 yaml-combine-0.3.0/src/yaml_combine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2022-04-19 05:43:21.000000 yaml-combine-0.3.0/src/yaml_combine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 00:32:37.285236 yaml-combine-0.4.0/
+-rw-rw-rw-   0        0        0     1340 2022-04-10 07:21:25.000000 yaml-combine-0.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1844 2023-06-19 00:32:37.285236 yaml-combine-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      672 2022-04-10 07:21:25.000000 yaml-combine-0.4.0/README.md
+-rw-rw-rw-   0        0        0      235 2022-04-10 07:21:25.000000 yaml-combine-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-06-19 00:32:37.292683 yaml-combine-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2009 2023-06-19 00:31:05.000000 yaml-combine-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:32:37.234989 yaml-combine-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 00:32:37.231004 yaml-combine-0.4.0/src/randomnoun/
+drwxrwxrwx   0        0        0        0 2023-06-19 00:32:37.265160 yaml-combine-0.4.0/src/randomnoun/yaml_combine/
+-rw-rw-rw-   0        0        0       23 2022-04-10 07:21:25.000000 yaml-combine-0.4.0/src/randomnoun/yaml_combine/__init__.py
+-rw-rw-rw-   0        0        0      877 2022-04-10 07:21:25.000000 yaml-combine-0.4.0/src/randomnoun/yaml_combine/__main__.py
+-rw-rw-rw-   0        0        0    10548 2023-06-19 00:27:58.000000 yaml-combine-0.4.0/src/randomnoun/yaml_combine/yaml_combiner.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:32:37.283236 yaml-combine-0.4.0/src/yaml_combine.egg-info/
+-rw-rw-rw-   0        0        0     1844 2023-06-19 00:32:37.000000 yaml-combine-0.4.0/src/yaml_combine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2023-06-19 00:32:37.000000 yaml-combine-0.4.0/src/yaml_combine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 00:32:37.000000 yaml-combine-0.4.0/src/yaml_combine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-19 00:32:37.000000 yaml-combine-0.4.0/src/yaml_combine.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 00:32:37.000000 yaml-combine-0.4.0/src/yaml_combine.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       46 2023-06-19 00:32:37.000000 yaml-combine-0.4.0/src/yaml_combine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 00:32:37.000000 yaml-combine-0.4.0/src/yaml_combine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 00:32:37.284242 yaml-combine-0.4.0/tests/
+-rw-rw-rw-   0        0        0     2996 2023-06-19 00:27:58.000000 yaml-combine-0.4.0/tests/test_swagger_combiner.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yaml-combine-0.3.0/LICENSE.txt` & `yaml-combine-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yaml-combine-0.3.0/PKG-INFO` & `yaml-combine-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-combine
-Version: 0.3.0
+Version: 0.4.0
 Summary: A YAML pre-processor to combine one or more YAML files with $xref references.
 Home-page: https://github.com/randomnoun/yaml-combine-py
 Author: Greg Knox
 Author-email: knoxg+pypi@randomnoun.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/randomnoun/yaml-combine-py/issues
 Project-URL: Source, https://github.com/randomnoun/yaml-combine-py/
```

### Comparing `yaml-combine-0.3.0/README.md` & `yaml-combine-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `yaml-combine-0.3.0/setup.py` & `yaml-combine-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="yaml-combine",
-    version="0.3.0",
+    version="0.4.0",
     description="A YAML pre-processor to combine one or more YAML files with $xref references.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/randomnoun/yaml-combine-py",
     author="Greg Knox",
     author_email="knoxg+pypi@randomnoun.com",
     classifiers=[
```

### Comparing `yaml-combine-0.3.0/src/randomnoun/yaml_combine/__main__.py` & `yaml-combine-0.4.0/src/randomnoun/yaml_combine/__main__.py`

 * *Files identical despite different names*

### Comparing `yaml-combine-0.3.0/src/yaml_combine.egg-info/PKG-INFO` & `yaml-combine-0.4.0/src/yaml_combine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-combine
-Version: 0.3.0
+Version: 0.4.0
 Summary: A YAML pre-processor to combine one or more YAML files with $xref references.
 Home-page: https://github.com/randomnoun/yaml-combine-py
 Author: Greg Knox
 Author-email: knoxg+pypi@randomnoun.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/randomnoun/yaml-combine-py/issues
 Project-URL: Source, https://github.com/randomnoun/yaml-combine-py/
```

