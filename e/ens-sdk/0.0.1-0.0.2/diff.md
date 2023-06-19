# Comparing `tmp/ens_sdk-0.0.1.tar.gz` & `tmp/ens_sdk-0.0.2.tar.gz`

## Comparing `ens_sdk-0.0.1.tar` & `ens_sdk-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/__init__.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/.idea/encipher-notification-service-sdk.iml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0     8761 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/src/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/src/ens_sdk/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/src/ens_sdk/utils/__init__.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/LICENSE
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/README.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 ens_sdk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/src/ens_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/src/ens_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/src/ens_sdk/utils/cache.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/src/ens_sdk/utils/decouple.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/src/ens_sdk/utils/timezone.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/LICENSE
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/README.md
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/PKG-INFO
```

### Comparing `ens_sdk-0.0.1/LICENSE` & `ens_sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ens_sdk-0.0.1/PKG-INFO` & `ens_sdk-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ens_sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: An SDK to simplify connectivity to ENS Services
 Project-URL: Homepage, https://github.com/enciphertz/encipher-notificaition-service-python-sdk
 Project-URL: Bug Tracker, https://github.com/enciphertz/encipher-notificaition-service-python-sdk/issues
 Author-email: Joseph Daudi <joseph@encipher.dev>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

