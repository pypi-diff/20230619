# Comparing `tmp/gengive-2022.8.2.tar.gz` & `tmp/gengive-2023.6.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gengive-2022.8.2.tar", last modified: Tue Aug  2 04:24:04 2022, max compression
+gzip compressed data, was "gengive-2023.6.19.tar", last modified: Mon Jun 19 20:46:47 2023, max compression
```

## Comparing `gengive-2022.8.2.tar` & `gengive-2023.6.19.tar`

### file list

```diff
@@ -1,63 +1,22 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-02 04:24:04.422702 gengive-2022.8.2/
--rw-r--r--   0 ruth       (501) staff       (20)     1161 2022-04-30 21:02:24.000000 gengive-2022.8.2/.editorconfig
--rw-r--r--   0 ruth       (501) staff       (20)       19 2022-06-18 09:14:29.000000 gengive-2022.8.2/.gitattributes
--rw-r--r--   0 ruth       (501) staff       (20)     1957 2022-08-02 04:09:34.000000 gengive-2022.8.2/.gitignore
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2022-01-11 18:58:55.000000 gengive-2022.8.2/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 gengive-2022.8.2/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     2000 2022-08-02 04:11:17.000000 gengive-2022.8.2/Makefile
--rw-r--r--   0 ruth       (501) staff       (20)     2158 2022-08-02 04:24:04.423037 gengive-2022.8.2/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1186 2022-08-02 04:01:23.000000 gengive-2022.8.2/README.md
--rw-r--r--   0 ruth       (501) staff       (20)     1699 2022-08-02 04:15:05.000000 gengive-2022.8.2/baseline-bandit.json
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-02 04:24:04.390833 gengive-2022.8.2/docs/
--rw-r--r--   0 ruth       (501) staff       (20)       37 2022-01-11 20:29:14.000000 gengive-2022.8.2/docs/api.md
--rw-r--r--   0 ruth       (501) staff       (20)     1093 2022-08-02 04:07:19.000000 gengive-2022.8.2/docs/changes.md
--rw-r--r--   0 ruth       (501) staff       (20)     1116 2022-08-02 04:01:47.000000 gengive-2022.8.2/docs/index.md
--rw-r--r--   0 ruth       (501) staff       (20)      237 2022-08-02 04:00:18.000000 gengive-2022.8.2/docs/install.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-02 04:24:04.398744 gengive-2022.8.2/docs/third-party/
--rw-r--r--   0 ruth       (501) staff       (20)     3725 2022-08-02 04:16:05.000000 gengive-2022.8.2/docs/third-party/README.md
--rw-r--r--   0 ruth       (501) staff       (20)     8911 2022-08-02 04:15:59.000000 gengive-2022.8.2/docs/third-party/all-dependency-licenses.json
--rw-r--r--   0 ruth       (501) staff       (20)     6955 2022-08-02 04:15:58.000000 gengive-2022.8.2/docs/third-party/direct-dependency-licenses.json
--rw-r--r--   0 ruth       (501) staff       (20)      260 2022-08-02 04:16:05.000000 gengive-2022.8.2/docs/third-party/package-dependency-tree.console.txt
--rw-r--r--   0 ruth       (501) staff       (20)      440 2022-08-02 04:16:00.000000 gengive-2022.8.2/docs/third-party/package-dependency-tree.dot.txt
--rw-r--r--   0 ruth       (501) staff       (20)     1668 2022-08-02 04:16:03.000000 gengive-2022.8.2/docs/third-party/package-dependency-tree.json
--rw-r--r--   0 ruth       (501) staff       (20)     5225 2022-08-02 04:16:02.000000 gengive-2022.8.2/docs/third-party/package-dependency-tree.svg
--rw-r--r--   0 ruth       (501) staff       (20)     9356 2022-08-02 04:00:02.000000 gengive-2022.8.2/docs/usage.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-02 04:24:04.365741 gengive-2022.8.2/examples/
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-02 04:24:04.400748 gengive-2022.8.2/examples/bar/
--rw-r--r--   0 ruth       (501) staff       (20)        7 2022-01-30 15:41:15.000000 gengive-2022.8.2/examples/bar/bind-default.txt
--rw-r--r--   0 ruth       (501) staff       (20)      410 2022-02-02 21:03:29.000000 gengive-2022.8.2/examples/bar/foo.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-02 04:24:04.401724 gengive-2022.8.2/examples/bar/images/
--rw-r--r--   0 ruth       (501) staff       (20)      277 2022-02-02 21:05:34.000000 gengive-2022.8.2/examples/bar/images/red.png
--rw-r--r--   0 ruth       (501) staff       (20)       92 2022-02-03 21:49:52.000000 gengive-2022.8.2/examples/bar/render-config.json
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-02 04:24:04.402935 gengive-2022.8.2/examples/bar/styles/
--rw-r--r--   0 ruth       (501) staff       (20)      687 2022-02-03 21:49:11.000000 gengive-2022.8.2/examples/bar/styles/default.css
--rwxr-xr-x   0 ruth       (501) staff       (20)      240 2022-02-27 12:03:21.000000 gengive-2022.8.2/gen-sbom
--rw-r--r--   0 ruth       (501) staff       (20)     5810 2022-07-28 15:18:24.000000 gengive-2022.8.2/gen_licenses.py
--rw-r--r--   0 ruth       (501) staff       (20)      599 2022-07-28 15:11:55.000000 gengive-2022.8.2/gen_sbom.py
--rw-r--r--   0 ruth       (501) staff       (20)     1093 2022-07-09 20:50:34.000000 gengive-2022.8.2/gen_version.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-02 04:24:04.409256 gengive-2022.8.2/gengive/
--rw-r--r--   0 ruth       (501) staff       (20)      748 2022-08-02 04:20:21.000000 gengive-2022.8.2/gengive/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      232 2022-01-11 20:35:11.000000 gengive-2022.8.2/gengive/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     2556 2022-02-02 21:24:11.000000 gengive-2022.8.2/gengive/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)    20814 2022-02-03 22:09:48.000000 gengive-2022.8.2/gengive/gengive.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-02 04:24:04.416596 gengive-2022.8.2/gengive.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     2158 2022-08-02 04:24:04.000000 gengive-2022.8.2/gengive.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1151 2022-08-02 04:24:04.000000 gengive-2022.8.2/gengive.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2022-08-02 04:24:04.000000 gengive-2022.8.2/gengive.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       44 2022-08-02 04:24:04.000000 gengive-2022.8.2/gengive.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      123 2022-08-02 04:24:04.000000 gengive-2022.8.2/gengive.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)       13 2022-08-02 04:24:04.000000 gengive-2022.8.2/gengive.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     1304 2022-08-02 04:02:54.000000 gengive-2022.8.2/mkdocs.yml
--rw-r--r--   0 ruth       (501) staff       (20)      200 2022-05-22 10:06:06.000000 gengive-2022.8.2/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       57 2022-07-16 06:35:50.000000 gengive-2022.8.2/requirements.txt
--rw-r--r--   0 ruth       (501) staff       (20)     2758 2022-08-02 04:15:56.000000 gengive-2022.8.2/sbom.json
--rw-r--r--   0 ruth       (501) staff       (20)       65 2022-08-02 04:15:56.000000 gengive-2022.8.2/sbom.json.sha256
--rw-r--r--   0 ruth       (501) staff       (20)     1842 2022-08-02 04:24:04.424445 gengive-2022.8.2/setup.cfg
--rw-r--r--   0 ruth       (501) staff       (20)       38 2021-12-08 15:53:54.000000 gengive-2022.8.2/setup.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-02 04:24:04.422217 gengive-2022.8.2/test/
--rw-r--r--   0 ruth       (501) staff       (20)      130 2021-12-20 19:14:02.000000 gengive-2022.8.2/test/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-01-11 19:01:13.000000 gengive-2022.8.2/test/conftest.py
--rw-r--r--   0 ruth       (501) staff       (20)      681 2022-08-02 03:35:26.000000 gengive-2022.8.2/test/requirements-dev.txt
--rw-r--r--   0 ruth       (501) staff       (20)      705 2022-07-25 17:54:01.000000 gengive-2022.8.2/test/requirements.txt
--rw-r--r--   0 ruth       (501) staff       (20)     4595 2022-02-03 22:13:35.000000 gengive-2022.8.2/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     1420 2022-07-09 13:42:52.000000 gengive-2022.8.2/test/test_gengive.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-19 20:46:47.675721 gengive-2023.6.19/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 gengive-2023.6.19/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 gengive-2023.6.19/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3105 2023-06-19 20:46:47.675592 gengive-2023.6.19/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2085 2023-03-14 22:19:36.000000 gengive-2023.6.19/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-19 20:46:47.672808 gengive-2023.6.19/gengive/
+-rw-r--r--   0 ruth       (501) staff       (20)      749 2023-06-19 20:43:58.000000 gengive-2023.6.19/gengive/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      232 2022-01-11 20:35:11.000000 gengive-2023.6.19/gengive/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2556 2022-02-02 21:24:11.000000 gengive-2023.6.19/gengive/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)    20814 2022-02-03 22:09:48.000000 gengive-2023.6.19/gengive/gengive.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-19 20:46:47.674759 gengive-2023.6.19/gengive.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3105 2023-06-19 20:46:47.000000 gengive-2023.6.19/gengive.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)      344 2023-06-19 20:46:47.000000 gengive-2023.6.19/gengive.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-19 20:46:47.000000 gengive-2023.6.19/gengive.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       44 2023-06-19 20:46:47.000000 gengive-2023.6.19/gengive.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      133 2023-06-19 20:46:47.000000 gengive-2023.6.19/gengive.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        8 2023-06-19 20:46:47.000000 gengive-2023.6.19/gengive.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     2677 2023-06-19 20:23:55.000000 gengive-2023.6.19/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-19 20:46:47.675758 gengive-2023.6.19/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-19 20:46:47.675429 gengive-2023.6.19/test/
+-rw-r--r--   0 ruth       (501) staff       (20)     4595 2022-02-03 22:13:35.000000 gengive-2023.6.19/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1420 2022-07-09 13:42:52.000000 gengive-2023.6.19/test/test_gengive.py
```

### Comparing `gengive-2022.8.2/LICENSE` & `gengive-2023.6.19/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Stefan Hagen
+Copyright (c) 2023 Stefan Hagen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `gengive-2022.8.2/PKG-INFO` & `gengive-2023.6.19/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,69 @@
 Metadata-Version: 2.1
 Name: gengive
-Version: 2022.8.2
-Summary: Render text (Danish: gengive tekst)..
-Home-page: https://git.sr.ht/~sthagen/gengive
-Author: Stefan Hagen
-Author-email: stefan@hagen.link
-Maintainer: Stefan Hagen
-Maintainer-email: stefan@hagen.link
-Project-URL: Bug Tracker, https://todo.sr.ht/~sthagen/gengive
+Version: 2023.6.19
+Summary: Render text (Danish: gengive tekst).
+Author-email: Stefan Hagen <stefan@hagen.link>
+Maintainer-email: Stefan Hagen <stefan@hagen.link>
+Project-URL: Homepage, https://git.sr.ht/~sthagen/gengive
+Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/gengive
 Project-URL: Documentation, https://codes.dilettant.life/docs/gengive
-Project-URL: Source Code, https://git.sr.ht/~sthagen/gengive
-Project-URL: Test Coverage, https://codes.dilettant.life/coverage/gengive
-Keywords: markdown,developer-tools,verification
+Project-URL: Source-Code, https://git.sr.ht/~sthagen/gengive
+Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/gengive
+Keywords: developer-tools,markdown,verification
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# gengive
+# Gengive
 
 Render text (Danish: gengive tekst).
 
 [License: MIT](https://git.sr.ht/~sthagen/gengive/tree/default/item/LICENSE)
 
+Third party dependencies are documented in the folder [third-party](docs/third-party/README.md).
+
 [![version](https://img.shields.io/pypi/v/gengive.svg?style=flat)](https://pypi.python.org/pypi/gengive/)
 [![downloads](https://pepy.tech/badge/gengive/month)](https://pepy.tech/project/gengive)
 [![wheel](https://img.shields.io/pypi/wheel/gengive.svg?style=flat)](https://pypi.python.org/pypi/gengive/)
 [![supported-versions](https://img.shields.io/pypi/pyversions/gengive.svg?style=flat)](https://pypi.python.org/pypi/gengive/)
 [![supported-implementations](https://img.shields.io/pypi/implementation/gengive.svg?style=flat)](https://pypi.python.org/pypi/gengive/)
 
 ## Documentation
 
 User and developer [documentation of gengive](https://codes.dilettant.life/docs/gengive).
 
 ## Bug Tracker
 
-Feature requests and bug reports are bested entered in the [todos of gengive](https://todo.sr.ht/~sthagen/gengive).
+Any feature requests or bug reports shall go to the [todos of gengive](https://todo.sr.ht/~sthagen/gengive).
 
 ## Primary Source repository
 
-The primary source repository of [gengive is at sourcehut](https://git.sr.ht/~sthagen/gengive)
-a collection of tools useful for software development.
+The main source of `gengive` is on a mountain in central Switzerland.
+We use distributed version control (git).
+There is no central hub.
+Every clone can become a new source for the benefit of all.
+The preferred public clones of `gengive` are:
+
+* [on codeberg](https://codeberg.org/sthagen/gengive) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
+* [at sourcehut](https://git.sr.ht/~sthagen/gengive) - a collection of tools useful for software development.
+
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
 
 ## Status
 
 Experimental.
 
 **Note**: The default branch is `default`.
```

### Comparing `gengive-2022.8.2/gengive/__init__.py` & `gengive-2023.6.19/gengive/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 STRICT = bool(os.getenv(f'{APP_ENV}_STRICT', ''))
 ENCODING = 'utf-8'
 ENCODING_ERRORS_POLICY = 'ignore'
 DEFAULT_CONFIG_NAME = '.gengive.json'
 DEFAULT_LF_ONLY = 'YES'
 
 # [[[fill git_describe()]]]
-__version__ = '2022.8.2+parent.976ad259'
-# [[[end]]] (checksum: c8cf91bc8a2a034e7c3ce5d04db22cf0)
+__version__ = '2023.6.19+parent.365b32fd'
+# [[[end]]] (checksum: 9dc45f1fac14aaef6add1a675c4d9f13)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 __all__: List[str] = []
```

### Comparing `gengive-2022.8.2/gengive/cli.py` & `gengive-2023.6.19/gengive/cli.py`

 * *Files identical despite different names*

### Comparing `gengive-2022.8.2/gengive/gengive.py` & `gengive-2023.6.19/gengive/gengive.py`

 * *Files identical despite different names*

### Comparing `gengive-2022.8.2/gengive.egg-info/PKG-INFO` & `gengive-2023.6.19/gengive.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,69 @@
 Metadata-Version: 2.1
 Name: gengive
-Version: 2022.8.2
-Summary: Render text (Danish: gengive tekst)..
-Home-page: https://git.sr.ht/~sthagen/gengive
-Author: Stefan Hagen
-Author-email: stefan@hagen.link
-Maintainer: Stefan Hagen
-Maintainer-email: stefan@hagen.link
-Project-URL: Bug Tracker, https://todo.sr.ht/~sthagen/gengive
+Version: 2023.6.19
+Summary: Render text (Danish: gengive tekst).
+Author-email: Stefan Hagen <stefan@hagen.link>
+Maintainer-email: Stefan Hagen <stefan@hagen.link>
+Project-URL: Homepage, https://git.sr.ht/~sthagen/gengive
+Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/gengive
 Project-URL: Documentation, https://codes.dilettant.life/docs/gengive
-Project-URL: Source Code, https://git.sr.ht/~sthagen/gengive
-Project-URL: Test Coverage, https://codes.dilettant.life/coverage/gengive
-Keywords: markdown,developer-tools,verification
+Project-URL: Source-Code, https://git.sr.ht/~sthagen/gengive
+Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/gengive
+Keywords: developer-tools,markdown,verification
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# gengive
+# Gengive
 
 Render text (Danish: gengive tekst).
 
 [License: MIT](https://git.sr.ht/~sthagen/gengive/tree/default/item/LICENSE)
 
+Third party dependencies are documented in the folder [third-party](docs/third-party/README.md).
+
 [![version](https://img.shields.io/pypi/v/gengive.svg?style=flat)](https://pypi.python.org/pypi/gengive/)
 [![downloads](https://pepy.tech/badge/gengive/month)](https://pepy.tech/project/gengive)
 [![wheel](https://img.shields.io/pypi/wheel/gengive.svg?style=flat)](https://pypi.python.org/pypi/gengive/)
 [![supported-versions](https://img.shields.io/pypi/pyversions/gengive.svg?style=flat)](https://pypi.python.org/pypi/gengive/)
 [![supported-implementations](https://img.shields.io/pypi/implementation/gengive.svg?style=flat)](https://pypi.python.org/pypi/gengive/)
 
 ## Documentation
 
 User and developer [documentation of gengive](https://codes.dilettant.life/docs/gengive).
 
 ## Bug Tracker
 
-Feature requests and bug reports are bested entered in the [todos of gengive](https://todo.sr.ht/~sthagen/gengive).
+Any feature requests or bug reports shall go to the [todos of gengive](https://todo.sr.ht/~sthagen/gengive).
 
 ## Primary Source repository
 
-The primary source repository of [gengive is at sourcehut](https://git.sr.ht/~sthagen/gengive)
-a collection of tools useful for software development.
+The main source of `gengive` is on a mountain in central Switzerland.
+We use distributed version control (git).
+There is no central hub.
+Every clone can become a new source for the benefit of all.
+The preferred public clones of `gengive` are:
+
+* [on codeberg](https://codeberg.org/sthagen/gengive) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
+* [at sourcehut](https://git.sr.ht/~sthagen/gengive) - a collection of tools useful for software development.
+
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
 
 ## Status
 
 Experimental.
 
 **Note**: The default branch is `default`.
```

### Comparing `gengive-2022.8.2/test/test_cli.py` & `gengive-2023.6.19/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `gengive-2022.8.2/test/test_gengive.py` & `gengive-2023.6.19/test/test_gengive.py`

 * *Files identical despite different names*

