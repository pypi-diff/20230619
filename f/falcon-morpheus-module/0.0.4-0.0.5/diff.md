# Comparing `tmp/falcon_morpheus_module-0.0.4.tar.gz` & `tmp/falcon_morpheus_module-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_morpheus_module-0.0.4.tar", max compression
+gzip compressed data, was "falcon_morpheus_module-0.0.5.tar", max compression
```

## Comparing `falcon_morpheus_module-0.0.4.tar` & `falcon_morpheus_module-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     6251 2023-06-16 19:49:38.263575 falcon_morpheus_module-0.0.4/README.md
--rw-r--r--   0        0        0       61 2023-06-16 19:49:38.263575 falcon_morpheus_module-0.0.4/falcon_morpheus_module/__init__.py
--rw-r--r--   0        0        0     6656 2023-06-16 19:49:38.264575 falcon_morpheus_module-0.0.4/falcon_morpheus_module/dock_sftp_api.py
--rw-r--r--   0        0        0      325 2023-06-16 19:49:38.264575 falcon_morpheus_module-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6755 1970-01-01 00:00:00.000000 falcon_morpheus_module-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6251 2023-06-19 13:58:40.486323 falcon_morpheus_module-0.0.5/README.md
+-rw-r--r--   0        0        0       61 2023-06-19 13:58:40.486323 falcon_morpheus_module-0.0.5/falcon_morpheus_module/__init__.py
+-rw-r--r--   0        0        0     7266 2023-06-19 13:58:40.486323 falcon_morpheus_module-0.0.5/falcon_morpheus_module/dock_sftp_api.py
+-rw-r--r--   0        0        0      325 2023-06-19 13:58:40.486323 falcon_morpheus_module-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6755 1970-01-01 00:00:00.000000 falcon_morpheus_module-0.0.5/PKG-INFO
```

### Comparing `falcon_morpheus_module-0.0.4/README.md` & `falcon_morpheus_module-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `falcon_morpheus_module-0.0.4/falcon_morpheus_module/dock_sftp_api.py` & `falcon_morpheus_module-0.0.5/falcon_morpheus_module/dock_sftp_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,35 +86,59 @@
             self.base_url + f"/v1/sftp/{ticket}", headers=headers
         )
         if response.status_code == 204:
             print(f"SFTP user with ticket: {ticket} deleted successfully.")
         else:
             raise Exception(f"Error: {response.status_code}, {response.text}")
 
-    def request_file(self, filename, limit, page, file_type, column_names):
+    def request_file(
+        self,
+        filename,
+        limit,
+        page,
+        file_type,
+        column_names,
+        start_date=None,
+        end_date=None,
+    ):
         """
         A method to make a POST request to the API to fetch specific data.
 
         Parameters:
         filename (str): The name of the file.
         limit (int): Limit for the number of entries returned.
         page (int): Page number for pagination.
         file_type (str): The type of file being requested.
         column_names (list): The list of column names to be included in the response.
+        start_date (str): The start date for the creation_date filter.
+        end_date (str): The end date for the creation_date filter.
 
         Returns:
         Response from the API call.
         """
+        filter_string = ""
+        if start_date and end_date:
+            filter_string = f"""
+            filter: {{
+                creation_date: {{
+                    between: {{
+                        start: "{start_date}",
+                        end: "{end_date}"
+                    }}
+                }}
+            }},"""
+
         query_string = f"""
         query {{
             {filename}(
                 limit: {limit},
                 page: {page},
                 generate_file: true,
-                file_type: {file_type}
+                file_type: {file_type},
+                {filter_string}
             )
             {{
                 list {{
                     { ' '.join(column_names) }
                 }}
             }}
         }}"""
```

### Comparing `falcon_morpheus_module-0.0.4/PKG-INFO` & `falcon_morpheus_module-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon-morpheus-module
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: NG.CASH
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

