# Comparing `tmp/WqUtils-0.0.6-py3-none-any.whl.zip` & `tmp/WqUtils-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2977 bytes, number of entries: 6
--rw-r--r--  2.0 unx     4318 b- defN 23-Jun-15 02:22 WqUtils/Utils.py
+Zip file size: 3311 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     5333 b- defN 23-Jun-19 08:15 WqUtils/Utils.py
 -rw-r--r--  2.0 unx      250 b- defN 22-Nov-25 08:56 WqUtils/__init__.py
--rw-r--r--  2.0 unx      208 b- defN 23-Jun-15 02:24 WqUtils-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 02:24 WqUtils-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-15 02:24 WqUtils-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      444 b- defN 23-Jun-15 02:24 WqUtils-0.0.6.dist-info/RECORD
-6 files, 5320 bytes uncompressed, 2173 bytes compressed:  59.2%
+-rw-r--r--  2.0 unx      208 b- defN 23-Jun-19 15:22 WqUtils-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 15:22 WqUtils-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-19 15:22 WqUtils-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      444 b- defN 23-Jun-19 15:22 WqUtils-0.0.7.dist-info/RECORD
+6 files, 6335 bytes uncompressed, 2507 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: WqUtils/Utils.py
 Comment: 
 
 Filename: WqUtils/__init__.py
 Comment: 
 
-Filename: WqUtils-0.0.6.dist-info/METADATA
+Filename: WqUtils-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: WqUtils-0.0.6.dist-info/WHEEL
+Filename: WqUtils-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: WqUtils-0.0.6.dist-info/top_level.txt
+Filename: WqUtils-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: WqUtils-0.0.6.dist-info/RECORD
+Filename: WqUtils-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## WqUtils/Utils.py

```diff
@@ -8,14 +8,15 @@
 @ LastEditTime: 2022-11-08 17:35
 @ ProjectName: YiliEcommerceNewProductProject
 @ Description: to do
 """
 import os
 import logging
 from logging import handlers
+import toml
 
 
 def get_base_file(name=None):
     base_path = os.path.dirname(os.path.abspath(name))
     return base_path
 
 
@@ -110,10 +111,46 @@
     def warning(self, message):
         self.__console('warning', message)
 
     def error(self, message):
         self.__console('error', message)
 
 
+class TomlConfig:
+    """
+    读写toml对象，实际就是个dict
+    """
+
+    def __init__(self, toml_fileanme):
+        self.t_dict = dict()  # 创建空字典
+        self.toml_file_path = toml_fileanme
+
+    def update(self, t_data):
+        # 给toml文件添加配置
+        self.t_dict.update(t_data)
+        return self.t_dict
+
+    def write(self, t_data):
+        # 写入到toml文件
+        with open(self.toml_file_path, "w", encoding="utf-8") as fs:
+            toml.dump(t_data, fs)
+
+    def read(self):
+        # 读取toml文件
+        with open(self.toml_file_path, "r", encoding="utf-8") as fs:
+            t_data = toml.load(fs)
+        return t_data
+
+    def read_str(self, s_data):
+        # 从字符串中解析TOML，返回一个字典对象或类的实例对象
+        t_data = toml.loads(s_data, _dict=dict)
+        return t_data
+
+    def read_dict(self, dict):
+        # 将字典对象格式化成toml字符串
+        t_data = toml.dumps(dict)
+        return t_data
+
+
 if __name__ == '__main__':
     print(get_base_file(__file__))
```

