# Comparing `tmp/hedgesql-1.2.2.tar.gz` & `tmp/hedgesql-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hedgesql-1.2.2.tar", last modified: Mon Jun 19 16:25:23 2023, max compression
+gzip compressed data, was "hedgesql-1.2.3.tar", last modified: Mon Jun 19 16:30:02 2023, max compression
```

## Comparing `hedgesql-1.2.2.tar` & `hedgesql-1.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-19 16:25:23.347914 hedgesql-1.2.2/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 hedgesql-1.2.2/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      616 2023-06-19 16:25:23.347914 hedgesql-1.2.2/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     1927 2023-06-18 18:28:20.000000 hedgesql-1.2.2/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-19 16:25:23.347914 hedgesql-1.2.2/hedgesql/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)       96 2023-06-18 17:46:31.000000 hedgesql-1.2.2/hedgesql/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 hedgesql-1.2.2/hedgesql/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     9120 2023-06-19 16:23:30.000000 hedgesql-1.2.2/hedgesql/hedge_sql.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-19 16:25:23.347914 hedgesql-1.2.2/hedgesql.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      616 2023-06-19 16:25:23.000000 hedgesql-1.2.2/hedgesql.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      250 2023-06-19 16:25:23.000000 hedgesql-1.2.2/hedgesql.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-19 16:25:23.000000 hedgesql-1.2.2/hedgesql.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-19 16:25:23.000000 hedgesql-1.2.2/hedgesql.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        9 2023-06-19 16:25:23.000000 hedgesql-1.2.2/hedgesql.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-19 16:25:23.347914 hedgesql-1.2.2/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      761 2023-06-19 16:24:46.000000 hedgesql-1.2.2/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-19 16:30:02.884616 hedgesql-1.2.3/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 hedgesql-1.2.3/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      616 2023-06-19 16:30:02.884616 hedgesql-1.2.3/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     1927 2023-06-18 18:28:20.000000 hedgesql-1.2.3/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-19 16:30:02.880616 hedgesql-1.2.3/hedgesql/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)       96 2023-06-18 17:46:31.000000 hedgesql-1.2.3/hedgesql/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 hedgesql-1.2.3/hedgesql/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8921 2023-06-19 16:29:13.000000 hedgesql-1.2.3/hedgesql/hedge_sql.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-19 16:30:02.884616 hedgesql-1.2.3/hedgesql.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      616 2023-06-19 16:30:02.000000 hedgesql-1.2.3/hedgesql.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      250 2023-06-19 16:30:02.000000 hedgesql-1.2.3/hedgesql.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-19 16:30:02.000000 hedgesql-1.2.3/hedgesql.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-19 16:30:02.000000 hedgesql-1.2.3/hedgesql.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        9 2023-06-19 16:30:02.000000 hedgesql-1.2.3/hedgesql.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-19 16:30:02.884616 hedgesql-1.2.3/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      761 2023-06-19 16:29:13.000000 hedgesql-1.2.3/setup.py
```

### Comparing `hedgesql-1.2.2/LICENSE` & `hedgesql-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hedgesql-1.2.2/PKG-INFO` & `hedgesql-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedgesql
-Version: 1.2.2
+Version: 1.2.3
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/I-HedgeDev/litesqlite
 Author: HedgeDev
 Author-email: hedge_dev@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `hedgesql-1.2.2/README.md` & `hedgesql-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hedgesql-1.2.2/hedgesql/datatypes.py` & `hedgesql-1.2.3/hedgesql/datatypes.py`

 * *Files identical despite different names*

### Comparing `hedgesql-1.2.2/hedgesql/hedge_sql.py` & `hedgesql-1.2.3/hedgesql/hedge_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,16 @@
     def __init__(self,
                  db_name: str) -> None:
         self.__db_name = db_name
         self.__conn = None
         self.__cursor = None
 
     def open_conn(self) -> None:
-        if self.__conn is None:
-            self.__conn = sqlite3.connect(self.__db_name)
-            self.__cursor = self.__conn.cursor()
+        self.__conn = sqlite3.connect(self.__db_name)
+        self.__cursor = self.__conn.cursor()
 
     def __enter__(self) -> 'Sqlite':
         self.open_conn()
         return self
 
     def create_table(self,
                      table_name: str,
@@ -104,35 +103,31 @@
             where_clause = ''
             values = ()
         query = f"DELETE FROM {table_name} {where_clause}"
         self.__cursor.execute(query, values)
         self.__conn.commit()
 
     def close_conn(self) -> None:
-        try:
-            self.__conn.close()
-        except ValueError:
-            pass
+        self.__conn.close()
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         self.open_conn()
 
 
 class AioSqlite:
 
     def __init__(self,
                  db_name: str) -> None:
         self.__db_name = db_name
         self.__conn = None
         self.__cursor = None
 
     async def open_conn(self) -> None:
-        if self.__conn is None:
-            self.__conn = await aiosqlite.connect(self.__db_name)
-            self.__cursor = await self.__conn.cursor()
+        self.__conn = await aiosqlite.connect(self.__db_name)
+        self.__cursor = await self.__conn.cursor()
 
     async def __aenter__(self) -> 'AioSqlite':
         await self.open_conn()
         return self
 
     async def create_table(self,
                            table_name: str,
@@ -217,14 +212,11 @@
             where_clause = ''
             values = ()
         query = f"DELETE FROM {table_name} {where_clause}"
         await self.__cursor.execute(query, values)
         await self.__conn.commit()
 
     async def close_conn(self) -> None:
-       try:
-           await self.__conn.close()
-       except ValueError:
-           pass
+       await self.__conn.close()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.close_conn()
```

### Comparing `hedgesql-1.2.2/hedgesql.egg-info/PKG-INFO` & `hedgesql-1.2.3/hedgesql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedgesql
-Version: 1.2.2
+Version: 1.2.3
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/I-HedgeDev/litesqlite
 Author: HedgeDev
 Author-email: hedge_dev@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `hedgesql-1.2.2/setup.py` & `hedgesql-1.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='hedgesql',
-    version='1.2.2',
+    version='1.2.3',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/I-HedgeDev/litesqlite',
     author='HedgeDev',
     author_email='hedge_dev@mail.ru',
     packages=['hedgesql'],
     install_requires=[
         'aiosqlite'
```

