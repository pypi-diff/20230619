# Comparing `tmp/pipeline-data-1.2.3.tar.gz` & `tmp/pipeline-data-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline-data-1.2.3.tar", last modified: Thu Jun 15 03:16:06 2023, max compression
+gzip compressed data, was "pipeline-data-1.2.4.tar", last modified: Mon Jun 19 06:30:53 2023, max compression
```

## Comparing `pipeline-data-1.2.3.tar` & `pipeline-data-1.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-15 03:16:06.261892 pipeline-data-1.2.3/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       97 2023-06-15 03:16:06.260639 pipeline-data-1.2.3/PKG-INFO
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-15 03:16:06.046741 pipeline-data-1.2.3/pipeline_data/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      163 2022-10-21 07:17:13.000000 pipeline-data-1.2.3/pipeline_data/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7894 2022-10-21 07:21:49.000000 pipeline-data-1.2.3/pipeline_data/lock.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    28399 2023-02-24 08:33:16.000000 pipeline-data-1.2.3/pipeline_data/pipeline.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-15 03:16:06.164801 pipeline-data-1.2.3/pipeline_data/sqla_decorator/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      595 2022-09-13 05:51:43.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    28892 2022-09-13 05:51:43.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/engine.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    29600 2022-09-13 05:51:43.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/manager.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2787 2023-02-24 08:38:10.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/models.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4240 2022-09-13 05:51:43.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/session_ctx.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-15 03:16:06.246986 pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      266 2022-10-21 06:22:51.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    19197 2023-06-15 02:54:48.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/db.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4726 2022-09-13 05:51:43.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/explain.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1373 2022-09-13 05:51:43.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/query_count.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3560 2022-10-21 06:12:05.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/tool.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-15 03:16:06.099030 pipeline-data-1.2.3/pipeline_data.egg-info/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       97 2023-06-15 03:16:05.000000 pipeline-data-1.2.3/pipeline_data.egg-info/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      696 2023-06-15 03:16:05.000000 pipeline-data-1.2.3/pipeline_data.egg-info/SOURCES.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-15 03:16:05.000000 pipeline-data-1.2.3/pipeline_data.egg-info/dependency_links.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       90 2023-06-15 03:16:05.000000 pipeline-data-1.2.3/pipeline_data.egg-info/requires.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       14 2023-06-15 03:16:05.000000 pipeline-data-1.2.3/pipeline_data.egg-info/top_level.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-15 03:16:06.263254 pipeline-data-1.2.3/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      513 2023-06-15 02:54:48.000000 pipeline-data-1.2.3/setup.py
+drwxr-xr-x   0 kewei      (501) staff       (20)        0 2023-06-19 06:30:53.414615 pipeline-data-1.2.4/
+-rw-r--r--   0 kewei      (501) staff       (20)       97 2023-06-19 06:30:53.414786 pipeline-data-1.2.4/PKG-INFO
+drwxr-xr-x   0 kewei      (501) staff       (20)        0 2023-06-19 06:30:53.407236 pipeline-data-1.2.4/pipeline_data/
+-rwxrwxrwx   0 kewei      (501) staff       (20)      163 2022-10-21 07:17:13.000000 pipeline-data-1.2.4/pipeline_data/__init__.py
+-rwxrwxrwx   0 kewei      (501) staff       (20)     7858 2023-06-19 05:34:44.000000 pipeline-data-1.2.4/pipeline_data/lock.py
+-rwxrwxrwx   0 kewei      (501) staff       (20)    28399 2023-02-24 08:33:16.000000 pipeline-data-1.2.4/pipeline_data/pipeline.py
+drwxr-xr-x   0 kewei      (501) staff       (20)        0 2023-06-19 06:30:53.411782 pipeline-data-1.2.4/pipeline_data/sqla_decorator/
+-rwxrwxrwx   0 kewei      (501) staff       (20)      595 2022-09-13 05:51:43.000000 pipeline-data-1.2.4/pipeline_data/sqla_decorator/__init__.py
+-rwxrwxrwx   0 kewei      (501) staff       (20)    28892 2022-09-13 05:51:43.000000 pipeline-data-1.2.4/pipeline_data/sqla_decorator/engine.py
+-rwxrwxrwx   0 kewei      (501) staff       (20)    29600 2022-09-13 05:51:43.000000 pipeline-data-1.2.4/pipeline_data/sqla_decorator/manager.py
+-rwxrwxrwx   0 kewei      (501) staff       (20)     2787 2023-02-24 08:38:10.000000 pipeline-data-1.2.4/pipeline_data/sqla_decorator/models.py
+-rwxrwxrwx   0 kewei      (501) staff       (20)     4240 2022-09-13 05:51:43.000000 pipeline-data-1.2.4/pipeline_data/sqla_decorator/session_ctx.py
+drwxr-xr-x   0 kewei      (501) staff       (20)        0 2023-06-19 06:30:53.414312 pipeline-data-1.2.4/pipeline_data/sqla_decorator/utils/
+-rwxrwxrwx   0 kewei      (501) staff       (20)      266 2022-10-21 06:22:51.000000 pipeline-data-1.2.4/pipeline_data/sqla_decorator/utils/__init__.py
+-rwxrwxrwx   0 kewei      (501) staff       (20)    20391 2023-06-19 06:22:53.000000 pipeline-data-1.2.4/pipeline_data/sqla_decorator/utils/db.py
+-rwxrwxrwx   0 kewei      (501) staff       (20)     4726 2022-09-13 05:51:43.000000 pipeline-data-1.2.4/pipeline_data/sqla_decorator/utils/explain.py
+-rwxrwxrwx   0 kewei      (501) staff       (20)     1373 2022-09-13 05:51:43.000000 pipeline-data-1.2.4/pipeline_data/sqla_decorator/utils/query_count.py
+-rwxrwxrwx   0 kewei      (501) staff       (20)     3560 2022-10-21 06:12:05.000000 pipeline-data-1.2.4/pipeline_data/sqla_decorator/utils/tool.py
+drwxr-xr-x   0 kewei      (501) staff       (20)        0 2023-06-19 06:30:53.409266 pipeline-data-1.2.4/pipeline_data.egg-info/
+-rwxrwxrwx   0 kewei      (501) staff       (20)       97 2023-06-19 06:30:53.000000 pipeline-data-1.2.4/pipeline_data.egg-info/PKG-INFO
+-rwxrwxrwx   0 kewei      (501) staff       (20)      706 2023-06-19 06:30:53.000000 pipeline-data-1.2.4/pipeline_data.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kewei      (501) staff       (20)        1 2023-06-19 06:30:53.000000 pipeline-data-1.2.4/pipeline_data.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kewei      (501) staff       (20)       90 2023-06-19 06:30:53.000000 pipeline-data-1.2.4/pipeline_data.egg-info/requires.txt
+-rwxrwxrwx   0 kewei      (501) staff       (20)       14 2023-06-19 06:30:53.000000 pipeline-data-1.2.4/pipeline_data.egg-info/top_level.txt
+-rwxrwxrwx   0 kewei      (501) staff       (20)       38 2023-06-19 06:30:53.415349 pipeline-data-1.2.4/setup.cfg
+-rwxrwxrwx   0 kewei      (501) staff       (20)      513 2023-06-19 06:30:50.000000 pipeline-data-1.2.4/setup.py
```

### Comparing `pipeline-data-1.2.3/pipeline_data/lock.py` & `pipeline-data-1.2.4/pipeline_data/lock.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,16 +60,14 @@
                 res = session.execute(insert_sql)
                 session.commit()
 
                 return True
             except IntegrityError as ie:
                 # 主键冲突
                 res = session.execute(select_sql)
-                session.commit()
-
                 res = sqlalchemy_result_format(res)
                 # 若主键冲突，且没有查到对应的记录，则等待0.5s，跳过下面的判断
                 # tidb会出现的情况，可能是由于tidb是分布式的，在某一个节点上查询不到对应的数据，
                 # 需要等待一会，数据同步之后，才能查出来
                 if not res:
                     time.sleep(0.5)
                     continue
```

### Comparing `pipeline-data-1.2.3/pipeline_data/pipeline.py` & `pipeline-data-1.2.4/pipeline_data/pipeline.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.3/pipeline_data/sqla_decorator/__init__.py` & `pipeline-data-1.2.4/pipeline_data/sqla_decorator/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.3/pipeline_data/sqla_decorator/engine.py` & `pipeline-data-1.2.4/pipeline_data/sqla_decorator/engine.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.3/pipeline_data/sqla_decorator/manager.py` & `pipeline-data-1.2.4/pipeline_data/sqla_decorator/manager.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.3/pipeline_data/sqla_decorator/models.py` & `pipeline-data-1.2.4/pipeline_data/sqla_decorator/models.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.3/pipeline_data/sqla_decorator/session_ctx.py` & `pipeline-data-1.2.4/pipeline_data/sqla_decorator/session_ctx.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/db.py` & `pipeline-data-1.2.4/pipeline_data/sqla_decorator/utils/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,21 @@
 
 from sqlalchemy import update, and_, case, select, desc
 from sqlalchemy.orm.session import Session
 
 from ..session_ctx import ctx_session
 
 try:
+    from sqlalchemy.engine.row import Row
+    from sqlalchemy.engine.result import ChunkedIteratorResult
+    sqlalchemy_version = '1.4'
+except ModuleNotFoundError:
+    sqlalchemy_version = '1.3'
+
+try:
     from sqlalchemy.engine.result import ResultProxy, RowProxy, ChunkedIteratorResult
 except ImportError:
     # sqlalchemy 1.4以上用法
     from sqlalchemy.engine.cursor import CursorResult as ResultProxy
     from sqlalchemy.engine.row import RowProxy
     from sqlalchemy.engine.result import ChunkedIteratorResult
 
@@ -124,14 +131,17 @@
             results = results.fetchall()
         else:
             results = results.all()
 
     if not results or not isinstance(results, list):
         return results
 
+    if hasattr(results[0], '_data') and hasattr(results[0]._data[0], 'metadata'):
+        results = [d[0] for d in results]
+
     keys = sqlalchemy_result_field_format(results[0])
 
     output = []
     for result in results:
         option = {}
         if result is None:
             output.append(option)
@@ -144,14 +154,50 @@
             else:
                 option[k] = v
 
         output.append(option)
     return output
 
 
+def result_to_dict_1_4(res):
+    result = res.all()
+    if not result:
+        return []
+
+    if sqlalchemy_version == '1.4' and \
+            isinstance(result[0], Row):
+        return result_to_dict_1_3(result)
+        result = [d[0] for d in result]
+
+
+    format_res = []
+    for one in result:
+        res = vars(one)
+        if '_sa_instance_state' in res:
+            del res['_sa_instance_state']
+
+        format_res.append(res)
+
+    return format_res
+
+
+def result_to_dict_1_3(result):
+    result = [dict(row) for row in result]
+
+    return result
+
+
+def sqlalchemy_result_format_new(result):
+    if isinstance(result, Query) or \
+            (sqlalchemy_version == '1.4' and isinstance(result, ChunkedIteratorResult)):
+        return result_to_dict_1_4(result)
+    else:
+        return result_to_dict_1_3(result)
+
+
 def sqlalchemy_data_commit(models,
                            data_lst: list, mode='ignore',
                            on_duplicate_key='',
                            auto_commit=False,
                            filter_args: set = None,
                            ignore_exception=True):
     """
```

### Comparing `pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/explain.py` & `pipeline-data-1.2.4/pipeline_data/sqla_decorator/utils/explain.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/query_count.py` & `pipeline-data-1.2.4/pipeline_data/sqla_decorator/utils/query_count.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/tool.py` & `pipeline-data-1.2.4/pipeline_data/sqla_decorator/utils/tool.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.3/pipeline_data.egg-info/SOURCES.txt` & `pipeline-data-1.2.4/pipeline_data.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+setup.cfg
 setup.py
 pipeline_data/__init__.py
 pipeline_data/lock.py
 pipeline_data/pipeline.py
 pipeline_data.egg-info/PKG-INFO
 pipeline_data.egg-info/SOURCES.txt
 pipeline_data.egg-info/dependency_links.txt
```

### Comparing `pipeline-data-1.2.3/setup.py` & `pipeline-data-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Time      :2022/10/21 14:26
 # @Author    :huangkewei
 
 import setuptools
 
 setuptools.setup(
     name='pipeline-data',
-    version='1.2.3',
+    version='1.2.4',
     author='zhongbiao',
     description='数据同步',
     packages=setuptools.find_packages(),
     install_requires=[
         'sqlalchemy~=1.4.0',
         'pottery==3.0.0',
         'werkzeug',
```

