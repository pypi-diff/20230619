# Comparing `tmp/overwatch_ci_helper-0.1.0.tar.gz` & `tmp/overwatch_ci_helper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overwatch_ci_helper-0.1.0.tar", max compression
+gzip compressed data, was "overwatch_ci_helper-0.1.1.tar", max compression
```

## Comparing `overwatch_ci_helper-0.1.0.tar` & `overwatch_ci_helper-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-19 14:19:49.240182 overwatch_ci_helper-0.1.0/README.md
--rw-r--r--   0        0        0     7040 2023-06-19 19:38:40.944208 overwatch_ci_helper-0.1.0/overwatch_ci_helper/needs.py
--rw-r--r--   0        0        0     2297 2023-06-19 19:42:22.953731 overwatch_ci_helper-0.1.0/overwatch_ci_helper/template.config.yaml
--rw-r--r--   0        0        0      519 2023-06-19 19:48:56.612908 overwatch_ci_helper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      435 1970-01-01 00:00:00.000000 overwatch_ci_helper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1037 2023-06-19 20:15:21.224854 overwatch_ci_helper-0.1.1/README.md
+-rw-r--r--   0        0        0     7126 2023-06-19 20:15:21.224854 overwatch_ci_helper-0.1.1/overwatch_ci_helper/needs.py
+-rw-r--r--   0        0        0     2297 2023-06-19 20:15:21.224854 overwatch_ci_helper-0.1.1/overwatch_ci_helper/template.config.yaml
+-rw-r--r--   0        0        0      519 2023-06-19 20:15:21.228854 overwatch_ci_helper-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 overwatch_ci_helper-0.1.1/PKG-INFO
```

### Comparing `overwatch_ci_helper-0.1.0/overwatch_ci_helper/needs.py` & `overwatch_ci_helper-0.1.1/overwatch_ci_helper/needs.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,16 @@
         if dependency in list(all_containers.keys()):
             print(f"Cleaning up {dependency}")
             container = all_containers[dependency]
             container.stop()
             container.wait()
             mounts = container.attrs['Mounts']
             for mount in mounts:
+                if mount['Destination'] == '/root/.dcp':
+                    continue
                 if os.path.exists(mount['Source']) and os.path.isdir(mount['Source']):
                     shutil.rmtree(mount['Source'])
                 elif os.path.exists(mount['Source']):
                     os.remove(mount['Source'])
             container.remove()
             print(f"Done cleaning up {dependency}")
     print("Finished cleaning up all dependencies")
```

### Comparing `overwatch_ci_helper-0.1.0/overwatch_ci_helper/template.config.yaml` & `overwatch_ci_helper-0.1.1/overwatch_ci_helper/template.config.yaml`

 * *Files identical despite different names*

### Comparing `overwatch_ci_helper-0.1.0/pyproject.toml` & `overwatch_ci_helper-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "overwatch-ci-helper"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Hamada Gasmallah <hamada@distributive.network>"]
 readme = "README.md"
 packages = [{include = "overwatch_ci_helper"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

