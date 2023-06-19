# Comparing `tmp/onedep_deposition-0.1.dev2.tar.gz` & `tmp/onedep_deposition-0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onedep_deposition-0.1.dev2.tar", last modified: Mon Jun 19 14:34:19 2023, max compression
+gzip compressed data, was "onedep_deposition-0.1.dev3.tar", last modified: Mon Jun 19 15:36:28 2023, max compression
```

## Comparing `onedep_deposition-0.1.dev2.tar` & `onedep_deposition-0.1.dev3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 14:34:19.875651 onedep_deposition-0.1.dev2/
--rw-r--r--   0 peisach    (502) staff       (20)      552 2023-06-13 13:04:02.000000 onedep_deposition-0.1.dev2/LICENSE
--rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-19 14:34:19.875110 onedep_deposition-0.1.dev2/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)     4641 2023-06-17 15:30:45.000000 onedep_deposition-0.1.dev2/README.md
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 14:34:19.870230 onedep_deposition-0.1.dev2/onedep_deposition/
--rw-r--r--   0 peisach    (502) staff       (20)       25 2023-06-19 14:21:15.000000 onedep_deposition-0.1.dev2/onedep_deposition/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 14:34:19.874408 onedep_deposition-0.1.dev2/onedep_deposition/cli/
--rw-r--r--   0 peisach    (502) staff       (20)        0 2023-06-17 17:42:03.000000 onedep_deposition-0.1.dev2/onedep_deposition/cli/__init__.py
--rw-r--r--   0 peisach    (502) staff       (20)    12091 2023-06-17 17:38:06.000000 onedep_deposition-0.1.dev2/onedep_deposition/cli/cli.py
--rw-r--r--   0 peisach    (502) staff       (20)    16794 2023-06-17 16:20:15.000000 onedep_deposition-0.1.dev2/onedep_deposition/constants.py
--rw-r--r--   0 peisach    (502) staff       (20)    14441 2023-06-19 14:33:49.000000 onedep_deposition-0.1.dev2/onedep_deposition/deposit_api.py
--rw-r--r--   0 peisach    (502) staff       (20)     9006 2023-06-15 13:32:19.000000 onedep_deposition-0.1.dev2/onedep_deposition/enum.py
--rw-r--r--   0 peisach    (502) staff       (20)      159 2023-06-08 16:58:15.000000 onedep_deposition-0.1.dev2/onedep_deposition/exceptions.py
--rw-r--r--   0 peisach    (502) staff       (20)    12949 2023-06-19 14:32:24.000000 onedep_deposition-0.1.dev2/onedep_deposition/models.py
--rw-r--r--   0 peisach    (502) staff       (20)     5806 2023-06-19 14:21:05.000000 onedep_deposition-0.1.dev2/onedep_deposition/rest_adapter.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 14:34:19.873368 onedep_deposition-0.1.dev2/onedep_deposition.egg-info/
--rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-19 14:34:19.000000 onedep_deposition-0.1.dev2/onedep_deposition.egg-info/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)      557 2023-06-19 14:34:19.000000 onedep_deposition-0.1.dev2/onedep_deposition.egg-info/SOURCES.txt
--rw-r--r--   0 peisach    (502) staff       (20)        1 2023-06-19 14:34:19.000000 onedep_deposition-0.1.dev2/onedep_deposition.egg-info/dependency_links.txt
--rw-r--r--   0 peisach    (502) staff       (20)       68 2023-06-19 14:34:19.000000 onedep_deposition-0.1.dev2/onedep_deposition.egg-info/entry_points.txt
--rw-r--r--   0 peisach    (502) staff       (20)       15 2023-06-19 14:34:19.000000 onedep_deposition-0.1.dev2/onedep_deposition.egg-info/requires.txt
--rw-r--r--   0 peisach    (502) staff       (20)       18 2023-06-19 14:34:19.000000 onedep_deposition-0.1.dev2/onedep_deposition.egg-info/top_level.txt
--rw-r--r--   0 peisach    (502) staff       (20)     1039 2023-06-17 17:50:36.000000 onedep_deposition-0.1.dev2/pyproject.toml
--rw-r--r--   0 peisach    (502) staff       (20)       38 2023-06-19 14:34:19.875802 onedep_deposition-0.1.dev2/setup.cfg
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 15:36:28.005573 onedep_deposition-0.1.dev3/
+-rw-r--r--   0 peisach    (502) staff       (20)      552 2023-06-13 13:04:02.000000 onedep_deposition-0.1.dev3/LICENSE
+-rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-19 15:36:28.005145 onedep_deposition-0.1.dev3/PKG-INFO
+-rw-r--r--   0 peisach    (502) staff       (20)     4641 2023-06-17 15:30:45.000000 onedep_deposition-0.1.dev3/README.md
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 15:36:28.000415 onedep_deposition-0.1.dev3/onedep_deposition/
+-rw-r--r--   0 peisach    (502) staff       (20)       25 2023-06-19 15:35:51.000000 onedep_deposition-0.1.dev3/onedep_deposition/__init__.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 15:36:28.004556 onedep_deposition-0.1.dev3/onedep_deposition/cli/
+-rw-r--r--   0 peisach    (502) staff       (20)        0 2023-06-17 17:42:03.000000 onedep_deposition-0.1.dev3/onedep_deposition/cli/__init__.py
+-rw-r--r--   0 peisach    (502) staff       (20)    12124 2023-06-19 15:35:16.000000 onedep_deposition-0.1.dev3/onedep_deposition/cli/cli.py
+-rw-r--r--   0 peisach    (502) staff       (20)    16794 2023-06-17 16:20:15.000000 onedep_deposition-0.1.dev3/onedep_deposition/constants.py
+-rw-r--r--   0 peisach    (502) staff       (20)    14441 2023-06-19 14:33:49.000000 onedep_deposition-0.1.dev3/onedep_deposition/deposit_api.py
+-rw-r--r--   0 peisach    (502) staff       (20)     9006 2023-06-15 13:32:19.000000 onedep_deposition-0.1.dev3/onedep_deposition/enum.py
+-rw-r--r--   0 peisach    (502) staff       (20)      159 2023-06-08 16:58:15.000000 onedep_deposition-0.1.dev3/onedep_deposition/exceptions.py
+-rw-r--r--   0 peisach    (502) staff       (20)    12948 2023-06-19 15:35:41.000000 onedep_deposition-0.1.dev3/onedep_deposition/models.py
+-rw-r--r--   0 peisach    (502) staff       (20)     5810 2023-06-19 15:34:56.000000 onedep_deposition-0.1.dev3/onedep_deposition/rest_adapter.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 15:36:28.003656 onedep_deposition-0.1.dev3/onedep_deposition.egg-info/
+-rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-19 15:36:27.000000 onedep_deposition-0.1.dev3/onedep_deposition.egg-info/PKG-INFO
+-rw-r--r--   0 peisach    (502) staff       (20)      557 2023-06-19 15:36:27.000000 onedep_deposition-0.1.dev3/onedep_deposition.egg-info/SOURCES.txt
+-rw-r--r--   0 peisach    (502) staff       (20)        1 2023-06-19 15:36:27.000000 onedep_deposition-0.1.dev3/onedep_deposition.egg-info/dependency_links.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       68 2023-06-19 15:36:27.000000 onedep_deposition-0.1.dev3/onedep_deposition.egg-info/entry_points.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       15 2023-06-19 15:36:27.000000 onedep_deposition-0.1.dev3/onedep_deposition.egg-info/requires.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       18 2023-06-19 15:36:27.000000 onedep_deposition-0.1.dev3/onedep_deposition.egg-info/top_level.txt
+-rw-r--r--   0 peisach    (502) staff       (20)     1039 2023-06-17 17:50:36.000000 onedep_deposition-0.1.dev3/pyproject.toml
+-rw-r--r--   0 peisach    (502) staff       (20)       38 2023-06-19 15:36:28.005741 onedep_deposition-0.1.dev3/setup.cfg
```

### Comparing `onedep_deposition-0.1.dev2/LICENSE` & `onedep_deposition-0.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev2/PKG-INFO` & `onedep_deposition-0.1.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedep_deposition
-Version: 0.1.dev2
+Version: 0.1.dev3
 Summary: Package for wrapping the OneDep deposition API services
 Author-email: Neli Jose da Fonseca Junior <neli@ebi.ac.uk>
 License: apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `onedep_deposition-0.1.dev2/README.md` & `onedep_deposition-0.1.dev3/README.md`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev2/onedep_deposition/cli/cli.py` & `onedep_deposition-0.1.dev3/onedep_deposition/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     click.echo(deposition)
 
 
 @deposition_group.command(name="get", help="Get deposition info")
 @click.argument("dep_id")
 @click.pass_context
 @create_api
-def get(api: DepositApi, ctx: Dict, dep_id: str):
+def get_deposition(api: DepositApi, ctx: Dict, dep_id: str):
     """`get` deposition command handler"""
     deposition = api.get_deposition(dep_id)
     click.echo(deposition)
 
 
 @deposition_group.command(name="status", help="Status of processing")
 @click.argument("dep_id")
@@ -175,15 +175,15 @@
     """`users` command group"""
 
 
 @users_group.command(name="get", help="Get users in deposition")
 @click.argument("dep_id")
 @click.pass_context
 @create_api
-def get(api: DepositApi, ctx: Dict, dep_id: str):
+def get_users(api: DepositApi, ctx: Dict, dep_id: str):
     """`get` users command handler"""
     users = api.get_users(dep_id)
     for user in users:
         click.echo(user)
         click.echo("---------------------------------")
 
 
@@ -205,15 +205,15 @@
 
 
 @users_group.command(name="remove", help="Remove an user from a deposition")
 @click.argument("dep_id")
 @click.option("-O", "--orcid", "orcid", multiple=False, help="User orcid to be removed from the deposition")
 @click.pass_context
 @create_api
-def remove(api: DepositApi, ctx: Dict, dep_id: str, orcid: str):
+def remove_user(api: DepositApi, ctx: Dict, dep_id: str, orcid: str):
     """`remove` command handler"""
     used_deleted = api.remove_user(dep_id, orcid)
     if used_deleted:
         click.echo(f"User {orcid} was removed from the deposition {dep_id}.")
 
 
 @click.group(name="files", help="Manage deposition files")
@@ -242,28 +242,28 @@
     click.echo(f"Uploaded file: {file}")
 
 
 @files_group.command(name="get", help="Get files in deposition")
 @click.argument("dep_id")
 @click.pass_context
 @create_api
-def get(api: DepositApi, ctx: Dict, dep_id: str):
+def get_files(api: DepositApi, ctx: Dict, dep_id: str):
     """`list` command handler"""
     files = api.get_files(dep_id)
     for file in files:
         click.echo(file)
         click.echo("---------------------------------")
 
 
 @files_group.command(name="remove", help="Remove a file from the deposition")
 @click.argument("dep_id")
 @click.argument("file_id")
 @click.pass_context
 @create_api
-def remove(api: DepositApi, ctx: Dict, dep_id: str, file_id: int):
+def remove_file(api: DepositApi, ctx: Dict, dep_id: str, file_id: int):
     """`remove` command handler"""
     file_removed = api.remove_file(dep_id, file_id)
     if file_removed:
         click.echo(f"File {file_id} was removed from the deposition {dep_id}.")
 
 
 @click.group()
```

### Comparing `onedep_deposition-0.1.dev2/onedep_deposition/constants.py` & `onedep_deposition-0.1.dev3/onedep_deposition/constants.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev2/onedep_deposition/deposit_api.py` & `onedep_deposition-0.1.dev3/onedep_deposition/deposit_api.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev2/onedep_deposition/enum.py` & `onedep_deposition-0.1.dev3/onedep_deposition/enum.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev2/onedep_deposition/models.py` & `onedep_deposition-0.1.dev3/onedep_deposition/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,8 +432,7 @@
     @property
     def details(self) -> str:
         return self._details
 
     @property
     def date(self) -> datetime:
         return self._date
-
```

### Comparing `onedep_deposition-0.1.dev2/onedep_deposition/rest_adapter.py` & `onedep_deposition-0.1.dev3/onedep_deposition/rest_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,26 +75,26 @@
                                             params=params, data=data, files=files, timeout=self._timeout)
         except requests.exceptions.RequestException as e:
             self._logger.error(msg=(str(e)))
             raise DepositApiException("Failed to access the API", 403) from e
         if response.status_code == 204:
             # Django is redirecting 204 to OneDep home page
             return Response(204)
+        is_success = 299 >= response.status_code >= 200
+        log_line = log_line_post.format(is_success, response.status_code, response.reason)
+        if not is_success:
+            self._logger.error(msg=log_line)
+            raise DepositApiException(response.reason, response.status_code)
         try:
             data_out = response.json()
         except (ValueError, JSONDecodeError) as e:
             self._logger.error(msg=log_line_post.format(False, None, e))
             raise DepositApiException("Bad JSON in response", 502) from e
-        is_success = 299 >= response.status_code >= 200
-        log_line = log_line_post.format(is_success, response.status_code, response.reason)
-        if is_success:
-            self._logger.debug(msg=log_line)
-            return Response(response.status_code, response.reason, data_out)
-        self._logger.error(msg=log_line)
-        raise DepositApiException(response.reason, response.status_code)
+        self._logger.debug(msg=log_line)
+        return Response(response.status_code, response.reason, data_out)
 
     def get(self, endpoint: str, params: Dict = None, content_type: str = "application/json") -> Response:
         """
         Perform GET requests
         :param endpoint: endpoint path
         :param params: Dictionary with requests params
         :param content_type Request content type
```

### Comparing `onedep_deposition-0.1.dev2/onedep_deposition.egg-info/PKG-INFO` & `onedep_deposition-0.1.dev3/onedep_deposition.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedep-deposition
-Version: 0.1.dev2
+Version: 0.1.dev3
 Summary: Package for wrapping the OneDep deposition API services
 Author-email: Neli Jose da Fonseca Junior <neli@ebi.ac.uk>
 License: apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `onedep_deposition-0.1.dev2/onedep_deposition.egg-info/SOURCES.txt` & `onedep_deposition-0.1.dev3/onedep_deposition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev2/pyproject.toml` & `onedep_deposition-0.1.dev3/pyproject.toml`

 * *Files identical despite different names*

