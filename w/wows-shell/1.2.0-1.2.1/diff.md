# Comparing `tmp/wows_shell-1.2.0.tar.gz` & `tmp/wows_shell-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wows_shell-1.2.0.tar", last modified: Wed Feb 23 03:58:42 2022, max compression
+gzip compressed data, was "wows_shell-1.2.1.tar", last modified: Mon Jun 19 19:00:29 2023, max compression
```

## Comparing `wows_shell-1.2.0.tar` & `wows_shell-1.2.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.580452 wows_shell-1.2.0/
--rw-rw-rw-   0        0        0     1084 2020-07-28 13:49:29.000000 wows_shell-1.2.0/LICENSE
--rw-rw-rw-   0        0        0       31 2021-01-23 20:09:16.000000 wows_shell-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3257 2022-02-23 03:58:42.579454 wows_shell-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3003 2020-12-29 19:40:43.000000 wows_shell-1.2.0/README.md
--rw-rw-rw-   0        0        0      131 2021-01-23 20:09:16.000000 wows_shell-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-02-23 03:58:42.580452 wows_shell-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1095 2022-02-23 03:50:40.000000 wows_shell-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.535573 wows_shell-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.536570 wows_shell-1.2.0/src/Python/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.517620 wows_shell-1.2.0/src/Python/out/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.517620 wows_shell-1.2.0/src/Python/out/build/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.518617 wows_shell-1.2.0/src/Python/out/build/x64-Debug (default)/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.518617 wows_shell-1.2.0/src/Python/out/build/x64-Debug (default)/CMakeFiles/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.537568 wows_shell-1.2.0/src/Python/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/
--rw-rw-rw-   0        0        0        2 2021-01-23 06:11:54.000000 wows_shell-1.2.0/src/Python/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/foo.h
--rw-rw-rw-   0        0        0    24784 2022-02-21 19:07:47.000000 wows_shell-1.2.0/src/Python/wows_shell_python.cpp
--rw-rw-rw-   0        0        0     3197 2022-02-01 03:51:03.000000 wows_shell-1.2.0/src/controlEnums.hpp
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.519614 wows_shell-1.2.0/src/fitShell/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.519614 wows_shell-1.2.0/src/fitShell/out/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.520612 wows_shell-1.2.0/src/fitShell/out/build/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.520612 wows_shell-1.2.0/src/fitShell/out/build/x64-Debug/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.521609 wows_shell-1.2.0/src/fitShell/out/build/x64-Debug/CMakeFiles/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.539563 wows_shell-1.2.0/src/fitShell/out/build/x64-Debug/CMakeFiles/ShowIncludes/
--rw-rw-rw-   0        0        0        2 2020-12-26 00:29:01.000000 wows_shell-1.2.0/src/fitShell/out/build/x64-Debug/CMakeFiles/ShowIncludes/foo.h
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.519614 wows_shell-1.2.0/src/fitShell/out/build/x64-Debug (default)/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.520612 wows_shell-1.2.0/src/fitShell/out/build/x64-Debug (default)/CMakeFiles/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.538565 wows_shell-1.2.0/src/fitShell/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/
--rw-rw-rw-   0        0        0        2 2021-01-23 06:11:50.000000 wows_shell-1.2.0/src/fitShell/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/foo.h
--rw-rw-rw-   0        0        0    24904 2021-11-03 17:37:58.000000 wows_shell-1.2.0/src/shell.hpp
--rw-rw-rw-   0        0        0    77495 2022-02-21 18:03:31.000000 wows_shell-1.2.0/src/shellCPP.hpp
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.521609 wows_shell-1.2.0/src/test/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.522607 wows_shell-1.2.0/src/test/out/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.523604 wows_shell-1.2.0/src/test/out/build/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.522607 wows_shell-1.2.0/src/test/out/build/x64-Debug/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.522607 wows_shell-1.2.0/src/test/out/build/x64-Debug/CMakeFiles/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.540560 wows_shell-1.2.0/src/test/out/build/x64-Debug/CMakeFiles/ShowIncludes/
--rw-rw-rw-   0        0        0        2 2021-01-07 19:49:47.000000 wows_shell-1.2.0/src/test/out/build/x64-Debug/CMakeFiles/ShowIncludes/foo.h
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.523604 wows_shell-1.2.0/src/test/out/build/x64-Release/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.524601 wows_shell-1.2.0/src/test/out/build/x64-Release/CMakeFiles/
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.542554 wows_shell-1.2.0/src/test/out/build/x64-Release/CMakeFiles/ShowIncludes/
--rw-rw-rw-   0        0        0        2 2021-01-07 19:53:01.000000 wows_shell-1.2.0/src/test/out/build/x64-Release/CMakeFiles/ShowIncludes/foo.h
--rw-rw-rw-   0        0        0     6534 2021-11-04 18:20:45.000000 wows_shell-1.2.0/src/utility.hpp
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.572478 wows_shell-1.2.0/src/version2/
--rw-rw-rw-   0        0        0    65564 2021-01-23 19:57:18.000000 wows_shell-1.2.0/src/version2/instrset.h
--rw-rw-rw-   0        0        0    16541 2021-01-23 19:57:18.000000 wows_shell-1.2.0/src/version2/vector_convert.h
--rw-rw-rw-   0        0        0     3357 2021-01-23 19:57:18.000000 wows_shell-1.2.0/src/version2/vectorclass.h
--rw-rw-rw-   0        0        0   103276 2021-01-23 19:57:18.000000 wows_shell-1.2.0/src/version2/vectorf128.h
--rw-rw-rw-   0        0        0   108363 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectorf256.h
--rw-rw-rw-   0        0        0    65665 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectorf256e.h
--rw-rw-rw-   0        0        0    78870 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectorf512.h
--rw-rw-rw-   0        0        0    67972 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectorf512e.h
--rw-rw-rw-   0        0        0   267691 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectori128.h
--rw-rw-rw-   0        0        0   223226 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectori256.h
--rw-rw-rw-   0        0        0   136921 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectori256e.h
--rw-rw-rw-   0        0        0    85149 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectori512.h
--rw-rw-rw-   0        0        0    79858 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectori512e.h
--rw-rw-rw-   0        0        0    95406 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectori512s.h
--rw-rw-rw-   0        0        0    74561 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectori512se.h
--rw-rw-rw-   0        0        0    13288 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectormath_common.h
--rw-rw-rw-   0        0        0    77691 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectormath_exp.h
--rw-rw-rw-   0        0        0    22661 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectormath_hyp.h
--rw-rw-rw-   0        0        0    77876 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectormath_lib.h
--rw-rw-rw-   0        0        0    29775 2021-01-17 18:51:59.000000 wows_shell-1.2.0/src/version2/vectormath_trig.h
-drwxrwxrwx   0        0        0        0 2022-02-23 03:58:42.578459 wows_shell-1.2.0/wows_shell.egg-info/
--rw-rw-rw-   0        0        0     3257 2022-02-23 03:58:42.000000 wows_shell-1.2.0/wows_shell.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1204 2022-02-23 03:58:42.000000 wows_shell-1.2.0/wows_shell.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-23 03:58:42.000000 wows_shell-1.2.0/wows_shell.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-02-23 03:58:42.000000 wows_shell-1.2.0/wows_shell.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.479077 wows_shell-1.2.1/
+-rw-rw-rw-   0        0        0     1084 2020-07-28 13:49:29.000000 wows_shell-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0       31 2021-01-23 20:09:16.000000 wows_shell-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3257 2023-06-19 19:00:29.478082 wows_shell-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3003 2020-12-29 19:40:43.000000 wows_shell-1.2.1/README.md
+-rw-rw-rw-   0        0        0      131 2021-01-23 20:09:16.000000 wows_shell-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 19:00:29.480119 wows_shell-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2023-06-19 14:50:35.000000 wows_shell-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.396871 wows_shell-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.399847 wows_shell-1.2.1/src/Python/
+drwxrwxrwx   0        0        0        0 2023-06-19 18:51:10.703243 wows_shell-1.2.1/src/Python/out/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.366842 wows_shell-1.2.1/src/Python/out/build/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.366842 wows_shell-1.2.1/src/Python/out/build/x64-Debug (default)/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.366842 wows_shell-1.2.1/src/Python/out/build/x64-Debug (default)/CMakeFiles/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.401618 wows_shell-1.2.1/src/Python/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/
+-rw-rw-rw-   0        0        0        2 2021-01-23 06:11:54.000000 wows_shell-1.2.1/src/Python/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/foo.h
+-rw-rw-rw-   0        0        0    24784 2023-06-19 14:50:35.000000 wows_shell-1.2.1/src/Python/wows_shell_python.cpp
+-rw-rw-rw-   0        0        0     3197 2022-02-01 03:51:03.000000 wows_shell-1.2.1/src/controlEnums.hpp
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.368808 wows_shell-1.2.1/src/fitShell/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.368808 wows_shell-1.2.1/src/fitShell/out/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.370921 wows_shell-1.2.1/src/fitShell/out/build/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.371919 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.371919 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug/CMakeFiles/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.407608 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug/CMakeFiles/ShowIncludes/
+-rw-rw-rw-   0        0        0        2 2020-12-26 00:29:01.000000 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug/CMakeFiles/ShowIncludes/foo.h
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.370921 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug (default)/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.370921 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug (default)/CMakeFiles/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.405621 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/
+-rw-rw-rw-   0        0        0        2 2021-01-23 06:11:50.000000 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/foo.h
+-rw-rw-rw-   0        0        0    24869 2023-06-19 14:50:35.000000 wows_shell-1.2.1/src/shell.hpp
+-rw-rw-rw-   0        0        0    77483 2023-06-19 14:50:35.000000 wows_shell-1.2.1/src/shellCPP.hpp
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.373912 wows_shell-1.2.1/src/test/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.373912 wows_shell-1.2.1/src/test/out/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.375909 wows_shell-1.2.1/src/test/out/build/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.374909 wows_shell-1.2.1/src/test/out/build/x64-Debug/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.374909 wows_shell-1.2.1/src/test/out/build/x64-Debug/CMakeFiles/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.409608 wows_shell-1.2.1/src/test/out/build/x64-Debug/CMakeFiles/ShowIncludes/
+-rw-rw-rw-   0        0        0        2 2021-01-07 19:49:47.000000 wows_shell-1.2.1/src/test/out/build/x64-Debug/CMakeFiles/ShowIncludes/foo.h
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.375909 wows_shell-1.2.1/src/test/out/build/x64-Release/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.376906 wows_shell-1.2.1/src/test/out/build/x64-Release/CMakeFiles/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.411637 wows_shell-1.2.1/src/test/out/build/x64-Release/CMakeFiles/ShowIncludes/
+-rw-rw-rw-   0        0        0        2 2021-01-07 19:53:01.000000 wows_shell-1.2.1/src/test/out/build/x64-Release/CMakeFiles/ShowIncludes/foo.h
+-rw-rw-rw-   0        0        0     6534 2023-06-19 14:50:35.000000 wows_shell-1.2.1/src/utility.hpp
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.466108 wows_shell-1.2.1/src/version2/
+-rw-rw-rw-   0        0        0    65564 2021-01-23 19:57:18.000000 wows_shell-1.2.1/src/version2/instrset.h
+-rw-rw-rw-   0        0        0    16541 2021-01-23 19:57:18.000000 wows_shell-1.2.1/src/version2/vector_convert.h
+-rw-rw-rw-   0        0        0     3357 2021-01-23 19:57:18.000000 wows_shell-1.2.1/src/version2/vectorclass.h
+-rw-rw-rw-   0        0        0   103276 2021-01-23 19:57:18.000000 wows_shell-1.2.1/src/version2/vectorf128.h
+-rw-rw-rw-   0        0        0   108363 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectorf256.h
+-rw-rw-rw-   0        0        0    65665 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectorf256e.h
+-rw-rw-rw-   0        0        0    78870 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectorf512.h
+-rw-rw-rw-   0        0        0    67972 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectorf512e.h
+-rw-rw-rw-   0        0        0   267691 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectori128.h
+-rw-rw-rw-   0        0        0   223226 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectori256.h
+-rw-rw-rw-   0        0        0   136921 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectori256e.h
+-rw-rw-rw-   0        0        0    85149 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectori512.h
+-rw-rw-rw-   0        0        0    79858 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectori512e.h
+-rw-rw-rw-   0        0        0    95406 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectori512s.h
+-rw-rw-rw-   0        0        0    74561 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectori512se.h
+-rw-rw-rw-   0        0        0    13288 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectormath_common.h
+-rw-rw-rw-   0        0        0    77691 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectormath_exp.h
+-rw-rw-rw-   0        0        0    22661 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectormath_hyp.h
+-rw-rw-rw-   0        0        0    77876 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectormath_lib.h
+-rw-rw-rw-   0        0        0    29775 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectormath_trig.h
+drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.475083 wows_shell-1.2.1/wows_shell.egg-info/
+-rw-rw-rw-   0        0        0     3257 2023-06-19 19:00:28.000000 wows_shell-1.2.1/wows_shell.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1204 2023-06-19 19:00:29.000000 wows_shell-1.2.1/wows_shell.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 19:00:28.000000 wows_shell-1.2.1/wows_shell.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 19:00:28.000000 wows_shell-1.2.1/wows_shell.egg-info/top_level.txt
```

### Comparing `wows_shell-1.2.0/LICENSE` & `wows_shell-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/PKG-INFO` & `wows_shell-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wows_shell
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python extension of wows_shell
 Home-page: https://github.com/jcw780/wows_shell
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wows_shell-1.2.0/README.md` & `wows_shell-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/setup.py` & `wows_shell-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     cxx_compile_args.append('-march=native')
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="wows_shell",
-    version="1.2.0",
+    version="1.2.1",
     description="Python extension of wows_shell",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jcw780/wows_shell",
     cmdclass={"build_ext": build_ext},
     ext_modules=ext_modules,
 )
```

### Comparing `wows_shell-1.2.0/src/Python/wows_shell_python.cpp` & `wows_shell-1.2.1/src/Python/wows_shell_python.cpp`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/controlEnums.hpp` & `wows_shell-1.2.1/src/controlEnums.hpp`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/shell.hpp` & `wows_shell-1.2.1/src/shell.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -100,16 +100,15 @@
 };
 
 double combinedAirDrag(double cD, double caliber, double mass) {
     return 0.5 * cD * pow((caliber / 2), 2) * M_PI / mass;
 }
 
 double combinedPenetration(double krupp, double mass, double caliber) {
-    return 0.00046905491615181766 * krupp / 2400 * pow(mass, 0.5506) *
-           pow(caliber, -0.6521);
+    return 0.0000001 * krupp * pow(mass, 0.69) * pow(caliber, -1.07); 
 }
 
 class shell {
    public:  // Description                units
     // Shell
     double v0;             // muzzle velocity            m/s
     double caliber;        // shell caliber              m
```

### Comparing `wows_shell-1.2.0/src/shellCPP.hpp` & `wows_shell-1.2.1/src/shellCPP.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     double precision = .1;  // Angle Step                   | degrees
     double x0 = 0, y0 = 0;  // Starting x0, y0              | m
     double dt_min = .02;    // Time step                    | s
 
     static constexpr double timeMultiplier = 2.75;
     // For some reason the game has a different shell multiplier than the
     // global speed multiplier of 2.61 used for everything else.
-    static constexpr double velocityPower = 1.4822064892953855;
+    static constexpr double velocityPower = 2*0.69;
     // Effect of impact velocity on penetration: P = K * v ^ velocity power
 
     // delta t (dtf) for fusing needs to be smaller than the delta t (dt) used
     // for trajectories due to the shorter distances. Otherwise results become
     // jagged - precision suffers.
     double dtf = 0.0001;
     double xf0 = 0, yf0 = 0;
```

### Comparing `wows_shell-1.2.0/src/utility.hpp` & `wows_shell-1.2.1/src/utility.hpp`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/instrset.h` & `wows_shell-1.2.1/src/version2/instrset.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vector_convert.h` & `wows_shell-1.2.1/src/version2/vector_convert.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectorclass.h` & `wows_shell-1.2.1/src/version2/vectorclass.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectorf128.h` & `wows_shell-1.2.1/src/version2/vectorf128.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectorf256.h` & `wows_shell-1.2.1/src/version2/vectorf256.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectorf256e.h` & `wows_shell-1.2.1/src/version2/vectorf256e.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectorf512.h` & `wows_shell-1.2.1/src/version2/vectorf512.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectorf512e.h` & `wows_shell-1.2.1/src/version2/vectorf512e.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectori128.h` & `wows_shell-1.2.1/src/version2/vectori128.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectori256.h` & `wows_shell-1.2.1/src/version2/vectori256.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectori256e.h` & `wows_shell-1.2.1/src/version2/vectori256e.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectori512.h` & `wows_shell-1.2.1/src/version2/vectori512.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectori512e.h` & `wows_shell-1.2.1/src/version2/vectori512e.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectori512s.h` & `wows_shell-1.2.1/src/version2/vectori512s.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectori512se.h` & `wows_shell-1.2.1/src/version2/vectori512se.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectormath_common.h` & `wows_shell-1.2.1/src/version2/vectormath_common.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectormath_exp.h` & `wows_shell-1.2.1/src/version2/vectormath_exp.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectormath_hyp.h` & `wows_shell-1.2.1/src/version2/vectormath_hyp.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectormath_lib.h` & `wows_shell-1.2.1/src/version2/vectormath_lib.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/src/version2/vectormath_trig.h` & `wows_shell-1.2.1/src/version2/vectormath_trig.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.0/wows_shell.egg-info/PKG-INFO` & `wows_shell-1.2.1/wows_shell.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wows-shell
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python extension of wows_shell
 Home-page: https://github.com/jcw780/wows_shell
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wows_shell-1.2.0/wows_shell.egg-info/SOURCES.txt` & `wows_shell-1.2.1/wows_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

