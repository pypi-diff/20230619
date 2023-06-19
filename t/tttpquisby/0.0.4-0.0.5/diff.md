# Comparing `tmp/tttpquisby-0.0.4.tar.gz` & `tmp/tttpquisby-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tttpquisby-0.0.4.tar", last modified: Fri Jun  2 07:43:57 2023, max compression
+gzip compressed data, was "tttpquisby-0.0.5.tar", last modified: Mon Jun 19 14:18:43 2023, max compression
```

## Comparing `tttpquisby-0.0.4.tar` & `tttpquisby-0.0.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:43:57.862078 tttpquisby-0.0.4/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)    35149 2023-06-02 07:42:14.000000 tttpquisby-0.0.4/LICENSE
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)       39 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/MANIFEST.in
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1268 2023-06-02 07:43:57.862078 tttpquisby-0.0.4/PKG-INFO
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      940 2023-06-02 07:43:24.000000 tttpquisby-0.0.4/README.md
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     3903 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/requirements.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)       38 2023-06-02 07:43:57.862078 tttpquisby-0.0.4/setup.cfg
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      953 2023-06-02 07:43:57.000000 tttpquisby-0.0.4/setup.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:43:57.856078 tttpquisby-0.0.4/src/
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:43:57.857078 tttpquisby-0.0.4/src/pquisby/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/__init__.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:43:57.858078 tttpquisby-0.0.4/src/pquisby/command/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/command/__init__.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      488 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/command/compare_benchmark.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      300 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/command/main.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     3384 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/command/process_benchmark.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:43:57.859078 tttpquisby-0.0.4/src/pquisby/lib/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/__init__.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:43:57.859078 tttpquisby-0.0.4/src/pquisby/lib/benchmarks/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/benchmarks/__init__.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:43:57.859078 tttpquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/__init__.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1214 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/comparison.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     5175 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/graph.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     5364 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/uperf.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     2481 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/compare_result.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:43:57.860078 tttpquisby-0.0.4/src/pquisby/lib/credentials/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/credentials/__init__.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1119 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/credentials/creds.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      917 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/post_processing.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:43:57.860078 tttpquisby-0.0.4/src/pquisby/lib/pricing/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/pricing/__init__.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     4728 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/pricing/cloud_pricing.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     7603 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/process_result.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:43:57.861078 tttpquisby-0.0.4/src/pquisby/lib/sheet/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/sheet/__init__.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     5692 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/sheet/sheet_util.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      945 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/sheet/sheetapi.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     2370 2023-06-02 07:42:33.000000 tttpquisby-0.0.4/src/pquisby/lib/util.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-06-02 07:43:57.862078 tttpquisby-0.0.4/src/tttpquisby.egg-info/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1268 2023-06-02 07:43:57.000000 tttpquisby-0.0.4/src/tttpquisby.egg-info/PKG-INFO
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1079 2023-06-02 07:43:57.000000 tttpquisby-0.0.4/src/tttpquisby.egg-info/SOURCES.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        1 2023-06-02 07:43:57.000000 tttpquisby-0.0.4/src/tttpquisby.egg-info/dependency_links.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)       54 2023-06-02 07:43:57.000000 tttpquisby-0.0.4/src/tttpquisby.egg-info/entry_points.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1990 2023-06-02 07:43:57.000000 tttpquisby-0.0.4/src/tttpquisby.egg-info/requires.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        8 2023-06-02 07:43:57.000000 tttpquisby-0.0.4/src/tttpquisby.egg-info/top_level.txt
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.222933 tttpquisby-0.0.5/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)    35149 2023-06-13 14:39:53.000000 tttpquisby-0.0.5/LICENSE
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)       39 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/MANIFEST.in
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1268 2023-06-19 14:18:43.222933 tttpquisby-0.0.5/PKG-INFO
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      940 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/README.md
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3903 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/requirements.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)       38 2023-06-19 14:18:43.222933 tttpquisby-0.0.5/setup.cfg
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      953 2023-06-19 14:18:42.000000 tttpquisby-0.0.5/setup.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.217933 tttpquisby-0.0.5/src/
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.218933 tttpquisby-0.0.5/src/pquisby/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/__init__.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.218933 tttpquisby-0.0.5/src/pquisby/command/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/command/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      488 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/command/compare_benchmark.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      300 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/command/main.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3382 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/command/process_benchmark.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.219933 tttpquisby-0.0.5/src/pquisby/lib/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/__init__.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.219933 tttpquisby-0.0.5/src/pquisby/lib/benchmarks/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/benchmarks/__init__.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.220933 tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1214 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/comparison.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5175 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/graph.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5326 2023-06-13 15:02:10.000000 tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/uperf.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1655 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/compare_sheets.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.220933 tttpquisby-0.0.5/src/pquisby/lib/credentials/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/credentials/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1119 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/credentials/creds.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     2382 2023-06-19 14:14:22.000000 tttpquisby-0.0.5/src/pquisby/lib/post_processing.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.221933 tttpquisby-0.0.5/src/pquisby/lib/pricing/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/pricing/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     4728 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/pricing/cloud_pricing.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     6775 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/process_result.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.221933 tttpquisby-0.0.5/src/pquisby/lib/sheet/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/sheet/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5692 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/sheet/sheet_util.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      945 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/sheet/sheetapi.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     2370 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/util.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.222933 tttpquisby-0.0.5/src/tttpquisby.egg-info/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1268 2023-06-19 14:18:43.000000 tttpquisby-0.0.5/src/tttpquisby.egg-info/PKG-INFO
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1079 2023-06-19 14:18:43.000000 tttpquisby-0.0.5/src/tttpquisby.egg-info/SOURCES.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        1 2023-06-19 14:18:43.000000 tttpquisby-0.0.5/src/tttpquisby.egg-info/dependency_links.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)       54 2023-06-19 14:18:43.000000 tttpquisby-0.0.5/src/tttpquisby.egg-info/entry_points.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1990 2023-06-19 14:18:43.000000 tttpquisby-0.0.5/src/tttpquisby.egg-info/requires.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        8 2023-06-19 14:18:43.000000 tttpquisby-0.0.5/src/tttpquisby.egg-info/top_level.txt
```

### Comparing `tttpquisby-0.0.4/LICENSE` & `tttpquisby-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.4/PKG-INFO` & `tttpquisby-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tttpquisby
-Version: 0.0.4
+Version: 0.0.5
 Summary: Quisby is a data processing and visualization tool for benchmark testing.
 Home-page: https://github.com/sousinha1997/Quisby
 Author: Soumya Sinha
 Author-email: sinhasoumya97@gmail.com
 License: GPL v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tttpquisby-0.0.4/README.md` & `tttpquisby-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.4/requirements.txt` & `tttpquisby-0.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.4/setup.py` & `tttpquisby-0.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 README = (HERE / "README.md").read_text()
 
 # The text of the README file
 REQUIRE = (HERE / "requirements.txt").read_text()
 
 setup(
     name="tttpquisby",
-    version="0.0.4",
+    version="0.0.5",
     description="Quisby is a data processing and visualization tool for benchmark testing.",
     url = 'https://github.com/sousinha1997/Quisby',
     author = 'Soumya Sinha',
     author_email = 'sinhasoumya97@gmail.com',
     license = 'GPL v3.0',
     packages=find_packages("src"),
     package_dir={"":"src"},
```

### Comparing `tttpquisby-0.0.4/src/pquisby/command/process_benchmark.py` & `tttpquisby-0.0.5/src/pquisby/command/process_benchmark.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 import shutil
 import click
 from pquisby.lib.process_result import data_handler, extract_data
 from pquisby.lib.util import write_config
 
 
 @click.command()
-@click.option('-l', '--results', help="Results (results_path")
-@click.option('-t', '--test-name', help="Benchmark test name")
-@click.option('-v', '--os-type', help="Distro")
+@click.option('-l', '--results', help="Results")
+@click.option('-t', '--test-name', help="Test name")
+@click.option('-o', '--os-type', help="Distro")
 @click.option('-v', '--os-version', help="Distro version")
-@click.option('-s', '--system-name', help="Controller Name")
 @click.option('-d', '--dataset-name', help="Dataset Name")
 @click.option('-n', '--spreadsheet-name', help="Any specific spreadsheet name")
 @click.option('-i', '--spreadsheet-id', help="Any specific spreadsheet")
-@click.option('-v', '--cloud', help="cloud/local")
+@click.option('-e', '--environment', help="cloud/localhost")
 @click.option('-p', '--platform', help="platform for processing")
 @click.option('-c', '--config-path', help="config-path")
 @click.option('-it', '--input_type', help="data type for processioning , file/csv/stream ")
-def process_run(results, test_name, os_type, os_version, system_name, dataset_name, spreadsheet_name, spreadsheet_id, cloud, platform,
+def process_run(results, test_name, os_type, os_version, dataset_name, spreadsheet_name, spreadsheet_id, environment, platform,
                 config, input_type):
     if config:
         config_location = config
     else:
         logging.INFO("No config path found,switching to default location")
         conf_dir = os.getenv("HOME") + "/.config/pquisby/"
         config_location = conf_dir + "config.ini"
@@ -34,44 +33,48 @@
             # Copy the file to the destination directory
             shutil.copy("pquisby/lib/sample_files/config.ini", conf_dir)
             return
     if results:
         write_config(config_location, "test", "results", results)
     if test_name:
         write_config(config_location, "test", "test_name", test_name)
+    else:
+        return "Test name not provided"
     if os_type:
         write_config(config_location, "test", "os_type", os_type)
+    else:
+        return "OS type not provided"
     if os_version:
         write_config(config_location, "test", "os_version", os_version)
-    if system_name:
-        write_config(config_location, "test", "system_name", system_name)
     else:
-        system_name = "baremetal"
-        write_config(config_location, "test", "system_name", system_name)
+        return "OS version not provided"
+    if environment:
+        write_config(config_location, "test", "environment", system_name)
+    else:
+        print("Environment not provided. Taking default values..")
+        environment = "baremetal"
+        write_config(config_location, "test", "environment", environment)
     if dataset_name:
         write_config(config_location, "test", "dataset_name", dataset_name)
     else:
-        dataset_name = "test_" +test_name+"_"+system_name+"_"+os_type+"_"+os_version
+        dataset_name = "test_" +test_name+"_"+environment+"_"+os_type+"_"+os_version
         write_config(config_location, "test", "dataset_name", dataset_name)
     if input_type:
         write_config(config_location, "test", "input_type", input_type)
     else:
         input_type = "file"
         write_config(config_location, "test", "input_type", input_type)
     if spreadsheet_name:
         write_config(config_location, "spreadsheet", "spreadsheet_name", spreadsheet_name)
     if spreadsheet_id:
         write_config(config_location, "spreadsheet", "spreadsheet_id", spreadsheet_id)
-    if cloud:
-        write_config(config_location, "cloud", "cloud_type", cloud)
-    else:
-        write_config(config_location, "cloud", "cloud_type", "baremetal")
 
     if platform == "pbench":
-        json_res = extract_data(test_name, dataset_name, system_name, input_type, results)
+        input_type = "stream"
+        json_res = extract_data(test_name, dataset_name, environment, input_type, results)
         if json_res["jsonData"]:
             return json_res["jsonData"]
 
     elif platform == "google-doc":
         spreadsheet_id = data_handler(config_location)
```

### Comparing `tttpquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/comparison.py` & `tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/comparison.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/graph.py` & `tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/graph.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/uperf.py` & `tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/uperf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-import csv
 from itertools import groupby
-import requests
-
 
 def combine_uperf_data(results):
     result_data = []
     group_data = []
 
     for data in results:
-        if data == ['']:
+        if data == [""]:
             group_data.append(result_data)
             result_data = []
         if data:
             result_data.append(data)
     # Last data point insertion
     group_data.append(result_data)
     group_data.remove([])
     return group_data
 
 
-def create_summary_uperf_data(results,run_name,OS_RELEASE):
+def create_summary_uperf_data(results, run_name, OS_RELEASE):
     summary_results = []
     group_by_test_name = {}
     sorted_results = [combine_uperf_data(results)]
     for result in sorted_results:
         for row in result:
             key = row[1][0].split(".")[0] + "-" + row[2][0] + "-" + row[3][1]
             if key in group_by_test_name:
@@ -36,30 +33,30 @@
         test_identifier = key.rsplit("-", 2)
 
         summary_results.append([""])
         summary_results.append(test_identifier)
         summary_results.append(["Instance Count"])
 
         for ele in value:
-            summary_results[-1].append(run_name+"-os-release-"+OS_RELEASE)
+            summary_results[-1].append(run_name + "-os-release-" + OS_RELEASE)
             for index in ele[4:]:
                 if index[0] in run_data:
                     run_data[index[0]].append(index[1].strip())
                 else:
                     run_data[index[0]] = [index[1].strip()]
 
         for instance_count_data in value[0][4:]:
             summary_results.append(
                 [instance_count_data[0], *run_data[instance_count_data[0]]]
             )
 
     return summary_results
 
 
-def extract_uperf_data(dataset_name, system_name,csv_data):
+def extract_uperf_data(dataset_name, csv_data):
     """"""
     results = []
     data_position = {}
     results_json = {"data": []}
     tests_supported = ["tcp_stream", "tcp_rr", "tcp_bidirec", "tcp_maerts"]
 
     for index, row in enumerate(csv_data[0]):
@@ -72,45 +69,47 @@
         try:
             if result[1].split("-")[0] in tests_supported:
                 filtered_result.append(result)
         except Exception as exc:
             pass
     # filtered_result = list(filter(lambda x: x[1].split("-")[0] in tests_supported, csv_reader))
     # Group data by test name and pkt size
-    for test_name, items in groupby(
-        filtered_result, key=lambda x: x[1].split("-")[:2]
-    ):
+    for test_name, items in groupby(filtered_result, key=lambda x: x[1].split("-")[:2]):
         data_dict = {}
 
         for item in items:
             instance_count = "-".join(item[1].split("-")[2:])
 
             # Extract BW, trans_sec & latency data
             for key in data_position.keys():
 
                 if item[data_position[key]]:
                     if key in data_dict:
                         data_dict[key].append(
                             [instance_count, item[data_position[key]]]
                         )
                     else:
-                        data_dict[key] = [
-                            [instance_count, item[data_position[key]]]
-                        ]
-        test_json = {"vm_name": "", "test_name": "", "metrics_unit": "", "instances": []}
+                        data_dict[key] = [[instance_count, item[data_position[key]]]]
+        test_json = {
+            "vm_name": "",
+            "test_name": "",
+            "metrics_unit": "",
+            "instances": [],
+        }
         for key, test_results in data_dict.items():
             if test_results:
                 test_json["dataset_name"] = dataset_name
                 test_json["test_name"] = "".join(test_name)
                 test_json["metrics_unit"] = key
                 results.append([""])
-                results.append([system_name])
                 results.append(["".join(test_name)])
                 results.append(["Instance Count", key])
-                for instance_count, items in groupby(test_results, key=lambda x: x[0].split("-")[0]):
+                for instance_count, items in groupby(
+                    test_results, key=lambda x: x[0].split("-")[0]
+                ):
                     items = list(items)
                     item_json = {}
                     item_json["name"] = instance_count
                     if len(items) > 1:
                         failed_run = True
                         for item in items:
                             if "fail" not in item[0]:
@@ -134,10 +133,11 @@
 
     return results, results_json
 
 
 if __name__ == "__main__":
     print(
         extract_uperf_data(
-            "localhost", "/Users/soumyasinha/Workspace/2022/rocky_rhel_gvnic/hackathon/pbench.perf.lab.eng.bos.redhat.com/results/pravins.localhost/uperf__2022.10.07T06.49.32/results_uperf.csv"
+            "localhost",
+            "/Users/soumyasinha/Workspace/2022/rocky_rhel_gvnic/hackathon/pbench.perf.lab.eng.bos.redhat.com/results/pravins.localhost/uperf__2022.10.07T06.49.32/results_uperf.csv",
         )
     )
```

### Comparing `tttpquisby-0.0.4/src/pquisby/lib/credentials/creds.py` & `tttpquisby-0.0.5/src/pquisby/lib/credentials/creds.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.4/src/pquisby/lib/pricing/cloud_pricing.py` & `tttpquisby-0.0.5/src/pquisby/lib/pricing/cloud_pricing.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.4/src/pquisby/lib/process_result.py` & `tttpquisby-0.0.5/src/pquisby/lib/process_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import fileinput
 import json
 import logging
 import os.path
-import requests
-import csv
-from pquisby.lib.benchmarks.uperf.uperf import extract_uperf_data
-from pquisby.lib.util import read_config, stream_to_csv
-
+from pquisby.lib.util import read_config
 from pquisby.lib.sheet.sheet_util import (create_sheet, append_to_sheet, create_spreadsheet, delete_sheet_content)
 from pquisby.lib.benchmarks.uperf.uperf import create_summary_uperf_data
 from pquisby.lib.benchmarks.uperf.graph import graph_uperf_data
 from pquisby.lib.benchmarks.uperf.comparison import compare_uperf_results
+from pquisby.lib.post_processing import extract_data
 
 
 def process_results(results, test_name, cloud, os_type, os_version, spreadsheet_name, spreadsheet_id):
     # Create spreadsheet if it doesn't exist, otherwise delete old records
     if not spreadsheet_name:
         spreadsheet_name = test_name + "-" + cloud + "-" + os_type + "-" + os_version
     if not spreadsheet_id:
@@ -79,15 +76,15 @@
 
 def data_handler(config_location):
     global test_name
     global source
     global count
     results = []
     print(config_location)
-    cloud = read_config(config_location, 'cloud', 'cloud')
+    environment = read_config(config_location, 'test', 'environment')
     os_type = read_config(config_location, 'test', 'os_type')
     os_version = read_config(config_location, 'test', 'os_version')
     spreadsheet_name = read_config(config_location, 'spreadsheet', 'spreadsheet_name')
     spreadsheet_id = read_config(config_location, 'spreadsheet', 'spreadsheet_id')
     results_path = read_config(config_location, 'test', 'results')
     input_type = read_config(config_location, 'test', 'input_type')
     dataset_name = read_config(config_location, 'test', 'dataset_name')
@@ -134,29 +131,10 @@
             exception_type = type(exc)
             return {"status": "failed", "Exception": str(exc), "Exception_type": exception_type}
         print(f"https://docs.google.com/spreadsheets/d/{spreadsheet_id}")
         register_details_json(spreadsheet_name, spreadsheet_id)
         return spreadsheet_id
 
 
-def extract_data(test_name, dataset_name, system_name, input_type, data):
-    try:
-        if input_type == "stream":
-            csv_data = stream_to_csv(data)
-        elif input_type == "csv":
-            csv_data = data
-        elif input_type == "file":
-            with open(data) as csv_file:
-                csv_data = list(csv.reader(csv_file))
-        ret_val = []
-        json_data = {}
-        if test_name == "uperf":
-            ret_val, json_data = extract_uperf_data(dataset_name, system_name, csv_data)
-        else:
-            pass
-    except Exception as exc:
-        exception_type = type(exc)
-        return {"status": "failed", "Exception": str(exc), "Exception_type": exception_type}
-    return {"status": "success", "csvData": ret_val, "jsonData": json_data}
 
 # if __name__ == '__main__':
 #    extract_data("uperf","localhost",[['iteration_number', 'iteration_name', 'Gb_sec:client_hostname:127.0.0.1-server_hostname:192.168.122.142-server_port:20010', 'Gb_sec:client_hostname:all-server_hostname:all-server_port:all', 'trans_sec:client_hostname:127.0.0.1-server_hostname:192.168.122.142-server_port:20010', 'trans_sec:client_hostname:all-server_hostname:all-server_port:all', 'usec:client_hostname:127.0.0.1-server_hostname:192.168.122.142-server_port:20010', 'usec:client_hostname:all-server_hostname:all-server_port:all'], ['1', 'tcp_stream-65535B-1i', ' 0.0010', ' 0.0010', '', '', '', '', ''], ['2', 'tcp_maerts-65535B-1i', ' 1.1396', ' 1.1396', '', '', '', '', ''], ['3', 'tcp_bidirec-65535B-1i', ' 0.8890', ' 0.8890', '', '', '', '', ''], ['4', 'tcp_rr-65535B-1i', '', '', ' 1.8146', ' 1.8146', ' 592316.6667', ' 592316.6667', ''], ['5', 'udp_stream-65535B-1i', '', '', '', '', '', '', ''], ['6', 'udp_maerts-65535B-1i', '', '', '', '', '', '', ''], ['7', 'udp_bidirec-65535B-1i', '', '', '', '', '', '', ''], ['8', 'udp_rr-65535B-1i', '', '', '', '', '', '', ''], []])
```

### Comparing `tttpquisby-0.0.4/src/pquisby/lib/sheet/sheet_util.py` & `tttpquisby-0.0.5/src/pquisby/lib/sheet/sheet_util.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.4/src/pquisby/lib/sheet/sheetapi.py` & `tttpquisby-0.0.5/src/pquisby/lib/sheet/sheetapi.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.4/src/pquisby/lib/util.py` & `tttpquisby-0.0.5/src/pquisby/lib/util.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.4/src/tttpquisby.egg-info/PKG-INFO` & `tttpquisby-0.0.5/src/tttpquisby.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tttpquisby
-Version: 0.0.4
+Version: 0.0.5
 Summary: Quisby is a data processing and visualization tool for benchmark testing.
 Home-page: https://github.com/sousinha1997/Quisby
 Author: Soumya Sinha
 Author-email: sinhasoumya97@gmail.com
 License: GPL v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tttpquisby-0.0.4/src/tttpquisby.egg-info/SOURCES.txt` & `tttpquisby-0.0.5/src/tttpquisby.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 setup.py
 src/pquisby/__init__.py
 src/pquisby/command/__init__.py
 src/pquisby/command/compare_benchmark.py
 src/pquisby/command/main.py
 src/pquisby/command/process_benchmark.py
 src/pquisby/lib/__init__.py
-src/pquisby/lib/compare_result.py
+src/pquisby/lib/compare_sheets.py
 src/pquisby/lib/post_processing.py
 src/pquisby/lib/process_result.py
 src/pquisby/lib/util.py
 src/pquisby/lib/benchmarks/__init__.py
 src/pquisby/lib/benchmarks/uperf/__init__.py
 src/pquisby/lib/benchmarks/uperf/comparison.py
 src/pquisby/lib/benchmarks/uperf/graph.py
```

### Comparing `tttpquisby-0.0.4/src/tttpquisby.egg-info/requires.txt` & `tttpquisby-0.0.5/src/tttpquisby.egg-info/requires.txt`

 * *Files identical despite different names*

