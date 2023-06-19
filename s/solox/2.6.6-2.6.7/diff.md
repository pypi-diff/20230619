# Comparing `tmp/solox-2.6.6.tar.gz` & `tmp/solox-2.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-dj6s18av/solox-2.6.6.tar", last modified: Wed Jun 14 03:07:52 2023, max compression
+gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-5wsd0zoo/solox-2.6.7.tar", last modified: Mon Jun 19 10:07:24 2023, max compression
```

## Comparing `solox-2.6.6.tar` & `solox-2.6.7.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-14 03:07:43.000000 solox-2.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-14 03:07:43.000000 solox-2.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-14 03:07:52.000000 solox-2.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-14 03:07:43.000000 solox-2.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-14 03:07:52.000000 solox-2.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-14 03:07:43.000000 solox-2.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-14 03:07:43.000000 solox-2.6.6/solox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-14 03:07:43.000000 solox-2.6.6/solox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-14 03:07:43.000000 solox-2.6.6/solox/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/public/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/_iosPerf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/public/adb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/public/adb/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/adb/linux/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/public/adb/linux_arm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/adb/linux_arm/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/public/adb/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/adb/mac/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/public/adb/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/adb/windows/AdbWinApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/adb/windows/AdbWinUsbApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/adb/windows/adb.exe
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)    21834 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/apm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/apm_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)    32904 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/fps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/public/iosperf/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30884 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    41300 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_hexdump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_imagemounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)    39237 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_ipautil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_safe_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/_wdaproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/bplist.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/plistlib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/requests_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/iosperf/struct2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/public/report_template/
--rw-r--r--   0 runner    (1001) docker     (123)    29240 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/report_template/android.html
--rw-r--r--   0 runner    (1001) docker     (123)    29276 2023-06-14 03:07:43.000000 solox-2.6.6/solox/public/report_template/ios.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/css/highlight.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/css/select2-bootstrap-5-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/css/sweetalert2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/css/tabler.demo.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/css/tabler.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/static/image/
--rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/image/404.png
--rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/image/500.png
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/image/avatar.png
--rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/image/coffee.png
--rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/image/empty.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/static/image/readme/
--rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/image/readme/home.png
--rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/image/readme/pk.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/js/apexcharts.js
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/js/gray.js
--rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/js/highstock.js
--rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/js/html2canvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/js/socket.io.js
--rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/js/sweetalert2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/js/tabler.demo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/js/tabler.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-06-14 03:07:43.000000 solox-2.6.6/solox/static/logo/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-06-14 03:07:43.000000 solox-2.6.6/solox/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-06-14 03:07:43.000000 solox-2.6.6/solox/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)    65911 2023-06-14 03:07:43.000000 solox-2.6.6/solox/templates/analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)    43308 2023-06-14 03:07:43.000000 solox-2.6.6/solox/templates/analysis_compare.html
--rw-r--r--   0 runner    (1001) docker     (123)    38458 2023-06-14 03:07:43.000000 solox-2.6.6/solox/templates/analysis_pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    35262 2023-06-14 03:07:43.000000 solox-2.6.6/solox/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)   101321 2023-06-14 03:07:43.000000 solox-2.6.6/solox/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    55677 2023-06-14 03:07:43.000000 solox-2.6.6/solox/templates/pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-06-14 03:07:43.000000 solox-2.6.6/solox/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox/view/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 03:07:43.000000 solox-2.6.6/solox/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30915 2023-06-14 03:07:43.000000 solox-2.6.6/solox/view/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-06-14 03:07:43.000000 solox-2.6.6/solox/view/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-14 03:07:43.000000 solox-2.6.6/solox/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:07:52.000000 solox-2.6.6/solox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-14 03:07:52.000000 solox-2.6.6/solox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-14 03:07:52.000000 solox-2.6.6/solox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:07:52.000000 solox-2.6.6/solox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 03:07:52.000000 solox-2.6.6/solox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 03:07:52.000000 solox-2.6.6/solox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-19 10:07:14.000000 solox-2.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-19 10:07:14.000000 solox-2.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-19 10:07:24.000000 solox-2.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-19 10:07:14.000000 solox-2.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-19 10:07:24.000000 solox-2.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-19 10:07:14.000000 solox-2.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-19 10:07:14.000000 solox-2.6.7/solox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-19 10:07:14.000000 solox-2.6.7/solox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-19 10:07:14.000000 solox-2.6.7/solox/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/_iosPerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/adb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/adb/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/adb/linux/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/adb/linux_arm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/adb/linux_arm/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/adb/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/adb/mac/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/adb/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/adb/windows/AdbWinApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/adb/windows/AdbWinUsbApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/adb/windows/adb.exe
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21836 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/apm_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32917 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/fps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/iosperf/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30884 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41300 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_hexdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_imagemounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39237 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_ipautil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_safe_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_wdaproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/bplist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/plistlib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/requests_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/struct2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/report_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    29411 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/report_template/android.html
+-rw-r--r--   0 runner    (1001) docker     (123)    29447 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/report_template/ios.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/css/highlight.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/css/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/css/sweetalert2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/css/tabler.demo.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/css/tabler.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/static/image/
+-rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/image/404.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/image/500.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/image/avatar.png
+-rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/image/coffee.png
+-rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/image/empty.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/static/image/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/image/readme/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/image/readme/pk.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/apexcharts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/gray.js
+-rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/highstock.js
+-rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/html2canvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/socket.io.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/sweetalert2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/tabler.demo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/tabler.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/logo/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)    65914 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)    43489 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/analysis_compare.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38461 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/analysis_pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    33843 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)   101320 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    55683 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 10:07:14.000000 solox-2.6.7/solox/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30915 2023-06-19 10:07:14.000000 solox-2.6.7/solox/view/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-06-19 10:07:14.000000 solox-2.6.7/solox/view/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-19 10:07:14.000000 solox-2.6.7/solox/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-19 10:07:24.000000 solox-2.6.7/solox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-19 10:07:24.000000 solox-2.6.7/solox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 10:07:24.000000 solox-2.6.7/solox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-19 10:07:24.000000 solox-2.6.7/solox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 10:07:24.000000 solox-2.6.7/solox.egg-info/top_level.txt
```

### Comparing `solox-2.6.6/LICENSE` & `solox-2.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/PKG-INFO` & `solox-2.6.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solox
-Version: 2.6.6
+Version: 2.6.7
 Summary: SoloX - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/smart-test-ti/SoloX
 Author: Rafa Chen
 Author-email: rafacheninc@gamil.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,15 +33,15 @@
 
 ## 🔎Preview
 
 SoloX - Real-time collection tool for Android/iOS performance data.
 
 We are committed to solving inefficient, cumbersome test execution, and our goal is Simple Test In SoloX!
 
-![preview](https://github.com/smart-test-ti/SoloX/assets/24454096/6941452f-6410-4730-a532-0d69d0f7fdb8)
+![preview](https://github.com/smart-test-ti/SoloX/assets/24454096/4d9d9dab-9e24-4327-a60a-84f14b79206d)
 
 ## 📦Requirements
 
 - Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
 - Install adb and configure environment variables (SoloX's  adb may not necessarily fit your computer) [**Download**](https://developer.android.com/studio/releases/platform-tools)
 
 💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4.
```

### Comparing `solox-2.6.6/README.md` & `solox-2.6.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 ## 🔎Preview
 
 SoloX - Real-time collection tool for Android/iOS performance data.
 
 We are committed to solving inefficient, cumbersome test execution, and our goal is Simple Test In SoloX!
 
-![preview](https://github.com/smart-test-ti/SoloX/assets/24454096/6941452f-6410-4730-a532-0d69d0f7fdb8)
+![preview](https://github.com/smart-test-ti/SoloX/assets/24454096/4d9d9dab-9e24-4327-a60a-84f14b79206d)
 
 ## 📦Requirements
 
 - Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
 - Install adb and configure environment variables (SoloX's  adb may not necessarily fit your computer) [**Download**](https://developer.android.com/studio/releases/platform-tools)
 
 💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4.
```

### Comparing `solox-2.6.6/setup.py` & `solox-2.6.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     install_requires=['flask>=2.0.1', 'requests', 'logzero', 'Flask-SocketIO==4.3.1', 'fire',
                       'python-engineio==3.13.2', 'python-socketio==4.6.0', 'Werkzeug==2.0.3',
-                      'Jinja2==3.0.1','tidevice==0.9.7', 'tqdm', 'xlwt'],
+                      'Jinja2==3.0.1','tidevice==0.9.7', 'tqdm', 'xlwt','pyfiglet'],
     version=__version__,
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="SoloX - Real-time collection tool for Android/iOS performance data.",
     packages=setuptools.find_namespace_packages(include=["solox", "solox.*"], ),
     include_package_data=True
 )
```

### Comparing `solox-2.6.6/solox/__main__.py` & `solox-2.6.7/solox/__main__.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/debug.py` & `solox-2.6.7/solox/debug.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/_iosPerf.py` & `solox-2.6.7/solox/public/_iosPerf.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/adb/mac/adb` & `solox-2.6.7/solox/public/adb/mac/adb`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/adb.py` & `solox-2.6.7/solox/public/adb.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/apm.py` & `solox-2.6.7/solox/public/apm.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         return sysCpu
 
     def getAndroidCpuRate(self, noLog=False):
         """get the Android cpu rate of a process"""
         processCpuTime_1 = self.getprocessCpuStat()
         totalCpuTime_1 = self.getTotalCpuStat()
         sysCpuTime_1 = self.getSysCpuStat()
-        time.sleep(1)
+        time.sleep(0.5)
         processCpuTime_2 = self.getprocessCpuStat()
         totalCpuTime_2 = self.getTotalCpuStat()
         sysCpuTime_2 = self.getSysCpuStat()
         appCpuRate = round(float((processCpuTime_2 - processCpuTime_1) / (totalCpuTime_2 - totalCpuTime_1) * 100), 2)
         sysCpuRate = round(float((sysCpuTime_2 - sysCpuTime_1) / (totalCpuTime_2 - totalCpuTime_1) * 100), 2)
         if noLog is False:
             apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
```

### Comparing `solox-2.6.6/solox/public/apm_pk.py` & `solox-2.6.7/solox/public/apm_pk.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/common.py` & `solox-2.6.7/solox/public/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -700,16 +700,16 @@
             with(open(os.path.join(path, name), 'ab')) as f:
                 for chunk in req.iter_content(chunk_size=1024):
                     if chunk:
                          f.write(chunk)
                          pbar.update(1024)
             pbar.close()
             return True
-        except:
-            traceback.print_exc()
+        except Exception as e:
+            logger.exception(e)
             return False
 
     def installAPK(self, path):
         result = adb.shell_noDevice(cmd='install -r {}'.format(path))
         if result == 0:
             os.remove(path)
             return True, result
```

### Comparing `solox-2.6.6/solox/public/fps.py` & `solox-2.6.7/solox/public/fps.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/__main__.py` & `solox-2.6.7/solox/public/iosperf/__main__.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_crash.py` & `solox-2.6.7/solox/public/iosperf/_crash.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_device.py` & `solox-2.6.7/solox/public/iosperf/_device.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_hexdump.py` & `solox-2.6.7/solox/public/iosperf/_hexdump.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_imagemounter.py` & `solox-2.6.7/solox/public/iosperf/_imagemounter.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_installation.py` & `solox-2.6.7/solox/public/iosperf/_installation.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_instruments.py` & `solox-2.6.7/solox/public/iosperf/_instruments.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_ipautil.py` & `solox-2.6.7/solox/public/iosperf/_ipautil.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_perf.py` & `solox-2.6.7/solox/public/iosperf/_perf.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_proto.py` & `solox-2.6.7/solox/public/iosperf/_proto.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_relay.py` & `solox-2.6.7/solox/public/iosperf/_relay.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_safe_socket.py` & `solox-2.6.7/solox/public/iosperf/_safe_socket.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_ssl.py` & `solox-2.6.7/solox/public/iosperf/_ssl.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_sync.py` & `solox-2.6.7/solox/public/iosperf/_sync.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_types.py` & `solox-2.6.7/solox/public/iosperf/_types.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_usbmux.py` & `solox-2.6.7/solox/public/iosperf/_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_utils.py` & `solox-2.6.7/solox/public/iosperf/_utils.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/_wdaproxy.py` & `solox-2.6.7/solox/public/iosperf/_wdaproxy.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/bplist.py` & `solox-2.6.7/solox/public/iosperf/bplist.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/exceptions.py` & `solox-2.6.7/solox/public/iosperf/exceptions.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/plistlib2.py` & `solox-2.6.7/solox/public/iosperf/plistlib2.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/requests_usbmux.py` & `solox-2.6.7/solox/public/iosperf/requests_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/iosperf/struct2.py` & `solox-2.6.7/solox/public/iosperf/struct2.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/public/report_template/android.html` & `solox-2.6.7/solox/public/report_template/android.html`

 * *Files 1% similar despite different names*

```diff
@@ -385,14 +385,21 @@
             grid: {
                 padding: {
                     top: -20,
                     bottom: -4
                 },
             strokeDashArray: 4,
             },
+            xaxis: {
+                name: "time",
+                tickAmount:6,
+                labels: {
+                    rotate: 0,
+                }
+            },
         };
         return options
     }
 
     var cpu_chart = new ApexCharts(document.querySelector("#chart-cpu"), options('line'));
     cpu_chart.render();
     cpu_chart.updateSeries([{
```

### Comparing `solox-2.6.6/solox/public/report_template/ios.html` & `solox-2.6.7/solox/public/report_template/ios.html`

 * *Files 1% similar despite different names*

```diff
@@ -386,14 +386,21 @@
             grid: {
                 padding: {
                     top: -20,
                     bottom: -4
                 },
             strokeDashArray: 4,
             },
+            xaxis: {
+                name: "time",
+                tickAmount:6,
+                labels: {
+                    rotate: 0,
+                }
+            },
         };
         return options
     }
 
     var cpu_chart = new ApexCharts(document.querySelector("#chart-cpu"), options('line'));
     cpu_chart.render();
     cpu_chart.updateSeries([{
```

### Comparing `solox-2.6.6/solox/static/css/highlight.min.css` & `solox-2.6.7/solox/static/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/css/select2-bootstrap-5-theme.min.css` & `solox-2.6.7/solox/static/css/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/css/select2-bootstrap-5-theme.rtl.min.css` & `solox-2.6.7/solox/static/css/select2-bootstrap-5-theme.rtl.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/css/select2.min.css` & `solox-2.6.7/solox/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/css/sweetalert2.min.css` & `solox-2.6.7/solox/static/css/sweetalert2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/css/tabler.demo.min.css` & `solox-2.6.7/solox/static/css/tabler.demo.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/css/tabler.min.css` & `solox-2.6.7/solox/static/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/image/404.png` & `solox-2.6.7/solox/static/image/404.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/image/500.png` & `solox-2.6.7/solox/static/image/500.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/image/avatar.png` & `solox-2.6.7/solox/static/image/avatar.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/image/coffee.png` & `solox-2.6.7/solox/static/image/coffee.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/image/empty.png` & `solox-2.6.7/solox/static/image/empty.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/image/readme/home.png` & `solox-2.6.7/solox/static/image/readme/home.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/image/readme/pk.png` & `solox-2.6.7/solox/static/image/readme/pk.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/js/apexcharts.js` & `solox-2.6.7/solox/static/js/apexcharts.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/js/gray.js` & `solox-2.6.7/solox/static/js/gray.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/js/highlight.min.js` & `solox-2.6.7/solox/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/js/highstock.js` & `solox-2.6.7/solox/static/js/highstock.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/js/html2canvas.min.js` & `solox-2.6.7/solox/static/js/html2canvas.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/js/jquery.min.js` & `solox-2.6.7/solox/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/js/select2.min.js` & `solox-2.6.7/solox/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/js/socket.io.js` & `solox-2.6.7/solox/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/js/sweetalert2.min.js` & `solox-2.6.7/solox/static/js/sweetalert2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/js/tabler.demo.min.js` & `solox-2.6.7/solox/static/js/tabler.demo.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/js/tabler.min.js` & `solox-2.6.7/solox/static/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/static/logo/logo.png` & `solox-2.6.7/solox/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/templates/404.html` & `solox-2.6.7/solox/templates/404.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/templates/500.html` & `solox-2.6.7/solox/templates/500.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/templates/analysis.html` & `solox-2.6.7/solox/templates/analysis.html`

 * *Files 0% similar despite different names*

```diff
@@ -416,15 +416,15 @@
         </div>
         <div class="card-body">
             <div id="chart-cpu"></div>
         </div>
     </div>
     <div class="card mem-card mt-3">
         <div class="card-header">
-            <div class='card-title'>MEM（MB）</div>
+            <div class='card-title'>Memory（MB）</div>
             <div class="card-actions btn-actions">
                 <a class="btn-action cursor-pointer" id="mem_loading">
                     <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
                 </a>
                 <a class="btn-action cursor-pointer" id="mem_png" onclick="screenshot('mem-card','mem.png')">
                     <svg t="1646303797379" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5790" width="2000" height="2000"><path d="M897.856 842.56c14.464-6.72 18.624-20.48 9.28-30.848l-241.216-263.296a25.792 25.792 0 0 0-7.68-5.888c-14.016-7.296-33.6-5.184-43.776 4.8l-241.152 233.088-103.808-70.528a30.912 30.912 0 0 0-3.52-1.92c-14.08-7.36-33.664-4.992-43.776 4.864l-101.056 97.728a18.368 18.368 0 0 0-6.08 13.952c0.512 12.288 14.848 22.016 32.128 21.696h732.8a40.768 40.768 0 0 0 17.856-3.648zM259.84 399.68a78.464 78.464 0 0 0 117.504 67.84 78.272 78.272 0 0 0 0-135.744A78.208 78.208 0 0 0 259.84 399.68" p-id="5791"></path><path d="M864.832 872.256H159.232a83.84 83.84 0 0 1-83.776-83.776V235.52a83.84 83.84 0 0 1 83.776-83.776h705.536a83.84 83.84 0 0 1 83.776 83.776v552.96a83.84 83.84 0 0 1-83.712 83.776zM159.232 183.744a51.84 51.84 0 0 0-51.776 51.776v552.96a51.84 51.84 0 0 0 51.776 51.776h705.536a51.84 51.84 0 0 0 51.776-51.776V235.52a51.84 51.84 0 0 0-51.776-51.776H159.232z" p-id="5792"></path></svg>
                 </a>
```

### Comparing `solox-2.6.6/solox/templates/analysis_compare.html` & `solox-2.6.7/solox/templates/analysis_compare.html`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         </div>
         <div class="card-body">
             <div id="chart-cpu"></div>
         </div>
     </div>
     <div class="card mem-card mt-3">
         <div class="card-header">
-            <div class='card-title'>MEM（MB）: Total Usage</div>
+            <div class='card-title'>Memory（MB）: Total Usage</div>
             <div class="card-actions btn-actions">
                 <a class="btn-action cursor-pointer" id="mem_loading">
                     <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
                 </a>
                 <a class="btn-action cursor-pointer" id="mem_png" onclick="screenshot('mem-card','mem.png')">
                     <svg t="1646303797379" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5790" width="2000" height="2000"><path d="M897.856 842.56c14.464-6.72 18.624-20.48 9.28-30.848l-241.216-263.296a25.792 25.792 0 0 0-7.68-5.888c-14.016-7.296-33.6-5.184-43.776 4.8l-241.152 233.088-103.808-70.528a30.912 30.912 0 0 0-3.52-1.92c-14.08-7.36-33.664-4.992-43.776 4.864l-101.056 97.728a18.368 18.368 0 0 0-6.08 13.952c0.512 12.288 14.848 22.016 32.128 21.696h732.8a40.768 40.768 0 0 0 17.856-3.648zM259.84 399.68a78.464 78.464 0 0 0 117.504 67.84 78.272 78.272 0 0 0 0-135.744A78.208 78.208 0 0 0 259.84 399.68" p-id="5791"></path><path d="M864.832 872.256H159.232a83.84 83.84 0 0 1-83.776-83.776V235.52a83.84 83.84 0 0 1 83.776-83.776h705.536a83.84 83.84 0 0 1 83.776 83.776v552.96a83.84 83.84 0 0 1-83.712 83.776zM159.232 183.744a51.84 51.84 0 0 0-51.776 51.776v552.96a51.84 51.84 0 0 0 51.776 51.776h705.536a51.84 51.84 0 0 0 51.776-51.776V235.52a51.84 51.84 0 0 0-51.776-51.776H159.232z" p-id="5792"></path></svg>
                 </a>
@@ -359,19 +359,26 @@
             grid: {
                 padding: {
                     top: -20,
                     bottom: -4
                 },
             strokeDashArray: 4,
             },
+            xaxis: {
+                name: "time",
+                tickAmount:6,
+                labels: {
+                    rotate: 0,
+                }
+            },
         };
         return options
     }
 
-    var cpu_chart = new ApexCharts(document.querySelector("#chart-cpu"), options('bar'));
+    var cpu_chart = new ApexCharts(document.querySelector("#chart-cpu"), options('line'));
     cpu_chart.render();
     $('#cpu_loading').click(function () {
         $.ajax({
             url: '/apm/log/compare',
             type: "GET",
             async: true,
             cache: false,
@@ -395,15 +402,15 @@
                     name: '{{ scene2 }}',
                     data: data['scene2']
                 }])
             }
         });
     });
     
-    var battery_chart = new ApexCharts(document.querySelector("#chart-battery"), options('bar'));
+    var battery_chart = new ApexCharts(document.querySelector("#chart-battery"), options('line'));
         battery_chart.render();
         $('#battery_loading').click(function () {
             $.ajax({
                 url: '/apm/log/compare',
                 type: "GET",
                 async: true,
                 cache: false,
@@ -427,15 +434,15 @@
                         name: '{{ scene2 }}',
                         data: data['scene2']
                     }])
                 }
             });
         });
     if(platform == 'iOS'){
-        var gpu_chart = new ApexCharts(document.querySelector("#chart-gpu"), options('bar'));
+        var gpu_chart = new ApexCharts(document.querySelector("#chart-gpu"), options('line'));
         gpu_chart.render();
         $('#gpu_loading').click(function () {
             $.ajax({
                 url: '/apm/log/compare',
                 type: "GET",
                 async: true,
                 cache: false,
@@ -460,15 +467,15 @@
                         data: data['scene2']
                     }])
                 }
             });
         });
     }
 
-    var fps_chart = new ApexCharts(document.querySelector("#chart-fps"), options('bar'));
+    var fps_chart = new ApexCharts(document.querySelector("#chart-fps"), options('line'));
     fps_chart.render();
     $('#fps_loading').click(function () {
         $.ajax({
             url: '/apm/log/compare',
             type: "GET",
             async: true,
             cache: false,
@@ -492,15 +499,15 @@
                     name: '{{ scene2 }}',
                     data: data['scene2']
                 }])
             }
         });
     });
 
-    var mem_chart = new ApexCharts(document.querySelector("#chart-mem"), options('bar'));
+    var mem_chart = new ApexCharts(document.querySelector("#chart-mem"), options('line'));
     mem_chart.render();
     $('#mem_loading').click(function () {
         $.ajax({
             url: '/apm/log/compare',
             type: "GET",
             async: true,
             cache: false,
@@ -524,15 +531,15 @@
                     name: '{{ scene2 }}',
                     data: data['scene2']
                 }])
             }
         });
     });
 
-    var network_recv_chart = new ApexCharts(document.querySelector("#chart-networkdata-recv"), options('bar',false));
+    var network_recv_chart = new ApexCharts(document.querySelector("#chart-networkdata-recv"), options('line',false));
     network_recv_chart.render();
     $('#networkdata_recv_loading').click(function () {
         $.ajax({
             url: '/apm/log/compare',
             type: "GET",
             async: true,
             cache: false,
@@ -556,15 +563,15 @@
                     name: '{{ scene2 }}',
                     data: data['scene2']
                 }])
             }
         });
     });
 
-    var network_send_chart = new ApexCharts(document.querySelector("#chart-networkdata-send"), options('bar',false));
+    var network_send_chart = new ApexCharts(document.querySelector("#chart-networkdata-send"), options('line',false));
     network_send_chart.render();
     $('#networkdata_send_loading').click(function () {
         $.ajax({
             url: '/apm/log/compare',
             type: "GET",
             async: true,
             cache: false,
```

### Comparing `solox-2.6.6/solox/templates/analysis_pk.html` & `solox-2.6.7/solox/templates/analysis_pk.html`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,15 @@
         </div>
         <div class="card-body">
             <div id="chart-cpu"></div>
         </div>
     </div>
     <div class="card mem-card mt-3">
         <div class="card-header">
-            <div class='card-title'>MEM（MB）</div>
+            <div class='card-title'>Memory（MB）</div>
             <div class="card-actions btn-actions">
                 <a class="btn-action cursor-pointer" id="mem_loading">
                     <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
                 </a>
                 <a class="btn-action cursor-pointer" id="mem_png" onclick="screenshot('mem-card','mem.png')">
                     <svg t="1646303797379" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5790" width="2000" height="2000"><path d="M897.856 842.56c14.464-6.72 18.624-20.48 9.28-30.848l-241.216-263.296a25.792 25.792 0 0 0-7.68-5.888c-14.016-7.296-33.6-5.184-43.776 4.8l-241.152 233.088-103.808-70.528a30.912 30.912 0 0 0-3.52-1.92c-14.08-7.36-33.664-4.992-43.776 4.864l-101.056 97.728a18.368 18.368 0 0 0-6.08 13.952c0.512 12.288 14.848 22.016 32.128 21.696h732.8a40.768 40.768 0 0 0 17.856-3.648zM259.84 399.68a78.464 78.464 0 0 0 117.504 67.84 78.272 78.272 0 0 0 0-135.744A78.208 78.208 0 0 0 259.84 399.68" p-id="5791"></path><path d="M864.832 872.256H159.232a83.84 83.84 0 0 1-83.776-83.776V235.52a83.84 83.84 0 0 1 83.776-83.776h705.536a83.84 83.84 0 0 1 83.776 83.776v552.96a83.84 83.84 0 0 1-83.712 83.776zM159.232 183.744a51.84 51.84 0 0 0-51.776 51.776v552.96a51.84 51.84 0 0 0 51.776 51.776h705.536a51.84 51.84 0 0 0 51.776-51.776V235.52a51.84 51.84 0 0 0-51.776-51.776H159.232z" p-id="5792"></path></svg>
                 </a>
```

### Comparing `solox-2.6.6/solox/templates/base.html` & `solox-2.6.7/solox/templates/base.html`

 * *Files 4% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                     <ul class="list-inline list-inline-dots mb-0">
                         <li class="list-inline-item">
                             Copyright &copy; <label id="curYear"></label>
                             <a href="https://github.com/smart-test-ti" class="link-secondary">SoloX</a>.{% if lan == 'cn' %} 保留所有权利 {% else %} All rights reserved {% endif %}
                         </li>
                         <li class="list-inline-item">
                             <a href="https://github.com/smart-test-ti/SoloX/releases" target="_blank" class="link-secondary" rel="noopener">
-                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.6.6
+                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.6.7
                             </a>
                         </li>
                     </ul>
                 </div>
             </div>
         </div>
     </footer>
@@ -147,50 +147,27 @@
         </h2>
         <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
     </div>
     <div class="offcanvas-body">
         <div class="card-tabs">
             <ul class="nav nav-tabs">
                 <!-- https://adbshell.com/commands/adb-connect -->
-                <!-- <li class="nav-item"><a href="#tab-top-1" class="nav-link active" data-bs-toggle="tab">{% if lan == 'cn' %} 无线连接 {% else %} Wireless {% endif %}</a></li> -->
-                <li class="nav-item"><a href="#tab-top-2" class="nav-link" data-bs-toggle="tab">{% if lan == 'cn' %} 告警值 {% else %} Warning Value {% endif %}</a></li>
+                <li class="nav-item active"><a href="#tab-top-2" class="nav-link active" data-bs-toggle="tab">{% if lan == 'cn' %} 告警值 {% else %} Warning Value {% endif %}</a></li>
                 <li class="nav-item"><a href="#tab-top-3" class="nav-link" data-bs-toggle="tab">{% if lan == 'cn' %} 定时器 {% else %} Timer {% endif %}</a></li>
                 <li class="nav-item"><a href="#tab-top-4" class="nav-link" data-bs-toggle="tab">{% if lan == 'cn' %} 远程访问 {% else %} Remote {% endif %} &nbsp;
                     {% if lan == 'en' %}
                     <span class="form-help" data-bs-toggle="popover" data-bs-placement="top" data-bs-html="true" data-bs-content="
                     Start solox on the Slave machine first, and then configure the Host here.</p>Note: The port number cannot be the same as the Master machine</p>">?</span>
                     {% else %}
                     <span class="form-help" data-bs-toggle="popover" data-bs-placement="top" data-bs-html="true" data-bs-content="先在其他机器启动solox,然后将Host配置在这里</p>注意：端口号不能和主机器一样</p> ">?</span>
                     {% endif %}</a>
                 </li>
             </ul>
             <div class="tab-content">
-                <!-- <div id="tab-top-1" class="card tab-pane active show">
-                    <div class="card-body">
-                        <div class="card">
-                            <div class="ribbon bg-green">Device</div>
-                            <div class="card-body">
-                                <h3 class="card-title">BRNUT21B15044184</h3>
-                            </div>
-                            <div class="card-footer">
-                                <div class="row align-items-center">
-                                    <div class="col-auto">
-                                        <input id="port" type="text" class="form-control"  placeholder="Input tcp mode port">
-                                    </div>
-                                    <div class="col-auto ms-auto">
-                                        <label class="form-check form-switch m-0">
-                                            <input class="form-check-input position-static" type="checkbox">
-                                        </label>
-                                    </div>
-                                </div>
-                            </div>
-                        </div>
-                    </div>
-                </div> -->
-              <div id="tab-top-2" class="card tab-pane">
+              <div id="tab-top-2" class="card tab-pane active show">
                 <div class="card-body">
                     <div class="row mb-3">
                         <div class="col-md-6 col-xl-12">
                             <div class="mb-3">
                                 <label class="form-label">{% if lan == 'cn' %} CPU告警值 {% else %} CPU warning value {% endif %}</label>
                                 <input id="cpu_warning_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ cpuWarning }}">
                             </div>
```

#### html2text {}

```diff
@@ -24,17 +24,16 @@
 ***** {% block page_title %} {% endblock %} *****
 {% block ms_auto %}{% endblock %}
 {% block page_body %}{% endblock %}
     * {%_if_lan_==_'cn'_%}_ææ¡£_{%_else_%}_Documentation_{%_endif_%}
     * {%_if_lan_==_'cn'_%}_æºç _{%_else_%}_Source_code_{%_endif_%}
     * Copyright ©  SoloX.{% if lan == 'cn' %} ä¿çæææå© {% else %} All
       rights reserved {% endif %}
-    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.6.6
+    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.6.7
 *****  {% if lan == 'cn' %} è®¾ç½® {% else %} Setting {% endif %} *****
-    *
     * {%_if_lan_==_'cn'_%}_åè­¦å¼_{%_else_%}_Warning_Value_{%_endif_%}
     * {%_if_lan_==_'cn'_%}_å®æ¶å¨_{%_else_%}_Timer_{%_endif_%}
     * {%_if_lan_==_'cn'_%}_è¿ç¨è®¿é®_{%_else_%}_Remote_{%_endif_%}_ _{%_if
       lan_==_'en'_%}_?_{%_else_%}_?_{%_endif_%}
 {% if lan == 'cn' %} CPUåè­¦å¼ {% else %} CPU warning value {% endif %} [{
 { cpuWarning }}    ]
 {% if lan == 'cn' %} åå­åè­¦å¼ {% else %} Memory warning value {% endif
```

### Comparing `solox-2.6.6/solox/templates/index.html` & `solox-2.6.7/solox/templates/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -505,15 +505,15 @@
                             var app_series = cpu_chart.series[0];
                             var sys_series = cpu_chart.series[1];
                             var x = (new Date()).getTime(),
                                 y_app = data['appCpuRate'];
                                 y_sys = data['systemCpuRate'];
                             app_series.addPoint([x, y_app], true, true);
                             sys_series.addPoint([x, y_sys], true, true);
-                            timerQ = setTimeout(getCpuRate(pkgname,device), 1500);
+                            timerQ = setTimeout(getCpuRate(pkgname,device), 1000);
                         }catch (e) {}
                     }else{
                         SwalFire('error','something error',data['msg'],2000);
                     }
                 }
             },
             error: function(error){
@@ -596,15 +596,15 @@
                                 y_voltage = data['voltage'];
                                 y_power = data['power'];
                                 seriesTemperature.addPoint([x, y_temperature], true, true);
                                 seriesCurrent.addPoint([x, y_current], true, true);
                                 seriesVoltage.addPoint([x, y_voltage], true, true);
                                 seriesPower.addPoint([x, y_power], true, true);
                             } 
-                            timerQ = setTimeout(getBattery(device), 10000);
+                            timerQ = setTimeout(getBattery(device), 1000);
                         }catch (e) {}
                     }else{
                         SwalFire('error','something error',data['msg'],2000);
                     }
                 }
             },
             error: function(error){
@@ -652,15 +652,15 @@
                                 seriesDalvik.addPoint([x, y_dalvik], true, true);
                             }else{
                                 var series = mem_chart.series[0];
                                 var x = (new Date()).getTime(),
                                     y = data['totalPass'];
                                 series.addPoint([x, y], true, true);
                             }
-                            timerQ = setTimeout(getMemPss(pkgname,device), 1500);
+                            timerQ = setTimeout(getMemPss(pkgname,device), 1000);
 
                         }catch (e) {}
                     }else{
                         SwalFire('error','something error',data['msg'],2000);
                     }
                 }
             },
@@ -730,15 +730,15 @@
                             var seriesDownFlow = network_chart.series[1];
                             var x_up = (new Date()).getTime(),
                                 y_up = data['upflow'];
                             var x_down = (new Date()).getTime(),
                                 y_down = data['downflow'];
                             seriesUpFlow.addPoint([x_up, y_up], true, true);
                             seriesDownFlow.addPoint([x_down, y_down], true, true);
-                            timerQ = setTimeout(getNetWork(pkgname,device,net_switch), 1500);
+                            timerQ = setTimeout(getNetWork(pkgname,device,net_switch), 1000);
                         }catch (e) {
                             console.log(e)
                         }
                     }else{
                         SwalFire('error','something error',data['msg'],2000);
                     }
                 }
@@ -777,15 +777,15 @@
                             seriesFps.addPoint([x_fps, y_fps], true, true);
                             if(platform == 'Android'){
                                 let seriesJank = fps_chart.series[1];
                                 let x_jsnk = (new Date()).getTime(),
                                     y_jank = data['jank'];
                                 seriesJank.addPoint([x_jsnk, y_jank], true, true);
                             }
-                            timerQ = setTimeout(getFps(pkgname,device,fps_switch), 1500);
+                            timerQ = setTimeout(getFps(pkgname,device,fps_switch), 1000);
                         }catch (e) {}
                     }else{
                         SwalFire('error','something error',data['msg'],2000);
                     }
                 }
             },
             error: function(error){
```

### Comparing `solox-2.6.6/solox/templates/pk.html` & `solox-2.6.7/solox/templates/pk.html`

 * *Files 0% similar despite different names*

```diff
@@ -546,15 +546,15 @@
         //初始化cpu
         let cpu_chart = chartsInitialize('cpu','CPU（%）');
         return cpu_chart
     }
 
     function memInitialize(){
         //初始化mem
-        let mem_chart = chartsInitialize('mem','MEM（MB）');
+        let mem_chart = chartsInitialize('mem','Memory（MB）');
         return mem_chart
     }
 
     function networkInitialize(){
         //初始化network
         let network_chart = chartsInitialize('network','Network Data（KB)');
         return network_chart
@@ -645,15 +645,15 @@
     function collectCpu(device,pkgname){
         cpuInitialize();
         cpu_chart = collectPers(device,pkgname,'cpu','CPU（%）',getCpuRate(pkgname,device));
     }
 
     function collectMem(device,pkgname){
         memInitialize();
-        mem_chart = collectPers(device,pkgname,'mem','MEM（MB）',getMemPss(pkgname,device));
+        mem_chart = collectPers(device,pkgname,'mem','Memory（MB）',getMemPss(pkgname,device));
     }
 
     function collectNetwork(device,pkgname){
         networkInitialize();
         network_chart = collectPers(device,pkgname,'network','Network Data（KB）',getNetWork(pkgname,device));
     }
```

### Comparing `solox-2.6.6/solox/templates/report.html` & `solox-2.6.7/solox/templates/report.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/view/apis.py` & `solox-2.6.7/solox/view/apis.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/view/pages.py` & `solox-2.6.7/solox/view/pages.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.6/solox/web.py` & `solox-2.6.7/solox/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import traceback
 from solox.view.apis import api
 from solox.view.pages import page
 from logzero import logger
 from threading import Lock
 from flask_socketio import SocketIO, disconnect
 from flask import Flask
+from pyfiglet import Figlet
 
 app = Flask(__name__, template_folder='templates', static_folder='static')
 app.register_blueprint(api)
 app.register_blueprint(page)
 
 socketio = SocketIO(app, cors_allowed_origins="*")
 thread = True
@@ -104,14 +105,16 @@
     return flag
 
 
 def openUrl(host: str, port: int):
     flag = True
     while flag:
         logger.info('Start solox server ...')
+        f = Figlet(font="slant", width=300)
+        print(f.renderText("SOLOX 2. 6. 7"))
         flag = getServerStatus(host, port)
     webbrowser.open('http://{}:{}/?platform=Android&lan=en'.format(host, port), new=2)
     logger.info('Running on http://{}:{}/?platform=Android&lan=en (Press CTRL+C to quit)'.format(host, port))
 
 
 def startServer(host: str, port: int):
     socketio.run(app, host=host, debug=False, port=port)
```

### Comparing `solox-2.6.6/solox.egg-info/PKG-INFO` & `solox-2.6.7/solox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solox
-Version: 2.6.6
+Version: 2.6.7
 Summary: SoloX - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/smart-test-ti/SoloX
 Author: Rafa Chen
 Author-email: rafacheninc@gamil.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,15 +33,15 @@
 
 ## 🔎Preview
 
 SoloX - Real-time collection tool for Android/iOS performance data.
 
 We are committed to solving inefficient, cumbersome test execution, and our goal is Simple Test In SoloX!
 
-![preview](https://github.com/smart-test-ti/SoloX/assets/24454096/6941452f-6410-4730-a532-0d69d0f7fdb8)
+![preview](https://github.com/smart-test-ti/SoloX/assets/24454096/4d9d9dab-9e24-4327-a60a-84f14b79206d)
 
 ## 📦Requirements
 
 - Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
 - Install adb and configure environment variables (SoloX's  adb may not necessarily fit your computer) [**Download**](https://developer.android.com/studio/releases/platform-tools)
 
 💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4.
```

### Comparing `solox-2.6.6/solox.egg-info/SOURCES.txt` & `solox-2.6.7/solox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

