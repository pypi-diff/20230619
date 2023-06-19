# Comparing `tmp/projhelper-0.1.6.tar.gz` & `tmp/projhelper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/projhelper-0.1.6.tar", last modified: Mon Mar  6 09:26:03 2023, max compression
+gzip compressed data, was "projhelper-0.1.7.tar", last modified: Mon Jun 19 09:57:39 2023, max compression
```

## Comparing `projhelper-0.1.6.tar` & `projhelper-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-06 09:26:12.000000 projhelper-0.1.6/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      148 2021-08-02 01:33:06.000000 projhelper-0.1.6/MANIFEST.in
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      265 2023-03-06 09:26:12.000000 projhelper-0.1.6/PKG-INFO
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-06 09:26:12.000000 projhelper-0.1.6/projhelper/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5281 2023-03-06 09:23:41.000000 projhelper-0.1.6/projhelper/ch_helper.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-06 09:26:12.000000 projhelper-0.1.6/projhelper/conf/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      761 2021-08-02 01:33:06.000000 projhelper-0.1.6/projhelper/conf/conf_dev.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3065 2022-07-15 03:08:40.000000 projhelper-0.1.6/projhelper/conf/logging.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2718 2022-07-15 03:12:09.000000 projhelper-0.1.6/projhelper/conf/logging_win.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5086 2022-07-15 06:07:51.000000 projhelper-0.1.6/projhelper/dbGenerator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1933 2022-07-15 02:38:28.000000 projhelper-0.1.6/projhelper/loadConf.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1772 2022-07-15 03:43:37.000000 projhelper-0.1.6/projhelper/log.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2023 2022-07-15 03:31:48.000000 projhelper-0.1.6/projhelper/osCmd.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1734 2022-12-19 01:25:51.000000 projhelper-0.1.6/projhelper/pushPrometheus.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      332 2021-08-02 01:33:06.000000 projhelper-0.1.6/projhelper/setenv.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1127 2022-07-15 03:33:03.000000 projhelper-0.1.6/projhelper/timeHelper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      155 2021-08-02 01:33:06.000000 projhelper-0.1.6/projhelper/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-06 09:26:12.000000 projhelper-0.1.6/projhelper.egg-info/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-06 09:26:12.000000 projhelper-0.1.6/projhelper.egg-info/dependency_links.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      265 2023-03-06 09:26:12.000000 projhelper-0.1.6/projhelper.egg-info/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      464 2023-03-06 09:26:12.000000 projhelper-0.1.6/projhelper.egg-info/SOURCES.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       11 2023-03-06 09:26:12.000000 projhelper-0.1.6/projhelper.egg-info/top_level.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1650 2023-03-06 09:24:49.000000 projhelper-0.1.6/README.md
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2023-03-06 09:26:12.000000 projhelper-0.1.6/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      720 2023-03-06 09:24:32.000000 projhelper-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:57:39.139509 projhelper-0.1.7/
+-rw-rw-rw-   0        0        0      148 2021-08-02 01:33:06.000000 projhelper-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      276 2023-06-19 09:57:39.139509 projhelper-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1650 2023-03-06 09:24:49.000000 projhelper-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 09:57:39.124508 projhelper-0.1.7/projhelper/
+-rw-rw-rw-   0        0        0      155 2021-08-02 01:33:06.000000 projhelper-0.1.7/projhelper/__init__.py
+-rw-rw-rw-   0        0        0     5281 2023-03-06 09:23:41.000000 projhelper-0.1.7/projhelper/ch_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:57:39.138507 projhelper-0.1.7/projhelper/conf/
+-rw-rw-rw-   0        0        0      761 2021-08-02 01:33:06.000000 projhelper-0.1.7/projhelper/conf/conf_dev.cfg
+-rw-rw-rw-   0        0        0     3065 2022-07-15 03:08:40.000000 projhelper-0.1.7/projhelper/conf/logging.cfg
+-rw-rw-rw-   0        0        0     2718 2022-07-15 03:12:09.000000 projhelper-0.1.7/projhelper/conf/logging_win.cfg
+-rw-rw-rw-   0        0        0     5502 2023-06-19 09:55:52.000000 projhelper-0.1.7/projhelper/dbGenerator.py
+-rw-rw-rw-   0        0        0     1933 2022-07-15 02:38:28.000000 projhelper-0.1.7/projhelper/loadConf.py
+-rw-rw-rw-   0        0        0     1772 2022-07-15 03:43:37.000000 projhelper-0.1.7/projhelper/log.py
+-rw-rw-rw-   0        0        0     2023 2022-07-15 03:31:48.000000 projhelper-0.1.7/projhelper/osCmd.py
+-rw-rw-rw-   0        0        0     1734 2022-12-19 01:25:51.000000 projhelper-0.1.7/projhelper/pushPrometheus.py
+-rw-rw-rw-   0        0        0      332 2021-08-02 01:33:06.000000 projhelper-0.1.7/projhelper/setenv.py
+-rw-rw-rw-   0        0        0     1127 2022-07-15 03:33:03.000000 projhelper-0.1.7/projhelper/timeHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:57:39.135512 projhelper-0.1.7/projhelper.egg-info/
+-rw-rw-rw-   0        0        0      276 2023-06-19 09:57:39.000000 projhelper-0.1.7/projhelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-06-19 09:57:39.000000 projhelper-0.1.7/projhelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:57:39.000000 projhelper-0.1.7/projhelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 09:57:39.000000 projhelper-0.1.7/projhelper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 09:57:39.139509 projhelper-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      720 2023-06-19 09:57:37.000000 projhelper-0.1.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `projhelper-0.1.6/projhelper/ch_helper.py` & `projhelper-0.1.7/projhelper/ch_helper.py`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.6/projhelper/conf/conf_dev.cfg` & `projhelper-0.1.7/projhelper/conf/conf_dev.cfg`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.6/projhelper/conf/logging.cfg` & `projhelper-0.1.7/projhelper/conf/logging.cfg`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.6/projhelper/conf/logging_win.cfg` & `projhelper-0.1.7/projhelper/conf/logging_win.cfg`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.6/projhelper/dbGenerator.py` & `projhelper-0.1.7/projhelper/dbGenerator.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,21 +33,21 @@
                      #设置为"-1"，那么连接池会允许“上溢”无限多
         #实际最大连接数为 pool_size+max_overflow
         '''
         # DML操作加上事务 , 如果不加事务, 用engine.execute执行DML,默认是一个SQL一次提交
         Session = sessionmaker(bind=self.engine)  # 在 engine连接上绑定事务
         self.session = Session()
     #sql_before_exec=["set @@sql_log_bin = 1"])
-    def execute_dml(self,s_sql,commit=1,sql_before_exec=[]):
+    def execute_dml(self,s_sql,params=(),commit=1,sql_before_exec=[]):
         #try:
         # 中间有用 engine.execute 执行DML, 不影响session的事务
         try:
             for bef_sql in sql_before_exec:
                 self.session.execute(bef_sql)
-            res= self.session.execute(s_sql).rowcount
+            res= self.session.execute(s_sql,params).rowcount
             if commit==1:
                 self.session.commit()
             return res
         except BaseException as e:
             logger.error(traceback.format_exc())
             raise e
     #except:
@@ -97,17 +97,32 @@
     #quote_plus 解决密码有特殊字符
     DB_CON_STR = 'mysql+mysqldb://user:%s@localhost:3306/mysql?charset=utf8'%quote_plus('eff%1124&eee')
     s_sql = text("select user,host from mysql.user limit 2")
 
     #mssql
     #DB_CON_STR = 'mssql+pymssql://user:pass@localhost/ccds?charset=utf8'
 
+
+
     db=getDb(DB_CON_STR)
-    #s_sql = " update t_sys_dic t set modifier_global_id=3 where id=229"
-    #db.execute_dml(s_sql)
+
+    #传参： https://www.adamsmith.haus/python/docs/sqlalchemy.orm.session.Session.execute
+    s_sql = text(" update t set str=:str where id=:id")
+    db.execute_dml(s_sql,{'str':'b','id':1})
+
+    s_sql = text(" insert into t values(:id,:str)")
+    db.execute_dml(s_sql,[{'id':2,'str':'b'},{'id':3,'str':'c'}])
+
+    s_sql = text(" update t set str='cd' where id=1")
+    db.execute_dml(s_sql,params=(),commit=1)
+
+
+
+    l_rowsColsWithCol = db.execute_query_return_with_col(s_sql)
+
 
     l_rowsCols = db.execute_query(s_sql)
 
     for t_rowCols in l_rowsCols:
         for col in t_rowCols:
             print (col,)
     #转成  [{u'host': u'%', u'user': u'alog_kettle'}xxx] 格式
```

### Comparing `projhelper-0.1.6/projhelper/loadConf.py` & `projhelper-0.1.7/projhelper/loadConf.py`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.6/projhelper/log.py` & `projhelper-0.1.7/projhelper/log.py`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.6/projhelper/osCmd.py` & `projhelper-0.1.7/projhelper/osCmd.py`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.6/projhelper/pushPrometheus.py` & `projhelper-0.1.7/projhelper/pushPrometheus.py`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.6/projhelper/timeHelper.py` & `projhelper-0.1.7/projhelper/timeHelper.py`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.6/README.md` & `projhelper-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.6/setup.py` & `projhelper-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # @mail  : ojhtyy@163.com
 # @File    : setup.py
 from __future__ import print_function
 from setuptools import setup, find_packages
 import sys
 setup(
     name = "projhelper",
-    version = "0.1.6",
+    version = "0.1.7",
     keywords = ("pip", "datacanvas", "helper", "proj"),
     description = "project base helper, include logger ",
     long_description = "eds sdk for python",
     license = "MIT Licence",
 
     url = "",
     author = "oujh",
```

