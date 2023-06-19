# Comparing `tmp/nxsconfigserver-db-1.10.3.tar.gz` & `tmp/nxsconfigserver-db-1.10.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nxsconfigserver-db-1.10.3.tar", last modified: Fri Oct 11 16:46:47 2019, max compression
+gzip compressed data, was "nxsconfigserver-db-1.10.4.tar", last modified: Mon Jun 19 06:38:21 2023, max compression
```

## Comparing `nxsconfigserver-db-1.10.3.tar` & `nxsconfigserver-db-1.10.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2019-10-11 16:46:47.000000 nxsconfigserver-db-1.10.3/
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2019-10-11 16:46:47.000000 nxsconfigserver-db-1.10.3/conf/
--rw-r--r--   0 jkotan   (15949) irc         (39)     1197 2015-02-16 13:04:15.000000 nxsconfigserver-db-1.10.3/conf/mysql_create.sql
--rw-r--r--   0 jkotan   (15949) irc         (39)    21056 2014-07-29 06:43:42.000000 nxsconfigserver-db-1.10.3/conf/my.cnf
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2014-07-29 06:43:42.000000 nxsconfigserver-db-1.10.3/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)      158 2016-07-04 14:03:04.000000 nxsconfigserver-db-1.10.3/setup.cfg
--rwxr-xr-x   0 jkotan   (15949) irc         (39)     2927 2019-10-11 16:44:55.000000 nxsconfigserver-db-1.10.3/setup.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2831 2019-10-11 16:44:41.000000 nxsconfigserver-db-1.10.3/README.rst
--rw-r--r--   0 jkotan   (15949) irc         (39)     4746 2019-10-11 16:46:47.000000 nxsconfigserver-db-1.10.3/PKG-INFO
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-19 06:38:21.057699 nxsconfigserver-db-1.10.4/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2014-07-29 06:43:42.000000 nxsconfigserver-db-1.10.4/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5864 2023-06-19 06:38:21.057699 nxsconfigserver-db-1.10.4/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3630 2023-02-01 13:28:18.120510 nxsconfigserver-db-1.10.4/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-19 06:38:21.057699 nxsconfigserver-db-1.10.4/conf/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    21056 2014-07-29 06:43:42.000000 nxsconfigserver-db-1.10.4/conf/my.cnf
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1197 2015-02-16 13:04:15.000000 nxsconfigserver-db-1.10.4/conf/mysql_create.sql
+-rw-r--r--   0 jkotan   (15949) irc         (39)      158 2016-07-04 14:03:04.000000 nxsconfigserver-db-1.10.4/setup.cfg
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)     3092 2023-06-19 06:38:02.321855 nxsconfigserver-db-1.10.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nxsconfigserver-db-1.10.3/conf/mysql_create.sql` & `nxsconfigserver-db-1.10.4/conf/mysql_create.sql`

 * *Files identical despite different names*

### Comparing `nxsconfigserver-db-1.10.3/conf/my.cnf` & `nxsconfigserver-db-1.10.4/conf/my.cnf`

 * *Files identical despite different names*

### Comparing `nxsconfigserver-db-1.10.3/COPYRIGHT` & `nxsconfigserver-db-1.10.4/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxsconfigserver-db-1.10.3/setup.py` & `nxsconfigserver-db-1.10.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     :param fname: readme file name
     """
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 #: (:obj:`str`) full release number
-release = '1.10.3'
+release = '1.10.4'
 #: (:obj:`str`) release verion number
 version = ".".join(release.split(".")[:2])
 #: (:obj:`str`) program name
 name = "NXSConfigServer-db"
 
 #: (:obj:`dict` <:obj:`str` , any >`) metadata for distutils
 SETUPDATA = dict(
@@ -65,16 +65,20 @@
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
     cmdclass={'build_sphinx': BuildDoc},
+    packages=[],
     command_options={
         'build_sphinx': {
             'project': ('setup.py', name),
             'version': ('setup.py', version),
             'release': ('setup.py', release)}},
     long_description=read('README.rst')
 )
```

### Comparing `nxsconfigserver-db-1.10.3/README.rst` & `nxsconfigserver-db-1.10.4/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,60 @@
 ===============================================================
 Welcome to NeXuS Configuration Server Database's documentation!
 ===============================================================
 
+|github workflow|
+|docs|
+|Pypi Version|
+|Python Versions|
+
+.. |github workflow| image:: https://github.com/nexdatas/nxsconfigserver-db/actions/workflows/tests.yml/badge.svg
+   :target: https://github.com/nexdatas/nxsconfigserver-db/actions
+   :alt:
+
+.. |docs| image:: https://img.shields.io/badge/Documentation-webpages-ADD8E6.svg
+   :target: https://nexdatas.github.io/nxsconfigserver-db/index.html
+   :alt:
+
+.. |Pypi Version| image:: https://img.shields.io/pypi/v/nxsconfigserver-db.svg
+                  :target: https://pypi.python.org/pypi/nxsconfigserver-db
+                  :alt:
+
+.. |Python Versions| image:: https://img.shields.io/pypi/pyversions/nxsconfigserver-db.svg
+                     :target: https://pypi.python.org/pypi/nxsconfigserver-db/
+                     :alt:
+
 
 Authors: Jan Kotanski, Eugen Wintersberger, Halil Pasic
 
 The package contains SQL files to create the MySQL database for Configuration Server.
 
 NeXuS Configuration Server is a Tango Server with its implementation based
 on a MySQL database. It allows to store XML configuration datasources
 and components. It also gives possibility to select mandatory components
 and perform the process of component merging.
 
-| Source code: https://github.com/nexdatas/configserver-db
-| Web page: https://nexdatas.github.io/configserver-db
+| Source code: https://github.com/nexdatas/nxsconfigserver-db
+| Web page: https://nexdatas.github.io/nxsconfigserver-db
 
 ------------
 Installation
 ------------
 
 Install the dependencies:
 
 |    MySQLdb, PyTango, sphinx
 
 From sources
 ^^^^^^^^^^^^
 
 Download the latest version of NeXuS Configuration Server from
 
-|     https://github.com/nexdatas/configserver
-|     https://github.com/nexdatas/configserver-db
+|     https://github.com/nexdatas/nxsconfigserver
+|     https://github.com/nexdatas/nxsconfigserver-db
 
 Extract the sources and run for both packages
 
 .. code-block:: console
 
 	  $ python setup.py install
```

### Comparing `nxsconfigserver-db-1.10.3/PKG-INFO` & `nxsconfigserver-db-1.10.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,68 @@
 Metadata-Version: 1.1
 Name: nxsconfigserver-db
-Version: 1.10.3
+Version: 1.10.4
 Summary: Configuration Server  DataBase
 Home-page: https://github.com/jkotan/nexdatas/nxsconfigserver-db
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: ===============================================================
         Welcome to NeXuS Configuration Server Database's documentation!
         ===============================================================
         
+        |github workflow|
+        |docs|
+        |Pypi Version|
+        |Python Versions|
+        
+        .. |github workflow| image:: https://github.com/nexdatas/nxsconfigserver-db/actions/workflows/tests.yml/badge.svg
+           :target: https://github.com/nexdatas/nxsconfigserver-db/actions
+           :alt:
+        
+        .. |docs| image:: https://img.shields.io/badge/Documentation-webpages-ADD8E6.svg
+           :target: https://nexdatas.github.io/nxsconfigserver-db/index.html
+           :alt:
+        
+        .. |Pypi Version| image:: https://img.shields.io/pypi/v/nxsconfigserver-db.svg
+                          :target: https://pypi.python.org/pypi/nxsconfigserver-db
+                          :alt:
+        
+        .. |Python Versions| image:: https://img.shields.io/pypi/pyversions/nxsconfigserver-db.svg
+                             :target: https://pypi.python.org/pypi/nxsconfigserver-db/
+                             :alt:
+        
         
         Authors: Jan Kotanski, Eugen Wintersberger, Halil Pasic
         
         The package contains SQL files to create the MySQL database for Configuration Server.
         
         NeXuS Configuration Server is a Tango Server with its implementation based
         on a MySQL database. It allows to store XML configuration datasources
         and components. It also gives possibility to select mandatory components
         and perform the process of component merging.
         
-        | Source code: https://github.com/nexdatas/configserver-db
-        | Web page: https://nexdatas.github.io/configserver-db
+        | Source code: https://github.com/nexdatas/nxsconfigserver-db
+        | Web page: https://nexdatas.github.io/nxsconfigserver-db
         
         ------------
         Installation
         ------------
         
         Install the dependencies:
         
         |    MySQLdb, PyTango, sphinx
         
         From sources
         ^^^^^^^^^^^^
         
         Download the latest version of NeXuS Configuration Server from
         
-        |     https://github.com/nexdatas/configserver
-        |     https://github.com/nexdatas/configserver-db
+        |     https://github.com/nexdatas/nxsconfigserver
+        |     https://github.com/nexdatas/nxsconfigserver-db
         
         Extract the sources and run for both packages
         
         .. code-block:: console
         
         	  $ python setup.py install
         
@@ -135,7 +156,10 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
```

