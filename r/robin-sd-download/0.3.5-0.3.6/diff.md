# Comparing `tmp/robin_sd_download-0.3.5.tar.gz` & `tmp/robin_sd_download-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robin_sd_download-0.3.5.tar", last modified: Thu May  4 12:56:37 2023, max compression
+gzip compressed data, was "dist/robin_sd_download-0.3.6.tar", last modified: Mon Jun 19 10:06:19 2023, max compression
```

## Comparing `robin_sd_download-0.3.5.tar` & `robin_sd_download-0.3.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/
--rw-r--r--   0 root         (0) root         (0)      649 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download/api_interaction/
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/api_interaction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1722 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/api_interaction/get_bearer_token.py
--rw-rw-rw-   0 root         (0) root         (0)     5452 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/api_interaction/get_software.py
--rw-rw-rw-   0 root         (0) root         (0)     4897 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/api_interaction/get_software_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download/apt_interaction/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/apt_interaction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1895 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/apt_interaction/ensure_hook.py
--rw-rw-rw-   0 root         (0) root         (0)     3864 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/apt_interaction/ensure_local_repo.py
--rw-rw-rw-   0 root         (0) root         (0)    15269 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/apt_interaction/offline_install.py
--rw-rw-rw-   0 root         (0) root         (0)     4768 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/apt_interaction/prepare_install.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download/slack_interaction/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/slack_interaction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2952 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/slack_interaction/slack_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3426 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/arg_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     2220 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     1574 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/sudo_file.py
--rw-rw-rw-   0 root         (0) root         (0)     2099 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/version_checker.py
--rw-rw-rw-   0 root         (0) root         (0)     5108 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download.egg-info/
--rw-r--r--   0 root         (0) root         (0)      649 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1254 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3747 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/tests/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/robin_sd_download/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/robin_sd_download/api_interaction/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/api_interaction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/api_interaction/get_bearer_token.py
+-rw-rw-rw-   0 root         (0) root         (0)     5452 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/api_interaction/get_software.py
+-rw-rw-rw-   0 root         (0) root         (0)     4830 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/api_interaction/get_software_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/robin_sd_download/apt_interaction/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/apt_interaction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1895 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/apt_interaction/ensure_hook.py
+-rw-rw-rw-   0 root         (0) root         (0)     3864 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/apt_interaction/ensure_local_repo.py
+-rw-rw-rw-   0 root         (0) root         (0)    15269 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/apt_interaction/offline_install.py
+-rw-rw-rw-   0 root         (0) root         (0)     4768 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/apt_interaction/prepare_install.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/robin_sd_download/slack_interaction/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/slack_interaction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/slack_interaction/slack_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/robin_sd_download/supportive_scripts/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/supportive_scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3426 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/supportive_scripts/arg_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2220 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/supportive_scripts/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/supportive_scripts/sudo_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     2099 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/supportive_scripts/version_checker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5108 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/robin_sd_download/supportive_scripts/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/robin_sd_download.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/robin_sd_download.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/robin_sd_download.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/robin_sd_download.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/robin_sd_download.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/robin_sd_download.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/robin_sd_download.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:06:19.000000 robin_sd_download-0.3.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3747 2023-06-19 10:06:01.000000 robin_sd_download-0.3.6/tests/test.py
```

### Comparing `robin_sd_download-0.3.5/PKG-INFO` & `robin_sd_download-0.3.6/robin_sd_download.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: robin_sd_download
-Version: 0.3.5
+Name: robin-sd-download
+Version: 0.3.6
 Summary: Package to download files to the Robin Radar API
 Home-page: https://bitbucket.org/robin-radar-systems/sd-api-download-pip-package.git
 Author: Robin Radar Systems
 Author-email: it-team@robinradar.com
 License: MIT
 Description: # robin-sd-download
```

### Comparing `robin_sd_download-0.3.5/robin_sd_download/api_interaction/get_bearer_token.py` & `robin_sd_download-0.3.6/robin_sd_download/api_interaction/get_bearer_token.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.5/robin_sd_download/api_interaction/get_software.py` & `robin_sd_download-0.3.6/robin_sd_download/api_interaction/get_software.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.5/robin_sd_download/api_interaction/get_software_info.py` & `robin_sd_download-0.3.6/robin_sd_download/api_interaction/get_software_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,14 @@
         software = {
             'id': software_info['_id'],
             'software_path': software_info['softwarePath'],
             'software_type': software_info['softwareType'],
             'radar_type': software_info['radarType'],
             'version': software_info['version'],
             'recalled': software_info['recalled'],
-            'available_for_all': software_info['availableForAll'],
             'created_at': datetime.datetime.strptime(software_info['createdAt'], '%Y-%m-%dT%H:%M:%S.%fZ'),
             'updated_at': datetime.datetime.strptime(software_info['updatedAt'], '%Y-%m-%dT%H:%M:%S.%fZ')
         }
 
         # Log the software information
         logger.log(
             message=f"Software ID: {software['id']}", log_level="info", to_terminal=True)
```

### Comparing `robin_sd_download-0.3.5/robin_sd_download/apt_interaction/ensure_hook.py` & `robin_sd_download-0.3.6/robin_sd_download/apt_interaction/ensure_hook.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.5/robin_sd_download/apt_interaction/ensure_local_repo.py` & `robin_sd_download-0.3.6/robin_sd_download/apt_interaction/ensure_local_repo.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.5/robin_sd_download/apt_interaction/offline_install.py` & `robin_sd_download-0.3.6/robin_sd_download/apt_interaction/offline_install.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.5/robin_sd_download/apt_interaction/prepare_install.py` & `robin_sd_download-0.3.6/robin_sd_download/apt_interaction/prepare_install.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.5/robin_sd_download/slack_interaction/slack_handler.py` & `robin_sd_download-0.3.6/robin_sd_download/slack_interaction/slack_handler.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/arg_parse.py` & `robin_sd_download-0.3.6/robin_sd_download/supportive_scripts/arg_parse.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/logger.py` & `robin_sd_download-0.3.6/robin_sd_download/supportive_scripts/logger.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/sudo_file.py` & `robin_sd_download-0.3.6/robin_sd_download/supportive_scripts/sudo_file.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/version_checker.py` & `robin_sd_download-0.3.6/robin_sd_download/supportive_scripts/version_checker.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/yaml_parser.py` & `robin_sd_download-0.3.6/robin_sd_download/supportive_scripts/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.5/robin_sd_download.egg-info/PKG-INFO` & `robin_sd_download-0.3.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: robin-sd-download
-Version: 0.3.5
+Name: robin_sd_download
+Version: 0.3.6
 Summary: Package to download files to the Robin Radar API
 Home-page: https://bitbucket.org/robin-radar-systems/sd-api-download-pip-package.git
 Author: Robin Radar Systems
 Author-email: it-team@robinradar.com
 License: MIT
 Description: # robin-sd-download
```

### Comparing `robin_sd_download-0.3.5/robin_sd_download.egg-info/SOURCES.txt` & `robin_sd_download-0.3.6/robin_sd_download.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.5/setup.py` & `robin_sd_download-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.5/tests/test.py` & `robin_sd_download-0.3.6/tests/test.py`

 * *Files identical despite different names*

