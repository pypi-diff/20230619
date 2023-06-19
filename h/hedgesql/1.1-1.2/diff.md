# Comparing `tmp/hedgesql-1.1.tar.gz` & `tmp/hedgesql-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hedgesql-1.1.tar", last modified: Sun Jun 18 18:39:40 2023, max compression
+gzip compressed data, was "hedgesql-1.2.tar", last modified: Mon Jun 19 16:00:04 2023, max compression
```

## Comparing `hedgesql-1.1.tar` & `hedgesql-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-18 18:39:40.531112 hedgesql-1.1/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 hedgesql-1.1/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      614 2023-06-18 18:39:40.531112 hedgesql-1.1/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     1927 2023-06-18 18:28:20.000000 hedgesql-1.1/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-18 18:39:40.527111 hedgesql-1.1/hedgesql/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)       96 2023-06-18 17:46:31.000000 hedgesql-1.1/hedgesql/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 hedgesql-1.1/hedgesql/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     9001 2023-06-18 18:25:44.000000 hedgesql-1.1/hedgesql/hedge_sql.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-18 18:39:40.531112 hedgesql-1.1/hedgesql.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      614 2023-06-18 18:39:40.000000 hedgesql-1.1/hedgesql.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      250 2023-06-18 18:39:40.000000 hedgesql-1.1/hedgesql.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-18 18:39:40.000000 hedgesql-1.1/hedgesql.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-18 18:39:40.000000 hedgesql-1.1/hedgesql.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        9 2023-06-18 18:39:40.000000 hedgesql-1.1/hedgesql.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-18 18:39:40.531112 hedgesql-1.1/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      759 2023-06-18 18:39:24.000000 hedgesql-1.1/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-19 16:00:04.104960 hedgesql-1.2/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 hedgesql-1.2/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      614 2023-06-19 16:00:04.104960 hedgesql-1.2/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     1927 2023-06-18 18:28:20.000000 hedgesql-1.2/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-19 16:00:04.100960 hedgesql-1.2/hedgesql/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)       96 2023-06-18 17:46:31.000000 hedgesql-1.2/hedgesql/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 hedgesql-1.2/hedgesql/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     9081 2023-06-18 22:29:42.000000 hedgesql-1.2/hedgesql/hedge_sql.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-19 16:00:04.100960 hedgesql-1.2/hedgesql.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      614 2023-06-19 16:00:03.000000 hedgesql-1.2/hedgesql.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      250 2023-06-19 16:00:03.000000 hedgesql-1.2/hedgesql.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-19 16:00:03.000000 hedgesql-1.2/hedgesql.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-19 16:00:03.000000 hedgesql-1.2/hedgesql.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        9 2023-06-19 16:00:03.000000 hedgesql-1.2/hedgesql.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-19 16:00:04.104960 hedgesql-1.2/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      759 2023-06-19 16:00:01.000000 hedgesql-1.2/setup.py
```

### Comparing `hedgesql-1.1/LICENSE` & `hedgesql-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hedgesql-1.1/PKG-INFO` & `hedgesql-1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedgesql
-Version: 1.1
+Version: 1.2
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/I-HedgeDev/litesqlite
 Author: HedgeDev
 Author-email: hedge_dev@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `hedgesql-1.1/README.md` & `hedgesql-1.2/README.md`

 * *Files identical despite different names*

### Comparing `hedgesql-1.1/hedgesql/datatypes.py` & `hedgesql-1.2/hedgesql/datatypes.py`

 * *Files identical despite different names*

### Comparing `hedgesql-1.1/hedgesql/hedge_sql.py` & `hedgesql-1.2/hedgesql/hedge_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,16 @@
             where_clause = ''
             values = ()
         query = f"DELETE FROM {table_name} {where_clause}"
         self.__cursor.execute(query, values)
         self.__conn.commit()
 
     def close_conn(self) -> None:
-        self.__conn.close()
+        if self.__conn is not None:
+            self.__conn.close()
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         self.open_conn()
 
 
 class AioSqlite:
 
@@ -214,11 +215,12 @@
             where_clause = ''
             values = ()
         query = f"DELETE FROM {table_name} {where_clause}"
         await self.__cursor.execute(query, values)
         await self.__conn.commit()
 
     async def close_conn(self) -> None:
-        await self.__conn.close()
+        if self.__conn is not None:
+            await self.__conn.close()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.close_conn()
```

### Comparing `hedgesql-1.1/hedgesql.egg-info/PKG-INFO` & `hedgesql-1.2/hedgesql.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedgesql
-Version: 1.1
+Version: 1.2
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/I-HedgeDev/litesqlite
 Author: HedgeDev
 Author-email: hedge_dev@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `hedgesql-1.1/setup.py` & `hedgesql-1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='hedgesql',
-    version='1.1',
+    version='1.2',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/I-HedgeDev/litesqlite',
     author='HedgeDev',
     author_email='hedge_dev@mail.ru',
     packages=['hedgesql'],
     install_requires=[
         'aiosqlite'
```

