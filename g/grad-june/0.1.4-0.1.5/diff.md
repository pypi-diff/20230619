# Comparing `tmp/grad_june-0.1.4.tar.gz` & `tmp/grad_june-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grad_june-0.1.4.tar", last modified: Thu Jun 15 13:59:20 2023, max compression
+gzip compressed data, was "grad_june-0.1.5.tar", last modified: Mon Jun 19 09:13:43 2023, max compression
```

## Comparing `grad_june-0.1.4.tar` & `grad_june-0.1.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:59:20.600081 grad_june-0.1.4/
--rw-r--r--   0 arnull     (504) staff       (20)     1077 2022-06-16 10:39:12.000000 grad_june-0.1.4/LICENSE
--rw-r--r--   0 arnull     (504) staff       (20)       25 2023-06-15 13:58:58.000000 grad_june-0.1.4/MANIFEST.in
--rw-r--r--   0 arnull     (504) staff       (20)     1059 2023-06-15 13:59:20.600159 grad_june-0.1.4/PKG-INFO
--rw-r--r--   0 arnull     (504) staff       (20)      748 2023-06-15 13:45:30.000000 grad_june-0.1.4/README.md
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:59:20.596940 grad_june-0.1.4/grad_june/
--rw-r--r--   0 arnull     (504) staff       (20)      368 2023-06-15 10:47:46.000000 grad_june-0.1.4/grad_june/__init__.py
--rw-r--r--   0 arnull     (504) staff       (20)      755 2023-01-20 11:11:57.000000 grad_june-0.1.4/grad_june/cuda_utils.py
--rw-r--r--   0 arnull     (504) staff       (20)     5931 2023-01-20 11:11:57.000000 grad_june-0.1.4/grad_june/default_parameters.py
--rw-r--r--   0 arnull     (504) staff       (20)     2601 2023-06-15 10:48:16.000000 grad_june-0.1.4/grad_june/infection.py
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:59:20.597913 grad_june-0.1.4/grad_june/infection_networks/
--rw-r--r--   0 arnull     (504) staff       (20)      315 2023-03-20 16:13:20.000000 grad_june-0.1.4/grad_june/infection_networks/__init__.py
--rw-r--r--   0 arnull     (504) staff       (20)     5657 2023-06-15 10:48:16.000000 grad_june-0.1.4/grad_june/infection_networks/base.py
--rw-r--r--   0 arnull     (504) staff       (20)     4166 2023-06-15 10:48:16.000000 grad_june-0.1.4/grad_june/infection_networks/leisure_network.py
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:59:20.599130 grad_june-0.1.4/grad_june/june_world_loader/
--rw-r--r--   0 arnull     (504) staff       (20)       85 2023-01-20 11:11:57.000000 grad_june-0.1.4/grad_june/june_world_loader/__init__.py
--rw-r--r--   0 arnull     (504) staff       (20)     1398 2023-01-20 11:11:57.000000 grad_june-0.1.4/grad_june/june_world_loader/agent_data_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)      184 2023-01-20 11:11:57.000000 grad_june-0.1.4/grad_june/june_world_loader/care_home_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)      178 2023-01-20 11:11:57.000000 grad_june-0.1.4/grad_june/june_world_loader/company_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)     1462 2023-01-20 11:11:57.000000 grad_june-0.1.4/grad_june/june_world_loader/graph_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)      184 2023-01-20 11:11:57.000000 grad_june-0.1.4/grad_june/june_world_loader/household_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)     4032 2023-03-20 13:17:17.000000 grad_june-0.1.4/grad_june/june_world_loader/leisure_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)     1624 2023-01-20 11:11:57.000000 grad_june-0.1.4/grad_june/june_world_loader/network_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)      175 2023-01-20 11:11:57.000000 grad_june-0.1.4/grad_june/june_world_loader/school_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)      188 2023-01-20 11:11:57.000000 grad_june-0.1.4/grad_june/june_world_loader/university_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)     5414 2023-06-15 10:48:16.000000 grad_june-0.1.4/grad_june/model.py
--rw-r--r--   0 arnull     (504) staff       (20)      194 2023-06-15 13:49:23.000000 grad_june-0.1.4/grad_june/paths.py
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:59:20.599732 grad_june-0.1.4/grad_june/policies/
--rw-r--r--   0 arnull     (504) staff       (20)      258 2023-01-20 11:11:57.000000 grad_june-0.1.4/grad_june/policies/__init__.py
--rw-r--r--   0 arnull     (504) staff       (20)      757 2023-04-18 17:56:26.000000 grad_june-0.1.4/grad_june/policies/close_venue_policies.py
--rw-r--r--   0 arnull     (504) staff       (20)     1027 2023-06-15 10:47:46.000000 grad_june-0.1.4/grad_june/policies/interaction_policies.py
--rw-r--r--   0 arnull     (504) staff       (20)     4073 2023-03-20 11:51:45.000000 grad_june-0.1.4/grad_june/policies/policies.py
--rw-r--r--   0 arnull     (504) staff       (20)     1097 2023-01-20 11:11:57.000000 grad_june-0.1.4/grad_june/policies/quarantine_policies.py
--rw-r--r--   0 arnull     (504) staff       (20)     9423 2023-06-15 10:48:16.000000 grad_june-0.1.4/grad_june/runner.py
--rw-r--r--   0 arnull     (504) staff       (20)     9981 2023-06-15 10:48:16.000000 grad_june-0.1.4/grad_june/symptoms.py
--rw-r--r--   0 arnull     (504) staff       (20)     4579 2023-01-20 11:11:57.000000 grad_june-0.1.4/grad_june/timer.py
--rw-r--r--   0 arnull     (504) staff       (20)     1877 2023-06-15 10:48:16.000000 grad_june-0.1.4/grad_june/transmission.py
--rw-r--r--   0 arnull     (504) staff       (20)     4572 2023-06-15 10:48:16.000000 grad_june-0.1.4/grad_june/utils.py
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:59:20.597541 grad_june-0.1.4/grad_june.egg-info/
--rw-r--r--   0 arnull     (504) staff       (20)     1059 2023-06-15 13:59:20.000000 grad_june-0.1.4/grad_june.egg-info/PKG-INFO
--rw-r--r--   0 arnull     (504) staff       (20)     1285 2023-06-15 13:59:20.000000 grad_june-0.1.4/grad_june.egg-info/SOURCES.txt
--rw-r--r--   0 arnull     (504) staff       (20)        1 2023-06-15 13:59:20.000000 grad_june-0.1.4/grad_june.egg-info/dependency_links.txt
--rw-r--r--   0 arnull     (504) staff       (20)       94 2023-06-15 13:59:20.000000 grad_june-0.1.4/grad_june.egg-info/requires.txt
--rw-r--r--   0 arnull     (504) staff       (20)       15 2023-06-15 13:59:20.000000 grad_june-0.1.4/grad_june.egg-info/top_level.txt
--rw-r--r--   0 arnull     (504) staff       (20)       94 2023-06-15 13:30:05.000000 grad_june-0.1.4/requirements.txt
--rw-r--r--   0 arnull     (504) staff       (20)      126 2023-06-15 13:59:20.600436 grad_june-0.1.4/setup.cfg
--rw-r--r--   0 arnull     (504) staff       (20)      891 2023-06-15 13:59:06.000000 grad_june-0.1.4/setup.py
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:59:20.599971 grad_june-0.1.4/test/
--rw-r--r--   0 arnull     (504) staff       (20)        0 2022-06-16 10:39:12.000000 grad_june-0.1.4/test/__init__.py
--rw-r--r--   0 arnull     (504) staff       (20)     3869 2023-06-15 10:48:16.000000 grad_june-0.1.4/test/conftest.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-19 09:13:43.534114 grad_june-0.1.5/
+-rw-r--r--   0 arnull     (504) staff       (20)     1077 2022-06-16 10:39:12.000000 grad_june-0.1.5/LICENSE
+-rw-r--r--   0 arnull     (504) staff       (20)       25 2023-06-15 13:58:58.000000 grad_june-0.1.5/MANIFEST.in
+-rw-r--r--   0 arnull     (504) staff       (20)     1071 2023-06-19 09:13:43.534218 grad_june-0.1.5/PKG-INFO
+-rw-r--r--   0 arnull     (504) staff       (20)      760 2023-06-15 14:01:42.000000 grad_june-0.1.5/README.md
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-19 09:13:43.530952 grad_june-0.1.5/grad_june/
+-rw-r--r--   0 arnull     (504) staff       (20)      368 2023-06-15 10:47:46.000000 grad_june-0.1.5/grad_june/__init__.py
+-rw-r--r--   0 arnull     (504) staff       (20)      755 2023-01-20 11:11:57.000000 grad_june-0.1.5/grad_june/cuda_utils.py
+-rw-r--r--   0 arnull     (504) staff       (20)     5931 2023-01-20 11:11:57.000000 grad_june-0.1.5/grad_june/default_parameters.py
+-rw-r--r--   0 arnull     (504) staff       (20)     2601 2023-06-15 10:48:16.000000 grad_june-0.1.5/grad_june/infection.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-19 09:13:43.531874 grad_june-0.1.5/grad_june/infection_networks/
+-rw-r--r--   0 arnull     (504) staff       (20)      315 2023-03-20 16:13:20.000000 grad_june-0.1.5/grad_june/infection_networks/__init__.py
+-rw-r--r--   0 arnull     (504) staff       (20)     5657 2023-06-15 10:48:16.000000 grad_june-0.1.5/grad_june/infection_networks/base.py
+-rw-r--r--   0 arnull     (504) staff       (20)     4166 2023-06-15 10:48:16.000000 grad_june-0.1.5/grad_june/infection_networks/leisure_network.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-19 09:13:43.533121 grad_june-0.1.5/grad_june/june_world_loader/
+-rw-r--r--   0 arnull     (504) staff       (20)       85 2023-01-20 11:11:57.000000 grad_june-0.1.5/grad_june/june_world_loader/__init__.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1398 2023-01-20 11:11:57.000000 grad_june-0.1.5/grad_june/june_world_loader/agent_data_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)      184 2023-01-20 11:11:57.000000 grad_june-0.1.5/grad_june/june_world_loader/care_home_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)      178 2023-01-20 11:11:57.000000 grad_june-0.1.5/grad_june/june_world_loader/company_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1462 2023-01-20 11:11:57.000000 grad_june-0.1.5/grad_june/june_world_loader/graph_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)      184 2023-01-20 11:11:57.000000 grad_june-0.1.5/grad_june/june_world_loader/household_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)     4032 2023-03-20 13:17:17.000000 grad_june-0.1.5/grad_june/june_world_loader/leisure_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1624 2023-01-20 11:11:57.000000 grad_june-0.1.5/grad_june/june_world_loader/network_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)      175 2023-01-20 11:11:57.000000 grad_june-0.1.5/grad_june/june_world_loader/school_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)      188 2023-01-20 11:11:57.000000 grad_june-0.1.5/grad_june/june_world_loader/university_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)     5414 2023-06-15 10:48:16.000000 grad_june-0.1.5/grad_june/model.py
+-rw-r--r--   0 arnull     (504) staff       (20)      194 2023-06-15 13:49:23.000000 grad_june-0.1.5/grad_june/paths.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-19 09:13:43.533722 grad_june-0.1.5/grad_june/policies/
+-rw-r--r--   0 arnull     (504) staff       (20)      258 2023-01-20 11:11:57.000000 grad_june-0.1.5/grad_june/policies/__init__.py
+-rw-r--r--   0 arnull     (504) staff       (20)      757 2023-04-18 17:56:26.000000 grad_june-0.1.5/grad_june/policies/close_venue_policies.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1027 2023-06-15 10:47:46.000000 grad_june-0.1.5/grad_june/policies/interaction_policies.py
+-rw-r--r--   0 arnull     (504) staff       (20)     4073 2023-03-20 11:51:45.000000 grad_june-0.1.5/grad_june/policies/policies.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1097 2023-01-20 11:11:57.000000 grad_june-0.1.5/grad_june/policies/quarantine_policies.py
+-rw-r--r--   0 arnull     (504) staff       (20)     9423 2023-06-15 10:48:16.000000 grad_june-0.1.5/grad_june/runner.py
+-rw-r--r--   0 arnull     (504) staff       (20)     9981 2023-06-15 10:48:16.000000 grad_june-0.1.5/grad_june/symptoms.py
+-rw-r--r--   0 arnull     (504) staff       (20)     4579 2023-01-20 11:11:57.000000 grad_june-0.1.5/grad_june/timer.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1877 2023-06-15 10:48:16.000000 grad_june-0.1.5/grad_june/transmission.py
+-rw-r--r--   0 arnull     (504) staff       (20)     4572 2023-06-15 10:48:16.000000 grad_june-0.1.5/grad_june/utils.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-19 09:13:43.531518 grad_june-0.1.5/grad_june.egg-info/
+-rw-r--r--   0 arnull     (504) staff       (20)     1071 2023-06-19 09:13:43.000000 grad_june-0.1.5/grad_june.egg-info/PKG-INFO
+-rw-r--r--   0 arnull     (504) staff       (20)     1285 2023-06-19 09:13:43.000000 grad_june-0.1.5/grad_june.egg-info/SOURCES.txt
+-rw-r--r--   0 arnull     (504) staff       (20)        1 2023-06-19 09:13:43.000000 grad_june-0.1.5/grad_june.egg-info/dependency_links.txt
+-rw-r--r--   0 arnull     (504) staff       (20)       94 2023-06-19 09:13:43.000000 grad_june-0.1.5/grad_june.egg-info/requires.txt
+-rw-r--r--   0 arnull     (504) staff       (20)       15 2023-06-19 09:13:43.000000 grad_june-0.1.5/grad_june.egg-info/top_level.txt
+-rw-r--r--   0 arnull     (504) staff       (20)       94 2023-06-15 13:30:05.000000 grad_june-0.1.5/requirements.txt
+-rw-r--r--   0 arnull     (504) staff       (20)      126 2023-06-19 09:13:43.534498 grad_june-0.1.5/setup.cfg
+-rw-r--r--   0 arnull     (504) staff       (20)      891 2023-06-19 09:13:29.000000 grad_june-0.1.5/setup.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-19 09:13:43.533926 grad_june-0.1.5/test/
+-rw-r--r--   0 arnull     (504) staff       (20)        0 2022-06-16 10:39:12.000000 grad_june-0.1.5/test/__init__.py
+-rw-r--r--   0 arnull     (504) staff       (20)     3869 2023-06-15 10:48:16.000000 grad_june-0.1.5/test/conftest.py
```

### Comparing `grad_june-0.1.4/LICENSE` & `grad_june-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/PKG-INFO` & `grad_june-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grad_june
-Version: 0.1.4
+Version: 0.1.5
 Summary: Differentiable implementation of the JUNE model.
 Home-page: https://github.com/arnauqb/GradABM-JUNE
 Author: Arnau Quera-Bofarull
 Author-email: arnauq@protonmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,13 +17,13 @@
 Implementation of the JUNE model using the GradABM framework.
 
 # Setup 
 
 The easiest way is to install the package from the PyPI package repository
 
 ```
-pip install 
-
+pip install grad-june
+```
 
 # Usage
 
 See the [docs](https://arnauqb.github.io/GradABM-JUNE/).
```

### Comparing `grad_june-0.1.4/README.md` & `grad_june-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 Implementation of the JUNE model using the GradABM framework.
 
 # Setup 
 
 The easiest way is to install the package from the PyPI package repository
 
 ```
-pip install 
-
+pip install grad-june
+```
 
 # Usage
 
 See the [docs](https://arnauqb.github.io/GradABM-JUNE/).
```

### Comparing `grad_june-0.1.4/grad_june/cuda_utils.py` & `grad_june-0.1.5/grad_june/cuda_utils.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/default_parameters.py` & `grad_june-0.1.5/grad_june/default_parameters.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/infection.py` & `grad_june-0.1.5/grad_june/infection.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/infection_networks/base.py` & `grad_june-0.1.5/grad_june/infection_networks/base.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/infection_networks/leisure_network.py` & `grad_june-0.1.5/grad_june/infection_networks/leisure_network.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/june_world_loader/agent_data_loader.py` & `grad_june-0.1.5/grad_june/june_world_loader/agent_data_loader.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/june_world_loader/graph_loader.py` & `grad_june-0.1.5/grad_june/june_world_loader/graph_loader.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/june_world_loader/leisure_loader.py` & `grad_june-0.1.5/grad_june/june_world_loader/leisure_loader.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/june_world_loader/network_loader.py` & `grad_june-0.1.5/grad_june/june_world_loader/network_loader.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/model.py` & `grad_june-0.1.5/grad_june/model.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/policies/close_venue_policies.py` & `grad_june-0.1.5/grad_june/policies/close_venue_policies.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/policies/interaction_policies.py` & `grad_june-0.1.5/grad_june/policies/interaction_policies.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/policies/policies.py` & `grad_june-0.1.5/grad_june/policies/policies.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/policies/quarantine_policies.py` & `grad_june-0.1.5/grad_june/policies/quarantine_policies.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/runner.py` & `grad_june-0.1.5/grad_june/runner.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/symptoms.py` & `grad_june-0.1.5/grad_june/symptoms.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/timer.py` & `grad_june-0.1.5/grad_june/timer.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/transmission.py` & `grad_june-0.1.5/grad_june/transmission.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june/utils.py` & `grad_june-0.1.5/grad_june/utils.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/grad_june.egg-info/PKG-INFO` & `grad_june-0.1.5/grad_june.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grad-june
-Version: 0.1.4
+Version: 0.1.5
 Summary: Differentiable implementation of the JUNE model.
 Home-page: https://github.com/arnauqb/GradABM-JUNE
 Author: Arnau Quera-Bofarull
 Author-email: arnauq@protonmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,13 +17,13 @@
 Implementation of the JUNE model using the GradABM framework.
 
 # Setup 
 
 The easiest way is to install the package from the PyPI package repository
 
 ```
-pip install 
-
+pip install grad-june
+```
 
 # Usage
 
 See the [docs](https://arnauqb.github.io/GradABM-JUNE/).
```

### Comparing `grad_june-0.1.4/grad_june.egg-info/SOURCES.txt` & `grad_june-0.1.5/grad_june.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.4/setup.py` & `grad_june-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
 
 setup(
     name="grad_june",
-    version="0.1.4",
+    version="0.1.5",
     description="Differentiable implementation of the JUNE model.",
     url="https://github.com/arnauqb/GradABM-JUNE",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="Arnau Quera-Bofarull",
     author_email="arnauq@protonmail.com",
     license="MIT License",
```

### Comparing `grad_june-0.1.4/test/conftest.py` & `grad_june-0.1.5/test/conftest.py`

 * *Files identical despite different names*

