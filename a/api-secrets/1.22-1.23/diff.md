# Comparing `tmp/api_secrets-1.22.tar.gz` & `tmp/api_secrets-1.23.tar.gz`

## Comparing `api_secrets-1.22.tar` & `api_secrets-1.23.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 api_secrets-1.22/__init__.py
--rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 api_secrets-1.22/api_secrets.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 api_secrets-1.22/LICENSE
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 api_secrets-1.22/README.md
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 api_secrets-1.22/pyproject.toml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 api_secrets-1.22/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 api_secrets-1.23/__init__.py
+-rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 api_secrets-1.23/api_secrets.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 api_secrets-1.23/LICENSE
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 api_secrets-1.23/README.md
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 api_secrets-1.23/pyproject.toml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 api_secrets-1.23/PKG-INFO
```

### Comparing `api_secrets-1.22/api_secrets.py` & `api_secrets-1.23/api_secrets.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,17 +161,15 @@
         password = password.strip()
 
         if len(password) > 8:
             return password
         else:
             print("Password appears too short. Please check you copied correctly")    
 
-
-
-if __name__ == '__main__':
+def main():
     menu = {
         "1": "Print secret",
         "2": "Write secret",
         "3": "Delete secret"
         }
 
     print("Menu")
@@ -206,8 +204,12 @@
     if opt == "3":
         system_instance = get_system_instance()
         user = get_user()
         delete_secret(system_instance, user)
         print("Successfully deleted secret")
 
 
-    input("Press enter to exit")
+    input("Press enter to exit")   
+
+if __name__ == '__main__':
+    main()
+
```

### Comparing `api_secrets-1.22/LICENSE` & `api_secrets-1.23/LICENSE`

 * *Files identical despite different names*

### Comparing `api_secrets-1.22/pyproject.toml` & `api_secrets-1.23/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "api_secrets"
-version = "1.22"
+version = "1.23"
 authors = [
   { name="Brodie Zambergs", email="brodie.zambergs@monash.edu" },
 ]
 description = "A wrapper package to manage specific cross-platform management requirements including supplementary data (i.e. URLs)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `api_secrets-1.22/PKG-INFO` & `api_secrets-1.23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api_secrets
-Version: 1.22
+Version: 1.23
 Summary: A wrapper package to manage specific cross-platform management requirements including supplementary data (i.e. URLs)
 Author-email: Brodie Zambergs <brodie.zambergs@monash.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

