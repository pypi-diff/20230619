# Comparing `tmp/meow-sim-0.6.4.tar.gz` & `tmp/meow-sim-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.6.4.tar", last modified: Mon Jun 19 14:30:05 2023, max compression
+gzip compressed data, was "meow-sim-0.6.5.tar", last modified: Mon Jun 19 16:19:06 2023, max compression
```

## Comparing `meow-sim-0.6.4.tar` & `meow-sim-0.6.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:30:05.104225 meow-sim-0.6.4/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-19 14:30:01.000000 meow-sim-0.6.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-19 14:30:05.104225 meow-sim-0.6.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2023-06-19 14:30:01.000000 meow-sim-0.6.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:30:05.100225 meow-sim-0.6.4/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:30:05.100225 meow-sim-0.6.4/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8378 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     3855 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     6032 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:30:05.100225 meow-sim-0.6.4/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6191 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3938 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:30:05.100225 meow-sim-0.6.4/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4911 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10421 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    12146 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    17355 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     8099 2023-06-19 14:30:01.000000 meow-sim-0.6.4/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:30:05.100225 meow-sim-0.6.4/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-19 14:30:05.000000 meow-sim-0.6.4/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-19 14:30:05.000000 meow-sim-0.6.4/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 14:30:05.000000 meow-sim-0.6.4/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      444 2023-06-19 14:30:05.000000 meow-sim-0.6.4/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-19 14:30:05.000000 meow-sim-0.6.4/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1864 2023-06-19 14:30:01.000000 meow-sim-0.6.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 14:30:05.104225 meow-sim-0.6.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:30:05.104225 meow-sim-0.6.4/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-19 14:30:01.000000 meow-sim-0.6.4/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-19 14:30:01.000000 meow-sim-0.6.4/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-19 14:30:01.000000 meow-sim-0.6.4/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:19:06.175910 meow-sim-0.6.5/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-19 16:19:01.000000 meow-sim-0.6.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-19 16:19:06.175910 meow-sim-0.6.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-06-19 16:19:01.000000 meow-sim-0.6.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:19:06.175910 meow-sim-0.6.5/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:19:06.175910 meow-sim-0.6.5/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8378 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     6032 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:19:06.175910 meow-sim-0.6.5/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6191 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3938 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:19:06.175910 meow-sim-0.6.5/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4911 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10421 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    12794 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     4786 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    17355 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     8099 2023-06-19 16:19:01.000000 meow-sim-0.6.5/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:19:06.175910 meow-sim-0.6.5/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-19 16:19:06.000000 meow-sim-0.6.5/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-19 16:19:06.000000 meow-sim-0.6.5/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 16:19:06.000000 meow-sim-0.6.5/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      444 2023-06-19 16:19:06.000000 meow-sim-0.6.5/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-19 16:19:06.000000 meow-sim-0.6.5/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-06-19 16:19:01.000000 meow-sim-0.6.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 16:19:06.175910 meow-sim-0.6.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:19:06.175910 meow-sim-0.6.5/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-19 16:19:01.000000 meow-sim-0.6.5/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-19 16:19:01.000000 meow-sim-0.6.5/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-19 16:19:01.000000 meow-sim-0.6.5/tests/test_nbs.py
```

### Comparing `meow-sim-0.6.4/LICENSE` & `meow-sim-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/PKG-INFO` & `meow-sim-0.6.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.4
+Version: 0.6.5
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.4/README.md` & `meow-sim-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/__init__.py` & `meow-sim-0.6.5/meow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.6.4"
+__version__ = "0.6.5"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.6.4/meow/assets/silicon.csv` & `meow-sim-0.6.5/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/assets/silicon_oxide.csv` & `meow-sim-0.6.5/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/base_model.py` & `meow-sim-0.6.5/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/cache.py` & `meow-sim-0.6.5/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/cell.py` & `meow-sim-0.6.5/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/cross_section.py` & `meow-sim-0.6.5/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/eme/__init__.py` & `meow-sim-0.6.5/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/eme/common.py` & `meow-sim-0.6.5/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/eme/sax.py` & `meow-sim-0.6.5/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/environment.py` & `meow-sim-0.6.5/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/fde/lumerical.py` & `meow-sim-0.6.5/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/fde/tidy3d.py` & `meow-sim-0.6.5/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/gds_structures.py` & `meow-sim-0.6.5/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/geometries.py` & `meow-sim-0.6.5/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/integrate.py` & `meow-sim-0.6.5/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/materials.py` & `meow-sim-0.6.5/meow/materials.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,45 @@
 from scipy.constants import c
 from scipy.ndimage import map_coordinates
 from tidy3d import material_library
 
 from .base_model import BaseModel, _array
 from .environment import Environment
 
+MATERIAL_TYPES: Dict[str, type] = {}
+
 
 class Material(BaseModel):
     """a `Material` defines the refractive index of a `Structure` within an `Environment`."""
 
+    type: str = ""
+
     name: str = Field(description="the name of the material")
 
     meta: Dict[str, Any] = Field(
         default_factory=lambda: {}, description="metadata for the material"
     )
 
+    def __init_subclass__(cls):
+        MATERIAL_TYPES[cls.__name__] = cls
+
+    def __new__(cls, **kwargs):
+        cls = MATERIAL_TYPES.get(kwargs.get("type", cls.__name__), cls)
+        return BaseModel.__new__(cls)  # type: ignore
+
+    @validator("type", pre=True, always=True)
+    def validate_type(cls, value):
+        if not value:
+            value = getattr(cls, "__name__", "Geometry")
+        if value not in MATERIAL_TYPES:
+            raise ValueError(
+                f"Invalid Material type. Got: {value!r}. Valid types: {MATERIAL_TYPES}."
+            )
+        return value
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         MATERIALS[self.name] = self
 
     def __call__(self, env: Environment) -> NDArray[np.complex_]:
         """returns an array of the refractive index at the wavelengths specified by the environment"""
         raise NotImplementedError("Please use one of the Material child classes")
```

### Comparing `meow-sim-0.6.4/meow/mesh.py` & `meow-sim-0.6.5/meow/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,11 +142,11 @@
         """Y at Hz locations"""
         return self.Y_full[1::2, 1::2].view(_array)
 
     def __eq__(self, other):
         eq = True
         for k, v in self.dict().items():
             if isinstance(v, np.ndarray):
-                eq &= ((v - getattr(other, k)) < 1e-6).all()
+                eq &= bool(((v - getattr(other, k)) < 1e-6).all())
             else:
-                eq &= v == getattr(other, k)
+                eq &= bool(v == getattr(other, k))
         return eq
```

### Comparing `meow-sim-0.6.4/meow/mode.py` & `meow-sim-0.6.5/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/structures.py` & `meow-sim-0.6.5/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow/visualize.py` & `meow-sim-0.6.5/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.6.5/meow_sim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.4
+Version: 0.6.5
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.4/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.6.5/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/pyproject.toml` & `meow-sim-0.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.6.4"
+version = "0.6.5"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.6.4/tests/test_deserialization.py` & `meow-sim-0.6.5/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/tests/test_mode_operators.py` & `meow-sim-0.6.5/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.4/tests/test_nbs.py` & `meow-sim-0.6.5/tests/test_nbs.py`

 * *Files identical despite different names*

