# Comparing `tmp/sqlalchemy_pytds-0.3.5-py2.py3-none-any.whl.zip` & `tmp/sqlalchemy_pytds-0.4.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7036 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      145 b- defN 23-Feb-17 22:41 sqlalchemy_pytds/__init__.py
--rw-rw-r--  2.0 unx     4306 b- defN 23-Feb-17 22:40 sqlalchemy_pytds/connector.py
+Zip file size: 7030 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      145 b- defN 23-Jun-19 10:23 sqlalchemy_pytds/__init__.py
+-rw-rw-r--  2.0 unx     4313 b- defN 23-Jun-19 10:20 sqlalchemy_pytds/connector.py
 -rw-rw-r--  2.0 unx     4412 b- defN 21-Apr-11 22:23 sqlalchemy_pytds/dialect.py
 -rw-rw-r--  2.0 unx     5530 b- defN 18-Apr-02 19:21 sqlalchemy_pytds/requirements.py
--rw-rw-r--  2.0 unx     1086 b- defN 23-Feb-17 22:42 sqlalchemy_pytds-0.3.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx      796 b- defN 23-Feb-17 22:42 sqlalchemy_pytds-0.3.5.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Feb-17 22:42 sqlalchemy_pytds-0.3.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       77 b- defN 23-Feb-17 22:42 sqlalchemy_pytds-0.3.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       17 b- defN 23-Feb-17 22:42 sqlalchemy_pytds-0.3.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      878 b- defN 23-Feb-17 22:42 sqlalchemy_pytds-0.3.5.dist-info/RECORD
-10 files, 17357 bytes uncompressed, 5516 bytes compressed:  68.2%
+-rw-rw-r--  2.0 unx     1086 b- defN 23-Jun-19 10:24 sqlalchemy_pytds-0.4.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      796 b- defN 23-Jun-19 10:24 sqlalchemy_pytds-0.4.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-19 10:24 sqlalchemy_pytds-0.4.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       77 b- defN 23-Jun-19 10:24 sqlalchemy_pytds-0.4.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       17 b- defN 23-Jun-19 10:24 sqlalchemy_pytds-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-Jun-19 10:24 sqlalchemy_pytds-0.4.0.dist-info/RECORD
+10 files, 17364 bytes uncompressed, 5510 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: sqlalchemy_pytds/dialect.py
 Comment: 
 
 Filename: sqlalchemy_pytds/requirements.py
 Comment: 
 
-Filename: sqlalchemy_pytds-0.3.5.dist-info/LICENSE
+Filename: sqlalchemy_pytds-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: sqlalchemy_pytds-0.3.5.dist-info/METADATA
+Filename: sqlalchemy_pytds-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: sqlalchemy_pytds-0.3.5.dist-info/WHEEL
+Filename: sqlalchemy_pytds-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: sqlalchemy_pytds-0.3.5.dist-info/entry_points.txt
+Filename: sqlalchemy_pytds-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sqlalchemy_pytds-0.3.5.dist-info/top_level.txt
+Filename: sqlalchemy_pytds-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlalchemy_pytds-0.3.5.dist-info/RECORD
+Filename: sqlalchemy_pytds-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlalchemy_pytds/__init__.py

```diff
@@ -1,5 +1,5 @@
-__version__ = '0.3.5'
+__version__ = '0.4.0'
 
 from sqlalchemy.dialects import registry
 
 registry.register("mssql.pytds", "sqlalchemy_pytds.dialect", "MSDialect_pytds")
```

## sqlalchemy_pytds/connector.py

```diff
@@ -61,15 +61,15 @@
     supports_unicode = True
     supports_unicode_binds = True
     supports_unicode_statements = True
     supports_native_decimal = True
     default_paramstyle = "pyformat"
 
     @classmethod
-    def dbapi(cls):
+    def import_dbapi(cls):
         return pytds
 
     def is_disconnect(self, e, connection, cursor):
         if isinstance(e, self.dbapi.ProgrammingError):
             return "The cursor's connection has been closed." in str(
                 e
             ) or "Attempt to use a closed connection." in str(e)
```

## Comparing `sqlalchemy_pytds-0.3.5.dist-info/LICENSE` & `sqlalchemy_pytds-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sqlalchemy_pytds-0.3.5.dist-info/METADATA` & `sqlalchemy_pytds-0.4.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-pytds
-Version: 0.3.5
+Version: 0.4.0
 Summary: A Microsoft SQL Server TDS connector for SQLAlchemy.
 Home-page: https://github.com/m32/sqlalchemy-tds
 Author: Grzegorz Makarewicz
 Author-email: mak@trisoft.com.pl
 License: MIT
 Keywords: SQLAlchemy Microsoft SQL Server
 Platform: any
```

