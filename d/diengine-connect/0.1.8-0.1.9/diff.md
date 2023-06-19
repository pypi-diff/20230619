# Comparing `tmp/diengine-connect-0.1.8.tar.gz` & `tmp/diengine-connect-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diengine-connect-0.1.8.tar", last modified: Tue Apr 25 04:52:06 2023, max compression
+gzip compressed data, was "diengine-connect-0.1.9.tar", last modified: Mon Jun 19 11:08:40 2023, max compression
```

## Comparing `diengine-connect-0.1.8.tar` & `diengine-connect-0.1.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-25 04:52:06.133425 diengine-connect-0.1.8/
--rw-r--r--   0 xushihao   (501) staff       (20)    11389 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/LICENSE
--rw-r--r--   0 xushihao   (501) staff       (20)     1334 2023-04-25 04:52:06.133283 diengine-connect-0.1.8/PKG-INFO
--rw-r--r--   0 xushihao   (501) staff       (20)      313 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/README.md
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-25 04:52:06.123775 diengine-connect-0.1.8/diengine_connect/
--rw-r--r--   0 xushihao   (501) staff       (20)        5 2023-04-25 04:45:47.000000 diengine-connect-0.1.8/diengine_connect/VERSION
--rw-r--r--   0 xushihao   (501) staff       (20)      261 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/__init__.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-25 04:52:06.125315 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/
--rw-r--r--   0 xushihao   (501) staff       (20)      200 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/__init__.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-25 04:52:06.125830 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/datatypes/
--rw-r--r--   0 xushihao   (501) staff       (20)       57 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/datatypes/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     4768 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/datatypes/base.py
--rw-r--r--   0 xushihao   (501) staff       (20)    13573 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/datatypes/sqltypes.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-25 04:52:06.126268 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/ddl/
--rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/ddl/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1593 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/ddl/custom.py
--rw-r--r--   0 xushihao   (501) staff       (20)     7509 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/ddl/tableengine.py
--rw-r--r--   0 xushihao   (501) staff       (20)     3512 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/dialect.py
--rw-r--r--   0 xushihao   (501) staff       (20)     2435 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/inspector.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-25 04:52:06.126790 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/sql/
--rw-r--r--   0 xushihao   (501) staff       (20)      458 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/sql/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)      884 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/sql/ddlcompiler.py
--rw-r--r--   0 xushihao   (501) staff       (20)      281 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/sql/preparer.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-25 04:52:06.127229 diengine-connect-0.1.8/diengine_connect/cc_superset/
--rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/cc_superset/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1226 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/cc_superset/datatypes.py
--rw-r--r--   0 xushihao   (501) staff       (20)     8396 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/cc_superset/engine.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1987 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/common.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-25 04:52:06.128759 diengine-connect-0.1.8/diengine_connect/datatypes/
--rw-r--r--   0 xushihao   (501) staff       (20)      297 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/datatypes/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)    14598 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/datatypes/base.py
--rw-r--r--   0 xushihao   (501) staff       (20)     9226 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/datatypes/container.py
--rw-r--r--   0 xushihao   (501) staff       (20)     2548 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/datatypes/format.py
--rw-r--r--   0 xushihao   (501) staff       (20)     4643 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/datatypes/network.py
--rw-r--r--   0 xushihao   (501) staff       (20)    11138 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/datatypes/numeric.py
--rw-r--r--   0 xushihao   (501) staff       (20)     2326 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/datatypes/registry.py
--rw-r--r--   0 xushihao   (501) staff       (20)     3717 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/datatypes/special.py
--rw-r--r--   0 xushihao   (501) staff       (20)     5926 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/datatypes/string.py
--rw-r--r--   0 xushihao   (501) staff       (20)     8396 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/datatypes/temporal.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-25 04:52:06.129217 diengine-connect-0.1.8/diengine_connect/dbapi/
--rw-r--r--   0 xushihao   (501) staff       (20)      880 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/dbapi/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1525 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/dbapi/connection.py
--rw-r--r--   0 xushihao   (501) staff       (20)     4462 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/dbapi/cursor.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-25 04:52:06.132991 diengine-connect-0.1.8/diengine_connect/driver/
--rw-r--r--   0 xushihao   (501) staff       (20)     6640 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     4379 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/buffer.py
--rw-r--r--   0 xushihao   (501) staff       (20)    34594 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/client.py
--rw-r--r--   0 xushihao   (501) staff       (20)     6051 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/common.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1756 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/compression.py
--rw-r--r--   0 xushihao   (501) staff       (20)       80 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/constants.py
--rw-r--r--   0 xushihao   (501) staff       (20)     2410 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/context.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1306 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/ctypes.py
--rw-r--r--   0 xushihao   (501) staff       (20)     3466 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/dataconv.py
--rw-r--r--   0 xushihao   (501) staff       (20)      817 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/ddl.py
--rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/diengine.py
--rw-r--r--   0 xushihao   (501) staff       (20)     2832 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/exceptions.py
--rw-r--r--   0 xushihao   (501) staff       (20)     7170 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/extras.py
--rw-r--r--   0 xushihao   (501) staff       (20)    18955 2023-04-25 03:15:45.000000 diengine-connect-0.1.8/diengine_connect/driver/httpclient.py
--rw-r--r--   0 xushihao   (501) staff       (20)     6474 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/httputil.py
--rw-r--r--   0 xushihao   (501) staff       (20)     6974 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/insert.py
--rw-r--r--   0 xushihao   (501) staff       (20)      726 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/models.py
--rw-r--r--   0 xushihao   (501) staff       (20)      312 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/npconv.py
--rw-r--r--   0 xushihao   (501) staff       (20)     4232 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/npquery.py
--rw-r--r--   0 xushihao   (501) staff       (20)      682 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/options.py
--rw-r--r--   0 xushihao   (501) staff       (20)     5706 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/parser.py
--rw-r--r--   0 xushihao   (501) staff       (20)    19939 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/query.py
--rw-r--r--   0 xushihao   (501) staff       (20)      799 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/tools.py
--rw-r--r--   0 xushihao   (501) staff       (20)     5383 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/transform.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1011 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driver/types.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-25 04:52:06.133121 diengine-connect-0.1.8/diengine_connect/driverc/
--rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/driverc/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1294 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/entry_points.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1306 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/diengine_connect/json_impl.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-25 04:52:06.124719 diengine-connect-0.1.8/diengine_connect.egg-info/
--rw-r--r--   0 xushihao   (501) staff       (20)     1334 2023-04-25 04:52:06.000000 diengine-connect-0.1.8/diengine_connect.egg-info/PKG-INFO
--rw-r--r--   0 xushihao   (501) staff       (20)     2554 2023-04-25 04:52:06.000000 diengine-connect-0.1.8/diengine_connect.egg-info/SOURCES.txt
--rw-r--r--   0 xushihao   (501) staff       (20)        1 2023-04-25 04:52:06.000000 diengine-connect-0.1.8/diengine_connect.egg-info/dependency_links.txt
--rw-r--r--   0 xushihao   (501) staff       (20)      263 2023-04-25 04:52:06.000000 diengine-connect-0.1.8/diengine_connect.egg-info/entry_points.txt
--rw-r--r--   0 xushihao   (501) staff       (20)        1 2023-04-25 04:52:06.000000 diengine-connect-0.1.8/diengine_connect.egg-info/not-zip-safe
--rw-r--r--   0 xushihao   (501) staff       (20)      179 2023-04-25 04:52:06.000000 diengine-connect-0.1.8/diengine_connect.egg-info/requires.txt
--rw-r--r--   0 xushihao   (501) staff       (20)       17 2023-04-25 04:52:06.000000 diengine-connect-0.1.8/diengine_connect.egg-info/top_level.txt
--rw-r--r--   0 xushihao   (501) staff       (20)      192 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/pyproject.toml
--rw-r--r--   0 xushihao   (501) staff       (20)       38 2023-04-25 04:52:06.133467 diengine-connect-0.1.8/setup.cfg
--rw-r--r--   0 xushihao   (501) staff       (20)     3152 2023-04-23 08:56:23.000000 diengine-connect-0.1.8/setup.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-06-19 11:08:40.917472 diengine-connect-0.1.9/
+-rw-r--r--   0 xushihao   (501) staff       (20)    11389 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/LICENSE
+-rw-r--r--   0 xushihao   (501) staff       (20)     1334 2023-06-19 11:08:40.917336 diengine-connect-0.1.9/PKG-INFO
+-rw-r--r--   0 xushihao   (501) staff       (20)      313 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/README.md
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-06-19 11:08:40.907200 diengine-connect-0.1.9/diengine_connect/
+-rw-r--r--   0 xushihao   (501) staff       (20)        5 2023-06-19 11:08:39.000000 diengine-connect-0.1.9/diengine_connect/VERSION
+-rw-r--r--   0 xushihao   (501) staff       (20)      261 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/__init__.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-06-19 11:08:40.908864 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/
+-rw-r--r--   0 xushihao   (501) staff       (20)      200 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/__init__.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-06-19 11:08:40.909321 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/datatypes/
+-rw-r--r--   0 xushihao   (501) staff       (20)       57 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/datatypes/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     4768 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/datatypes/base.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    13573 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/datatypes/sqltypes.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-06-19 11:08:40.909734 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/ddl/
+-rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/ddl/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1593 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/ddl/custom.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     7509 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/ddl/tableengine.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     3508 2023-06-19 11:05:42.000000 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/dialect.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     2435 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/inspector.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-06-19 11:08:40.910223 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/sql/
+-rw-r--r--   0 xushihao   (501) staff       (20)      458 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/sql/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      884 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/sql/ddlcompiler.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      281 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/sql/preparer.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-06-19 11:08:40.910779 diengine-connect-0.1.9/diengine_connect/cc_superset/
+-rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/cc_superset/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1226 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/cc_superset/datatypes.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     8396 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/cc_superset/engine.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1987 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/common.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-06-19 11:08:40.912248 diengine-connect-0.1.9/diengine_connect/datatypes/
+-rw-r--r--   0 xushihao   (501) staff       (20)      297 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/datatypes/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    14598 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/datatypes/base.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     9226 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/datatypes/container.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     2548 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/datatypes/format.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     4643 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/datatypes/network.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    11138 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/datatypes/numeric.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     2326 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/datatypes/registry.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     3717 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/datatypes/special.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     5926 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/datatypes/string.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     8396 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/datatypes/temporal.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-06-19 11:08:40.912659 diengine-connect-0.1.9/diengine_connect/dbapi/
+-rw-r--r--   0 xushihao   (501) staff       (20)      880 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/dbapi/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1525 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/dbapi/connection.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     4462 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/dbapi/cursor.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-06-19 11:08:40.917002 diengine-connect-0.1.9/diengine_connect/driver/
+-rw-r--r--   0 xushihao   (501) staff       (20)     6640 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     4379 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/buffer.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    34594 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/client.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     6051 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/common.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1756 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/compression.py
+-rw-r--r--   0 xushihao   (501) staff       (20)       80 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/constants.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     2410 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/context.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1306 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/ctypes.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     3466 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/dataconv.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      817 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/ddl.py
+-rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/diengine.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     2832 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/exceptions.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     7170 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/extras.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    18955 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/httpclient.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     6474 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/httputil.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     6974 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/insert.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      726 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/models.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      312 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/npconv.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     4232 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/npquery.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      682 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/options.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     5706 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/parser.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    19939 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/query.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      799 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/tools.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     5383 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/transform.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1011 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driver/types.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-06-19 11:08:40.917144 diengine-connect-0.1.9/diengine_connect/driverc/
+-rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/driverc/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1294 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/entry_points.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1306 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/diengine_connect/json_impl.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-06-19 11:08:40.908321 diengine-connect-0.1.9/diengine_connect.egg-info/
+-rw-r--r--   0 xushihao   (501) staff       (20)     1334 2023-06-19 11:08:40.000000 diengine-connect-0.1.9/diengine_connect.egg-info/PKG-INFO
+-rw-r--r--   0 xushihao   (501) staff       (20)     2554 2023-06-19 11:08:40.000000 diengine-connect-0.1.9/diengine_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 xushihao   (501) staff       (20)        1 2023-06-19 11:08:40.000000 diengine-connect-0.1.9/diengine_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 xushihao   (501) staff       (20)      263 2023-06-19 11:08:40.000000 diengine-connect-0.1.9/diengine_connect.egg-info/entry_points.txt
+-rw-r--r--   0 xushihao   (501) staff       (20)        1 2023-04-25 04:52:06.000000 diengine-connect-0.1.9/diengine_connect.egg-info/not-zip-safe
+-rw-r--r--   0 xushihao   (501) staff       (20)      179 2023-06-19 11:08:40.000000 diengine-connect-0.1.9/diengine_connect.egg-info/requires.txt
+-rw-r--r--   0 xushihao   (501) staff       (20)       17 2023-06-19 11:08:40.000000 diengine-connect-0.1.9/diengine_connect.egg-info/top_level.txt
+-rw-r--r--   0 xushihao   (501) staff       (20)      192 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/pyproject.toml
+-rw-r--r--   0 xushihao   (501) staff       (20)       38 2023-06-19 11:08:40.917526 diengine-connect-0.1.9/setup.cfg
+-rw-r--r--   0 xushihao   (501) staff       (20)     3152 2023-05-18 04:11:27.000000 diengine-connect-0.1.9/setup.py
```

### Comparing `diengine-connect-0.1.8/LICENSE` & `diengine-connect-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/PKG-INFO` & `diengine-connect-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diengine-connect
-Version: 0.1.8
+Version: 0.1.9
 Summary: Diengine core driver, SqlAlchemy, and Superset libraries
 Home-page: UNKNOWN
 Author: diengine Inc.
 License: Apache License 2.0
 Description: ## Diengine Connect
         
         A suite of Python packages for connecting Python to Diengine:
```

### Comparing `diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/datatypes/base.py` & `diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/datatypes/sqltypes.py` & `diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/datatypes/sqltypes.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/ddl/custom.py` & `diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/ddl/custom.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/ddl/tableengine.py` & `diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/ddl/tableengine.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/dialect.py` & `diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,25 +34,25 @@
         return dbapi
 
     def initialize(self, connection):
         pass
 
     @staticmethod
     def get_schema_names(connection, **_):
-        return [row.name for row in connection.execute('SHOW DATABASES')]
+        return [row[0] for row in connection.execute('SHOW DATABASES')]
 
     @staticmethod
     def has_database(connection, db_name):
         return (connection.execute(f"SELECT name FROM system.databases WHERE name = '{db_name}'")).rowcount > 0
 
     def get_table_names(self, connection, schema=None, **kw):
         cmd = 'SHOW TABLES'
         if schema:
             cmd += ' FROM ' + schema
-        return [row.name for row in connection.execute(cmd)]
+        return [row[0] for row in connection.execute(cmd)]
 
     def get_primary_keys(self, connection, table_name, schema=None, **kw):
         return []
 
     def get_pk_constraint(self, conn, table_name, schema=None, **kw):
         return []
```

### Comparing `diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/inspector.py` & `diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/inspector.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/cc_sqlalchemy/sql/ddlcompiler.py` & `diengine-connect-0.1.9/diengine_connect/cc_sqlalchemy/sql/ddlcompiler.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/cc_superset/datatypes.py` & `diengine-connect-0.1.9/diengine_connect/cc_superset/datatypes.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/cc_superset/engine.py` & `diengine-connect-0.1.9/diengine_connect/cc_superset/engine.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/common.py` & `diengine-connect-0.1.9/diengine_connect/common.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/datatypes/base.py` & `diengine-connect-0.1.9/diengine_connect/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/datatypes/container.py` & `diengine-connect-0.1.9/diengine_connect/datatypes/container.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/datatypes/format.py` & `diengine-connect-0.1.9/diengine_connect/datatypes/format.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/datatypes/network.py` & `diengine-connect-0.1.9/diengine_connect/datatypes/network.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/datatypes/numeric.py` & `diengine-connect-0.1.9/diengine_connect/datatypes/numeric.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/datatypes/registry.py` & `diengine-connect-0.1.9/diengine_connect/datatypes/registry.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/datatypes/special.py` & `diengine-connect-0.1.9/diengine_connect/datatypes/special.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/datatypes/string.py` & `diengine-connect-0.1.9/diengine_connect/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/datatypes/temporal.py` & `diengine-connect-0.1.9/diengine_connect/datatypes/temporal.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/dbapi/__init__.py` & `diengine-connect-0.1.9/diengine_connect/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/dbapi/connection.py` & `diengine-connect-0.1.9/diengine_connect/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/dbapi/cursor.py` & `diengine-connect-0.1.9/diengine_connect/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/__init__.py` & `diengine-connect-0.1.9/diengine_connect/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/buffer.py` & `diengine-connect-0.1.9/diengine_connect/driver/buffer.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/client.py` & `diengine-connect-0.1.9/diengine_connect/driver/client.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/common.py` & `diengine-connect-0.1.9/diengine_connect/driver/common.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/compression.py` & `diengine-connect-0.1.9/diengine_connect/driver/compression.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/context.py` & `diengine-connect-0.1.9/diengine_connect/driver/context.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/ctypes.py` & `diengine-connect-0.1.9/diengine_connect/driver/ctypes.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/dataconv.py` & `diengine-connect-0.1.9/diengine_connect/driver/dataconv.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/ddl.py` & `diengine-connect-0.1.9/diengine_connect/driver/ddl.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/exceptions.py` & `diengine-connect-0.1.9/diengine_connect/driver/exceptions.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/extras.py` & `diengine-connect-0.1.9/diengine_connect/driver/extras.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/httpclient.py` & `diengine-connect-0.1.9/diengine_connect/driver/httpclient.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/httputil.py` & `diengine-connect-0.1.9/diengine_connect/driver/httputil.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/insert.py` & `diengine-connect-0.1.9/diengine_connect/driver/insert.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/models.py` & `diengine-connect-0.1.9/diengine_connect/driver/models.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/npquery.py` & `diengine-connect-0.1.9/diengine_connect/driver/npquery.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/options.py` & `diengine-connect-0.1.9/diengine_connect/driver/options.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/parser.py` & `diengine-connect-0.1.9/diengine_connect/driver/parser.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/query.py` & `diengine-connect-0.1.9/diengine_connect/driver/query.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/tools.py` & `diengine-connect-0.1.9/diengine_connect/driver/tools.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/transform.py` & `diengine-connect-0.1.9/diengine_connect/driver/transform.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/driver/types.py` & `diengine-connect-0.1.9/diengine_connect/driver/types.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/entry_points.py` & `diengine-connect-0.1.9/diengine_connect/entry_points.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect/json_impl.py` & `diengine-connect-0.1.9/diengine_connect/json_impl.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/diengine_connect.egg-info/PKG-INFO` & `diengine-connect-0.1.9/diengine_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diengine-connect
-Version: 0.1.8
+Version: 0.1.9
 Summary: Diengine core driver, SqlAlchemy, and Superset libraries
 Home-page: UNKNOWN
 Author: diengine Inc.
 License: Apache License 2.0
 Description: ## Diengine Connect
         
         A suite of Python packages for connecting Python to Diengine:
```

### Comparing `diengine-connect-0.1.8/diengine_connect.egg-info/SOURCES.txt` & `diengine-connect-0.1.9/diengine_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.1.8/setup.py` & `diengine-connect-0.1.9/setup.py`

 * *Files identical despite different names*

