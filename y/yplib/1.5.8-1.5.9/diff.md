# Comparing `tmp/yplib-1.5.8.tar.gz` & `tmp/yplib-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.5.8.tar", last modified: Mon Jun 19 00:11:30 2023, max compression
+gzip compressed data, was "dist\yplib-1.5.9.tar", last modified: Mon Jun 19 00:52:32 2023, max compression
```

## Comparing `yplib-1.5.8.tar` & `yplib-1.5.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 00:11:30.026224 yplib-1.5.8/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.8/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-19 00:11:30.026224 yplib-1.5.8/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 00:11:30.026224 yplib-1.5.8/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-19 00:11:11.000000 yplib-1.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 00:11:30.023277 yplib-1.5.8/yplib/
--rw-rw-rw-   0        0        0      357 2023-06-16 03:11:06.000000 yplib-1.5.8/yplib/__init__.py
--rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.5.8/yplib/chart.py
--rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.5.8/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.8/yplib/file.py
--rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.8/yplib/html_parser.py
--rw-rw-rw-   0        0        0    21818 2023-06-19 00:09:12.000000 yplib-1.5.8/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-19 00:11:30.025318 yplib-1.5.8/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-19 00:11:29.000000 yplib-1.5.8/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-19 00:11:29.000000 yplib-1.5.8/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 00:11:29.000000 yplib-1.5.8/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 00:11:29.000000 yplib-1.5.8/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 00:52:32.715611 yplib-1.5.9/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.9/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-19 00:52:32.715611 yplib-1.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 00:52:32.715611 yplib-1.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-19 00:52:23.000000 yplib-1.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:52:32.706293 yplib-1.5.9/yplib/
+-rw-rw-rw-   0        0        0      357 2023-06-16 03:11:06.000000 yplib-1.5.9/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.5.9/yplib/chart.py
+-rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.5.9/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.9/yplib/file.py
+-rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.9/yplib/html_parser.py
+-rw-rw-rw-   0        0        0    24191 2023-06-19 00:51:57.000000 yplib-1.5.9/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:52:32.714386 yplib-1.5.9/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-19 00:52:32.000000 yplib-1.5.9/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-19 00:52:32.000000 yplib-1.5.9/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 00:52:32.000000 yplib-1.5.9/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 00:52:32.000000 yplib-1.5.9/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.5.8/LICENSE` & `yplib-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.5.8/setup.py` & `yplib-1.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.5.8",
+  version="1.5.9",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.5.8/yplib/chart.py` & `yplib-1.5.9/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.8/yplib/chart_html.py` & `yplib-1.5.9/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.8/yplib/file.py` & `yplib-1.5.9/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.8/yplib/html_parser.py` & `yplib-1.5.9/yplib/html_parser.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.8/yplib/index.py` & `yplib-1.5.9/yplib/index.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,14 +120,19 @@
     # '%Y-%m-%d %H:%M:%S'
     return str(file_name) \
         + '_' + t[0] \
         + '_' + t[1] + ns[0] + random_int(1) \
         + suffix
 
 
+# 获得文件名称
+def file_is_empty(file_name=None):
+    return file_name is None or file_name == '' or os.path.exists(file_name) is False
+
+
 def do_md5(data='do_md5'):
     return hashlib.md5(data.encode(encoding='UTF-8')).hexdigest()
 
 
 def do_sha256(data='do_sha256'):
     h = hashlib.sha256()
     h.update(data.encode('utf-8'))
@@ -311,117 +316,165 @@
             end_index=None,
             end_line=None,
             count=None,
             sheet_index=1,
             column_index=None,
             column_date=None,
             column_datetime=None):
-    if file_name is None or file_name == '' or os.path.exists(file_name) is False:
+    if file_name.endswith('.xls') or file_name.endswith('.xlsx'):
+        return to_list_from_excel(file_name=file_name,
+                                  sheet_index=sheet_index,
+                                  column_index=column_index,
+                                  column_date=column_date,
+                                  column_datetime=column_datetime)
+    return to_list_from_txt(file_name=file_name,
+                            separator=separator,
+                            separator_all=separator_all,
+                            start_index=start_index,
+                            start_line=start_line,
+                            end_index=end_index,
+                            end_line=end_line,
+                            count=count)
+
+
+# 当读取 excel 之类的文件的时候
+# 将 excel 文件读取到 list 中, 可以指定 sheet, 也可以指定列 column_index(列) ,自动过滤掉每个单元格前后的特殊字符
+# sheet_index  : 从 1 开始编号,
+# column_index : 从 1 开始编号, 指定列, 如果是指定值是一个, 这个时候返回的是一个 list, 没有嵌套 list
+#                如果是 '1,2,3,4'   [1,2,3,4], 返回的是一个嵌套 list[list]
+# column_date :  指定日期格式的列,规则与 column_index 一样
+# column_datetime : 指定日期格式的列,规则与 column_index 一样
+def to_list_from_excel(file_name='a.xls',
+                       sheet_index=1,
+                       column_index=None,
+                       column_date=None,
+                       column_datetime=None):
+    if file_is_empty(file_name):
         return []
     data_list = list()
     # excel 表格解析成 list 数据
-    if file_name.endswith('.xls') or file_name.endswith('.xlsx'):
-        list_index = []
-        for one_index in [column_index, column_date, column_datetime]:
-            list_index_one = None
-            if one_index is not None:
-                list_index_one = []
-                if isinstance(one_index, int):
-                    list_index_one.append(one_index)
-                if isinstance(one_index, str):
-                    i_list = one_index.split(',')
-                    for i in i_list:
-                        list_index_one.append(int(i))
-                if isinstance(one_index, list):
-                    for i in one_index:
-                        list_index_one.append(int(i))
-            list_index.append(list_index_one)
-        list_all = []
-        for one_list in list_index:
-            if one_list is not None:
-                for o in one_list:
-                    list_all.append(o)
-        if len(list_all) > 0 and list_index[0] is not None:
-            list_index[0] = list_all
-        # 是否是单 list 类型的数据
-        list_only_one = False
-        if list_index[0] is not None and len(list_index[0]) == 1:
-            list_only_one = True
-        book = xlrd.open_workbook(file_name)  # 打开一个excel
-        sheet = book.sheet_by_index(sheet_index - 1)  # 根据顺序获取sheet
-        for i in range(sheet.nrows):  # 0 1 2 3 4 5
-            rows = sheet.row_values(i)
-            row_data = []
-            for j in range(len(rows)):
-                cell_data = str(rows[j]).strip()
-                is_date = False
-                is_datetime = False
-                # 日期格式的列
-                if list_index[1] is not None and j + 1 in list_index[1]:
-                    cell_data = to_date(xlrd.xldate_as_datetime(to_int(rows[j]), 0))
-                    is_date = True
+    list_index = []
+    for one_index in [column_index, column_date, column_datetime]:
+        list_index_one = None
+        if one_index is not None:
+            list_index_one = []
+            if isinstance(one_index, int):
+                list_index_one.append(one_index)
+            if isinstance(one_index, str):
+                i_list = one_index.split(',')
+                for i in i_list:
+                    list_index_one.append(int(i))
+            if isinstance(one_index, list):
+                for i in one_index:
+                    list_index_one.append(int(i))
+        list_index.append(list_index_one)
+    list_all = []
+    for one_list in list_index:
+        if one_list is not None:
+            for o in one_list:
+                list_all.append(o)
+    if len(list_all) > 0 and list_index[0] is not None:
+        list_index[0] = list_all
+    # 是否是单 list 类型的数据
+    list_only_one = False
+    if list_index[0] is not None and len(list_index[0]) == 1:
+        list_only_one = True
+    book = xlrd.open_workbook(file_name)  # 打开一个excel
+    sheet = book.sheet_by_index(sheet_index - 1)  # 根据顺序获取sheet
+    for i in range(sheet.nrows):  # 0 1 2 3 4 5
+        rows = sheet.row_values(i)
+        row_data = []
+        for j in range(len(rows)):
+            cell_data = str(rows[j]).strip()
+            is_date = False
+            is_datetime = False
+            # 日期格式的列
+            if list_index[1] is not None and j + 1 in list_index[1]:
+                cell_data = to_date(xlrd.xldate_as_datetime(to_int(rows[j]), 0))
+                is_date = True
+                row_data.append(cell_data)
+                if list_only_one:
+                    row_data = cell_data
+            # 日期时间格式的列
+            if is_date is False and list_index[2] is not None and j + 1 in list_index[2]:
+                cell_data = to_datetime(xlrd.xldate_as_datetime(to_int(rows[j]), 0))
+                is_datetime = True
+                row_data.append(cell_data)
+                if list_only_one:
+                    row_data = cell_data
+            # 指定需要的列
+            if is_date is False and is_datetime is False:
+                if list_index[0] is None:
                     row_data.append(cell_data)
-                    if list_only_one:
-                        row_data = cell_data
-                # 日期时间格式的列
-                if is_date is False and list_index[2] is not None and j + 1 in list_index[2]:
-                    cell_data = to_datetime(xlrd.xldate_as_datetime(to_int(rows[j]), 0))
-                    is_datetime = True
-                    row_data.append(cell_data)
-                    if list_only_one:
-                        row_data = cell_data
-                # 指定需要的列
-                if is_date is False and is_datetime is False:
-                    if list_index[0] is None:
+                else:
+                    # 指定需要的列
+                    if j + 1 in list_index[0]:
                         row_data.append(cell_data)
-                    else:
-                        # 指定需要的列
-                        if j + 1 in list_index[0]:
-                            row_data.append(cell_data)
-                            if list_only_one:
-                                row_data = cell_data
-            data_list.append(row_data)
-    else:
-        # 普通文件的解析
-        d_list = open(file_name, 'r', encoding='utf-8').readlines()
-        c = 0
-        start_flag = None
-        end_flag = None
-        if start_line is not None:
-            start_flag = False
-        if end_line is not None:
-            end_flag = False
-        for i in range(len(d_list)):
-            line = d_list[i].strip()
-            # 判断开始位置
-            if start_index is not None and i + 1 < to_int(start_index):
-                continue
-            # 判断结束位置
-            if end_index is not None and i + 1 >= to_int(end_index):
-                continue
-            # 判断数量
-            if count is not None and c >= to_int(count):
-                continue
-            # 开始标记位
-            if start_flag is False and line.find(start_line) > -1:
-                start_flag = True
-            # 开始标记位
-            if end_flag is False and line.find(end_line) > -1:
-                end_flag = True
-            if start_flag is False:
-                continue
-            elif end_flag:
-                continue
-            c += 1
-            if separator is not None:
-                data_list.append(line.split(str(separator)))
-            else:
-                data_list.append(line)
-        if separator_all is not None:
-            data_list = ''.join(data_list).split(str(separator_all))
+                        if list_only_one:
+                            row_data = cell_data
+        data_list.append(row_data)
+
+
+# 当读取 txt 之类的文件的时候
+# 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
+# separator : 是否对每一行进行分割,如果存在这个字段,就分割
+# separator_all : 将文件转化成一个字符串,然后对这个字符串,再次总体分割
+# start_index : 从这个地方开始读取,从1开始标号 , 包含这一行
+# start_line :  从这个地方开始读取,从第一行开始找到这个字符串开始标记 , 包含这一行
+# end_index :   读取到这个地方结束,从1开始标号 , 不包含这一行
+# end_line :    读取到这个地方结束,从第一行开始找到这个字符串开始标记 , 不包含这一行
+# count :       读取指定的行数
+def to_list_from_txt(file_name='a.txt',
+                     separator=None,
+                     separator_all=None,
+                     start_index=None,
+                     start_line=None,
+                     end_index=None,
+                     end_line=None,
+                     count=None):
+    if file_is_empty(file_name=file_name):
+        return []
+    data_list = list()
+    # 普通文件的解析
+    d_list = open(file_name, 'r', encoding='utf-8').readlines()
+    c = 0
+    start_flag = None
+    end_flag = None
+    if start_line is not None:
+        start_flag = False
+    if end_line is not None:
+        end_flag = False
+    for i in range(len(d_list)):
+        line = d_list[i].strip()
+        # 判断开始位置
+        if start_index is not None and i + 1 < to_int(start_index):
+            continue
+        # 判断结束位置
+        if end_index is not None and i + 1 >= to_int(end_index):
+            continue
+        # 判断数量
+        if count is not None and c >= to_int(count):
+            continue
+        # 开始标记位
+        if start_flag is False and line.find(start_line) > -1:
+            start_flag = True
+        # 开始标记位
+        if end_flag is False and line.find(end_line) > -1:
+            end_flag = True
+        if start_flag is False:
+            continue
+        elif end_flag:
+            continue
+        c += 1
+        if separator is not None:
+            data_list.append(line.split(str(separator)))
+        else:
+            data_list.append(line)
+    if separator_all is not None:
+        data_list = ''.join(data_list).split(str(separator_all))
     return data_list
 
 
 # 在 to_list 方法上再嵌套一层,
 # r_str : 返回的数据是否是一个 字符串, ''.join(list)
 # r_json : 返回的数据是否是一个 json 类型的数据
 def to_list_data(file_name='a.txt',
```

