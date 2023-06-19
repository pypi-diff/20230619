# Comparing `tmp/mysqlx-1.2.5.tar.gz` & `tmp/mysqlx-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.2.5.tar", last modified: Mon Jun 19 14:00:47 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.2.8.tar", last modified: Mon Jun 19 14:14:29 2023, max compression
```

## Comparing `mysqlx-1.2.5.tar` & `mysqlx-1.2.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 14:00:47.000000 mysqlx-1.2.5/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.2.5/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-19 14:00:47.000000 mysqlx-1.2.5/mysqlx/
--rw-rw-rw-   0        0        0     5827 2023-06-19 12:47:48.000000 mysqlx-1.2.5/mysqlx/coder.py
--rw-rw-rw-   0        0        0     1589 2023-06-09 01:09:35.000000 mysqlx-1.2.5/mysqlx/coder.tpl
--rw-rw-rw-   0        0        0    17467 2023-06-18 07:05:30.000000 mysqlx-1.2.5/mysqlx/db.py
--rw-rw-rw-   0        0        0     9832 2023-06-18 07:05:30.000000 mysqlx-1.2.5/mysqlx/dbx.py
--rw-rw-rw-   0        0        0    30506 2023-06-19 05:19:22.000000 mysqlx-1.2.5/mysqlx/orm.py
--rw-rw-rw-   0        0        0     6107 2023-06-18 03:07:16.000000 mysqlx-1.2.5/mysqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.2.5/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:00:47.000000 mysqlx-1.2.5/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-19 14:00:47.000000 mysqlx-1.2.5/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-06 08:06:39.000000 mysqlx-1.2.5/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3725 2023-06-19 14:00:47.000000 mysqlx-1.2.5/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-06-19 14:00:47.000000 mysqlx-1.2.5/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      476 2023-06-19 14:00:47.000000 mysqlx-1.2.5/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2023-06-19 14:00:47.000000 mysqlx-1.2.5/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3725 2023-06-19 14:00:47.000000 mysqlx-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3295 2023-06-12 03:58:38.000000 mysqlx-1.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 14:00:47.000000 mysqlx-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      856 2023-06-19 13:58:23.000000 mysqlx-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:00:47.000000 mysqlx-1.2.5/test/
--rw-rw-rw-   0        0        0      216 2023-06-10 13:13:30.000000 mysqlx-1.2.5/test/all_unit_test.py
--rw-rw-rw-   0        0        0      312 2023-06-19 03:27:12.000000 mysqlx-1.2.5/test/coder_test.py
--rw-rw-rw-   0        0        0     2966 2023-06-13 02:46:47.000000 mysqlx-1.2.5/test/dbx_test.py
--rw-rw-rw-   0        0        0     5025 2023-06-13 09:20:17.000000 mysqlx-1.2.5/test/db_test.py
--rw-rw-rw-   0        0        0     5090 2023-06-19 12:47:52.000000 mysqlx-1.2.5/test/models.py
--rw-rw-rw-   0        0        0     6869 2023-06-19 05:16:27.000000 mysqlx-1.2.5/test/orm_test.py
--rw-rw-rw-   0        0        0      710 2023-06-11 02:56:34.000000 mysqlx-1.2.5/test/unit_test.py
--rw-rw-rw-   0        0        0      320 2023-06-13 02:39:09.000000 mysqlx-1.2.5/test/user_mapper.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.2.5/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 14:14:29.000000 mysqlx-1.2.8/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.2.8/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-19 14:14:29.000000 mysqlx-1.2.8/mysqlx/
+-rw-rw-rw-   0        0        0     5827 2023-06-19 12:47:48.000000 mysqlx-1.2.8/mysqlx/coder.py
+-rw-rw-rw-   0        0        0     1589 2023-06-09 01:09:35.000000 mysqlx-1.2.8/mysqlx/coder.tpl
+-rw-rw-rw-   0        0        0    17467 2023-06-18 07:05:30.000000 mysqlx-1.2.8/mysqlx/db.py
+-rw-rw-rw-   0        0        0     9832 2023-06-18 07:05:30.000000 mysqlx-1.2.8/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0    30506 2023-06-19 05:19:22.000000 mysqlx-1.2.8/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     6107 2023-06-18 03:07:16.000000 mysqlx-1.2.8/mysqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.2.8/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 14:14:29.000000 mysqlx-1.2.8/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-19 14:14:29.000000 mysqlx-1.2.8/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 14:08:07.000000 mysqlx-1.2.8/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      406 2023-06-19 14:14:29.000000 mysqlx-1.2.8/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-06-19 14:14:29.000000 mysqlx-1.2.8/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      476 2023-06-19 14:14:29.000000 mysqlx-1.2.8/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-06-19 14:14:29.000000 mysqlx-1.2.8/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      406 2023-06-19 14:14:29.000000 mysqlx-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3295 2023-06-12 03:58:38.000000 mysqlx-1.2.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 14:14:29.000000 mysqlx-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      851 2023-06-19 14:14:23.000000 mysqlx-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 14:14:29.000000 mysqlx-1.2.8/test/
+-rw-rw-rw-   0        0        0      216 2023-06-10 13:13:30.000000 mysqlx-1.2.8/test/all_unit_test.py
+-rw-rw-rw-   0        0        0      312 2023-06-19 03:27:12.000000 mysqlx-1.2.8/test/coder_test.py
+-rw-rw-rw-   0        0        0     2966 2023-06-13 02:46:47.000000 mysqlx-1.2.8/test/dbx_test.py
+-rw-rw-rw-   0        0        0     5025 2023-06-13 09:20:17.000000 mysqlx-1.2.8/test/db_test.py
+-rw-rw-rw-   0        0        0     5090 2023-06-19 12:47:52.000000 mysqlx-1.2.8/test/models.py
+-rw-rw-rw-   0        0        0     6869 2023-06-19 05:16:27.000000 mysqlx-1.2.8/test/orm_test.py
+-rw-rw-rw-   0        0        0      710 2023-06-11 02:56:34.000000 mysqlx-1.2.8/test/unit_test.py
+-rw-rw-rw-   0        0        0      320 2023-06-13 02:39:09.000000 mysqlx-1.2.8/test/user_mapper.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.2.8/test/__init__.py
```

### Comparing `mysqlx-1.2.5/LICENSE` & `mysqlx-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.5/mysqlx/coder.py` & `mysqlx-1.2.8/mysqlx/coder.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.5/mysqlx/coder.tpl` & `mysqlx-1.2.8/mysqlx/coder.tpl`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.5/mysqlx/db.py` & `mysqlx-1.2.8/mysqlx/db.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.5/mysqlx/dbx.py` & `mysqlx-1.2.8/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.5/mysqlx/orm.py` & `mysqlx-1.2.8/mysqlx/orm.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.5/mysqlx/support.py` & `mysqlx-1.2.8/mysqlx/support.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.5/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.2.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,8 @@
-Metadata-Version: 2.1
-Name: mysqlx
-Version: 1.2.5
-Summary: MySqlx is a simple python sql executor for MySQL like iBatis.
-Home-page: https://gitee.com/summry/mysqlx
-Author: summry
-Author-email: xiazhongbiao@126.com
-License: UNKNOWN
-Keywords: sql,MySQL,iBatis,MyBatis,python
-Platform: UNKNOWN
-Requires-Python: >=3.6.0
-Description-Content-Type: ##### Install
+##### Install
 ```
 pip install mysqlx
 ```
 ##### Sample
 ```
 from mysqlx import db
 
@@ -28,34 +17,34 @@
     'mapper_path': 'mapper'
 }
 
 if __name__ == '__main__':
     db.init_db(**db_conf)
     
     # Return effect rowcount
-    rowcount = db.insert('user', name='寮犱笁', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+    rowcount = db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
     assert rowcount == 1, 'insert'
     assert db.get('select count(1) from user') == 1, 'insert'
 
-    id2 = db.save('user', name='鏉庡洓', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+    id2 = db.save('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
     assert id2 > 0, 'save'
     assert db.get('select count(1) from user') == 2, 'save'
 
-    db.execute('update user set name=? where id=?', '鐜嬩簲', id2)
-    assert db.get('select name from user where id=?', id2) == '鐜嬩簲', 'execute'
+    db.execute('update user set name=? where id=?', '王五', id2)
+    assert db.get('select name from user where id=?', id2) == '王五', 'execute'
 
-    db.execute('update user set name=:name where id=:id', name='璧靛叚', id=id2)
+    db.execute('update user set name=:name where id=:id', name='赵六', id=id2)
     assert db.select_one('select id, name from user where id=:id', id=id2)[0] == id2, 'execute'
 
-    db.execute('update user set name=:name where id=:id', name='璧靛叚', id=id2)
-    assert db.query_one('select name from user where id=:id', id=id2)['name'] == '璧靛叚', 'execute'
+    db.execute('update user set name=:name where id=:id', name='赵六', id=id2)
+    assert db.query_one('select name from user where id=:id', id=id2)['name'] == '赵六', 'execute'
 
     args = [
-        ('寮犱笁', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56),
-        ('寮犱笁', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56)
+        ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56),
+        ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56)
     ]
     db.batch_execute('insert into user(name, age, birth_date, sex, grade, point, money) values(?,?,?,?,?,?,?)', args)
     users = db.select('select id, del_flag from user')
     assert len(users) == 4, 'batch_execute'
     users = db.query('select id, del_flag from user')
     assert len(users) == 4, 'batch_execute'
 
@@ -72,30 +61,26 @@
     db.execute('delete from user where id=? limit 1', id2)
     assert db.get('select count(1) from user') == 3, 'execute delete'
 ```
 ##### Transaction
 ```
 @db.with_transaction
 def test_transaction():
-    db.insert('user', name='寮犱笁', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-    db.insert('user', name='鏉庡洓', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+    db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+    db.insert('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
 
 
 def test_transaction2():
     with db.transaction():
-        db.insert('user', name='寮犱笁', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-        db.insert('user', name='鏉庡洓', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+        db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+        db.insert('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
 ```
 ##### Note
 ```
 get: Return only one object, like count
 query_one: Return one row with dict
 select_one: Return one row with tuple
 find_by_id: Return one row with class instance object
 query: Return list of dict
 select: Return list of tuple
 find: Return list of class instance object
-```
-License-File: LICENSE
-
-UNKNOWN
-
+```
```

### Comparing `mysqlx-1.2.5/test/dbx_test.py` & `mysqlx-1.2.8/test/dbx_test.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.5/test/db_test.py` & `mysqlx-1.2.8/test/db_test.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.5/test/models.py` & `mysqlx-1.2.8/test/models.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.5/test/orm_test.py` & `mysqlx-1.2.8/test/orm_test.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.5/test/unit_test.py` & `mysqlx-1.2.8/test/unit_test.py`

 * *Files identical despite different names*

