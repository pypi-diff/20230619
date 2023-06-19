# Comparing `tmp/Chameleon-4.0.0.tar.gz` & `tmp/Chameleon-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chameleon-4.0.0.tar", last modified: Mon Mar  6 18:06:09 2023, max compression
+gzip compressed data, was "Chameleon-4.0.1.tar", last modified: Mon Jun 19 05:47:35 2023, max compression
```

## Comparing `Chameleon-4.0.0.tar` & `Chameleon-4.0.1.tar`

### file list

```diff
@@ -1,45 +1,422 @@
-drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-03-06 18:06:09.917778 Chameleon-4.0.0/
--rw-r--r--   0 mborch     (503) staff       (20)    44312 2023-03-06 18:05:51.000000 Chameleon-4.0.0/CHANGES.rst
--rw-r--r--   0 mborch     (503) staff       (20)      210 2023-03-06 17:34:13.000000 Chameleon-4.0.0/COPYRIGHT.txt
--rw-r--r--   0 mborch     (503) staff       (20)     8499 2023-03-06 17:34:13.000000 Chameleon-4.0.0/LICENSE.txt
--rw-r--r--   0 mborch     (503) staff       (20)      478 2023-03-06 18:02:45.000000 Chameleon-4.0.0/MANIFEST.in
--rw-r--r--   0 mborch     (503) staff       (20)     3135 2023-03-06 17:34:13.000000 Chameleon-4.0.0/Makefile
--rw-r--r--   0 mborch     (503) staff       (20)    46043 2023-03-06 18:06:09.917846 Chameleon-4.0.0/PKG-INFO
--rw-r--r--   0 mborch     (503) staff       (20)      642 2023-03-06 18:05:51.000000 Chameleon-4.0.0/README.rst
--rw-r--r--   0 mborch     (503) staff       (20)      499 2023-03-06 18:06:09.918117 Chameleon-4.0.0/setup.cfg
--rw-r--r--   0 mborch     (503) staff       (20)     2355 2023-03-06 18:03:40.000000 Chameleon-4.0.0/setup.py
-drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-03-06 18:06:09.908445 Chameleon-4.0.0/src/
-drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-03-06 18:06:09.913041 Chameleon-4.0.0/src/Chameleon.egg-info/
--rw-r--r--   0 mborch     (503) staff       (20)    46043 2023-03-06 18:06:09.000000 Chameleon-4.0.0/src/Chameleon.egg-info/PKG-INFO
--rw-r--r--   0 mborch     (503) staff       (20)      939 2023-03-06 18:06:09.000000 Chameleon-4.0.0/src/Chameleon.egg-info/SOURCES.txt
--rw-r--r--   0 mborch     (503) staff       (20)        1 2023-03-06 18:06:09.000000 Chameleon-4.0.0/src/Chameleon.egg-info/dependency_links.txt
--rw-r--r--   0 mborch     (503) staff       (20)        1 2023-03-06 17:34:32.000000 Chameleon-4.0.0/src/Chameleon.egg-info/not-zip-safe
--rw-r--r--   0 mborch     (503) staff       (20)       32 2023-03-06 18:06:09.000000 Chameleon-4.0.0/src/Chameleon.egg-info/requires.txt
--rw-r--r--   0 mborch     (503) staff       (20)       10 2023-03-06 18:06:09.000000 Chameleon-4.0.0/src/Chameleon.egg-info/top_level.txt
-drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-03-06 18:06:09.916780 Chameleon-4.0.0/src/chameleon/
--rw-r--r--   0 mborch     (503) staff       (20)      264 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/__init__.py
--rw-r--r--   0 mborch     (503) staff       (20)    31013 2023-03-06 17:53:57.000000 Chameleon-4.0.0/src/chameleon/astutil.py
--rw-r--r--   0 mborch     (503) staff       (20)    15138 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/benchmark.py
--rw-r--r--   0 mborch     (503) staff       (20)     6194 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/codegen.py
--rw-r--r--   0 mborch     (503) staff       (20)      421 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/compat.py
--rw-r--r--   0 mborch     (503) staff       (20)    54941 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/compiler.py
--rw-r--r--   0 mborch     (503) staff       (20)     1871 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/config.py
--rw-r--r--   0 mborch     (503) staff       (20)     8728 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/exc.py
--rw-r--r--   0 mborch     (503) staff       (20)     3762 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/i18n.py
--rw-r--r--   0 mborch     (503) staff       (20)     2707 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/interfaces.py
--rw-r--r--   0 mborch     (503) staff       (20)     4960 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/loader.py
--rw-r--r--   0 mborch     (503) staff       (20)      786 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/metal.py
--rw-r--r--   0 mborch     (503) staff       (20)      405 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/namespaces.py
--rw-r--r--   0 mborch     (503) staff       (20)     4282 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/nodes.py
--rw-r--r--   0 mborch     (503) staff       (20)     7368 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/parser.py
--rw-r--r--   0 mborch     (503) staff       (20)     1049 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/program.py
--rw-r--r--   0 mborch     (503) staff       (20)    12297 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/tal.py
--rw-r--r--   0 mborch     (503) staff       (20)    16556 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/tales.py
--rw-r--r--   0 mborch     (503) staff       (20)    10838 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/template.py
--rw-r--r--   0 mborch     (503) staff       (20)     4296 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/tokenize.py
--rw-r--r--   0 mborch     (503) staff       (20)    10859 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/utils.py
-drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-03-06 18:06:09.917645 Chameleon-4.0.0/src/chameleon/zpt/
--rw-r--r--   0 mborch     (503) staff       (20)        2 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/zpt/__init__.py
--rw-r--r--   0 mborch     (503) staff       (20)      798 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/zpt/loader.py
--rw-r--r--   0 mborch     (503) staff       (20)    27911 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/zpt/program.py
--rw-r--r--   0 mborch     (503) staff       (20)    13867 2023-03-06 17:34:13.000000 Chameleon-4.0.0/src/chameleon/zpt/template.py
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-06-19 05:47:35.344384 Chameleon-4.0.1/
+-rw-r--r--   0 mborch     (503) staff       (20)    44574 2023-06-19 05:46:59.000000 Chameleon-4.0.1/CHANGES.rst
+-rw-r--r--   0 mborch     (503) staff       (20)      210 2023-03-06 17:34:13.000000 Chameleon-4.0.1/COPYRIGHT.txt
+-rw-r--r--   0 mborch     (503) staff       (20)     8496 2023-06-17 15:00:31.000000 Chameleon-4.0.1/LICENSE.txt
+-rw-r--r--   0 mborch     (503) staff       (20)      478 2023-03-06 18:02:45.000000 Chameleon-4.0.1/MANIFEST.in
+-rw-r--r--   0 mborch     (503) staff       (20)     3135 2023-03-06 17:34:13.000000 Chameleon-4.0.1/Makefile
+-rw-r--r--   0 mborch     (503) staff       (20)    46291 2023-06-19 05:47:35.344477 Chameleon-4.0.1/PKG-INFO
+-rw-r--r--   0 mborch     (503) staff       (20)      628 2023-06-17 15:00:31.000000 Chameleon-4.0.1/README.rst
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-06-19 05:47:35.272855 Chameleon-4.0.1/benchmarks/
+-rw-r--r--   0 mborch     (503) staff       (20)     4039 2023-03-06 18:09:14.000000 Chameleon-4.0.1/benchmarks/bm_chameleon.py
+-rw-r--r--   0 mborch     (503) staff       (20)     3874 2023-06-17 15:00:31.000000 Chameleon-4.0.1/benchmarks/bm_mako.py
+-rw-r--r--   0 mborch     (503) staff       (20)     1869 2023-06-17 15:00:31.000000 Chameleon-4.0.1/benchmarks/util.py
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-06-19 05:47:35.275101 Chameleon-4.0.1/docs/
+-rw-r--r--   0 mborch     (503) staff       (20)     6742 2023-03-06 18:09:14.000000 Chameleon-4.0.1/docs/conf.py
+-rw-r--r--   0 mborch     (503) staff       (20)     1101 2023-03-06 18:09:14.000000 Chameleon-4.0.1/docs/configuration.rst
+-rw-r--r--   0 mborch     (503) staff       (20)     7194 2023-03-06 18:09:14.000000 Chameleon-4.0.1/docs/index.rst
+-rw-r--r--   0 mborch     (503) staff       (20)     1393 2023-03-06 18:09:14.000000 Chameleon-4.0.1/docs/integration.rst
+-rw-r--r--   0 mborch     (503) staff       (20)     5563 2023-03-06 18:09:14.000000 Chameleon-4.0.1/docs/library.rst
+-rw-r--r--   0 mborch     (503) staff       (20)    53547 2023-06-17 15:00:31.000000 Chameleon-4.0.1/docs/reference.rst
+-rw-r--r--   0 mborch     (503) staff       (20)       15 2023-03-06 18:09:14.000000 Chameleon-4.0.1/docs/requirements.txt
+-rw-r--r--   0 mborch     (503) staff       (20)      505 2023-06-19 05:47:35.345080 Chameleon-4.0.1/setup.cfg
+-rw-r--r--   0 mborch     (503) staff       (20)     2336 2023-06-19 05:46:07.000000 Chameleon-4.0.1/setup.py
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-06-19 05:47:35.269798 Chameleon-4.0.1/src/
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-06-19 05:47:35.276084 Chameleon-4.0.1/src/Chameleon.egg-info/
+-rw-r--r--   0 mborch     (503) staff       (20)    46291 2023-06-19 05:47:35.000000 Chameleon-4.0.1/src/Chameleon.egg-info/PKG-INFO
+-rw-r--r--   0 mborch     (503) staff       (20)    15803 2023-06-19 05:47:35.000000 Chameleon-4.0.1/src/Chameleon.egg-info/SOURCES.txt
+-rw-r--r--   0 mborch     (503) staff       (20)        1 2023-06-19 05:47:35.000000 Chameleon-4.0.1/src/Chameleon.egg-info/dependency_links.txt
+-rw-r--r--   0 mborch     (503) staff       (20)        1 2023-03-06 17:34:32.000000 Chameleon-4.0.1/src/Chameleon.egg-info/not-zip-safe
+-rw-r--r--   0 mborch     (503) staff       (20)       32 2023-06-19 05:47:35.000000 Chameleon-4.0.1/src/Chameleon.egg-info/requires.txt
+-rw-r--r--   0 mborch     (503) staff       (20)       10 2023-06-19 05:47:35.000000 Chameleon-4.0.1/src/Chameleon.egg-info/top_level.txt
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-06-19 05:47:35.279827 Chameleon-4.0.1/src/chameleon/
+-rw-r--r--   0 mborch     (503) staff       (20)      264 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/__init__.py
+-rw-r--r--   0 mborch     (503) staff       (20)    31041 2023-06-19 05:46:42.000000 Chameleon-4.0.1/src/chameleon/astutil.py
+-rw-r--r--   0 mborch     (503) staff       (20)    15077 2023-06-17 15:00:31.000000 Chameleon-4.0.1/src/chameleon/benchmark.py
+-rw-r--r--   0 mborch     (503) staff       (20)     6194 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/codegen.py
+-rw-r--r--   0 mborch     (503) staff       (20)    54941 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/compiler.py
+-rw-r--r--   0 mborch     (503) staff       (20)     1871 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/config.py
+-rw-r--r--   0 mborch     (503) staff       (20)     8729 2023-06-17 15:00:31.000000 Chameleon-4.0.1/src/chameleon/exc.py
+-rw-r--r--   0 mborch     (503) staff       (20)     3762 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/i18n.py
+-rw-r--r--   0 mborch     (503) staff       (20)     2707 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/interfaces.py
+-rw-r--r--   0 mborch     (503) staff       (20)     4960 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/loader.py
+-rw-r--r--   0 mborch     (503) staff       (20)      786 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/metal.py
+-rw-r--r--   0 mborch     (503) staff       (20)      405 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/namespaces.py
+-rw-r--r--   0 mborch     (503) staff       (20)     4282 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/nodes.py
+-rw-r--r--   0 mborch     (503) staff       (20)     7368 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/parser.py
+-rw-r--r--   0 mborch     (503) staff       (20)     1049 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/program.py
+-rw-r--r--   0 mborch     (503) staff       (20)    12297 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/tal.py
+-rw-r--r--   0 mborch     (503) staff       (20)    16558 2023-06-17 15:00:31.000000 Chameleon-4.0.1/src/chameleon/tales.py
+-rw-r--r--   0 mborch     (503) staff       (20)    10838 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/template.py
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-06-19 05:47:35.281380 Chameleon-4.0.1/src/chameleon/tests/
+-rw-r--r--   0 mborch     (503) staff       (20)        2 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/__init__.py
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-06-19 05:47:35.325986 Chameleon-4.0.1/src/chameleon/tests/inputs/
+-rw-r--r--   0 mborch     (503) staff       (20)       22 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/001-interpolation.txt
+-rw-r--r--   0 mborch     (503) staff       (20)      115 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/001-variable-scope.html
+-rw-r--r--   0 mborch     (503) staff       (20)      207 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/001-variable-scope.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       60 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/001.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      217 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/002-repeat-scope.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       61 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/002.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      506 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/003-content.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       61 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/003.xml
+-rw-r--r--   0 mborch     (503) staff       (20)     1337 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/004-attributes.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      102 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/004.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      444 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/005-default.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      104 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/005.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      399 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/006-attribute-interpolation.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      102 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/006.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      431 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/007-content-interpolation.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       65 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/007.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      411 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/008-builtins.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       85 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/008.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       49 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/009-literals.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       66 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/009.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      317 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/010-structure.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      103 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/010.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      235 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/011-messages.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      128 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/011.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      567 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/012-translation.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      100 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/012.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      173 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/013-repeat-nested.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      124 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/013.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      130 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/014-repeat-nested-similar.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      150 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/014.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      202 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/015-translation-nested.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      150 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/015.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      406 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/016-explicit-translation.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       66 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/016.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      366 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/017-omit-tag.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       83 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/017.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      430 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/018-translation-nested-dynamic.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       77 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/018.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      381 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/019-replace.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       74 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/019.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      392 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/020-on-error.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       77 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/020.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      387 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/021-translation-domain.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       78 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/021.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      566 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/022-switch.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       80 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/022.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      170 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/023-condition.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       79 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/023.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      258 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/024-namespace-elements.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      116 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/024.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      489 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/025-repeat-whitespace.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      100 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/025.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      605 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/026-repeat-variable.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       96 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/026.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      432 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/027-attribute-replacement.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       94 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/027.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      256 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/028-attribute-toggle.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       83 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/028.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      206 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/029-attribute-ordering.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       83 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/029.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      137 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/030-repeat-tuples.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       85 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/030.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      236 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/031-namespace-with-tal.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      100 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/031.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      617 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/032-master-template.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      100 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/032.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       73 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/033-use-macro-trivial.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      117 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/033.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       57 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/034-use-template-as-macro.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       55 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/034.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      165 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/035-use-macro-with-fill-slot.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       56 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/035.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      115 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/036-use-macro-inherits-dynamic-scope.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       73 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/036.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      195 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/037-use-macro-local-variable-scope.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       80 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/037.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      140 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/038-use-macro-globals.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       80 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/038.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       44 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/039-globals.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       73 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/039.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      863 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/040-macro-using-template-symbol.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      125 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/040.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      501 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/041-translate-nested-names.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      105 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/041.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      144 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/042-use-macro-fill-footer.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       98 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/042.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      396 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/043-macro-nested-dynamic-vars.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      108 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/043.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       78 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/044-tuple-define.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      187 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/044.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      551 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/045-namespaces.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      120 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/045.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      229 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/046-extend-macro.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      120 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/046.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      122 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/047-use-extended-macro.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       64 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/047.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      158 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/048-use-extended-macro-fill-original.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       61 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/048.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      455 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/049-entities-in-attributes.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      124 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/049.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      188 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/050-define-macro-and-use-not-extend.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      132 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/050.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      183 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/051-use-non-extended-macro.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      140 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/051.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      258 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/052-i18n-domain-inside-filled-slot.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       68 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/052.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      120 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/053-special-characters-in-attributes.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       97 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/053.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      100 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/054-import-expression.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       72 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/054.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       98 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/055-attribute-fallback-to-dict-lookup.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       74 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/055.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      104 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/056-comment-attribute.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      104 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/056.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      202 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/057-order.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       55 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/057.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      378 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/058-script.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      111 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/058.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      174 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/059-embedded-javascript.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      227 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/059.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      223 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/060-macro-with-multiple-same-slots.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       67 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/060.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      152 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/061-fill-one-slot-but-two-defined.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       66 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/061.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      372 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/062-comments-and-expressions.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       87 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/062.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       67 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/063-continuation.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      108 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/063.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       69 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/064-tags-and-special-characters.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       79 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/064.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      276 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/065-use-macro-in-fill.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       81 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/065.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       85 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/066-load-expression.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      155 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/066.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      201 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/067-attribute-decode.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       65 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/067.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      210 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/068-less-than-greater-than-in-attributes.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       84 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/068.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      167 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/069-translation-domain-and-macro.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       93 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/069.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      167 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/070-translation-domain-and-use-macro.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       81 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/070.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      555 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/071-html-attribute-defaults.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       90 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/071.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      251 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/072-repeat-interpolation.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       93 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/072.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      147 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/073-utf8-encoded.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       94 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/073.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      169 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/074-encoded-template.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       94 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/074.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      282 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/075-nested-macros.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       96 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/075.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      138 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/076-nested-macro-override.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      192 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/076.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      104 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/077-i18n-attributes.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       93 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/077.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      798 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/078-tags-and-newlines.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      100 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/078.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      420 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/079-implicit-i18n.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      101 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/079.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      250 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/080-xmlns-namespace-on-tal.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       95 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/080.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       70 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/081-load-spec.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      140 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/081.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       98 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/082-load-spec-computed.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       90 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/082.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      100 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/083-template-dict-to-macro.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      101 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/083.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      121 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/084-interpolation-in-cdata.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       54 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/084.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      309 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/085-nested-translation.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      102 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/085.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      251 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/086-self-closing.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      100 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/086.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      443 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/087-code-blocks.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      107 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/087.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       63 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/088-python-newlines.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       87 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/088.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      124 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/089-load-fallback.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      108 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/089.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      289 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/090-tuple-expression.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      150 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/090.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       75 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/091-repeat-none.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      181 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/091.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      102 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/092.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       60 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/093.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      112 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/094.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      141 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/095.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       99 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/096.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      157 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/097.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       71 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/098.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      100 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/099.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      101 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/100.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       67 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/101-unclosed-tags.html
+-rw-r--r--   0 mborch     (503) staff       (20)       81 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/101.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       84 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/102-unquoted-attributes.html
+-rw-r--r--   0 mborch     (503) staff       (20)      103 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/102.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      208 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/103-simple-attribute.html
+-rw-r--r--   0 mborch     (503) staff       (20)       69 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/103.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      101 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/104.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      104 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/105.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      105 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/106.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      105 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/107.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      121 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/108.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       98 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/109.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      129 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/110.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      123 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/111.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       89 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/112.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       91 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/113.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       96 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/114.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      103 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/115.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       74 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/116.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       86 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/117.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       87 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/118.xml
+-rw-r--r--   0 mborch     (503) staff       (20)       66 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/119.xml
+-rw-r--r--   0 mborch     (503) staff       (20)      279 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/120-translation-context.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      116 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/121-translation-comment.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      225 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/122-translation-ignore.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       90 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/123-html5-data-attributes.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      171 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/124-translation-target.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      370 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/125-macro-translation-ordering.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      232 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/126-define-escaping.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       79 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/127-tags-and-attributes-special-chars.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      173 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/237-double-define.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      219 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/238-macroname.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       41 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/greeting.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       55 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/hello_world.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       18 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/hello_world.txt
+-rw-r--r--   0 mborch     (503) staff       (20)       47 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/inputs/multinode-implicit-i18n.pt
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-06-19 05:47:35.343267 Chameleon-4.0.1/src/chameleon/tests/outputs/
+-rw-r--r--   0 mborch     (503) staff       (20)       85 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/001.html
+-rw-r--r--   0 mborch     (503) staff       (20)       61 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/001.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       17 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/001.txt
+-rw-r--r--   0 mborch     (503) staff       (20)      191 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/002.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      355 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/003.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      672 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/004.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      224 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/005.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      252 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/006.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      353 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/007.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      212 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/008.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       62 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/009.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      164 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/010.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      308 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/011-en.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      138 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/011.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      497 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/012-en.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      269 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/012.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      277 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/013.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      180 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/014.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      179 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/015-en.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       92 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/015.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      379 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/016-en.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      186 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/016.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      160 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/017.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      177 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/018-en.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       65 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/018.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      162 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/019.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      133 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/020.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      414 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/021-en.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      196 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/021.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      179 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/022.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       55 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/023.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       77 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/024.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      243 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/025.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      347 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/026.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      173 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/027.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      143 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/028.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      107 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/029.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      104 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/030.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       71 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/031.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      188 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/032.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      188 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/033.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      188 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/034.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      189 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/035.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      182 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/036.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      178 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/037.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       55 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/038.pt
+-rw-r--r--   0 mborch     (503) staff       (20)        0 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/039.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      458 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/040.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      139 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/041.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      203 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/042.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       56 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/043.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       43 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/044.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      463 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/045.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      216 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/046.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      217 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/047.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      208 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/048.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      212 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/049.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      178 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/050.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      178 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/051.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      194 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/052.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       93 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/053.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       34 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/054.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       25 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/055.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       55 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/056.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       53 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/057.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      295 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/058.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      142 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/059.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      103 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/060.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      108 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/061.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      282 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/062.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       16 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/063.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       41 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/064.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      170 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/065.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       51 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/066.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       98 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/067.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      172 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/068.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      228 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/069-en.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      177 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/069.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      228 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/070-en.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      177 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/070.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      328 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/071.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      222 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/072.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      137 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/073.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      159 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/074.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      176 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/075.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      205 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/076.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      120 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/077-en.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       69 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/077.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      283 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/078.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      571 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/079-en.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      321 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/079.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       17 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/080.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       50 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/081.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       50 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/082.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      187 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/083.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      116 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/084.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      288 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/085-en.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      162 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/085.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      264 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/086.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      215 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/087.pt
+-rw-r--r--   0 mborch     (503) staff       (20)        8 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/088.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       50 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/089.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      266 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/090.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       35 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/091.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       67 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/101.html
+-rw-r--r--   0 mborch     (503) staff       (20)       84 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/102.html
+-rw-r--r--   0 mborch     (503) staff       (20)      208 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/103.html
+-rw-r--r--   0 mborch     (503) staff       (20)      301 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/120-en.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      135 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/120.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       60 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/121.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      168 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/122.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       72 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/123.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      171 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/124-en.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      127 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/124.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      141 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/125.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      112 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/126.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       51 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/127.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       39 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/237.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       34 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/238.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       29 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/greeting.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       50 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/hello_world.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       13 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/hello_world.txt
+-rw-r--r--   0 mborch     (503) staff       (20)      119 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/multinode-en.pt
+-rw-r--r--   0 mborch     (503) staff       (20)       44 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/outputs/multinode.pt
+-rw-r--r--   0 mborch     (503) staff       (20)      910 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/test_astutil.py
+-rw-r--r--   0 mborch     (503) staff       (20)     1020 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/test_doctests.py
+-rw-r--r--   0 mborch     (503) staff       (20)      872 2023-06-17 15:00:31.000000 Chameleon-4.0.1/src/chameleon/tests/test_exc.py
+-rw-r--r--   0 mborch     (503) staff       (20)     3485 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/test_loader.py
+-rw-r--r--   0 mborch     (503) staff       (20)     3433 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/test_parser.py
+-rw-r--r--   0 mborch     (503) staff       (20)     3666 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/test_sniffing.py
+-rw-r--r--   0 mborch     (503) staff       (20)    26589 2023-06-19 05:46:42.000000 Chameleon-4.0.1/src/chameleon/tests/test_templates.py
+-rw-r--r--   0 mborch     (503) staff       (20)     1451 2023-03-06 18:09:14.000000 Chameleon-4.0.1/src/chameleon/tests/test_tokenizer.py
+-rw-r--r--   0 mborch     (503) staff       (20)     4296 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/tokenize.py
+-rw-r--r--   0 mborch     (503) staff       (20)    10421 2023-06-17 15:00:31.000000 Chameleon-4.0.1/src/chameleon/utils.py
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-06-19 05:47:35.344220 Chameleon-4.0.1/src/chameleon/zpt/
+-rw-r--r--   0 mborch     (503) staff       (20)        2 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/zpt/__init__.py
+-rw-r--r--   0 mborch     (503) staff       (20)      798 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/zpt/loader.py
+-rw-r--r--   0 mborch     (503) staff       (20)    27911 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/zpt/program.py
+-rw-r--r--   0 mborch     (503) staff       (20)    13867 2023-03-06 17:34:13.000000 Chameleon-4.0.1/src/chameleon/zpt/template.py
+-rw-r--r--   0 mborch     (503) staff       (20)     1648 2023-06-17 15:00:31.000000 Chameleon-4.0.1/tox.ini
```

### Comparing `Chameleon-4.0.0/CHANGES.rst` & `Chameleon-4.0.1/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 Changes
 =======
 
+4.0.1 (2023-06-19)
+------------------
+
+- Fix format spec applying for f-strings.
+  (`#376 <https://github.com/malthe/chameleon/issues/376>`_)
+
 4.0.0 (2023-03-06)
 ------------------
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 - Add support for set- and dict comprehensions
   (`#367 <https://github.com/malthe/chameleon/issues/367>`_)
 
+- Remove the following functions resp. modules:
+
+  + ``.utils.text_()``
+  + ``.utils.unescape()``
+  + ``.compat``
+
+
 3.10.2 (2022-12-16)
 -------------------
 
 - Fix handling of eager compilation with subclassing (e.g. Pyramid integration).
 
 3.10.1 (2022-05-17)
 -------------------
@@ -92,15 +105,15 @@
 
 - Allow setting a custom value representation function, allowing
   custom formatting of variables during exception formatting.
 
 3.7.1 (2020-05-10)
 ------------------
 
-- Fix compatiblity issue with Python 3.9.
+- Fix compatibility issue with Python 3.9.
 
 
 3.7.0 (2020-03-26)
 ------------------
 
 - Fixed garbage collection issue with variable scope objects (issue #301).
 
@@ -666,15 +679,15 @@
 - The exception formatter now keeps track of already formatted
   exceptions, and ignores them from further output.
 
 2.7.4 (2012-02-27)
 ------------------
 
 - The error handler now invokes the ``__init__`` method of
-  ``BaseException`` instead of the possibly overriden method (which
+  ``BaseException`` instead of the possibly overridden method (which
   may take required arguments). This fixes issue #97.
   [j23d, malthe]
 
 2.7.3 (2012-01-16)
 ------------------
 
 Bugfixes:
@@ -1088,15 +1101,15 @@
 - The default symbol is now ``True`` for an attribute if the attribute
   default is not provided. Note that the result is that the attribute
   is dropped. This fixes issue #41.
 
 - Fixed an issue where assignment to a variable ``"type"`` would
   fail. This fixes issue #40.
 
-- Fixed an issue where an (unsuccesful) assignment for a repeat loop
+- Fixed an issue where an (unsuccessful) assignment for a repeat loop
   to a compiler internal name would not result in an error.
 
 - If the translation function returns the identical object, manually
   coerce it to string. This fixes a compatibility issue with
   translation functions which do not convert non-string objects to a
   string value, but simply return them unchanged.
 
@@ -1227,15 +1240,15 @@
 - The compiled template module now contains an ``initialize`` function
   which takes values that map to the template builtins. The return
   value of this function is a dictionary that contains the render
   functions.
 
 Bugfixes:
 
-- The file-based template class no longer verifies the existance of a
+- The file-based template class no longer verifies the existence of a
   template file (using ``os.lstat``). This now happens implicitly if
   eager parsing is enabled, or otherwise when first needed (e.g. at
   render time).
 
   This is classified as a bug fix because the previous behavior was
   probably not what you'd expect, especially if an application
   initializes a lot of templates without needing to render them
@@ -1318,15 +1331,15 @@
 Bugfixes:
 
 - The tab character (``\t``) is now parsed correctly when used inside
   tags.
 
 Features:
 
-- The ``RepeatDict`` class now works as a proxy behind a seperate
+- The ``RepeatDict`` class now works as a proxy behind a separate
   dictionary instance.
 
 - Added template constructor option ``keep_body`` which is a flag
   (also available as a class attribute) that controls whether to save
   the template body input in the ``body`` attribute.
 
   This is disabled by default, unless debug-mode is enabled.
```

### Comparing `Chameleon-4.0.0/LICENSE.txt` & `Chameleon-4.0.1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
     ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR
     TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF
     THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
     SUCH DAMAGE.
 
 Portions of the code in Chameleon are supplied under the ZPL (headers
-within individiual files indicate that these portions are licensed
+within individual files indicate that these portions are licensed
 under the ZPL):
 
   Zope Public License (ZPL) Version 2.1
   -------------------------------------
 
   A copyright notice accompanies this license document that
   identifies the copyright holders.
@@ -95,15 +95,15 @@
     HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
     CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
     OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
     SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
     DAMAGE.
 
 Portions of the code in Chameleon are supplied under the BSD license
-(headers within individiual files indicate that these portions are
+(headers within individual files indicate that these portions are
 licensed under this license):
 
   All rights reserved.
 
   Redistribution and use in source and binary forms, with or without
   modification, are permitted provided that the following conditions
   are met:
@@ -128,15 +128,15 @@
   INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
   IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
   OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
   IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 Portions of the code in Chameleon are supplied under the Python
-License (headers within individiual files indicate that these portions
+License (headers within individual files indicate that these portions
 are licensed under this license):
 
   PYTHON SOFTWARE FOUNDATION LICENSE VERSION 2
   --------------------------------------------
 
   1. This LICENSE AGREEMENT is between the Python Software Foundation
   ("PSF"), and the Individual or Organization ("Licensee") accessing and
```

### Comparing `Chameleon-4.0.0/Makefile` & `Chameleon-4.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/PKG-INFO` & `Chameleon-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chameleon
-Version: 4.0.0
+Version: 4.0.1
 Summary: Fast HTML/XML Template Compiler.
 Home-page: https://chameleon.readthedocs.io
 Author: Malthe Borch
 Author-email: mborch@gmail.com
 License: BSD-like (http://repoze.org/license.html)
 Project-URL: Documentation, https://chameleon.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/malthe/chameleon/issues
@@ -27,15 +27,15 @@
 Overview
 ========
 
 Chameleon is an HTML/XML template engine for `Python
 <http://www.python.org>`_. It uses the *page templates* language.
 
 You can use it in any Python web application with just about any
-version of Python (2.7 and up, including 3.4+ and `pypy
+version of Python (3.7 and up and `pypy 3
 <http://pypy.org>`_).
 
 Visit the `documentation <https://chameleon.readthedocs.io/en/latest/>`_
 for more information.
 
 License and Copyright
 ---------------------
@@ -50,22 +50,35 @@
 .. [1] This software is licensed under the `Repoze
        <http://repoze.org/license.html>`_ license.
 
 
 Changes
 =======
 
+4.0.1 (2023-06-19)
+------------------
+
+- Fix format spec applying for f-strings.
+  (`#376 <https://github.com/malthe/chameleon/issues/376>`_)
+
 4.0.0 (2023-03-06)
 ------------------
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 - Add support for set- and dict comprehensions
   (`#367 <https://github.com/malthe/chameleon/issues/367>`_)
 
+- Remove the following functions resp. modules:
+
+  + ``.utils.text_()``
+  + ``.utils.unescape()``
+  + ``.compat``
+
+
 3.10.2 (2022-12-16)
 -------------------
 
 - Fix handling of eager compilation with subclassing (e.g. Pyramid integration).
 
 3.10.1 (2022-05-17)
 -------------------
@@ -145,15 +158,15 @@
 
 - Allow setting a custom value representation function, allowing
   custom formatting of variables during exception formatting.
 
 3.7.1 (2020-05-10)
 ------------------
 
-- Fix compatiblity issue with Python 3.9.
+- Fix compatibility issue with Python 3.9.
 
 
 3.7.0 (2020-03-26)
 ------------------
 
 - Fixed garbage collection issue with variable scope objects (issue #301).
 
@@ -719,15 +732,15 @@
 - The exception formatter now keeps track of already formatted
   exceptions, and ignores them from further output.
 
 2.7.4 (2012-02-27)
 ------------------
 
 - The error handler now invokes the ``__init__`` method of
-  ``BaseException`` instead of the possibly overriden method (which
+  ``BaseException`` instead of the possibly overridden method (which
   may take required arguments). This fixes issue #97.
   [j23d, malthe]
 
 2.7.3 (2012-01-16)
 ------------------
 
 Bugfixes:
@@ -1141,15 +1154,15 @@
 - The default symbol is now ``True`` for an attribute if the attribute
   default is not provided. Note that the result is that the attribute
   is dropped. This fixes issue #41.
 
 - Fixed an issue where assignment to a variable ``"type"`` would
   fail. This fixes issue #40.
 
-- Fixed an issue where an (unsuccesful) assignment for a repeat loop
+- Fixed an issue where an (unsuccessful) assignment for a repeat loop
   to a compiler internal name would not result in an error.
 
 - If the translation function returns the identical object, manually
   coerce it to string. This fixes a compatibility issue with
   translation functions which do not convert non-string objects to a
   string value, but simply return them unchanged.
 
@@ -1280,15 +1293,15 @@
 - The compiled template module now contains an ``initialize`` function
   which takes values that map to the template builtins. The return
   value of this function is a dictionary that contains the render
   functions.
 
 Bugfixes:
 
-- The file-based template class no longer verifies the existance of a
+- The file-based template class no longer verifies the existence of a
   template file (using ``os.lstat``). This now happens implicitly if
   eager parsing is enabled, or otherwise when first needed (e.g. at
   render time).
 
   This is classified as a bug fix because the previous behavior was
   probably not what you'd expect, especially if an application
   initializes a lot of templates without needing to render them
@@ -1371,15 +1384,15 @@
 Bugfixes:
 
 - The tab character (``\t``) is now parsed correctly when used inside
   tags.
 
 Features:
 
-- The ``RepeatDict`` class now works as a proxy behind a seperate
+- The ``RepeatDict`` class now works as a proxy behind a separate
   dictionary instance.
 
 - Added template constructor option ``keep_body`` which is a flag
   (also available as a class attribute) that controls whether to save
   the template body input in the ``body`` attribute.
 
   This is disabled by default, unless debug-mode is enabled.
```

### Comparing `Chameleon-4.0.0/README.rst` & `Chameleon-4.0.1/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Overview
 ========
 
 Chameleon is an HTML/XML template engine for `Python
 <http://www.python.org>`_. It uses the *page templates* language.
 
 You can use it in any Python web application with just about any
-version of Python (2.7 and up, including 3.4+ and `pypy
+version of Python (3.7 and up and `pypy 3
 <http://pypy.org>`_).
 
 Visit the `documentation <https://chameleon.readthedocs.io/en/latest/>`_
 for more information.
 
 License and Copyright
 ---------------------
```

### Comparing `Chameleon-4.0.0/setup.py` & `Chameleon-4.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '4.0.0'
+__version__ = '4.0.1'
 
 import os
 
 from setuptools import find_packages
 from setuptools import setup
 from setuptools.command.test import test
 
@@ -60,15 +60,15 @@
     url="https://chameleon.readthedocs.io",
     project_urls={
         'Documentation': 'https://chameleon.readthedocs.io',
         'Issue Tracker': 'https://github.com/malthe/chameleon/issues',
         'Sources': 'https://github.com/malthe/chameleon',
     },
     license='BSD-like (http://repoze.org/license.html)',
-    packages=find_packages('src', exclude=['test*']),
+    packages=find_packages('src'),
     package_dir={'': 'src'},
     include_package_data=True,
     python_requires='>=3.7',
     install_requires=install_requires,
     extras_require={
         'docs': {
             'Sphinx',
```

### Comparing `Chameleon-4.0.0/src/Chameleon.egg-info/PKG-INFO` & `Chameleon-4.0.1/src/Chameleon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chameleon
-Version: 4.0.0
+Version: 4.0.1
 Summary: Fast HTML/XML Template Compiler.
 Home-page: https://chameleon.readthedocs.io
 Author: Malthe Borch
 Author-email: mborch@gmail.com
 License: BSD-like (http://repoze.org/license.html)
 Project-URL: Documentation, https://chameleon.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/malthe/chameleon/issues
@@ -27,15 +27,15 @@
 Overview
 ========
 
 Chameleon is an HTML/XML template engine for `Python
 <http://www.python.org>`_. It uses the *page templates* language.
 
 You can use it in any Python web application with just about any
-version of Python (2.7 and up, including 3.4+ and `pypy
+version of Python (3.7 and up and `pypy 3
 <http://pypy.org>`_).
 
 Visit the `documentation <https://chameleon.readthedocs.io/en/latest/>`_
 for more information.
 
 License and Copyright
 ---------------------
@@ -50,22 +50,35 @@
 .. [1] This software is licensed under the `Repoze
        <http://repoze.org/license.html>`_ license.
 
 
 Changes
 =======
 
+4.0.1 (2023-06-19)
+------------------
+
+- Fix format spec applying for f-strings.
+  (`#376 <https://github.com/malthe/chameleon/issues/376>`_)
+
 4.0.0 (2023-03-06)
 ------------------
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 - Add support for set- and dict comprehensions
   (`#367 <https://github.com/malthe/chameleon/issues/367>`_)
 
+- Remove the following functions resp. modules:
+
+  + ``.utils.text_()``
+  + ``.utils.unescape()``
+  + ``.compat``
+
+
 3.10.2 (2022-12-16)
 -------------------
 
 - Fix handling of eager compilation with subclassing (e.g. Pyramid integration).
 
 3.10.1 (2022-05-17)
 -------------------
@@ -145,15 +158,15 @@
 
 - Allow setting a custom value representation function, allowing
   custom formatting of variables during exception formatting.
 
 3.7.1 (2020-05-10)
 ------------------
 
-- Fix compatiblity issue with Python 3.9.
+- Fix compatibility issue with Python 3.9.
 
 
 3.7.0 (2020-03-26)
 ------------------
 
 - Fixed garbage collection issue with variable scope objects (issue #301).
 
@@ -719,15 +732,15 @@
 - The exception formatter now keeps track of already formatted
   exceptions, and ignores them from further output.
 
 2.7.4 (2012-02-27)
 ------------------
 
 - The error handler now invokes the ``__init__`` method of
-  ``BaseException`` instead of the possibly overriden method (which
+  ``BaseException`` instead of the possibly overridden method (which
   may take required arguments). This fixes issue #97.
   [j23d, malthe]
 
 2.7.3 (2012-01-16)
 ------------------
 
 Bugfixes:
@@ -1141,15 +1154,15 @@
 - The default symbol is now ``True`` for an attribute if the attribute
   default is not provided. Note that the result is that the attribute
   is dropped. This fixes issue #41.
 
 - Fixed an issue where assignment to a variable ``"type"`` would
   fail. This fixes issue #40.
 
-- Fixed an issue where an (unsuccesful) assignment for a repeat loop
+- Fixed an issue where an (unsuccessful) assignment for a repeat loop
   to a compiler internal name would not result in an error.
 
 - If the translation function returns the identical object, manually
   coerce it to string. This fixes a compatibility issue with
   translation functions which do not convert non-string objects to a
   string value, but simply return them unchanged.
 
@@ -1280,15 +1293,15 @@
 - The compiled template module now contains an ``initialize`` function
   which takes values that map to the template builtins. The return
   value of this function is a dictionary that contains the render
   functions.
 
 Bugfixes:
 
-- The file-based template class no longer verifies the existance of a
+- The file-based template class no longer verifies the existence of a
   template file (using ``os.lstat``). This now happens implicitly if
   eager parsing is enabled, or otherwise when first needed (e.g. at
   render time).
 
   This is classified as a bug fix because the previous behavior was
   probably not what you'd expect, especially if an application
   initializes a lot of templates without needing to render them
@@ -1371,15 +1384,15 @@
 Bugfixes:
 
 - The tab character (``\t``) is now parsed correctly when used inside
   tags.
 
 Features:
 
-- The ``RepeatDict`` class now works as a proxy behind a seperate
+- The ``RepeatDict`` class now works as a proxy behind a separate
   dictionary instance.
 
 - Added template constructor option ``keep_body`` which is a flag
   (also available as a class attribute) that controls whether to save
   the template body input in the ``body`` attribute.
 
   This is disabled by default, unless debug-mode is enabled.
```

### Comparing `Chameleon-4.0.0/src/chameleon/astutil.py` & `Chameleon-4.0.1/src/chameleon/astutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,16 +409,17 @@
         elif node.conversion == ord('a'):
             self._write('ascii')
         else:
             self._write('str')
         self._write('(')
         self.visit(node.value)
         if node.format_spec is not None:
-            self._write(').__format__(')
+            self._write('.__format__(')
             self.visit(node.format_spec)
+            self._write(')')
         self._write(')')
 
     # Print(expr? dest, expr* values, bool nl)
     def visit_Print(self, node):
         self._new_line()
         self._write('print')
         if getattr(node, 'dest', None):
```

### Comparing `Chameleon-4.0.0/src/chameleon/benchmark.py` & `Chameleon-4.0.1/src/chameleon/benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import os
 import re
 import time
 import unittest
 from itertools import chain
 
-from .utils import text_
-
 
 re_amp = re.compile(r'&(?!([A-Za-z]+|#[0-9]+);)')
 
 BIGTABLE_ZPT = """\
 <table xmlns="http://www.w3.org/1999/xhtml"
 xmlns:tal="http://xml.zope.org/namespaces/tal">
 <tr tal:repeat="row python: options['table']">
@@ -365,15 +363,15 @@
     @staticmethod
     def _zope(body):
         from zope.pagetemplate.pagetemplatefile import PageTemplate
         template = PageTemplate()
         template.pt_edit(body, 'text/xhtml')
         return template
 
-    @benchmark(text_("BIGTABLE [python]"))
+    @benchmark("BIGTABLE [python]")
     def test_bigtable(self):
         options = {'table': self.table}
 
         t_chameleon = timing(self._chameleon(BIGTABLE_ZPT), options=options)
         print("chameleon:         %7.2f" % t_chameleon)
 
         t_chameleon_utf8 = timing(
@@ -399,55 +397,55 @@
 
         print("--------------------------")
         print("check: %d vs %d" % (
             len(self._chameleon(BIGTABLE_ZPT)(options=options)),
             len(self._zope(BIGTABLE_ZPT)(table=self.table))))
         print("--------------------------")
 
-    @benchmark(text_("MANY STRINGS [python]"))
+    @benchmark("MANY STRINGS [python]")
     def test_many_strings(self):
         t_chameleon = timing(self._chameleon(MANY_STRINGS_ZPT))
         print("chameleon:         %7.2f" % t_chameleon)
         t_zope = timing(self._zope(MANY_STRINGS_ZPT))
         print("zope.pagetemplate: %7.2f" % t_zope)
         print("                  %7.1fX" % (t_zope / t_chameleon))
 
         print("--------------------------")
         print("check: %d vs %d" % (
             len(self._chameleon(MANY_STRINGS_ZPT)()),
             len(self._zope(MANY_STRINGS_ZPT)())))
         print("--------------------------")
 
-    @benchmark(text_("HELLO WORLD"))
+    @benchmark("HELLO WORLD")
     def test_hello_world(self):
         t_chameleon = timing(self._chameleon(HELLO_WORLD_ZPT)) * 1000
         print("chameleon:         %7.2f" % t_chameleon)
         t_zope = timing(self._zope(HELLO_WORLD_ZPT)) * 1000
         print("zope.pagetemplate: %7.2f" % t_zope)
         print("                  %7.1fX" % (t_zope / t_chameleon))
 
         print("--------------------------")
         print("check: %d vs %d" % (
             len(self._chameleon(HELLO_WORLD_ZPT)()),
             len(self._zope(HELLO_WORLD_ZPT)())))
         print("--------------------------")
 
-    @benchmark(text_("I18N"))
+    @benchmark("I18N")
     def test_i18n(self):
         from zope.i18n import translate
         t_chameleon = timing(
             self._chameleon(I18N_ZPT),
             translate=translate,
             language="klingon") * 1000
         print("chameleon:         %7.2f" % t_chameleon)
         t_zope = timing(self._zope(I18N_ZPT), env=self.env) * 1000
         print("zope.pagetemplate: %7.2f" % t_zope)
         print("                  %7.1fX" % (t_zope / t_chameleon))
 
-    @benchmark(text_("COMPILATION"))
+    @benchmark("COMPILATION")
     def test_compilation(self):
         template = self._chameleon(HELLO_WORLD_ZPT)
 
         def chameleon_cook_and_render(template=template):
             template.cook(HELLO_WORLD_ZPT)
             template()
```

### Comparing `Chameleon-4.0.0/src/chameleon/codegen.py` & `Chameleon-4.0.1/src/chameleon/codegen.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/src/chameleon/compiler.py` & `Chameleon-4.0.1/src/chameleon/compiler.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/src/chameleon/config.py` & `Chameleon-4.0.1/src/chameleon/config.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/src/chameleon/exc.py` & `Chameleon-4.0.1/src/chameleon/exc.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
            ^^^
 
     >>> test('  foo bar baz  ', 6, 'bar', 6)
     ··· o bar ···
           ^^^
 
     The entire expression is always shown, even if ``size`` does not
-    accomodate for it.
+    accommodate for it.
 
     >>> test('  foo bar baz  ', 6, 'bar baz', 10)
     ··· oo bar baz
            ^^^^^^^
 
     >>> test('      foo bar', 10, 'bar', 5)
     ··· o bar
```

### Comparing `Chameleon-4.0.0/src/chameleon/i18n.py` & `Chameleon-4.0.1/src/chameleon/i18n.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/src/chameleon/interfaces.py` & `Chameleon-4.0.1/src/chameleon/interfaces.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/src/chameleon/loader.py` & `Chameleon-4.0.1/src/chameleon/loader.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/src/chameleon/metal.py` & `Chameleon-4.0.1/src/chameleon/metal.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/src/chameleon/nodes.py` & `Chameleon-4.0.1/src/chameleon/nodes.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/src/chameleon/parser.py` & `Chameleon-4.0.1/src/chameleon/parser.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/src/chameleon/program.py` & `Chameleon-4.0.1/src/chameleon/program.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/src/chameleon/tal.py` & `Chameleon-4.0.1/src/chameleon/tal.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/src/chameleon/tales.py` & `Chameleon-4.0.1/src/chameleon/tales.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,15 @@
     def parse(self, string):
         return parse(string, 'eval').body
 
     def translate(self, expression, target):
         # Strip spaces
         string = expression.strip()
 
-        # Conver line continuations to newlines
+        # Convert line continuations to newlines
         string = substitute(re_continuation, '\n', string)
 
         # Convert newlines to spaces
         string = string.replace('\n', ' ')
 
         try:
             value = self.parse(string)
@@ -423,15 +423,15 @@
     >>> test(StringExpr('test $$ ${1}'))
     'test $ 1'
 
     In the above examples, the expression is evaluated using the
     dummy engine which just returns the input as a string.
 
     As an example, we'll implement an expression engine which
-    instead counts the number of characters in the expresion and
+    instead counts the number of characters in the expression and
     returns an integer result.
 
     >>> class engine:
     ...     @staticmethod
     ...     def parse(expression, char_escape=None):
     ...         class compiler:
     ...             @staticmethod
```

### Comparing `Chameleon-4.0.0/src/chameleon/template.py` & `Chameleon-4.0.1/src/chameleon/template.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/src/chameleon/tokenize.py` & `Chameleon-4.0.1/src/chameleon/tokenize.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/src/chameleon/utils.py` & `Chameleon-4.0.1/src/chameleon/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,14 @@
     raise exc
 
 
 def encode_string(s):
     return bytes(s, 'utf-8')
 
 
-def text_(s, encoding='latin-1', errors='strict'):
-    """ If ``s`` is an instance of ``bytes``, return
-    ``s.decode(encoding, errors)``, otherwise return ``s``"""
-    if isinstance(s, bytes):
-        return s.decode(encoding, errors)
-    return s
-
-
 entity_re = re.compile(r'&(#?)(x?)(\d{1,5}|\w{1,8});')
 
 module_cache = {}
 
 xml_prefixes = (
     (codecs.BOM_UTF8, 'utf-8-sig'),
     (codecs.BOM_UTF16_BE, 'utf-16-be'),
@@ -183,22 +175,14 @@
         return inst
     except ValueError:
         name = type(exc).__name__
         log.warn("Unable to copy exception of type '%s'." % name)
         raise TypeError(exc)
 
 
-def unescape(string):
-    for name in ('lt', 'gt', 'quot'):
-        cp = htmlentitydefs.name2codepoint[name]
-        string = string.replace('&%s;' % name, chr(cp))
-
-    return string
-
-
 _concat = "".join
 
 
 def join(stream):
     """Concatenate stream.
 
     >>> print(join(('Hello', ' ', 'world')))
```

### Comparing `Chameleon-4.0.0/src/chameleon/zpt/loader.py` & `Chameleon-4.0.1/src/chameleon/zpt/loader.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/src/chameleon/zpt/program.py` & `Chameleon-4.0.1/src/chameleon/zpt/program.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.0.0/src/chameleon/zpt/template.py` & `Chameleon-4.0.1/src/chameleon/zpt/template.py`

 * *Files identical despite different names*

