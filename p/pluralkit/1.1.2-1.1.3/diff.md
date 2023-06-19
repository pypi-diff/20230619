# Comparing `tmp/pluralkit-1.1.2.tar.gz` & `tmp/pluralkit-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluralkit-1.1.2.tar", last modified: Sun Apr 16 00:48:33 2023, max compression
+gzip compressed data, was "pluralkit-1.1.3.tar", last modified: Mon Jun 19 13:21:14 2023, max compression
```

## Comparing `pluralkit-1.1.2.tar` & `pluralkit-1.1.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/
--rw-rw-r--   0 k         (1001) k         (1001)     1068 2022-12-30 16:02:53.000000 pluralkit-1.1.2/LICENSE
--rw-rw-r--   0 k         (1001) k         (1001)      267 2022-12-30 16:02:53.000000 pluralkit-1.1.2/MANIFEST.in
--rw-rw-r--   0 k         (1001) k         (1001)     5450 2023-04-16 00:48:33.764970 pluralkit-1.1.2/PKG-INFO
--rw-rw-r--   0 k         (1001) k         (1001)     3519 2022-12-30 16:02:53.000000 pluralkit-1.1.2/README.md
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/
--rw-rw-r--   0 k         (1001) k         (1001)      634 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/Makefile
--rw-rw-r--   0 k         (1001) k         (1001)      652 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/README.md
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/_sources/
--rw-rw-r--   0 k         (1001) k         (1001)     1273 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/_build/html/_sources/index.rst.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/_sources/source/
--rw-rw-r--   0 k         (1001) k         (1001)     3929 2022-12-30 19:14:51.000000 pluralkit-1.1.2/docs/_build/html/_sources/source/changelog.rst.txt
--rw-rw-r--   0 k         (1001) k         (1001)    12062 2022-12-30 16:22:51.000000 pluralkit-1.1.2/docs/_build/html/_sources/source/quickstart.rst.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/_sources/source/v1/
--rw-rw-r--   0 k         (1001) k         (1001)     1761 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/_build/html/_sources/source/v1/api.rst.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/_build/html/_sources/source/v2/
--rw-rw-r--   0 k         (1001) k         (1001)     2943 2022-12-30 18:59:51.000000 pluralkit-1.1.2/docs/_build/html/_sources/source/v2/api.rst.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/_build/html/_static/
--rw-rw-r--   0 k         (1001) k         (1001)        0 2022-12-30 16:23:23.000000 pluralkit-1.1.2/docs/_build/html/_static/__init__.py
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/_static/vendor/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/_static/vendor/fontawesome/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/_build/html/_static/vendor/fontawesome/5.13.0/
--rw-rw-r--   0 k         (1001) k         (1001)     1548 2022-12-30 16:23:23.000000 pluralkit-1.1.2/docs/_build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/_static/vendor/lato_latin-ext/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/
--rw-rw-r--   0 k         (1001) k         (1001)     1054 2022-12-30 16:23:23.000000 pluralkit-1.1.2/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/LICENSE.md
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/_static/vendor/open-sans_all/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/_build/html/_static/vendor/open-sans_all/1.44.1/
--rw-rw-r--   0 k         (1001) k         (1001)     1054 2022-12-30 16:23:23.000000 pluralkit-1.1.2/docs/_build/html/_static/vendor/open-sans_all/1.44.1/LICENSE.md
--rw-rw-r--   0 k         (1001) k         (1001)     3312 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/conf.py
--rw-rw-r--   0 k         (1001) k         (1001)     1273 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/index.rst
--rw-rw-r--   0 k         (1001) k         (1001)      234 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/requirements.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/source/
--rw-rw-r--   0 k         (1001) k         (1001)     3932 2022-12-30 19:15:15.000000 pluralkit-1.1.2/docs/source/changelog.rst
--rw-rw-r--   0 k         (1001) k         (1001)    12062 2022-12-30 16:22:51.000000 pluralkit-1.1.2/docs/source/quickstart.rst
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/source/v1/
--rw-rw-r--   0 k         (1001) k         (1001)     1761 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/source/v1/api.rst
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/source/v2/
--rw-rw-r--   0 k         (1001) k         (1001)     2943 2022-12-30 18:59:51.000000 pluralkit-1.1.2/docs/source/v2/api.rst
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/pluralkit/
--rw-rw-r--   0 k         (1001) k         (1001)      252 2022-12-31 00:26:34.000000 pluralkit-1.1.2/pluralkit/__init__.py
--rw-rw-r--   0 k         (1001) k         (1001)      248 2023-04-16 00:45:21.000000 pluralkit-1.1.2/pluralkit/__version__.py
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/pluralkit/v1/
--rw-rw-r--   0 k         (1001) k         (1001)      217 2022-12-30 16:02:53.000000 pluralkit-1.1.2/pluralkit/v1/__init__.py
--rw-rw-r--   0 k         (1001) k         (1001)    32468 2022-12-30 16:02:53.000000 pluralkit-1.1.2/pluralkit/v1/client.py
--rw-rw-r--   0 k         (1001) k         (1001)     2824 2022-12-30 16:02:53.000000 pluralkit-1.1.2/pluralkit/v1/errors.py
--rw-rw-r--   0 k         (1001) k         (1001)    38036 2022-12-30 16:02:53.000000 pluralkit-1.1.2/pluralkit/v1/models.py
--rw-rw-r--   0 k         (1001) k         (1001)     4302 2022-12-30 16:02:53.000000 pluralkit-1.1.2/pluralkit/v1/utils.py
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/pluralkit/v2/
--rw-rw-r--   0 k         (1001) k         (1001)      666 2022-12-30 18:59:05.000000 pluralkit-1.1.2/pluralkit/v2/__init__.py
--rw-rw-r--   0 k         (1001) k         (1001)    49619 2022-12-30 18:30:46.000000 pluralkit-1.1.2/pluralkit/v2/client.py
--rw-rw-r--   0 k         (1001) k         (1001)     2821 2022-12-30 16:02:53.000000 pluralkit-1.1.2/pluralkit/v2/errors.py
--rw-rw-r--   0 k         (1001) k         (1001)    38954 2023-04-16 00:40:49.000000 pluralkit-1.1.2/pluralkit/v2/models.py
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/pluralkit.egg-info/
--rw-rw-r--   0 k         (1001) k         (1001)     5450 2023-04-16 00:48:33.000000 pluralkit-1.1.2/pluralkit.egg-info/PKG-INFO
--rw-rw-r--   0 k         (1001) k         (1001)     1166 2023-04-16 00:48:33.000000 pluralkit-1.1.2/pluralkit.egg-info/SOURCES.txt
--rw-rw-r--   0 k         (1001) k         (1001)        1 2023-04-16 00:48:33.000000 pluralkit-1.1.2/pluralkit.egg-info/dependency_links.txt
--rw-rw-r--   0 k         (1001) k         (1001)      188 2023-04-16 00:48:33.000000 pluralkit-1.1.2/pluralkit.egg-info/requires.txt
--rw-rw-r--   0 k         (1001) k         (1001)       10 2023-04-16 00:48:33.000000 pluralkit-1.1.2/pluralkit.egg-info/top_level.txt
--rw-rw-r--   0 k         (1001) k         (1001)       38 2023-04-16 00:48:33.764970 pluralkit-1.1.2/setup.cfg
--rw-rw-r--   0 k         (1001) k         (1001)     2217 2022-12-31 00:34:09.000000 pluralkit-1.1.2/setup.py
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/tests/
--rw-rw-r--   0 k         (1001) k         (1001)     6785 2022-12-30 16:02:53.000000 pluralkit-1.1.2/tests/test_member.py
--rw-rw-r--   0 k         (1001) k         (1001)      503 2022-12-30 16:02:53.000000 pluralkit-1.1.2/tests/test_misc.py
--rw-rw-r--   0 k         (1001) k         (1001)     2671 2022-12-30 16:02:53.000000 pluralkit-1.1.2/tests/test_system.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.464726 pluralkit-1.1.3/
+-rw-rw-r--   0 k         (1001) k         (1001)     1068 2022-12-30 16:02:53.000000 pluralkit-1.1.3/LICENSE
+-rw-rw-r--   0 k         (1001) k         (1001)      267 2022-12-30 16:02:53.000000 pluralkit-1.1.3/MANIFEST.in
+-rw-rw-r--   0 k         (1001) k         (1001)     4903 2023-06-19 13:21:14.464726 pluralkit-1.1.3/PKG-INFO
+-rw-rw-r--   0 k         (1001) k         (1001)     3729 2023-06-19 13:14:23.000000 pluralkit-1.1.3/README.md
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.460726 pluralkit-1.1.3/docs/
+-rw-rw-r--   0 k         (1001) k         (1001)      634 2022-12-30 16:02:53.000000 pluralkit-1.1.3/docs/Makefile
+-rw-rw-r--   0 k         (1001) k         (1001)      652 2022-12-30 16:02:53.000000 pluralkit-1.1.3/docs/README.md
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.456726 pluralkit-1.1.3/docs/_build/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.456726 pluralkit-1.1.3/docs/_build/html/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.460726 pluralkit-1.1.3/docs/_build/html/_sources/
+-rw-rw-r--   0 k         (1001) k         (1001)     1273 2022-12-30 16:02:53.000000 pluralkit-1.1.3/docs/_build/html/_sources/index.rst.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.460726 pluralkit-1.1.3/docs/_build/html/_sources/source/
+-rw-rw-r--   0 k         (1001) k         (1001)     3929 2022-12-30 19:14:51.000000 pluralkit-1.1.3/docs/_build/html/_sources/source/changelog.rst.txt
+-rw-rw-r--   0 k         (1001) k         (1001)    12062 2022-12-30 16:22:51.000000 pluralkit-1.1.3/docs/_build/html/_sources/source/quickstart.rst.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.460726 pluralkit-1.1.3/docs/_build/html/_sources/source/v1/
+-rw-rw-r--   0 k         (1001) k         (1001)     1761 2022-12-30 16:02:53.000000 pluralkit-1.1.3/docs/_build/html/_sources/source/v1/api.rst.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.460726 pluralkit-1.1.3/docs/_build/html/_sources/source/v2/
+-rw-rw-r--   0 k         (1001) k         (1001)     2943 2022-12-30 18:59:51.000000 pluralkit-1.1.3/docs/_build/html/_sources/source/v2/api.rst.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.460726 pluralkit-1.1.3/docs/_build/html/_static/
+-rw-rw-r--   0 k         (1001) k         (1001)        0 2022-12-30 16:23:23.000000 pluralkit-1.1.3/docs/_build/html/_static/__init__.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.456726 pluralkit-1.1.3/docs/_build/html/_static/vendor/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.456726 pluralkit-1.1.3/docs/_build/html/_static/vendor/fontawesome/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.460726 pluralkit-1.1.3/docs/_build/html/_static/vendor/fontawesome/5.13.0/
+-rw-rw-r--   0 k         (1001) k         (1001)     1548 2022-12-30 16:23:23.000000 pluralkit-1.1.3/docs/_build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.456726 pluralkit-1.1.3/docs/_build/html/_static/vendor/lato_latin-ext/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.460726 pluralkit-1.1.3/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/
+-rw-rw-r--   0 k         (1001) k         (1001)     1054 2022-12-30 16:23:23.000000 pluralkit-1.1.3/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/LICENSE.md
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.456726 pluralkit-1.1.3/docs/_build/html/_static/vendor/open-sans_all/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.460726 pluralkit-1.1.3/docs/_build/html/_static/vendor/open-sans_all/1.44.1/
+-rw-rw-r--   0 k         (1001) k         (1001)     1054 2022-12-30 16:23:23.000000 pluralkit-1.1.3/docs/_build/html/_static/vendor/open-sans_all/1.44.1/LICENSE.md
+-rw-rw-r--   0 k         (1001) k         (1001)     3312 2022-12-30 16:02:53.000000 pluralkit-1.1.3/docs/conf.py
+-rw-rw-r--   0 k         (1001) k         (1001)     1273 2022-12-30 16:02:53.000000 pluralkit-1.1.3/docs/index.rst
+-rw-rw-r--   0 k         (1001) k         (1001)      234 2022-12-30 16:02:53.000000 pluralkit-1.1.3/docs/requirements.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.460726 pluralkit-1.1.3/docs/source/
+-rw-rw-r--   0 k         (1001) k         (1001)     3932 2022-12-30 19:15:15.000000 pluralkit-1.1.3/docs/source/changelog.rst
+-rw-rw-r--   0 k         (1001) k         (1001)    12062 2022-12-30 16:22:51.000000 pluralkit-1.1.3/docs/source/quickstart.rst
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.460726 pluralkit-1.1.3/docs/source/v1/
+-rw-rw-r--   0 k         (1001) k         (1001)     1761 2022-12-30 16:02:53.000000 pluralkit-1.1.3/docs/source/v1/api.rst
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.460726 pluralkit-1.1.3/docs/source/v2/
+-rw-rw-r--   0 k         (1001) k         (1001)     2943 2022-12-30 18:59:51.000000 pluralkit-1.1.3/docs/source/v2/api.rst
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.460726 pluralkit-1.1.3/pluralkit/
+-rw-rw-r--   0 k         (1001) k         (1001)      252 2022-12-31 00:26:34.000000 pluralkit-1.1.3/pluralkit/__init__.py
+-rw-rw-r--   0 k         (1001) k         (1001)      248 2023-06-19 13:17:48.000000 pluralkit-1.1.3/pluralkit/__version__.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.460726 pluralkit-1.1.3/pluralkit/v1/
+-rw-rw-r--   0 k         (1001) k         (1001)      217 2022-12-30 16:02:53.000000 pluralkit-1.1.3/pluralkit/v1/__init__.py
+-rw-rw-r--   0 k         (1001) k         (1001)    32468 2022-12-30 16:02:53.000000 pluralkit-1.1.3/pluralkit/v1/client.py
+-rw-rw-r--   0 k         (1001) k         (1001)     2824 2022-12-30 16:02:53.000000 pluralkit-1.1.3/pluralkit/v1/errors.py
+-rw-rw-r--   0 k         (1001) k         (1001)    38036 2022-12-30 16:02:53.000000 pluralkit-1.1.3/pluralkit/v1/models.py
+-rw-rw-r--   0 k         (1001) k         (1001)     4302 2022-12-30 16:02:53.000000 pluralkit-1.1.3/pluralkit/v1/utils.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.464726 pluralkit-1.1.3/pluralkit/v2/
+-rw-rw-r--   0 k         (1001) k         (1001)      666 2022-12-30 18:59:05.000000 pluralkit-1.1.3/pluralkit/v2/__init__.py
+-rw-rw-r--   0 k         (1001) k         (1001)    49619 2022-12-30 18:30:46.000000 pluralkit-1.1.3/pluralkit/v2/client.py
+-rw-rw-r--   0 k         (1001) k         (1001)     2821 2022-12-30 16:02:53.000000 pluralkit-1.1.3/pluralkit/v2/errors.py
+-rw-rw-r--   0 k         (1001) k         (1001)    39157 2023-06-19 13:12:49.000000 pluralkit-1.1.3/pluralkit/v2/models.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.460726 pluralkit-1.1.3/pluralkit.egg-info/
+-rw-rw-r--   0 k         (1001) k         (1001)     4903 2023-06-19 13:21:14.000000 pluralkit-1.1.3/pluralkit.egg-info/PKG-INFO
+-rw-rw-r--   0 k         (1001) k         (1001)     1166 2023-06-19 13:21:14.000000 pluralkit-1.1.3/pluralkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 k         (1001) k         (1001)        1 2023-06-19 13:21:14.000000 pluralkit-1.1.3/pluralkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 k         (1001) k         (1001)      188 2023-06-19 13:21:14.000000 pluralkit-1.1.3/pluralkit.egg-info/requires.txt
+-rw-rw-r--   0 k         (1001) k         (1001)       10 2023-06-19 13:21:14.000000 pluralkit-1.1.3/pluralkit.egg-info/top_level.txt
+-rw-rw-r--   0 k         (1001) k         (1001)       38 2023-06-19 13:21:14.464726 pluralkit-1.1.3/setup.cfg
+-rw-rw-r--   0 k         (1001) k         (1001)     2217 2022-12-31 00:34:09.000000 pluralkit-1.1.3/setup.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-19 13:21:14.464726 pluralkit-1.1.3/tests/
+-rw-rw-r--   0 k         (1001) k         (1001)     6785 2022-12-30 16:02:53.000000 pluralkit-1.1.3/tests/test_member.py
+-rw-rw-r--   0 k         (1001) k         (1001)      503 2022-12-30 16:02:53.000000 pluralkit-1.1.3/tests/test_misc.py
+-rw-rw-r--   0 k         (1001) k         (1001)     2671 2022-12-30 16:02:53.000000 pluralkit-1.1.3/tests/test_system.py
```

### Comparing `pluralkit-1.1.2/LICENSE` & `pluralkit-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/README.md` & `pluralkit-1.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -71,18 +71,19 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 
 <table>
    <tr>
-      <td align="center"><a href="https://github.com/Alyx-W"><img src="https://avatars.githubusercontent.com/u/58519807?v=4&s=100" width="100px;" alt=""/><br/><sub><b>Alyx</b></sub></a><br/>💻🤔🚇⚠️💬</td>
+      <td align="center"><a href="https://github.com/moon-dew/"><img src="https://avatars.githubusercontent.com/u/58519807?v=4&s=100" width="100px;" alt=""/><br/><sub><b>Alyx</b></sub></a><br/>💻🤔🚇⚠️💬</td>
       <td align="center"><a href="https://github.com/almond0166"><img src="https://avatars.githubusercontent.com/u/42977337?v=4&s=100" width="100px;" alt=""/><br/><sub><b>Kotocade</b></sub></a><br/>💻📖🤔🚧📆💬</td>
       <td align="center"><a href="https://github.com/powertashton"><img src="https://avatars.githubusercontent.com/u/48048360?v=4&s=100" width="100px;" alt=""/><br/><sub><b>Ashton Power</b></sub></a><br/>💻📓</td>
       <td align="center"><a href="https://github.com/systeminabox"><img src="https://avatars.githubusercontent.com/u/106895862?v=4&s=100" width="100px;" alt=""/><br/><sub><b>System in a Box</b></sub></a><br/>🐛</td>
+      <td align="center"><a href="https://github.com/Ringlings"><img src="https://avatars.githubusercontent.com/u/110815694?v=4&s=100" width="100px;" alt=""/><br/><sub><b>Gem</b></sub></a><br/>💻🐛</td>
    </tr>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -22,15 +22,15 @@
 {member.id}`)") ``` ## Token The client can be used without one's [PluralKit
 authorization token](https://pluralkit.me/api/#authentication), but it's
 required for editing one's system or members or for accessing one's private
 system or member info. ## Contributors â¨ Thanks to these wonderful people (
 [emoji key](https://allcontributors.org/docs/en/emoji-key)) and users in the
 Discord who actively supported development:
 
-                    Alyx                                         Kotocade                       Ashton_Power    System
+                    Alyx                                         Kotocade                       Ashton_Power    System        Gem
                                                                                                                in_a_Box
-           ð»ð¤ðâ ï¸            ð»ðð¤ð§ð�    ð»ð�
+           ð»ð¤ðâ ï¸            ð»ðð¤ð§ð�    ð»ð�             ð»ð
                                                                                                                  ð
    ## Links * [PyPI link](https://pypi.org/project/pluralkit/) * [Latest build
 of the docs](https://pluralkit.readthedocs.io/en/latest/) * [pluralkit.py
 Discord support server](https://discord.gg/secvguatbC) * [PluralKit support
 server](https://discord.gg/PczBt78) * [PluralKit's API](https://pluralkit.me/)
```

### Comparing `pluralkit-1.1.2/docs/Makefile` & `pluralkit-1.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/docs/README.md` & `pluralkit-1.1.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/docs/_build/html/_sources/index.rst.txt` & `pluralkit-1.1.3/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/docs/_build/html/_sources/source/changelog.rst.txt` & `pluralkit-1.1.3/docs/_build/html/_sources/source/changelog.rst.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/docs/_build/html/_sources/source/quickstart.rst.txt` & `pluralkit-1.1.3/docs/_build/html/_sources/source/quickstart.rst.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/docs/_build/html/_sources/source/v1/api.rst.txt` & `pluralkit-1.1.3/docs/_build/html/_sources/source/v1/api.rst.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/docs/_build/html/_sources/source/v2/api.rst.txt` & `pluralkit-1.1.3/docs/_build/html/_sources/source/v2/api.rst.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/docs/_build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt` & `pluralkit-1.1.3/docs/_build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/LICENSE.md` & `pluralkit-1.1.3/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/docs/_build/html/_static/vendor/open-sans_all/1.44.1/LICENSE.md` & `pluralkit-1.1.3/docs/_build/html/_static/vendor/open-sans_all/1.44.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/docs/conf.py` & `pluralkit-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/docs/index.rst` & `pluralkit-1.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/docs/source/changelog.rst` & `pluralkit-1.1.3/docs/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/docs/source/quickstart.rst` & `pluralkit-1.1.3/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/docs/source/v1/api.rst` & `pluralkit-1.1.3/docs/source/v1/api.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/docs/source/v2/api.rst` & `pluralkit-1.1.3/docs/source/v2/api.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/pluralkit/v1/client.py` & `pluralkit-1.1.3/pluralkit/v1/client.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/pluralkit/v1/errors.py` & `pluralkit-1.1.3/pluralkit/v1/errors.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/pluralkit/v1/models.py` & `pluralkit-1.1.3/pluralkit/v1/models.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/pluralkit/v1/utils.py` & `pluralkit-1.1.3/pluralkit/v1/utils.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/pluralkit/v2/__init__.py` & `pluralkit-1.1.3/pluralkit/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/pluralkit/v2/client.py` & `pluralkit-1.1.3/pluralkit/v2/client.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/pluralkit/v2/errors.py` & `pluralkit-1.1.3/pluralkit/v2/errors.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/pluralkit/v2/models.py` & `pluralkit-1.1.3/pluralkit/v2/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,15 +690,17 @@
         name: The member's name.
         created: The member's creation timestamp.
         display_name: The member's display name.
         description: The member's description.
         color: The member's color.
         birthday: The member's birthday.
         pronouns: The member's pronouns.
-        avatar_url: The member's avatar url.
+        avatar_url: The member's main avatar url that appears uncropped on the member card.
+        webhook_avatar_url: The member's avatar url used for proxied messages instead of the main
+            avatar.
         banner: The member's banner url.
         proxy_tags: The member's proxy tags.
         keep_proxy (bool): Whether the member's proxy tags remain in the proxied message or not.
         name_privacy: Whether the member name is visible to others or only the display name.
         description_privacy: Whether this member's description is visible to others.
         birthday_privacy: Whether the member's birthday is visible to others.
         pronoun_privacy: Whether the member's pronouns are visible to others.
@@ -725,14 +727,15 @@
     visibility: Optional[Privacy]
     display_name: Optional[str]
     description: Optional[str]
     color: Optional[Color]
     birthday: Optional[Birthday]
     pronouns: Optional[str]
     avatar_url: Optional[str]
+    webhook_avatar_url: Optional[str]
     keep_proxy: bool
     proxy_tags: Optional[ProxyTags]
     system: SystemId
     banner: Optional[str]
     autoproxy_enabled: Optional[bool]
     message_count: Optional[int]
     last_message_timestamp: Optional[Timestamp]
```

### Comparing `pluralkit-1.1.2/pluralkit.egg-info/SOURCES.txt` & `pluralkit-1.1.3/pluralkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/setup.py` & `pluralkit-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/tests/test_member.py` & `pluralkit-1.1.3/tests/test_member.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.2/tests/test_system.py` & `pluralkit-1.1.3/tests/test_system.py`

 * *Files identical despite different names*

