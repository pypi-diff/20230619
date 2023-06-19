# Comparing `tmp/netbox-cisco-support-plugin-0.0.2.tar.gz` & `tmp/netbox-cisco-support-plugin-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-cisco-support-plugin-0.0.2.tar", last modified: Mon Jun 19 16:05:31 2023, max compression
+gzip compressed data, was "netbox-cisco-support-plugin-0.0.3.tar", last modified: Mon Jun 19 16:14:56 2023, max compression
```

## Comparing `netbox-cisco-support-plugin-0.0.2.tar` & `netbox-cisco-support-plugin-0.0.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.923740 netbox-cisco-support-plugin-0.0.2/
--rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     5383 2023-06-19 16:05:31.923740 netbox-cisco-support-plugin-0.0.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4737 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.915740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (123)      645 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1665 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.919740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/api/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2424 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/api/serializers.py
--rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/api/urls.py
--rw-r--r--   0 vsts      (1001) docker     (123)      695 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/api/views.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4395 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/filtersets.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10150 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/forms.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.919740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/management/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.919740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    43543 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.919740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/
--rw-r--r--   0 vsts      (1001) docker     (123)     3497 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0001_initial.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0002_ciscodevicesupport_and_more.py
--rw-r--r--   0 vsts      (1001) docker     (123)      400 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0003_rename_model_ciscodevicesupport_pid.py
--rw-r--r--   0 vsts      (1001) docker     (123)      832 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0004_ciscodevicesupport_name_ciscodevicetypesupport_name_and_more.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1101 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0005_ciscodevicesupport_partner_coverage_end_date_and_more.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6845 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/models.py
--rw-r--r--   0 vsts      (1001) docker     (123)      350 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/navigation.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3925 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1844 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.915740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.919740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (123)     6722 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
--rw-r--r--   0 vsts      (1001) docker     (123)     3485 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
--rw-r--r--   0 vsts      (1001) docker     (123)      324 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/no_data_available.html
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.923740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2441 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1105 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/urls.py
--rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/version.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1739 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/views.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.919740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5383 2023-06-19 16:05:31.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1940 2023-06-19 16:05:31.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-19 16:05:31.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-19 16:05:31.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       28 2023-06-19 16:05:31.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-19 16:05:31.923740 netbox-cisco-support-plugin-0.0.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1568 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:14:56.307048 netbox-cisco-support-plugin-0.0.3/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     5383 2023-06-19 16:14:56.307048 netbox-cisco-support-plugin-0.0.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4737 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:14:56.303048 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)      645 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1665 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:14:56.307048 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/api/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2424 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/api/serializers.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/api/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      695 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/api/views.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4395 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/filtersets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10150 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/forms.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:14:56.307048 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/management/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:14:56.307048 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    43543 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:14:56.307048 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3497 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/migrations/0001_initial.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/migrations/0002_ciscodevicesupport_and_more.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      400 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/migrations/0003_rename_model_ciscodevicesupport_pid.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      832 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/migrations/0004_ciscodevicesupport_name_ciscodevicetypesupport_name_and_more.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1101 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/migrations/0005_ciscodevicesupport_partner_coverage_end_date_and_more.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6845 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      350 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/navigation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3925 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1844 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:14:56.303048 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:14:56.307048 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6682 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     3490 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      324 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/no_data_available.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:14:56.307048 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2441 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1105 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1739 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/views.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:14:56.307048 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5383 2023-06-19 16:14:56.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1940 2023-06-19 16:14:56.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-19 16:14:56.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-19 16:14:56.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       28 2023-06-19 16:14:56.000000 netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-19 16:14:56.307048 netbox-cisco-support-plugin-0.0.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1568 2023-06-19 16:14:38.000000 netbox-cisco-support-plugin-0.0.3/setup.py
```

### Comparing `netbox-cisco-support-plugin-0.0.2/LICENSE` & `netbox-cisco-support-plugin-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/PKG-INFO` & `netbox-cisco-support-plugin-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-support-plugin
-Version: 0.0.2
+Version: 0.0.3
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-support-plugin-0.0.2/README.md` & `netbox-cisco-support-plugin-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/__init__.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/admin.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/api/serializers.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/api/views.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/filtersets.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/forms.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0001_initial.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0002_ciscodevicesupport_and_more.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/migrations/0002_ciscodevicesupport_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0004_ciscodevicesupport_name_ciscodevicetypesupport_name_and_more.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/migrations/0004_ciscodevicesupport_name_ciscodevicetypesupport_name_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0005_ciscodevicesupport_partner_coverage_end_date_and_more.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/migrations/0005_ciscodevicesupport_partner_coverage_end_date_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/models.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/models.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/tables.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/template_content.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html`

 * *Files 0% similar despite different names*

```diff
@@ -83,17 +83,15 @@
                         <tr {{ cisco_device_support.warranty_type|coverage_class }}>
                             <td>Warranty Type</td>
                             <td colspan="2">{{ cisco_device_support.warranty_type }}</td>
                         </tr>
                 </tbody>
             </table>
 
-            {% if not cisco_device_support.contract_supplier or
-                    "Cisco SNTC" in cisco_device_support.contract_supplier or
-                    "Not covered by any contract" in cisco_device_support.contract_supplier %}
+            {% if not cisco_device_support.contract_supplier or "Cisco SNTC" in cisco_device_support.contract_supplier or "Not covered by any contract" in cisco_device_support.contract_supplier %}
                 {# Comment: Omit the partner support contract table #}
             {% else %}
                 <h5 class="card-header" style="padding:16px 0px 16px 0px">{{ cisco_device_support.contract_supplier }} Device Support</h5>
 
                 <table class="table table-hover panel-body attr-table">
                     <tbody>
                         <tr {{ cisco_device_support.partner_status|coverage_class }}>
```

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <div class="card">
 
     <h5 class="card-header">Cisco Device Type Support</h5>
 
     <div class="card-body">
 
-        {% if not cisco_device_support %}
+        {% if not cisco_device_type_support %}
             {% include "netbox_cisco_support_plugin/no_data_available.html" %}
         {% else %}
             <table class="table table-hover panel-body attr-table">
                 <tbody>
                     {% if cisco_device_type_support.eox_announcement_date %}
                         <tr {{ cisco_device_type_support.eox_announcement_date|expiration_class }}>
                             <td style="width: 40%">EoX Announcement Date</td>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 {% load filters %}
 ** Cisco Device Type Support **
-{% if not cisco_device_support %} {% include "netbox_cisco_support_plugin/
+{% if not cisco_device_type_support %} {% include "netbox_cisco_support_plugin/
 no_data_available.html" %} {% else %}
 Last updated: {{ cisco_device_type_support.last_updated }}
 {% endif %}
```

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templatetags/filters.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/urls.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/views.py` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin/views.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/PKG-INFO` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-support-plugin
-Version: 0.0.2
+Version: 0.0.3
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/SOURCES.txt` & `netbox-cisco-support-plugin-0.0.3/netbox_cisco_support_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.2/setup.py` & `netbox-cisco-support-plugin-0.0.3/setup.py`

 * *Files identical despite different names*

