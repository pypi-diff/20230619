# Comparing `tmp/gggdtparser-0.0.9.tar.gz` & `tmp/gggdtparser-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gggdtparser-0.0.9.tar", last modified: Tue May 30 11:55:17 2023, max compression
+gzip compressed data, was "gggdtparser-0.1.0.tar", last modified: Mon Jun 19 03:16:00 2023, max compression
```

## Comparing `gggdtparser-0.0.9.tar` & `gggdtparser-0.1.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 11:55:17.916194 gggdtparser-0.0.9/
--rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggdtparser-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     3404 2023-05-30 11:55:17.916194 gggdtparser-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2689 2023-04-10 04:20:03.000000 gggdtparser-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 11:55:17.873308 gggdtparser-0.0.9/gggdtparser/
--rw-rw-rw-   0        0        0      227 2023-05-16 08:44:33.000000 gggdtparser-0.0.9/gggdtparser/__init__.py
--rw-rw-rw-   0        0        0     2824 2023-05-30 08:08:48.000000 gggdtparser-0.0.9/gggdtparser/dtconfigs.py
--rw-rw-rw-   0        0        0    17946 2023-05-30 06:56:51.000000 gggdtparser-0.0.9/gggdtparser/dtparser.py
-drwxrwxrwx   0        0        0        0 2023-05-30 11:55:17.901234 gggdtparser-0.0.9/gggdtparser/langs/
--rw-rw-rw-   0        0        0       88 2023-04-20 07:19:51.000000 gggdtparser-0.0.9/gggdtparser/langs/__init__.py
--rw-rw-rw-   0        0        0      235 2023-05-30 07:17:00.000000 gggdtparser-0.0.9/gggdtparser/langs/_id.py
--rw-rw-rw-   0        0        0      246 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/az.py
--rw-rw-rw-   0        0        0      678 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/de.py
--rw-rw-rw-   0        0        0     4773 2023-05-30 07:53:40.000000 gggdtparser-0.0.9/gggdtparser/langs/default.py
--rw-rw-rw-   0        0        0     3399 2023-05-30 08:20:26.000000 gggdtparser-0.0.9/gggdtparser/langs/en.py
--rw-rw-rw-   0        0        0      703 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/es.py
--rw-rw-rw-   0        0        0      943 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/fra.py
--rw-rw-rw-   0        0        0      223 2023-05-30 08:08:07.000000 gggdtparser-0.0.9/gggdtparser/langs/hi.py
--rw-rw-rw-   0        0        0      239 2023-05-30 06:33:25.000000 gggdtparser-0.0.9/gggdtparser/langs/ky.py
--rw-rw-rw-   0        0        0      345 2023-05-30 07:58:49.000000 gggdtparser-0.0.9/gggdtparser/langs/mr.py
--rw-rw-rw-   0        0        0      804 2023-05-30 07:50:28.000000 gggdtparser-0.0.9/gggdtparser/langs/ru.py
--rw-rw-rw-   0        0        0      249 2023-05-30 07:52:16.000000 gggdtparser-0.0.9/gggdtparser/langs/rw.py
--rw-rw-rw-   0        0        0      238 2023-05-30 08:00:58.000000 gggdtparser-0.0.9/gggdtparser/langs/si.py
--rw-rw-rw-   0        0        0      230 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/so.py
--rw-rw-rw-   0        0        0      329 2023-05-30 07:55:53.000000 gggdtparser-0.0.9/gggdtparser/langs/sw.py
--rw-rw-rw-   0        0        0      745 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/swe.py
--rw-rw-rw-   0        0        0      195 2023-05-30 08:05:09.000000 gggdtparser-0.0.9/gggdtparser/langs/tg.py
--rw-rw-rw-   0        0        0      300 2023-05-30 08:05:26.000000 gggdtparser-0.0.9/gggdtparser/langs/tr.py
--rw-rw-rw-   0        0        0      811 2023-05-30 07:48:04.000000 gggdtparser-0.0.9/gggdtparser/langs/uk.py
--rw-rw-rw-   0        0        0      231 2023-05-30 06:37:38.000000 gggdtparser-0.0.9/gggdtparser/langs/ur.py
--rw-rw-rw-   0        0        0      432 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/vie.py
--rw-rw-rw-   0        0        0      802 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/zh.py
--rw-rw-rw-   0        0        0      609 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/zht.py
-drwxrwxrwx   0        0        0        0 2023-05-30 11:55:17.915197 gggdtparser-0.0.9/gggdtparser/test/
--rw-rw-rw-   0        0        0    43437 2023-05-25 04:15:16.000000 gggdtparser-0.0.9/gggdtparser/test/__init__.py
--rw-rw-rw-   0        0        0      112 2023-05-30 07:17:35.000000 gggdtparser-0.0.9/gggdtparser/test/_id.py
--rw-rw-rw-   0        0        0      829 2023-04-20 08:57:23.000000 gggdtparser-0.0.9/gggdtparser/test/az.py
--rw-rw-rw-   0        0        0      120 2023-05-30 08:08:48.000000 gggdtparser-0.0.9/gggdtparser/test/hi.py
--rw-rw-rw-   0        0        0      118 2023-05-30 06:34:41.000000 gggdtparser-0.0.9/gggdtparser/test/ky.py
--rw-rw-rw-   0        0        0      211 2023-05-30 07:59:04.000000 gggdtparser-0.0.9/gggdtparser/test/mr.py
--rw-rw-rw-   0        0        0      117 2023-05-30 07:52:38.000000 gggdtparser-0.0.9/gggdtparser/test/ru.py
--rw-rw-rw-   0        0        0      136 2023-05-30 07:52:38.000000 gggdtparser-0.0.9/gggdtparser/test/rw.py
--rw-rw-rw-   0        0        0      129 2023-05-30 08:01:52.000000 gggdtparser-0.0.9/gggdtparser/test/si.py
--rw-rw-rw-   0        0        0      158 2023-05-30 07:56:38.000000 gggdtparser-0.0.9/gggdtparser/test/sw.py
--rw-rw-rw-   0        0        0      129 2023-05-30 08:06:27.000000 gggdtparser-0.0.9/gggdtparser/test/tg.py
--rw-rw-rw-   0        0        0      127 2023-05-30 08:03:19.000000 gggdtparser-0.0.9/gggdtparser/test/tr.py
--rw-rw-rw-   0        0        0      178 2023-05-30 07:49:10.000000 gggdtparser-0.0.9/gggdtparser/test/uk.py
--rw-rw-rw-   0        0        0      140 2023-05-30 06:39:37.000000 gggdtparser-0.0.9/gggdtparser/test/ur.py
--rw-rw-rw-   0        0        0      570 2023-05-30 11:54:30.000000 gggdtparser-0.0.9/gggdtparser/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-30 11:55:17.877297 gggdtparser-0.0.9/gggdtparser.egg-info/
--rw-rw-rw-   0        0        0     3404 2023-05-30 11:55:17.000000 gggdtparser-0.0.9/gggdtparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1191 2023-05-30 11:55:17.000000 gggdtparser-0.0.9/gggdtparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 11:55:17.000000 gggdtparser-0.0.9/gggdtparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-30 11:55:17.000000 gggdtparser-0.0.9/gggdtparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      775 2023-05-30 11:55:17.917191 gggdtparser-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      165 2023-03-27 07:16:57.000000 gggdtparser-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:16:00.253761 gggdtparser-0.1.0/
+-rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggdtparser-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3404 2023-06-19 03:16:00.254760 gggdtparser-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2689 2023-04-10 04:20:03.000000 gggdtparser-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 03:16:00.211414 gggdtparser-0.1.0/gggdtparser/
+-rw-rw-rw-   0        0        0      227 2023-05-16 08:44:33.000000 gggdtparser-0.1.0/gggdtparser/__init__.py
+-rw-rw-rw-   0        0        0     3260 2023-06-19 03:06:17.000000 gggdtparser-0.1.0/gggdtparser/dtconfigs.py
+-rw-rw-rw-   0        0        0    17850 2023-06-19 03:07:20.000000 gggdtparser-0.1.0/gggdtparser/dtparser.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:16:00.238182 gggdtparser-0.1.0/gggdtparser/langs/
+-rw-rw-rw-   0        0        0       88 2023-04-20 07:19:51.000000 gggdtparser-0.1.0/gggdtparser/langs/__init__.py
+-rw-rw-rw-   0        0        0      235 2023-06-19 02:32:34.000000 gggdtparser-0.1.0/gggdtparser/langs/_id.py
+-rw-rw-rw-   0        0        0      246 2023-06-19 02:32:40.000000 gggdtparser-0.1.0/gggdtparser/langs/az.py
+-rw-rw-rw-   0        0        0      678 2023-06-19 02:44:22.000000 gggdtparser-0.1.0/gggdtparser/langs/de.py
+-rw-rw-rw-   0        0        0     4773 2023-05-30 07:53:40.000000 gggdtparser-0.1.0/gggdtparser/langs/default.py
+-rw-rw-rw-   0        0        0     3438 2023-06-19 01:52:13.000000 gggdtparser-0.1.0/gggdtparser/langs/en.py
+-rw-rw-rw-   0        0        0      703 2023-05-25 03:05:13.000000 gggdtparser-0.1.0/gggdtparser/langs/es.py
+-rw-rw-rw-   0        0        0      943 2023-05-25 03:05:13.000000 gggdtparser-0.1.0/gggdtparser/langs/fra.py
+-rw-rw-rw-   0        0        0      223 2023-05-30 08:08:07.000000 gggdtparser-0.1.0/gggdtparser/langs/hi.py
+-rw-rw-rw-   0        0        0      239 2023-05-30 06:33:25.000000 gggdtparser-0.1.0/gggdtparser/langs/ky.py
+-rw-rw-rw-   0        0        0      345 2023-05-30 07:58:49.000000 gggdtparser-0.1.0/gggdtparser/langs/mr.py
+-rw-rw-rw-   0        0        0      813 2023-06-19 02:00:07.000000 gggdtparser-0.1.0/gggdtparser/langs/ru.py
+-rw-rw-rw-   0        0        0      249 2023-05-30 07:52:16.000000 gggdtparser-0.1.0/gggdtparser/langs/rw.py
+-rw-rw-rw-   0        0        0      238 2023-05-30 08:00:58.000000 gggdtparser-0.1.0/gggdtparser/langs/si.py
+-rw-rw-rw-   0        0        0      230 2023-05-25 03:05:13.000000 gggdtparser-0.1.0/gggdtparser/langs/so.py
+-rw-rw-rw-   0        0        0      329 2023-05-30 07:55:53.000000 gggdtparser-0.1.0/gggdtparser/langs/sw.py
+-rw-rw-rw-   0        0        0      745 2023-05-25 03:05:13.000000 gggdtparser-0.1.0/gggdtparser/langs/swe.py
+-rw-rw-rw-   0        0        0      195 2023-05-30 08:05:09.000000 gggdtparser-0.1.0/gggdtparser/langs/tg.py
+-rw-rw-rw-   0        0        0      300 2023-05-30 08:05:26.000000 gggdtparser-0.1.0/gggdtparser/langs/tr.py
+-rw-rw-rw-   0        0        0      815 2023-06-19 02:54:06.000000 gggdtparser-0.1.0/gggdtparser/langs/uk.py
+-rw-rw-rw-   0        0        0      231 2023-05-30 06:37:38.000000 gggdtparser-0.1.0/gggdtparser/langs/ur.py
+-rw-rw-rw-   0        0        0      432 2023-05-25 03:05:13.000000 gggdtparser-0.1.0/gggdtparser/langs/vie.py
+-rw-rw-rw-   0        0        0      802 2023-05-25 03:05:13.000000 gggdtparser-0.1.0/gggdtparser/langs/zh.py
+-rw-rw-rw-   0        0        0      609 2023-05-25 03:05:13.000000 gggdtparser-0.1.0/gggdtparser/langs/zht.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:16:00.252781 gggdtparser-0.1.0/gggdtparser/test/
+-rw-rw-rw-   0        0        0    43437 2023-05-25 04:15:16.000000 gggdtparser-0.1.0/gggdtparser/test/__init__.py
+-rw-rw-rw-   0        0        0      112 2023-05-30 07:17:35.000000 gggdtparser-0.1.0/gggdtparser/test/_id.py
+-rw-rw-rw-   0        0        0      829 2023-04-20 08:57:23.000000 gggdtparser-0.1.0/gggdtparser/test/az.py
+-rw-rw-rw-   0        0        0      120 2023-05-30 08:08:48.000000 gggdtparser-0.1.0/gggdtparser/test/hi.py
+-rw-rw-rw-   0        0        0      118 2023-05-30 06:34:41.000000 gggdtparser-0.1.0/gggdtparser/test/ky.py
+-rw-rw-rw-   0        0        0      211 2023-05-30 07:59:04.000000 gggdtparser-0.1.0/gggdtparser/test/mr.py
+-rw-rw-rw-   0        0        0      117 2023-05-30 07:52:38.000000 gggdtparser-0.1.0/gggdtparser/test/ru.py
+-rw-rw-rw-   0        0        0      136 2023-05-30 07:52:38.000000 gggdtparser-0.1.0/gggdtparser/test/rw.py
+-rw-rw-rw-   0        0        0      129 2023-05-30 08:01:52.000000 gggdtparser-0.1.0/gggdtparser/test/si.py
+-rw-rw-rw-   0        0        0      158 2023-05-30 07:56:38.000000 gggdtparser-0.1.0/gggdtparser/test/sw.py
+-rw-rw-rw-   0        0        0      129 2023-05-30 08:06:27.000000 gggdtparser-0.1.0/gggdtparser/test/tg.py
+-rw-rw-rw-   0        0        0      127 2023-05-30 08:03:19.000000 gggdtparser-0.1.0/gggdtparser/test/tr.py
+-rw-rw-rw-   0        0        0      178 2023-05-30 07:49:10.000000 gggdtparser-0.1.0/gggdtparser/test/uk.py
+-rw-rw-rw-   0        0        0      140 2023-05-30 06:39:37.000000 gggdtparser-0.1.0/gggdtparser/test/ur.py
+-rw-rw-rw-   0        0        0      570 2023-05-30 11:54:30.000000 gggdtparser-0.1.0/gggdtparser/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:16:00.215213 gggdtparser-0.1.0/gggdtparser.egg-info/
+-rw-rw-rw-   0        0        0     3404 2023-06-19 03:16:00.000000 gggdtparser-0.1.0/gggdtparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1191 2023-06-19 03:16:00.000000 gggdtparser-0.1.0/gggdtparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 03:16:00.000000 gggdtparser-0.1.0/gggdtparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-19 03:16:00.000000 gggdtparser-0.1.0/gggdtparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      775 2023-06-19 03:16:00.255946 gggdtparser-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-03-27 07:16:57.000000 gggdtparser-0.1.0/setup.py
```

### Comparing `gggdtparser-0.0.9/LICENSE` & `gggdtparser-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.9/PKG-INFO` & `gggdtparser-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gggdtparser
-Version: 0.0.9
+Version: 0.1.0
 Summary: 通用、便捷、准确的字符串时间解析工具
 Home-page: https://github.com/kusen-alpha/gggdtparser
 Author: kusen
 Author-email: hu1194542196@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggdtparser/issues
 Project-URL: Documentation, https://github.com/kusen-alpha/gggdtparser/blob/master/README.md
```

### Comparing `gggdtparser-0.0.9/README.md` & `gggdtparser-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.9/gggdtparser/dtconfigs.py` & `gggdtparser-0.1.0/gggdtparser/dtconfigs.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # author: kusen
 # email: 1194542196@qq.com
 # date: 2023/3/24
 import copy
 import os
 import glob
 import importlib
+import re
+
 from .utils import get_sort_dict
 
 BASE_DIR = os.path.dirname(os.path.abspath(__file__))
 
 LANG_MAPPING = {
     # 英语
     "en": "en",
@@ -66,46 +68,58 @@
     # 印地语
     "hi": "hi",
 }
 
 TRANSLATE_LANGS = [
     # 阿拉伯语
     'ara',
-    'ar'
+    'ar',
+    # 泰语
+    'th'
 ]
 
 _LANG_LIST_SORT = ['default', 'en', 'zh', 'zht', 'de', 'fra', 'swe',
                    'vie', 'ru', 'es', 'so', 'mr', 'az', "uk", 'sw',
                    'tr', 'ky', 'ur', '_id', 'rw', 'si', 'tg', 'hi'
                    ]
 
+
+def compile_regex(regex, flags=0):
+    return re.compile(regex, flags)
+
+
+def compile_regex_list(regex_list, flags=0):
+    return [compile_regex(regex, flags) for regex in regex_list]
+
+
 _LANG_DIR = os.path.join(BASE_DIR, 'langs')
 _LANG_FILES = glob.glob(_LANG_DIR + '/*.py')
 _LANG_FILES = [filename for filename in _LANG_FILES if
                '__init__' not in filename]
 LANG_SUB_TRANSLATE = {}
 LANG_ACCURATE_REGEX_LIST = {}
 LANG_FUZZY_REGEX_LIST = {}
 for lang_file in _LANG_FILES:
     lang = os.path.basename(lang_file).replace('.py', '')
     module_name = 'gggdtparser.langs.' + lang
     module = importlib.import_module(module_name)
     if hasattr(module, 'SUB_TRANSLATE'):
-        LANG_SUB_TRANSLATE[lang] = getattr(module, 'SUB_TRANSLATE')
+        sub_list = []
+        for sub in getattr(module, 'SUB_TRANSLATE'):
+            sub_list.append((compile_regex(sub[0]), sub[1]))
+        LANG_SUB_TRANSLATE[lang] = sub_list
     if hasattr(module, 'ACCURATE_REGEX_LIST'):
-        LANG_ACCURATE_REGEX_LIST[lang] = getattr(
-            module, 'ACCURATE_REGEX_LIST')
+        LANG_ACCURATE_REGEX_LIST[lang] = compile_regex_list(getattr(
+            module, 'ACCURATE_REGEX_LIST'), flags=re.M | re.I | re.S)
     if hasattr(module, 'FUZZY_REGEX_LIST'):
-        LANG_FUZZY_REGEX_LIST[lang] = getattr(
-            module, 'FUZZY_REGEX_LIST')
+        LANG_FUZZY_REGEX_LIST[lang] = compile_regex_list(getattr(
+            module, 'FUZZY_REGEX_LIST'), flags=re.M | re.I | re.S)
 
 LANG_ACCURATE_REGEX_LIST = get_sort_dict(
     LANG_ACCURATE_REGEX_LIST, _LANG_LIST_SORT)
 LANG_FUZZY_REGEX_LIST = get_sort_dict(
     LANG_FUZZY_REGEX_LIST, _LANG_LIST_SORT)
 
 _SUB_LANG_LIST_SORT = copy.deepcopy(_LANG_LIST_SORT)
 (_SUB_LANG_LIST_SORT[0], _SUB_LANG_LIST_SORT[-1]) = (
     _SUB_LANG_LIST_SORT[-1], _SUB_LANG_LIST_SORT[0])
 LANG_SUB_TRANSLATE = get_sort_dict(LANG_SUB_TRANSLATE, _SUB_LANG_LIST_SORT)
-
-
```

### Comparing `gggdtparser-0.0.9/gggdtparser/dtparser.py` & `gggdtparser-0.1.0/gggdtparser/dtparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,20 +22,20 @@
         :return:
         """
         if not langs:
             langs = []
         if not langs:
             for _lang, sub_list in dtconfigs.LANG_SUB_TRANSLATE.items():
                 for sub in sub_list:
-                    string_datetime = re.sub(sub[0], sub[1], string_datetime)
+                    string_datetime = sub[0].sub(sub[1], string_datetime)
         for lang in langs:
             _sub_translate = dtconfigs.LANG_SUB_TRANSLATE.get(
                 lang) or []
             for sub in _sub_translate:
-                string_datetime = re.sub(sub[0], sub[1], string_datetime)
+                string_datetime = sub[0].sub(sub[1], string_datetime)
         return string_datetime
 
 
 class StringDateTimeRegexParser(object):
     # 默认时间顺序
     DEFAULT_DATETIME_SEQ = ['year', 'month', 'day', 'hour', 'minute', 'second']
 
@@ -113,27 +113,25 @@
         return dtconfigs.LANG_FUZZY_REGEX_LIST.get(lang) or []
 
     @classmethod
     def match_and_parse(cls, string_datetime, regex_list,
                         result_accurately, max_datetime, min_datetime):
         for regex in regex_list:
             try:
-                match_obj = re.search(
-                    regex, string_datetime, flags=re.M | re.I | re.S)
+                match_obj = regex.search(string_datetime)
             except (ValueError, re.error) as e:
                 continue
             if not match_obj:
                 continue
             group_dict = match_obj.groupdict()
             if group_dict:
                 try:
                     result = cls._parse_group_dict(
                         group_dict, result_accurately,
                         max_datetime, min_datetime)
-                    # print(regex)
                     return result
                 except Exception:
                     continue
 
     @classmethod
     def _parse_group_dict(cls, group_dict, result_accurately, max_datetime,
                           min_datetime):
```

### Comparing `gggdtparser-0.0.9/gggdtparser/langs/de.py` & `gggdtparser-0.1.0/gggdtparser/langs/de.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.9/gggdtparser/langs/default.py` & `gggdtparser-0.1.0/gggdtparser/langs/default.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.9/gggdtparser/langs/en.py` & `gggdtparser-0.1.0/gggdtparser/langs/en.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,9 +76,10 @@
     (r'Thursday|Thurs\.?|Thur\.?', ''),
     (r'Friday|Fri\.?', ''),
     (r'Saturday|Sat\.?', ''),
     (r'Sunday|Sun\.?', ''),
     (r'AT', ''),
     (r'AM', 'am'),
     (r'PM', 'pm'),
+    (r'yesterday\s*(at)?', '昨天'),
 ]
 FUZZY_REGEX_LIST = []
```

### Comparing `gggdtparser-0.0.9/gggdtparser/langs/es.py` & `gggdtparser-0.1.0/gggdtparser/langs/es.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.9/gggdtparser/langs/fra.py` & `gggdtparser-0.1.0/gggdtparser/langs/fra.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.9/gggdtparser/langs/ru.py` & `gggdtparser-0.1.0/gggdtparser/langs/ru.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 SUB_TRANSLATE = [
     (r"январь", "1月"),
     (r"февраль", "2月"),
     (r"март", "3月"),
     (r"апрель|апреля|апрел", "4月"),
     (r"май", "5月"),
-    (r"июнь", "6月"),
+    (r"июнь|июня", "6月"),
     (r"июль", "7月"),
     (r"август", "8月"),
     (r"сентябрь", "9月"),
     (r"октябрь", "10月"),
     (r"ноябрь", "11月"),
     (r"декабрь", "12月"),
     (r"сегодня  в|сегодня", "今天"),
```

### Comparing `gggdtparser-0.0.9/gggdtparser/langs/swe.py` & `gggdtparser-0.1.0/gggdtparser/langs/swe.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.9/gggdtparser/langs/uk.py` & `gggdtparser-0.1.0/gggdtparser/langs/uk.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,12 +23,12 @@
     (r"Жовтень", "10月"),
     (r"Листопад", "11月"),
     (r"Грудень", "12月"),
 
 ]
 
 FUZZY_REGEX_LIST = [
-    r"(?P<bH>\d+)\s*годин\(и\) тому"
-    r"(?P<bH>\d+)\s*години\) тому"
-    r"(?P<bM>\d+)\s*хвилин\(и\) тому"
-    r"(?P<bM>\d+)\s*хвилини\) тому"
+    r"(?P<bH>\d+)\s*годин\(и\) тому",
+    r"(?P<bH>\d+)\s*години\) тому",
+    r"(?P<bM>\d+)\s*хвилин\(и\) тому",
+    r"(?P<bM>\d+)\s*хвилини\) тому",
 ]
```

### Comparing `gggdtparser-0.0.9/gggdtparser/langs/zh.py` & `gggdtparser-0.1.0/gggdtparser/langs/zh.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.9/gggdtparser/langs/zht.py` & `gggdtparser-0.1.0/gggdtparser/langs/zht.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.9/gggdtparser/test/__init__.py` & `gggdtparser-0.1.0/gggdtparser/test/__init__.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.9/gggdtparser/test/az.py` & `gggdtparser-0.1.0/gggdtparser/test/az.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.9/gggdtparser/utils.py` & `gggdtparser-0.1.0/gggdtparser/utils.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.9/gggdtparser.egg-info/PKG-INFO` & `gggdtparser-0.1.0/gggdtparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gggdtparser
-Version: 0.0.9
+Version: 0.1.0
 Summary: 通用、便捷、准确的字符串时间解析工具
 Home-page: https://github.com/kusen-alpha/gggdtparser
 Author: kusen
 Author-email: hu1194542196@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggdtparser/issues
 Project-URL: Documentation, https://github.com/kusen-alpha/gggdtparser/blob/master/README.md
```

### Comparing `gggdtparser-0.0.9/gggdtparser.egg-info/SOURCES.txt` & `gggdtparser-0.1.0/gggdtparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.9/setup.cfg` & `gggdtparser-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6767 6474 7061 7273 6572 0d0a   = gggdtparser..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 390d  version = 0.0.9.
+00000020: 7665 7273 696f 6e20 3d20 302e 312e 300d  version = 0.1.0.
 00000030: 0a61 7574 686f 7220 3d20 6b75 7365 6e0d  .author = kusen.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6875 3131 3934 3534 3231 3936 4071 712e  hu1194542196@qq.
 00000060: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000070: 203d 20cd a8d3 c3a1 a2b1 e3bd dda1 a2d7   = .............
 00000080: bcc8 b7b5 c4d7 d6b7 fbb4 aeca b1bc e4bd  ................
 00000090: e2ce f6b9 a4be df0d 0a6c 6f6e 675f 6465  .........long_de
```

