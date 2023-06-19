# Comparing `tmp/pekat_vision_sdk-1.4.1.tar.gz` & `tmp/pekat_vision_sdk-1.4.2.tar.gz`

## Comparing `pekat_vision_sdk-1.4.1.tar` & `pekat_vision_sdk-1.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/PekatVisionSDK/__about__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/PekatVisionSDK/__init__.py
--rw-r--r--   0        0        0    12186 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/PekatVisionSDK/pekat_vision_instance.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/LICENSE
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/README.md
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/PekatVisionSDK/__about__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/PekatVisionSDK/__init__.py
+-rw-r--r--   0        0        0    12169 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/PekatVisionSDK/pekat_vision_instance.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/LICENSE
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/README.md
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/PKG-INFO
```

### Comparing `pekat_vision_sdk-1.4.1/PekatVisionSDK/pekat_vision_instance.py` & `pekat_vision_sdk-1.4.2/PekatVisionSDK/pekat_vision_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
     def __get_dist_path(self) -> Path:
         if self.dist_path:
             if self.dist_path.exists():
                 return self.dist_path
             else:
                 raise DistNotExists()
         elif platform.system() == "Windows":
-            program_files_path = Path(os.environ['systemdrive']) / "Program Files"
+            program_files_path = Path(os.environ["PROGRAMFILES"])
             for p in reversed(sorted(program_files_path.glob("PEKAT VISION *"))):
                 return program_files_path / p  # Path to the newest version of PEKAT VISION in Program Files
 
         raise DistNotFound()
 
     @staticmethod
     def __find_free_ports():
```

### Comparing `pekat_vision_sdk-1.4.1/LICENSE` & `pekat_vision_sdk-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pekat_vision_sdk-1.4.1/README.md` & `pekat_vision_sdk-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pekat_vision_sdk-1.4.1/pyproject.toml` & `pekat_vision_sdk-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pekat_vision_sdk-1.4.1/PKG-INFO` & `pekat_vision_sdk-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pekat-vision-sdk
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Python module for communication with PEKAT VISION
 Project-URL: Homepage, https://github.com/pekat-vision/pekat-vision-sdk-python
 Project-URL: repository, https://github.com/pekat-vision/pekat-vision-sdk-python.git
 Author-email: developers@pekatvision.com
 Maintainer-email: developers@pekatvision.com
 License-Expression: MIT
 License-File: LICENSE
```

