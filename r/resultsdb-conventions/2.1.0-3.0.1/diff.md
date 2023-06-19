# Comparing `tmp/resultsdb_conventions-2.1.0.tar.gz` & `tmp/resultsdb_conventions-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resultsdb_conventions-2.1.0.tar", last modified: Thu Aug 27 21:56:09 2020, from Unix
+gzip compressed data, was "resultsdb_conventions-3.0.1.tar", last modified: Mon Jun 19 17:20:38 2023, max compression
```

## Comparing `resultsdb_conventions-2.1.0.tar` & `resultsdb_conventions-3.0.1.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxr-x   0 adamw     (1001) adamw     (1001)        0 2020-08-27 21:56:09.550532 resultsdb_conventions-2.1.0/
--rw-rw-r--   0 adamw     (1001) adamw     (1001)      120 2017-02-16 21:47:56.000000 resultsdb_conventions-2.1.0/.gitignore
--rw-rw-r--   0 adamw     (1001) adamw     (1001)       29 2017-02-07 16:22:22.000000 resultsdb_conventions-2.1.0/.pylintrc
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     2191 2020-08-27 21:52:26.000000 resultsdb_conventions-2.1.0/CHANGELOG.md
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    35147 2017-02-16 21:47:56.000000 resultsdb_conventions-2.1.0/COPYING
--rw-rw-r--   0 adamw     (1001) adamw     (1001)       37 2017-02-16 21:47:56.000000 resultsdb_conventions-2.1.0/MANIFEST.in
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     4925 2020-08-27 21:56:09.550532 resultsdb_conventions-2.1.0/PKG-INFO
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     3610 2017-02-16 21:47:56.000000 resultsdb_conventions-2.1.0/README.md
--rw-rw-r--   0 adamw     (1001) adamw     (1001)       40 2018-02-27 19:19:02.000000 resultsdb_conventions-2.1.0/install.requires
--rwxrwxr-x   0 adamw     (1001) adamw     (1001)      989 2020-08-27 21:55:22.000000 resultsdb_conventions-2.1.0/release.sh
-drwxrwxr-x   0 adamw     (1001) adamw     (1001)        0 2020-08-27 21:56:09.549532 resultsdb_conventions-2.1.0/resultsdb_conventions/
--rw-rw-r--   0 adamw     (1001) adamw     (1001)      921 2020-08-27 21:55:46.000000 resultsdb_conventions-2.1.0/resultsdb_conventions/__init__.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     5822 2020-03-03 02:22:58.000000 resultsdb_conventions-2.1.0/resultsdb_conventions/base.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     4469 2020-03-03 02:22:58.000000 resultsdb_conventions-2.1.0/resultsdb_conventions/fedora.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     4080 2020-08-27 21:52:26.000000 resultsdb_conventions-2.1.0/resultsdb_conventions/fedoracoreos.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     1776 2020-03-03 02:22:58.000000 resultsdb_conventions-2.1.0/resultsdb_conventions/helpers.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     5321 2020-03-03 02:22:58.000000 resultsdb_conventions-2.1.0/resultsdb_conventions/prodmd.py
-drwxrwxr-x   0 adamw     (1001) adamw     (1001)        0 2020-08-27 21:56:09.549532 resultsdb_conventions-2.1.0/resultsdb_conventions.egg-info/
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     4925 2020-08-27 21:56:07.000000 resultsdb_conventions-2.1.0/resultsdb_conventions.egg-info/PKG-INFO
--rw-rw-r--   0 adamw     (1001) adamw     (1001)      629 2020-08-27 21:56:09.000000 resultsdb_conventions-2.1.0/resultsdb_conventions.egg-info/SOURCES.txt
--rw-rw-r--   0 adamw     (1001) adamw     (1001)        1 2020-08-27 21:56:07.000000 resultsdb_conventions-2.1.0/resultsdb_conventions.egg-info/dependency_links.txt
--rw-rw-r--   0 adamw     (1001) adamw     (1001)       58 2020-08-27 21:56:07.000000 resultsdb_conventions-2.1.0/resultsdb_conventions.egg-info/requires.txt
--rw-rw-r--   0 adamw     (1001) adamw     (1001)       22 2020-08-27 21:56:07.000000 resultsdb_conventions-2.1.0/resultsdb_conventions.egg-info/top_level.txt
--rw-rw-r--   0 adamw     (1001) adamw     (1001)       38 2020-08-27 21:56:09.550532 resultsdb_conventions-2.1.0/setup.cfg
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     2656 2020-08-27 21:55:46.000000 resultsdb_conventions-2.1.0/setup.py
-drwxrwxr-x   0 adamw     (1001) adamw     (1001)        0 2020-08-27 21:56:09.550532 resultsdb_conventions-2.1.0/tests/
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     7622 2017-02-24 23:57:25.000000 resultsdb_conventions-2.1.0/tests/test_fedora.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     3942 2020-08-27 21:52:19.000000 resultsdb_conventions-2.1.0/tests/test_fedoracoreos.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     2419 2017-02-21 03:10:42.000000 resultsdb_conventions-2.1.0/tests/test_helpers.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)       20 2017-02-16 21:47:56.000000 resultsdb_conventions-2.1.0/tests.requires
--rw-rw-r--   0 adamw     (1001) adamw     (1001)      442 2020-08-27 21:52:10.000000 resultsdb_conventions-2.1.0/tox.ini
--rw-rw-r--   0 adamw     (1001) adamw     (1001)       53 2017-02-16 21:47:56.000000 resultsdb_conventions-2.1.0/tox.requires
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 17:20:38.406517 resultsdb_conventions-3.0.1/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      120 2023-05-05 20:40:28.000000 resultsdb_conventions-3.0.1/.gitignore
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       29 2023-05-05 20:40:28.000000 resultsdb_conventions-3.0.1/.pylintrc
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     2656 2023-06-19 17:20:05.000000 resultsdb_conventions-3.0.1/CHANGELOG.md
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    35147 2023-05-05 20:40:28.000000 resultsdb_conventions-3.0.1/COPYING
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       37 2023-05-05 20:40:28.000000 resultsdb_conventions-3.0.1/MANIFEST.in
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     4160 2023-06-19 17:20:38.406517 resultsdb_conventions-3.0.1/PKG-INFO
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     3610 2023-05-05 20:40:28.000000 resultsdb_conventions-3.0.1/README.md
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       40 2023-05-05 20:40:28.000000 resultsdb_conventions-3.0.1/install.requires
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      334 2023-06-19 16:59:29.000000 resultsdb_conventions-3.0.1/pyproject.toml
+-rwxr-xr-x   0 adamw     (1000) adamw     (1000)      672 2023-06-19 17:13:51.000000 resultsdb_conventions-3.0.1/release.sh
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       38 2023-06-19 17:20:38.406517 resultsdb_conventions-3.0.1/setup.cfg
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     2116 2023-06-19 17:20:12.000000 resultsdb_conventions-3.0.1/setup.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 17:20:38.402517 resultsdb_conventions-3.0.1/src/
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 17:20:38.405517 resultsdb_conventions-3.0.1/src/resultsdb_conventions/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      912 2023-06-19 17:20:12.000000 resultsdb_conventions-3.0.1/src/resultsdb_conventions/__init__.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     5813 2023-05-05 20:40:28.000000 resultsdb_conventions-3.0.1/src/resultsdb_conventions/base.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     4606 2023-06-19 17:07:27.000000 resultsdb_conventions-3.0.1/src/resultsdb_conventions/fedora.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     4071 2023-05-05 20:40:28.000000 resultsdb_conventions-3.0.1/src/resultsdb_conventions/fedoracoreos.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     1767 2023-05-05 20:40:28.000000 resultsdb_conventions-3.0.1/src/resultsdb_conventions/helpers.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     5312 2023-05-05 20:40:28.000000 resultsdb_conventions-3.0.1/src/resultsdb_conventions/prodmd.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 17:20:38.406517 resultsdb_conventions-3.0.1/src/resultsdb_conventions.egg-info/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     4160 2023-06-19 17:20:38.000000 resultsdb_conventions-3.0.1/src/resultsdb_conventions.egg-info/PKG-INFO
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      688 2023-06-19 17:20:38.000000 resultsdb_conventions-3.0.1/src/resultsdb_conventions.egg-info/SOURCES.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)        1 2023-06-19 17:20:38.000000 resultsdb_conventions-3.0.1/src/resultsdb_conventions.egg-info/dependency_links.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       58 2023-06-19 17:20:38.000000 resultsdb_conventions-3.0.1/src/resultsdb_conventions.egg-info/requires.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       22 2023-06-19 17:20:38.000000 resultsdb_conventions-3.0.1/src/resultsdb_conventions.egg-info/top_level.txt
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 17:20:38.406517 resultsdb_conventions-3.0.1/tests/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     7617 2023-06-19 16:53:48.000000 resultsdb_conventions-3.0.1/tests/test_fedora.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     3933 2023-05-05 20:40:28.000000 resultsdb_conventions-3.0.1/tests/test_fedoracoreos.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     2410 2023-05-05 20:40:28.000000 resultsdb_conventions-3.0.1/tests/test_helpers.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       35 2023-06-19 17:02:56.000000 resultsdb_conventions-3.0.1/tests.requires
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      498 2023-06-19 16:58:17.000000 resultsdb_conventions-3.0.1/tox.ini
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       53 2023-05-05 20:40:28.000000 resultsdb_conventions-3.0.1/tox.requires
```

### Comparing `resultsdb_conventions-2.1.0/COPYING` & `resultsdb_conventions-3.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `resultsdb_conventions-2.1.0/PKG-INFO` & `resultsdb_conventions-3.0.1/src/resultsdb_conventions.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,50 @@
 Metadata-Version: 2.1
-Name: resultsdb_conventions
-Version: 2.1.0
+Name: resultsdb-conventions
+Version: 3.0.1
 Summary: Module for conveniently reporting to ResultsDB following conventions
 Home-page: https://pagure.io/fedora-qa/resultsdb_conventions
 Author: Adam Williamson
 Author-email: awilliam@redhat.com
 License: GPLv3+
-Description: resultsdb_conventions
-        =====================
-        
-        resultsdb_conventions is a Python library that represents various
-        conventions for reporting test results to
-        `ResultsDB <https://fedoraproject.org/wiki/ResultsDB>`__. It allows you
-        to report results easily and without a lot of boilerplate, and be
-        relatively confident their ResultsDB metadata will be consistent with
-        other results of the same basic nature.
-        
-        Installation
-        ------------
-        
-        resultsdb_conventions packages are available in the Fedora and
-        `EPEL <https://fedoraproject.org/wiki/EPEL>`__ 7 repositories. The core
-        package is ``python2-resultsdb_conventions``, and the ``fedora`` module
-        is in the package ``python2-resultsdb_conventions-fedora``. For other
-        distributions, or if you want to use the git code, you can simply make
-        the library available in the Python path for your consumer in some way,
-        or to install the library systemwide, just run
-        ``sudo python setup.py install``. You will need the ``cached-property``
-        library as well, and the ``fedfind`` library if you wish to use the
-        Fedora conventions (these are both packaged for Fedora and EPEL). For
-        actually submitting results, you will need the ``ResultsDBapi`` class
-        from the ``resultsdb_api`` module.
-        
-        resultsdb_conventions is intended to be compatible with Python 2.6+ and
-        current Python 3. Please report bugs if you find compatibility problems.
-        
-        Use
-        ---
-        
-        The simplest way to use resultsdb_conventions is to pick the ``Result``
-        subclass that most closely represents the kind of result you wish to
-        submit, instantiate it with appropriate arguments, get an instance of
-        ``ResultsDBapi``, and run the ``report()`` method. This will apply the
-        ‘default’ metadata for the result (based on the kind of result and the
-        args used for instantiation), and submit it to whichever ResultsDB you
-        got an API instance for. The ``Result`` subclasses should all document
-        their required and optional arguments.
-        
-        For simple modifications of the submitted result, you can simply adjust
-        the ``extradata`` property (which is just a dict of arbitrary string
-        key:value pairs that are passed to ResultsDB and stored as-is) after
-        getting the instance but before running ``report()``. You can also cause
-        the result to be added to more groups by including an iterable of group
-        dicts or UUID strings as the ``groups`` arg when instantiating the
-        result class, or by adjusting the instance’s ``groups`` property
-        directly.
-        
-        For more complex changes to the behaviour, you can of course start from
-        the most relevant class and create a subclass, then adjust things as
-        appropriate. The important conventions for how subclasses should be
-        implemented are documented in the ``Result`` class. If your subclass is
-        likely to have utility outside your project, you may want to submit a
-        pull request for it, so other projects can conveniently report results
-        according to the same conventions.
-        
-        A simple validation mechanism has been included, but currently none of
-        the included classes implements any significant validation. The
-        validation is intended to enforce the convention being encoded, not to
-        do fundamental checks on the validity of the result in ResultsDB terms;
-        ResultsDB will reject any outright invalid submission. Please consider
-        implementing validation for any pull requests you submit.
-        
-        Bugs, pull requests etc.
-        ------------------------
-        
-        You can file issues and pull requests on the `resultsdb_conventions
-        project <https://pagure.io/taskotron/resultsdb_conventions>`__ in
-        Pagure.
-        
-        Credits
-        -------
-        
-        Jan Sedlak and Josef Skladanka contributed valuable inspiration, ideas
-        and reviews.
-        
-        Licensing
-        ---------
-        
-        resultsdb_conventions is available under the GPL, version 3 or any later
-        version. A copy is included as COPYING.
-        
 Keywords: fedora rhel epel resultsdb test taskotron
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Provides-Extra: fedora
+License-File: COPYING
+
+# resultsdb_conventions
+
+resultsdb_conventions is a Python library that represents various conventions for reporting test results to [ResultsDB][1]. It allows you to report results easily and without a lot of boilerplate, and be relatively confident their ResultsDB metadata will be consistent with other results of the same basic nature.
+
+## Installation
+
+resultsdb_conventions packages are available in the Fedora and [EPEL][2] 7 repositories. The core package is `python2-resultsdb_conventions`, and the `fedora` module is in the package `python2-resultsdb_conventions-fedora`. For other distributions, or if you want to use the git code, you can simply make the library available in the Python path for your consumer in some way, or to install the library systemwide, just run `sudo python setup.py install`. You will need the `cached-property` library as well, and the `fedfind` library if you wish to use the Fedora conventions (these are both packaged for Fedora and EPEL). For actually submitting results, you will need the `ResultsDBapi` class from the `resultsdb_api` module.
+
+resultsdb_conventions is intended to be compatible with Python 2.6+ and current Python 3. Please report bugs if you find compatibility problems.
+
+## Use
+
+The simplest way to use resultsdb_conventions is to pick the `Result` subclass that most closely represents the kind of result you wish to submit, instantiate it with appropriate arguments, get an instance of `ResultsDBapi`, and run the `report()` method. This will apply the 'default' metadata for the result (based on the kind of result and the args used for instantiation), and submit it to whichever ResultsDB you got an API instance for. The `Result` subclasses should all document their required and optional arguments.
+
+For simple modifications of the submitted result, you can simply adjust the `extradata` property (which is just a dict of arbitrary string key:value pairs that are passed to ResultsDB and stored as-is) after getting the instance but before running `report()`. You can also cause the result to be added to more groups by including an iterable of group dicts or UUID strings as the `groups` arg when instantiating the result class, or by adjusting the instance's `groups` property directly.
+
+For more complex changes to the behaviour, you can of course start from the most relevant class and create a subclass, then adjust things as appropriate. The important conventions for how subclasses should be implemented are documented in the `Result` class. If your subclass is likely to have utility outside your project, you may want to submit a pull request for it, so other projects can conveniently report results according to the same conventions.
+
+A simple validation mechanism has been included, but currently none of the included classes implements any significant validation. The validation is intended to enforce the convention being encoded, not to do fundamental checks on the validity of the result in ResultsDB terms; ResultsDB will reject any outright invalid submission. Please consider implementing validation for any pull requests you submit.
+
+## Bugs, pull requests etc.
+
+You can file issues and pull requests on the [resultsdb_conventions project][3] in Pagure.
+
+## Credits
+
+Jan Sedlak and Josef Skladanka contributed valuable inspiration, ideas and reviews.
+
+## Licensing
+
+resultsdb_conventions is available under the GPL, version 3 or any later version. A copy is included as COPYING.
+
+[1]: https://fedoraproject.org/wiki/ResultsDB
+[2]: https://fedoraproject.org/wiki/EPEL
+[3]: https://pagure.io/taskotron/resultsdb_conventions
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `resultsdb_conventions-2.1.0/README.md` & `resultsdb_conventions-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `resultsdb_conventions-2.1.0/resultsdb_conventions/__init__.py` & `resultsdb_conventions-3.0.1/src/resultsdb_conventions/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) Red Hat Inc.
+# Copyright Red Hat
 #
 # resultsdb_conventions is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation, either version 3 of
 # the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -18,8 +18,8 @@
 """OO representation of conventions for reporting various types of
 result to ResultsDB.
 """
 
 from __future__ import unicode_literals
 from __future__ import print_function
 
-__version__ = "2.1.0"
+__version__ = "3.0.1"
```

### Comparing `resultsdb_conventions-2.1.0/resultsdb_conventions/base.py` & `resultsdb_conventions-3.0.1/src/resultsdb_conventions/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) Red Hat Inc.
+# Copyright Red Hat
 #
 # resultsdb_conventions is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation, either version 3 of
 # the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `resultsdb_conventions-2.1.0/resultsdb_conventions/fedora.py` & `resultsdb_conventions-3.0.1/src/resultsdb_conventions/fedora.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) Red Hat Inc.
+# Copyright Red Hat
 #
 # resultsdb_conventions is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation, either version 3 of
 # the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -39,16 +39,16 @@
 class FedoraComposeResult(ProductmdComposeResult):
     """Result from a test of a Fedora compose in general (not related
     to a specific deliverable). Functionally, just adds a URL to the
     compose group. Expects compose discovery from the compose ID, via
     fedfind: cid is the compose ID. May raise ValueError directly or
     via get_release.
     """
-    def __init__(self, cid, *args, **kwargs):
-        self.cid = cid
+    def __init__(self, locator, *args, **kwargs):
+        self._locator = locator
         composeinfo = self.ffrel.metadata['composeinfo']
         super(FedoraComposeResult, self).__init__(composeinfo, *args, **kwargs)
         self.conventions.append('fedora.compose')
 
     def default_groups(self):
         super(FedoraComposeResult, self).default_groups()
         # update the existing compose group with a URL
@@ -57,30 +57,32 @@
         except (ValueError, fedfind.exceptions.FedfindError):
             logger.warning("fedfind found no release for compose ID %s, compose group will have no URL", self.cid)
             return
 
     @cached_property
     def ffrel(self):
         """Cached instance of fedfind release object."""
-        return fedfind.release.get_release(cid=self.cid)
+        if self._locator.startswith("http"):
+            return fedfind.release.get_release(url=self._locator)
+        return fedfind.release.get_release(cid=self._locator)
 
 
 class FedoraImageResult(ProductmdImageResult, FedoraComposeResult):
     """Result from testing a specific image from a Fedora compose.
     filename is the image filename. cid is the compose ID (explicitly
     taken here as we need to use it before calling the parent class
     __init__). If imgdict is not provided, will use fedfind to find it
     from the filename.
     """
-    def __init__(self, filename, cid, imgdict=None, *args, **kwargs):
-        self.cid = cid
+    def __init__(self, filename, locator, imgdict=None, *args, **kwargs):
+        self._locator = locator
         self.filename = filename
         if not imgdict:
             imgdict = self.ffimg
-        super(FedoraImageResult, self).__init__(imgdict, cid, *args, **kwargs)
+        super(FedoraImageResult, self).__init__(imgdict, locator, *args, **kwargs)
         self.filename = filename
         self.conventions.append('fedora.image')
 
     @cached_property
     def ffimg(self):
         """Cached instance of fedfind image dict."""
         try:
```

### Comparing `resultsdb_conventions-2.1.0/resultsdb_conventions/fedoracoreos.py` & `resultsdb_conventions-3.0.1/src/resultsdb_conventions/fedoracoreos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) Red Hat Inc.
+# Copyright Red Hat
 #
 # resultsdb_conventions is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation, either version 3 of
 # the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `resultsdb_conventions-2.1.0/resultsdb_conventions/helpers.py` & `resultsdb_conventions-3.0.1/src/resultsdb_conventions/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) Red Hat Inc.
+# Copyright Red Hat
 #
 # resultsdb_conventions is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation, either version 3 of
 # the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `resultsdb_conventions-2.1.0/resultsdb_conventions/prodmd.py` & `resultsdb_conventions-3.0.1/src/resultsdb_conventions/prodmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) Red Hat Inc.
+# Copyright Red Hat
 #
 # resultsdb_conventions is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation, either version 3 of
 # the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `resultsdb_conventions-2.1.0/resultsdb_conventions.egg-info/PKG-INFO` & `resultsdb_conventions-3.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,50 @@
 Metadata-Version: 2.1
-Name: resultsdb-conventions
-Version: 2.1.0
+Name: resultsdb_conventions
+Version: 3.0.1
 Summary: Module for conveniently reporting to ResultsDB following conventions
 Home-page: https://pagure.io/fedora-qa/resultsdb_conventions
 Author: Adam Williamson
 Author-email: awilliam@redhat.com
 License: GPLv3+
-Description: resultsdb_conventions
-        =====================
-        
-        resultsdb_conventions is a Python library that represents various
-        conventions for reporting test results to
-        `ResultsDB <https://fedoraproject.org/wiki/ResultsDB>`__. It allows you
-        to report results easily and without a lot of boilerplate, and be
-        relatively confident their ResultsDB metadata will be consistent with
-        other results of the same basic nature.
-        
-        Installation
-        ------------
-        
-        resultsdb_conventions packages are available in the Fedora and
-        `EPEL <https://fedoraproject.org/wiki/EPEL>`__ 7 repositories. The core
-        package is ``python2-resultsdb_conventions``, and the ``fedora`` module
-        is in the package ``python2-resultsdb_conventions-fedora``. For other
-        distributions, or if you want to use the git code, you can simply make
-        the library available in the Python path for your consumer in some way,
-        or to install the library systemwide, just run
-        ``sudo python setup.py install``. You will need the ``cached-property``
-        library as well, and the ``fedfind`` library if you wish to use the
-        Fedora conventions (these are both packaged for Fedora and EPEL). For
-        actually submitting results, you will need the ``ResultsDBapi`` class
-        from the ``resultsdb_api`` module.
-        
-        resultsdb_conventions is intended to be compatible with Python 2.6+ and
-        current Python 3. Please report bugs if you find compatibility problems.
-        
-        Use
-        ---
-        
-        The simplest way to use resultsdb_conventions is to pick the ``Result``
-        subclass that most closely represents the kind of result you wish to
-        submit, instantiate it with appropriate arguments, get an instance of
-        ``ResultsDBapi``, and run the ``report()`` method. This will apply the
-        ‘default’ metadata for the result (based on the kind of result and the
-        args used for instantiation), and submit it to whichever ResultsDB you
-        got an API instance for. The ``Result`` subclasses should all document
-        their required and optional arguments.
-        
-        For simple modifications of the submitted result, you can simply adjust
-        the ``extradata`` property (which is just a dict of arbitrary string
-        key:value pairs that are passed to ResultsDB and stored as-is) after
-        getting the instance but before running ``report()``. You can also cause
-        the result to be added to more groups by including an iterable of group
-        dicts or UUID strings as the ``groups`` arg when instantiating the
-        result class, or by adjusting the instance’s ``groups`` property
-        directly.
-        
-        For more complex changes to the behaviour, you can of course start from
-        the most relevant class and create a subclass, then adjust things as
-        appropriate. The important conventions for how subclasses should be
-        implemented are documented in the ``Result`` class. If your subclass is
-        likely to have utility outside your project, you may want to submit a
-        pull request for it, so other projects can conveniently report results
-        according to the same conventions.
-        
-        A simple validation mechanism has been included, but currently none of
-        the included classes implements any significant validation. The
-        validation is intended to enforce the convention being encoded, not to
-        do fundamental checks on the validity of the result in ResultsDB terms;
-        ResultsDB will reject any outright invalid submission. Please consider
-        implementing validation for any pull requests you submit.
-        
-        Bugs, pull requests etc.
-        ------------------------
-        
-        You can file issues and pull requests on the `resultsdb_conventions
-        project <https://pagure.io/taskotron/resultsdb_conventions>`__ in
-        Pagure.
-        
-        Credits
-        -------
-        
-        Jan Sedlak and Josef Skladanka contributed valuable inspiration, ideas
-        and reviews.
-        
-        Licensing
-        ---------
-        
-        resultsdb_conventions is available under the GPL, version 3 or any later
-        version. A copy is included as COPYING.
-        
 Keywords: fedora rhel epel resultsdb test taskotron
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Provides-Extra: fedora
+License-File: COPYING
+
+# resultsdb_conventions
+
+resultsdb_conventions is a Python library that represents various conventions for reporting test results to [ResultsDB][1]. It allows you to report results easily and without a lot of boilerplate, and be relatively confident their ResultsDB metadata will be consistent with other results of the same basic nature.
+
+## Installation
+
+resultsdb_conventions packages are available in the Fedora and [EPEL][2] 7 repositories. The core package is `python2-resultsdb_conventions`, and the `fedora` module is in the package `python2-resultsdb_conventions-fedora`. For other distributions, or if you want to use the git code, you can simply make the library available in the Python path for your consumer in some way, or to install the library systemwide, just run `sudo python setup.py install`. You will need the `cached-property` library as well, and the `fedfind` library if you wish to use the Fedora conventions (these are both packaged for Fedora and EPEL). For actually submitting results, you will need the `ResultsDBapi` class from the `resultsdb_api` module.
+
+resultsdb_conventions is intended to be compatible with Python 2.6+ and current Python 3. Please report bugs if you find compatibility problems.
+
+## Use
+
+The simplest way to use resultsdb_conventions is to pick the `Result` subclass that most closely represents the kind of result you wish to submit, instantiate it with appropriate arguments, get an instance of `ResultsDBapi`, and run the `report()` method. This will apply the 'default' metadata for the result (based on the kind of result and the args used for instantiation), and submit it to whichever ResultsDB you got an API instance for. The `Result` subclasses should all document their required and optional arguments.
+
+For simple modifications of the submitted result, you can simply adjust the `extradata` property (which is just a dict of arbitrary string key:value pairs that are passed to ResultsDB and stored as-is) after getting the instance but before running `report()`. You can also cause the result to be added to more groups by including an iterable of group dicts or UUID strings as the `groups` arg when instantiating the result class, or by adjusting the instance's `groups` property directly.
+
+For more complex changes to the behaviour, you can of course start from the most relevant class and create a subclass, then adjust things as appropriate. The important conventions for how subclasses should be implemented are documented in the `Result` class. If your subclass is likely to have utility outside your project, you may want to submit a pull request for it, so other projects can conveniently report results according to the same conventions.
+
+A simple validation mechanism has been included, but currently none of the included classes implements any significant validation. The validation is intended to enforce the convention being encoded, not to do fundamental checks on the validity of the result in ResultsDB terms; ResultsDB will reject any outright invalid submission. Please consider implementing validation for any pull requests you submit.
+
+## Bugs, pull requests etc.
+
+You can file issues and pull requests on the [resultsdb_conventions project][3] in Pagure.
+
+## Credits
+
+Jan Sedlak and Josef Skladanka contributed valuable inspiration, ideas and reviews.
+
+## Licensing
+
+resultsdb_conventions is available under the GPL, version 3 or any later version. A copy is included as COPYING.
+
+[1]: https://fedoraproject.org/wiki/ResultsDB
+[2]: https://fedoraproject.org/wiki/EPEL
+[3]: https://pagure.io/taskotron/resultsdb_conventions
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `resultsdb_conventions-2.1.0/resultsdb_conventions.egg-info/SOURCES.txt` & `resultsdb_conventions-3.0.1/src/resultsdb_conventions.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 .gitignore
 .pylintrc
 CHANGELOG.md
 COPYING
 MANIFEST.in
 README.md
 install.requires
+pyproject.toml
 release.sh
 setup.py
 tests.requires
 tox.ini
 tox.requires
-resultsdb_conventions/__init__.py
-resultsdb_conventions/base.py
-resultsdb_conventions/fedora.py
-resultsdb_conventions/fedoracoreos.py
-resultsdb_conventions/helpers.py
-resultsdb_conventions/prodmd.py
-resultsdb_conventions.egg-info/PKG-INFO
-resultsdb_conventions.egg-info/SOURCES.txt
-resultsdb_conventions.egg-info/dependency_links.txt
-resultsdb_conventions.egg-info/requires.txt
-resultsdb_conventions.egg-info/top_level.txt
+src/resultsdb_conventions/__init__.py
+src/resultsdb_conventions/base.py
+src/resultsdb_conventions/fedora.py
+src/resultsdb_conventions/fedoracoreos.py
+src/resultsdb_conventions/helpers.py
+src/resultsdb_conventions/prodmd.py
+src/resultsdb_conventions.egg-info/PKG-INFO
+src/resultsdb_conventions.egg-info/SOURCES.txt
+src/resultsdb_conventions.egg-info/dependency_links.txt
+src/resultsdb_conventions.egg-info/requires.txt
+src/resultsdb_conventions.egg-info/top_level.txt
 tests/test_fedora.py
 tests/test_fedoracoreos.py
 tests/test_helpers.py
```

### Comparing `resultsdb_conventions-2.1.0/tests/test_fedora.py` & `resultsdb_conventions-3.0.1/tests/test_fedora.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) Red Hat Inc.
+# Copyright Red Hat
 #
 # resultsdb_conventions is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation, either version 3 of
 # the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -81,15 +81,15 @@
     @mock.patch.object(fedfind.release.RawhideNightly, 'metadata', METADATA01)
     def test_fedoraimage_basic(self):
         """This is just a pretty basic overall test that instantiates
         the most complex class, produces a result and checks its
         properties.
         """
         res = FedoraImageResult(
-            cid='Fedora-Rawhide-20170131.n.1',
+            locator='Fedora-Rawhide-20170131.n.1',
             filename='Fedora-Server-dvd-x86_64-Rawhide-20170131.n.1.iso',
             outcome='PASSED',
             tc_name='compose.some.test',
             note='note here',
             ref_url='https://www.job.link/',
             tc_url='https://www.test.case/',
             source='testsource'
```

### Comparing `resultsdb_conventions-2.1.0/tests/test_fedoracoreos.py` & `resultsdb_conventions-3.0.1/tests/test_fedoracoreos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) Red Hat Inc.
+# Copyright Red Hat
 #
 # resultsdb_conventions is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation, either version 3 of
 # the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `resultsdb_conventions-2.1.0/tests/test_helpers.py` & `resultsdb_conventions-3.0.1/tests/test_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) Red Hat Inc.
+# Copyright Red Hat
 #
 # resultsdb_conventions is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation, either version 3 of
 # the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

