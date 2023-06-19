# Comparing `tmp/mds_pim_memos-6.0.9.tar.gz` & `tmp/mds_pim_memos-6.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_pim_memos-6.0.9.tar", last modified: Mon Jun 19 10:15:25 2023, max compression
+gzip compressed data, was "mds_pim_memos-6.8.9.tar", last modified: Mon Jun 19 10:08:23 2023, max compression
```

## Comparing `mds_pim_memos-6.0.9.tar` & `mds_pim_memos-6.8.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 10:15:25.758625 mds_pim_memos-6.0.9/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1884 2023-06-19 10:15:25.754625 mds_pim_memos-6.0.9/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      535 2023-06-19 10:14:10.000000 mds_pim_memos-6.0.9/README.rst
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      523 2023-06-19 10:10:09.000000 mds_pim_memos-6.0.9/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2019 2023-06-19 10:10:09.000000 mds_pim_memos-6.0.9/category.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2924 2023-02-01 12:00:40.000000 mds_pim_memos-6.0.9/category.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 10:15:25.742625 mds_pim_memos-6.0.9/icon/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7162 2021-12-15 13:46:57.000000 mds_pim_memos-6.0.9/icon/memo-red-pin.svg
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 10:15:25.750625 mds_pim_memos-6.0.9/locale/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3657 2023-02-09 08:28:25.000000 mds_pim_memos-6.0.9/locale/de.po
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3009 2023-02-09 08:28:25.000000 mds_pim_memos-6.0.9/locale/en.po
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 10:15:25.754625 mds_pim_memos-6.0.9/mds_pim_memos.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1884 2023-06-19 10:15:25.000000 mds_pim_memos-6.0.9/mds_pim_memos.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      733 2023-06-19 10:15:25.000000 mds_pim_memos-6.0.9/mds_pim_memos.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 10:15:25.000000 mds_pim_memos-6.0.9/mds_pim_memos.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       69 2023-06-19 10:15:25.000000 mds_pim_memos-6.0.9/mds_pim_memos.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 10:15:25.000000 mds_pim_memos-6.0.9/mds_pim_memos.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       43 2023-06-19 10:15:25.000000 mds_pim_memos-6.0.9/mds_pim_memos.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-06-19 10:15:25.000000 mds_pim_memos-6.0.9/mds_pim_memos.egg-info/top_level.txt
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     7149 2023-06-19 10:11:40.000000 mds_pim_memos-6.0.9/memo.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3183 2023-02-01 12:00:40.000000 mds_pim_memos-6.0.9/memo.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      734 2023-02-01 12:00:40.000000 mds_pim_memos-6.0.9/menu.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      251 2021-12-15 13:46:57.000000 mds_pim_memos-6.0.9/menuicons.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      597 2023-02-01 12:00:40.000000 mds_pim_memos-6.0.9/message.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     5795 2023-06-19 10:10:09.000000 mds_pim_memos-6.0.9/notereport.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1778 2023-02-09 08:28:25.000000 mds_pim_memos-6.0.9/notereport.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 10:15:25.750625 mds_pim_memos-6.0.9/report/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    29662 2023-02-01 12:00:40.000000 mds_pim_memos-6.0.9/report/note.fodt
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     5078 2023-02-09 08:28:25.000000 mds_pim_memos-6.0.9/role_edit.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-06-19 10:15:25.758625 mds_pim_memos-6.0.9/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3722 2023-06-19 10:11:40.000000 mds_pim_memos-6.0.9/setup.py
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 10:15:25.750625 mds_pim_memos-6.0.9/tests/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      515 2023-06-19 10:10:09.000000 mds_pim_memos-6.0.9/tests/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    11141 2023-06-19 10:10:09.000000 mds_pim_memos-6.0.9/tests/test_memos.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      167 2023-06-19 10:14:22.000000 mds_pim_memos-6.0.9/tryton.cfg
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2021-12-15 13:46:57.000000 mds_pim_memos-6.0.9/versiondep.txt
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 10:15:25.754625 mds_pim_memos-6.0.9/view/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      507 2021-12-15 15:32:08.000000 mds_pim_memos-6.0.9/view/category_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      240 2021-12-15 15:32:08.000000 mds_pim_memos-6.0.9/view/category_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      320 2021-12-15 15:32:08.000000 mds_pim_memos-6.0.9/view/category_tree.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      793 2023-02-01 12:00:40.000000 mds_pim_memos-6.0.9/view/memos_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      407 2023-02-09 08:28:24.000000 mds_pim_memos-6.0.9/view/memos_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      551 2023-06-19 10:10:03.000000 mds_pim_memos-6.0.9/view/memos_tree2.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 10:08:23.419564 mds_pim_memos-6.8.9/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1402 2023-06-19 10:08:23.419564 mds_pim_memos-6.8.9/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      282 2023-06-19 10:08:03.000000 mds_pim_memos-6.8.9/README.rst
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      523 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     2006 2023-06-19 09:28:38.000000 mds_pim_memos-6.8.9/category.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2924 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/category.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 10:08:23.415564 mds_pim_memos-6.8.9/icon/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7162 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/icon/memo-red-pin.svg
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 10:08:23.415564 mds_pim_memos-6.8.9/locale/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3657 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/locale/de.po
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3009 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/locale/en.po
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 10:08:23.419564 mds_pim_memos-6.8.9/mds_pim_memos.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1402 2023-06-19 10:08:23.000000 mds_pim_memos-6.8.9/mds_pim_memos.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      733 2023-06-19 10:08:23.000000 mds_pim_memos-6.8.9/mds_pim_memos.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 10:08:23.000000 mds_pim_memos-6.8.9/mds_pim_memos.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       69 2023-06-19 10:08:23.000000 mds_pim_memos-6.8.9/mds_pim_memos.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 10:08:23.000000 mds_pim_memos-6.8.9/mds_pim_memos.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       43 2023-06-19 10:08:23.000000 mds_pim_memos-6.8.9/mds_pim_memos.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-06-19 10:08:23.000000 mds_pim_memos-6.8.9/mds_pim_memos.egg-info/top_level.txt
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     7664 2023-06-19 09:49:17.000000 mds_pim_memos-6.8.9/memo.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3183 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/memo.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      734 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/menu.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      251 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/menuicons.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      597 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/message.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5795 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/notereport.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1778 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/notereport.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 10:08:23.415564 mds_pim_memos-6.8.9/report/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    29662 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/report/note.fodt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5078 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/role_edit.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-06-19 10:08:23.419564 mds_pim_memos-6.8.9/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3647 2023-06-19 09:59:08.000000 mds_pim_memos-6.8.9/setup.py
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 10:08:23.415564 mds_pim_memos-6.8.9/tests/
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      204 2023-06-19 09:32:29.000000 mds_pim_memos-6.8.9/tests/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    11231 2023-06-19 09:32:59.000000 mds_pim_memos-6.8.9/tests/test_memos.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      166 2023-06-19 10:08:03.000000 mds_pim_memos-6.8.9/tryton.cfg
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/versiondep.txt
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 10:08:23.419564 mds_pim_memos-6.8.9/view/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      507 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/view/category_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      240 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/view/category_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      320 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/view/category_tree.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      793 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/view/memos_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      407 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/view/memos_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      551 2023-06-19 09:18:50.000000 mds_pim_memos-6.8.9/view/memos_tree2.xml
```

### Comparing `mds_pim_memos-6.0.9/__init__.py` & `mds_pim_memos-6.8.9/__init__.py`

 * *Files identical despite different names*

### Comparing `mds_pim_memos-6.0.9/category.py` & `mds_pim_memos-6.8.9/category.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class Category(tree(separator=' / '), ModelSQL, ModelView):
     "Categories"
     __name__ = "pim_memos.category"
 
     name = fields.Char('Name', required=True, translate=True)
-    parent = fields.Many2One('pim_memos.category', 'Parent', select=True)
+    parent = fields.Many2One('pim_memos.category', 'Parent')
     childs = fields.One2Many('pim_memos.category', 'parent', string='Children')
 
     @classmethod
     def __setup__(cls):
         super(Category, cls).__setup__()
         cls._order.insert(0, ('name', 'ASC'))
```

### Comparing `mds_pim_memos-6.0.9/category.xml` & `mds_pim_memos-6.8.9/category.xml`

 * *Files identical despite different names*

### Comparing `mds_pim_memos-6.0.9/icon/memo-red-pin.svg` & `mds_pim_memos-6.8.9/icon/memo-red-pin.svg`

 * *Files identical despite different names*

### Comparing `mds_pim_memos-6.0.9/locale/de.po` & `mds_pim_memos-6.8.9/locale/de.po`

 * *Files identical despite different names*

### Comparing `mds_pim_memos-6.0.9/locale/en.po` & `mds_pim_memos-6.8.9/locale/en.po`

 * *Files identical despite different names*

### Comparing `mds_pim_memos-6.0.9/mds_pim_memos.egg-info/SOURCES.txt` & `mds_pim_memos-6.8.9/mds_pim_memos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mds_pim_memos-6.0.9/memo.py` & `mds_pim_memos-6.8.9/memo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # This file is part the pim-memos-module for Tryton from m-ds.de.
 # The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
-from trytond.model import ModelView, ModelSQL, fields, tree
+from trytond.model import ModelView, ModelSQL, fields, tree, Index
 from sql import Null
 from sql.conditionals import Case
 from sql.functions import DateTrunc, Function
 from trytond.transaction import Transaction
 import html2text
 from trytond.exceptions import UserError
 from trytond.i18n import gettext
@@ -32,27 +32,26 @@
 
 
 class PimMemo(tree(separator=' / '), ModelSQL, ModelView):
     "Note"
     __name__ = "pim_memos.note"
 
     name = fields.Char(
-        string='Title', select=True, required=True, help='Title for the note')
+        string='Title', required=True, help='Title for the note')
     memo2 = fields.Text(string='Note', required=True)    # richtext
     memoshort = fields.Function(fields.Text(
         string='Memo', readonly=True),
         'on_change_with_memoshort', searcher='search_memoshort')
     category = fields.Many2One(
         model_name='pim_memos.category', string='Category',
         ondelete='RESTRICT')
-    sequence = fields.Integer(string='Sequence', select=True)
+    sequence = fields.Integer(string='Sequence')
 
     # hierarchy
-    parent = fields.Many2One(
-        model_name='pim_memos.note', string='Parent', select=True)
+    parent = fields.Many2One(model_name='pim_memos.note', string='Parent')
     childs = fields.One2Many(
         model_name='pim_memos.note', field='parent', string='Children')
 
     # info
     datecreated = fields.Function(fields.Date(
         string='created', readonly=True),
         'get_info', searcher='search_datecreated')
@@ -65,14 +64,31 @@
         super(PimMemo, cls).__register__(module_name)
         cls.migrate_name_title(module_name)
 
     @classmethod
     def __setup__(cls):
         super(PimMemo, cls).__setup__()
         cls._order.insert(0, ('sequence', 'ASC'))
+        t = cls.__table__()
+        cls._sql_indexes.update({
+            Index(
+                t,
+                (t.sequence, Index.Range(order='ASC'))),
+            Index(
+                t,
+                (t.memo2, Index.Similarity())),
+            Index(
+                t,
+                (DateTrunc('day', t.create_date), Index.Range()),
+                where=t.create_date != None),
+            Index(
+                t,
+                (DateTrunc('day', t.write_date), Index.Range()),
+                where=t.write_date != None),
+            })
 
     @classmethod
     def migrate_name_title(cls, module_name):
         """ column 'title' --> 'name', memo --> memo2
         """
         table = cls.__table_handler__(module_name)
         cursor = Transaction().connection.cursor()
```

### Comparing `mds_pim_memos-6.0.9/memo.xml` & `mds_pim_memos-6.8.9/memo.xml`

 * *Files identical despite different names*

### Comparing `mds_pim_memos-6.0.9/menu.xml` & `mds_pim_memos-6.8.9/menu.xml`

 * *Files identical despite different names*

### Comparing `mds_pim_memos-6.0.9/message.xml` & `mds_pim_memos-6.8.9/message.xml`

 * *Files identical despite different names*

### Comparing `mds_pim_memos-6.0.9/notereport.py` & `mds_pim_memos-6.8.9/notereport.py`

 * *Files identical despite different names*

### Comparing `mds_pim_memos-6.0.9/notereport.xml` & `mds_pim_memos-6.8.9/notereport.xml`

 * *Files identical despite different names*

### Comparing `mds_pim_memos-6.0.9/report/note.fodt` & `mds_pim_memos-6.8.9/report/note.fodt`

 * *Files identical despite different names*

### Comparing `mds_pim_memos-6.0.9/role_edit.xml` & `mds_pim_memos-6.8.9/role_edit.xml`

 * *Files identical despite different names*

### Comparing `mds_pim_memos-6.0.9/setup.py` & `mds_pim_memos-6.8.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         l2 = i.strip().split(';')
         if len(l2) < 4:
             continue
         modversion[l2[0]] = {'min': l2[1], 'max': l2[2], 'prefix': l2[3]}
 
 # tryton-version
 major_version = 6
-minor_version = 0
+minor_version = 8
 
 requires = ['html2text', 'python-slugify']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res|webdav)(\W|$)', dep):
         if dep in modversion.keys():
             prefix = 'mds'
             if len(modversion[dep]['prefix']) > 0:
@@ -67,33 +67,32 @@
 setup(
     name='%s_%s' % (PREFIX, MODULE),
     version=info.get('version', '0.0.1'),
     description='Tryton module to store memos',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     url='https://www.m-ds.de/',
-    download_url='https://scmdev.m-ds.de/PIM/pim_memos',
-    author='martin data - services',
+    author='m-ds',
     author_email='service@m-ds.de',
     license='GPL-3',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Plugins',
         'Framework :: Tryton',
         'Intended Audience :: Developers',
         'Intended Audience :: Customer Service',
         'Intended Audience :: Information Technology',
         'Topic :: Office/Business',
         'Natural Language :: German',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'License :: OSI Approved :: GNU General Public License (GPL)',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
 
     keywords='tryton notes memo information',
     package_dir={'trytond.modules.%s' % MODULE: '.'},
     packages=[
         'trytond.modules.%s' % MODULE,
         ],
```

### Comparing `mds_pim_memos-6.0.9/tests/test_memos.py` & `mds_pim_memos-6.8.9/tests/test_memos.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,16 @@
             }])
 
         m_lst = PimMemo.search([], order=[('memo2', 'ASC')])
         self.assertEqual(len(m_lst), 2)
 
         self.assertRaisesRegex(
             UserError,
-            'ir.recursion_error',
+            'Recursion error: Record "name 1" with parent "name 1" was ' +
+            'configured as ancestor of itself.',
             PimMemo.write,
             *[
                 [m_lst[0]],
                 {
                     'childs': [('add', [m_lst[0].id])],
                 },
             ])
```

### Comparing `mds_pim_memos-6.0.9/view/memos_form.xml` & `mds_pim_memos-6.8.9/view/memos_form.xml`

 * *Files identical despite different names*

### Comparing `mds_pim_memos-6.0.9/view/memos_tree2.xml` & `mds_pim_memos-6.8.9/view/memos_tree2.xml`

 * *Files identical despite different names*

