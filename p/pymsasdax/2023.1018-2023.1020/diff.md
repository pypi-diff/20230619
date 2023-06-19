# Comparing `tmp/pymsasdax-2023.1018.tar.gz` & `tmp/pymsasdax-2023.1020.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymsasdax-2023.1018.tar", last modified: Thu Apr 27 22:08:03 2023, max compression
+gzip compressed data, was "pymsasdax-2023.1020.tar", last modified: Mon Jun 19 16:23:27 2023, max compression
```

## Comparing `pymsasdax-2023.1018.tar` & `pymsasdax-2023.1020.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 22:08:03.336124 pymsasdax-2023.1018/
--rw-rw-rw-   0        0        0     1084 2023-02-20 22:20:56.000000 pymsasdax-2023.1018/LICENSE
--rw-rw-rw-   0        0        0        0 2023-02-21 01:10:15.000000 pymsasdax-2023.1018/MANIFEST.in
--rw-rw-rw-   0        0        0     6087 2023-04-27 22:08:03.333774 pymsasdax-2023.1018/PKG-INFO
--rw-rw-rw-   0        0        0     4252 2023-04-27 22:04:13.000000 pymsasdax-2023.1018/README.md
--rw-rw-rw-   0        0        0     1218 2023-04-27 22:06:35.000000 pymsasdax-2023.1018/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 22:08:03.336965 pymsasdax-2023.1018/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 22:08:03.276071 pymsasdax-2023.1018/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 22:08:03.300255 pymsasdax-2023.1018/src/pymsasdax/
--rw-rw-rw-   0        0        0       23 2023-04-27 22:06:35.000000 pymsasdax-2023.1018/src/pymsasdax/__init__.py
--rw-rw-rw-   0        0        0     6925 2023-04-27 22:02:19.000000 pymsasdax-2023.1018/src/pymsasdax/dax.py
-drwxrwxrwx   0        0        0        0 2023-04-27 22:08:03.326682 pymsasdax-2023.1018/src/pymsasdax.egg-info/
--rw-rw-rw-   0        0        0     6087 2023-04-27 22:08:03.000000 pymsasdax-2023.1018/src/pymsasdax.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-04-27 22:08:03.000000 pymsasdax-2023.1018/src/pymsasdax.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 22:08:03.000000 pymsasdax-2023.1018/src/pymsasdax.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-27 22:08:03.000000 pymsasdax-2023.1018/src/pymsasdax.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-27 22:08:03.000000 pymsasdax-2023.1018/src/pymsasdax.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 16:23:27.303141 pymsasdax-2023.1020/
+-rw-rw-rw-   0        0        0     1084 2023-02-20 22:20:56.000000 pymsasdax-2023.1020/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-02-21 01:10:15.000000 pymsasdax-2023.1020/MANIFEST.in
+-rw-rw-rw-   0        0        0     6177 2023-06-19 16:23:27.298208 pymsasdax-2023.1020/PKG-INFO
+-rw-rw-rw-   0        0        0     4342 2023-06-19 16:14:21.000000 pymsasdax-2023.1020/README.md
+-rw-rw-rw-   0        0        0     1218 2023-06-19 16:21:39.000000 pymsasdax-2023.1020/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 16:23:27.304772 pymsasdax-2023.1020/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 16:23:27.206008 pymsasdax-2023.1020/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 16:23:27.239419 pymsasdax-2023.1020/src/pymsasdax/
+-rw-rw-rw-   0        0        0       52 2023-06-19 16:21:39.000000 pymsasdax-2023.1020/src/pymsasdax/__init__.py
+-rw-rw-rw-   0        0        0     7008 2023-06-19 15:59:04.000000 pymsasdax-2023.1020/src/pymsasdax/dax.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:23:27.287981 pymsasdax-2023.1020/src/pymsasdax.egg-info/
+-rw-rw-rw-   0        0        0     6177 2023-06-19 16:23:27.000000 pymsasdax-2023.1020/src/pymsasdax.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-06-19 16:23:27.000000 pymsasdax-2023.1020/src/pymsasdax.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 16:23:27.000000 pymsasdax-2023.1020/src/pymsasdax.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-19 16:23:27.000000 pymsasdax-2023.1020/src/pymsasdax.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-19 16:23:27.000000 pymsasdax-2023.1020/src/pymsasdax.egg-info/top_level.txt
```

### Comparing `pymsasdax-2023.1018/LICENSE` & `pymsasdax-2023.1020/LICENSE`

 * *Files identical despite different names*

### Comparing `pymsasdax-2023.1018/PKG-INFO` & `pymsasdax-2023.1020/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymsasdax
-Version: 2023.1018
+Version: 2023.1020
 Summary: Run DAX queries against Analysis Services and get Pandas Dataframes
 Author-email: Gage Renzi <gagerenzi+pypy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 grenzi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -119,14 +119,16 @@
     print(df)
 ```
 
 # Dev Notes
 
 ## Version History
 
+* 2023.1020
+  * fix timeout not being honored as CommandTimeout
 * 2023.1018
   * fix bug using effective_user_name or kwargs
 * ~~2023.1017~~
   * ~~fix bug using effective_user_name~~
 * 2023.1016
   * Add at least some docstrings
   * Add Premium XMLA endpoint example
@@ -141,15 +143,15 @@
 
 Yes. There aren't any. Feel free to submit a PR. 
 
 ## Building
 
 This might not be right but if you ever go to update pypi - 
 ```
-bumpver update --minor
+bumpver update --dry --set-version="2023.1020"
 pip-compile pyproject.toml
 python -m pip install -e . 
 #test
 python -m build
 twine check dist/*
 twine upload dist/*
 ```
```

### Comparing `pymsasdax-2023.1018/README.md` & `pymsasdax-2023.1020/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,16 @@
     print(df)
 ```
 
 # Dev Notes
 
 ## Version History
 
+* 2023.1020
+  * fix timeout not being honored as CommandTimeout
 * 2023.1018
   * fix bug using effective_user_name or kwargs
 * ~~2023.1017~~
   * ~~fix bug using effective_user_name~~
 * 2023.1016
   * Add at least some docstrings
   * Add Premium XMLA endpoint example
@@ -104,15 +106,15 @@
 
 Yes. There aren't any. Feel free to submit a PR. 
 
 ## Building
 
 This might not be right but if you ever go to update pypi - 
 ```
-bumpver update --minor
+bumpver update --dry --set-version="2023.1020"
 pip-compile pyproject.toml
 python -m pip install -e . 
 #test
 python -m build
 twine check dist/*
 twine upload dist/*
 ```
```

### Comparing `pymsasdax-2023.1018/pyproject.toml` & `pymsasdax-2023.1020/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools", ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pymsasdax"
-version = "2023.1018"
+version = "2023.1020"
 description = "Run DAX queries against Analysis Services and get Pandas Dataframes"
 readme = "README.md"
 authors = [{ name = "Gage Renzi", email = "gagerenzi+pypy@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -27,15 +27,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pip-tools"]
 
 [project.urls]
 Homepage = "https://github.com/grenzi/pymsasdax"
 
 [tool.bumpver]
-current_version = "2023.1018"
+current_version = "2023.1020"
 version_pattern = "YYYY.BUILD"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `pymsasdax-2023.1018/src/pymsasdax/dax.py` & `pymsasdax-2023.1020/src/pymsasdax/dax.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,40 +12,41 @@
     uid (str): User ID for authentication. Default is empty string.
     password (str): Password for authentication. Default is empty string.
     effective_user_name (str): Username to impersonate, usually a UPN, such as joe@contoso.com
     tidy_column_names (bool): Flag for tidying column names. Default is True.
     tidy_map_function (function): A function to tidy column names. Default is to use the internal one, which leaves capitalization alone, replaces spaces with underscores, and removes square brackets.
     timeout (int): Timeout period (in seconds) for running queries. Default is 30.
     conn_str (str): Optional connection string for the connection.
-    **kwargs: Additional keyword value pairs, will be added to the connection string. 
+    **kwargs: Additional keyword value pairs, will be added to the connection string.
 
     Raises:
     ValueError: If initial_catalog and data_source are not specified when conn_str is not passed.
 
     Methods:
     _handle_oledb_field(f): Handles different data types returned from OleDbConnection query.
     _cleanup_column_name(c): Cleans up the column name by replacing some characters with underscores.
     __enter__(): Opens the connection when entering the context.
     __exit__(exc_type, exc_value, traceback): Closes the connection when exiting the context.
     query(daxcmd): Executes a DAX query on the connected server and returns the result as a Pandas DataFrame.
 
     Returns: Nothing
     """
+
     def __init__(
         self,
         initial_catalog=None,
         data_source=None,
         uid="",
         password="",
         effective_user_name=None,
         tidy_column_names=True,
         tidy_map_function=None,
         timeout=30,
         conn_str=None,
-        **kwargs
+        **kwargs,
     ):
         """Initializes the Connection object."""
         if conn_str is not None:
             self._connection_string = conn_str
         else:
             if not "initial_catalog" or not "data_source":
                 raise ValueError(
@@ -54,14 +55,15 @@
             self._connection_string = f"Provider=MSOLAP;Persist Security Info=True;Initial Catalog={initial_catalog};Data Source={data_source};Timeout={timeout};UID={uid};Password={password};"
             if effective_user_name:
                 self._connection_string += f"EffectiveUserName={effective_user_name};"
             for key, value in kwargs.items():
                 self._connection_string += f"{key}={value};"
 
         self._connection = None
+        self._timeout = timeout
         self._tidy_column_names = tidy_column_names
         self._tidy_map_function = tidy_map_function
         clr.AddReference("System.Data")
 
     def _handle_oledb_field(self, f):
         """Handles different data types returned from OleDbConnection query, converting to the appropriate python type
         Attempts type sniffing by getting the Class of the type from .NET
@@ -134,14 +136,15 @@
             import System.Data.OleDb as ADONET
 
             self._connection = ADONET.OleDbConnection(self._connection_string)
             self._connection.Open()
 
         command = self._connection.CreateCommand()
         command.CommandText = daxcmd
+        command.CommandTimeout = self._timeout
         reader = command.ExecuteReader()
         schema_table = reader.GetSchemaTable()
 
         # schema_table rows are query result columns
         columns = []
         for r in schema_table.Rows:
             columns.append(r["ColumnName"])
```

### Comparing `pymsasdax-2023.1018/src/pymsasdax.egg-info/PKG-INFO` & `pymsasdax-2023.1020/src/pymsasdax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymsasdax
-Version: 2023.1018
+Version: 2023.1020
 Summary: Run DAX queries against Analysis Services and get Pandas Dataframes
 Author-email: Gage Renzi <gagerenzi+pypy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 grenzi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -119,14 +119,16 @@
     print(df)
 ```
 
 # Dev Notes
 
 ## Version History
 
+* 2023.1020
+  * fix timeout not being honored as CommandTimeout
 * 2023.1018
   * fix bug using effective_user_name or kwargs
 * ~~2023.1017~~
   * ~~fix bug using effective_user_name~~
 * 2023.1016
   * Add at least some docstrings
   * Add Premium XMLA endpoint example
@@ -141,15 +143,15 @@
 
 Yes. There aren't any. Feel free to submit a PR. 
 
 ## Building
 
 This might not be right but if you ever go to update pypi - 
 ```
-bumpver update --minor
+bumpver update --dry --set-version="2023.1020"
 pip-compile pyproject.toml
 python -m pip install -e . 
 #test
 python -m build
 twine check dist/*
 twine upload dist/*
 ```
```

