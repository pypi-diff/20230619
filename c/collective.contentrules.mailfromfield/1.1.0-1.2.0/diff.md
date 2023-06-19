# Comparing `tmp/collective.contentrules.mailfromfield-1.1.0.tar.gz` & `tmp/collective.contentrules.mailfromfield-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.contentrules.mailfromfield-1.1.0.tar", last modified: Fri Mar  3 10:26:11 2023, max compression
+gzip compressed data, was "collective.contentrules.mailfromfield-1.2.0.tar", last modified: Mon Jun 19 12:49:40 2023, max compression
```

## Comparing `collective.contentrules.mailfromfield-1.1.0.tar` & `collective.contentrules.mailfromfield-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-03 10:26:11.543674 collective.contentrules.mailfromfield-1.1.0/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       93 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/MANIFEST.in
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9120 2023-03-03 10:26:11.543674 collective.contentrules.mailfromfield-1.1.0/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6543 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/README.rst
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-03 10:26:11.535673 collective.contentrules.mailfromfield-1.1.0/collective/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-03 10:26:11.539673 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-03 10:26:11.539673 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      322 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-03 10:26:11.539673 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/actions/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/actions/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1240 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/actions/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9888 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/actions/mail.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      507 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-03 10:26:11.539673 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/locales/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2575 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/locales/collective.contentrules.mailfromfield.pot
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-03 10:26:11.535673 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/locales/it/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-03 10:26:11.539673 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3752 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/collective.contentrules.mailfromfield.po
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      929 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/plone.po
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      744 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/locales/plone-manual.pot
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      745 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/locales/plone.pot
--rwxrwxr-x   0 mauro     (1000) mauro     (1000)      335 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/locales/rebuildAll.sh
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1030 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/testing.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-03 10:26:11.539673 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/tests/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/tests/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    11070 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/tests/test_actions_mailfromfield.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      963 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/vocabularies.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-03 10:26:11.539673 collective.contentrules.mailfromfield-1.1.0/collective.contentrules.mailfromfield.egg-info/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9120 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective.contentrules.mailfromfield.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1614 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective.contentrules.mailfromfield.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective.contentrules.mailfromfield.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       40 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective.contentrules.mailfromfield.egg-info/entry_points.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       35 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective.contentrules.mailfromfield.egg-info/namespace_packages.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective.contentrules.mailfromfield.egg-info/not-zip-safe
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       63 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective.contentrules.mailfromfield.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       11 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/collective.contentrules.mailfromfield.egg-info/top_level.txt
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-03 10:26:11.539673 collective.contentrules.mailfromfield-1.1.0/docs/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1260 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/docs/HISTORY.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1439 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/docs/INSTALL.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    17987 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/docs/LICENSE.GPL
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      773 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/docs/LICENSE.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      518 2023-03-03 10:26:11.543674 collective.contentrules.mailfromfield-1.1.0/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2140 2023-03-03 10:26:11.000000 collective.contentrules.mailfromfield-1.1.0/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.757548 collective.contentrules.mailfromfield-1.2.0/
+-rw-r--r--   0 cekk       (501) staff       (20)      225 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)    11265 2023-06-19 12:49:40.757773 collective.contentrules.mailfromfield-1.2.0/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     6547 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/README.rst
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.748477 collective.contentrules.mailfromfield-1.2.0/collective/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.751164 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.752343 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/
+-rw-r--r--   0 cekk       (501) staff       (20)      322 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.753143 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/actions/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/actions/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1240 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/actions/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)    10004 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/actions/mail.py
+-rw-r--r--   0 cekk       (501) staff       (20)      507 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.754326 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)     2575 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/collective.contentrules.mailfromfield.pot
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.746713 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.755548 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     2572 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/collective.contentrules.mailfromfield.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     3752 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/collective.contentrules.mailfromfield.po
+-rw-r--r--   0 cekk       (501) staff       (20)      783 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/plone.mo
+-rw-r--r--   0 cekk       (501) staff       (20)      929 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/plone.po
+-rw-r--r--   0 cekk       (501) staff       (20)      744 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/plone-manual.pot
+-rw-r--r--   0 cekk       (501) staff       (20)      745 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/plone.pot
+-rwxr-xr-x   0 cekk       (501) staff       (20)      335 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/rebuildAll.sh
+-rw-r--r--   0 cekk       (501) staff       (20)     1030 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.756080 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)    10943 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/tests/test_actions_mailfromfield.py
+-rw-r--r--   0 cekk       (501) staff       (20)      963 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/vocabularies.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.750878 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)    11265 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     1786 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       59 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       35 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)       63 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       11 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.757290 collective.contentrules.mailfromfield-1.2.0/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     1375 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/docs/HISTORY.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     1439 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/docs/INSTALL.txt
+-rw-r--r--   0 cekk       (501) staff       (20)    17987 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/docs/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      773 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/docs/LICENSE.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      518 2023-06-19 12:49:40.758457 collective.contentrules.mailfromfield-1.2.0/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2140 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/setup.py
```

### Comparing `collective.contentrules.mailfromfield-1.1.0/PKG-INFO` & `collective.contentrules.mailfromfield-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,268 @@
 Metadata-Version: 2.1
 Name: collective.contentrules.mailfromfield
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Plone content rule for send e-mail to addresses taken from the content
+Home-page: UNKNOWN
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.contentrules.mailfromfield
 Project-URL: Source, https://github.com/RedTurtle/collective.contentrules.mailfromfield
 Project-URL: Tracker, https://github.com/RedTurtle/collective.contentrules.mailfromfield/issues
+Description: 
+        .. image:: https://img.shields.io/pypi/v/collective.contentrules.mailfromfield.svg
+            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+            :alt: Latest Version
+        
+        .. image:: https://img.shields.io/pypi/pyversions/collective.contentrules.mailfromfield.svg?style=plastic
+            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+            :alt: Supported - Python Versions
+        
+        .. image:: https://img.shields.io/pypi/dm/collective.contentrules.mailfromfield.svg
+            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+            :alt: Number of PyPI downloads
+        
+        .. image:: https://img.shields.io/pypi/l/collective.contentrules.mailfromfield.svg
+            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+            :alt: License
+        
+        .. image:: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions/workflows/tests.yml/badge.svg
+            :target: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions
+            :alt: Tests
+            
+        .. image:: https://coveralls.io/repos/github/RedTurtle/collective.contentrules.mailfromfield/badge.svg?branch=master
+            :target: https://coveralls.io/github/RedTurtle/collective.contentrules.mailfromfield?branch=master
+            :alt: Coverage
+        
+        .. contents::
+        
+        Introduction
+        ============
+        
+        This product will add to Plone a new content rules, someway similar to the default "*Send an email*" ones.
+        The difference is that the email recipient is taken dinamically from a site content, not from a
+        static list of values.
+        
+        In this way the same rule, applied in different places in the site, can send the message to different users.
+        
+        How to use
+        ==========
+        
+        The rules can be enabled globally and locally like every one else, as default Plone feature.
+        In the rule configuration panel you need to fill a set of information:
+        
+        ``Subject``
+            The e-mail subject. You can place inside this text some markers (see below).
+        ``Sender email``
+            The sender of the e-mail. You can leave this empty and automatically use the one from the
+            general mail settings.
+        ``Source field``
+            You must put there the name of the attribute from which you want to retrieve the recipient
+            e-mail. See next section.
+        ``Target element``
+            You need to select if the recipient's e-mail must be taken from:
+        
+            * the container where the rules is activated on
+            * the content who notified the event that started the rule execution
+            * the parent of that content
+        
+            See below for details.
+        ``Mail message``
+            The body text of the e-mail that will be sent. The text is the same for all section where
+            the rule is activated on.
+        
+            You can place inside this text some markers (see below).
+        
+        How it take the email data
+        --------------------------
+        
+        First of all you must choose the *Target element*.
+        
+        If you choose to keep default "*From rule's container*" option address will be read from the section you have
+        activated the rule on.
+        
+        *Example*: if you activated the rule on folder ``/site/section`` and the rule will raise event when
+        working on a document ``/site/section/folder/foo`` the email address will be taken
+        from the folder.
+        
+        Changing to "*From content that triggered the event*" will change the behavior, trying to get email data
+        from the content that raised the event.
+        
+        *Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
+        working on a document ``/site/section/folder/foo`` the email address will be taken
+        from the ``foo`` document.
+        
+        Finally, if you choose "*From content's parent*", adresses will the taken from the container of the content
+        that triggered the event.
+        
+        *Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
+        working on a document ``/site/section/folder/foo`` the email address will be taken
+        from ``folder``.
+        
+        What it try to read
+        -------------------
+        
+        The rule try to get from the object:
+        
+        * an attribute of the given name
+        * a callable method from the given name
+        * an Archetypes field with given id
+        * a ZMI property with given id
+        
+        The rule try to read, one after one, all this data. The first match found will be the one used;
+        if not one give results, no e-mail is sent at all.
+        
+        Message interpolation
+        ---------------------
+        
+        Marker labels that follow can be used in the message text and subject.
+        
+        ``${title}``
+            The title of the content that triggered the event (``foo`` title in our example)
+        ``${url}``
+            The URL of the content that triggered the event (``foo`` URL in our example)
+        ``${section_name}``
+            The title of the folder where the rule is activated on (``section`` title in our example)
+        ``${section_url}``
+            The URL of the folder where the rule is activated on (``section`` URL in our example)
+        
+        A real Plone use case
+        ---------------------
+        
+        A Plone site use `Signup Sheet`__ for manage internal training session. The form fieldset is
+        customized as normal, but one of the field is ``director_email``.
+        
+        __ http://plone.org/products/signupsheet
+        
+        We want that this e-mail address is notified when a user subscribe and the user
+        itself put there the e-mail address of the proper director.
+        
+        To reach this we need to:
+        
+        * create a new rule triggered on "*Object added to this container*"
+        * add a filter condition based on content type *Registrant*
+        * add an action using the "*Send email to address taken from the content*"
+        * specify in the action the SignupSheet field with the director email
+        * specify in the action that we want to take the email from the target content
+          (the Registrant itself)
+        
+        TODO
+        ====
+        
+        * why don't support also looking in annotations?
+        * right now the rules check all mail source until one is found with a defined order;
+          maybe is better to leave this choice to the configuration
+        * Dexterity support (probably already there, but needs to be tested)
+        
+        Requirements
+        ============
+        
+        This product has been tested on:
+        
+        * Plone 4.2 with 0.4 version
+        * Plone 4.3 with 0.4 version
+        * Plone 5.0
+        * Plone 5.1
+        
+        Credits
+        =======
+        
+        Developed with the support of `S. Anna Hospital, Ferrara`__; S. Anna Hospital supports the
+        `PloneGov initiative`__.
+        
+        .. image:: http://www.ospfe.it/ospfe-logo.jpg
+           :alt: OspFE logo
+        
+        __ http://www.ospfe.it/
+        __ http://www.plonegov.it/
+        
+        This product was largely developed looking at the source of `collective.contentrules.mailtogroup`__.
+        
+        __ http://plone.org/products/collective.contentrules.mailtogroup
+        
+        Authors
+        =======
+        
+        This product was developed by RedTurtle Technology team.
+        
+        .. image:: http://www.redturtle.it/redturtle_banner.png
+           :alt: RedTurtle Technology Site
+           :target: http://www.redturtle.it/
+        
+        
+        Changelog
+        =========
+        
+        1.2.0 (2023-06-19)
+        ------------------
+        
+        - Change mail send method and allow to eventually add attachments.
+          [cekk]
+        
+        1.1.0 (2023-06-19)
+        ------------------
+        
+        - Plone 6 support
+          [foxtrot-dfm1]
+        
+        1.0.1 (2021-03-10)
+        ------------------
+        
+        - Allow to get to the end of the action execution if no mail is provided.
+          You don't want the page to break if the email is missing. 
+          For the anonymous user this wold be a bad UX
+          [lucabel]
+        
+        
+        1.0.0 (2020-11-23)
+        ------------------
+        
+        - Migrate code to Plone 5/python 3.
+          [lucabel]
+        - Add support for plone.stringinterp.
+          [cekk]
+        
+        0.4.0 (2015-03-13)
+        ------------------
+        
+        Dropped Plone 3 compatibility
+        
+        - Fixed some label that were not i18n compatible
+          [keul]
+        - Fixed wrong documentation mess introduced on version 0.3:
+          the new "parent" option was wrongly descripted
+          [keul]
+        - Updated documentation to reflect changes done in version 0.3
+          [keul]
+        
+        0.3.0 (2014-05-06)
+        ------------------
+        
+        - Fix unicode error while replacing strings [nicolasenno]
+        - Do not fail if a rule is activated on a non-AT content [keul]
+        - Do not try to send mail to empty string recipients [keul]
+        - Refactoring [alert]
+        - Added parent option in the target vocabulary [alert]
+        
+        0.2.0 (2013-05-02)
+        ------------------
+        
+        * lowered logging level to debug
+          [keul]
+        * fixed ruleAction factory
+          [cekk]
+        
+        0.1.0 (2011-10-21)
+        ------------------
+        
+        * Initial release
+        
 Keywords: plone rules mail plonegov
+Platform: UNKNOWN
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
@@ -21,250 +271,7 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Communications :: Email
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Provides-Extra: test
-
-
-.. image:: https://img.shields.io/pypi/v/collective.contentrules.mailfromfield.svg
-    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-    :alt: Latest Version
-
-.. image:: https://img.shields.io/pypi/pyversions/collective.contentrules.mailfromfield.svg?style=plastic
-    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-    :alt: Supported - Python Versions
-
-.. image:: https://img.shields.io/pypi/dm/collective.contentrules.mailfromfield.svg
-    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-    :alt: Number of PyPI downloads
-
-.. image:: https://img.shields.io/pypi/l/collective.contentrules.mailfromfield.svg
-    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-    :alt: License
-
-.. image:: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions/workflows/tests.yml/badge.svg
-    :target: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions
-    :alt: Tests
-    
-.. image:: https://coveralls.io/repos/github/RedTurtle/collective.contentrules.mailfromfield/badge.svg?branch=main
-    :target: https://coveralls.io/github/RedTurtle/collective.contentrules.mailfromfield?branch=main
-    :alt: Coverage
-
-.. contents::
-
-Introduction
-============
-
-This product will add to Plone a new content rules, someway similar to the default "*Send an email*" ones.
-The difference is that the email recipient is taken dinamically from a site content, not from a
-static list of values.
-
-In this way the same rule, applied in different places in the site, can send the message to different users.
-
-How to use
-==========
-
-The rules can be enabled globally and locally like every one else, as default Plone feature.
-In the rule configuration panel you need to fill a set of information:
-
-``Subject``
-    The e-mail subject. You can place inside this text some markers (see below).
-``Sender email``
-    The sender of the e-mail. You can leave this empty and automatically use the one from the
-    general mail settings.
-``Source field``
-    You must put there the name of the attribute from which you want to retrieve the recipient
-    e-mail. See next section.
-``Target element``
-    You need to select if the recipient's e-mail must be taken from:
-
-    * the container where the rules is activated on
-    * the content who notified the event that started the rule execution
-    * the parent of that content
-
-    See below for details.
-``Mail message``
-    The body text of the e-mail that will be sent. The text is the same for all section where
-    the rule is activated on.
-
-    You can place inside this text some markers (see below).
-
-How it take the email data
---------------------------
-
-First of all you must choose the *Target element*.
-
-If you choose to keep default "*From rule's container*" option address will be read from the section you have
-activated the rule on.
-
-*Example*: if you activated the rule on folder ``/site/section`` and the rule will raise event when
-working on a document ``/site/section/folder/foo`` the email address will be taken
-from the folder.
-
-Changing to "*From content that triggered the event*" will change the behavior, trying to get email data
-from the content that raised the event.
-
-*Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
-working on a document ``/site/section/folder/foo`` the email address will be taken
-from the ``foo`` document.
-
-Finally, if you choose "*From content's parent*", adresses will the taken from the container of the content
-that triggered the event.
-
-*Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
-working on a document ``/site/section/folder/foo`` the email address will be taken
-from ``folder``.
-
-What it try to read
--------------------
-
-The rule try to get from the object:
-
-* an attribute of the given name
-* a callable method from the given name
-* an Archetypes field with given id
-* a ZMI property with given id
-
-The rule try to read, one after one, all this data. The first match found will be the one used;
-if not one give results, no e-mail is sent at all.
-
-Message interpolation
----------------------
-
-Marker labels that follow can be used in the message text and subject.
-
-``${title}``
-    The title of the content that triggered the event (``foo`` title in our example)
-``${url}``
-    The URL of the content that triggered the event (``foo`` URL in our example)
-``${section_name}``
-    The title of the folder where the rule is activated on (``section`` title in our example)
-``${section_url}``
-    The URL of the folder where the rule is activated on (``section`` URL in our example)
-
-A real Plone use case
----------------------
-
-A Plone site use `Signup Sheet`__ for manage internal training session. The form fieldset is
-customized as normal, but one of the field is ``director_email``.
-
-__ http://plone.org/products/signupsheet
-
-We want that this e-mail address is notified when a user subscribe and the user
-itself put there the e-mail address of the proper director.
-
-To reach this we need to:
-
-* create a new rule triggered on "*Object added to this container*"
-* add a filter condition based on content type *Registrant*
-* add an action using the "*Send email to address taken from the content*"
-* specify in the action the SignupSheet field with the director email
-* specify in the action that we want to take the email from the target content
-  (the Registrant itself)
-
-TODO
-====
-
-* why don't support also looking in annotations?
-* right now the rules check all mail source until one is found with a defined order;
-  maybe is better to leave this choice to the configuration
-* Dexterity support (probably already there, but needs to be tested)
-
-Requirements
-============
-
-This product has been tested on:
-
-* Plone 4.2 with 0.4 version
-* Plone 4.3 with 0.4 version
-* Plone 5.0
-* Plone 5.1
-
-Credits
-=======
-
-Developed with the support of `S. Anna Hospital, Ferrara`__; S. Anna Hospital supports the
-`PloneGov initiative`__.
-
-.. image:: http://www.ospfe.it/ospfe-logo.jpg
-   :alt: OspFE logo
-
-__ http://www.ospfe.it/
-__ http://www.plonegov.it/
-
-This product was largely developed looking at the source of `collective.contentrules.mailtogroup`__.
-
-__ http://plone.org/products/collective.contentrules.mailtogroup
-
-Authors
-=======
-
-This product was developed by RedTurtle Technology team.
-
-.. image:: http://www.redturtle.it/redturtle_banner.png
-   :alt: RedTurtle Technology Site
-   :target: http://www.redturtle.it/
-
-
-Changelog
-=========
-
-1.1.0 (2023-03-03)
-------------------
-
-- Plone 6 support
-  [foxtrot-dfm1]
-
-
-1.0.1 (2021-03-10)
-------------------
-
-- Allow to get to the end of the action execution if no mail is provided.
-  You don't want the page to break if the email is missing. 
-  For the anonymous user this wold be a bad UX
-  [lucabel]
-
-
-1.0.0 (2020-11-23)
-------------------
-
-- Migrate code to Plone 5/python 3.
-  [lucabel]
-- Add support for plone.stringinterp.
-  [cekk]
-
-0.4.0 (2015-03-13)
-------------------
-
-Dropped Plone 3 compatibility
-
-- Fixed some label that were not i18n compatible
-  [keul]
-- Fixed wrong documentation mess introduced on version 0.3:
-  the new "parent" option was wrongly descripted
-  [keul]
-- Updated documentation to reflect changes done in version 0.3
-  [keul]
-
-0.3.0 (2014-05-06)
-------------------
-
-- Fix unicode error while replacing strings [nicolasenno]
-- Do not fail if a rule is activated on a non-AT content [keul]
-- Do not try to send mail to empty string recipients [keul]
-- Refactoring [alert]
-- Added parent option in the target vocabulary [alert]
-
-0.2.0 (2013-05-02)
-------------------
-
-* lowered logging level to debug
-  [keul]
-* fixed ruleAction factory
-  [cekk]
-
-0.1.0 (2011-10-21)
-------------------
-
-* Initial release
```

### Comparing `collective.contentrules.mailfromfield-1.1.0/README.rst` & `collective.contentrules.mailfromfield-1.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     :target: https://pypi.org/project/collective.contentrules.mailfromfield/
     :alt: License
 
 .. image:: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions
     :alt: Tests
     
-.. image:: https://coveralls.io/repos/github/RedTurtle/collective.contentrules.mailfromfield/badge.svg?branch=main
-    :target: https://coveralls.io/github/RedTurtle/collective.contentrules.mailfromfield?branch=main
+.. image:: https://coveralls.io/repos/github/RedTurtle/collective.contentrules.mailfromfield/badge.svg?branch=master
+    :target: https://coveralls.io/github/RedTurtle/collective.contentrules.mailfromfield?branch=master
     :alt: Coverage
 
 .. contents::
 
 Introduction
 ============
```

### Comparing `collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/actions/configure.zcml` & `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/actions/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/actions/mail.py` & `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/actions/mail.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from Acquisition import aq_base, aq_inner
 from collective.contentrules.mailfromfield import logger
 from collective.contentrules.mailfromfield import messageFactory as _
+from email.message import EmailMessage
 from OFS.SimpleItem import SimpleItem
 from plone import api
 from plone.app.contentrules.actions.mail import MailAddForm, MailEditForm
 from plone.app.contentrules.browser.formhelper import ContentRuleFormWrapper
 from plone.contentrules.rule.interfaces import IExecutable, IRuleElementData
 from plone.registry.interfaces import IRegistry
 from plone.stringinterp.interfaces import IStringInterpolator
@@ -245,21 +246,14 @@
         mailhost = self.get_mailhost()
         source = self.get_from()
         recipients = self.get_recipients()
 
         obj = self.event.object
 
         interpolator = IStringInterpolator(obj)
-
-        # No way to use self.context (where rule is fired) in interpolator
-        # self.context in interpolator is the obj given
-        # And having  two interpolators is strange, because they
-        # both adapt fully. Unless you can somehow adapt it to
-        # 'firing a rule' event, which isn't available to my knowledge.
-
         subject = self.element.subject
         message = self.element.message
         # Section title/url
         subject = self.expand_markers(subject)
         message = self.expand_markers(message)
         # All other stringinterp
         subject = interpolator(subject).strip()
@@ -267,25 +261,36 @@
 
         email_charset = None
         registry = getUtility(IRegistry)
         record = registry.records.get("plone.email_charset", None)
         if record:
             email_charset = record.value
 
+        msg = EmailMessage()
+        msg.set_content(message, charset=email_charset)
+        msg["Subject"] = subject
+        msg["From"] = source
+        msg["To"] = ""
+
+        self.manage_attachments(msg=msg)
         for email_recipient in recipients:
+            msg.replace_header("To", email_recipient)
+            # we set immediate=True because we need to catch exceptions.
+            # by default (False) exceptions are handled by MailHost and we can't catch them.
+            mailhost.send(msg, charset=email_charset, immediate=True)
+
             logger.debug("sending to: %s" % email_recipient)
-            mailhost.send(
-                message,
-                mto=email_recipient,
-                mfrom=source,
-                subject=subject,
-                charset=email_charset,
-            )
         return True
 
+    def manage_attachments(self, msg):
+        """
+        Customize this when needed
+        """
+        pass
+
 
 class MailFromFieldAddForm(MailAddForm):
     schema = IMailFromFieldAction
     Type = MailFromFieldAction
 
 
 class MailFromFieldAddFormView(ContentRuleFormWrapper):
```

### Comparing `collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/locales/collective.contentrules.mailfromfield.pot` & `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/collective.contentrules.mailfromfield.pot`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/collective.contentrules.mailfromfield.po` & `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/collective.contentrules.mailfromfield.po`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/plone.po` & `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/locales/plone-manual.pot` & `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/plone-manual.pot`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/locales/plone.pot` & `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/testing.py` & `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/testing.py`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/tests/test_actions_mailfromfield.py` & `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/tests/test_actions_mailfromfield.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 
     def testExecuteNoSource(self):
         self.loginAsPortalOwner()
         e = MailFromFieldAction()
         e.message = "Document created !"
         e.fieldName = "foo_attr"
         e.target = "object"
+        e.subject = "Subject"
         self.folder.foo_attr = "member1@dummy.org"
         email_from_address = api.portal.get_registry_record("plone.email_from_address")
         email_from_name = api.portal.get_registry_record("plone.email_from_name")
         api.portal.set_registry_record("plone.email_from_address", "")
         ex = getMultiAdapter((self.folder, e, DummyEvent(self.folder.d1)), IExecutable)
         self.assertRaises(ValueError, ex)
         # if we provide a site mail address this won't fail anymore
@@ -114,135 +115,136 @@
     def testExecuteSimpleByAttribute(self):
         self.loginAsPortalOwner()
         self.folder.foo_attr = "member1@dummy.org"
         e = MailFromFieldAction()
         e.source = "foo@bar.be"
         e.fieldName = "foo_attr"
         e.target = "object"
+        e.subject = "Subject"
         e.message = "Còntènt '${title}' created in ${url} - Section is '${section_name}' (${section_url}) !"
         ex = getMultiAdapter((self.folder, e, DummyEvent(self.folder.d1)), IExecutable)
         ex()
         mailSent = self.mailhost.messages[0]
         self.assertIn(b'Content-Type: text/plain; charset="utf-8"', mailSent)
         self.assertIn(b"To: member1@dummy.org", mailSent)
         self.assertIn(b"From: foo@bar.be", mailSent)
-        self.assertEqual(
-            b"C=C3=B2nt=C3=A8nt 'D=C3=B2cumento' created in http://nohost/plone/f1/d1 - S=\r\n"
-            b"ection is 'C=C3=A0rtella' (http://nohost/plone/f1) !",
-            mailSent.split(b"\r\n\r\n")[1],
+        self.assertIn(
+            b"'D=C3=B2cumento' created in http://nohost/plone/f1/d1 - Sec=\ntion is 'C=C3=A0rtella' (http://nohost/plone/f1) !",
+            mailSent,
         )
 
     def testExecuteTargetByAttribute(self):
         self.loginAsPortalOwner()
         self.folder.d1.foo_attr = "member1@dummy.org"
         e = MailFromFieldAction()
         e.source = "foo@bar.be"
         e.fieldName = "foo_attr"
         e.target = "target"
+        e.subject = "Subject"
         e.message = "Còntènt '${title}' created in ${url} - Section is '${section_name}' (${section_url}) !"
         ex = getMultiAdapter((self.folder, e, DummyEvent(self.folder.d1)), IExecutable)
         ex()
         mailSent = self.mailhost.messages[0]
         self.assertIn(b'Content-Type: text/plain; charset="utf-8"', mailSent)
         self.assertIn(b"To: member1@dummy.org", mailSent)
         self.assertIn(b"From: foo@bar.be", mailSent)
-        self.assertEqual(
-            b"C=C3=B2nt=C3=A8nt 'D=C3=B2cumento' created in http://nohost/plone/f1/d1 - S=\r\n"
-            b"ection is 'C=C3=A0rtella' (http://nohost/plone/f1) !",
-            mailSent.split(b"\r\n\r\n")[1],
+        self.assertIn(
+            b"'D=C3=B2cumento' created in http://nohost/plone/f1/d1 - Sec=\ntion is 'C=C3=A0rtella' (http://nohost/plone/f1) !",
+            mailSent,
         )
 
     def testExecuteSimpleByMethod(self):
         self.loginAsPortalOwner()
         self.folder.setDescription("member1@dummy.org")
         e = MailFromFieldAction()
         e.source = "foo@bar.be"
         e.fieldName = "Description"
         e.target = "object"
+        e.subject = "Subject"
         e.message = "Còntènt '${title}' created in ${url} - Section is '${section_name}' (${section_url}) !"
         ex = getMultiAdapter((self.folder, e, DummyEvent(self.folder.d1)), IExecutable)
         ex()
         mailSent = self.mailhost.messages[0]
         self.assertIn(b'Content-Type: text/plain; charset="utf-8"', mailSent)
         self.assertIn(b"To: member1@dummy.org", mailSent)
         self.assertIn(b"From: foo@bar.be", mailSent)
-        self.assertEqual(
-            b"C=C3=B2nt=C3=A8nt 'D=C3=B2cumento' created in http://nohost/plone/f1/d1 - S=\r\n"
-            b"ection is 'C=C3=A0rtella' (http://nohost/plone/f1) !",
-            mailSent.split(b"\r\n\r\n")[1],
+        self.assertIn(
+            b"'D=C3=B2cumento' created in http://nohost/plone/f1/d1 - Sec=\ntion is 'C=C3=A0rtella' (http://nohost/plone/f1) !",
+            mailSent,
         )
 
     def testExecuteTargetByFieldName(self):
         self.loginAsPortalOwner()
         self.folder.d1.text = "member1@dummy.org"
         e = MailFromFieldAction()
         e.source = "foo@bar.be"
         e.fieldName = "text"
         e.target = "target"
+        e.subject = "Subject"
         e.message = "Còntènt '${title}' created in ${url} - Section is '${section_name}' (${section_url}) !"
         ex = getMultiAdapter((self.folder, e, DummyEvent(self.folder.d1)), IExecutable)
         ex()
         mailSent = self.mailhost.messages[0]
         self.assertIn(b'Content-Type: text/plain; charset="utf-8"', mailSent)
         self.assertIn(b"To: member1@dummy.org", mailSent)
         self.assertIn(b"From: foo@bar.be", mailSent)
-        self.assertEqual(
-            b"C=C3=B2nt=C3=A8nt 'D=C3=B2cumento' created in http://nohost/plone/f1/d1 - S=\r\n"
-            b"ection is 'C=C3=A0rtella' (http://nohost/plone/f1) !",
-            mailSent.split(b"\r\n\r\n")[1],
+        self.assertIn(
+            b"'D=C3=B2cumento' created in http://nohost/plone/f1/d1 - Sec=\ntion is 'C=C3=A0rtella' (http://nohost/plone/f1) !",
+            mailSent,
         )
 
     def testExecuteSimpleByCMFProperty(self):
         self.loginAsPortalOwner()
         self.folder.manage_addProperty("foo_property", "member1@dummy.org", "string")
         e = MailFromFieldAction()
         e.source = "foo@bar.be"
         e.fieldName = "foo_property"
         e.target = "object"
+        e.subject = "Subject"
         e.message = "Còntènt '${title}' created in ${url} - Section is '${section_name}' (${section_url}) !"
         ex = getMultiAdapter((self.folder, e, DummyEvent(self.folder.d1)), IExecutable)
         ex()
         mailSent = self.mailhost.messages[0]
         self.assertIn(b'Content-Type: text/plain; charset="utf-8"', mailSent)
         self.assertIn(b"To: member1@dummy.org", mailSent)
         self.assertIn(b"From: foo@bar.be", mailSent)
-        self.assertEqual(
-            b"C=C3=B2nt=C3=A8nt 'D=C3=B2cumento' created in http://nohost/plone/f1/d1 - S=\r\n"
-            b"ection is 'C=C3=A0rtella' (http://nohost/plone/f1) !",
-            mailSent.split(b"\r\n\r\n")[1],
+        self.assertIn(
+            b"'D=C3=B2cumento' created in http://nohost/plone/f1/d1 - Sec=\ntion is 'C=C3=A0rtella' (http://nohost/plone/f1) !",
+            mailSent,
         )
 
     def testExecuteFolderModify(self):
         # can happen as rules are not triggered on the rule root itself
         self.loginAsPortalOwner()
         self.folder.foo_property = "member1@dummy.org"
         e = MailFromFieldAction()
         e.source = "foo@bar.be"
         e.fieldName = "foo_property"
         e.target = "object"
+        e.subject = "Subject"
         e.message = "Còntènt '${title}' created in ${url} - Section is '${section_name}' (${section_url}) !"
         ex = getMultiAdapter((self.folder, e, DummyEvent(self.folder)), IExecutable)
         ex()
         mailSent = self.mailhost.messages[0]
         self.assertIn(b'Content-Type: text/plain; charset="utf-8"', mailSent)
         self.assertIn(b"To: member1@dummy.org", mailSent)
         self.assertIn(b"From: foo@bar.be", mailSent)
-        self.assertEqual(
-            b"C=C3=B2nt=C3=A8nt 'C=C3=A0rtella' created in http://nohost/plone/f1 - Secti=\r\n"
-            b"on is 'C=C3=A0rtella' (http://nohost/plone/f1) !",
-            mailSent.split(b"\r\n\r\n")[1],
+        self.assertIn(
+            b"C=C3=A0rtella' created in http://nohost/plone/f1 - Section=\n is 'C=C3=A0rtella' (http://nohost/plone/f1) !",
+            mailSent,
         )
 
     def testExecuteEmptyValue(self):
         self.loginAsPortalOwner()
         self.folder.foo_attr = ""
         e = MailFromFieldAction()
         e.source = "foo@bar.be"
         e.fieldName = "foo_attr"
         e.target = "object"
+        e.subject = "Subject"
         e.message = "Còntènt '${title}' created in ${url} - Section is '${section_name}' (${section_url}) !"
         getMultiAdapter((self.folder, e, DummyEvent(self.folder.d1)), IExecutable)()
         self.assertEqual(self.mailhost.messages, [])
 
 
 def test_suite():
     from unittest import makeSuite, TestSuite
```

### Comparing `collective.contentrules.mailfromfield-1.1.0/collective/contentrules/mailfromfield/vocabularies.py` & `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.1.0/collective.contentrules.mailfromfield.egg-info/PKG-INFO` & `collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,268 @@
 Metadata-Version: 2.1
 Name: collective.contentrules.mailfromfield
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Plone content rule for send e-mail to addresses taken from the content
+Home-page: UNKNOWN
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.contentrules.mailfromfield
 Project-URL: Source, https://github.com/RedTurtle/collective.contentrules.mailfromfield
 Project-URL: Tracker, https://github.com/RedTurtle/collective.contentrules.mailfromfield/issues
+Description: 
+        .. image:: https://img.shields.io/pypi/v/collective.contentrules.mailfromfield.svg
+            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+            :alt: Latest Version
+        
+        .. image:: https://img.shields.io/pypi/pyversions/collective.contentrules.mailfromfield.svg?style=plastic
+            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+            :alt: Supported - Python Versions
+        
+        .. image:: https://img.shields.io/pypi/dm/collective.contentrules.mailfromfield.svg
+            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+            :alt: Number of PyPI downloads
+        
+        .. image:: https://img.shields.io/pypi/l/collective.contentrules.mailfromfield.svg
+            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+            :alt: License
+        
+        .. image:: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions/workflows/tests.yml/badge.svg
+            :target: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions
+            :alt: Tests
+            
+        .. image:: https://coveralls.io/repos/github/RedTurtle/collective.contentrules.mailfromfield/badge.svg?branch=master
+            :target: https://coveralls.io/github/RedTurtle/collective.contentrules.mailfromfield?branch=master
+            :alt: Coverage
+        
+        .. contents::
+        
+        Introduction
+        ============
+        
+        This product will add to Plone a new content rules, someway similar to the default "*Send an email*" ones.
+        The difference is that the email recipient is taken dinamically from a site content, not from a
+        static list of values.
+        
+        In this way the same rule, applied in different places in the site, can send the message to different users.
+        
+        How to use
+        ==========
+        
+        The rules can be enabled globally and locally like every one else, as default Plone feature.
+        In the rule configuration panel you need to fill a set of information:
+        
+        ``Subject``
+            The e-mail subject. You can place inside this text some markers (see below).
+        ``Sender email``
+            The sender of the e-mail. You can leave this empty and automatically use the one from the
+            general mail settings.
+        ``Source field``
+            You must put there the name of the attribute from which you want to retrieve the recipient
+            e-mail. See next section.
+        ``Target element``
+            You need to select if the recipient's e-mail must be taken from:
+        
+            * the container where the rules is activated on
+            * the content who notified the event that started the rule execution
+            * the parent of that content
+        
+            See below for details.
+        ``Mail message``
+            The body text of the e-mail that will be sent. The text is the same for all section where
+            the rule is activated on.
+        
+            You can place inside this text some markers (see below).
+        
+        How it take the email data
+        --------------------------
+        
+        First of all you must choose the *Target element*.
+        
+        If you choose to keep default "*From rule's container*" option address will be read from the section you have
+        activated the rule on.
+        
+        *Example*: if you activated the rule on folder ``/site/section`` and the rule will raise event when
+        working on a document ``/site/section/folder/foo`` the email address will be taken
+        from the folder.
+        
+        Changing to "*From content that triggered the event*" will change the behavior, trying to get email data
+        from the content that raised the event.
+        
+        *Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
+        working on a document ``/site/section/folder/foo`` the email address will be taken
+        from the ``foo`` document.
+        
+        Finally, if you choose "*From content's parent*", adresses will the taken from the container of the content
+        that triggered the event.
+        
+        *Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
+        working on a document ``/site/section/folder/foo`` the email address will be taken
+        from ``folder``.
+        
+        What it try to read
+        -------------------
+        
+        The rule try to get from the object:
+        
+        * an attribute of the given name
+        * a callable method from the given name
+        * an Archetypes field with given id
+        * a ZMI property with given id
+        
+        The rule try to read, one after one, all this data. The first match found will be the one used;
+        if not one give results, no e-mail is sent at all.
+        
+        Message interpolation
+        ---------------------
+        
+        Marker labels that follow can be used in the message text and subject.
+        
+        ``${title}``
+            The title of the content that triggered the event (``foo`` title in our example)
+        ``${url}``
+            The URL of the content that triggered the event (``foo`` URL in our example)
+        ``${section_name}``
+            The title of the folder where the rule is activated on (``section`` title in our example)
+        ``${section_url}``
+            The URL of the folder where the rule is activated on (``section`` URL in our example)
+        
+        A real Plone use case
+        ---------------------
+        
+        A Plone site use `Signup Sheet`__ for manage internal training session. The form fieldset is
+        customized as normal, but one of the field is ``director_email``.
+        
+        __ http://plone.org/products/signupsheet
+        
+        We want that this e-mail address is notified when a user subscribe and the user
+        itself put there the e-mail address of the proper director.
+        
+        To reach this we need to:
+        
+        * create a new rule triggered on "*Object added to this container*"
+        * add a filter condition based on content type *Registrant*
+        * add an action using the "*Send email to address taken from the content*"
+        * specify in the action the SignupSheet field with the director email
+        * specify in the action that we want to take the email from the target content
+          (the Registrant itself)
+        
+        TODO
+        ====
+        
+        * why don't support also looking in annotations?
+        * right now the rules check all mail source until one is found with a defined order;
+          maybe is better to leave this choice to the configuration
+        * Dexterity support (probably already there, but needs to be tested)
+        
+        Requirements
+        ============
+        
+        This product has been tested on:
+        
+        * Plone 4.2 with 0.4 version
+        * Plone 4.3 with 0.4 version
+        * Plone 5.0
+        * Plone 5.1
+        
+        Credits
+        =======
+        
+        Developed with the support of `S. Anna Hospital, Ferrara`__; S. Anna Hospital supports the
+        `PloneGov initiative`__.
+        
+        .. image:: http://www.ospfe.it/ospfe-logo.jpg
+           :alt: OspFE logo
+        
+        __ http://www.ospfe.it/
+        __ http://www.plonegov.it/
+        
+        This product was largely developed looking at the source of `collective.contentrules.mailtogroup`__.
+        
+        __ http://plone.org/products/collective.contentrules.mailtogroup
+        
+        Authors
+        =======
+        
+        This product was developed by RedTurtle Technology team.
+        
+        .. image:: http://www.redturtle.it/redturtle_banner.png
+           :alt: RedTurtle Technology Site
+           :target: http://www.redturtle.it/
+        
+        
+        Changelog
+        =========
+        
+        1.2.0 (2023-06-19)
+        ------------------
+        
+        - Change mail send method and allow to eventually add attachments.
+          [cekk]
+        
+        1.1.0 (2023-06-19)
+        ------------------
+        
+        - Plone 6 support
+          [foxtrot-dfm1]
+        
+        1.0.1 (2021-03-10)
+        ------------------
+        
+        - Allow to get to the end of the action execution if no mail is provided.
+          You don't want the page to break if the email is missing. 
+          For the anonymous user this wold be a bad UX
+          [lucabel]
+        
+        
+        1.0.0 (2020-11-23)
+        ------------------
+        
+        - Migrate code to Plone 5/python 3.
+          [lucabel]
+        - Add support for plone.stringinterp.
+          [cekk]
+        
+        0.4.0 (2015-03-13)
+        ------------------
+        
+        Dropped Plone 3 compatibility
+        
+        - Fixed some label that were not i18n compatible
+          [keul]
+        - Fixed wrong documentation mess introduced on version 0.3:
+          the new "parent" option was wrongly descripted
+          [keul]
+        - Updated documentation to reflect changes done in version 0.3
+          [keul]
+        
+        0.3.0 (2014-05-06)
+        ------------------
+        
+        - Fix unicode error while replacing strings [nicolasenno]
+        - Do not fail if a rule is activated on a non-AT content [keul]
+        - Do not try to send mail to empty string recipients [keul]
+        - Refactoring [alert]
+        - Added parent option in the target vocabulary [alert]
+        
+        0.2.0 (2013-05-02)
+        ------------------
+        
+        * lowered logging level to debug
+          [keul]
+        * fixed ruleAction factory
+          [cekk]
+        
+        0.1.0 (2011-10-21)
+        ------------------
+        
+        * Initial release
+        
 Keywords: plone rules mail plonegov
+Platform: UNKNOWN
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
@@ -21,250 +271,7 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Communications :: Email
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Provides-Extra: test
-
-
-.. image:: https://img.shields.io/pypi/v/collective.contentrules.mailfromfield.svg
-    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-    :alt: Latest Version
-
-.. image:: https://img.shields.io/pypi/pyversions/collective.contentrules.mailfromfield.svg?style=plastic
-    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-    :alt: Supported - Python Versions
-
-.. image:: https://img.shields.io/pypi/dm/collective.contentrules.mailfromfield.svg
-    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-    :alt: Number of PyPI downloads
-
-.. image:: https://img.shields.io/pypi/l/collective.contentrules.mailfromfield.svg
-    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-    :alt: License
-
-.. image:: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions/workflows/tests.yml/badge.svg
-    :target: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions
-    :alt: Tests
-    
-.. image:: https://coveralls.io/repos/github/RedTurtle/collective.contentrules.mailfromfield/badge.svg?branch=main
-    :target: https://coveralls.io/github/RedTurtle/collective.contentrules.mailfromfield?branch=main
-    :alt: Coverage
-
-.. contents::
-
-Introduction
-============
-
-This product will add to Plone a new content rules, someway similar to the default "*Send an email*" ones.
-The difference is that the email recipient is taken dinamically from a site content, not from a
-static list of values.
-
-In this way the same rule, applied in different places in the site, can send the message to different users.
-
-How to use
-==========
-
-The rules can be enabled globally and locally like every one else, as default Plone feature.
-In the rule configuration panel you need to fill a set of information:
-
-``Subject``
-    The e-mail subject. You can place inside this text some markers (see below).
-``Sender email``
-    The sender of the e-mail. You can leave this empty and automatically use the one from the
-    general mail settings.
-``Source field``
-    You must put there the name of the attribute from which you want to retrieve the recipient
-    e-mail. See next section.
-``Target element``
-    You need to select if the recipient's e-mail must be taken from:
-
-    * the container where the rules is activated on
-    * the content who notified the event that started the rule execution
-    * the parent of that content
-
-    See below for details.
-``Mail message``
-    The body text of the e-mail that will be sent. The text is the same for all section where
-    the rule is activated on.
-
-    You can place inside this text some markers (see below).
-
-How it take the email data
---------------------------
-
-First of all you must choose the *Target element*.
-
-If you choose to keep default "*From rule's container*" option address will be read from the section you have
-activated the rule on.
-
-*Example*: if you activated the rule on folder ``/site/section`` and the rule will raise event when
-working on a document ``/site/section/folder/foo`` the email address will be taken
-from the folder.
-
-Changing to "*From content that triggered the event*" will change the behavior, trying to get email data
-from the content that raised the event.
-
-*Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
-working on a document ``/site/section/folder/foo`` the email address will be taken
-from the ``foo`` document.
-
-Finally, if you choose "*From content's parent*", adresses will the taken from the container of the content
-that triggered the event.
-
-*Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
-working on a document ``/site/section/folder/foo`` the email address will be taken
-from ``folder``.
-
-What it try to read
--------------------
-
-The rule try to get from the object:
-
-* an attribute of the given name
-* a callable method from the given name
-* an Archetypes field with given id
-* a ZMI property with given id
-
-The rule try to read, one after one, all this data. The first match found will be the one used;
-if not one give results, no e-mail is sent at all.
-
-Message interpolation
----------------------
-
-Marker labels that follow can be used in the message text and subject.
-
-``${title}``
-    The title of the content that triggered the event (``foo`` title in our example)
-``${url}``
-    The URL of the content that triggered the event (``foo`` URL in our example)
-``${section_name}``
-    The title of the folder where the rule is activated on (``section`` title in our example)
-``${section_url}``
-    The URL of the folder where the rule is activated on (``section`` URL in our example)
-
-A real Plone use case
----------------------
-
-A Plone site use `Signup Sheet`__ for manage internal training session. The form fieldset is
-customized as normal, but one of the field is ``director_email``.
-
-__ http://plone.org/products/signupsheet
-
-We want that this e-mail address is notified when a user subscribe and the user
-itself put there the e-mail address of the proper director.
-
-To reach this we need to:
-
-* create a new rule triggered on "*Object added to this container*"
-* add a filter condition based on content type *Registrant*
-* add an action using the "*Send email to address taken from the content*"
-* specify in the action the SignupSheet field with the director email
-* specify in the action that we want to take the email from the target content
-  (the Registrant itself)
-
-TODO
-====
-
-* why don't support also looking in annotations?
-* right now the rules check all mail source until one is found with a defined order;
-  maybe is better to leave this choice to the configuration
-* Dexterity support (probably already there, but needs to be tested)
-
-Requirements
-============
-
-This product has been tested on:
-
-* Plone 4.2 with 0.4 version
-* Plone 4.3 with 0.4 version
-* Plone 5.0
-* Plone 5.1
-
-Credits
-=======
-
-Developed with the support of `S. Anna Hospital, Ferrara`__; S. Anna Hospital supports the
-`PloneGov initiative`__.
-
-.. image:: http://www.ospfe.it/ospfe-logo.jpg
-   :alt: OspFE logo
-
-__ http://www.ospfe.it/
-__ http://www.plonegov.it/
-
-This product was largely developed looking at the source of `collective.contentrules.mailtogroup`__.
-
-__ http://plone.org/products/collective.contentrules.mailtogroup
-
-Authors
-=======
-
-This product was developed by RedTurtle Technology team.
-
-.. image:: http://www.redturtle.it/redturtle_banner.png
-   :alt: RedTurtle Technology Site
-   :target: http://www.redturtle.it/
-
-
-Changelog
-=========
-
-1.1.0 (2023-03-03)
-------------------
-
-- Plone 6 support
-  [foxtrot-dfm1]
-
-
-1.0.1 (2021-03-10)
-------------------
-
-- Allow to get to the end of the action execution if no mail is provided.
-  You don't want the page to break if the email is missing. 
-  For the anonymous user this wold be a bad UX
-  [lucabel]
-
-
-1.0.0 (2020-11-23)
-------------------
-
-- Migrate code to Plone 5/python 3.
-  [lucabel]
-- Add support for plone.stringinterp.
-  [cekk]
-
-0.4.0 (2015-03-13)
-------------------
-
-Dropped Plone 3 compatibility
-
-- Fixed some label that were not i18n compatible
-  [keul]
-- Fixed wrong documentation mess introduced on version 0.3:
-  the new "parent" option was wrongly descripted
-  [keul]
-- Updated documentation to reflect changes done in version 0.3
-  [keul]
-
-0.3.0 (2014-05-06)
-------------------
-
-- Fix unicode error while replacing strings [nicolasenno]
-- Do not fail if a rule is activated on a non-AT content [keul]
-- Do not try to send mail to empty string recipients [keul]
-- Refactoring [alert]
-- Added parent option in the target vocabulary [alert]
-
-0.2.0 (2013-05-02)
-------------------
-
-* lowered logging level to debug
-  [keul]
-* fixed ruleAction factory
-  [cekk]
-
-0.1.0 (2011-10-21)
-------------------
-
-* Initial release
```

### Comparing `collective.contentrules.mailfromfield-1.1.0/collective.contentrules.mailfromfield.egg-info/SOURCES.txt` & `collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 collective/contentrules/mailfromfield/actions/__init__.py
 collective/contentrules/mailfromfield/actions/configure.zcml
 collective/contentrules/mailfromfield/actions/mail.py
 collective/contentrules/mailfromfield/locales/collective.contentrules.mailfromfield.pot
 collective/contentrules/mailfromfield/locales/plone-manual.pot
 collective/contentrules/mailfromfield/locales/plone.pot
 collective/contentrules/mailfromfield/locales/rebuildAll.sh
+collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/collective.contentrules.mailfromfield.mo
 collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/collective.contentrules.mailfromfield.po
+collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/plone.mo
 collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/plone.po
 collective/contentrules/mailfromfield/tests/__init__.py
 collective/contentrules/mailfromfield/tests/test_actions_mailfromfield.py
 docs/HISTORY.rst
 docs/INSTALL.txt
 docs/LICENSE.GPL
 docs/LICENSE.txt
```

### Comparing `collective.contentrules.mailfromfield-1.1.0/docs/HISTORY.rst` & `collective.contentrules.mailfromfield-1.2.0/docs/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Changelog
 =========
 
-1.1.0 (2023-03-03)
+1.2.0 (2023-06-19)
+------------------
+
+- Change mail send method and allow to eventually add attachments.
+  [cekk]
+
+1.1.0 (2023-06-19)
 ------------------
 
 - Plone 6 support
   [foxtrot-dfm1]
 
-
 1.0.1 (2021-03-10)
 ------------------
 
 - Allow to get to the end of the action execution if no mail is provided.
   You don't want the page to break if the email is missing. 
   For the anonymous user this wold be a bad UX
   [lucabel]
```

### Comparing `collective.contentrules.mailfromfield-1.1.0/docs/INSTALL.txt` & `collective.contentrules.mailfromfield-1.2.0/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.1.0/docs/LICENSE.GPL` & `collective.contentrules.mailfromfield-1.2.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.1.0/docs/LICENSE.txt` & `collective.contentrules.mailfromfield-1.2.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.1.0/setup.cfg` & `collective.contentrules.mailfromfield-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.1.0/setup.py` & `collective.contentrules.mailfromfield-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-version = "1.1.0"
+version = "1.2.0"
 
 tests_require = ["plone.app.robotframework"]
 
 setup(
     name="collective.contentrules.mailfromfield",
     version=version,
     description="A Plone content rule for send e-mail to addresses taken from the content",
```

