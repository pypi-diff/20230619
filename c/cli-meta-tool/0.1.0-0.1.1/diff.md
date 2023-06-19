# Comparing `tmp/cli-meta-tool-0.1.0.tar.gz` & `tmp/cli-meta-tool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-meta-tool-0.1.0.tar", last modified: Fri Jun 16 10:51:32 2023, max compression
+gzip compressed data, was "cli-meta-tool-0.1.1.tar", last modified: Mon Jun 19 06:06:39 2023, max compression
```

## Comparing `cli-meta-tool-0.1.0.tar` & `cli-meta-tool-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-16 10:51:32.349684 cli-meta-tool-0.1.0/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      216 2023-06-16 10:51:32.349684 cli-meta-tool-0.1.0/PKG-INFO
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-16 10:51:32.349684 cli-meta-tool-0.1.0/cliMetaTool/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3590 2023-06-16 10:51:19.000000 cli-meta-tool-0.1.0/cliMetaTool/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2535 2023-06-16 10:51:19.000000 cli-meta-tool-0.1.0/cliMetaTool/_const.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-16 10:51:32.349684 cli-meta-tool-0.1.0/cliMetaTool/data/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      138 2023-06-16 10:51:19.000000 cli-meta-tool-0.1.0/cliMetaTool/data/blob_config.ini
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10918 2023-06-16 10:51:19.000000 cli-meta-tool-0.1.0/cliMetaTool/meta_change.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15639 2023-06-16 10:51:19.000000 cli-meta-tool-0.1.0/cliMetaTool/meta_change_detect.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6933 2023-06-16 10:51:19.000000 cli-meta-tool-0.1.0/cliMetaTool/utils.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-16 10:51:32.349684 cli-meta-tool-0.1.0/cli_meta_tool.egg-info/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      216 2023-06-16 10:51:32.000000 cli-meta-tool-0.1.0/cli_meta_tool.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      353 2023-06-16 10:51:32.000000 cli-meta-tool-0.1.0/cli_meta_tool.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-06-16 10:51:32.000000 cli-meta-tool-0.1.0/cli_meta_tool.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       18 2023-06-16 10:51:32.000000 cli-meta-tool-0.1.0/cli_meta_tool.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       12 2023-06-16 10:51:32.000000 cli-meta-tool-0.1.0/cli_meta_tool.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-06-16 10:51:32.349684 cli-meta-tool-0.1.0/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      920 2023-06-16 10:51:19.000000 cli-meta-tool-0.1.0/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-19 06:06:39.102640 cli-meta-tool-0.1.1/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      216 2023-06-19 06:06:39.102640 cli-meta-tool-0.1.1/PKG-INFO
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-19 06:06:39.102640 cli-meta-tool-0.1.1/cliMetaTool/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3624 2023-06-19 06:06:22.000000 cli-meta-tool-0.1.1/cliMetaTool/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2535 2023-06-19 06:06:22.000000 cli-meta-tool-0.1.1/cliMetaTool/_const.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-19 06:06:39.102640 cli-meta-tool-0.1.1/cliMetaTool/data/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      138 2023-06-19 06:06:22.000000 cli-meta-tool-0.1.1/cliMetaTool/data/blob_config.ini
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10918 2023-06-19 06:06:22.000000 cli-meta-tool-0.1.1/cliMetaTool/meta_change.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15639 2023-06-19 06:06:22.000000 cli-meta-tool-0.1.1/cliMetaTool/meta_change_detect.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6982 2023-06-19 06:06:22.000000 cli-meta-tool-0.1.1/cliMetaTool/utils.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-19 06:06:39.102640 cli-meta-tool-0.1.1/cli_meta_tool.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      216 2023-06-19 06:06:39.000000 cli-meta-tool-0.1.1/cli_meta_tool.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      353 2023-06-19 06:06:39.000000 cli-meta-tool-0.1.1/cli_meta_tool.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-06-19 06:06:39.000000 cli-meta-tool-0.1.1/cli_meta_tool.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       18 2023-06-19 06:06:39.000000 cli-meta-tool-0.1.1/cli_meta_tool.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       12 2023-06-19 06:06:39.000000 cli-meta-tool-0.1.1/cli_meta_tool.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-06-19 06:06:39.102640 cli-meta-tool-0.1.1/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      920 2023-06-19 06:06:22.000000 cli-meta-tool-0.1.1/setup.py
```

### Comparing `cli-meta-tool-0.1.0/cliMetaTool/__init__.py` & `cli-meta-tool-0.1.1/cliMetaTool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,21 +47,21 @@
     else:
         detected_changes = MetaChangeDetect(diff, command_tree_before, command_tree_after)
         detected_changes.check_deep_diffs()
         result = detected_changes.export_meta_changes(only_break, output_type)
         return export_meta_changes_to_json(result, output_file)
 
 
-def version_diff(base_version, diff_version, only_break=False, version_diff_file=None):
+def version_diff(base_version, diff_version, only_break=False, version_diff_file=None, use_cache=False):
     config = load_blob_config_file()
     blob_url, path_prefix, index_file = get_blob_config(config)
-    base_version_module_list = get_target_version_modules(blob_url, path_prefix, index_file, base_version)
-    get_target_version_modules(blob_url, path_prefix, index_file, diff_version)
+    base_version_module_list = get_target_version_modules(blob_url, path_prefix, index_file, base_version, use_cache)
+    get_target_version_modules(blob_url, path_prefix, index_file, diff_version, use_cache)
     version_diffs = []
-    for _, base_meta_file_full_path, base_meta_file in base_version_module_list[:10]:
+    for _, base_meta_file_full_path, base_meta_file in base_version_module_list:
         module_name = extrct_module_name_from_meta_file(base_meta_file)
         if not module_name:
             continue
         diff_meta_file_full_path = os.path.join(os.getcwd(), path_prefix + diff_version, base_meta_file)
         if not os.path.exists(diff_meta_file_full_path):
             print(f"Module {module_name} removed for {diff_version}")
             continue
```

### Comparing `cli-meta-tool-0.1.0/cliMetaTool/_const.py` & `cli-meta-tool-0.1.1/cliMetaTool/_const.py`

 * *Files identical despite different names*

### Comparing `cli-meta-tool-0.1.0/cliMetaTool/meta_change.py` & `cli-meta-tool-0.1.1/cliMetaTool/meta_change.py`

 * *Files identical despite different names*

### Comparing `cli-meta-tool-0.1.0/cliMetaTool/meta_change_detect.py` & `cli-meta-tool-0.1.1/cliMetaTool/meta_change_detect.py`

 * *Files identical despite different names*

### Comparing `cli-meta-tool-0.1.0/cliMetaTool/utils.py` & `cli-meta-tool-0.1.1/cliMetaTool/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import configparser
 import requests
 import re
 import csv
 import logging
 from enum import Enum
 from concurrent.futures import ThreadPoolExecutor, wait, ALL_COMPLETED
-from ._const import CONFIG_FILE_PATH, CHANGE_RULE_MESSAGE_MAPPING, CHANGE_SUGGEST_MESSAGE_MAPPING, \
+from _const import CONFIG_FILE_PATH, CHANGE_RULE_MESSAGE_MAPPING, CHANGE_SUGGEST_MESSAGE_MAPPING, \
     EXPORTED_CSV_META_HEADER, DOWNLOAD_THREADS
 logger = logging.getLogger(__name__)
 
 
 MODULE_NAME_PATTERN = re.compile(r"az_([a-zA-Z0-9\-\_]+)_meta.json")
 SUBGROUP_NAME_PATTERN = re.compile(r"\[\'sub_groups\'\]\[\'([a-zA-Z0-9\-\s]+)\'\]")
 CMD_NAME_PATTERN = re.compile(r"\[\'commands\'\]\[\'([a-zA-Z0-9\-\s]+)\'\]")
@@ -87,39 +87,42 @@
                 "group_name": " ".join(name_arr[len(name_arr): (i - 1): -1]),
                 "sub_info": ret
             }
         ret = tmp
     return ret
 
 
-def module_meta_file_downloader(meta_file_url, meta_file_save_path, module_file):
+def module_meta_file_downloader(meta_file_url, meta_file_save_path, module_file, use_cache):
+    if use_cache and os.path.exists(meta_file_save_path):
+        print("Using cached {0} for {1}".format(meta_file_save_path, module_file))
+        return
     print("Downloading {0} for {1}".format(meta_file_url, module_file))
     try:
         res = requests.get(meta_file_url)
         with open(meta_file_save_path, "w") as f:
             f.write(json.dumps(res.json(), indent=4))
     except Exception as e:
         print(str(e))
 
 
-def get_target_version_modules(blob_url, path_prefix, index_file, version):
+def get_target_version_modules(blob_url, path_prefix, index_file, version, use_cache=False):
     version_meta_path = path_prefix + version
     version_meta_index_file = blob_url + "/" + version_meta_path + "/" + index_file
     version_meta_module_file_list = []
     try:
         res = requests.get(version_meta_index_file)
         module_file_list = res.text.split("\n")
         version_meta_folder = os.getcwd() + "/" + version_meta_path
         if not os.path.exists(version_meta_folder):
             os.makedirs(version_meta_folder)
         version_meta_module_file_list = [(blob_url + "/" + version_meta_path + "/" + module_file,
                                           version_meta_folder + "/" + module_file,
                                           module_file) for module_file in module_file_list if module_file]
         with ThreadPoolExecutor(max_workers=DOWNLOAD_THREADS) as pool:
-            download_module_jobs = [pool.submit(module_meta_file_downloader, _url, _save_path, module_file)
+            download_module_jobs = [pool.submit(module_meta_file_downloader, _url, _save_path, module_file, use_cache)
                                     for _url, _save_path, module_file in version_meta_module_file_list]
             wait(download_module_jobs, return_when=ALL_COMPLETED)
     except Exception as e:
         print(str(e))
     finally:
         return version_meta_module_file_list
 
@@ -194,11 +197,7 @@
     diff_file_folder = os.path.dirname(version_diff_file)
     if diff_file_folder and not os.path.exists(diff_file_folder):
         os.makedirs(diff_file_folder)
     with open(version_diff_file, "w", newline='') as f:
         writer = csv.writer(f)
         writer.writerows(csv_res)
     return None
-
-
-if __name__ == "__main__":
-    get_target_version_modules("https://versionmeta.z13.web.core.windows.net/", "azure-cli-", "index.txt", "2.49.0")
```

### Comparing `cli-meta-tool-0.1.0/setup.py` & `cli-meta-tool-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # license information.
 # -----------------------------------------------------------------------------
 
 """Azure Command Meta Tools package that can be installed using setuptools"""
 
 from setuptools import setup, find_packages
 setup(name="cli-meta-tool",
-      version='0.1.0',
+      version='0.1.1',
       description="A tool for cli metadata management",
       long_description="A tool for cli metadata management",
       license='MIT',
       author='Microsoft Corporation',
       author_email='azpycli@microsoft.com',
       packages=find_packages(),
       include_package_data=True,
```

