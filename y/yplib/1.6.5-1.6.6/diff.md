# Comparing `tmp/yplib-1.6.5.tar.gz` & `tmp/yplib-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.6.5.tar", last modified: Mon Jun 19 01:34:20 2023, max compression
+gzip compressed data, was "dist\yplib-1.6.6.tar", last modified: Mon Jun 19 07:21:13 2023, max compression
```

## Comparing `yplib-1.6.5.tar` & `yplib-1.6.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 01:34:20.162084 yplib-1.6.5/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.6.5/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-19 01:34:20.161652 yplib-1.6.5/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.6.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 01:34:20.162084 yplib-1.6.5/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-19 01:33:47.000000 yplib-1.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:34:20.158059 yplib-1.6.5/yplib/
--rw-rw-rw-   0        0        0      355 2023-06-19 01:15:00.000000 yplib-1.6.5/yplib/__init__.py
--rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.6.5/yplib/chart.py
--rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.6.5/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.6.5/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.6.5/yplib/http_util.py
--rw-rw-rw-   0        0        0    24344 2023-06-19 00:55:36.000000 yplib-1.6.5/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:34:20.161140 yplib-1.6.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-19 01:34:20.000000 yplib-1.6.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-19 01:34:20.000000 yplib-1.6.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 01:34:20.000000 yplib-1.6.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 01:34:20.000000 yplib-1.6.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 07:21:13.838218 yplib-1.6.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.6.6/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-19 07:21:13.838157 yplib-1.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.6.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 07:21:13.838218 yplib-1.6.6/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-19 07:18:22.000000 yplib-1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:21:13.834359 yplib-1.6.6/yplib/
+-rw-rw-rw-   0        0        0      355 2023-06-19 01:15:00.000000 yplib-1.6.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.6.6/yplib/chart.py
+-rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.6.6/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.6.6/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.6.6/yplib/http_util.py
+-rw-rw-rw-   0        0        0    24707 2023-06-19 07:20:57.000000 yplib-1.6.6/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:21:13.837243 yplib-1.6.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-19 07:21:13.000000 yplib-1.6.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-19 07:21:13.000000 yplib-1.6.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 07:21:13.000000 yplib-1.6.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 07:21:13.000000 yplib-1.6.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.6.5/LICENSE` & `yplib-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.6.5/setup.py` & `yplib-1.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.6.5",
+  version="1.6.6",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.6.5/yplib/chart.py` & `yplib-1.6.6/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.5/yplib/chart_html.py` & `yplib-1.6.6/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.5/yplib/file.py` & `yplib-1.6.6/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.5/yplib/http_util.py` & `yplib-1.6.6/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.5/yplib/index.py` & `yplib-1.6.6/yplib/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,21 +43,21 @@
     lo = to_log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
     to_txt([lo], file_name, 'log', True, '.txt')
 
 
 # 将下划线命名转成驼峰命名
 # 例如 : user_id -> userId
 # 例如 : USER_ID -> userId
-def to_hump(a1=''):
-    if a1 == '':
-        return a1
-    a1 = a1.lower()
-    words = a1.split('_')
+def to_hump(s=''):
+    if s == '' or s is None:
+        return s
+    s = s.lower()
+    s1 = s.split('_')
     r = ""
-    for w in words:
+    for w in s1:
         r += w.capitalize()
     return r[0].lower() + r[1:]
 
 
 def to_hump_more(a1='', a2='', a3='', a4='', a5=''):
     if a1 == '':
         return a1
@@ -70,23 +70,23 @@
     elif a5 == '':
         return to_hump(a1), to_hump(a2), to_hump(a3), to_hump(a4)
     return to_hump(a1), to_hump(a2), to_hump(a3), to_hump(a4), to_hump(a5)
 
 
 # 将驼峰命名转成下划线命名
 # 例如 : userId -> user_id
-def to_underline(a1=''):
-    if a1 == '':
-        return a1
+def to_underline(s=''):
+    if s == '' or s is None:
+        return s
     r = ''
-    for char in a1:
-        if char.isupper():
-            r += '_' + char.lower()
+    for c in s:
+        if c.isupper():
+            r += '_' + c.lower()
         else:
-            r += char
+            r += c
     return r
 
 
 def to_underline_more(a1='', a2='', a3='', a4='', a5=''):
     if a1 == '':
         return a1
     elif a2 == '':
@@ -111,20 +111,18 @@
 def check_file(file_name):
     if file_name != '' and os.path.exists(file_name) is False:
         os.mkdir(file_name)
 
 
 # 获得文件名称
 def get_file_name(file_name, suffix='.txt'):
-    ns = str(datetime.now()).split('.')[1]
-    t = datetime.today().strftime('%m%d%H%M_%S').split('_')
-    # '%Y-%m-%d %H:%M:%S'
+    t = datetime.today().strftime('%d%H%M_%S_%f').split('_')
     return str(file_name) \
         + '_' + t[0] \
-        + '_' + t[1] + ns[0] + random_int(1) \
+        + '_' + t[1] + t[2][0] + random_int(1) \
         + suffix
 
 
 # 获得文件名称
 def file_is_empty(file_name=None):
     return file_name is None or file_name == '' or os.path.exists(file_name) is False
 
@@ -243,21 +241,24 @@
 # 将 list 中的数据以 json 或者基本类型的形式写入到文件中
 # data_list : 数组数据, 也可以不是数组
 # file_name : 文件名
 # fixed_name : 是否固定文件名
 # file_path : 文件路径
 def to_txt(data_list, file_name='txt', file_path='txt', fixed_name=False, suffix='.txt'):
     file_name = str(file_name)
+    # 检查路径 file_path
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
+    # 生成 file_name
     if fixed_name:
         file_name = file_name + suffix
     else:
         file_name = get_file_name(file_name, suffix)
+    # 文件路径
     file_name_path = file_name
     if file_path != '':
         file_name_path = file_path + '/' + file_name
     text_file = open(file_name_path, 'a', encoding='utf-8')
     if isinstance(data_list, list) is False:
         text_file.write(to_str(data_list) + '\n')
     else:
@@ -277,20 +278,28 @@
         s = json.dumps(data)
     else:
         s = str(data)
     return s
 
 
 # 根据json的key排序,用于签名
-def sort_by_json_key(data):
-    data_key_sort = sorted(data, key=lambda x: x[0])
-    r_list = []
-    for one_key in data_key_sort:
-        r_list.append(one_key + '=' + data[one_key])
-    return '&'.join(r_list)
+def sort_by_json_key(data_obj):
+    return '&'.join(list(map(
+        lambda x: f'{x}={data_obj[x]}',
+        sorted(data_obj, key=lambda x: x[0])
+    )))
+
+
+# data = {}
+# data['merchantId'] = "merchantId"
+# data['currency'] = "IDR"
+# data['accType'] = "payout"
+# data['version'] = "1.0"
+# sign = sort_by_json_key(data)
+# print(sign)
 
 
 # 当读取 txt 之类的文件的时候
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
 # separator : 是否对每一行进行分割,如果存在这个字段,就分割
 # separator_all : 将文件转化成一个字符串,然后对这个字符串,再次总体分割
 # start_index : 从这个地方开始读取,从1开始标号 , 包含这一行
@@ -676,7 +685,17 @@
 # print(get_file_name('a'))
 
 # print(to_list(r'D:\notepad_file\202306\asfdf.html', start_index=1285, end_index=1288))
 # print(to_list(r'D:\notepad_file\202306\asfdf.html', start_index=1285, count=3))
 # print(to_list(r'D:\notepad_file\202306\asfdf.html', start_line='<h2>Unicode 字符串</h2>', count=1))
 # print(to_list(r'D:\notepad_file\202306\asfdf.html', start_line='<h2>Unicode 字符串</h2>', end_line='所有的字符串都是Unicode字符串'))
 # print(to_list(r'D:\notepad_file\202306\asfdf.html', start_line='<h2>Unicode 字符串</h2>', end_line='所有的字符串都是Unicode字符串'))
+
+#
+# print(datetime.now())
+# print(datetime.today())
+# print(datetime.today().strftime('%m%d%H%M_%S_%f'))
+# print(get_file_name('1'))
+#
+# for i in range(100):
+#     print(get_file_name('a'))
+#     # print(random_int(i))
```

