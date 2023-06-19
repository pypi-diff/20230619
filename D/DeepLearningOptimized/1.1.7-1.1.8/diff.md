# Comparing `tmp/deeplearningoptimized-1.1.7.tar.gz` & `tmp/deeplearningoptimized-1.1.8.tar.gz`

## Comparing `deeplearningoptimized-1.1.7.tar` & `deeplearningoptimized-1.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/src/Pipfile
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/src/Pipfile.lock
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/src/DeepLearningOptimized/Data_DL.py
--rw-r--r--   0        0        0    18742 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/src/DeepLearningOptimized/Model_DL.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/src/DeepLearningOptimized/__init__.py
--rw-r--r--   0        0        0   257492 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/src/DeepLearningOptimized/deepC.dll
--rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/src/DeepLearningOptimized/deepC.so
--rw-r--r--   0        0        0   380928 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/src/DeepLearningOptimized/deepCUDA.dll
--rw-r--r--   0        0        0    23230 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/src/DeepLearningOptimized/interface.c
--rw-r--r--   0        0        0    19069 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/src/DeepLearningOptimized/interface.cu
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/src/DeepLearningOptimized/interface.cuh
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/src/DeepLearningOptimized/interface.h
--rw-r--r--   0        0        0    16660 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/src/DeepLearningOptimized/interface.o
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/LICENSE.lic
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/README.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/pyproject.toml
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/src/Pipfile
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/src/Pipfile.lock
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/src/DeepLearningOptimized/Data_DL.py
+-rw-r--r--   0        0        0    18722 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/src/DeepLearningOptimized/Model_DL.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/src/DeepLearningOptimized/__init__.py
+-rw-r--r--   0        0        0   257492 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/src/DeepLearningOptimized/deepC.dll
+-rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/src/DeepLearningOptimized/deepC.so
+-rw-r--r--   0        0        0   380928 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/src/DeepLearningOptimized/deepCUDA.dll
+-rw-r--r--   0        0        0    23230 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/src/DeepLearningOptimized/interface.c
+-rw-r--r--   0        0        0    19069 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/src/DeepLearningOptimized/interface.cu
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/src/DeepLearningOptimized/interface.cuh
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/src/DeepLearningOptimized/interface.h
+-rw-r--r--   0        0        0    16660 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/src/DeepLearningOptimized/interface.o
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/LICENSE.lic
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/README.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.8/PKG-INFO
```

### Comparing `deeplearningoptimized-1.1.7/src/Pipfile.lock` & `deeplearningoptimized-1.1.8/src/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.7/src/DeepLearningOptimized/Data_DL.py` & `deeplearningoptimized-1.1.8/src/DeepLearningOptimized/Data_DL.py`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.7/src/DeepLearningOptimized/Model_DL.py` & `deeplearningoptimized-1.1.8/src/DeepLearningOptimized/Model_DL.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 getcontext().prec = 64
 
 c_type = c_double
 
 mydir = str(pathlib.Path(__file__).parent.resolve())
 
 if os.system("nvcc --version") == 0:
-    clib = cdll.LoadLibrary(mydir + "\\deepCUDA.dll")
+    clib = WinDLL(mydir + "\\deepCUDA.dll")
     
     c_type = c_float
 elif os.name == "nt":
     os.system("cls")
-    clib = cdll.LoadLibrary(mydir + "\\deepC.dll")
+    clib = WinDLL(mydir + "\\deepC.dll")
 else:
     os.system("clear")
     clib = CDLL(mydir + "/deepC.so")
     
 def findsize(hidden_sizes, bias_count):
     total_size = 0
```

### Comparing `deeplearningoptimized-1.1.7/src/DeepLearningOptimized/deepC.dll` & `deeplearningoptimized-1.1.8/src/DeepLearningOptimized/deepC.dll`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.7/src/DeepLearningOptimized/deepC.so` & `deeplearningoptimized-1.1.8/src/DeepLearningOptimized/deepC.so`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.7/src/DeepLearningOptimized/deepCUDA.dll` & `deeplearningoptimized-1.1.8/src/DeepLearningOptimized/deepCUDA.dll`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.7/src/DeepLearningOptimized/interface.c` & `deeplearningoptimized-1.1.8/src/DeepLearningOptimized/interface.c`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.7/src/DeepLearningOptimized/interface.cu` & `deeplearningoptimized-1.1.8/src/DeepLearningOptimized/interface.cu`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.7/src/DeepLearningOptimized/interface.cuh` & `deeplearningoptimized-1.1.8/src/DeepLearningOptimized/interface.cuh`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.7/src/DeepLearningOptimized/interface.h` & `deeplearningoptimized-1.1.8/src/DeepLearningOptimized/interface.h`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.7/src/DeepLearningOptimized/interface.o` & `deeplearningoptimized-1.1.8/src/DeepLearningOptimized/interface.o`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.7/LICENSE.lic` & `deeplearningoptimized-1.1.8/LICENSE.lic`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.7/pyproject.toml` & `deeplearningoptimized-1.1.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "DeepLearningOptimized"
-version = "1.1.7"
+version = "1.1.8"
 authors = [
   { name="Liam Roan Watson", email="lrwatson@uwaterloo.ca" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

