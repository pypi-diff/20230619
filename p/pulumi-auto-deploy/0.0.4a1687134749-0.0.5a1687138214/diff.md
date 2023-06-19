# Comparing `tmp/pulumi_auto_deploy-0.0.4a1687134749.tar.gz` & `tmp/pulumi_auto_deploy-0.0.5a1687138214.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_auto_deploy-0.0.4a1687134749.tar", last modified: Mon Jun 19 00:35:21 2023, max compression
+gzip compressed data, was "dist/pulumi_auto_deploy-0.0.5a1687138214.tar", last modified: Mon Jun 19 01:32:35 2023, max compression
```

## Comparing `pulumi_auto_deploy-0.0.4a1687134749.tar` & `pulumi_auto_deploy-0.0.5a1687138214.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:35:21.000000 pulumi_auto_deploy-0.0.4a1687134749/
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-19 00:35:21.000000 pulumi_auto_deploy-0.0.4a1687134749/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-19 00:35:19.000000 pulumi_auto_deploy-0.0.4a1687134749/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:35:21.000000 pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy/
--rw-------   0 runner    (1001) docker     (123)      654 2023-06-19 00:35:19.000000 pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy/__init__.py
--rw-------   0 runner    (1001) docker     (123)     8047 2023-06-19 00:35:19.000000 pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy/_utilities.py
--rw-------   0 runner    (1001) docker     (123)     8953 2023-06-19 00:35:19.000000 pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy/auto_deployer.py
--rw-------   0 runner    (1001) docker     (123)     2731 2023-06-19 00:35:19.000000 pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy/provider.py
--rw-------   0 runner    (1001) docker     (123)       48 2023-06-19 00:35:19.000000 pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)        0 2023-06-19 00:35:19.000000 pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:35:21.000000 pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-19 00:35:21.000000 pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-19 00:35:21.000000 pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 00:35:21.000000 pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 00:35:21.000000 pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-19 00:35:21.000000 pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 00:35:21.000000 pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 00:35:21.000000 pulumi_auto_deploy-0.0.4a1687134749/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     1862 2023-06-19 00:35:19.000000 pulumi_auto_deploy-0.0.4a1687134749/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:32:35.000000 pulumi_auto_deploy-0.0.5a1687138214/
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-19 01:32:35.000000 pulumi_auto_deploy-0.0.5a1687138214/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-19 01:32:34.000000 pulumi_auto_deploy-0.0.5a1687138214/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:32:35.000000 pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy/
+-rw-------   0 runner    (1001) docker     (123)      654 2023-06-19 01:32:34.000000 pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     8047 2023-06-19 01:32:34.000000 pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)     8953 2023-06-19 01:32:34.000000 pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy/auto_deployer.py
+-rw-------   0 runner    (1001) docker     (123)     2731 2023-06-19 01:32:34.000000 pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy/provider.py
+-rw-------   0 runner    (1001) docker     (123)       48 2023-06-19 01:32:34.000000 pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)        0 2023-06-19 01:32:34.000000 pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:32:35.000000 pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-19 01:32:35.000000 pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-19 01:32:35.000000 pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 01:32:35.000000 pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 01:32:35.000000 pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-19 01:32:35.000000 pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 01:32:35.000000 pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 01:32:35.000000 pulumi_auto_deploy-0.0.5a1687138214/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     1862 2023-06-19 01:32:34.000000 pulumi_auto_deploy-0.0.5a1687138214/setup.py
```

### Comparing `pulumi_auto_deploy-0.0.4a1687134749/PKG-INFO` & `pulumi_auto_deploy-0.0.5a1687138214/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_auto_deploy
-Version: 0.0.4a1687134749
+Version: 0.0.5a1687138214
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Pulumi Auto Deploy
         
         [![Slack](https://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fauto-deploy.svg)](https://www.npmjs.com/package/@pulumi/auto-deploy)
```

### Comparing `pulumi_auto_deploy-0.0.4a1687134749/README.md` & `pulumi_auto_deploy-0.0.5a1687138214/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy/__init__.py` & `pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy/_utilities.py` & `pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy/auto_deployer.py` & `pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy/auto_deployer.py`

 * *Files identical despite different names*

### Comparing `pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy/provider.py` & `pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_auto_deploy-0.0.4a1687134749/pulumi_auto_deploy.egg-info/PKG-INFO` & `pulumi_auto_deploy-0.0.5a1687138214/pulumi_auto_deploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-auto-deploy
-Version: 0.0.4a1687134749
+Version: 0.0.5a1687138214
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Pulumi Auto Deploy
         
         [![Slack](https://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fauto-deploy.svg)](https://www.npmjs.com/package/@pulumi/auto-deploy)
```

### Comparing `pulumi_auto_deploy-0.0.4a1687134749/setup.py` & `pulumi_auto_deploy-0.0.5a1687138214/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.4a1687134749"
-PLUGIN_VERSION = "0.0.4-alpha.1687134749+cbad54cb"
+VERSION = "0.0.5a1687138214"
+PLUGIN_VERSION = "0.0.5-alpha.1687138214+3f6df2ed"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'auto-deploy', PLUGIN_VERSION])
         except OSError as error:
```

