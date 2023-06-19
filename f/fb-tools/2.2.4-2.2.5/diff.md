# Comparing `tmp/fb_tools-2.2.4.tar.gz` & `tmp/fb_tools-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb_tools-2.2.4.tar", last modified: Tue Jun 13 10:26:17 2023, max compression
+gzip compressed data, was "fb_tools-2.2.5.tar", last modified: Mon Jun 19 09:34:44 2023, max compression
```

## Comparing `fb_tools-2.2.4.tar` & `fb_tools-2.2.5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/
--rw-r--r--   0 root         (0) root         (0)     7652 2023-06-13 10:25:53.000000 fb_tools-2.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      120 2023-06-13 10:25:53.000000 fb_tools-2.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1729 2023-06-13 10:26:17.410981 fb_tools-2.2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      503 2023-06-13 10:25:53.000000 fb_tools-2.2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.406981 fb_tools-2.2.4/bin/
--rwxr-xr-x   0 root         (0) root         (0)     2463 2023-06-13 10:25:53.000000 fb_tools-2.2.4/bin/get-file-to-remove
--rwxr-xr-x   0 root         (0) root         (0)     1574 2023-06-13 10:25:53.000000 fb_tools-2.2.4/bin/myip
--rwxr-xr-x   0 root         (0) root         (0)     1588 2023-06-13 10:25:53.000000 fb_tools-2.2.4/bin/update-ddns
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.406981 fb_tools-2.2.4/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.406981 fb_tools-2.2.4/lib/fb_tools/
--rw-r--r--   0 root         (0) root         (0)      406 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28444 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/app.py
--rw-r--r--   0 root         (0) root         (0)     8423 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/argparse_actions.py
--rw-r--r--   0 root         (0) root         (0)     9654 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/cfg_app.py
--rw-r--r--   0 root         (0) root         (0)    36990 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/collections.py
--rw-r--r--   0 root         (0) root         (0)    24990 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/common.py
--rw-r--r--   0 root         (0) root         (0)     8163 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/lib/fb_tools/ddns/
--rw-r--r--   0 root         (0) root         (0)    18917 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/ddns/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10614 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/ddns/config.py
--rw-r--r--   0 root         (0) root         (0)     5590 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/ddns/myip_app.py
--rw-r--r--   0 root         (0) root         (0)    14002 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/ddns/update_app.py
--rw-r--r--   0 root         (0) root         (0)    12591 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/errors.py
--rw-r--r--   0 root         (0) root         (0)    24522 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/get_file_rm_app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/lib/fb_tools/handler/
--rw-r--r--   0 root         (0) root         (0)    14092 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43539 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/handler/lock.py
--rw-r--r--   0 root         (0) root         (0)    39509 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/handling_obj.py
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-13 10:26:17.000000 fb_tools-2.2.4/lib/fb_tools/local_version.py
--rw-r--r--   0 root         (0) root         (0)    34973 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/mailaddress.py
--rw-r--r--   0 root         (0) root         (0)     2391 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/merge.py
--rw-r--r--   0 root         (0) root         (0)    43962 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/multi_config.py
--rw-r--r--   0 root         (0) root         (0)    11761 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/obj.py
--rw-r--r--   0 root         (0) root         (0)    17133 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/pidfile.py
--rw-r--r--   0 root         (0) root         (0)     2953 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/xlate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/lib/fb_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1729 2023-06-13 10:26:17.000000 fb_tools-2.2.4/lib/fb_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1378 2023-06-13 10:26:17.000000 fb_tools-2.2.4/lib/fb_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 10:26:17.000000 fb_tools-2.2.4/lib/fb_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-13 10:26:17.000000 fb_tools-2.2.4/lib/fb_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-13 10:26:17.000000 fb_tools-2.2.4/lib/fb_tools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.406981 fb_tools-2.2.4/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/locale/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    41697 2023-06-13 10:26:17.000000 fb_tools-2.2.4/locale/de/LC_MESSAGES/fb_tools.mo
--rw-r--r--   0 root         (0) root         (0)    60345 2023-06-13 10:25:53.000000 fb_tools-2.2.4/locale/de/LC_MESSAGES/fb_tools.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.406981 fb_tools-2.2.4/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/locale/en/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     5422 2023-06-13 10:26:17.000000 fb_tools-2.2.4/locale/en/LC_MESSAGES/fb_tools.mo
--rw-r--r--   0 root         (0) root         (0)    43159 2023-06-13 10:25:53.000000 fb_tools-2.2.4/locale/en/LC_MESSAGES/fb_tools.po
--rw-r--r--   0 root         (0) root         (0)    41282 2023-06-13 10:25:53.000000 fb_tools-2.2.4/locale/fb_tools.pot
--rw-r--r--   0 root         (0) root         (0)     1795 2023-06-13 10:26:17.414981 fb_tools-2.2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8889 2023-06-13 10:25:53.000000 fb_tools-2.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/test/
--rwxr-xr-x   0 root         (0) root         (0)      270 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/call_script.sh
--rwxr-xr-x   0 root         (0) root         (0)      438 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/call_sleep.sh
--rwxr-xr-x   0 root         (0) root         (0)      438 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/do_sleep
--rw-r--r--   0 root         (0) root         (0)     3257 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/general.py
--rwxr-xr-x   0 root         (0) root         (0)     4459 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_00_errors.py
--rwxr-xr-x   0 root         (0) root         (0)    24389 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_05_common.py
--rwxr-xr-x   0 root         (0) root         (0)     6432 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_10_base_object.py
--rwxr-xr-x   0 root         (0) root         (0)    59500 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_13_collections.py
--rwxr-xr-x   0 root         (0) root         (0)    52741 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_15_mailaddress.py
--rwxr-xr-x   0 root         (0) root         (0)    17995 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_17_multicfg.py
--rwxr-xr-x   0 root         (0) root         (0)     5817 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_18_pidfile.py
--rwxr-xr-x   0 root         (0) root         (0)    19877 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_20_handling_object.py
--rwxr-xr-x   0 root         (0) root         (0)     7626 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_30_base_handler.py
--rwxr-xr-x   0 root         (0) root         (0)    14476 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_33_lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:34:44.709758 fb_tools-2.2.5/
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-06-19 09:34:22.000000 fb_tools-2.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      120 2023-06-19 09:34:22.000000 fb_tools-2.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-06-19 09:34:44.713758 fb_tools-2.2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      503 2023-06-19 09:34:22.000000 fb_tools-2.2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:34:44.701758 fb_tools-2.2.5/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     2463 2023-06-19 09:34:22.000000 fb_tools-2.2.5/bin/get-file-to-remove
+-rwxr-xr-x   0 root         (0) root         (0)     1574 2023-06-19 09:34:22.000000 fb_tools-2.2.5/bin/myip
+-rwxr-xr-x   0 root         (0) root         (0)     1588 2023-06-19 09:34:22.000000 fb_tools-2.2.5/bin/update-ddns
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:34:44.701758 fb_tools-2.2.5/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:34:44.705758 fb_tools-2.2.5/lib/fb_tools/
+-rw-r--r--   0 root         (0) root         (0)      406 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28542 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/app.py
+-rw-r--r--   0 root         (0) root         (0)     8423 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/argparse_actions.py
+-rw-r--r--   0 root         (0) root         (0)     9654 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/cfg_app.py
+-rw-r--r--   0 root         (0) root         (0)    36990 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/collections.py
+-rw-r--r--   0 root         (0) root         (0)    24990 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/common.py
+-rw-r--r--   0 root         (0) root         (0)     8163 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:34:44.709758 fb_tools-2.2.5/lib/fb_tools/ddns/
+-rw-r--r--   0 root         (0) root         (0)    18917 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/ddns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10614 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/ddns/config.py
+-rw-r--r--   0 root         (0) root         (0)     5590 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/ddns/myip_app.py
+-rw-r--r--   0 root         (0) root         (0)    14002 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/ddns/update_app.py
+-rw-r--r--   0 root         (0) root         (0)    12591 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/errors.py
+-rw-r--r--   0 root         (0) root         (0)    24522 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/get_file_rm_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:34:44.709758 fb_tools-2.2.5/lib/fb_tools/handler/
+-rw-r--r--   0 root         (0) root         (0)    14092 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43539 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/handler/lock.py
+-rw-r--r--   0 root         (0) root         (0)    39509 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/handling_obj.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-19 09:34:44.000000 fb_tools-2.2.5/lib/fb_tools/local_version.py
+-rw-r--r--   0 root         (0) root         (0)    34973 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/mailaddress.py
+-rw-r--r--   0 root         (0) root         (0)     2391 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/merge.py
+-rw-r--r--   0 root         (0) root         (0)    43962 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/multi_config.py
+-rw-r--r--   0 root         (0) root         (0)    11761 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/obj.py
+-rw-r--r--   0 root         (0) root         (0)    17133 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/pidfile.py
+-rw-r--r--   0 root         (0) root         (0)     3390 2023-06-19 09:34:22.000000 fb_tools-2.2.5/lib/fb_tools/xlate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:34:44.705758 fb_tools-2.2.5/lib/fb_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-06-19 09:34:44.000000 fb_tools-2.2.5/lib/fb_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-06-19 09:34:44.000000 fb_tools-2.2.5/lib/fb_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 09:34:44.000000 fb_tools-2.2.5/lib/fb_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-19 09:34:44.000000 fb_tools-2.2.5/lib/fb_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-19 09:34:44.000000 fb_tools-2.2.5/lib/fb_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:34:44.709758 fb_tools-2.2.5/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:34:44.701758 fb_tools-2.2.5/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:34:44.709758 fb_tools-2.2.5/locale/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    41697 2023-06-19 09:34:44.000000 fb_tools-2.2.5/locale/de/LC_MESSAGES/fb_tools.mo
+-rw-r--r--   0 root         (0) root         (0)    60345 2023-06-19 09:34:22.000000 fb_tools-2.2.5/locale/de/LC_MESSAGES/fb_tools.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:34:44.701758 fb_tools-2.2.5/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:34:44.709758 fb_tools-2.2.5/locale/en/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     5422 2023-06-19 09:34:44.000000 fb_tools-2.2.5/locale/en/LC_MESSAGES/fb_tools.mo
+-rw-r--r--   0 root         (0) root         (0)    43159 2023-06-19 09:34:22.000000 fb_tools-2.2.5/locale/en/LC_MESSAGES/fb_tools.po
+-rw-r--r--   0 root         (0) root         (0)    41282 2023-06-19 09:34:22.000000 fb_tools-2.2.5/locale/fb_tools.pot
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-06-19 09:34:44.713758 fb_tools-2.2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8889 2023-06-19 09:34:22.000000 fb_tools-2.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:34:44.709758 fb_tools-2.2.5/test/
+-rwxr-xr-x   0 root         (0) root         (0)      270 2023-06-19 09:34:22.000000 fb_tools-2.2.5/test/call_script.sh
+-rwxr-xr-x   0 root         (0) root         (0)      438 2023-06-19 09:34:22.000000 fb_tools-2.2.5/test/call_sleep.sh
+-rwxr-xr-x   0 root         (0) root         (0)      438 2023-06-19 09:34:22.000000 fb_tools-2.2.5/test/do_sleep
+-rw-r--r--   0 root         (0) root         (0)     3257 2023-06-19 09:34:22.000000 fb_tools-2.2.5/test/general.py
+-rwxr-xr-x   0 root         (0) root         (0)     4459 2023-06-19 09:34:22.000000 fb_tools-2.2.5/test/test_00_errors.py
+-rwxr-xr-x   0 root         (0) root         (0)    24389 2023-06-19 09:34:22.000000 fb_tools-2.2.5/test/test_05_common.py
+-rwxr-xr-x   0 root         (0) root         (0)     6432 2023-06-19 09:34:22.000000 fb_tools-2.2.5/test/test_10_base_object.py
+-rwxr-xr-x   0 root         (0) root         (0)    59500 2023-06-19 09:34:22.000000 fb_tools-2.2.5/test/test_13_collections.py
+-rwxr-xr-x   0 root         (0) root         (0)    52741 2023-06-19 09:34:22.000000 fb_tools-2.2.5/test/test_15_mailaddress.py
+-rwxr-xr-x   0 root         (0) root         (0)    17995 2023-06-19 09:34:22.000000 fb_tools-2.2.5/test/test_17_multicfg.py
+-rwxr-xr-x   0 root         (0) root         (0)     5817 2023-06-19 09:34:22.000000 fb_tools-2.2.5/test/test_18_pidfile.py
+-rwxr-xr-x   0 root         (0) root         (0)    19877 2023-06-19 09:34:22.000000 fb_tools-2.2.5/test/test_20_handling_object.py
+-rwxr-xr-x   0 root         (0) root         (0)     7626 2023-06-19 09:34:22.000000 fb_tools-2.2.5/test/test_30_base_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)    14476 2023-06-19 09:34:22.000000 fb_tools-2.2.5/test/test_33_lock.py
```

### Comparing `fb_tools-2.2.4/LICENSE` & `fb_tools-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/PKG-INFO` & `fb_tools-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb_tools
-Version: 2.2.4
+Version: 2.2.5
 Summary: Modules for common used objects, error classes and methods.
 Home-page: https://github.com/fbrehm/python_fb_tools
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fb_tools-2.2.4/bin/get-file-to-remove` & `fb_tools-2.2.5/bin/get-file-to-remove`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/bin/myip` & `fb_tools-2.2.5/bin/myip`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/bin/update-ddns` & `fb_tools-2.2.5/bin/update-ddns`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/app.py` & `fb_tools-2.2.5/lib/fb_tools/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,19 @@
 from .argparse_actions import TimeoutOptionAction
 from .common import terminal_can_colors
 from .errors import FbAppError
 from .errors import FunctionNotImplementedError
 from .handling_obj import HandlingObject
 from .xlate import DOMAIN, LOCALE_DIR, XLATOR
 from .xlate import __base_dir__ as __xlate_base_dir__
+from .xlate import __lib_dir__ as __xlate_lib_dir__
 from .xlate import __mo_file__ as __xlate_mo_file__
 from .xlate import __module_dir__ as __xlate_module_dir__
 
-__version__ = '2.2.3'
+__version__ = '2.2.4'
 LOG = logging.getLogger(__name__)
 
 SIGNAL_NAMES = {
     signal.SIGHUP: 'HUP',
     signal.SIGINT: 'INT',
     signal.SIGABRT: 'ABRT',
     signal.SIGTERM: 'TERM',
@@ -321,14 +322,15 @@
         res['show_quiet_option'] = self.show_quiet_option
         res['show_simulate_option'] = self.show_simulate_option
         res['usage'] = self.usage
         if 'xlate' not in res:
             res['xlate'] = {}
         res['xlate']['fb_tools'] = {
             '__module_dir__': __xlate_module_dir__,
+            '__lib_dir__': __xlate_lib_dir__,
             '__base_dir__': __xlate_base_dir__,
             'LOCALE_DIR': LOCALE_DIR,
             'DOMAIN': DOMAIN,
             '__mo_file__': __xlate_mo_file__,
         }
 
         return res
```

### Comparing `fb_tools-2.2.4/lib/fb_tools/argparse_actions.py` & `fb_tools-2.2.5/lib/fb_tools/argparse_actions.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/cfg_app.py` & `fb_tools-2.2.5/lib/fb_tools/cfg_app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/collections.py` & `fb_tools-2.2.5/lib/fb_tools/collections.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/common.py` & `fb_tools-2.2.5/lib/fb_tools/common.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/config.py` & `fb_tools-2.2.5/lib/fb_tools/config.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/ddns/__init__.py` & `fb_tools-2.2.5/lib/fb_tools/ddns/__init__.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/ddns/config.py` & `fb_tools-2.2.5/lib/fb_tools/ddns/config.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/ddns/myip_app.py` & `fb_tools-2.2.5/lib/fb_tools/ddns/myip_app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/ddns/update_app.py` & `fb_tools-2.2.5/lib/fb_tools/ddns/update_app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/errors.py` & `fb_tools-2.2.5/lib/fb_tools/errors.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/get_file_rm_app.py` & `fb_tools-2.2.5/lib/fb_tools/get_file_rm_app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/handler/__init__.py` & `fb_tools-2.2.5/lib/fb_tools/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/handler/lock.py` & `fb_tools-2.2.5/lib/fb_tools/handler/lock.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/handling_obj.py` & `fb_tools-2.2.5/lib/fb_tools/handling_obj.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/mailaddress.py` & `fb_tools-2.2.5/lib/fb_tools/mailaddress.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/merge.py` & `fb_tools-2.2.5/lib/fb_tools/merge.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/multi_config.py` & `fb_tools-2.2.5/lib/fb_tools/multi_config.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/obj.py` & `fb_tools-2.2.5/lib/fb_tools/obj.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/pidfile.py` & `fb_tools-2.2.5/lib/fb_tools/pidfile.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/lib/fb_tools/xlate.py` & `fb_tools-2.2.5/lib/fb_tools/xlate.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,29 +31,40 @@
 except ImportError:
     from distutils.version import LooseVersion as Version
 
 DOMAIN = 'fb_tools'
 
 LOG = logging.getLogger(__name__)
 
-__version__ = '2.0.3'
+__version__ = '2.0.4'
 
 __me__ = Path(__file__).resolve()
 __module_dir__ = __me__.parent
 __lib_dir__ = __module_dir__.parent
 __base_dir__ = __lib_dir__.parent
-LOCALE_DIR = __base_dir__.joinpath('locale')
+LOCALE_DIR = __base_dir__ / 'locale'
 if LOCALE_DIR.is_dir():
+    # Not installed, in development workdir
     LOCALE_DIR = str(LOCALE_DIR)
 else:
-    LOCALE_DIR = __module_dir__.joinpath('locale')
-    if LOCALE_DIR.is_dir():
-        LOCALE_DIR = str(LOCALE_DIR)
-    else:
+    # Somehow installed
+    if sys.prefix == sys.base_prefix:
+        # installed as a package
         LOCALE_DIR = sys.prefix + '/share/locale'
+    else:
+        # Obviously in a virtual environment
+        LOCALE_DIR = __lib_dir__ / 'usr' / 'local' / 'share' / 'locale'
+        if LOCALE_DIR.is_dir():
+            LOCALE_DIR = str(LOCALE_DIR.resolve())
+        else:
+            LOCALE_DIR = __module_dir__ / 'locale'
+            if LOCALE_DIR.is_dir():
+                LOCALE_DIR = str(LOCALE_DIR)
+            else:
+                LOCALE_DIR = sys.prefix + '/share/locale'
 
 DEFAULT_LOCALE_DEF = 'en_US'
 DEFAULT_LOCALE = babel.core.default_locale()
 if not DEFAULT_LOCALE:
     DEFAULT_LOCALE = DEFAULT_LOCALE_DEF
 
 __mo_file__ = gettext.find(DOMAIN, LOCALE_DIR)
```

### Comparing `fb_tools-2.2.4/lib/fb_tools.egg-info/PKG-INFO` & `fb_tools-2.2.5/lib/fb_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb-tools
-Version: 2.2.4
+Version: 2.2.5
 Summary: Modules for common used objects, error classes and methods.
 Home-page: https://github.com/fbrehm/python_fb_tools
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fb_tools-2.2.4/lib/fb_tools.egg-info/SOURCES.txt` & `fb_tools-2.2.5/lib/fb_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/locale/de/LC_MESSAGES/fb_tools.mo` & `fb_tools-2.2.5/locale/de/LC_MESSAGES/fb_tools.mo`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/locale/de/LC_MESSAGES/fb_tools.po` & `fb_tools-2.2.5/locale/de/LC_MESSAGES/fb_tools.po`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/locale/en/LC_MESSAGES/fb_tools.mo` & `fb_tools-2.2.5/locale/en/LC_MESSAGES/fb_tools.mo`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/locale/en/LC_MESSAGES/fb_tools.po` & `fb_tools-2.2.5/locale/en/LC_MESSAGES/fb_tools.po`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/locale/fb_tools.pot` & `fb_tools-2.2.5/locale/fb_tools.pot`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/setup.cfg` & `fb_tools-2.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/setup.py` & `fb_tools-2.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/test/general.py` & `fb_tools-2.2.5/test/general.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/test/test_00_errors.py` & `fb_tools-2.2.5/test/test_00_errors.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/test/test_05_common.py` & `fb_tools-2.2.5/test/test_05_common.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/test/test_10_base_object.py` & `fb_tools-2.2.5/test/test_10_base_object.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/test/test_13_collections.py` & `fb_tools-2.2.5/test/test_13_collections.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/test/test_15_mailaddress.py` & `fb_tools-2.2.5/test/test_15_mailaddress.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/test/test_17_multicfg.py` & `fb_tools-2.2.5/test/test_17_multicfg.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/test/test_18_pidfile.py` & `fb_tools-2.2.5/test/test_18_pidfile.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/test/test_20_handling_object.py` & `fb_tools-2.2.5/test/test_20_handling_object.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/test/test_30_base_handler.py` & `fb_tools-2.2.5/test/test_30_base_handler.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.4/test/test_33_lock.py` & `fb_tools-2.2.5/test/test_33_lock.py`

 * *Files identical despite different names*

