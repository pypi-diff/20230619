# Comparing `tmp/rouse-0.1.0.tar.gz` & `tmp/rouse-0.1.1.tar.gz`

## Comparing `rouse-0.1.0.tar` & `rouse-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    31364 2020-02-02 00:00:00.000000 rouse-0.1.0/rouse.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 rouse-0.1.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 rouse-0.1.0/LICENSE
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 rouse-0.1.0/README.md
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 rouse-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 rouse-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    31346 2020-02-02 00:00:00.000000 rouse-0.1.1/rouse.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 rouse-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 rouse-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 rouse-0.1.1/README.md
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 rouse-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 rouse-0.1.1/PKG-INFO
```

### Comparing `rouse-0.1.0/rouse.py` & `rouse-0.1.1/rouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,16 +324,16 @@
             V = self._dynamics['V']
             e = self._dynamics['exp_w_1']
             G = V @ (e[:, None] * (V.T @ self.F))
         
         self._dynamics['G'] = G
         self._dynamics['ss_M'] = self._dynamics['ss_CoD'] @ self.F
 
-        if override_full_update: # pragma: no cover
-            self._dynamics['needs_updating'] = True
+        if override_full_update:
+            self._dynamics['needs_updating'] = False
 
     def check_dynamics(self, dt=None, run_if_necessary=True):
         """
         Check that dynamics are set up properly
 
         Parameters
         ----------
```

### Comparing `rouse-0.1.0/LICENSE` & `rouse-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rouse-0.1.0/README.md` & `rouse-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rouse-0.1.0/pyproject.toml` & `rouse-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build]
 include = [
   "rouse.py" # Have to explicitly include single module
 ]
 
 [project]
 name = "rouse"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Simon Grosse-Holz", email="sgh256@mit.edu" }
 ]
 description = "An implementation of the Rouse model of polymer dynamics"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `rouse-0.1.0/PKG-INFO` & `rouse-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rouse
-Version: 0.1.0
+Version: 0.1.1
 Summary: An implementation of the Rouse model of polymer dynamics
 Project-URL: Homepage, https://github.com/OpenTrajectoryAnalysis/rouse
 Project-URL: Documentation, https://rouse.readthedocs.org/en/latest
 Project-URL: Bug Tracker, https://github.com/OpenTrajectoryAnalysis/rouse/issues
 Author-email: Simon Grosse-Holz <sgh256@mit.edu>
 License: MIT License
```

