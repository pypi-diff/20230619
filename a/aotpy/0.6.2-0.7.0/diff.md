# Comparing `tmp/aotpy-0.6.2.tar.gz` & `tmp/aotpy-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aotpy-0.6.2.tar", last modified: Tue May 16 14:43:58 2023, max compression
+gzip compressed data, was "aotpy-0.7.0.tar", last modified: Mon Jun 19 17:04:13 2023, max compression
```

## Comparing `aotpy-0.6.2.tar` & `aotpy-0.7.0.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.205047 aotpy-0.6.2/
--rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.6.2/LICENSE
--rw-rw-rw-   0        0        0     2991 2023-05-16 14:43:58.205047 aotpy-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2023-05-02 22:45:22.000000 aotpy-0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.138066 aotpy-0.6.2/aotpy/
--rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-0.6.2/aotpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.174776 aotpy-0.6.2/aotpy/core/
--rw-rw-rw-   0        0        0      555 2023-05-08 11:52:45.000000 aotpy-0.6.2/aotpy/core/__init__.py
--rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.6.2/aotpy/core/aberration.py
--rw-rw-rw-   0        0        0     3967 2023-05-03 10:26:29.000000 aotpy-0.6.2/aotpy/core/ao_system.py
--rw-rw-rw-   0        0        0     3050 2023-05-08 11:38:37.000000 aotpy-0.6.2/aotpy/core/atmosphere.py
--rw-rw-rw-   0        0        0      618 2023-05-03 10:52:05.000000 aotpy-0.6.2/aotpy/core/base.py
--rw-rw-rw-   0        0        0     1840 2023-05-02 13:49:09.000000 aotpy-0.6.2/aotpy/core/image.py
--rw-rw-rw-   0        0        0     5293 2023-05-03 17:08:11.000000 aotpy-0.6.2/aotpy/core/loop.py
--rw-rw-rw-   0        0        0    11452 2023-05-08 11:39:26.000000 aotpy-0.6.2/aotpy/core/optical_sensor.py
--rw-rw-rw-   0        0        0     2701 2023-05-02 09:42:13.000000 aotpy-0.6.2/aotpy/core/source.py
--rw-rw-rw-   0        0        0     4887 2023-05-08 11:39:26.000000 aotpy-0.6.2/aotpy/core/telescope.py
--rw-rw-rw-   0        0        0      708 2023-05-02 09:43:33.000000 aotpy-0.6.2/aotpy/core/time.py
--rw-rw-rw-   0        0        0     3554 2023-05-08 11:39:26.000000 aotpy-0.6.2/aotpy/core/wavefront_corrector.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.175753 aotpy-0.6.2/aotpy/data/
-drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.177709 aotpy-0.6.2/aotpy/data/AOF/
--rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.6.2/aotpy/data/AOF/subap.fits
-drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.179659 aotpy-0.6.2/aotpy/data/ERIS/
--rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.6.2/aotpy/data/ERIS/subap.fits
-drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.180636 aotpy-0.6.2/aotpy/data/NAOMI/
--rw-rw-rw-   0        0        0  7344000 2023-05-03 14:12:48.000000 aotpy-0.6.2/aotpy/data/NAOMI/zernike_control_modes.fits
--rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-0.6.2/aotpy/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.189424 aotpy-0.6.2/aotpy/io/
--rw-rw-rw-   0        0        0      436 2023-05-02 11:33:11.000000 aotpy-0.6.2/aotpy/io/__init__.py
--rw-rw-rw-   0        0        0     2785 2023-05-02 11:47:25.000000 aotpy-0.6.2/aotpy/io/base.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.196259 aotpy-0.6.2/aotpy/io/fits/
--rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.6.2/aotpy/io/fits/__init__.py
--rw-rw-rw-   0        0        0    26711 2023-05-16 13:12:55.000000 aotpy-0.6.2/aotpy/io/fits/_keywords.py
--rw-rw-rw-   0        0        0    42036 2023-05-08 12:12:15.000000 aotpy-0.6.2/aotpy/io/fits/reader.py
--rw-rw-rw-   0        0        0     8760 2023-05-03 10:32:11.000000 aotpy-0.6.2/aotpy/io/fits/utils.py
--rw-rw-rw-   0        0        0    31083 2023-05-08 11:41:08.000000 aotpy-0.6.2/aotpy/io/fits/writer.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.204072 aotpy-0.6.2/aotpy/translators/
--rw-rw-rw-   0        0        0      358 2023-05-02 17:59:07.000000 aotpy-0.6.2/aotpy/translators/__init__.py
--rw-rw-rw-   0        0        0    11058 2023-05-16 13:51:26.000000 aotpy-0.6.2/aotpy/translators/aof.py
--rw-rw-rw-   0        0        0      979 2023-05-02 18:03:17.000000 aotpy-0.6.2/aotpy/translators/base.py
--rw-rw-rw-   0        0        0     6842 2023-05-15 12:17:23.000000 aotpy-0.6.2/aotpy/translators/ciao.py
--rw-rw-rw-   0        0        0    14290 2023-05-16 13:51:26.000000 aotpy-0.6.2/aotpy/translators/eris.py
--rw-rw-rw-   0        0        0     9095 2023-05-15 14:15:02.000000 aotpy-0.6.2/aotpy/translators/eso.py
--rw-rw-rw-   0        0        0     7181 2023-05-16 13:43:00.000000 aotpy-0.6.2/aotpy/translators/naomi.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.158575 aotpy-0.6.2/aotpy.egg-info/
--rw-rw-rw-   0        0        0     2991 2023-05-16 14:43:58.000000 aotpy-0.6.2/aotpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      953 2023-05-16 14:43:58.000000 aotpy-0.6.2/aotpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 14:43:58.000000 aotpy-0.6.2/aotpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2023-05-16 14:43:58.000000 aotpy-0.6.2/aotpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-16 14:43:58.000000 aotpy-0.6.2/aotpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.6.2/pyproject.toml
--rw-rw-rw-   0        0        0     1019 2023-05-16 14:43:58.207979 aotpy-0.6.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.298122 aotpy-0.7.0/
+-rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     2997 2023-06-19 17:04:13.298122 aotpy-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-05-02 22:45:22.000000 aotpy-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.210634 aotpy-0.7.0/aotpy/
+-rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-0.7.0/aotpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.245322 aotpy-0.7.0/aotpy/core/
+-rw-rw-rw-   0        0        0      555 2023-05-08 11:52:45.000000 aotpy-0.7.0/aotpy/core/__init__.py
+-rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.7.0/aotpy/core/aberration.py
+-rw-rw-rw-   0        0        0     3897 2023-06-05 13:40:11.000000 aotpy-0.7.0/aotpy/core/ao_system.py
+-rw-rw-rw-   0        0        0     3050 2023-05-08 11:38:37.000000 aotpy-0.7.0/aotpy/core/atmosphere.py
+-rw-rw-rw-   0        0        0      616 2023-06-19 16:50:55.000000 aotpy-0.7.0/aotpy/core/base.py
+-rw-rw-rw-   0        0        0     1831 2023-06-19 16:50:55.000000 aotpy-0.7.0/aotpy/core/image.py
+-rw-rw-rw-   0        0        0     5293 2023-05-03 17:08:11.000000 aotpy-0.7.0/aotpy/core/loop.py
+-rw-rw-rw-   0        0        0    11452 2023-05-08 11:39:26.000000 aotpy-0.7.0/aotpy/core/optical_sensor.py
+-rw-rw-rw-   0        0        0     2863 2023-05-22 10:44:57.000000 aotpy-0.7.0/aotpy/core/source.py
+-rw-rw-rw-   0        0        0     4887 2023-06-19 16:50:55.000000 aotpy-0.7.0/aotpy/core/telescope.py
+-rw-rw-rw-   0        0        0      706 2023-06-19 16:50:55.000000 aotpy-0.7.0/aotpy/core/time.py
+-rw-rw-rw-   0        0        0     3552 2023-06-19 16:50:55.000000 aotpy-0.7.0/aotpy/core/wavefront_corrector.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.246299 aotpy-0.7.0/aotpy/data/
+drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.254674 aotpy-0.7.0/aotpy/data/AOF/
+-rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.7.0/aotpy/data/AOF/subap.fits
+drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.257576 aotpy-0.7.0/aotpy/data/ERIS/
+-rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.7.0/aotpy/data/ERIS/ho_subap.fits
+-rw-rw-rw-   0        0        0     5760 2023-06-19 12:38:42.000000 aotpy-0.7.0/aotpy/data/ERIS/lo_subap.fits
+drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.263952 aotpy-0.7.0/aotpy/data/NAOMI/
+-rw-rw-rw-   0        0        0  7344000 2023-05-03 14:12:48.000000 aotpy-0.7.0/aotpy/data/NAOMI/zernike_control_modes.fits
+drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.276639 aotpy-0.7.0/aotpy/data/PAPYRUS/
+-rw-rw-rw-   0        0        0  1013760 2023-06-19 15:05:10.000000 aotpy-0.7.0/aotpy/data/PAPYRUS/T152_pupil.fits
+-rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-0.7.0/aotpy/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.280545 aotpy-0.7.0/aotpy/io/
+-rw-rw-rw-   0        0        0      436 2023-06-19 16:50:12.000000 aotpy-0.7.0/aotpy/io/__init__.py
+-rw-rw-rw-   0        0        0     2789 2023-06-19 16:50:12.000000 aotpy-0.7.0/aotpy/io/base.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.288359 aotpy-0.7.0/aotpy/io/fits/
+-rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.7.0/aotpy/io/fits/__init__.py
+-rw-rw-rw-   0        0        0    26710 2023-06-19 16:49:27.000000 aotpy-0.7.0/aotpy/io/fits/_keywords.py
+-rw-rw-rw-   0        0        0    42034 2023-06-19 16:49:27.000000 aotpy-0.7.0/aotpy/io/fits/reader.py
+-rw-rw-rw-   0        0        0     9252 2023-06-19 16:19:02.000000 aotpy-0.7.0/aotpy/io/fits/utils.py
+-rw-rw-rw-   0        0        0    31083 2023-05-08 11:41:08.000000 aotpy-0.7.0/aotpy/io/fits/writer.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.297145 aotpy-0.7.0/aotpy/translators/
+-rw-rw-rw-   0        0        0      432 2023-06-19 16:00:06.000000 aotpy-0.7.0/aotpy/translators/__init__.py
+-rw-rw-rw-   0        0        0    11304 2023-06-19 16:46:11.000000 aotpy-0.7.0/aotpy/translators/aof.py
+-rw-rw-rw-   0        0        0      981 2023-06-19 16:46:11.000000 aotpy-0.7.0/aotpy/translators/base.py
+-rw-rw-rw-   0        0        0     6993 2023-06-19 16:46:11.000000 aotpy-0.7.0/aotpy/translators/ciao.py
+-rw-rw-rw-   0        0        0    18293 2023-06-19 16:47:44.000000 aotpy-0.7.0/aotpy/translators/eris.py
+-rw-rw-rw-   0        0        0    10438 2023-06-19 16:46:11.000000 aotpy-0.7.0/aotpy/translators/eso.py
+-rw-rw-rw-   0        0        0     7412 2023-06-19 16:46:11.000000 aotpy-0.7.0/aotpy/translators/naomi.py
+-rw-rw-rw-   0        0        0     3642 2023-06-19 16:46:11.000000 aotpy-0.7.0/aotpy/translators/papyrus.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.232117 aotpy-0.7.0/aotpy.egg-info/
+-rw-rw-rw-   0        0        0     2997 2023-06-19 17:04:13.000000 aotpy-0.7.0/aotpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-06-19 17:04:13.000000 aotpy-0.7.0/aotpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 17:04:13.000000 aotpy-0.7.0/aotpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-06-19 17:04:13.000000 aotpy-0.7.0/aotpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 17:04:13.000000 aotpy-0.7.0/aotpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1029 2023-06-19 17:04:13.302035 aotpy-0.7.0/setup.cfg
```

### Comparing `aotpy-0.6.2/LICENSE` & `aotpy-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.2/PKG-INFO` & `aotpy-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.6.2
+Version: 0.7.0
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
-Home-page: https://github.com/kYwzor/aotpy
+Home-page: https://github.com/STAR-PORT/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
-Project-URL: Bug Tracker, https://github.com/kYwzor/aotpy/issues
+Project-URL: Bug Tracker, https://github.com/STAR-PORT/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.10
```

### Comparing `aotpy-0.6.2/README.md` & `aotpy-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.2/aotpy/__init__.py` & `aotpy-0.7.0/aotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.2/aotpy/core/__init__.py` & `aotpy-0.7.0/aotpy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.2/aotpy/core/aberration.py` & `aotpy-0.7.0/aotpy/core/aberration.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.2/aotpy/core/ao_system.py` & `aotpy-0.7.0/aotpy/core/ao_system.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,19 +75,18 @@
         filename
             Path to the file to be written.
         kwargs
             Optional keyword arguments passed on as options to the writer function.
         """
         ext = Path(filename).suffix[1:]
         try:
-            WriterClass = _AVAILABLE_WRITERS[ext.lower()]
+            _AVAILABLE_WRITERS[ext.lower()](self).write(filename, **kwargs)
         except KeyError:
             raise ValueError(f"No available writer for extension '{ext}'. "
                              f"Available extensions: {str(list(_AVAILABLE_WRITERS.keys()))[1:-1]}")
-        WriterClass(self).write(filename, **kwargs)
 
     @staticmethod
     def read_from_file(filename: str | os.PathLike, **kwargs) -> 'AOSystem':
         """
         Reads `AOSystem` from a file. The reading function is deduced by the extension in the specified `filename`.
 
         Parameters
@@ -95,12 +94,11 @@
         filename
             Path to the file to be read.
         kwargs
             Optional keyword arguments passed on as options to the reader function.
         """
         ext = Path(filename).suffix[1:]
         try:
-            ReaderClass = _AVAILABLE_READERS[ext.lower()]
+            return _AVAILABLE_READERS[ext.lower()](filename, **kwargs).get_system()
         except KeyError:
             raise ValueError(f"No available reader for extension '{ext}'. "
                              f"Available extensions: {str(list(_AVAILABLE_READERS.keys()))[1:-1]}")
-        return ReaderClass(filename, **kwargs).get_system()
```

### Comparing `aotpy-0.6.2/aotpy/core/atmosphere.py` & `aotpy-0.7.0/aotpy/core/atmosphere.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.2/aotpy/core/base.py` & `aotpy-0.7.0/aotpy/core/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,7 @@
     """Abstract class for all classes which can be referenced via a UID."""
     uid: str
     """Unique identifier of the object, which allows unambiguous referencing."""
 
     def __post_init__(self):
         if self.__class__ == Referenceable:
             raise TypeError("Cannot instantiate abstract class.")
-
```

### Comparing `aotpy-0.6.2/aotpy/core/image.py` & `aotpy-0.7.0/aotpy/core/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains classes that define multidimensional data in AOT and their respective metadata.
 """
 
-from dataclasses import dataclass, field, KW_ONLY
+from dataclasses import dataclass, field
 from typing import Any
 
 import numpy as np
 
 from .time import Time
 
 __all__ = ['Image', 'Metadatum']
```

### Comparing `aotpy-0.6.2/aotpy/core/loop.py` & `aotpy-0.7.0/aotpy/core/loop.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.2/aotpy/core/optical_sensor.py` & `aotpy-0.7.0/aotpy/core/optical_sensor.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.2/aotpy/core/source.py` & `aotpy-0.7.0/aotpy/core/source.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,22 +44,26 @@
 @dataclass(kw_only=True)
 class NaturalGuideStar(Source):
     """Contains data regarding a natural guide star being observed by the system."""
     pass
 
 
 @dataclass(kw_only=True)
-class _LaserGuideStar(Source):
-    """Contains data regarding a laser guide star being observed by the system."""
+class LaserGuideStar(Source):
+    """Abstract class that contains data regarding a laser guide star being observed by the system."""
 
     laser_launch_telescope: LaserLaunchTelescope = None
 
+    def __post_init__(self):
+        if self.__class__ == LaserGuideStar:
+            raise TypeError("Cannot instantiate abstract class.")
+
 
 @dataclass(kw_only=True)
-class SodiumLaserGuideStar(_LaserGuideStar):
+class SodiumLaserGuideStar(LaserGuideStar):
     """Contains data regarding a sodium laser guide star being observed by the system."""
 
     height: float = None
     'Mean LGS height at zenith. (in m units)'
 
     profile: Image = None
     """Normalised LGS profile (each set of :math:`l` layers :math:`\\sum = 1`) at zenith, over time.
@@ -67,15 +71,15 @@
 
     altitudes: list[float] = field(default_factory=list)
     """LGS layer profile altitudes at zenith. Must be the same length as the number of layers defined in `profile`.
     (in m units)"""
 
 
 @dataclass(kw_only=True)
-class RayleighLaserGuideStar(_LaserGuideStar):
+class RayleighLaserGuideStar(LaserGuideStar):
     """Contains data regarding a Rayleigh laser guide star being observed by the system."""
 
     distance: float = None
     'Fixed distance of the LGS from the telescope. (in m units)'
 
     depth: float = None
     'TODO: Depth (in m units)'
```

### Comparing `aotpy-0.6.2/aotpy/core/telescope.py` & `aotpy-0.7.0/aotpy/core/telescope.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 This module contains classes for describing telescopes in a system. These may be the main telescope itself of laser
 launch telescopes.
 """
 
-
 from dataclasses import dataclass, field
 
 from .aberration import Aberration
 from .base import Referenceable, Coordinates
 
 __all__ = ['Segments', 'Monolithic', 'CircularSegments', 'HexagonalSegments', 'Telescope', 'MainTelescope',
            'LaserLaunchTelescope']
@@ -28,14 +27,15 @@
     def __post_init__(self):
         if self.__class__ == Segments:
             raise TypeError("Cannot instantiate abstract class.")
 
 
 class Monolithic(Segments):
     """Describes a monolithic pupil."""
+
     def __init__(self):
         super().__init__()  # Use default initialization values for Segments
 
 
 class HexagonalSegments(Segments):
     """Describes the hexagonal segments that constitute the pupil."""
     pass
```

### Comparing `aotpy-0.6.2/aotpy/core/time.py` & `aotpy-0.7.0/aotpy/core/time.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 This module contains a class for describing the passage of time related to data in the system.
 """
 
-
 from dataclasses import dataclass, field
 
 from .base import Referenceable
 
 __all__ = ['Time']
```

### Comparing `aotpy-0.6.2/aotpy/core/wavefront_corrector.py` & `aotpy-0.7.0/aotpy/core/wavefront_corrector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 This module contains classes that describe different types of wavefront correctors in a system.
 """
 
-
 from dataclasses import dataclass, field
 
 from .aberration import Aberration
 from .base import Referenceable, Coordinates
 from .image import Image
 from .telescope import Telescope
```

### Comparing `aotpy-0.6.2/aotpy/data/AOF/subap.fits` & `aotpy-0.7.0/aotpy/data/AOF/subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.2/aotpy/data/ERIS/subap.fits` & `aotpy-0.7.0/aotpy/data/ERIS/ho_subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.2/aotpy/data/NAOMI/zernike_control_modes.fits` & `aotpy-0.7.0/aotpy/data/NAOMI/zernike_control_modes.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.2/aotpy/io/base.py` & `aotpy-0.7.0/aotpy/io/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
     Parameters
     ----------
     system
         `AOSystem` to be written into a file.
 
     """
+
     @abstractmethod
     def __init__(self, system: aotpy.AOSystem) -> None:
         self._system = system
 
     @abstractmethod
     def write(self, filename: str | os.PathLike, **kwargs) -> None:
         """
@@ -49,14 +50,15 @@
         Path to file to be read into an `AOSystem`.
     extra_data : default = False
         Whether it is expected that the file contains some data that does not fit the AOT standard. If `extra_data` is
         not `True`, user will be warned if extra data is detected.
     **kwargs
         Keyword arguments passed on as options to the file handling function.
     """
+
     def __init__(self, filename: str | os.PathLike, *, extra_data: bool = False, **kwargs) -> None:
         self._filename = filename
         self._extra_data_flag = extra_data
 
         self._initialize_data()
         self._system, self._extra_data = self._read(**kwargs)
```

### Comparing `aotpy-0.6.2/aotpy/io/fits/_keywords.py` & `aotpy-0.7.0/aotpy/io/fits/_keywords.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module contains data that defines the AOT FITS format itself, including the specific FITS keywords and tables used.
 Not meant to be imported by users.
 """
 
 import re
 from dataclasses import dataclass
 
-CURRENT_AOT_VERSION = '0.6'
+CURRENT_AOT_VERSION = '1.0.0'
 
 
 @dataclass
 class AOTField:
     name: str
     format: str
     unit: str
@@ -123,15 +123,14 @@
 TIME_FIELDS = AOTFieldDict(
     AOTField(name=REFERENCE_UID, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS, mandatory=True, unique=True),
     AOTField(name=TIME_TIMESTAMPS, format=LIST_FORMAT, unit=UNIT_SECONDS),
     AOTField(name=TIME_FRAME_NUMBERS, format=LIST_FORMAT, unit=UNIT_COUNT)
 )
 TABLE_FIELDS[TIME_TABLE] = TIME_FIELDS
 
-
 # AOT_ATMOSPHERIC_PARAMETERS fields
 ATMOSPHERIC_PARAMETERS_WAVELENGTH = 'WAVELENGTH'
 ATMOSPHERIC_PARAMETERS_R0 = 'R0'
 ATMOSPHERIC_PARAMETERS_FWHM = 'FWHM'
 ATMOSPHERIC_PARAMETERS_TAU0 = 'TAU0'
 ATMOSPHERIC_PARAMETERS_THETA0 = 'THETA0'
 ATMOSPHERIC_PARAMETERS_LAYERS_WEIGHT = 'LAYERS_WEIGHT'
@@ -348,15 +347,15 @@
     AOTField(name=WAVEFRONT_SENSOR_DIMENSIONS, format=INTEGER_FORMAT, unit=UNIT_COUNT, mandatory=True),
     AOTField(name=WAVEFRONT_SENSOR_N_VALID_SUBAPERTURES, format=INTEGER_FORMAT, unit=UNIT_COUNT, mandatory=True),
     AOTField(name=WAVEFRONT_SENSOR_MEASUREMENTS, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=WAVEFRONT_SENSOR_REF_MEASUREMENTS, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=WAVEFRONT_SENSOR_SUBAPERTURE_MASK, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=WAVEFRONT_SENSOR_MASK_X_OFFSETS, format=LIST_FORMAT, unit=UNIT_PIXELS),
     AOTField(name=WAVEFRONT_SENSOR_MASK_Y_OFFSETS, format=LIST_FORMAT, unit=UNIT_PIXELS),
-    AOTField(name=WAVEFRONT_SENSOR_SUBAPERTURE_SIZE, format=STRING_FORMAT, unit=UNIT_PIXELS),
+    AOTField(name=WAVEFRONT_SENSOR_SUBAPERTURE_SIZE, format=FLOAT_FORMAT, unit=UNIT_PIXELS),
     AOTField(name=WAVEFRONT_SENSOR_SUBAPERTURE_INTENSITIES, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=WAVEFRONT_SENSOR_WAVELENGTH, format=FLOAT_FORMAT, unit=UNIT_METERS),
     AOTField(name=WAVEFRONT_SENSOR_OPTICAL_GAIN, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=TRANSFORMATION_MATRIX, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=DETECTOR_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=ABERRATION_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=NCPA_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS)
```

### Comparing `aotpy-0.6.2/aotpy/io/fits/reader.py` & `aotpy-0.7.0/aotpy/io/fits/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 This module contains classes and functions that enable reading AOT FITS files.
 """
 
-
 import re
 import warnings
 from datetime import datetime
 
 import numpy as np
 from astropy.io import fits
```

### Comparing `aotpy-0.6.2/aotpy/io/fits/utils.py` & `aotpy-0.7.0/aotpy/io/fits/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -84,60 +84,72 @@
         self.index = index
         self.name, self.data, self.unit, self._time, self.metadata = _get_image_fields_from_file(url, index, **kwargs)
 
     def __eq__(self, other):
         return self.url == other.url and self.index == other.index and self.time == other.time
 
 
-def image_from_file(path: str | os.PathLike, index: int = None, **kwargs) -> aotpy.Image:
+def image_from_file(path: str | os.PathLike, index: int = None, *, name: str = None, **kwargs) -> aotpy.Image:
     """
     Get `Image` from specified path or URL.
 
     Parameters
     ----------
     path
         Path/URL to FITS file that contains multidimensional data.
     index: int, optional
         Index of the HDU that contains the image data. If omitted, the first HDU containing image data is assumed.
+    name: str, optional
+        Name of the Image. If None, the name is the same as in the file.
     **kwargs
         Keyword arguments passed on as options to the file handling function.
     """
-    name, data, unit, _time, metadata = _get_image_fields_from_file(path, index, **kwargs)
+    _name, data, unit, _time, metadata = _get_image_fields_from_file(path, index, **kwargs)
+    if name is None:
+        name = _name
     image = aotpy.Image(name=name, data=data, unit=unit, metadata=metadata)
     image._time = _time
     return image
 
 
-def image_from_hdus(hdus: fits.HDUList, index: int = None) -> aotpy.Image:
+def image_from_hdus(hdus: fits.HDUList, index: int = None, *, name: str = None) -> aotpy.Image:
     """
     Get `Image` from specified path or URL.
 
     Parameters
     ----------
     hdus
         List of HDUs from which `Image` is to be extracted.
     index: int, optional
         Index of the HDU that contains the image data. If omitted, the first HDU containing image data is assumed.
+    name: str, optional
+        Name of the Image. If None, the name is the same as in the HDU.
     """
-    name, data, unit, _time, metadata = _get_image_fields_from_hdus(hdus, index)
+    _name, data, unit, _time, metadata = _get_image_fields_from_hdus(hdus, index)
+    if name is None:
+        name = _name
     image = aotpy.Image(name=name, data=data, unit=unit, metadata=metadata)
     image._time = _time
     return image
 
 
-def image_from_hdu(hdu: fits.ImageHDU) -> aotpy.Image:
+def image_from_hdu(hdu: fits.ImageHDU, *, name: str = None) -> aotpy.Image:
     """
     Get `Image` from specified HDU.
 
     Parameters
     ----------
     hdu
-        HDU from which `Image` is to be extracted..
-    """
-    name, data, unit, _time, metadata = _get_image_fields_from_hdu(hdu)
+        HDU from which `Image` is to be extracted.
+    name: str, optional
+        Name of the Image. If None, the name is the same as in the HDU.
+    """
+    _name, data, unit, _time, metadata = _get_image_fields_from_hdu(hdu)
+    if name is None:
+        name = _name
     image = aotpy.Image(name=name, data=data, unit=unit, metadata=metadata)
     image._time = _time
     return image
 
 
 def _get_image_fields_from_file(path: str | os.PathLike, index: int = None, **kwargs) -> \
         tuple[str, np.ndarray, str, str, list[aotpy.Metadatum]]:
```

### Comparing `aotpy-0.6.2/aotpy/io/fits/writer.py` & `aotpy-0.7.0/aotpy/io/fits/writer.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.2/aotpy/translators/aof.py` & `aotpy-0.7.0/aotpy/translators/aof.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 This module contains a class for translating data produced by ESO's AOF system.
 """
 
 import importlib.resources
+import warnings
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 from astropy.io import fits
 
 import aotpy
 from aotpy.io import image_from_file
 from .eso import ESOTranslator
 
+
 # TODO set image units
 
 
 class AOFTranslator(ESOTranslator):
     """Contains functions for translating telemetry data produced by ESO's AOF system.
 
     Parameters
@@ -182,15 +184,19 @@
             ref_measurements=aotpy.Image('IRAcq.DET1.REFSLP_WITH_OFFSETS', reference),
             subaperture_intensities=aotpy.Image('WFS_Intensities', ir_loop_frame['WFS_Intensities'])
         )
         self.system.wavefront_sensors.append(ngs_wfs)
 
         # Find the indexes where the counter for pixels matches the counter for ngs
         # Assumes the frames for pixel are contained in the frames for ngs
-        pix_time_mask = np.searchsorted(ir_loop_frame['FrameCounter'], pix_loop_frame['FrameCounter'])
+        ir_fc = ir_loop_frame['FrameCounter']
+        pix_fc = pix_loop_frame['FrameCounter']
+        if pix_fc[0] < ir_fc[0] or pix_fc[-1] > ir_fc[-1]:
+            warnings.warn('Pixel frame counter not contained in IR frame counter, pixel time data may be incorrect.')
+        pix_time_mask = np.searchsorted(ir_fc, pix_fc)
         pix_timestamps = ngs_timestamps[pix_time_mask]
         if np.all(pix_timestamps == 0):
             # The file has no timestamps
             pix_timestamps_list = []
         else:
             pix_timestamps_list = pix_timestamps.tolist()
```

### Comparing `aotpy-0.6.2/aotpy/translators/base.py` & `aotpy-0.7.0/aotpy/translators/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
     Parameters
     ----------
     *args
         Arguments used to initialize the translator class.
 
     """
+
     @abstractmethod
     def __init__(self, *args) -> None:
         self.system: aotpy.AOSystem = aotpy.AOSystem()
 
     @classmethod
     def translate(cls, *args) -> aotpy.AOSystem:
         """
```

### Comparing `aotpy-0.6.2/aotpy/translators/ciao.py` & `aotpy-0.7.0/aotpy/translators/ciao.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 
 import numpy as np
 from astropy.io import fits
 
 import aotpy
 from .eso import ESOTranslator
 
+
 # TODO set image units
 
 
 class CIAOTranslator(ESOTranslator):
     """Contains functions for translating telemetry data produced by ESO's CIAO system.
 
     Parameters
     ----------
     path
         Path to folder containing telemetry data.
     at_number : {1, 2, 3, 4}
         Number of the AT that produced the data.
     """
+
     def __init__(self, path: str, at_number: int):
         path = Path(path)
         self._at_number = at_number
 
         with fits.open(path / 'CIAO_LOOP_0001.fits', extname='LoopFrame') as hdus:
             main_hdr = hdus[0].header
             main_loop_frame = hdus['LoopFrame'].data
@@ -144,11 +146,15 @@
         self.system.sources = [ngs]
         self.system.wavefront_sensors = [wfs]
         self.system.wavefront_correctors = [ho_dm, ittm]
         self.system.loops = [ho_loop, tt_loop]
         self.system.atmosphere_params = [asm, aos]
 
     def _get_eso_telescope_name(self) -> str:
-        return f"ESO-VLTI-A{self._at_number}"
+        # Allow for both:
+        #   ESO-VLTI-Amnop
+        #   ESO-VLTI-Uijkl-Amnop
+        # as long as mnop contains the correct number
+        return f"ESO-VLTI-%A%{self._at_number}%"
 
     def _get_eso_ao_name(self) -> str:
         return 'CIAO'
```

### Comparing `aotpy-0.6.2/aotpy/translators/eso.py` & `aotpy-0.7.0/aotpy/translators/eso.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,31 +11,32 @@
 from abc import abstractmethod
 from datetime import timedelta, datetime, timezone
 
 import astropy.table
 import numpy as np
 from astropy.io import fits
 from astropy.time import Time
+
 try:
     from pyvo.dal import tap
 except (ImportError, ModuleNotFoundError):
     tap = None
 
-
 from aotpy.io.fits import FITSWriter
 from .base import BaseTranslator
 
 ESO_TAP_OBS = "https://archive.eso.org/tap_obs"
 
 
 class ESOTranslator(BaseTranslator):
     """Abstract class for translators for ESO systems.
 
     Translators are able to convert non-standard AO telemetry data files into an `AOSystem` object.
     """
+
     @abstractmethod
     def _get_eso_telescope_name(self) -> str:
         """
         Get value for TELESCOP keyword in ESO's science archive.
 
         Possible values listed below, according to ESO's Data Interface Control Document.
 
@@ -83,67 +84,91 @@
     @abstractmethod
     def _get_eso_ao_name(self) -> str:
         """
         Get abbreviation of the adaptive optics system's name (e.g. 'AOF', 'NAOMI', 'CIAO', ...).
         """
         pass
 
-    def to_archive_ready_file(self, filename, **kwargs) -> None:
+    def to_archive_ready_file(self, filename: str, query_archive: bool = True, **kwargs) -> None:
         """
         Writes translated system into an AOT FITS file with the necessary metadata for ESO Archive.
 
         Requires pyvo.
 
         Parameters
         ----------
         filename
             Path to the file that will be written.
+        query_archive : default = True
+            Whether the ESO archive should be queried to find relevant metadata already in the archive.
         **kwargs
             Keyword arguments passed on as options to the file handling function.
 
         """
-        if tap is None:
-            raise ImportError("Querying the ESO archive requires the pyvo module.")
-        beg = Time(self.system.date_beginning, scale='utc')
         telescope = self._get_eso_telescope_name()
-
-        delta = timedelta(hours=1)
-        query = f"""SELECT TOP 1 ABS(mjd_obs - {beg.mjd}) as diff, *
-        FROM dbo.raw
-        WHERE telescope='{telescope}'
-        and mjd_obs between {(beg - delta).mjd} and {(beg + delta).mjd}
-        and not dp_type LIKE '%AOT%'
-        ORDER BY 1 ASC
-        """
-        res = tap.TAPService(ESO_TAP_OBS).search(query).to_table()
-        if not res:
-            raise ValueError(f"Could not find data from telescope '{telescope}' near mjd_obs {beg.mjd} at ESO Archive")
-        res = res[0]
         metadata = {
             'ORIGIN': 'ESO-PARANAL',
+            'TELESCOP': telescope.replace('%', ''),
             'DATE': datetime.now().isoformat(timespec='milliseconds'),
-            'TELESCOP': telescope,
-            'INSTRUME': res['instrument'],
             'OBJECT': 'AO-TELEM',
-            'RA': res['ra'],
-            'DEC': res['dec'],
-            'PI-COI': res['pi_coi'],
             'OBSERVER': 'I, Condor',
             'DATE-OBS': self.system.date_beginning.astimezone(timezone.utc).replace(tzinfo=None).isoformat(
                 timespec='milliseconds'),
             'MJD-OBS': Time(self.system.date_beginning, scale='utc').mjd,
             'MJD-END': Time(self.system.date_end, scale='utc').mjd,
             'EXPTIME': (self.system.date_end - self.system.date_beginning).total_seconds(),
-            'HIERARCH ESO OBS PROG ID': res['prog_id'],
             'HIERARCH ESO DPR CATG': 'CALIB',
             'HIERARCH ESO DPR TYPE': f'AO-TELEM,AOT,{self._get_eso_ao_name()}',
             'HIERARCH ESO DPR TECH': self.system.ao_mode,
-            'HIERARCH ESO INS MODE': res['ins_mode']
         }
-        # TODO tel_az, tel_alt,
+        if self.system.main_telescope.azimuth is not None:
+            metadata['HIERARCH ESO TEL AZ'] = self.system.main_telescope.azimuth
+        if self.system.main_telescope.elevation is not None:
+            metadata['HIERARCH ESO TEL ALT'] = self.system.main_telescope.elevation
+
+        if query_archive:
+            if tap is None:
+                raise ImportError("Querying the ESO archive requires the pyvo module."
+                                  "You can set the 'query_archive' option to False to skip querying the archive.")
+            beg = Time(self.system.date_beginning, scale='utc')
+
+            if '%' in telescope:
+                tel_comparator = " LIKE "
+            else:
+                tel_comparator = "="
+
+            delta = timedelta(hours=1)
+            query = f"""
+            SELECT TOP 1 ABS(mjd_obs - {beg.mjd}) as diff, *
+            FROM dbo.raw
+            WHERE mjd_obs between {(beg - delta).mjd} and {(beg + delta).mjd}
+                and telescope{tel_comparator}'{telescope}'
+                and not dp_type LIKE '%AOT%'
+            ORDER BY 1 ASC
+            """
+            res = tap.TAPService(ESO_TAP_OBS).search(query).to_table()
+            if res:
+                res = res[0]
+                metadata |= {
+                    'INSTRUME': res['instrument'],
+                    'RA': res['ra'],
+                    'DEC': res['dec'],
+                    # 'PI-COI': res['pi_coi'],
+                    # we do not store PI-COI because it is not needed and can cause issues with special chars
+                    'HIERARCH ESO OBS PROG ID': res['prog_id'],
+                    'HIERARCH ESO INS MODE': res['ins_mode'],
+                }
+                if 'HIERARCH ESO TEL AZ' not in metadata:
+                    metadata['HIERARCH ESO TEL AZ'] = res['tel_az']
+                if 'HIERARCH ESO TEL ALT' not in metadata:
+                    metadata['HIERARCH ESO TEL ALT'] = res['tel_alt']
+            else:
+                warnings.warn(f"Could not find data from telescope '{telescope}' near mjd_obs {beg.mjd} at the "
+                              f"ESO Archive")
+
         hdul = FITSWriter(self.system).get_hdus()
         hdr: fits.Header = hdul[0].header
         hdr.extend(metadata)
         hdul.writeto(filename, **kwargs)
 
     def get_atmospheric_parameters_from_archive(self) -> astropy.table.Table:
         """
@@ -154,15 +179,16 @@
         if tap is None:
             raise ImportError("Querying the ESO archive requires the pyvo module.")
 
         delta = timedelta(minutes=1)
         beg = (self.system.date_beginning - delta).isoformat(timespec='milliseconds')
         end = (self.system.date_end + delta).isoformat(timespec='milliseconds')
 
-        query = f"""SELECT *
+        query = f"""
+        SELECT *
         FROM asm.meteo_paranal
         WHERE midpoint_date between '{beg}' and '{end}'
         AND valid=1
         """
         res = tap.TAPService(ESO_TAP_OBS).search(query).to_table()
         return res
 
@@ -179,31 +205,31 @@
         az
             ESO azimuth to be converted
         """
         # We need to subtract the angle between north and south and then apply symmetry.
         return -(az - 180) % 360
 
     @staticmethod
-    def _get_pixel_data_from_table(pix_loop_frame: fits.FITS_rec) -> np.ndarray:
+    def _get_pixel_data_from_table(pix_frame: fits.FITS_rec) -> np.ndarray:
         """
         Get properly reshaped pixel data from FITS binary table data.
 
         Parameters
         ----------
-        pix_loop_frame
+        pix_frame
             Binary table data containing pixel image.
         """
-        sizes_x = pix_loop_frame['WindowSizeX']
-        sizes_y = pix_loop_frame['WindowSizeY']
+        sizes_x = pix_frame['WindowSizeX']
+        sizes_y = pix_frame['WindowSizeY']
         if np.any(sizes_x != sizes_x[0]) or np.any(sizes_y != sizes_y[0]):
             warnings.warn('Pixel window size seems to change over time.')
         sizes_x = sizes_x[0]
         sizes_y = sizes_y[0]
 
-        return pix_loop_frame['Pixels'][:, :sizes_x * sizes_y].reshape(-1, sizes_x, sizes_y)
+        return pix_frame['Pixels'][:, :sizes_x * sizes_y].reshape(-1, sizes_x, sizes_y)
 
     @staticmethod
     def _stack_slopes(data: np.ndarray, slope_axis: int) -> np.ndarray:
         # ESO slopes are ordered tip1, tilt1, tip2, tilt2, etc., so even numbers are tip and odd numbers are tilt.
         # We separate and then stack them.
         if slope_axis == 0:
             tip = data[::2]
```

### Comparing `aotpy-0.6.2/aotpy/translators/naomi.py` & `aotpy-0.7.0/aotpy/translators/naomi.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,51 +10,55 @@
 import numpy as np
 from astropy.io import fits
 
 import aotpy
 from aotpy.io import image_from_file
 from .eso import ESOTranslator
 
+
 # TODO set image units
 
 
 class NAOMITranslator(ESOTranslator):
     """Contains functions for translating telemetry data produced by ESO's NAOMI system.
 
     Parameters
     ----------
     path
         Path to folder containing telemetry data.
     at_number : {1, 2, 3, 4}
         Number of the AT that produced the data.
     """
+
     def __init__(self, path: str, at_number: int):
         path = Path(path)
         self._at_number = at_number
 
         with fits.open(path / 'NAOMI_LOOP_0001.fits', extname='LoopFrame') as hdus:
             main_hdr = hdus[0].header
             main_loop_frame: fits.FITS_rec = hdus['LoopFrame'].data
 
         self.system = aotpy.AOSystem(ao_mode='SCAO')
         self.system.main_telescope = aotpy.MainTelescope(
             uid=f'ESO VLT AT{at_number}',
             elevation=main_hdr['ESO TEL ALT'],
             azimuth=self._azimuth_conversion(main_hdr['ESO TEL AZ']),
-            parallactic=main_hdr['ESO TEL PRLTIC']
+            parallactic=main_hdr['ESO TEL PRLTIC'],
+            enclosing_diameter=1.82,
+            inscribed_diameter=1.82
         )
         naomi_data_path = importlib.resources.files('aotpy.data') / 'NAOMI'
         with importlib.resources.as_file(naomi_data_path / 'zernike_control_modes.fits') as p:
             # Load file with the representation of the modes controlled in NAOMI (Zernike modes 2 to 15)
             control_modes = aotpy.Image('CONTROL MODES', fits.getdata(p))
 
         if main_hdr['ESO AOS CM MODES CONTROLLED'] != control_modes.data.shape[0]:
             warnings.warn("Keyword 'ESO AOS CM MODES CONTROLLED' does not match expected number of control modes.")
 
-        ngs = aotpy.NaturalGuideStar('NGS',
+        ngs = aotpy.NaturalGuideStar(uid='NGS',
                                      right_ascension=main_hdr['RA'],
                                      declination=main_hdr['DEC'])
 
         main_timestamps = main_loop_frame['Seconds'] + main_loop_frame['USeconds'] / 1.e6
         self.system.date_beginning = datetime.utcfromtimestamp(main_timestamps[0])
         self.system.date_end = datetime.utcfromtimestamp(main_timestamps[-1])
         main_frame_numbers = main_loop_frame['FrameCounter']
@@ -142,11 +146,15 @@
         self.system.sources = [ngs]
         self.system.wavefront_sensors = [wfs]
         self.system.wavefront_correctors = [dm]
         self.system.loops = [loop]
         self.system.atmosphere_params = [asm]
 
     def _get_eso_telescope_name(self) -> str:
-        return f"ESO-VLTI-A{self._at_number}"
+        # Allow for both:
+        #   ESO-VLTI-Amnop
+        #   ESO-VLTI-Uijkl-Amnop
+        # as long as mnop contains the correct number
+        return f"ESO-VLTI-%A%{self._at_number}%"
 
     def _get_eso_ao_name(self) -> str:
         return 'NAOMI'
```

### Comparing `aotpy-0.6.2/aotpy.egg-info/PKG-INFO` & `aotpy-0.7.0/aotpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.6.2
+Version: 0.7.0
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
-Home-page: https://github.com/kYwzor/aotpy
+Home-page: https://github.com/STAR-PORT/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
-Project-URL: Bug Tracker, https://github.com/kYwzor/aotpy/issues
+Project-URL: Bug Tracker, https://github.com/STAR-PORT/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.10
```

### Comparing `aotpy-0.6.2/aotpy.egg-info/SOURCES.txt` & `aotpy-0.7.0/aotpy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -18,23 +18,26 @@
 aotpy/core/optical_sensor.py
 aotpy/core/source.py
 aotpy/core/telescope.py
 aotpy/core/time.py
 aotpy/core/wavefront_corrector.py
 aotpy/data/__init__.py
 aotpy/data/AOF/subap.fits
-aotpy/data/ERIS/subap.fits
+aotpy/data/ERIS/ho_subap.fits
+aotpy/data/ERIS/lo_subap.fits
 aotpy/data/NAOMI/zernike_control_modes.fits
+aotpy/data/PAPYRUS/T152_pupil.fits
 aotpy/io/__init__.py
 aotpy/io/base.py
 aotpy/io/fits/__init__.py
 aotpy/io/fits/_keywords.py
 aotpy/io/fits/reader.py
 aotpy/io/fits/utils.py
 aotpy/io/fits/writer.py
 aotpy/translators/__init__.py
 aotpy/translators/aof.py
 aotpy/translators/base.py
 aotpy/translators/ciao.py
 aotpy/translators/eris.py
 aotpy/translators/eso.py
-aotpy/translators/naomi.py
+aotpy/translators/naomi.py
+aotpy/translators/papyrus.py
```

### Comparing `aotpy-0.6.2/setup.cfg` & `aotpy-0.7.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6f74 7079 0d0a 7665 7273 696f   = aotpy..versio
-00000020: 6e20 3d20 302e 362e 320d 0a61 7574 686f  n = 0.6.2..autho
+00000020: 6e20 3d20 302e 372e 300d 0a61 7574 686f  n = 0.7.0..autho
 00000030: 7220 3d20 5469 6167 6f20 476f 6d65 730d  r = Tiago Gomes.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 7469 6167 6f67 6f6d 6573 4066 652e 7570  tiagogomes@fe.up
 00000060: 2e70 740d 0a64 6573 6372 6970 7469 6f6e  .pt..description
 00000070: 203d 2048 656c 7065 7220 7061 636b 6167   = Helper packag
 00000080: 6520 666f 7220 6861 6e64 6c69 6e67 2041  e for handling A
 00000090: 6461 7074 6976 6520 4f70 7469 6373 2054  daptive Optics T
@@ -12,53 +12,54 @@
 000000b0: 7461 6e64 6172 6420 6669 6c65 730d 0a6c  tandard files..l
 000000c0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 000000d0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
 000000e0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
 000000f0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
 00000100: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
 00000110: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-00000120: 6769 7468 7562 2e63 6f6d 2f6b 5977 7a6f  github.com/kYwzo
-00000130: 722f 616f 7470 790d 0a70 726f 6a65 6374  r/aotpy..project
-00000140: 5f75 726c 7320 3d20 0d0a 0942 7567 2054  _urls = ...Bug T
-00000150: 7261 636b 6572 203d 2068 7474 7073 3a2f  racker = https:/
-00000160: 2f67 6974 6875 622e 636f 6d2f 6b59 777a  /github.com/kYwz
-00000170: 6f72 2f61 6f74 7079 2f69 7373 7565 730d  or/aotpy/issues.
-00000180: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
-00000190: 0a09 4465 7665 6c6f 706d 656e 7420 5374  ..Development St
-000001a0: 6174 7573 203a 3a20 3420 2d20 4265 7461  atus :: 4 - Beta
-000001b0: 0d0a 0949 6e74 656e 6465 6420 4175 6469  ...Intended Audi
-000001c0: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
-000001d0: 5265 7365 6172 6368 0d0a 0950 726f 6772  Research...Progr
-000001e0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001f0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
-00000200: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-00000210: 4170 7072 6f76 6564 203a 3a20 4253 4420  Approved :: BSD 
-00000220: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
-00000230: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
-00000240: 2049 6e64 6570 656e 6465 6e74 0d0a 0954   Independent...T
-00000250: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
-00000260: 6963 2f45 6e67 696e 6565 7269 6e67 203a  ic/Engineering :
-00000270: 3a20 4173 7472 6f6e 6f6d 790d 0a0d 0a5b  : Astronomy....[
-00000280: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
-00000290: 6573 203d 2066 696e 643a 0d0a 696e 636c  es = find:..incl
-000002a0: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
-000002b0: 203d 2054 7275 650d 0a70 7974 686f 6e5f   = True..python_
-000002c0: 7265 7175 6972 6573 203d 203e 3d33 2e31  requires = >=3.1
-000002d0: 300d 0a69 6e73 7461 6c6c 5f72 6571 7569  0..install_requi
-000002e0: 7265 7320 3d20 0d0a 0961 7374 726f 7079  res = ...astropy
-000002f0: 3e3d 352e 312e 310d 0a09 6e75 6d70 793e  >=5.1.1...numpy>
-00000300: 3d31 2e32 300d 0a0d 0a5b 6f70 7469 6f6e  =1.20....[option
-00000310: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
-00000320: 0a61 6f74 7079 2e64 6174 6120 3d20 2a2f  .aotpy.data = */
-00000330: 2a2e 6669 7473 0d0a 0d0a 5b6f 7074 696f  *.fits....[optio
-00000340: 6e73 2e65 7874 7261 735f 7265 7175 6972  ns.extras_requir
-00000350: 655d 0d0a 6573 6f61 7263 6869 7665 203d  e]..esoarchive =
-00000360: 200d 0a09 7079 766f 3e3d 312e 340d 0a73   ...pyvo>=1.4..s
-00000370: 6176 6669 6c65 7320 3d20 0d0a 0973 6369  avfiles = ...sci
-00000380: 7079 3e3d 312e 330d 0a64 6f63 7320 3d20  py>=1.3..docs = 
-00000390: 0d0a 0973 7068 696e 780d 0a09 7370 6869  ...sphinx...sphi
-000003a0: 6e78 2d72 7464 2d74 6865 6d65 0d0a 616c  nx-rtd-theme..al
-000003b0: 6c20 3d20 0d0a 0970 7976 6f3e 3d31 2e34  l = ...pyvo>=1.4
-000003c0: 0d0a 0973 6369 7079 3e3d 312e 330d 0a0d  ...scipy>=1.3...
-000003d0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-000003e0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-000003f0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000120: 6769 7468 7562 2e63 6f6d 2f53 5441 522d  github.com/STAR-
+00000130: 504f 5254 2f61 6f74 7079 0d0a 7072 6f6a  PORT/aotpy..proj
+00000140: 6563 745f 7572 6c73 203d 200d 0a09 4275  ect_urls = ...Bu
+00000150: 6720 5472 6163 6b65 7220 3d20 6874 7470  g Tracker = http
+00000160: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
+00000170: 5441 522d 504f 5254 2f61 6f74 7079 2f69  TAR-PORT/aotpy/i
+00000180: 7373 7565 730d 0a63 6c61 7373 6966 6965  ssues..classifie
+00000190: 7273 203d 200d 0a09 4465 7665 6c6f 706d  rs = ...Developm
+000001a0: 656e 7420 5374 6174 7573 203a 3a20 3420  ent Status :: 4 
+000001b0: 2d20 4265 7461 0d0a 0949 6e74 656e 6465  - Beta...Intende
+000001c0: 6420 4175 6469 656e 6365 203a 3a20 5363  d Audience :: Sc
+000001d0: 6965 6e63 652f 5265 7365 6172 6368 0d0a  ience/Research..
+000001e0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000001f0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000200: 3a3a 2033 0d0a 094c 6963 656e 7365 203a  :: 3...License :
+00000210: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+00000220: 3a20 4253 4420 4c69 6365 6e73 650d 0a09  : BSD License...
+00000230: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000240: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+00000250: 6e74 0d0a 0954 6f70 6963 203a 3a20 5363  nt...Topic :: Sc
+00000260: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
+00000270: 7269 6e67 203a 3a20 4173 7472 6f6e 6f6d  ring :: Astronom
+00000280: 790d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  y....[options]..
+00000290: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+000002a0: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
+000002b0: 655f 6461 7461 203d 2054 7275 650d 0a70  e_data = True..p
+000002c0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+000002d0: 203e 3d33 2e31 300d 0a69 6e73 7461 6c6c   >=3.10..install
+000002e0: 5f72 6571 7569 7265 7320 3d20 0d0a 0961  _requires = ...a
+000002f0: 7374 726f 7079 3e3d 352e 312e 310d 0a09  stropy>=5.1.1...
+00000300: 6e75 6d70 793e 3d31 2e32 300d 0a0d 0a5b  numpy>=1.20....[
+00000310: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
+00000320: 6461 7461 5d0d 0a61 6f74 7079 2e64 6174  data]..aotpy.dat
+00000330: 6120 3d20 2a2f 2a2e 6669 7473 0d0a 0d0a  a = */*.fits....
+00000340: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
+00000350: 7265 7175 6972 655d 0d0a 6573 6f61 7263  require]..esoarc
+00000360: 6869 7665 203d 200d 0a09 7079 766f 3e3d  hive = ...pyvo>=
+00000370: 312e 340d 0a73 6176 6669 6c65 7320 3d20  1.4..savfiles = 
+00000380: 0d0a 0973 6369 7079 3e3d 312e 352e 300d  ...scipy>=1.5.0.
+00000390: 0a64 6f63 7320 3d20 0d0a 0973 7068 696e  .docs = ...sphin
+000003a0: 780d 0a09 7370 6869 6e78 2d72 7464 2d74  x...sphinx-rtd-t
+000003b0: 6865 6d65 0d0a 616c 6c20 3d20 0d0a 0970  heme..all = ...p
+000003c0: 7976 6f3e 3d31 2e34 0d0a 0973 6369 7079  yvo>=1.4...scipy
+000003d0: 3e3d 312e 352e 300d 0a0d 0a5b 6567 675f  >=1.5.0....[egg_
+000003e0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+000003f0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000400: 300d 0a0d 0a                             0....
```

