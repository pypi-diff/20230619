# Comparing `tmp/glocalx-0.0.4.tar.gz` & `tmp/glocalx-0.0.5.tar.gz`

## Comparing `glocalx-0.0.4.tar` & `glocalx-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/__init__.py
--rwxr-xr-x   0        0        0     9852 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/api.py
--rwxr-xr-x   0        0        0     4808 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/callbacks.py
--rwxr-xr-x   0        0        0    26407 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/evaluators.py
--rwxr-xr-x   0        0        0     8618 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/generators.py
--rwxr-xr-x   0        0        0    24742 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/glocalx.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/glocax_probabilistic.py
--rwxr-xr-x   0        0        0    12664 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/models.py
--rwxr-xr-x   0        0        0      969 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/requirements.txt
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/serialization.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/data/dummy/dummy_dataset.csv
--rw-r--r--   0        0        0    32544 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/data/dummy/dummy_model.h5
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/data/dummy/dummy_rules.json
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/data/loaders/adult_info.json
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 glocalx-0.0.4/src/glocalx/loaders/lore.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 glocalx-0.0.4/LICENSE
--rwxr-xr-x   0        0        0    11369 2020-02-02 00:00:00.000000 glocalx-0.0.4/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 glocalx-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    12213 2020-02-02 00:00:00.000000 glocalx-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/__init__.py
+-rwxr-xr-x   0        0        0     9852 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/api.py
+-rwxr-xr-x   0        0        0     4808 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/callbacks.py
+-rwxr-xr-x   0        0        0    26407 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/evaluators.py
+-rwxr-xr-x   0        0        0     8618 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/generators.py
+-rwxr-xr-x   0        0        0    24742 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/glocalx.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/glocax_probabilistic.py
+-rwxr-xr-x   0        0        0    12664 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/models.py
+-rwxr-xr-x   0        0        0      969 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/requirements.txt
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/serialization.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/data/dummy/dummy_dataset.csv
+-rw-r--r--   0        0        0    32544 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/data/dummy/dummy_model.h5
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/data/dummy/dummy_rules.json
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/data/loaders/adult_info.json
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 glocalx-0.0.5/src/glocalx/loaders/lore.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 glocalx-0.0.5/LICENSE
+-rwxr-xr-x   0        0        0    11369 2020-02-02 00:00:00.000000 glocalx-0.0.5/README.md
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 glocalx-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 glocalx-0.0.5/PKG-INFO
```

### Comparing `glocalx-0.0.4/src/glocalx/.gitignore` & `glocalx-0.0.5/src/glocalx/.gitignore`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.4/src/glocalx/api.py` & `glocalx-0.0.5/src/glocalx/api.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.4/src/glocalx/callbacks.py` & `glocalx-0.0.5/src/glocalx/callbacks.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.4/src/glocalx/evaluators.py` & `glocalx-0.0.5/src/glocalx/evaluators.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.4/src/glocalx/generators.py` & `glocalx-0.0.5/src/glocalx/generators.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.4/src/glocalx/glocalx.py` & `glocalx-0.0.5/src/glocalx/glocalx.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.4/src/glocalx/glocax_probabilistic.py` & `glocalx-0.0.5/src/glocalx/glocax_probabilistic.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.4/src/glocalx/models.py` & `glocalx-0.0.5/src/glocalx/models.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.4/src/glocalx/requirements.txt` & `glocalx-0.0.5/src/glocalx/requirements.txt`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.4/src/glocalx/serialization.py` & `glocalx-0.0.5/src/glocalx/serialization.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.4/src/glocalx/data/dummy/dummy_model.h5` & `glocalx-0.0.5/src/glocalx/data/dummy/dummy_model.h5`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.4/src/glocalx/data/loaders/adult_info.json` & `glocalx-0.0.5/src/glocalx/data/loaders/adult_info.json`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.4/src/glocalx/loaders/lore.py` & `glocalx-0.0.5/src/glocalx/loaders/lore.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.4/LICENSE` & `glocalx-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.4/README.md` & `glocalx-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.4/pyproject.toml` & `glocalx-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "glocalx"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Mattia Setzu", email="mattia.setzu@di.unipi.it" },
 ]
 description = "Generating global explanations from local ones."
 readme = "README.md"
 requires-python = ">=3.8, <3.10"
 classifiers = [
@@ -22,14 +22,14 @@
 ]
 dependencies = [
     "click==7.1.2",
     "logzero==1.6.2",
     "numpy",
     "pandas",
     "scikit-learn",
-    "scipy==1.5.4",
-    "tensorflow==2.5.0",
+    "scipy",
+    "tensorflow==2.5",
 ]
 
 [project.urls]
 	"Homepage" = "https://github.com/msetzu/glocalx"
 	"Bug Tracker" = "https://github.com/msetzu/glocalx/issues"
```

### Comparing `glocalx-0.0.4/PKG-INFO` & `glocalx-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glocalx
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generating global explanations from local ones.
 Project-URL: Homepage, https://github.com/msetzu/glocalx
 Project-URL: Bug Tracker, https://github.com/msetzu/glocalx/issues
 Author-email: Mattia Setzu <mattia.setzu@di.unipi.it>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: <3.10,>=3.8
 Requires-Dist: click==7.1.2
 Requires-Dist: logzero==1.6.2
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
-Requires-Dist: scipy==1.5.4
-Requires-Dist: tensorflow==2.5.0
+Requires-Dist: scipy
+Requires-Dist: tensorflow==2.5
 Description-Content-Type: text/markdown
 
 # GLocalX - Global through Local Explainability
 
 Explanations come in two forms: local, explaining a single model prediction, and global, explaining all model predictions. The Local to Global (L2G) problem consists in bridging these two family of explanations. Simply put, we generate global explanations by merging local ones.
 
 ## The algorithm
```

