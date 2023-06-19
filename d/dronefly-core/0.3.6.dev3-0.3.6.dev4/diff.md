# Comparing `tmp/dronefly_core-0.3.6.dev3.tar.gz` & `tmp/dronefly_core-0.3.6.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronefly_core-0.3.6.dev3.tar", max compression
+gzip compressed data, was "dronefly_core-0.3.6.dev4.tar", max compression
```

## Comparing `dronefly_core-0.3.6.dev3.tar` & `dronefly_core-0.3.6.dev4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.6.dev3/LICENSE
--rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.6.dev3/README.md
--rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.6.dev3/dronefly/core/__init__.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev3/dronefly/core/clients/__init__.py
--rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.6.dev3/dronefly/core/clients/inat.py
--rw-r--r--   0        0        0     7991 2023-06-18 15:08:05.888074 dronefly_core-0.3.6.dev3/dronefly/core/commands/__init__.py
--rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.6.dev3/dronefly/core/constants.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev3/dronefly/core/formatters/__init__.py
--rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.6.dev3/dronefly/core/formatters/constants.py
--rw-r--r--   0        0        0    34585 2023-06-18 15:07:29.087299 dronefly_core-0.3.6.dev3/dronefly/core/formatters/generic.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.6.dev3/dronefly/core/models/__init__.py
--rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.6.dev3/dronefly/core/models/controlled_terms.py
--rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.6.dev3/dronefly/core/models/user.py
--rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.6.dev3/dronefly/core/parsers/__init__.py
--rw-r--r--   0        0        0     3721 2023-06-14 15:48:19.092273 dronefly_core-0.3.6.dev3/dronefly/core/parsers/constants.py
--rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.6.dev3/dronefly/core/parsers/natural.py
--rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.6.dev3/dronefly/core/parsers/unixlike.py
--rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.6.dev3/dronefly/core/parsers/url.py
--rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.6.dev3/dronefly/core/query/__init__.py
--rw-r--r--   0        0        0    21941 2023-06-18 15:05:34.396886 dronefly_core-0.3.6.dev3/dronefly/core/query/query.py
--rw-r--r--   0        0        0     1366 2023-06-18 14:57:16.774410 dronefly_core-0.3.6.dev3/dronefly/core/utils/__init__.py
--rw-r--r--   0        0        0      741 2023-06-19 11:01:37.055511 dronefly_core-0.3.6.dev3/pyproject.toml
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev3/setup.py
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev3/PKG-INFO
+-rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.6.dev4/LICENSE
+-rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.6.dev4/README.md
+-rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.6.dev4/dronefly/core/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev4/dronefly/core/clients/__init__.py
+-rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.6.dev4/dronefly/core/clients/inat.py
+-rw-r--r--   0        0        0     7991 2023-06-18 15:08:05.888074 dronefly_core-0.3.6.dev4/dronefly/core/commands/__init__.py
+-rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.6.dev4/dronefly/core/constants.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev4/dronefly/core/formatters/__init__.py
+-rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.6.dev4/dronefly/core/formatters/constants.py
+-rw-r--r--   0        0        0    34585 2023-06-18 15:07:29.087299 dronefly_core-0.3.6.dev4/dronefly/core/formatters/generic.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.6.dev4/dronefly/core/models/__init__.py
+-rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.6.dev4/dronefly/core/models/controlled_terms.py
+-rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.6.dev4/dronefly/core/models/user.py
+-rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.6.dev4/dronefly/core/parsers/__init__.py
+-rw-r--r--   0        0        0     3721 2023-06-14 15:48:19.092273 dronefly_core-0.3.6.dev4/dronefly/core/parsers/constants.py
+-rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.6.dev4/dronefly/core/parsers/natural.py
+-rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.6.dev4/dronefly/core/parsers/unixlike.py
+-rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.6.dev4/dronefly/core/parsers/url.py
+-rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.6.dev4/dronefly/core/query/__init__.py
+-rw-r--r--   0        0        0    21941 2023-06-18 15:05:34.396886 dronefly_core-0.3.6.dev4/dronefly/core/query/query.py
+-rw-r--r--   0        0        0     1366 2023-06-18 14:57:16.774410 dronefly_core-0.3.6.dev4/dronefly/core/utils/__init__.py
+-rw-r--r--   0        0        0      741 2023-06-19 16:29:59.863532 dronefly_core-0.3.6.dev4/pyproject.toml
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev4/setup.py
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev4/PKG-INFO
```

### Comparing `dronefly_core-0.3.6.dev3/LICENSE` & `dronefly_core-0.3.6.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev3/README.md` & `dronefly_core-0.3.6.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev3/dronefly/core/clients/inat.py` & `dronefly_core-0.3.6.dev4/dronefly/core/clients/inat.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev3/dronefly/core/commands/__init__.py` & `dronefly_core-0.3.6.dev4/dronefly/core/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev3/dronefly/core/constants.py` & `dronefly_core-0.3.6.dev4/dronefly/core/constants.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev3/dronefly/core/formatters/generic.py` & `dronefly_core-0.3.6.dev4/dronefly/core/formatters/generic.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev3/dronefly/core/models/controlled_terms.py` & `dronefly_core-0.3.6.dev4/dronefly/core/models/controlled_terms.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev3/dronefly/core/parsers/constants.py` & `dronefly_core-0.3.6.dev4/dronefly/core/parsers/constants.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev3/dronefly/core/parsers/natural.py` & `dronefly_core-0.3.6.dev4/dronefly/core/parsers/natural.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev3/dronefly/core/parsers/unixlike.py` & `dronefly_core-0.3.6.dev4/dronefly/core/parsers/unixlike.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev3/dronefly/core/parsers/url.py` & `dronefly_core-0.3.6.dev4/dronefly/core/parsers/url.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev3/dronefly/core/query/query.py` & `dronefly_core-0.3.6.dev4/dronefly/core/query/query.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev3/dronefly/core/utils/__init__.py` & `dronefly_core-0.3.6.dev4/dronefly/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev3/setup.py` & `dronefly_core-0.3.6.dev4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'html2markdown>=0.1.7,<0.2.0',
  'inflect>=5.3.0,<6.0.0',
  'pyinaturalist>=0.19.0.dev2,<0.20',
  'rich>=10.9,<14']
 
 setup_kwargs = {
     'name': 'dronefly-core',
-    'version': '0.3.6.dev3',
+    'version': '0.3.6.dev4',
     'description': 'Core dronefly components',
     'long_description': "# Dronefly core\n\nThis is an incomplete rewrite of [Dronefly](https://dronefly.readthedocs.io)\nDiscord bot's core components. We're not yet making version guarantees until\nit is more usable.\n\n# Related packages\n\n## Dronefly command-line client\n\nThe [dronefly-cli](https://github.com/dronefly-garden/dronefly-cli) command-line\nclient will provide a standalone text user interface that can perform a usable\nsubset of Dronefly Discord bot's capabilities, built solely with Dronefly core.\n\n## Dronefly Discord bot\n\nDronefly Discord bot brings [iNaturalist](https://www.inaturalist.org) taxa,\nobservations, and other data from the site into conversations on the\n[Discord](https://discord.com) chat platform.\n",
     'author': 'Ben Armstrong',
     'author_email': 'synrg@debian.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dronefly_core-0.3.6.dev3/PKG-INFO` & `dronefly_core-0.3.6.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dronefly-core
-Version: 0.3.6.dev3
+Version: 0.3.6.dev4
 Summary: Core dronefly components
 License: AGPL-3.0-or-later
 Author: Ben Armstrong
 Author-email: synrg@debian.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

