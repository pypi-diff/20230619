# Comparing `tmp/mysqlx-1.2.4.tar.gz` & `tmp/mysqlx-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.2.4.tar", last modified: Fri Jun  9 07:20:24 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.2.5.tar", last modified: Mon Jun 19 14:00:47 2023, max compression
```

## Comparing `mysqlx-1.2.4.tar` & `mysqlx-1.2.5.tar`

### file list

```diff
@@ -1,21 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 07:20:24.000000 mysqlx-1.2.4/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.2.4/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-09 07:20:24.000000 mysqlx-1.2.4/mysqlx/
--rw-rw-rw-   0        0        0     5989 2023-06-09 01:21:35.000000 mysqlx-1.2.4/mysqlx/coder.py
--rw-rw-rw-   0        0        0     1589 2023-06-09 01:09:35.000000 mysqlx-1.2.4/mysqlx/coder.tpl
--rw-rw-rw-   0        0        0    10185 2023-06-07 12:34:06.000000 mysqlx-1.2.4/mysqlx/db.py
--rw-rw-rw-   0        0        0     3370 2023-06-06 00:29:56.000000 mysqlx-1.2.4/mysqlx/dbx.py
--rw-rw-rw-   0        0        0     5295 2023-06-06 23:27:22.000000 mysqlx-1.2.4/mysqlx/helper.py
--rw-rw-rw-   0        0        0    10862 2023-06-09 07:16:35.000000 mysqlx-1.2.4/mysqlx/orm.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.2.4/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 07:20:24.000000 mysqlx-1.2.4/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-09 07:20:24.000000 mysqlx-1.2.4/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-06 08:06:39.000000 mysqlx-1.2.4/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      404 2023-06-09 07:20:24.000000 mysqlx-1.2.4/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-06-09 07:20:24.000000 mysqlx-1.2.4/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      314 2023-06-09 07:20:24.000000 mysqlx-1.2.4/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-06-09 07:20:24.000000 mysqlx-1.2.4/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      404 2023-06-09 07:20:24.000000 mysqlx-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2598 2023-06-06 12:09:45.000000 mysqlx-1.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 07:20:24.000000 mysqlx-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      816 2023-06-09 07:20:09.000000 mysqlx-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 14:00:47.000000 mysqlx-1.2.5/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.2.5/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-19 14:00:47.000000 mysqlx-1.2.5/mysqlx/
+-rw-rw-rw-   0        0        0     5827 2023-06-19 12:47:48.000000 mysqlx-1.2.5/mysqlx/coder.py
+-rw-rw-rw-   0        0        0     1589 2023-06-09 01:09:35.000000 mysqlx-1.2.5/mysqlx/coder.tpl
+-rw-rw-rw-   0        0        0    17467 2023-06-18 07:05:30.000000 mysqlx-1.2.5/mysqlx/db.py
+-rw-rw-rw-   0        0        0     9832 2023-06-18 07:05:30.000000 mysqlx-1.2.5/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0    30506 2023-06-19 05:19:22.000000 mysqlx-1.2.5/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     6107 2023-06-18 03:07:16.000000 mysqlx-1.2.5/mysqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.2.5/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 14:00:47.000000 mysqlx-1.2.5/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-19 14:00:47.000000 mysqlx-1.2.5/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-06 08:06:39.000000 mysqlx-1.2.5/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3725 2023-06-19 14:00:47.000000 mysqlx-1.2.5/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-06-19 14:00:47.000000 mysqlx-1.2.5/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      476 2023-06-19 14:00:47.000000 mysqlx-1.2.5/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-06-19 14:00:47.000000 mysqlx-1.2.5/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3725 2023-06-19 14:00:47.000000 mysqlx-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3295 2023-06-12 03:58:38.000000 mysqlx-1.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 14:00:47.000000 mysqlx-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      856 2023-06-19 13:58:23.000000 mysqlx-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 14:00:47.000000 mysqlx-1.2.5/test/
+-rw-rw-rw-   0        0        0      216 2023-06-10 13:13:30.000000 mysqlx-1.2.5/test/all_unit_test.py
+-rw-rw-rw-   0        0        0      312 2023-06-19 03:27:12.000000 mysqlx-1.2.5/test/coder_test.py
+-rw-rw-rw-   0        0        0     2966 2023-06-13 02:46:47.000000 mysqlx-1.2.5/test/dbx_test.py
+-rw-rw-rw-   0        0        0     5025 2023-06-13 09:20:17.000000 mysqlx-1.2.5/test/db_test.py
+-rw-rw-rw-   0        0        0     5090 2023-06-19 12:47:52.000000 mysqlx-1.2.5/test/models.py
+-rw-rw-rw-   0        0        0     6869 2023-06-19 05:16:27.000000 mysqlx-1.2.5/test/orm_test.py
+-rw-rw-rw-   0        0        0      710 2023-06-11 02:56:34.000000 mysqlx-1.2.5/test/unit_test.py
+-rw-rw-rw-   0        0        0      320 2023-06-13 02:39:09.000000 mysqlx-1.2.5/test/user_mapper.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.2.5/test/__init__.py
```

### Comparing `mysqlx-1.2.4/LICENSE` & `mysqlx-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.4/mysqlx/coder.py` & `mysqlx-1.2.5/mysqlx/coder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 import os
 from . import db
 from jinja2 import FileSystemLoader, Environment
 from typing import Union, Iterable
 
+COMMON_COLS = ['create_by', 'create_time']
+ATTRIBUTES = {'__pk__': 'id', '__update_by__': 'update_by', '__update_time__': 'update_time', '__del_flag__': 'del_flag'}
+
 
 class Coder:
     comma1 = ','
     comma2 = '，'
     sql = '''
     SELECT column_name, data_type, character_maximum_length, NUMERIC_precision, NUMERIC_scale, column_key FROM information_schema.columns
      WHERE table_schema = (SELECT DATABASE())
        AND table_name = ? 
     '''
 
-    def __init__(self, user: str, password: str, database: str, host='127.0.0.1', port=3306, use_unicode=True, pool_size=1, show_sql=True, **kwargs):
+    def __init__(self, user='root', password='', database='test', host='127.0.0.1', port=3306, use_unicode=True, pool_size=1, show_sql=False,
+            **kwargs):
         db.init_db(user, password, database, host, port, pool_size, use_unicode, show_sql, **kwargs)
 
-    def generate_with_schema(self, schema: str = None, path: str = None, common_cols=['create_by', 'create_time'],
-                             attributes={'__pk__': 'id', '__update_by__': 'update_by', '__update_time__': 'update_time', '__del_flag__': 'del_flag'}):
+    def generate_with_schema(self, schema: str = None, path: str = None, *args, **kwargs):
         if schema:
             db.execute('use %s' % schema)
         tables = db.select('show tables')
-        tables = [table['Tables_in_investment'] for table in tables]
-        self.generate_with_tables(tables=tables, path=path, common_cols=common_cols, attributes=attributes)
+        tables = [table[0] for table in tables]
+        self.generate_with_tables(tables=tables, path=path, *args, **kwargs)
 
-    def generate_with_tables(self, tables: Union[str, Iterable[str]], path: str = None, common_cols=['create_by', 'create_time'],
-                             attributes={'__pk__': 'id', '__update_by__': 'update_by', '__update_time__': 'update_time', '__del_flag__': 'del_flag'}):
+    def generate_with_tables(self, tables: Union[str, Iterable[str]], path: str = None, *args, **kwargs):
         metas = None
         only_one_table = False
-
-        columns = [v for v in attributes.values()]
-        if common_cols:
-            common_cols.reverse()
-            for i in range(0, len(common_cols)):
-                columns.insert(1, common_cols[i])
+        if not args:
+            args = COMMON_COLS
+        if not kwargs:
+            kwargs = ATTRIBUTES
+
+        columns = [v for v in kwargs.values()]
+        if args:
+            args.reverse()
+            for i in range(0, len(args)):
+                columns.insert(1, args[i])
 
             # 去重
             base_columns = list(set(columns))
             # 保持原有顺序
             base_columns.sort(key=columns.index)
         else:
             base_columns = columns
@@ -64,52 +70,53 @@
         if len(metas) > 0:
             cols = [col for mata in metas for col in mata['super_columns']]
             col_dict = {col['COLUMN_NAME']: col for col in cols}
 
             def get_type(col):
                 if col in col_dict:
                     return col_dict[col]['DATA_TYPE']
-                elif col == attributes.get('__pk__') or col == attributes.get('__update_by__') or col == attributes.get('__del_flag__'):
+                elif col == kwargs.get('__pk__') or col == kwargs.get('__update_by__') or col == kwargs.get('__del_flag__'):
                     return 'int'
-                elif col == attributes.get('__update_time__'):
+                elif col == kwargs.get('__update_time__'):
                     return 'datetime'
                 elif col.endswith("_time"):
                     return 'datetime'
                 elif col.endswith("_date"):
                     return 'date'
                 else:
                     return 'None'
 
-            attributes['metas'] = metas
-            attributes['base_columns'] = [{'COLUMN_NAME': col, 'DATA_TYPE': get_type(col)} for col in base_columns]
-            self._generate(attributes, path)
+            kwargs['metas'] = metas
+            kwargs['base_columns'] = [{'COLUMN_NAME': col, 'DATA_TYPE': get_type(col)} for col in base_columns]
+            self._generate(kwargs, path)
 
     def _get_table_meta(self, table: str, base_columns):
+        def convert_type(col_type):
+            if col_type in ('int', 'tinyint', 'bigint'):
+                return 'int'
+            elif col_type in ('float', 'double'):
+                return 'float'
+            elif col_type == 'decimal':
+                return 'Decimal'
+            elif col_type in ('char', 'varchar', 'text'):
+                return 'str'
+            elif col_type in ('date', 'datetime'):
+                return col_type
+            else:
+                return 'None'
+
         pk = None
         super_columns = []
-        columns = db.do_select(self.sql, table)
+        columns = db.do_query(self.sql, table)
         for col in columns:
             if col['COLUMN_KEY'] == 'PRI':
                 pk = col['COLUMN_NAME']
-
             if col['COLUMN_NAME'] in base_columns:
                 super_columns.append(col)
-
-            if col['DATA_TYPE'] in ('int', 'tinyint', 'bigint'):
-                col['DATA_TYPE'] = 'int'
-            elif col['DATA_TYPE'] in ('float', 'double'):
-                col['DATA_TYPE'] = 'float'
-            elif col['DATA_TYPE'] == 'decimal':
-                col['DATA_TYPE'] = 'Decimal'
-            elif col['DATA_TYPE'] in ('char', 'varchar', 'text'):
-                col['DATA_TYPE'] = 'str'
-            elif col['DATA_TYPE'] in ('date', 'datetime'):
-                pass
-            else:
-                col['DATA_TYPE'] = 'None'
+            col['DATA_TYPE'] = convert_type(col['DATA_TYPE'])
 
         if pk is None:
             return table
 
         class_name = self._get_class_name(table)
         return {
             'pk': pk,
@@ -139,8 +146,7 @@
     def _get_class_name(table):
         if '_' not in table:
             return table.capitalize()
 
         names = table.split('_')
         names = [name.capitalize() for name in names]
         return ''.join(names)
-
```

### Comparing `mysqlx-1.2.4/mysqlx/coder.tpl` & `mysqlx-1.2.5/mysqlx/coder.tpl`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.4/mysqlx/helper.py` & `mysqlx-1.2.5/mysqlx/support.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 import logging
 import threading
 from jinja2 import Template
 
+LIMIT_1 = 1
 _REGEX = r':[\w|\d]*'
 DYNAMIC_REGEX = '{%|{{|}}|%}'
 
 
 def try_commit(db_ctx):
     if db_ctx.transactions == 0:
         logging.debug('Commit transaction...')
@@ -17,29 +18,50 @@
             logging.warning('Commit failed, try rollback...')
             db_ctx.connection.rollback()
             logging.warning('Rollback ok.')
             raise
 
 
 def simple_sql(sql, *args, **kwargs):
-    return _get_named_sql_args(sql, **kwargs) if kwargs else (sql, args)
+    return get_named_sql_args(sql, **kwargs) if kwargs else (sql, args)
+
+
+def is_dynamic_sql(sql: str):
+    return re.search(DYNAMIC_REGEX, sql)
 
 
 def dynamic_sql(sql, *args, **kwargs):
     if kwargs:
-        if re.search(DYNAMIC_REGEX, sql):
+        if is_dynamic_sql(sql):
             sql = Template(sql).render(**kwargs)
-        return _get_named_sql_args(sql, **kwargs)
+        return get_named_sql_args(sql, **kwargs)
 
     return sql, args
 
 
-def _get_named_sql_args(sql: str, **kwargs):
-    args = [kwargs[r[1:]] for r in re.findall(_REGEX, sql)]
-    return re.sub(_REGEX, '?', sql), args
+def log(function: str, sql: str, *args, **kwargs):
+    logging.debug("Exec func 'mysqlx.%s' \n\t\tsql: %s \n\t\targs: %s \n\t\tkwargs: %s" % (function, sql.strip(), args, kwargs))
+
+
+def page_log(function: str, sql: str, page_num, page_size, *args, **kwargs):
+    logging.debug("Exec func 'mysqlx.%s', page_num: %d, page_size: %d \n\t\tsql: %s \n\t\targs: %s \n\t\tkwargs: %s" % (
+        function, page_num, page_size, sql.strip(), args, kwargs))
+
+
+def get_named_sql_args(sql: str, **kwargs):
+    args = get_named_args(sql, **kwargs)
+    return get_named_sql(sql), args
+
+
+def get_named_sql(sql: str):
+    return re.sub(_REGEX, '?', sql)
+
+
+def get_named_args(sql: str, **kwargs):
+    return [kwargs[r[1:]] for r in re.findall(_REGEX, sql)]
 
 
 class DBCtx(threading.local):
     """
     Thread local object that holds connection info.
     """
 
@@ -63,15 +85,15 @@
             self.connection.close()
             self.connection = None
 
     def cursor(self):
         """
         Return cursor
         """
-        logging.debug('Cursor prepared: %s' % self.prepared)
+        # logging.debug('Cursor prepared: %s' % self.prepared)
         return self.connection.cursor(prepared=self.prepared)
 
     def statement(self, sql):
         """
         Return statement
         """
         return self.connection.statement(sql)
@@ -143,14 +165,18 @@
         logging.debug('Rollback ok.')
 
 
 class DBError(Exception):
     pass
 
 
+class MapperError(DBError):
+    pass
+
+
 class MultiColumnsError(DBError):
     pass
 
 
 class Dict(dict):
     """
     Simple dict but support access as x.y style.
@@ -193,12 +219,13 @@
             raise AttributeError(r"'Dict' object has no attribute '%s'" % key)
 
     def __setattr__(self, key, value):
         self[key] = value
 
 
 class SqlModel:
-    def __init__(self, sql: str, dynamic: bool = False, include: str = None):
+    from typing import List
+    def __init__(self, sql: str, namespace: str, dynamic=False, includes: List[str] = None):
         self.sql = sql
+        self.namespace = namespace
         self.dynamic = dynamic
-        self.include = include
-
+        self.includes = includes
```

### Comparing `mysqlx-1.2.4/README.md` & `mysqlx-1.2.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -10,51 +10,57 @@
     'host': HOST,
     'port': 3306, 
     'user': 'root', 
     'password': 'xxx', 
     'database': 'test',
     'pool_size': 5,
     'show_sql': True,
-    # 'mapper_path': 'mapper'
+    'mapper_path': 'mapper'
 }
 
 if __name__ == '__main__':
     db.init_db(**db_conf)
     
     # Return effect rowcount
     rowcount = db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
     assert rowcount == 1, 'insert'
     assert db.get('select count(1) from user') == 1, 'insert'
 
-    # Return primery key when use auto_increment
     id2 = db.save('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
     assert id2 > 0, 'save'
-    # Return one value.
     assert db.get('select count(1) from user') == 2, 'save'
 
     db.execute('update user set name=? where id=?', '王五', id2)
     assert db.get('select name from user where id=?', id2) == '王五', 'execute'
 
     db.execute('update user set name=:name where id=:id', name='赵六', id=id2)
-    # Return one row.
-    assert db.select_one('select name from user where id=:id', id=id2)['name'] == '赵六', 'execute'
+    assert db.select_one('select id, name from user where id=:id', id=id2)[0] == id2, 'execute'
+
+    db.execute('update user set name=:name where id=:id', name='赵六', id=id2)
+    assert db.query_one('select name from user where id=:id', id=id2)['name'] == '赵六', 'execute'
 
     args = [
         ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56),
         ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56)
     ]
     db.batch_execute('insert into user(name, age, birth_date, sex, grade, point, money) values(?,?,?,?,?,?,?)', args)
     users = db.select('select id, del_flag from user')
     assert len(users) == 4, 'batch_execute'
+    users = db.query('select id, del_flag from user')
+    assert len(users) == 4, 'batch_execute'
 
     users = db.select('select id, del_flag from user where id=?', id2)
     assert len(users) == 1, 'select'
+    users = db.query('select id, del_flag from user where id=?', id2)
+    assert len(users) == 1, 'select'
 
     users = db.select('select id, del_flag from user where id=:id', id=id2)
     assert len(users) == 1, 'select'
+    users = db.query('select id, del_flag from user where id=:id', id=id2)
+    assert len(users) == 1, 'select'
 
     db.execute('delete from user where id=? limit 1', id2)
     assert db.get('select count(1) from user') == 3, 'execute delete'
 ```
 ##### Transaction
 ```
 @db.with_transaction
@@ -64,7 +70,17 @@
 
 
 def test_transaction2():
     with db.transaction():
         db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
         db.insert('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
 ```
+##### Note
+```
+get: Return only one object, like count
+query_one: Return one row with dict
+select_one: Return one row with tuple
+find_by_id: Return one row with class instance object
+query: Return list of dict
+select: Return list of tuple
+find: Return list of class instance object
+```
```

### Comparing `mysqlx-1.2.4/setup.py` & `mysqlx-1.2.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from setuptools import setup, find_packages
 
 # INSTALL_PACKAGES = open(path.join(DIR, 'requirements.txt')).read().splitlines()
+with open('README.md', 'r') as f:
+    readme = f.read()
 
 setup(
     name='mysqlx',
     packages=find_packages(),
-    description="mysqlx is a simple python sql executor for MySQL like iBatis.",
-    long_description_content_type='text/markdown',
+    description="MySqlx is a simple python sql executor for MySQL like iBatis.",
+    long_description_content_type=readme,
     install_requires=[
         'Jinja2>=3.0.3',
         'mysql-connector-python>=8.0.20',
     ],
-    version='1.2.4',
+    version='1.2.5',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'iBatis', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
-        '': ['*.rst', '*.txt', '*.tpl'],
+        '': ['*.dtd', '*.tpl'],
     },
     include_package_data=True,
-    python_requires='>=3.4.0',
+    python_requires='>=3.6.0',
     zip_safe=False
 )
```

