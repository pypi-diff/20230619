# Comparing `tmp/netbox-cisco-support-plugin-0.0.1.tar.gz` & `tmp/netbox-cisco-support-plugin-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-cisco-support-plugin-0.0.1.tar", last modified: Mon Jun 19 15:50:59 2023, max compression
+gzip compressed data, was "netbox-cisco-support-plugin-0.0.2.tar", last modified: Mon Jun 19 16:05:31 2023, max compression
```

## Comparing `netbox-cisco-support-plugin-0.0.1.tar` & `netbox-cisco-support-plugin-0.0.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 15:50:59.125193 netbox-cisco-support-plugin-0.0.1/
--rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     5383 2023-06-19 15:50:59.125193 netbox-cisco-support-plugin-0.0.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4737 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 15:50:59.121193 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (123)      645 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1665 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 15:50:59.121193 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/api/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2424 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/api/serializers.py
--rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/api/urls.py
--rw-r--r--   0 vsts      (1001) docker     (123)      695 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/api/views.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4395 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/filtersets.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10150 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/forms.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 15:50:59.121193 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/management/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 15:50:59.121193 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    43543 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 15:50:59.125193 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/migrations/
--rw-r--r--   0 vsts      (1001) docker     (123)     3497 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/migrations/0001_initial.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/migrations/0002_ciscodevicesupport_and_more.py
--rw-r--r--   0 vsts      (1001) docker     (123)      400 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/migrations/0003_rename_model_ciscodevicesupport_pid.py
--rw-r--r--   0 vsts      (1001) docker     (123)      832 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/migrations/0004_ciscodevicesupport_name_ciscodevicetypesupport_name_and_more.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1101 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/migrations/0005_ciscodevicesupport_partner_coverage_end_date_and_more.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6845 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/models.py
--rw-r--r--   0 vsts      (1001) docker     (123)      350 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/navigation.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3925 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1844 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 15:50:59.117193 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 15:50:59.125193 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (123)     6556 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
--rw-r--r--   0 vsts      (1001) docker     (123)     3364 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
--rw-r--r--   0 vsts      (1001) docker     (123)      186 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/no_data_available.html
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 15:50:59.125193 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2441 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1105 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/urls.py
--rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/version.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1739 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/views.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 15:50:59.121193 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5383 2023-06-19 15:50:59.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1940 2023-06-19 15:50:59.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-19 15:50:59.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-19 15:50:58.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       28 2023-06-19 15:50:59.000000 netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-19 15:50:59.125193 netbox-cisco-support-plugin-0.0.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1568 2023-06-19 15:50:39.000000 netbox-cisco-support-plugin-0.0.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.923740 netbox-cisco-support-plugin-0.0.2/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     5383 2023-06-19 16:05:31.923740 netbox-cisco-support-plugin-0.0.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4737 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.915740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)      645 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1665 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.919740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/api/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2424 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/api/serializers.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/api/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      695 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/api/views.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4395 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/filtersets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10150 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/forms.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.919740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/management/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.919740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    43543 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.919740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3497 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0001_initial.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0002_ciscodevicesupport_and_more.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      400 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0003_rename_model_ciscodevicesupport_pid.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      832 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0004_ciscodevicesupport_name_ciscodevicetypesupport_name_and_more.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1101 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0005_ciscodevicesupport_partner_coverage_end_date_and_more.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6845 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      350 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/navigation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3925 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1844 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.915740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.919740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6722 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     3485 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      324 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/no_data_available.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.923740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2441 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1105 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1739 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/views.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-19 16:05:31.919740 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5383 2023-06-19 16:05:31.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1940 2023-06-19 16:05:31.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-19 16:05:31.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-19 16:05:31.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       28 2023-06-19 16:05:31.000000 netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-19 16:05:31.923740 netbox-cisco-support-plugin-0.0.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1568 2023-06-19 16:05:13.000000 netbox-cisco-support-plugin-0.0.2/setup.py
```

### Comparing `netbox-cisco-support-plugin-0.0.1/LICENSE` & `netbox-cisco-support-plugin-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/PKG-INFO` & `netbox-cisco-support-plugin-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-support-plugin
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-support-plugin-0.0.1/README.md` & `netbox-cisco-support-plugin-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/__init__.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/admin.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/api/serializers.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/api/views.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/filtersets.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/forms.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/migrations/0001_initial.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/migrations/0002_ciscodevicesupport_and_more.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0002_ciscodevicesupport_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/migrations/0004_ciscodevicesupport_name_ciscodevicetypesupport_name_and_more.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0004_ciscodevicesupport_name_ciscodevicetypesupport_name_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/migrations/0005_ciscodevicesupport_partner_coverage_end_date_and_more.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/migrations/0005_ciscodevicesupport_partner_coverage_end_date_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/models.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/models.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/tables.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/template_content.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 {% load filters %}
 
 <div class="card">
 
     <h5 class="card-header">Cisco Software Release</h5>
 
     <div class="card-body">
-        
-        <table class="table table-hover panel-body attr-table">
-            <tbody>
-                {% if not cisco_device_support %}
-                    {% include "netbox_cisco_support_plugin/no_data_available.html" %}
-                {% else %}
+
+        {% if not cisco_device_support %}
+            {% include "netbox_cisco_support_plugin/no_data_available.html" %}
+        {% else %}
+            <table class="table table-hover panel-body attr-table">
+                <tbody>
                     <tr {{ cisco_device_support.recommended_release|coverage_class }} >
                         <td style="width: 40%">Recommended Release</td>
                         <td colspan="2">{{ cisco_device_support.recommended_release|linebreaks }}</td>
                     </tr>
                     {% if "PID without Cisco software" in cisco_device_support.recommended_release %}
                         {# Comment: If PID have no Cisco software omit the desired and current release #}
                     {% else %}
@@ -25,103 +25,101 @@
                         </tr>
                         <tr {{ cisco_device_support.current_release_status|current_release_status_class }}>
                             <td>Current Release</td>
                             <td style="width: 40px"><i {{ cisco_device_support.current_release_status|coverage_class_boolian }}></i></td>
                             <td>{{ cisco_device_support.current_release }}</td>
                         </tr>
                     {% endif %}
-                {% endif %}
-            </tbody>
-        </table>
+                </tbody>
+            </table>
 
-        {% if cisco_device_support %}
             <div class="text-muted">Last updated: {{ cisco_device_support.last_updated }}</div>
         {% endif %}
 
     </div>
 
 </div>
 
 <div class="card">
 
     <div class="card-body">
 
         <h5 class="card-header" style="padding:0px 0px 16px 0px">Cisco Device Support</h5>
 
-        <table class="table table-hover panel-body attr-table">
-            <tbody>
-                {% if not cisco_device_support %}
-                    {% include "netbox_cisco_support_plugin/no_data_available.html" %}
-                {% else %}
-                    <tr {{ cisco_device_support.sr_no_owner|coverage_class }}>
-                        <td style="width: 40%">Is associated with a Cisco ID</td>
-                        <td style="width: 40px"><i {{ cisco_device_support.sr_no_owner|coverage_class_boolian }}></i></td>
-                        <td>{{ cisco_device_support.api_status }}</td>
-                    </tr>
-                    <tr {{ cisco_device_support.is_covered|coverage_class }}>
-                        <td>Contract Status</td>
-                        <td><i {{ cisco_device_support.contract_supplier|coverage_class_boolian }}></i></td>
-                        <td>Covered by: {{ cisco_device_support.contract_supplier }}</td>
-                    </tr>
-                    <tr {{ cisco_device_support.is_covered|coverage_class }}>
-                        <td>Is under Cisco Support?</td>
-                        <td colspan="2"><i {{ cisco_device_support.is_covered|coverage_class_boolian }}></i></td>
-                    </tr>
-                    <tr {{ cisco_device_support.coverage_end_date|expiration_class }}>
-                        <td>Contract Coverage End Date</td>
-                        <td colspan="2">{{ cisco_device_support.coverage_end_date }}</td>
-                    </tr>
-                    <tr {{ cisco_device_support.service_line_descr|coverage_class }}>
-                        <td>Service Level Description</td>
-                        <td colspan="2">{{ cisco_device_support.service_line_descr }}</td>
-                    </tr>
-                    <tr {{ cisco_device_support.service_contract_number|coverage_class }}>
-                        <td>Service Contract Number</td>
-                        <td colspan="2">{{ cisco_device_support.service_contract_number }}</td>
-                    </tr>
-                    <tr {{ cisco_device_support.warranty_end_date|expiration_class }}>
-                        <td>Warranty End Date</td>
-                        <td colspan="2">{{ cisco_device_support.warranty_end_date }}</td>
-                    </tr>
-                    <tr {{ cisco_device_support.warranty_type|coverage_class }}>
-                        <td>Warranty Type</td>
-                        <td colspan="2">{{ cisco_device_support.warranty_type }}</td>
-                    </tr>
-                {% endif %}
-            </tbody>
-        </table>
-
-        {% if "Cisco SNTC" in cisco_device_support.contract_supplier or "Not covered by any contract" in cisco_device_support.contract_supplier %}
-            {# Comment: Omit the partner support contract table #}
+        {% if not cisco_device_support %}
+            {% include "netbox_cisco_support_plugin/no_data_available.html" %}
         {% else %}
-            <h5 class="card-header" style="padding:16px 0px 16px 0px">{{ cisco_device_support.contract_supplier }} Device Support</h5>
-
             <table class="table table-hover panel-body attr-table">
                 <tbody>
-                    <tr {{ cisco_device_support.partner_status|coverage_class }}>
-                        <td style="width: 40%">Contract Status</td>
-                        <td>{{ cisco_device_support.partner_status }}</td>
-                    </tr>
-                    <tr {{ cisco_device_support.partner_coverage_end_date|expiration_class }}>
-                        <td>Contract Coverage End Date</td>
-                        <td>{{ cisco_device_support.partner_coverage_end_date }}</td>
-                    </tr>
-                    <tr {{ cisco_device_support.partner_service_level|coverage_class }}>
-                        <td>Service Level Description</td>
-                        <td>{{ cisco_device_support.partner_service_level }}</td>
-                    </tr>
-                    <tr {{ cisco_device_support.partner_customer_number|coverage_class }}>
-                        <td>Customer Number</td>
-                        <td>{{ cisco_device_support.partner_customer_number }}</td>
-                    </tr>
+                        <tr {{ cisco_device_support.sr_no_owner|coverage_class }}>
+                            <td style="width: 40%">Is associated with a Cisco ID</td>
+                            <td style="width: 40px"><i {{ cisco_device_support.sr_no_owner|coverage_class_boolian }}></i></td>
+                            <td>{{ cisco_device_support.api_status }}</td>
+                        </tr>
+                        <tr {{ cisco_device_support.is_covered|coverage_class }}>
+                            <td>Contract Status</td>
+                            <td><i {{ cisco_device_support.contract_supplier|coverage_class_boolian }}></i></td>
+                            <td>Covered by: {{ cisco_device_support.contract_supplier }}</td>
+                        </tr>
+                        <tr {{ cisco_device_support.is_covered|coverage_class }}>
+                            <td>Is under Cisco Support?</td>
+                            <td colspan="2"><i {{ cisco_device_support.is_covered|coverage_class_boolian }}></i></td>
+                        </tr>
+                        <tr {{ cisco_device_support.coverage_end_date|expiration_class }}>
+                            <td>Contract Coverage End Date</td>
+                            <td colspan="2">{{ cisco_device_support.coverage_end_date }}</td>
+                        </tr>
+                        <tr {{ cisco_device_support.service_line_descr|coverage_class }}>
+                            <td>Service Level Description</td>
+                            <td colspan="2">{{ cisco_device_support.service_line_descr }}</td>
+                        </tr>
+                        <tr {{ cisco_device_support.service_contract_number|coverage_class }}>
+                            <td>Service Contract Number</td>
+                            <td colspan="2">{{ cisco_device_support.service_contract_number }}</td>
+                        </tr>
+                        <tr {{ cisco_device_support.warranty_end_date|expiration_class }}>
+                            <td>Warranty End Date</td>
+                            <td colspan="2">{{ cisco_device_support.warranty_end_date }}</td>
+                        </tr>
+                        <tr {{ cisco_device_support.warranty_type|coverage_class }}>
+                            <td>Warranty Type</td>
+                            <td colspan="2">{{ cisco_device_support.warranty_type }}</td>
+                        </tr>
                 </tbody>
             </table>
-        {% endif %}
 
-        {% if cisco_device_support %}
+            {% if not cisco_device_support.contract_supplier or
+                    "Cisco SNTC" in cisco_device_support.contract_supplier or
+                    "Not covered by any contract" in cisco_device_support.contract_supplier %}
+                {# Comment: Omit the partner support contract table #}
+            {% else %}
+                <h5 class="card-header" style="padding:16px 0px 16px 0px">{{ cisco_device_support.contract_supplier }} Device Support</h5>
+
+                <table class="table table-hover panel-body attr-table">
+                    <tbody>
+                        <tr {{ cisco_device_support.partner_status|coverage_class }}>
+                            <td style="width: 40%">Contract Status</td>
+                            <td>{{ cisco_device_support.partner_status }}</td>
+                        </tr>
+                        <tr {{ cisco_device_support.partner_coverage_end_date|expiration_class }}>
+                            <td>Contract Coverage End Date</td>
+                            <td>{{ cisco_device_support.partner_coverage_end_date }}</td>
+                        </tr>
+                        <tr {{ cisco_device_support.partner_service_level|coverage_class }}>
+                            <td>Service Level Description</td>
+                            <td>{{ cisco_device_support.partner_service_level }}</td>
+                        </tr>
+                        <tr {{ cisco_device_support.partner_customer_number|coverage_class }}>
+                            <td>Customer Number</td>
+                            <td>{{ cisco_device_support.partner_customer_number }}</td>
+                        </tr>
+                    </tbody>
+                </table>
+            {% endif %}
+
             <div class="text-muted">Last updated: {{ cisco_device_support.last_updated }}</div>
         {% endif %}
 
     </div>
 
 </div>
```

#### html2text {}

```diff
@@ -1,14 +1,18 @@
 {% load filters %}
 ** Cisco Software Release **
-{% if cisco_device_support %}
+{% if not cisco_device_support %} {% include "netbox_cisco_support_plugin/
+no_data_available.html" %} {% else %}
 Last updated: {{ cisco_device_support.last_updated }}
 {% endif %}
 ** Cisco Device Support **
-{% if "Cisco SNTC" in cisco_device_support.contract_supplier or "Not covered by
-any contract" in cisco_device_support.contract_supplier %} {# Comment: Omit the
-partner support contract table #} {% else %}
+{% if not cisco_device_support %} {% include "netbox_cisco_support_plugin/
+no_data_available.html" %} {% else %}
+{% if not cisco_device_support.contract_supplier or "Cisco SNTC" in
+cisco_device_support.contract_supplier or "Not covered by any contract" in
+cisco_device_support.contract_supplier %} {# Comment: Omit the partner support
+contract table #} {% else %}
 ** {{ cisco_device_support.contract_supplier }} Device Support **
-{% endif %} {% if cisco_device_support %}
+{% endif %}
 Last updated: {{ cisco_device_support.last_updated }}
 {% endif %}
 {% include "netbox_cisco_support_plugin/cisco_support_device_type.html" %}
```

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,61 +2,61 @@
 
 <div class="card">
 
     <h5 class="card-header">Cisco Device Type Support</h5>
 
     <div class="card-body">
 
-        <table class="table table-hover panel-body attr-table">
-            <tbody>
-                {% if not cisco_device_type_support %}
-                    {% include "netbox_cisco_support_plugin/no_data_available.html" %}
-                {% elif cisco_device_type_support.eox_announcement_date %}
-                    <tr {{ cisco_device_type_support.eox_announcement_date|expiration_class }}>
-                        <td style="width: 40%">EoX Announcement Date</td>
-                        <td>{{ cisco_device_type_support.eox_announcement_date }}</td>
-                    </tr>
-                    <tr {{ cisco_device_type_support.end_of_sale_date|expiration_class }}>
-                        <td>End-of-Sale Date</td>
-                        <td>{{ cisco_device_type_support.end_of_sale_date }}</td>
-                    </tr>
-                    <tr {{ cisco_device_type_support.end_of_sw_maintenance_releases|expiration_class }}>
-                        <td>End of SW Maintenance Releases Date</td>
-                        <td>{{ cisco_device_type_support.end_of_sw_maintenance_releases }}</td>
-                    </tr>
-                    <tr {{ cisco_device_type_support.end_of_routine_failure_analysis_date|expiration_class }}>
-                        <td>End of Routine Failure Analysis Date</td>
-                        <td>{{ cisco_device_type_support.end_of_routine_failure_analysis_date }}</td>
-                    </tr>
-                    <tr {{ cisco_device_type_support.end_of_svc_attach_date|expiration_class }}>
-                        <td>End of New Service Attachment Date</td>
-                        <td>{{ cisco_device_type_support.end_of_svc_attach_date }}</td>
-                    </tr>
-                    <tr {{ cisco_device_type_support.end_of_service_contract_renewal|expiration_class }}>
-                        <td>End of Service Contract Renewal Date</td>
-                        <td>{{ cisco_device_type_support.end_of_service_contract_renewal }}</td>
-                    </tr>
-                    <tr {{ cisco_device_type_support.end_of_security_vul_support_date|expiration_class }}>
-                        <td>End of Vulnerability/Security Support</td>
-                        <td>{{ cisco_device_type_support.end_of_security_vul_support_date }}</td>
-                    </tr>
-                    <tr {{ cisco_device_type_support.last_date_of_support|expiration_class }}>
-                        <td>Last Date of Support</td>
-                        <td>{{ cisco_device_type_support.last_date_of_support }}</td>
-                    </tr>
-                {% else %}
-                    <tr {{ cisco_device_type_support.eox_has_error|eox_class }}>
-                        <td style="width: 40%">EoX Status</td>
-                        <td style="width: 40px"><i {{ cisco_device_type_support.eox_has_error|eox_class_boolian }}></i></td>
-                        <td>{{ cisco_device_type_support.eox_error }}</td>
-                    </tr>
-                {% endif %}
-            </tbody>
-        </table>
+        {% if not cisco_device_support %}
+            {% include "netbox_cisco_support_plugin/no_data_available.html" %}
+        {% else %}
+            <table class="table table-hover panel-body attr-table">
+                <tbody>
+                    {% if cisco_device_type_support.eox_announcement_date %}
+                        <tr {{ cisco_device_type_support.eox_announcement_date|expiration_class }}>
+                            <td style="width: 40%">EoX Announcement Date</td>
+                            <td>{{ cisco_device_type_support.eox_announcement_date }}</td>
+                        </tr>
+                        <tr {{ cisco_device_type_support.end_of_sale_date|expiration_class }}>
+                            <td>End-of-Sale Date</td>
+                            <td>{{ cisco_device_type_support.end_of_sale_date }}</td>
+                        </tr>
+                        <tr {{ cisco_device_type_support.end_of_sw_maintenance_releases|expiration_class }}>
+                            <td>End of SW Maintenance Releases Date</td>
+                            <td>{{ cisco_device_type_support.end_of_sw_maintenance_releases }}</td>
+                        </tr>
+                        <tr {{ cisco_device_type_support.end_of_routine_failure_analysis_date|expiration_class }}>
+                            <td>End of Routine Failure Analysis Date</td>
+                            <td>{{ cisco_device_type_support.end_of_routine_failure_analysis_date }}</td>
+                        </tr>
+                        <tr {{ cisco_device_type_support.end_of_svc_attach_date|expiration_class }}>
+                            <td>End of New Service Attachment Date</td>
+                            <td>{{ cisco_device_type_support.end_of_svc_attach_date }}</td>
+                        </tr>
+                        <tr {{ cisco_device_type_support.end_of_service_contract_renewal|expiration_class }}>
+                            <td>End of Service Contract Renewal Date</td>
+                            <td>{{ cisco_device_type_support.end_of_service_contract_renewal }}</td>
+                        </tr>
+                        <tr {{ cisco_device_type_support.end_of_security_vul_support_date|expiration_class }}>
+                            <td>End of Vulnerability/Security Support</td>
+                            <td>{{ cisco_device_type_support.end_of_security_vul_support_date }}</td>
+                        </tr>
+                        <tr {{ cisco_device_type_support.last_date_of_support|expiration_class }}>
+                            <td>Last Date of Support</td>
+                            <td>{{ cisco_device_type_support.last_date_of_support }}</td>
+                        </tr>
+                    {% else %}
+                        <tr {{ cisco_device_type_support.eox_has_error|eox_class }}>
+                            <td style="width: 40%">EoX Status</td>
+                            <td style="width: 40px"><i {{ cisco_device_type_support.eox_has_error|eox_class_boolian }}></i></td>
+                            <td>{{ cisco_device_type_support.eox_error }}</td>
+                        </tr>
+                    {% endif %}
+                </tbody>
+            </table>
 
-        {% if cisco_device_type_support %}
             <div class="text-muted">Last updated: {{ cisco_device_type_support.last_updated }}</div>
         {% endif %}
-        
+
     </div>
 
 </div>
```

#### html2text {}

```diff
@@ -1,5 +1,6 @@
 {% load filters %}
 ** Cisco Device Type Support **
-{% if cisco_device_type_support %}
+{% if not cisco_device_support %} {% include "netbox_cisco_support_plugin/
+no_data_available.html" %} {% else %}
 Last updated: {{ cisco_device_type_support.last_updated }}
 {% endif %}
```

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/templatetags/filters.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/urls.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin/views.py` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin/views.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin.egg-info/PKG-INFO` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-support-plugin
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-support-plugin-0.0.1/netbox_cisco_support_plugin.egg-info/SOURCES.txt` & `netbox-cisco-support-plugin-0.0.2/netbox_cisco_support_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.1/setup.py` & `netbox-cisco-support-plugin-0.0.2/setup.py`

 * *Files identical despite different names*

