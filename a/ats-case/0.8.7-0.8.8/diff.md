# Comparing `tmp/ats_case-0.8.7.tar.gz` & `tmp/ats_case-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.8.7.tar", last modified: Sat Jun 17 06:14:57 2023, max compression
+gzip compressed data, was "ats_case-0.8.8.tar", last modified: Mon Jun 19 03:08:01 2023, max compression
```

## Comparing `ats_case-0.8.7.tar` & `ats_case-0.8.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 06:14:57.637641 ats_case-0.8.7/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.8.7/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.8.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-06-17 06:14:57.631662 ats_case-0.8.7/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.8.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 06:14:57.146163 ats_case-0.8.7/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.8.7/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 06:14:57.353406 ats_case-0.8.7/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.8.7/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    18831 2023-06-14 05:51:39.000000 ats_case-0.8.7/ats_case/case/command.py
--rw-rw-rw-   0        0        0    12042 2023-06-17 06:14:22.000000 ats_case-0.8.7/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7505 2023-06-15 02:18:37.000000 ats_case-0.8.7/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.8.7/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-17 06:14:57.453134 ats_case-0.8.7/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.8.7/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.8.7/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.8.7/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-06-17 06:14:57.526937 ats_case-0.8.7/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.7/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.8.7/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.8.7/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-06-17 06:14:57.585785 ats_case-0.8.7/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.7/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2400 2023-05-29 01:45:03.000000 ats_case-0.8.7/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-06-17 06:14:57.238956 ats_case-0.8.7/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-06-17 06:14:56.000000 ats_case-0.8.7/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-06-17 06:14:56.000000 ats_case-0.8.7/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 06:14:56.000000 ats_case-0.8.7/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-17 06:14:56.000000 ats_case-0.8.7/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-17 06:14:56.000000 ats_case-0.8.7/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 06:14:57.638646 ats_case-0.8.7/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-06-17 06:14:44.000000 ats_case-0.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:08:01.526783 ats_case-0.8.8/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.8.8/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.8.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-06-19 03:08:01.524815 ats_case-0.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.8.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 03:08:01.142668 ats_case-0.8.8/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.8.8/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:08:01.350217 ats_case-0.8.8/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.8.8/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    18857 2023-06-19 03:05:41.000000 ats_case-0.8.8/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    12042 2023-06-17 06:14:22.000000 ats_case-0.8.8/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7505 2023-06-15 02:18:37.000000 ats_case-0.8.8/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.8.8/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:08:01.415588 ats_case-0.8.8/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.8.8/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.8.8/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.8.8/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:08:01.477913 ats_case-0.8.8/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.8/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.8.8/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.8.8/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:08:01.516811 ats_case-0.8.8/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.8/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2400 2023-05-29 01:45:03.000000 ats_case-0.8.8/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-06-19 03:08:01.233518 ats_case-0.8.8/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-06-19 03:08:00.000000 ats_case-0.8.8/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-06-19 03:08:00.000000 ats_case-0.8.8/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 03:08:00.000000 ats_case-0.8.8/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-19 03:08:00.000000 ats_case-0.8.8/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-19 03:08:00.000000 ats_case-0.8.8/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 03:08:01.526783 ats_case-0.8.8/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-06-19 02:42:21.000000 ats_case-0.8.8/setup.py
```

### Comparing `ats_case-0.8.7/PKG-INFO` & `ats_case-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.8.7
+Version: 0.8.8
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.8.7/README.md` & `ats_case-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.7/ats_case/case/command.py` & `ats_case-0.8.8/ats_case/case/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,16 +425,14 @@
             self._parameter = _replace_bench0(context, self._parameter)
         if self._function is not None and len(self._function) > 0:
             self._build_in(context)
 
     def decode(self, context: Context):
         logger.info('~ @BENCH<- manufacture:{} operation:{} result:{}'.format(context.bench.manufacture,
                                                                               self._operation, self._result))
-
-        self._result = self._result.get('result')
         self._flush(context)
 
     def _build_in(self, context: Context):
         logger.info('~ @BUILTIN-> module:{} parameter:{}'.format('bench', self._parameter))
         for op, d in self._function.items():
             v_data = build_in.handle(module='bench', function=op, data=func.to_dict(
                 param=d, iabc=context.meter.iabc, voltage=context.meter.rated_voltage,
@@ -467,15 +465,15 @@
 
     def _flush(self, context: Context):
         context.runtime.steps.update({context.runtime.step: func.to_dict(obj='bench', op=self._operation
                                                                          , parameter=self._parameter,
                                                                          result=self._result)})
 
     def rest(self, context: Context):
-        if self._sleep > 0:
+        if self._result == '1' and self._sleep > 0:
             send(context, todo={'app:show': {'msg': '系统休眠{}秒, 等待表台调整完毕...'.format(self._sleep)}})
             sleep(self._sleep)
 
     def _times(self, context: Context):
         if self._interval > 0:
             if context.runtime.loop_index == 0 or (context.runtime.loop_index + 1) % self._interval != 0:
                 return
@@ -484,14 +482,15 @@
 
     def exec(self, context: Context):
         if context.meter.index == 0:
             self._times(context)
 
             self.encode(context)
             self._result = send(context, todo={'bench:{}'.format(self._operation): self._parameter})
+            self._result = self._result.get('result')
             self.decode(context)
 
             send(context, todo={'app:show': {'msg': self.acv(context)}})
 
             self.rest(context)
```

### Comparing `ats_case-0.8.7/ats_case/case/context.py` & `ats_case-0.8.8/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.7/ats_case/case/executor.py` & `ats_case-0.8.8/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.7/ats_case/case/translator.py` & `ats_case-0.8.8/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.7/ats_case/common/error.py` & `ats_case-0.8.8/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.7/ats_case/manage/core.py` & `ats_case-0.8.8/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.7/ats_case/manage/start.py` & `ats_case-0.8.8/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.7/ats_case/template/testcase_v1.tmp` & `ats_case-0.8.8/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.7/ats_case.egg-info/PKG-INFO` & `ats_case-0.8.8/ats_case.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.8.7
+Version: 0.8.8
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.8.7/ats_case.egg-info/SOURCES.txt` & `ats_case-0.8.8/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.7/setup.py` & `ats_case-0.8.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.8.7",
+    version="0.8.8",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

