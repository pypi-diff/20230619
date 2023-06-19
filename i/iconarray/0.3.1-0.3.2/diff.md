# Comparing `tmp/iconarray-0.3.1.tar.gz` & `tmp/iconarray-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iconarray-0.3.1.tar", last modified: Mon Jun 19 13:53:06 2023, max compression
+gzip compressed data, was "iconarray-0.3.2.tar", last modified: Mon Jun 19 14:06:16 2023, max compression
```

## Comparing `iconarray-0.3.1.tar` & `iconarray-0.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.588451 iconarray-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-19 13:52:57.000000 iconarray-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-06-19 13:53:06.588451 iconarray-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-06-19 13:52:57.000000 iconarray-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.584451 iconarray-0.3.1/iconarray/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.584451 iconarray-0.3.1/iconarray/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26233 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/backend/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.584451 iconarray-0.3.1/iconarray/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/core/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/core/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/core/latlonhash.py
--rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/core/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.588451 iconarray-0.3.1/iconarray/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.588451 iconarray-0.3.1/iconarray/plot/formatoptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/formatoptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/formatoptions/borders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/formatoptions/customtext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/formatoptions/lakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/formatoptions/meanmaxwind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/formatoptions/rivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/formatoptions/standardtitle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.588451 iconarray-0.3.1/iconarray/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/utils/get_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.584451 iconarray-0.3.1/iconarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-06-19 13:53:06.000000 iconarray-0.3.1/iconarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-19 13:53:06.000000 iconarray-0.3.1/iconarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:53:06.000000 iconarray-0.3.1/iconarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-19 13:53:06.000000 iconarray-0.3.1/iconarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-19 13:53:06.000000 iconarray-0.3.1/iconarray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-19 13:53:06.588451 iconarray-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-19 13:52:57.000000 iconarray-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:06:16.156397 iconarray-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-19 14:06:06.000000 iconarray-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-06-19 14:06:16.156397 iconarray-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-06-19 14:06:06.000000 iconarray-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:06:16.152397 iconarray-0.3.2/iconarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:06:16.152397 iconarray-0.3.2/iconarray/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26233 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/backend/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:06:16.152397 iconarray-0.3.2/iconarray/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/core/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/core/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/core/latlonhash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/core/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:06:16.152397 iconarray-0.3.2/iconarray/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/plot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:06:16.156397 iconarray-0.3.2/iconarray/plot/formatoptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/plot/formatoptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/plot/formatoptions/borders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/plot/formatoptions/customtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/plot/formatoptions/lakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/plot/formatoptions/meanmaxwind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/plot/formatoptions/rivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/plot/formatoptions/standardtitle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:06:16.156397 iconarray-0.3.2/iconarray/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-19 14:06:06.000000 iconarray-0.3.2/iconarray/utils/get_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:06:16.152397 iconarray-0.3.2/iconarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-06-19 14:06:16.000000 iconarray-0.3.2/iconarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-19 14:06:16.000000 iconarray-0.3.2/iconarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:06:16.000000 iconarray-0.3.2/iconarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-19 14:06:16.000000 iconarray-0.3.2/iconarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-19 14:06:16.000000 iconarray-0.3.2/iconarray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-19 14:06:16.156397 iconarray-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-19 14:06:06.000000 iconarray-0.3.2/setup.py
```

### Comparing `iconarray-0.3.1/LICENSE` & `iconarray-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/PKG-INFO` & `iconarray-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iconarray
-Version: 0.3.1
+Version: 0.3.2
 Summary: A package of modules for processing and plotting ICON data.
 Home-page: https://github.com/C2SM/iconarray
 Author: MeteoSwiss, C2SM
 Author-email: victoria.cherkas@meteoswiss.ch, annika.lauber@c2sm.ethz.ch
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `iconarray-0.3.1/README.md` & `iconarray-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/iconarray/backend/grid.py` & `iconarray-0.3.2/iconarray/backend/grid.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/iconarray/core/crop.py` & `iconarray-0.3.2/iconarray/core/crop.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/iconarray/core/interpolate.py` & `iconarray-0.3.2/iconarray/core/interpolate.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/iconarray/core/latlonhash.py` & `iconarray-0.3.2/iconarray/core/latlonhash.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/iconarray/core/utilities.py` & `iconarray-0.3.2/iconarray/core/utilities.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/iconarray/plot/config.py` & `iconarray-0.3.2/iconarray/plot/config.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/iconarray/plot/formatoptions/borders.py` & `iconarray-0.3.2/iconarray/plot/formatoptions/borders.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/iconarray/plot/formatoptions/customtext.py` & `iconarray-0.3.2/iconarray/plot/formatoptions/customtext.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/iconarray/plot/formatoptions/lakes.py` & `iconarray-0.3.2/iconarray/plot/formatoptions/lakes.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/iconarray/plot/formatoptions/meanmaxwind.py` & `iconarray-0.3.2/iconarray/plot/formatoptions/meanmaxwind.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/iconarray/plot/formatoptions/rivers.py` & `iconarray-0.3.2/iconarray/plot/formatoptions/rivers.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/iconarray/plot/formatoptions/standardtitle.py` & `iconarray-0.3.2/iconarray/plot/formatoptions/standardtitle.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/iconarray/utils/get_data.py` & `iconarray-0.3.2/iconarray/utils/get_data.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/iconarray.egg-info/PKG-INFO` & `iconarray-0.3.2/iconarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iconarray
-Version: 0.3.1
+Version: 0.3.2
 Summary: A package of modules for processing and plotting ICON data.
 Home-page: https://github.com/C2SM/iconarray
 Author: MeteoSwiss, C2SM
 Author-email: victoria.cherkas@meteoswiss.ch, annika.lauber@c2sm.ethz.ch
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `iconarray-0.3.1/iconarray.egg-info/SOURCES.txt` & `iconarray-0.3.2/iconarray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/setup.cfg` & `iconarray-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.1/setup.py` & `iconarray-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="iconarray",  # Required
-    version="v0.3.1",  # Required
+    version="v0.3.2",  # Required
     description="A package of modules for processing and plotting ICON data.",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional
     url="https://github.com/C2SM/iconarray",  # Optional
     author="MeteoSwiss, C2SM",  # Optional
     author_email="victoria.cherkas@meteoswiss.ch, annika.lauber@c2sm.ethz.ch",  # Optional
     # package_dir={"": "iconarray"},  # Optional
```

