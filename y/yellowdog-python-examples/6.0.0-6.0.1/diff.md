# Comparing `tmp/yellowdog-python-examples-6.0.0.tar.gz` & `tmp/yellowdog-python-examples-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowdog-python-examples-6.0.0.tar", last modified: Fri Jun  9 10:29:58 2023, max compression
+gzip compressed data, was "yellowdog-python-examples-6.0.1.tar", last modified: Mon Jun 19 07:58:26 2023, max compression
```

## Comparing `yellowdog-python-examples-6.0.0.tar` & `yellowdog-python-examples-6.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-09 10:29:58.349112 yellowdog-python-examples-6.0.0/
--rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-6.0.0/LICENSE
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-09 10:29:58.349183 yellowdog-python-examples-6.0.0/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-6.0.0/PYPI_README.md
--rw-r--r--   0 pwt        (501) staff       (20)   108894 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/README.md
--rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-6.0.0/pyproject.toml
--rw-r--r--   0 pwt        (501) staff       (20)       46 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-06-09 10:29:58.349493 yellowdog-python-examples-6.0.0/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.0/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-09 10:29:58.348269 yellowdog-python-examples-6.0.0/yd_commands/
--rw-r--r--   0 pwt        (501) staff       (20)       22 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/__init__.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3415 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/abort.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-6.0.0/yd_commands/admin.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    18382 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/args.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     5114 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/cancel.py
--rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-6.0.0/yd_commands/check_imports.py
--rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-6.0.0/yd_commands/compact_json.py
--rw-r--r--   0 pwt        (501) staff       (20)    17400 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/config.py
--rw-r--r--   0 pwt        (501) staff       (20)     5019 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/config_keys.py
--rw-r--r--   0 pwt        (501) staff       (20)    12135 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/csv_data.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1657 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/delete.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3626 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/download.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     9251 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/instantiate.py
--rw-r--r--   0 pwt        (501) staff       (20)     3729 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/interactive.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-6.0.0/yd_commands/jsonnet2json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     7798 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/list.py
--rw-r--r--   0 pwt        (501) staff       (20)     3000 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/object_utilities.py
--rw-r--r--   0 pwt        (501) staff       (20)     9525 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/printing.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    13218 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/provision.py
--rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.0/yd_commands/provision_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.0/yd_commands/reformat_json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3232 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/shutdown.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    40530 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/submit.py
--rw-r--r--   0 pwt        (501) staff       (20)     6052 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.0/yd_commands/submit_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2916 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/terminate.py
--rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-6.0.0/yd_commands/type_check.py
--rw-r--r--   0 pwt        (501) staff       (20)     2237 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/upload.py
--rw-r--r--   0 pwt        (501) staff       (20)     3389 2023-04-19 15:22:46.000000 yellowdog-python-examples-6.0.0/yd_commands/upload_utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     2177 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/validate_properties.py
--rw-r--r--   0 pwt        (501) staff       (20)    11037 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/variables.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-6.0.0/yd_commands/version.py
--rw-r--r--   0 pwt        (501) staff       (20)     2200 2023-04-19 15:22:46.000000 yellowdog-python-examples-6.0.0/yd_commands/wrapper.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-09 10:29:58.349008 yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-09 10:29:58.000000 yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-06-09 10:29:58.000000 yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2023-06-09 10:29:58.000000 yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      574 2023-06-09 10:29:58.000000 yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)       61 2023-06-09 10:29:58.000000 yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)       12 2023-06-09 10:29:58.000000 yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-19 07:58:26.677713 yellowdog-python-examples-6.0.1/
+-rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-6.0.1/LICENSE
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-19 07:58:26.677782 yellowdog-python-examples-6.0.1/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-6.0.1/PYPI_README.md
+-rw-r--r--   0 pwt        (501) staff       (20)   109494 2023-06-19 07:57:31.000000 yellowdog-python-examples-6.0.1/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-6.0.1/pyproject.toml
+-rw-r--r--   0 pwt        (501) staff       (20)       46 2023-06-19 07:57:31.000000 yellowdog-python-examples-6.0.1/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-06-19 07:58:26.678058 yellowdog-python-examples-6.0.1/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.1/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-19 07:58:26.676720 yellowdog-python-examples-6.0.1/yd_commands/
+-rw-r--r--   0 pwt        (501) staff       (20)       22 2023-06-19 07:57:31.000000 yellowdog-python-examples-6.0.1/yd_commands/__init__.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3415 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/abort.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-6.0.1/yd_commands/admin.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    18382 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.1/yd_commands/args.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     5114 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/cancel.py
+-rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-6.0.1/yd_commands/check_imports.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-6.0.1/yd_commands/compact_json.py
+-rw-r--r--   0 pwt        (501) staff       (20)    17400 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.1/yd_commands/config.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5019 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.1/yd_commands/config_keys.py
+-rw-r--r--   0 pwt        (501) staff       (20)    12135 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.1/yd_commands/csv_data.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1657 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/delete.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3626 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/download.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     9251 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/instantiate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3729 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/interactive.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-6.0.1/yd_commands/jsonnet2json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     7798 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/list.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3000 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/object_utilities.py
+-rw-r--r--   0 pwt        (501) staff       (20)     9525 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/printing.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    13218 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.1/yd_commands/provision.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.1/yd_commands/provision_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.1/yd_commands/reformat_json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3232 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/shutdown.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    40685 2023-06-19 07:57:31.000000 yellowdog-python-examples-6.0.1/yd_commands/submit.py
+-rw-r--r--   0 pwt        (501) staff       (20)     6052 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.1/yd_commands/submit_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2916 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/terminate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-6.0.1/yd_commands/type_check.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2237 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/upload.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3389 2023-06-17 13:30:23.000000 yellowdog-python-examples-6.0.1/yd_commands/upload_utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2177 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.1/yd_commands/validate_properties.py
+-rw-r--r--   0 pwt        (501) staff       (20)    11037 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/variables.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-6.0.1/yd_commands/version.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2200 2023-04-19 15:22:46.000000 yellowdog-python-examples-6.0.1/yd_commands/wrapper.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-19 07:58:26.677599 yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-19 07:58:26.000000 yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-06-19 07:58:26.000000 yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2023-06-19 07:58:26.000000 yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      574 2023-06-19 07:58:26.000000 yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       61 2023-06-19 07:58:26.000000 yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       12 2023-06-19 07:58:26.000000 yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/top_level.txt
```

### Comparing `yellowdog-python-examples-6.0.0/LICENSE` & `yellowdog-python-examples-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/PKG-INFO` & `yellowdog-python-examples-6.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 6.0.0
+Version: 6.0.1
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-6.0.0/PYPI_README.md` & `yellowdog-python-examples-6.0.1/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/README.md` & `yellowdog-python-examples-6.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 * [Work Requirement Properties](#work-requirement-properties)
    * [Work Requirement JSON File Structure](#work-requirement-json-file-structure)
    * [Property Inheritance](#property-inheritance)
    * [Work Requirement Property Dictionary](#work-requirement-property-dictionary)
    * [Automatic Properties](#automatic-properties)
       * [Work Requirement, Task Group and Task Naming](#work-requirement-task-group-and-task-naming)
       * [Task Types](#task-types)
-         * [Bash, Python and PowerShell Tasks](#bash-python-and-powershell-tasks)
+         * [Bash, Python, PowerShell and cmd/bat Tasks](#bash-python-powershell-and-cmdbat-tasks)
          * [Docker Tasks](#docker-tasks)
-         * [Bash, Python, PowerShell and Docker without Automatic Processing](#bash-python-powershell-and-docker-without-automatic-processing)
+         * [Bash, Python, PowerShell, cmd/bat and Docker without Automatic Processing](#bash-python-powershell-cmdbat-and-docker-without-automatic-processing)
       * [Task Counts](#task-counts)
    * [Examples](#examples)
       * [TOML Properties in the workRequirement Section](#toml-properties-in-the-workrequirement-section)
       * [JSON Properties at the Work Requirement Level](#json-properties-at-the-work-requirement-level)
       * [JSON Properties at the Task Group Level](#json-properties-at-the-task-group-level)
       * [JSON Properties at the Task Level](#json-properties-at-the-task-level)
    * [Variable Substitutions in Work Requirement Properties](#variable-substitutions-in-work-requirement-properties)
@@ -80,15 +80,15 @@
    * [yd-delete](#yd-delete)
    * [yd-upload](#yd-upload)
    * [yd-shutdown](#yd-shutdown)
    * [yd-instantiate](#yd-instantiate)
       * [Test-Running a Dynamic Template](#test-running-a-dynamic-template)
    * [yd-terminate](#yd-terminate)
 
-<!-- Added by: pwt, at: Mon Jun  5 18:32:03 BST 2023 -->
+<!-- Added by: pwt, at: Sat Jun 17 14:37:49 BST 2023 -->
 
 <!--te-->
 
 # Overview
 
 This repository contains a set of example Python scripts for interacting with the YellowDog Platform. The scripts use the **[YellowDog Python SDK](https://docs.yellowdog.co/api/python/index.html)**, the code for which can be found [on GitHub](https://github.com/yellowdog/yellowdog-sdk-python-public).
 
@@ -482,19 +482,19 @@
 
 ### Task Types
 
 - If `taskType` is set only at the TOML file level, then `taskTypes` is automatically populated for Task Groups, unless overridden.
 - If `taskType` is set at the Task level, then `taskTypes` is automatically populated for the Task Groups level using the accumulated Task Types from the Tasks included in each Task Group, unless overridden.
 - If `taskTypes` is set at the Task Group Level, and has only one Task Type entry, then `taskType` is automatically set at the Task Level using the single Task Type, unless overridden.
 
-For the **`bash`**, **`powershell`** and **`docker`** task types, some automatic processing will be performed if the **`executable`** property is set.
+For the **`bash`**, **`powershell`**, **`cmd`**/**`bat`** and **`docker`** task types, some automatic processing will be performed if the **`executable`** property is set.
 
-#### Bash, Python and PowerShell Tasks
+#### Bash, Python, PowerShell and cmd/bat Tasks
 
-As a convenience, for the **`bash`**, **`python`**, and **`powershell`** Task Types, the script nominated in the **`executable`** property is automatically added to the `inputs` list (if not already present). This means the script file will be uploaded to the Object Store, and made a requirement of the Task when it runs.
+As a convenience, for the **`bash`**, **`python`**, **`powershell`**, and **`cmd`** (or **`bat`**) Task Types, the script nominated in the **`executable`** property is automatically added to the `inputs` list (if not already present). This means the script file will be uploaded to the Object Store, and made a requirement of the Task when it runs.
 
 Using a Bash Task as an example (in TOML form):
 
 ```toml
 taskType = "bash"
 executable = "my_bash_script.sh"
 arguments = ["1", "2", "3"]
@@ -503,39 +503,55 @@
 
 ```toml
 taskType = "bash"
 inputs = ["my_bash_script.sh"]
 arguments = ["{{wr_name}}/my_bash_script.sh", "1", "2", "3"]
 ```
 
+In the case of Windows batch (`.bat`) files, a `/c` flag is prepended to the `cmd.exe` argument list to ensure correct execution bahaviour. For example:
+
+```toml
+taskType = "cmd"  # or "bat"
+executable = "my_script.bat"
+arguments = ["1", "2", "3"]
+```
+
+is equivalent to:
+
+```toml
+taskType = "cmd"  # or "bat"
+inputs = ["my_script.bat"]
+arguments = ["/c", "{{wr_name}}\\my_bash_script.sh", "1", "2", "3"]
+```
+
 #### Docker Tasks
 
 For the **`docker`** Task Type, the variables supplied in the `dockerEnvironment` property are unpacked into the argument list as `--env` entries, the Docker container name supplied in the `executable` property is then added to the arguments list, followed by the arguments supplied in the `arguments` property. The `dockerUsername` and `dockerPassword` properties, if supplied, are added to the `environment` property.
 
 For example:
 ```toml
 taskType = "docker"
 executable = "my_dockerhub_repo/my_container_image"
-dockerEnvironment = { E1 = "EeeOne"}
+dockerEnvironment = {E1 = "EeeOne"}
 dockerUsername = "my_user"
 dockerPassword = "my_password"
 arguments = ["1", "2", "3"]
 ```
 
 is equivalent to the following being sent for processing by the `docker` Task Type, the YellowDog version of which will log in to the Docker repo (if required) then issue a `docker run` command with the arguments supplied:
 
 ```toml
 taskType = "docker"
 arguments = ["--env E1=EeeOne", "my_dockerhubrepo/my_container_image", "1", "2", "3"]
 environment = {DOCKER_USERNAME = "my_user", DOCKER_PASSWORD = "my_password"}
 ```
 
-#### Bash, Python, PowerShell and Docker without Automatic Processing
+#### Bash, Python, PowerShell, cmd/bat and Docker without Automatic Processing
 
-If the `executable` property is not supplied, the automatic processing described above for `bash`, `python`, `powershell`, and `docker` taskTypes is not applied.
+If the `executable` property is not supplied, the automatic processing described above for `bash`, `python`, `powershell`, `cmd` (or `bat`) and `docker` task types is not applied.
 
 ### Task Counts
 
 This property will expand the number of Tasks to match `taskCount`.
 
 The `taskCount` property can be set only in the `workRequirement` section of the `config.toml` file, or in the `taskGroup` section(s) of a JSON Work Requirement definition.
 
@@ -1343,15 +1359,17 @@
     targetInstanceCount = 1
     templateId = "ydid:crt:D9C548:465a107c-7cea-46e3-9fdd-15116cb92c40"
     # Note: only one of 'userData'/'userDataFile'/'userDataFiles' should be set
     userData = ""
     userDataFile = "myuserdata.txt"
     userDataFiles = ["myuserdata1.txt", "myuserdata2.txt"]
     workerTag = "tag-{{username}}"
+    # Specify either workersPerNode or workersPerVCPU
     workersPerNode = 1
+    workersPerVCPU = 1
 #   workerPoolData = "worker_pool.json"
 ```
 
 ## Worker Pool Specification Using JSON Documents
 
 It's also possible to capture a Worker Pool definition as a JSON document. The JSON filename can be supplied either using the command line with the `--worker-pool` or `-p` parameter with `yd-provision`, or by populating the `workerPoolData` property in the TOML configuration file with the JSON filename. Command line specification takes priority over TOML specification.
```

### Comparing `yellowdog-python-examples-6.0.0/pyproject.toml` & `yellowdog-python-examples-6.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/setup.cfg` & `yellowdog-python-examples-6.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/abort.py` & `yellowdog-python-examples-6.0.1/yd_commands/abort.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/admin.py` & `yellowdog-python-examples-6.0.1/yd_commands/admin.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/args.py` & `yellowdog-python-examples-6.0.1/yd_commands/args.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/cancel.py` & `yellowdog-python-examples-6.0.1/yd_commands/cancel.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/check_imports.py` & `yellowdog-python-examples-6.0.1/yd_commands/check_imports.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/compact_json.py` & `yellowdog-python-examples-6.0.1/yd_commands/compact_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/config.py` & `yellowdog-python-examples-6.0.1/yd_commands/config.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/config_keys.py` & `yellowdog-python-examples-6.0.1/yd_commands/config_keys.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/csv_data.py` & `yellowdog-python-examples-6.0.1/yd_commands/csv_data.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/delete.py` & `yellowdog-python-examples-6.0.1/yd_commands/delete.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/download.py` & `yellowdog-python-examples-6.0.1/yd_commands/download.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/instantiate.py` & `yellowdog-python-examples-6.0.1/yd_commands/instantiate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/interactive.py` & `yellowdog-python-examples-6.0.1/yd_commands/interactive.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/jsonnet2json.py` & `yellowdog-python-examples-6.0.1/yd_commands/jsonnet2json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/list.py` & `yellowdog-python-examples-6.0.1/yd_commands/list.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/object_utilities.py` & `yellowdog-python-examples-6.0.1/yd_commands/object_utilities.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/printing.py` & `yellowdog-python-examples-6.0.1/yd_commands/printing.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/provision.py` & `yellowdog-python-examples-6.0.1/yd_commands/provision.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/provision_utils.py` & `yellowdog-python-examples-6.0.1/yd_commands/provision_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/reformat_json.py` & `yellowdog-python-examples-6.0.1/yd_commands/reformat_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/shutdown.py` & `yellowdog-python-examples-6.0.1/yd_commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/submit.py` & `yellowdog-python-examples-6.0.1/yd_commands/submit.py`

 * *Files 1% similar despite different names*

```diff
@@ -955,18 +955,17 @@
                 wr_data.get(FLATTEN_PATHS, CONFIG_WR.flatten_input_paths),
             ),
         )
     ):
         flatten_input_paths = FlattenPath.FILE_NAME_ONLY
 
     # Special processing for Bash, Python & PowerShell tasks if the 'executable'
-    # property is set
-    # The script is uploaded if this hasn't already been done, and
-    # added to the list of required files.
-    if task_type in ["bash", "powershell", "python"]:
+    # property is set. The script is uploaded if this hasn't already been done,
+    # and added to the list of required files.
+    if task_type in ["bash", "powershell", "python", "cmd", "bat"]:
         if executable is None:
             print_log(f"Note: no 'executable' specified for '{task_type}' Task Type")
             return _make_task(flatten_input_paths)
 
         UPLOADED_FILES.add_input_file(
             filename=executable,
             flatten_upload_paths=flatten_upload_paths,
@@ -979,26 +978,27 @@
                 flatten_upload_paths=flatten_upload_paths,
             ),
             verification=TaskInputVerification.VERIFY_AT_START,
         )
         # Avoid duplicate TaskInputs
         if task_input.objectNamePattern not in [x.objectNamePattern for x in inputs]:
             inputs.append(task_input)
+        executable_pathname = unique_upload_pathname(
+            filename=executable,
+            id=ID,
+            inputs_folder_name=INPUTS_FOLDER_NAME,
+            flatten_upload_paths=flatten_upload_paths,
+        )
+        if task_type in ["powershell", "cmd", "bat"]:
+            executable_pathname = executable_pathname.replace("/", "\\")
         args = [
-            (
-                unique_upload_pathname(
-                    filename=executable,
-                    id=ID,
-                    inputs_folder_name=INPUTS_FOLDER_NAME,
-                    flatten_upload_paths=flatten_upload_paths,
-                )
-                if flatten_input_paths is None
-                else basename(executable)
-            )
+            executable_pathname if flatten_input_paths is None else basename(executable)
         ] + args
+        if task_type in ["cmd", "bat"]:
+            args.insert(0, "/c")
         return _make_task(flatten_input_paths)
 
     # Special processing for Docker tasks if the 'executable property is set.
     # Sets up the '-e' environment strings and the DockerHub username and
     # password if specified.
     elif task_type == "docker":
         if executable is None:
```

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/submit_utils.py` & `yellowdog-python-examples-6.0.1/yd_commands/submit_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/terminate.py` & `yellowdog-python-examples-6.0.1/yd_commands/terminate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/type_check.py` & `yellowdog-python-examples-6.0.1/yd_commands/type_check.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/upload.py` & `yellowdog-python-examples-6.0.1/yd_commands/upload.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/upload_utils.py` & `yellowdog-python-examples-6.0.1/yd_commands/upload_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/validate_properties.py` & `yellowdog-python-examples-6.0.1/yd_commands/validate_properties.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/variables.py` & `yellowdog-python-examples-6.0.1/yd_commands/variables.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/version.py` & `yellowdog-python-examples-6.0.1/yd_commands/version.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yd_commands/wrapper.py` & `yellowdog-python-examples-6.0.1/yd_commands/wrapper.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/PKG-INFO` & `yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 6.0.0
+Version: 6.0.1
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/SOURCES.txt` & `yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/entry_points.txt` & `yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/entry_points.txt`

 * *Files identical despite different names*

