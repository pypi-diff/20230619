# Comparing `tmp/denpy-1.0.7.tar.gz` & `tmp/denpy-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denpy-1.0.7.tar", last modified: Mon Jun 12 14:50:31 2023, max compression
+gzip compressed data, was "denpy-1.0.8.tar", last modified: Mon Jun 19 21:18:38 2023, max compression
```

## Comparing `denpy-1.0.7.tar` & `denpy-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 14:50:31.832041 denpy-1.0.7/
--rw-rw-rw-   0        0        0      112 2023-06-12 14:50:31.831045 denpy-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 14:50:31.814096 denpy-1.0.7/denpy/
--rw-rw-rw-   0        0        0      137 2023-05-31 18:58:29.000000 denpy-1.0.7/denpy/__init__.py
--rw-rw-rw-   0        0        0      401 2023-06-01 15:01:37.000000 denpy-1.0.7/denpy/color.py
--rw-rw-rw-   0        0        0     1784 2023-06-12 14:47:58.000000 denpy-1.0.7/denpy/database.py
--rw-rw-rw-   0        0        0      882 2023-06-06 19:57:37.000000 denpy-1.0.7/denpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:50:31.829049 denpy-1.0.7/denpy.egg-info/
--rw-rw-rw-   0        0        0      112 2023-06-12 14:50:31.000000 denpy-1.0.7/denpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-12 14:50:31.000000 denpy-1.0.7/denpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 14:50:31.000000 denpy-1.0.7/denpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 14:50:31.000000 denpy-1.0.7/denpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 14:50:31.832041 denpy-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      205 2023-06-12 14:50:10.000000 denpy-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 21:18:38.698305 denpy-1.0.8/
+-rw-rw-rw-   0        0        0      112 2023-06-19 21:18:38.697308 denpy-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 21:18:38.693318 denpy-1.0.8/denpy/
+-rw-rw-rw-   0        0        0      137 2023-05-31 18:58:29.000000 denpy-1.0.8/denpy/__init__.py
+-rw-rw-rw-   0        0        0      401 2023-06-01 15:01:37.000000 denpy-1.0.8/denpy/color.py
+-rw-rw-rw-   0        0        0     1820 2023-06-19 20:04:44.000000 denpy-1.0.8/denpy/database.py
+-rw-rw-rw-   0        0        0     1120 2023-06-17 16:24:29.000000 denpy-1.0.8/denpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 21:18:38.696310 denpy-1.0.8/denpy.egg-info/
+-rw-rw-rw-   0        0        0      112 2023-06-19 21:18:38.000000 denpy-1.0.8/denpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-19 21:18:38.000000 denpy-1.0.8/denpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 21:18:38.000000 denpy-1.0.8/denpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 21:18:38.000000 denpy-1.0.8/denpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 21:18:38.698305 denpy-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      205 2023-06-19 21:18:19.000000 denpy-1.0.8/setup.py
```

### Comparing `denpy-1.0.7/denpy/database.py` & `denpy-1.0.8/denpy/database.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 def disconnect(database: sqlite3.Connection, cursor: sqlite3.Cursor):
     database.commit()
     cursor.close()
     database.close()
 
 def add(table: str, data: str, values: list, __file__: str):
     database, cursor = connect(__file__=__file__)
-    cursor.execute(f'INSERT INTO {table}({data}) VALUES({", ".join(values)})')
+    cursor.execute(f'INSERT INTO {table}({data}) VALUES({", ".join(["?"] * len(values))})', tuple(values))
     disconnect(database, cursor)
 
 def get(table: str, data: str, __file__: str, where: str = None) -> str or None:
     database, cursor = connect(__file__=__file__)
     if where is None:
         data = cursor.execute(f'SELECT {data} FROM {table}').fetchone()
     else:
         data = cursor.execute(f'SELECT {data} FROM {table} WHERE {where}').fetchone()
     disconnect(database, cursor)
     return data if data is None else data[0]
 
 def edit(table: str, data: str, new_data: str, __file__: str, where: str = None):
     database, cursor = connect(__file__=__file__)
     if where is None:
-        cursor.execute(f'UPDATE {table} SET {data} = {new_data}')
+        cursor.execute(f'UPDATE {table} SET {data} = ?', (new_data,))
     else:
-        cursor.execute(f'UPDATE {table} SET {data} = {new_data} WHERE {where}')
+        cursor.execute(f'UPDATE {table} SET {data} = ? WHERE {where}', (new_data,))
     disconnect(database, cursor)
 
 def remove(table: str, __file__: str, where: str = None):
     database, cursor = connect(__file__=__file__)
     if where is None:
         cursor.execute(f'DELETE FROM {table}')
     else:
```

