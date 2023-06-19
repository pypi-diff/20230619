# Comparing `tmp/MCPoly-0.4.2.3.tar.gz` & `tmp/MCPoly-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MCPoly-0.4.2.3.tar", last modified: Mon Jun 12 17:24:21 2023, max compression
+gzip compressed data, was "MCPoly-0.5.0.tar", last modified: Mon Jun 19 08:26:12 2023, max compression
```

## Comparing `MCPoly-0.4.2.3.tar` & `MCPoly-0.5.0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.129286 MCPoly-0.4.2.3/
--rw-r--r--   0 cxs454     (503) staff       (20)     1091 2023-05-03 15:22:57.000000 MCPoly-0.4.2.3/LICENSE
--rw-r--r--   0 cxs454     (503) staff       (20)       17 2023-05-04 08:23:11.000000 MCPoly-0.4.2.3/MANIFEST.in
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.121744 MCPoly-0.4.2.3/MCPoly/
--rw-r--r--   0 cxs454     (503) staff       (20)    14340 2023-06-12 17:23:57.000000 MCPoly-0.4.2.3/MCPoly/.DS_Store
--rw-r--r--   0 cxs454     (503) staff       (20)      178 2023-05-15 14:05:30.000000 MCPoly-0.4.2.3/MCPoly/__init__.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.123581 MCPoly-0.4.2.3/MCPoly/lmpset/
--rw-r--r--   0 cxs454     (503) staff       (20)     5785 2023-06-12 14:51:07.000000 MCPoly-0.4.2.3/MCPoly/lmpset/DATAtoXYZ.py
--rw-r--r--   0 cxs454     (503) staff       (20)     4361 2023-06-12 14:51:59.000000 MCPoly-0.4.2.3/MCPoly/lmpset/DATAtomolTXT.py
--rw-r--r--   0 cxs454     (503) staff       (20)      146 2023-06-03 14:29:24.000000 MCPoly-0.4.2.3/MCPoly/lmpset/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    55548 2023-06-05 13:00:53.000000 MCPoly-0.4.2.3/MCPoly/lmpset/chain.py
--rw-r--r--   0 cxs454     (503) staff       (20)    16310 2023-06-03 14:28:50.000000 MCPoly-0.4.2.3/MCPoly/lmpset/infchain.py
--rw-r--r--   0 cxs454     (503) staff       (20)    50867 2023-06-12 14:57:57.000000 MCPoly-0.4.2.3/MCPoly/lmpset/mould.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.124686 MCPoly-0.4.2.3/MCPoly/moldraw/
--rw-r--r--   0 cxs454     (503) staff       (20)     8966 2023-05-26 12:59:21.000000 MCPoly-0.4.2.3/MCPoly/moldraw/C_selection.py
--rw-r--r--   0 cxs454     (503) staff       (20)      128 2023-05-29 06:59:26.000000 MCPoly-0.4.2.3/MCPoly/moldraw/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    64145 2023-05-26 10:41:02.000000 MCPoly-0.4.2.3/MCPoly/moldraw/bind_selection.py
--rw-r--r--   0 cxs454     (503) staff       (20)    24385 2023-05-29 07:03:41.000000 MCPoly-0.4.2.3/MCPoly/moldraw/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)   181892 2023-05-26 12:59:34.000000 MCPoly-0.4.2.3/MCPoly/moldraw/molecule.py
--rw-r--r--   0 cxs454     (503) staff       (20)    98156 2023-05-26 10:40:13.000000 MCPoly-0.4.2.3/MCPoly/moldraw/sub_selection.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.126086 MCPoly-0.4.2.3/MCPoly/orcaset/
--rw-r--r--   0 cxs454     (503) staff       (20)     8635 2023-05-02 16:35:59.000000 MCPoly-0.4.2.3/MCPoly/orcaset/XYZtoINP.py
--rw-r--r--   0 cxs454     (503) staff       (20)      158 2023-05-11 15:49:25.000000 MCPoly-0.4.2.3/MCPoly/orcaset/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    16723 2023-06-12 17:02:56.000000 MCPoly-0.4.2.3/MCPoly/orcaset/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     7592 2023-06-07 15:00:39.000000 MCPoly-0.4.2.3/MCPoly/orcaset/mgui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     4842 2023-05-02 16:29:09.000000 MCPoly-0.4.2.3/MCPoly/orcaset/multiorca.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2072 2023-05-15 15:20:42.000000 MCPoly-0.4.2.3/MCPoly/orcaset/orca.py
--rw-r--r--   0 cxs454     (503) staff       (20)    19705 2023-06-09 15:20:27.000000 MCPoly-0.4.2.3/MCPoly/orcaset/ssgui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     9044 2023-06-09 09:20:04.000000 MCPoly-0.4.2.3/MCPoly/orcaset/ssorca.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2145 2023-05-09 08:28:02.000000 MCPoly-0.4.2.3/MCPoly/orcaset/view3dchoose.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.126786 MCPoly-0.4.2.3/MCPoly/sscurve/
--rw-r--r--   0 cxs454     (503) staff       (20)     1193 2023-05-02 16:03:26.000000 MCPoly-0.4.2.3/MCPoly/sscurve/YModulus.py
--rw-r--r--   0 cxs454     (503) staff       (20)       88 2023-05-09 08:48:45.000000 MCPoly-0.4.2.3/MCPoly/sscurve/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    12770 2023-05-17 15:37:43.000000 MCPoly-0.4.2.3/MCPoly/sscurve/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     5843 2023-05-19 09:04:58.000000 MCPoly-0.4.2.3/MCPoly/sscurve/multiple.py
--rw-r--r--   0 cxs454     (503) staff       (20)     6832 2023-05-19 08:52:37.000000 MCPoly-0.4.2.3/MCPoly/sscurve/single.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.127367 MCPoly-0.4.2.3/MCPoly/status/
--rw-r--r--   0 cxs454     (503) staff       (20)       62 2023-05-18 16:46:40.000000 MCPoly-0.4.2.3/MCPoly/status/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     6202 2023-05-22 09:10:31.000000 MCPoly-0.4.2.3/MCPoly/status/echart.py
--rw-r--r--   0 cxs454     (503) staff       (20)    15750 2023-05-18 16:45:20.000000 MCPoly-0.4.2.3/MCPoly/status/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)    20682 2023-06-04 14:28:30.000000 MCPoly-0.4.2.3/MCPoly/status/status.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.127674 MCPoly-0.4.2.3/MCPoly/version/
--rw-r--r--   0 cxs454     (503) staff       (20)       23 2023-05-04 08:03:54.000000 MCPoly-0.4.2.3/MCPoly/version/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)       35 2023-06-12 17:24:12.000000 MCPoly-0.4.2.3/MCPoly/version/version.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.127946 MCPoly-0.4.2.3/MCPoly/view3d/
--rw-r--r--   0 cxs454     (503) staff       (20)       22 2023-04-30 18:16:37.000000 MCPoly-0.4.2.3/MCPoly/view3d/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     1970 2023-05-09 13:30:17.000000 MCPoly-0.4.2.3/MCPoly/view3d/view3d.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.128227 MCPoly-0.4.2.3/MCPoly/vis/
--rw-r--r--   0 cxs454     (503) staff       (20)       18 2023-05-15 14:05:55.000000 MCPoly-0.4.2.3/MCPoly/vis/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2071 2023-05-29 07:04:54.000000 MCPoly-0.4.2.3/MCPoly/vis/vis.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.122595 MCPoly-0.4.2.3/MCPoly.egg-info/
--rw-r--r--   0 cxs454     (503) staff       (20)     3675 2023-06-12 17:24:21.000000 MCPoly-0.4.2.3/MCPoly.egg-info/PKG-INFO
--rw-r--r--   0 cxs454     (503) staff       (20)     1254 2023-06-12 17:24:21.000000 MCPoly-0.4.2.3/MCPoly.egg-info/SOURCES.txt
--rw-r--r--   0 cxs454     (503) staff       (20)        1 2023-06-12 17:24:21.000000 MCPoly-0.4.2.3/MCPoly.egg-info/dependency_links.txt
--rw-r--r--   0 cxs454     (503) staff       (20)      143 2023-06-12 17:24:21.000000 MCPoly-0.4.2.3/MCPoly.egg-info/requires.txt
--rw-r--r--   0 cxs454     (503) staff       (20)        7 2023-06-12 17:24:21.000000 MCPoly-0.4.2.3/MCPoly.egg-info/top_level.txt
--rw-r--r--   0 cxs454     (503) staff       (20)     3675 2023-06-12 17:24:21.129119 MCPoly-0.4.2.3/PKG-INFO
--rw-r--r--   0 cxs454     (503) staff       (20)     3311 2023-06-12 08:44:44.000000 MCPoly-0.4.2.3/README.md
--rw-r--r--   0 cxs454     (503) staff       (20)       38 2023-06-12 17:24:21.129331 MCPoly-0.4.2.3/setup.cfg
--rw-r--r--   0 cxs454     (503) staff       (20)     1033 2023-06-12 17:23:45.000000 MCPoly-0.4.2.3/setup.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.128917 MCPoly-0.4.2.3/tests/
--rw-r--r--   0 cxs454     (503) staff       (20)     8592 2023-06-12 15:00:22.000000 MCPoly-0.4.2.3/tests/test_lmpset.py
--rw-r--r--   0 cxs454     (503) staff       (20)      799 2023-05-03 10:12:20.000000 MCPoly-0.4.2.3/tests/test_moldraw.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2932 2023-05-02 17:01:47.000000 MCPoly-0.4.2.3/tests/test_orcaset.py
--rw-r--r--   0 cxs454     (503) staff       (20)     3535 2023-05-19 13:19:19.000000 MCPoly-0.4.2.3/tests/test_sscurve.py
--rw-r--r--   0 cxs454     (503) staff       (20)     5241 2023-06-05 08:11:04.000000 MCPoly-0.4.2.3/tests/test_status.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.045613 MCPoly-0.5.0/
+-rw-r--r--   0 cxs454     (503) staff       (20)     1091 2023-05-03 15:22:57.000000 MCPoly-0.5.0/LICENSE
+-rw-r--r--   0 cxs454     (503) staff       (20)       17 2023-05-04 08:23:11.000000 MCPoly-0.5.0/MANIFEST.in
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.032032 MCPoly-0.5.0/MCPoly/
+-rw-r--r--   0 cxs454     (503) staff       (20)    14340 2023-06-12 17:23:57.000000 MCPoly-0.5.0/MCPoly/.DS_Store
+-rw-r--r--   0 cxs454     (503) staff       (20)      178 2023-05-15 14:05:30.000000 MCPoly-0.5.0/MCPoly/__init__.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.034875 MCPoly-0.5.0/MCPoly/lmpset/
+-rw-r--r--   0 cxs454     (503) staff       (20)     5719 2023-06-18 16:08:00.000000 MCPoly-0.5.0/MCPoly/lmpset/DATAtoXYZ.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     4361 2023-06-12 14:51:59.000000 MCPoly-0.5.0/MCPoly/lmpset/DATAtomolTXT.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      169 2023-06-17 16:42:13.000000 MCPoly-0.5.0/MCPoly/lmpset/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    55548 2023-06-05 13:00:53.000000 MCPoly-0.5.0/MCPoly/lmpset/chain.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    16310 2023-06-03 14:28:50.000000 MCPoly-0.5.0/MCPoly/lmpset/infchain.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    53042 2023-06-18 16:59:51.000000 MCPoly-0.5.0/MCPoly/lmpset/mould.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5425 2023-06-18 17:37:10.000000 MCPoly-0.5.0/MCPoly/lmpset/rebuild.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.037074 MCPoly-0.5.0/MCPoly/moldraw/
+-rw-r--r--   0 cxs454     (503) staff       (20)     8966 2023-05-26 12:59:21.000000 MCPoly-0.5.0/MCPoly/moldraw/C_selection.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      128 2023-05-29 06:59:26.000000 MCPoly-0.5.0/MCPoly/moldraw/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    64145 2023-05-26 10:41:02.000000 MCPoly-0.5.0/MCPoly/moldraw/bind_selection.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    24385 2023-05-29 07:03:41.000000 MCPoly-0.5.0/MCPoly/moldraw/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)   181892 2023-05-26 12:59:34.000000 MCPoly-0.5.0/MCPoly/moldraw/molecule.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    98156 2023-05-26 10:40:13.000000 MCPoly-0.5.0/MCPoly/moldraw/sub_selection.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.040334 MCPoly-0.5.0/MCPoly/orcaset/
+-rw-r--r--   0 cxs454     (503) staff       (20)     8635 2023-05-02 16:35:59.000000 MCPoly-0.5.0/MCPoly/orcaset/XYZtoINP.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      158 2023-05-11 15:49:25.000000 MCPoly-0.5.0/MCPoly/orcaset/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    16739 2023-06-16 15:10:25.000000 MCPoly-0.5.0/MCPoly/orcaset/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     7592 2023-06-07 15:00:39.000000 MCPoly-0.5.0/MCPoly/orcaset/mgui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     4842 2023-05-02 16:29:09.000000 MCPoly-0.5.0/MCPoly/orcaset/multiorca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2072 2023-05-15 15:20:42.000000 MCPoly-0.5.0/MCPoly/orcaset/orca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    19721 2023-06-16 15:10:30.000000 MCPoly-0.5.0/MCPoly/orcaset/ssgui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     9044 2023-06-09 09:20:04.000000 MCPoly-0.5.0/MCPoly/orcaset/ssorca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2145 2023-05-09 08:28:02.000000 MCPoly-0.5.0/MCPoly/orcaset/view3dchoose.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.041807 MCPoly-0.5.0/MCPoly/sscurve/
+-rw-r--r--   0 cxs454     (503) staff       (20)     1193 2023-05-02 16:03:26.000000 MCPoly-0.5.0/MCPoly/sscurve/YModulus.py
+-rw-r--r--   0 cxs454     (503) staff       (20)       88 2023-05-09 08:48:45.000000 MCPoly-0.5.0/MCPoly/sscurve/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    12770 2023-05-17 15:37:43.000000 MCPoly-0.5.0/MCPoly/sscurve/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5843 2023-05-19 09:04:58.000000 MCPoly-0.5.0/MCPoly/sscurve/multiple.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     6832 2023-05-19 08:52:37.000000 MCPoly-0.5.0/MCPoly/sscurve/single.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.042909 MCPoly-0.5.0/MCPoly/status/
+-rw-r--r--   0 cxs454     (503) staff       (20)       62 2023-05-18 16:46:40.000000 MCPoly-0.5.0/MCPoly/status/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     6192 2023-06-18 16:33:35.000000 MCPoly-0.5.0/MCPoly/status/echart.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    15750 2023-05-18 16:45:20.000000 MCPoly-0.5.0/MCPoly/status/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    21428 2023-06-18 17:31:17.000000 MCPoly-0.5.0/MCPoly/status/status.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.043338 MCPoly-0.5.0/MCPoly/version/
+-rw-r--r--   0 cxs454     (503) staff       (20)       23 2023-05-04 08:03:54.000000 MCPoly-0.5.0/MCPoly/version/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)       33 2023-06-19 08:23:12.000000 MCPoly-0.5.0/MCPoly/version/version.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.043782 MCPoly-0.5.0/MCPoly/view3d/
+-rw-r--r--   0 cxs454     (503) staff       (20)       22 2023-04-30 18:16:37.000000 MCPoly-0.5.0/MCPoly/view3d/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     1970 2023-05-09 13:30:17.000000 MCPoly-0.5.0/MCPoly/view3d/view3d.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.044378 MCPoly-0.5.0/MCPoly/vis/
+-rw-r--r--   0 cxs454     (503) staff       (20)       18 2023-05-15 14:05:55.000000 MCPoly-0.5.0/MCPoly/vis/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2071 2023-05-29 07:04:54.000000 MCPoly-0.5.0/MCPoly/vis/vis.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.032970 MCPoly-0.5.0/MCPoly.egg-info/
+-rw-r--r--   0 cxs454     (503) staff       (20)     4135 2023-06-19 08:26:12.000000 MCPoly-0.5.0/MCPoly.egg-info/PKG-INFO
+-rw-r--r--   0 cxs454     (503) staff       (20)     1279 2023-06-19 08:26:12.000000 MCPoly-0.5.0/MCPoly.egg-info/SOURCES.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)        1 2023-06-19 08:26:12.000000 MCPoly-0.5.0/MCPoly.egg-info/dependency_links.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)      143 2023-06-19 08:26:12.000000 MCPoly-0.5.0/MCPoly.egg-info/requires.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)        7 2023-06-19 08:26:12.000000 MCPoly-0.5.0/MCPoly.egg-info/top_level.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)     4135 2023-06-19 08:26:12.045436 MCPoly-0.5.0/PKG-INFO
+-rw-r--r--   0 cxs454     (503) staff       (20)     3773 2023-06-19 08:22:46.000000 MCPoly-0.5.0/README.md
+-rw-r--r--   0 cxs454     (503) staff       (20)       38 2023-06-19 08:26:12.045662 MCPoly-0.5.0/setup.cfg
+-rw-r--r--   0 cxs454     (503) staff       (20)     1031 2023-06-19 08:23:22.000000 MCPoly-0.5.0/setup.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.045229 MCPoly-0.5.0/tests/
+-rw-r--r--   0 cxs454     (503) staff       (20)     9627 2023-06-18 17:38:10.000000 MCPoly-0.5.0/tests/test_lmpset.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      799 2023-05-03 10:12:20.000000 MCPoly-0.5.0/tests/test_moldraw.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2932 2023-05-02 17:01:47.000000 MCPoly-0.5.0/tests/test_orcaset.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     3535 2023-05-19 13:19:19.000000 MCPoly-0.5.0/tests/test_sscurve.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5246 2023-06-18 16:42:29.000000 MCPoly-0.5.0/tests/test_status.py
```

### Comparing `MCPoly-0.4.2.3/LICENSE` & `MCPoly-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/.DS_Store` & `MCPoly-0.5.0/MCPoly/.DS_Store`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/lmpset/DATAtoXYZ.py` & `MCPoly-0.5.0/MCPoly/lmpset/DATAtoXYZ.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ase.io import write
 import os
 import re
 
 def DATAtoXYZ(file,loc='./',savename=''):
     """
     The method to change LAMMPS Data File into XYZ File. Powered by ASE.
-    chain(file,loc='./',savename='')
+    DATAtoXYZ(file,loc='./',savename='')
     file: Your molecule system name on your .data file.
     loc: File Location. The default is your current location.
     savename: Name of the saved XYZ File. The default is name of origin LAMMPS Data File.
     Example:
         Input:
             from MCPoly.lmpset import DATAtoXYZ
             DATAtoXYZ('Poly1_Chain')
@@ -23,17 +23,14 @@
             C       33.60940000       7.29160000       5.40582000
             H       33.81841000       6.25379000       5.63907000
             C       32.30303000       7.89744000       5.79799000
             H       31.98877000       7.45674000       6.75085000
             C       31.23940000       7.64473000       4.74277000
             
             ...
-            84 11 79 1
-            
-            ...
     """
     opath=os.getcwd()
     os.chdir(loc)
     elementsort=[]
     elements=[]
     XYZs=[]
     k=0
@@ -141,21 +138,21 @@
         c1=re.search('Atoms',line)
         if c1:
             w1=1
         elif w1==1:
             l1=re.findall(r'\-?[0-9]+\.?[0-9]*',line)
             if len(l1)>=6:
                 l.append(l1)
-                if l1[0]==num:
+                if len(l)==eval(num):
                     w1=2
         elif w1==2:
             for i4 in range(len(l)):
                 elements.append(elementsort[eval(l[i4][2])-1])
-                XYZs.append([eval(l[i4][-3]),eval(l[i4][-2]),eval(l[i4][-1])])
+                XYZs.append([eval(l[i4][4]),eval(l[i4][5]),eval(l[i4][6])])
             w1=0
     f.close()
     molecule = Atoms(elements, positions=XYZs)
     if savename=='':
-        write('{0}.xyz'.format(file),molecule)
+        write(file+'.xyz',molecule)
     else:
-        write('{0}.xyz'.format(savename),molecule)
+        write(savename+'.xyz',molecule)
     os.chdir(opath)
```

### Comparing `MCPoly-0.4.2.3/MCPoly/lmpset/DATAtomolTXT.py` & `MCPoly-0.5.0/MCPoly/lmpset/DATAtomolTXT.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/lmpset/chain.py` & `MCPoly-0.5.0/MCPoly/lmpset/chain.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/lmpset/infchain.py` & `MCPoly-0.5.0/MCPoly/lmpset/infchain.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/lmpset/mould.py` & `MCPoly-0.5.0/MCPoly/lmpset/mould.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 mydir = os.path.dirname( __file__ )
 lmpdir = os.path.join(mydir, '..', 'lmpset')
 sys.path.append(lmpdir)
 from chain import chain as normalchain
 from infchain import infchain as inf
 from DATAtomolTXT import DATAtomolTXT as ctxt
 from DATAtoXYZ import DATAtoXYZ as cxyz
+from rebuild import rebuild as rb
 
 def replication(filename,x,xgap,y,ygap,z,zgap,absolute=False,startloc=[0,0,0],loc='./',chain=False):
     if absolute==True:
         warnings.warn('Make sure you avoid all the overlaps of molecules!')
     opath=os.getcwd()
     os.chdir(loc)
     xloc=startloc[0]
@@ -968,27 +969,27 @@
         DATAtoXYZ(savename='')
         savename: Name of the saved XYZ File. The default is name of origin LAMMPS Data File.
         Example:
             Input:
                 from MCPoly.lmpset import mould
                 atoms=mould('Poly1')
                 atoms.DATAtoXYZ()
-            Output in Poly1.xyz:
+            Output in Poly1_Chain.xyz:
                 82
                 Properties=species:S:1:pos:R:3 pbc="F F F"
                 H       34.26389000       7.81856000       4.72112000
                 C       33.60940000       7.29160000       5.40582000
                 H       33.81841000       6.25379000       5.63907000
                 C       32.30303000       7.89744000       5.79799000
                 H       31.98877000       7.45674000       6.75085000
                 C       31.23940000       7.64473000       4.74277000
         
                 ...
         """
-        return cxyz(self.atoms,loc=self.loc,savename=savename)
+        return cxyz(self.atoms,self.loc,savename)
     
     def DATAtomolTXT(self,types={0:0},savename=''):
         """
         The method to change LAMMPS Data File into LAMMPS Molecule Text File.
         DATAtomolTXT(types={0:0, ...},savename='')
         file: Your molecule system name on your .data file.
         types: Change the Atom Type number to suit the main LAMMPS input files.
@@ -1061,15 +1062,15 @@
                 6 3
                 7 2
                 8 4
                 9 5
                 
                     ...
         """
-        return ctxt(self.atoms,types,loc=self.loc,savename=savename)
+        return ctxt(self.atoms,types,self.loc,savename)
     
     def infchain(self,bondtype):
         """
         The method to create a single molecule for periodical chain, specialised for polymers.
         infchain(bondtype)
         file: Your molecule system name on your .data file.
         bondtype: The bond type between the start and the end of the polymer. 
@@ -1124,8 +1125,55 @@
                 3 improper types
 
                 ...
                 82 1 83 1
 
                 ...
         """
-        return normalchain(self.atoms,bondtype,degree,self.loc)
+        return normalchain(self.atoms,bondtype,degree,self.loc)
+    
+    def rebuild(self, substitute, x=[99999,99999], y=[99999,99999], z=[99999,99999], subloc='./'):
+        """
+        The method to replace the geometry structure of LAMMPS Input File from an XYZ File.
+        rebuild(substitute, x=[xmin,xmax], y=[ymin,ymax], z=[zmin,zmax], subloc='./')
+        substitute: XYZ File used to replace.
+        x,y,z: Caption of the box.
+        subloc: XYZ File Location. The default is your current location.
+        Example:
+            Input:
+                from MCPoly.lmpset import mould
+                
+                atoms=mould('Atoms1')
+                atoms=atoms.cube(1,0,1,0,2,0) # Create the file Atoms1_112.data, see in lmpset.cube.
+                atoms.DATAtoXYZ('Atoms1_112') # Create Atoms1_112.xyz, see in lmpset.DATAtoXYZ
+                # After changing the geometry structure by GaussView or Avogrado and save it as Atoms1_replace.xyz
+                atoms.rebuild('Atoms1_replace')
+                
+            
+            Atoms1_replace.xyz:
+                106
+                
+                O          9.64263        4.67845        3.83021
+                C          9.97863        4.59047        2.66070
+                N         11.06345        5.23157        2.07395
+                O          9.31893        3.82840        1.73881
+                C         12.08548        6.09614        2.75528
+                H         11.25704        4.90681        1.13587
+                C          8.15829        2.96807        2.00836
+                ......
+            
+            Output in Atoms1_112.data:
+                ......
+                
+                Atoms
+                
+                1 1 1 -0.4804 9.64263 4.67845 3.83021
+                2 1 2 0.7694 9.97863 4.59047 2.66070
+                3 1 3 -1.1201 11.06345 5.23157 2.07395
+                4 1 4 -0.3798 9.31893 3.82840 1.73881
+                5 1 5 0.1753 12.08548 6.09614 2.75528
+                6 1 6 0.5150 11.25704 4.90681 1.13587
+                7 1 5 0.0718 8.15829 2.96807 2.00836
+                ......
+            
+    """
+        return rb(self.atoms, substitute, x=x, y=y, z=z, loc=self.loc, subloc=subloc)
```

### Comparing `MCPoly-0.4.2.3/MCPoly/moldraw/C_selection.py` & `MCPoly-0.5.0/MCPoly/moldraw/C_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/moldraw/bind_selection.py` & `MCPoly-0.5.0/MCPoly/moldraw/bind_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/moldraw/gui.py` & `MCPoly-0.5.0/MCPoly/moldraw/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/moldraw/molecule.py` & `MCPoly-0.5.0/MCPoly/moldraw/molecule.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/moldraw/sub_selection.py` & `MCPoly-0.5.0/MCPoly/moldraw/sub_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/orcaset/XYZtoINP.py` & `MCPoly-0.5.0/MCPoly/orcaset/XYZtoINP.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/orcaset/gui.py` & `MCPoly-0.5.0/MCPoly/orcaset/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,16 +247,16 @@
     roomox=widgets.ToggleButton(value=False,description='Default Space')
     corenum=widgets.IntText(description='Core:',value=4,min=1,layout=widgets.Layout(width='50%'))
     coreox=widgets.ToggleButton(value=False,description='Default CoreNumber')
     e=widgets.IntText(description='Charge:',value=0,layout=widgets.Layout(width='50%'))
     state=widgets.IntText(description='State:',value=1,layout=widgets.Layout(width='47.5%'))
     scanox=widgets.ToggleButton(value=False,description='Scan Settings',style=dict(font_weight='bold'),layout=widgets.Layout(width='98.5%'))
     forceox=widgets.ToggleButton(value=False,description='Constant External Force Settings',style=dict(font_weight='bold'),layout=widgets.Layout(width='98.5%'))
-    aim1=widgets.BoundedIntText(description='Atom 1:',value=0,min=0,layout=widgets.Layout(width='50%'))
-    aim2=widgets.BoundedIntText(description='Atom 2:',value=0,min=0,layout=widgets.Layout(width='47.5%'))
+    aim1=widgets.BoundedIntText(description='Atom 1:',value=0,min=0,max=200,layout=widgets.Layout(width='50%'))
+    aim2=widgets.BoundedIntText(description='Atom 2:',value=0,min=0,max=200,layout=widgets.Layout(width='47.5%'))
     strain=widgets.BoundedFloatText(description='Force(nN):',value=0.000,min=0.000,step=0.100)
     stretch=widgets.FloatText(description='Distance(Å):',value=1.000,step=0.100)
     scanstep=widgets.BoundedIntText(description='Steps:',value=10,min=0)
     scanout=widgets.interactive_output(scanshow, {'scanox': scanox})
     forceout=widgets.interactive_output(forceshow, {'forceox': forceox})
     eox=widgets.ToggleButton(value=False,description='Energy Status',style=dict(font_weight='bold'),layout=widgets.Layout(width='98.5%'))
     geoox=widgets.ToggleButton(value=False,description='Structure Status',style=dict(font_weight='bold'),layout=widgets.Layout(width='98.5%'))
```

### Comparing `MCPoly-0.4.2.3/MCPoly/orcaset/mgui.py` & `MCPoly-0.5.0/MCPoly/orcaset/mgui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/orcaset/multiorca.py` & `MCPoly-0.5.0/MCPoly/orcaset/multiorca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/orcaset/orca.py` & `MCPoly-0.5.0/MCPoly/orcaset/orca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/orcaset/ssgui.py` & `MCPoly-0.5.0/MCPoly/orcaset/ssgui.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,16 +321,16 @@
     method=widgets.Text(description='Method:')
     bs=widgets.Text(description='Basis Set:')
     freq=widgets.ToggleButton(value=False,description='Frequency',layout=widgets.Layout(width='33.3%'))
     room=widgets.IntText(description='Space(GB):',value=4,min=1,layout=widgets.Layout(width='50%'))
     roomox=widgets.ToggleButton(value=False,description='Default Space')
     corenum=widgets.IntText(description='Core:',value=4,min=1,layout=widgets.Layout(width='50%'))
     coreox=widgets.ToggleButton(value=False,description='Default CoreNumber')
-    aim1=widgets.BoundedIntText(description='Atom 1:',value=0,min=0,layout=widgets.Layout(width='50%'))
-    aim2=widgets.BoundedIntText(description='Atom 2:',value=0,min=0,layout=widgets.Layout(width='47.5%'))
+    aim1=widgets.BoundedIntText(description='Atom 1:',value=0,min=0,max=200,layout=widgets.Layout(width='50%'))
+    aim2=widgets.BoundedIntText(description='Atom 2:',value=0,min=0,max=200,layout=widgets.Layout(width='47.5%'))
     strain=widgets.BoundedFloatText(description='Start Force(nN):',value=0.000,min=0.000,step=0.100,style = {'description_width': 'initial'})
     addforce=widgets.BoundedFloatText(description='Force Add per Step(nN):',value=0.100,min=0.000,step=0.100,style = {'description_width': 'initial'})
     addox1=widgets.ToggleButton(value=False,description='The Second Stage',style=dict(font_weight='bold'))
     strain2=widgets.BoundedFloatText(description='Till Force(nN):',value=0.000,min=0.000,step=0.100,style = {'description_width': 'initial'})
     addforce2=widgets.BoundedFloatText(description='Force Add per Step(nN):',value=0.100,min=0.000,step=0.100,style = {'description_width': 'initial'})
     addox2=widgets.ToggleButton(value=False,description='The Third Stage',style=dict(font_weight='bold'))
     strain3=widgets.BoundedFloatText(description='Till Force(nN):',value=0.000,min=0.000,step=0.100,style = {'description_width': 'initial'})
```

### Comparing `MCPoly-0.4.2.3/MCPoly/orcaset/ssorca.py` & `MCPoly-0.5.0/MCPoly/orcaset/ssorca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/orcaset/view3dchoose.py` & `MCPoly-0.5.0/MCPoly/orcaset/view3dchoose.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/sscurve/YModulus.py` & `MCPoly-0.5.0/MCPoly/sscurve/YModulus.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/sscurve/gui.py` & `MCPoly-0.5.0/MCPoly/sscurve/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/sscurve/multiple.py` & `MCPoly-0.5.0/MCPoly/sscurve/multiple.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/sscurve/single.py` & `MCPoly-0.5.0/MCPoly/sscurve/single.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/status/echart.py` & `MCPoly-0.5.0/MCPoly/status/echart.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,26 +54,26 @@
                 a=re.search('_Result.txt', path)
                 if a:
                     files.append(path[:-11])
         files.sort()
     #print(files)
     if energy_pattern=='Energy':
         for file in files:
-            try:
-                data=status(file,loc).converged_energy()
-                datas.append(data)
-            except:
-                datas.append(None)
+            #try:
+            data=status(file,loc).converged_energy()
+            datas.append(data)
+            #except:
+            #    datas.append(None)
     elif energy_pattern=='Gibbs':
         for file in files:
-            try:
-                data=status(file,loc).gibbs()
-                datas.append(data)
-            except:
-                datas.append(None)
+            #try:
+            data=status(file,loc).gibbs()
+            datas.append(data)
+            #except:
+            #    datas.append(None)
     os.chdir(opath)
     os.chdir(loc)
     Ebar=np.array(datas)
     if absolute==False:
         Ebar=Ebar-datas[0]
     if hartree==False:
         Ebar=Ebar*627.509
```

### Comparing `MCPoly-0.4.2.3/MCPoly/status/gui.py` & `MCPoly-0.5.0/MCPoly/status/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/status/status.py` & `MCPoly-0.5.0/MCPoly/status/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,45 +150,62 @@
             if u:
                 x=2
         x3=re.search('aborting the run',line)
         if x3:
             s1=4
     if statusonly==True:
         if s2==1:
+            f.close()
+            os.chdir(path)
             return 2
         else:
+            f.close()
+            os.chdir(path)
             return s1
     if figureonly==False:
         print('{0} turns have been calculated.'.format(term))
         status_judge(s1,s2,converge)
         statusfig(energy,choose)
+    f.close()
     os.chdir(path)
     return energy
 
 def thermo(loc, file, keyword):
+    path = os.getcwd()
+    os.chdir(loc)
     f=open(file+'.out','r')
     for line in f:
         if keyword=='Gibbs':
             a=re.search('Final Gibbs free energy', line)
             if a:
                 b=re.search(r'-[0-9]+\.[0-9]+', line)
+                os.chdir(path)
+                f.close()
                 return '{0:.6f}'.format(eval(b.group(0)))
         if keyword=='Enthalpy':
             a=re.search('Total enthalpy', line)
             if a:
                 b=re.search(r'-[0-9]+\.[0-9]+', line)
+                os.chdir(path)
+                f.close()
                 return '{0:.6f}'.format(eval(b.group(0)))
         if keyword=='Entropy':
             a=re.search('Total entropy correction', line)
             if a:
                 b=re.findall(r'-[0-9]+\.[0-9]+', line)
+                os.chdir(path)
+                f.close()
                 return '{0:.6f}'.format(eval(b[0]))
+    os.chdir(path)
+    f.close()
     raise Exception("'{0}.out' may not have keyword freq, or it's aborted. Please check your input file and recalculate it.".format(file))
 
 def charge(loc, file, num, keyword):
+    path = os.getcwd()
+    os.chdir(loc)
     f=open(file+'.out','r')
     i=0
     ac=[None]*200
     for line in f:
         if keyword=='Mulliken':
             d=re.search('Sum of atomic charges',line)
             if d:
@@ -209,17 +226,20 @@
                 b=re.search(r'-?[0-9]+\.[0-9]+', line)
                 if b:
                     n=re.findall(r'[0-9]+', line)
                     ac[eval(n[0])]=eval(b.group(0))
             d=re.search('LOEWDIN REDUCED ORBITAL CHARGES',line)
             if d:
                 i=0
+    os.chdir(path)
     return ac[num]
 
 def atoms_all(loc, file):
+    path = os.getcwd()
+    os.chdir(loc)
     f=open(file+'.out','r')
     i=0
     n=0
     atoms=[['NOT','99999','99999','99999']]*200
     elements=['NOT']*200
     xyzs=[['99999','99999','99999']]*200
     for line in f:
@@ -236,54 +256,59 @@
                 except:
                     elements.append(b.group(0))
                 try:
                     xyzs[n]=xyz
                 except:
                     xyzs.append(xyz)
                 try:
-                    atoms[n]=[b.group(0),*xyz]
+                    atoms[n]=[b.group(0),eval(xyz[0]),eval(xyz[1]),eval(xyz[2])]
                 except:
-                    atoms.append([b.group(0),*xyz])
+                    atoms.append([b.group(0),eval(xyz[0]),eval(xyz[1]),eval(xyz[2])])
                 n=n+1
         a=re.search('CARTESIAN COORDINATES \(ANGSTROEM\)',line)
         if a:
             i=1
     while 1:
         try:
             atoms.remove(['NOT','99999','99999','99999'])
             elements.remove('NOT')
             xyzs.remove(['99999','99999','99999'])
         except:
             break
     f.close()
+    os.chdir(path)
     return atoms
 
-def atoms_all_xyz(loc, file):
+def atoms_all_xyz(loc, file,transfer=False):
+    path = os.getcwd()
+    if transfer==False:
+        os.chdir(loc)
     f=open(file+'.xyz','r')
     atoms=[['NOT','99999','99999','99999']]*200
     elements=['NOT']*200
     xyzs=[['99999','99999','99999']]*200
     i=0
     for line in f:
         b=re.findall(r'-?[0-9]+\.[0-9]+', line)
         if len(b)==3:
             ele=re.search(r'[A-Z][a-z]?', line)
             try:
-                atoms[i]=[ele.group(0),*b]
+                atoms[i]=[ele.group(0),eval(b[0]),eval(b[1]),eval(b[2])]
             except:
-                atoms.append([ele.group(0),*b])
+                atoms.append([ele.group(0),eval(b[0]),eval(b[1]),eval(b[2])])
         i=i+1
     while 1:
         try:
             atoms.remove(['NOT','99999','99999','99999'])
             elements.remove('NOT')
             xyzs.remove(['99999','99999','99999'])
         except:
             break
     f.close()
+    os.chdir(path)
     return atoms
 
 class status:
     """
     A method to see the current process of the ORCA optimisation, including convergence situation and relevant energy chart.
     status(file, loc='./')
     file: File Name.
@@ -432,15 +457,15 @@
     TIPS: In the following list, a piece of atom information is like that:
         ['C', 4.11199532065866, 1.93907233706568, -1.49149364116961]
         The first one is the element type, the following three numbers are location in x,y,z-axis.
         """
         try:
             return atoms_all(self.loc,self.file)
         except:
-            return atoms_all_xyz(self.loc,self.file)
+            return atoms_all_xyz(self.loc,self.file,transfer=True)
     
     def mass(self):
         """
     A method to find out the mass of all particles in system.
     mass()
         """
         M=0
@@ -513,15 +538,15 @@
                 M=M+192.22
             elif i[0]=='Pt':
                 M=M+195.08
             elif i[0]=='Au':
                 M=M+196.97
             elif i[0]=='Hg':
                 M=M+200.59
-        return M
+        return eval('{0:.3f}'.format(M))
     
     def atom_num(self):
         """
     A method to find out the atom number of the system.
     atom_num()
         """
         return len(atoms_all(self.loc,self.file))
```

### Comparing `MCPoly-0.4.2.3/MCPoly/view3d/view3d.py` & `MCPoly-0.5.0/MCPoly/view3d/view3d.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly/vis/vis.py` & `MCPoly-0.5.0/MCPoly/vis/vis.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/MCPoly.egg-info/PKG-INFO` & `MCPoly-0.5.0/MCPoly.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCPoly
-Version: 0.4.2.3
+Version: 0.5.0
 Summary: Useful tools for Computational Chemistry for polymers
 Home-page: https://github.com/Omicron-Fluor/MCPoly/
 Author: Omicron Fluor
 Author-email: cxs454@student.bham.ac.uk
 License: MIT
 Keywords: ORCA,Mechanical Property,Computational Chemistry
 Description-Content-Type: text/markdown
@@ -13,15 +13,23 @@
 # MCPoly
 Some methods to deal with some manipulation of computational chemistry, mostly about mechanical properties of polymers.
 ![](./reference/function.png)
 
 ## Overview
 `MCPoly` is a Python library to make some steps of computational chemistry easier. It includes some functions of drawing molecule structures, creating proper .xyz , .inp , .mol and .data file, which specialised for using ORCA and LAMMPS, and some functions for researching the mechanical property of some polymers.
 
-## Updated in v0.4.2.2(12.06.23)
+## Updated in v0.5.0(19.06.23)
+1. Add 'rebuild' in 'lmpset' package. You can now use it to rebuild geometry structure of LAMMPS input data now.
+2. Add 'DATAtoXYZ' in 'lmpset' package to convert LAMMPS Data File into XYZ File
+3. Add 'DATAtomolTXT' to convert LAMMPS Data File into LAMMPS Molecule Text File.
+4. All these functions can be used by lmpset.mould().XXX() now.
+5. Fix some bugs about ORCA Calculations Settings
+6. Fix some bugs about ORCA GUI display
+
+## Updated in v0.4.2.3(12.06.23)
 1. BIG UPDATE: Molecule Designer GUI is included in this package. You can now use it to draw molecule with 3D view at the same time.
 <img src="https://github.com/Omicron-Fluor/MCPoly/blob/main/reference/moldraw_gui.png">
 2. Add 'chain' in 'lmpset' package. You can now use it to convert periodic polymer structure input data now.
 3. Fix some bugs about ORCA Calculations
 4. Fix some bugs about calculating stress-strain curve
 
 ## Updated in v0.3.0 (19.05.23)
```

### Comparing `MCPoly-0.4.2.3/MCPoly.egg-info/SOURCES.txt` & `MCPoly-0.5.0/MCPoly.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 MCPoly.egg-info/top_level.txt
 MCPoly/lmpset/DATAtoXYZ.py
 MCPoly/lmpset/DATAtomolTXT.py
 MCPoly/lmpset/__init__.py
 MCPoly/lmpset/chain.py
 MCPoly/lmpset/infchain.py
 MCPoly/lmpset/mould.py
+MCPoly/lmpset/rebuild.py
 MCPoly/moldraw/C_selection.py
 MCPoly/moldraw/__init__.py
 MCPoly/moldraw/bind_selection.py
 MCPoly/moldraw/gui.py
 MCPoly/moldraw/molecule.py
 MCPoly/moldraw/sub_selection.py
 MCPoly/orcaset/XYZtoINP.py
```

### Comparing `MCPoly-0.4.2.3/PKG-INFO` & `MCPoly-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCPoly
-Version: 0.4.2.3
+Version: 0.5.0
 Summary: Useful tools for Computational Chemistry for polymers
 Home-page: https://github.com/Omicron-Fluor/MCPoly/
 Author: Omicron Fluor
 Author-email: cxs454@student.bham.ac.uk
 License: MIT
 Keywords: ORCA,Mechanical Property,Computational Chemistry
 Description-Content-Type: text/markdown
@@ -13,15 +13,23 @@
 # MCPoly
 Some methods to deal with some manipulation of computational chemistry, mostly about mechanical properties of polymers.
 ![](./reference/function.png)
 
 ## Overview
 `MCPoly` is a Python library to make some steps of computational chemistry easier. It includes some functions of drawing molecule structures, creating proper .xyz , .inp , .mol and .data file, which specialised for using ORCA and LAMMPS, and some functions for researching the mechanical property of some polymers.
 
-## Updated in v0.4.2.2(12.06.23)
+## Updated in v0.5.0(19.06.23)
+1. Add 'rebuild' in 'lmpset' package. You can now use it to rebuild geometry structure of LAMMPS input data now.
+2. Add 'DATAtoXYZ' in 'lmpset' package to convert LAMMPS Data File into XYZ File
+3. Add 'DATAtomolTXT' to convert LAMMPS Data File into LAMMPS Molecule Text File.
+4. All these functions can be used by lmpset.mould().XXX() now.
+5. Fix some bugs about ORCA Calculations Settings
+6. Fix some bugs about ORCA GUI display
+
+## Updated in v0.4.2.3(12.06.23)
 1. BIG UPDATE: Molecule Designer GUI is included in this package. You can now use it to draw molecule with 3D view at the same time.
 <img src="https://github.com/Omicron-Fluor/MCPoly/blob/main/reference/moldraw_gui.png">
 2. Add 'chain' in 'lmpset' package. You can now use it to convert periodic polymer structure input data now.
 3. Fix some bugs about ORCA Calculations
 4. Fix some bugs about calculating stress-strain curve
 
 ## Updated in v0.3.0 (19.05.23)
```

### Comparing `MCPoly-0.4.2.3/README.md` & `MCPoly-0.5.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 # MCPoly
 Some methods to deal with some manipulation of computational chemistry, mostly about mechanical properties of polymers.
 ![](./reference/function.png)
 
 ## Overview
 `MCPoly` is a Python library to make some steps of computational chemistry easier. It includes some functions of drawing molecule structures, creating proper .xyz , .inp , .mol and .data file, which specialised for using ORCA and LAMMPS, and some functions for researching the mechanical property of some polymers.
 
-## Updated in v0.4.2.2(12.06.23)
+## Updated in v0.5.0(19.06.23)
+1. Add 'rebuild' in 'lmpset' package. You can now use it to rebuild geometry structure of LAMMPS input data now.
+2. Add 'DATAtoXYZ' in 'lmpset' package to convert LAMMPS Data File into XYZ File
+3. Add 'DATAtomolTXT' to convert LAMMPS Data File into LAMMPS Molecule Text File.
+4. All these functions can be used by lmpset.mould().XXX() now.
+5. Fix some bugs about ORCA Calculations Settings
+6. Fix some bugs about ORCA GUI display
+
+## Updated in v0.4.2.3(12.06.23)
 1. BIG UPDATE: Molecule Designer GUI is included in this package. You can now use it to draw molecule with 3D view at the same time.
 <img src="https://github.com/Omicron-Fluor/MCPoly/blob/main/reference/moldraw_gui.png">
 2. Add 'chain' in 'lmpset' package. You can now use it to convert periodic polymer structure input data now.
 3. Fix some bugs about ORCA Calculations
 4. Fix some bugs about calculating stress-strain curve
 
 ## Updated in v0.3.0 (19.05.23)
```

### Comparing `MCPoly-0.4.2.3/setup.py` & `MCPoly-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='MCPoly',
-    version='0.4.2.3',
+    version='0.5.0',
     description='Useful tools for Computational Chemistry for polymers',
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=['MCPoly','MCPoly.lmpset','MCPoly.moldraw','MCPoly.orcaset','MCPoly.sscurve','MCPoly.status','MCPoly.view3d','MCPoly.version','MCPoly.vis'],
     author='Omicron Fluor',
     author_email='cxs454@student.bham.ac.uk',
```

### Comparing `MCPoly-0.4.2.3/tests/test_lmpset.py` & `MCPoly-0.5.0/tests/test_lmpset.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,53 +205,53 @@
             i9=1
             break
     fl.close()
     assert i1*i2*i3*i4*i5*i6*i7*i8*i9!=0
 
 @pytest.fixture
 def atoms():
-    return mould('Poly1',loc='./data_lmpset/')
+    return mould('Poly2',loc='./data_lmpset/')
 
 def test_DATAtoXYZ(atoms):
     opath=os.getcwd()
     os.chdir('./MCPoly/tests')
     atoms.DATAtoXYZ()
     os.chdir(opath)
-    fl=open('./MCPoly/tests/data_lmpset/Poly1.xyz','r')
+    fl=open('./MCPoly/tests/data_lmpset/Poly2.xyz','r')
     i1=0
     i2=0
     i3=0
     i4=0
     for line in fl:
         a=re.match('9',line)
         if a:
             i1=1
-        b=re.search('C       -7.66670000       0.30320000      -0.05380000',line)
+        b=re.search('C       -6.94821584       1.31130517      -1.06055707',line)
         if b:
             i2=1
-        c=re.search('O       -7.72351010       0.80779380       2.29626760',line)
+        c=re.search('H       -7.85312000       0.69751000      -1.04387000',line)
         if c:
             i3=1
-        d=re.search('H       -8.04585390      -0.09712450       2.44769150',line)
+        d=re.search('O       -4.55939129       1.28068339      -1.05975265',line)
         if d:
             i4=1
             break
     fl.close()
     assert i1*i2*i3*i4!=0
 
 @pytest.fixture
 def atoms():
     return mould('Poly1',loc='./data_lmpset/')
 
 def test1_DATAtomolTXT(atoms):
     opath=os.getcwd()
     os.chdir('./MCPoly/tests')
-    atoms.DATAtomolTXT()
+    atoms.DATAtomolTXT(savename='Poly1_1')
     os.chdir(opath)
-    fl=open('./MCPoly/tests/data_lmpset/Poly1.txt','r')
+    fl=open('./MCPoly/tests/data_lmpset/Poly1_1.txt','r')
     i1=0
     i2=0
     i3=1
     i4=0
     i5=0
     i6=0
     i7=0
@@ -292,17 +292,17 @@
             break
     fl.close()
     assert i1*i2*i3*i4*i5*i6*i7*i8*i9*i10!=0
 
 def test2_DATAtomolTXT(atoms):
     opath=os.getcwd()
     os.chdir('./MCPoly/tests')
-    atoms.DATAtomolTXT(types={1:11},savename='Poly1_2')
+    atoms.DATAtomolTXT(types={1:11},savename='Poly1_3')
     os.chdir(opath)
-    fl=open('./MCPoly/tests/data_lmpset/Poly1_2.txt','r')
+    fl=open('./MCPoly/tests/data_lmpset/Poly1_3.txt','r')
     i1=0
     i2=0
     i3=0
     for line in fl:
         a=re.match('2 11',line)
         if a:
             i1=1
@@ -383,8 +383,47 @@
         if e:
             i5=1
         f=re.match('12 2 14 10',line)
         if f:
             i6=1
             break
     fl.close()
+    assert i1*i2*i3*i4*i5*i6!=0
+
+@pytest.fixture
+def atoms3():
+    return mould('Poly3',loc='./data_lmpset/')
+
+def test_rebuild(atoms3):
+    opath=os.getcwd()
+    os.chdir('./MCPoly/tests')
+    atoms3.rebuild('Poly3_re',x=[-50,50], y=[-50,50], z=[-50,50],subloc='./data_lmpset/')
+    os.chdir(opath)
+    fl=open('./MCPoly/tests/data_lmpset/Poly3.data','r')
+    i1=0
+    i2=0
+    i3=0
+    i4=0
+    i5=0
+    i6=0
+    for line in fl:
+        a=re.search('-50.00000 50.00000 xlo xhi',line)
+        if a:
+            i1=1
+        b=re.search('-50.00000 50.00000 ylo yhi',line)
+        if b:
+            i2=1
+        c=re.search('-50.00000 50.00000 zlo zhi',line)
+        if c:
+            i3=1
+        d=re.search('2 1 2 0.7694 9.97863 4.59047 2.66070',line)
+        if d:
+            i4=1
+        e=re.search('10 1 7 0.1191 11.55624 6.78551 3.42033',line)
+        if e:
+            i5=1
+        f=re.search('73 1 8 -0.4064 19.29389 5.70762 2.26849',line)
+        if f:
+            i6=1
+            break
+    fl.close()
     assert i1*i2*i3*i4*i5*i6!=0
```

### Comparing `MCPoly-0.4.2.3/tests/test_moldraw.py` & `MCPoly-0.5.0/tests/test_moldraw.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/tests/test_orcaset.py` & `MCPoly-0.5.0/tests/test_orcaset.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/tests/test_sscurve.py` & `MCPoly-0.5.0/tests/test_sscurve.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.3/tests/test_status.py` & `MCPoly-0.5.0/tests/test_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,8 +202,9 @@
     assert num==14
 
 def test_status_mass(current1):
     opath=os.getcwd()
     os.chdir('./MCPoly/tests')
     num=current1.mass()
     os.chdir(opath)
-    assert num==207.015
+    assert num==238.024
+
```

