# Comparing `tmp/micawber-0.5.4.tar.gz` & `tmp/micawber-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micawber-0.5.4.tar", last modified: Mon Jul 12 14:05:33 2021, max compression
+gzip compressed data, was "dist/micawber-0.5.5.tar", last modified: Mon Jun 19 13:23:05 2023, max compression
```

## Comparing `micawber-0.5.4.tar` & `micawber-0.5.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2021-07-12 14:05:33.000000 micawber-0.5.4/
--rw-rw-r--   0 charles   (1000) charles   (1000)     1058 2018-08-16 18:40:47.000000 micawber-0.5.4/LICENSE
--rw-rw-r--   0 charles   (1000) charles   (1000)      131 2018-08-16 18:40:47.000000 micawber-0.5.4/MANIFEST.in
--rw-r--r--   0 charles   (1000) charles   (1000)     3248 2021-07-12 14:05:33.000000 micawber-0.5.4/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)     2037 2019-06-30 16:32:37.000000 micawber-0.5.4/README.rst
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2021-07-12 14:05:33.000000 micawber-0.5.4/micawber/
--rw-rw-r--   0 charles   (1000) charles   (1000)      687 2021-07-12 14:05:11.000000 micawber-0.5.4/micawber/__init__.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     1532 2021-06-09 13:01:14.000000 micawber-0.5.4/micawber/cache.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     9664 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/compat.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2021-07-12 14:05:33.000000 micawber-0.5.4/micawber/contrib/
--rw-rw-r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/contrib/__init__.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2021-07-12 14:05:33.000000 micawber-0.5.4/micawber/contrib/mcdjango/
--rw-rw-r--   0 charles   (1000) charles   (1000)     3090 2021-02-01 16:25:55.000000 micawber-0.5.4/micawber/contrib/mcdjango/__init__.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2021-07-12 14:05:33.000000 micawber-0.5.4/micawber/contrib/mcdjango/mcdjango_tests/
--rw-rw-r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/contrib/mcdjango/mcdjango_tests/__init__.py
--rw-rw-r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/contrib/mcdjango/mcdjango_tests/models.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     4929 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/contrib/mcdjango/mcdjango_tests/tests.py
--rw-rw-r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/contrib/mcdjango/models.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      425 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/contrib/mcdjango/providers.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2021-07-12 14:05:33.000000 micawber-0.5.4/micawber/contrib/mcdjango/templates/
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2021-07-12 14:05:33.000000 micawber-0.5.4/micawber/contrib/mcdjango/templates/micawber/
--rw-rw-r--   0 charles   (1000) charles   (1000)       83 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/contrib/mcdjango/templates/micawber/link.html
--rw-rw-r--   0 charles   (1000) charles   (1000)      122 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/contrib/mcdjango/templates/micawber/photo.html
--rw-rw-r--   0 charles   (1000) charles   (1000)       25 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/contrib/mcdjango/templates/micawber/rich.html
--rw-rw-r--   0 charles   (1000) charles   (1000)       25 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/contrib/mcdjango/templates/micawber/video.html
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2021-07-12 14:05:33.000000 micawber-0.5.4/micawber/contrib/mcdjango/templatetags/
--rw-rw-r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/contrib/mcdjango/templatetags/__init__.py
--rw-rw-r--   0 charles   (1000) charles   (1000)       47 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/contrib/mcdjango/templatetags/micawber_tags.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      837 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/contrib/mcflask.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     1715 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/contrib/providers.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      168 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/exceptions.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     6742 2020-11-08 02:22:26.000000 micawber-0.5.4/micawber/parsers.py
--rw-r--r--   0 charles   (1000) charles   (1000)    11896 2021-06-11 13:01:58.000000 micawber-0.5.4/micawber/providers.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     4033 2018-08-16 18:40:47.000000 micawber-0.5.4/micawber/test_utils.py
--rw-rw-r--   0 charles   (1000) charles   (1000)    14965 2020-11-08 02:22:26.000000 micawber-0.5.4/micawber/tests.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2021-07-12 14:05:33.000000 micawber-0.5.4/micawber.egg-info/
--rw-rw-r--   0 charles   (1000) charles   (1000)     3248 2021-07-12 14:05:33.000000 micawber-0.5.4/micawber.egg-info/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)     1026 2021-07-12 14:05:33.000000 micawber-0.5.4/micawber.egg-info/SOURCES.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        1 2021-07-12 14:05:33.000000 micawber-0.5.4/micawber.egg-info/dependency_links.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        9 2021-07-12 14:05:33.000000 micawber-0.5.4/micawber.egg-info/top_level.txt
--rwxrwxr-x   0 charles   (1000) charles   (1000)     2383 2018-08-16 18:40:47.000000 micawber-0.5.4/runtests.py
--rw-r--r--   0 charles   (1000) charles   (1000)       38 2021-07-12 14:05:33.000000 micawber-0.5.4/setup.cfg
--rw-rw-r--   0 charles   (1000) charles   (1000)     1164 2021-07-12 14:05:03.000000 micawber-0.5.4/setup.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-19 13:23:05.000000 micawber-0.5.5/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1058 2018-08-16 18:40:47.000000 micawber-0.5.5/LICENSE
+-rw-rw-r--   0 charles   (1000) charles   (1000)      131 2018-08-16 18:40:47.000000 micawber-0.5.5/MANIFEST.in
+-rw-r--r--   0 charles   (1000) charles   (1000)     3650 2023-06-19 13:23:05.000000 micawber-0.5.5/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)     2037 2019-06-30 16:32:37.000000 micawber-0.5.5/README.rst
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-19 13:23:05.000000 micawber-0.5.5/micawber/
+-rw-rw-r--   0 charles   (1000) charles   (1000)      687 2021-07-12 14:05:11.000000 micawber-0.5.5/micawber/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1539 2023-06-19 13:20:37.000000 micawber-0.5.5/micawber/cache.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     9664 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/compat.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-19 13:23:05.000000 micawber-0.5.5/micawber/contrib/
+-rw-rw-r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/contrib/__init__.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-19 13:23:05.000000 micawber-0.5.5/micawber/contrib/mcdjango/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3090 2021-02-01 16:25:55.000000 micawber-0.5.5/micawber/contrib/mcdjango/__init__.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-19 13:23:05.000000 micawber-0.5.5/micawber/contrib/mcdjango/mcdjango_tests/
+-rw-rw-r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/contrib/mcdjango/mcdjango_tests/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/contrib/mcdjango/mcdjango_tests/models.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     4929 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/contrib/mcdjango/mcdjango_tests/tests.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/contrib/mcdjango/models.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      425 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/contrib/mcdjango/providers.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-19 13:23:05.000000 micawber-0.5.5/micawber/contrib/mcdjango/templates/
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-19 13:23:05.000000 micawber-0.5.5/micawber/contrib/mcdjango/templates/micawber/
+-rw-rw-r--   0 charles   (1000) charles   (1000)       83 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/contrib/mcdjango/templates/micawber/link.html
+-rw-rw-r--   0 charles   (1000) charles   (1000)      122 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/contrib/mcdjango/templates/micawber/photo.html
+-rw-rw-r--   0 charles   (1000) charles   (1000)       25 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/contrib/mcdjango/templates/micawber/rich.html
+-rw-rw-r--   0 charles   (1000) charles   (1000)       25 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/contrib/mcdjango/templates/micawber/video.html
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-19 13:23:05.000000 micawber-0.5.5/micawber/contrib/mcdjango/templatetags/
+-rw-rw-r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/contrib/mcdjango/templatetags/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)       47 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/contrib/mcdjango/templatetags/micawber_tags.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      837 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/contrib/mcflask.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1715 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/contrib/providers.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      168 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/exceptions.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     6884 2023-06-13 13:11:57.000000 micawber-0.5.5/micawber/parsers.py
+-rw-r--r--   0 charles   (1000) charles   (1000)    11896 2021-06-11 13:01:58.000000 micawber-0.5.5/micawber/providers.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     4033 2018-08-16 18:40:47.000000 micawber-0.5.5/micawber/test_utils.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    14965 2020-11-08 02:22:26.000000 micawber-0.5.5/micawber/tests.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-19 13:23:05.000000 micawber-0.5.5/micawber.egg-info/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3650 2023-06-19 13:23:05.000000 micawber-0.5.5/micawber.egg-info/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1026 2023-06-19 13:23:05.000000 micawber-0.5.5/micawber.egg-info/SOURCES.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-06-19 13:23:05.000000 micawber-0.5.5/micawber.egg-info/dependency_links.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        9 2023-06-19 13:23:05.000000 micawber-0.5.5/micawber.egg-info/top_level.txt
+-rwxrwxr-x   0 charles   (1000) charles   (1000)     2383 2018-08-16 18:40:47.000000 micawber-0.5.5/runtests.py
+-rw-r--r--   0 charles   (1000) charles   (1000)       38 2023-06-19 13:23:05.000000 micawber-0.5.5/setup.cfg
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1558 2023-06-19 13:22:51.000000 micawber-0.5.5/setup.py
```

### Comparing `micawber-0.5.4/LICENSE` & `micawber-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `micawber-0.5.4/PKG-INFO` & `micawber-0.5.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: micawber
-Version: 0.5.4
+Version: 0.5.5
 Summary: a small library for extracting rich content from urls
 Home-page: http://github.com/coleifer/micawber/
 Author: Charles Leifer
 Author-email: coleifer@gmail.com
 License: UNKNOWN
 Description: .. image:: http://media.charlesleifer.com/blog/photos/micawber-logo-0.png
         
@@ -69,8 +69,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
```

### Comparing `micawber-0.5.4/README.rst` & `micawber-0.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `micawber-0.5.4/micawber/__init__.py` & `micawber-0.5.5/micawber/__init__.py`

 * *Files identical despite different names*

### Comparing `micawber-0.5.4/micawber/cache.py` & `micawber-0.5.5/micawber/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,20 @@
     class RedisCache(Cache):
         """
         :param str namespace: key prefix.
         :param int timeout: expiration timeout in seconds
         """
         def __init__(self, namespace='micawber', timeout=None, **conn):
             self.namespace = namespace
-            self.key_fn = lambda self, k: '%s.%s' % (self.namespace, k)
             self.timeout = timeout
             self.conn = Redis(**conn)
 
+        def key_fn(self, k):
+            return '%s.%s' % (self.namespace, k)
+
         def get(self, k):
             cached = self.conn.get(self.key_fn(k))
             if cached:
                 return pickle.loads(cached)
 
         def set(self, k, v):
             ck, cv = self.key_fn(k), pickle.dumps(v)
```

### Comparing `micawber-0.5.4/micawber/compat.py` & `micawber-0.5.5/micawber/compat.py`

 * *Files identical despite different names*

### Comparing `micawber-0.5.4/micawber/contrib/mcdjango/__init__.py` & `micawber-0.5.5/micawber/contrib/mcdjango/__init__.py`

 * *Files identical despite different names*

### Comparing `micawber-0.5.4/micawber/contrib/mcdjango/mcdjango_tests/tests.py` & `micawber-0.5.5/micawber/contrib/mcdjango/mcdjango_tests/tests.py`

 * *Files identical despite different names*

### Comparing `micawber-0.5.4/micawber/contrib/mcflask.py` & `micawber-0.5.5/micawber/contrib/mcflask.py`

 * *Files identical despite different names*

### Comparing `micawber-0.5.4/micawber/contrib/providers.py` & `micawber-0.5.5/micawber/contrib/providers.py`

 * *Files identical despite different names*

### Comparing `micawber-0.5.4/micawber/parsers.py` & `micawber-0.5.5/micawber/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,22 @@
 
 
 url_pattern = '(https?://[-A-Za-z0-9+&@#/%?=~_()|!:,.;]*[-A-Za-z0-9+&@#/%=~_|])'
 url_re = re.compile(url_pattern)
 standalone_url_re = re.compile('^\s*' + url_pattern + '\s*$')
 
 block_elements = set([
-    'address', 'blockquote', 'center', 'dir', 'div', 'dl', 'fieldset', 'form',
-    'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'isindex', 'menu', 'noframes',
-    'noscript', 'ol', 'p', 'pre', 'table', 'ul', 'dd', 'dt', 'frameset', 'li',
-    'tbody', 'td', 'tfoot', 'th', 'thead', 'tr', 'button', 'del', 'iframe',
-    'ins', 'map', 'object', 'script', '[document]'
+    'address', 'article', 'aside', 'blockquote', 'canvas', 'center', 'dir',
+    'dd', 'div', 'dl', 'dt', 'fieldset', 'figcaption', 'figure', 'footer',
+    'form', 'frameset', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'header', 'hr',
+    'isindex', 'li', 'main', 'menu', 'nav', 'noframes', 'noscript', 'ol', 'p',
+    'pre', 'section', 'table', 'tbody', 'td', 'tfoot', 'th', 'thead', 'tr',
+    'ul',
+    # Additional elements.
+    'button', 'del', 'iframe', 'ins', 'map', 'object', 'script', '[document]',
 ])
 
 skip_elements = set(['a', 'pre', 'code', 'input', 'textarea', 'select'])
 
 
 def full_handler(url, response_data, **params):
     if response_data['type'] == 'link':
```

### Comparing `micawber-0.5.4/micawber/providers.py` & `micawber-0.5.5/micawber/providers.py`

 * *Files identical despite different names*

### Comparing `micawber-0.5.4/micawber/test_utils.py` & `micawber-0.5.5/micawber/test_utils.py`

 * *Files identical despite different names*

### Comparing `micawber-0.5.4/micawber/tests.py` & `micawber-0.5.5/micawber/tests.py`

 * *Files identical despite different names*

### Comparing `micawber-0.5.4/micawber.egg-info/PKG-INFO` & `micawber-0.5.5/micawber.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: micawber
-Version: 0.5.4
+Version: 0.5.5
 Summary: a small library for extracting rich content from urls
 Home-page: http://github.com/coleifer/micawber/
 Author: Charles Leifer
 Author-email: coleifer@gmail.com
 License: UNKNOWN
 Description: .. image:: http://media.charlesleifer.com/blog/photos/micawber-logo-0.png
         
@@ -69,8 +69,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
```

### Comparing `micawber-0.5.4/micawber.egg-info/SOURCES.txt` & `micawber-0.5.5/micawber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micawber-0.5.4/runtests.py` & `micawber-0.5.5/runtests.py`

 * *Files identical despite different names*

