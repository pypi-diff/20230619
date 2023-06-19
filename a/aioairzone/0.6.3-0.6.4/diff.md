# Comparing `tmp/aioairzone-0.6.3.tar.gz` & `tmp/aioairzone-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-0.6.3.tar", last modified: Tue Jun  6 05:23:35 2023, max compression
+gzip compressed data, was "aioairzone-0.6.4.tar", last modified: Mon Jun 19 18:17:26 2023, max compression
```

## Comparing `aioairzone-0.6.3.tar` & `aioairzone-0.6.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-06 05:23:35.299924 aioairzone-0.6.3/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-01 18:26:58.000000 aioairzone-0.6.3/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       87 2022-05-10 12:55:46.000000 aioairzone-0.6.3/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-06-06 05:23:35.299924 aioairzone-0.6.3/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1897 2023-05-10 16:25:49.000000 aioairzone-0.6.3/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-06 05:23:35.295924 aioairzone-0.6.3/aioairzone/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       23 2022-03-01 19:23:56.000000 aioairzone-0.6.3/aioairzone/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4647 2023-05-26 14:19:03.000000 aioairzone-0.6.3/aioairzone/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     7039 2023-06-06 05:16:20.000000 aioairzone-0.6.3/aioairzone/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1396 2022-05-04 20:36:00.000000 aioairzone-0.6.3/aioairzone/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    17075 2023-06-06 05:20:29.000000 aioairzone-0.6.3/aioairzone/localapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2022-05-10 12:55:46.000000 aioairzone-0.6.3/aioairzone/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)     8044 2023-05-26 20:19:09.000000 aioairzone-0.6.3/aioairzone/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1565 2023-05-26 14:19:03.000000 aioairzone-0.6.3/aioairzone/thermostat.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4100 2022-12-28 09:48:21.000000 aioairzone-0.6.3/aioairzone/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    25108 2023-05-26 20:18:51.000000 aioairzone-0.6.3/aioairzone/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-06 05:23:35.299924 aioairzone-0.6.3/aioairzone.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-06-06 05:23:35.000000 aioairzone-0.6.3/aioairzone.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      494 2023-06-06 05:23:35.000000 aioairzone-0.6.3/aioairzone.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-06-06 05:23:35.000000 aioairzone-0.6.3/aioairzone.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-06-06 05:23:35.000000 aioairzone-0.6.3/aioairzone.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-06-06 05:23:35.000000 aioairzone-0.6.3/aioairzone.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       11 2023-06-06 05:23:35.000000 aioairzone-0.6.3/aioairzone.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      996 2023-06-06 05:22:42.000000 aioairzone-0.6.3/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-02 19:19:23.000000 aioairzone-0.6.3/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      303 2023-06-06 05:23:35.299924 aioairzone-0.6.3/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-19 18:17:26.154168 aioairzone-0.6.4/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-01 18:26:58.000000 aioairzone-0.6.4/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       87 2022-05-10 12:55:46.000000 aioairzone-0.6.4/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-06-19 18:17:26.154168 aioairzone-0.6.4/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1897 2023-05-10 16:25:49.000000 aioairzone-0.6.4/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-19 18:17:26.154168 aioairzone-0.6.4/aioairzone/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       23 2022-03-01 19:23:56.000000 aioairzone-0.6.4/aioairzone/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4647 2023-05-26 14:19:03.000000 aioairzone-0.6.4/aioairzone/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     7039 2023-06-06 05:16:20.000000 aioairzone-0.6.4/aioairzone/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1396 2022-05-04 20:36:00.000000 aioairzone-0.6.4/aioairzone/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    17065 2023-06-19 18:12:39.000000 aioairzone-0.6.4/aioairzone/localapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2022-05-10 12:55:46.000000 aioairzone-0.6.4/aioairzone/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     8044 2023-05-26 20:19:09.000000 aioairzone-0.6.4/aioairzone/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1565 2023-05-26 14:19:03.000000 aioairzone-0.6.4/aioairzone/thermostat.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4100 2022-12-28 09:48:21.000000 aioairzone-0.6.4/aioairzone/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    25108 2023-05-26 20:18:51.000000 aioairzone-0.6.4/aioairzone/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-19 18:17:26.154168 aioairzone-0.6.4/aioairzone.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-06-19 18:17:26.000000 aioairzone-0.6.4/aioairzone.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      494 2023-06-19 18:17:26.000000 aioairzone-0.6.4/aioairzone.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-06-19 18:17:26.000000 aioairzone-0.6.4/aioairzone.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-06-19 18:17:25.000000 aioairzone-0.6.4/aioairzone.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-06-19 18:17:26.000000 aioairzone-0.6.4/aioairzone.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       11 2023-06-19 18:17:26.000000 aioairzone-0.6.4/aioairzone.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      996 2023-06-19 18:14:57.000000 aioairzone-0.6.4/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-02 19:19:23.000000 aioairzone-0.6.4/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      303 2023-06-19 18:17:26.154168 aioairzone-0.6.4/setup.cfg
```

### Comparing `aioairzone-0.6.3/LICENSE` & `aioairzone-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.3/PKG-INFO` & `aioairzone-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone
-Version: 0.6.3
+Version: 0.6.4
 Summary: Library to control Airzone devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone/issues
 Keywords: airzone,hvac,home
 Platform: any
```

### Comparing `aioairzone-0.6.3/README.md` & `aioairzone-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.3/aioairzone/common.py` & `aioairzone-0.6.4/aioairzone/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.3/aioairzone/const.py` & `aioairzone-0.6.4/aioairzone/const.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.3/aioairzone/exceptions.py` & `aioairzone-0.6.4/aioairzone/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.3/aioairzone/localapi.py` & `aioairzone-0.6.4/aioairzone/localapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         except (SystemOutOfRange, ZoneNotProvided):
             pass
 
         try:
             version = await self.get_version()
             if API_VERSION in version:
                 self.version = version[API_VERSION]
-        except (InvalidHost, APIError):
+        except InvalidMethod:
             pass
 
         self.api_features_checked = True
 
     async def update_features(self) -> None:
         """Gather Airzone features data."""
         if not self.api_features_checked:
```

### Comparing `aioairzone-0.6.3/aioairzone/system.py` & `aioairzone-0.6.4/aioairzone/system.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.3/aioairzone/thermostat.py` & `aioairzone-0.6.4/aioairzone/thermostat.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.3/aioairzone/webserver.py` & `aioairzone-0.6.4/aioairzone/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.3/aioairzone/zone.py` & `aioairzone-0.6.4/aioairzone/zone.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.3/aioairzone.egg-info/PKG-INFO` & `aioairzone-0.6.4/aioairzone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone
-Version: 0.6.3
+Version: 0.6.4
 Summary: Library to control Airzone devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone/issues
 Keywords: airzone,hvac,home
 Platform: any
```

### Comparing `aioairzone-0.6.3/pyproject.toml` & `aioairzone-0.6.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone"
-version = "0.6.3"
+version = "0.6.4"
 description = "Library to control Airzone devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

