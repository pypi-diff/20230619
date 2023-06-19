# Comparing `tmp/deeplearningoptimized-1.1.4.tar.gz` & `tmp/deeplearningoptimized-1.1.5.tar.gz`

## Comparing `deeplearningoptimized-1.1.4.tar` & `deeplearningoptimized-1.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/src/Pipfile
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/src/Pipfile.lock
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/src/DeepLearningOptimized/Data_DL.py
--rw-r--r--   0        0        0    18718 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/src/DeepLearningOptimized/Model_DL.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/src/DeepLearningOptimized/__init__.py
--rw-r--r--   0        0        0   257492 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/src/DeepLearningOptimized/deepC.dll
--rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/src/DeepLearningOptimized/deepC.so
--rw-r--r--   0        0        0   380928 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/src/DeepLearningOptimized/deepCUDA.dll
--rw-r--r--   0        0        0    23230 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/src/DeepLearningOptimized/interface.c
--rw-r--r--   0        0        0    19069 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/src/DeepLearningOptimized/interface.cu
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/src/DeepLearningOptimized/interface.cuh
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/src/DeepLearningOptimized/interface.h
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/LICENSE.lic
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/README.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/src/Pipfile
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/src/Pipfile.lock
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/src/DeepLearningOptimized/Data_DL.py
+-rw-r--r--   0        0        0    18718 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/src/DeepLearningOptimized/Model_DL.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/src/DeepLearningOptimized/__init__.py
+-rw-r--r--   0        0        0   257492 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/src/DeepLearningOptimized/deepC.dll
+-rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/src/DeepLearningOptimized/deepC.so
+-rw-r--r--   0        0        0   380928 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/src/DeepLearningOptimized/deepCUDA.dll
+-rw-r--r--   0        0        0    23230 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/src/DeepLearningOptimized/interface.c
+-rw-r--r--   0        0        0    19069 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/src/DeepLearningOptimized/interface.cu
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/src/DeepLearningOptimized/interface.cuh
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/src/DeepLearningOptimized/interface.h
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/LICENSE.lic
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/README.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.5/PKG-INFO
```

### Comparing `deeplearningoptimized-1.1.4/src/Pipfile.lock` & `deeplearningoptimized-1.1.5/src/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.4/src/DeepLearningOptimized/Data_DL.py` & `deeplearningoptimized-1.1.5/src/DeepLearningOptimized/Data_DL.py`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.4/src/DeepLearningOptimized/Model_DL.py` & `deeplearningoptimized-1.1.5/src/DeepLearningOptimized/Model_DL.py`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.4/src/DeepLearningOptimized/deepC.dll` & `deeplearningoptimized-1.1.5/src/DeepLearningOptimized/deepC.dll`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.4/src/DeepLearningOptimized/deepC.so` & `deeplearningoptimized-1.1.5/src/DeepLearningOptimized/deepC.so`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.4/src/DeepLearningOptimized/deepCUDA.dll` & `deeplearningoptimized-1.1.5/src/DeepLearningOptimized/deepCUDA.dll`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.4/src/DeepLearningOptimized/interface.c` & `deeplearningoptimized-1.1.5/src/DeepLearningOptimized/interface.c`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.4/src/DeepLearningOptimized/interface.cu` & `deeplearningoptimized-1.1.5/src/DeepLearningOptimized/interface.cu`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.4/src/DeepLearningOptimized/interface.cuh` & `deeplearningoptimized-1.1.5/src/DeepLearningOptimized/interface.cuh`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.4/src/DeepLearningOptimized/interface.h` & `deeplearningoptimized-1.1.5/src/DeepLearningOptimized/interface.h`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.4/LICENSE.lic` & `deeplearningoptimized-1.1.5/LICENSE.lic`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.4/pyproject.toml` & `deeplearningoptimized-1.1.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "DeepLearningOptimized"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
   { name="Liam Roan Watson", email="lrwatson@uwaterloo.ca" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

