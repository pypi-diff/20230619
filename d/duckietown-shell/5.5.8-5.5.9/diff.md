# Comparing `tmp/duckietown-shell-5.5.8.tar.gz` & `tmp/duckietown-shell-5.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckietown-shell-5.5.8.tar", last modified: Wed Apr 26 13:48:59 2023, max compression
+gzip compressed data, was "duckietown-shell-5.5.9.tar", last modified: Mon Jun 19 20:11:23 2023, max compression
```

## Comparing `duckietown-shell-5.5.8.tar` & `duckietown-shell-5.5.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-26 13:48:59.379018 duckietown-shell-5.5.8/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    75933 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/LICENSE.pdf
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2023-04-26 13:48:59.379018 duckietown-shell-5.5.8/PKG-INFO
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-26 13:48:59.375018 duckietown-shell-5.5.8/lib/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-26 13:48:59.379018 duckietown-shell-5.5.8/lib/dt_shell/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1128 2023-04-26 13:48:57.000000 duckietown-shell-5.5.8/lib/dt_shell/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    13053 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/cli.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1306 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/cli_options.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1680 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/col_logging.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2307 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/commands_.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4291 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/config.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      895 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/constants.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2984 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/dt_command_abs.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      201 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/dt_command_placeholder.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3835 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/duckietown_tokens.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4741 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/env_checks.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      683 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      664 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/logging.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5530 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/main.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2467 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/package_version_check.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1994 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/tokens_cli.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4610 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/update_utils.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3239 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/utils.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4528 2023-04-19 20:12:13.000000 duckietown-shell-5.5.8/lib/dt_shell/version_check.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-26 13:48:59.379018 duckietown-shell-5.5.8/lib/duckietown_shell.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2023-04-26 13:48:59.000000 duckietown-shell-5.5.8/lib/duckietown_shell.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      854 2023-04-26 13:48:59.000000 duckietown-shell-5.5.8/lib/duckietown_shell.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-26 13:48:59.000000 duckietown-shell-5.5.8/lib/duckietown_shell.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       43 2023-04-26 13:48:59.000000 duckietown-shell-5.5.8/lib/duckietown_shell.egg-info/entry_points.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-20 04:24:53.000000 duckietown-shell-5.5.8/lib/duckietown_shell.egg-info/not-zip-safe
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      266 2023-04-26 13:48:59.000000 duckietown-shell-5.5.8/lib/duckietown_shell.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        9 2023-04-26 13:48:59.000000 duckietown-shell-5.5.8/lib/duckietown_shell.egg-info/top_level.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-04-26 13:48:59.379018 duckietown-shell-5.5.8/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2015 2023-04-26 13:48:46.000000 duckietown-shell-5.5.8/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-19 20:11:23.537938 duckietown-shell-5.5.9/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    75933 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/LICENSE.pdf
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2023-06-19 20:11:23.537938 duckietown-shell-5.5.9/PKG-INFO
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-19 20:11:23.533939 duckietown-shell-5.5.9/lib/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-19 20:11:23.537938 duckietown-shell-5.5.9/lib/dt_shell/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1128 2023-06-19 20:11:21.000000 duckietown-shell-5.5.9/lib/dt_shell/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    13053 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/cli.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1306 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/cli_options.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1680 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/col_logging.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2307 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/commands_.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4291 2023-06-19 20:08:35.000000 duckietown-shell-5.5.9/lib/dt_shell/config.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      895 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/constants.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2984 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/dt_command_abs.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      201 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/dt_command_placeholder.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3835 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/duckietown_tokens.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4741 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/env_checks.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      683 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      664 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/logging.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5530 2023-06-19 20:02:44.000000 duckietown-shell-5.5.9/lib/dt_shell/main.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2467 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/package_version_check.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1994 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/tokens_cli.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4610 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/update_utils.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3239 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/utils.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4528 2023-03-22 21:05:31.000000 duckietown-shell-5.5.9/lib/dt_shell/version_check.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-19 20:11:23.537938 duckietown-shell-5.5.9/lib/duckietown_shell.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2023-06-19 20:11:23.000000 duckietown-shell-5.5.9/lib/duckietown_shell.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      854 2023-06-19 20:11:23.000000 duckietown-shell-5.5.9/lib/duckietown_shell.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-06-19 20:11:23.000000 duckietown-shell-5.5.9/lib/duckietown_shell.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       43 2023-06-19 20:11:23.000000 duckietown-shell-5.5.9/lib/duckietown_shell.egg-info/entry_points.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-06-19 20:03:58.000000 duckietown-shell-5.5.9/lib/duckietown_shell.egg-info/not-zip-safe
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      266 2023-06-19 20:11:23.000000 duckietown-shell-5.5.9/lib/duckietown_shell.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        9 2023-06-19 20:11:23.000000 duckietown-shell-5.5.9/lib/duckietown_shell.egg-info/top_level.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-06-19 20:11:23.537938 duckietown-shell-5.5.9/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2015 2023-06-19 20:10:15.000000 duckietown-shell-5.5.9/setup.py
```

### Comparing `duckietown-shell-5.5.8/LICENSE.pdf` & `duckietown-shell-5.5.9/LICENSE.pdf`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/__init__.py` & `duckietown-shell-5.5.9/lib/dt_shell/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Optional
 
 logging.basicConfig()
 
 dtslogger = logging.getLogger("dts")
 dtslogger.setLevel(logging.INFO)
 
-__version__ = "5.5.8"
+__version__ = "5.5.9"
 
 
 dtslogger.debug(f"duckietown-shell {__version__}")
 
 import sys
 
 if sys.version_info < (3, 6):
```

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/cli.py` & `duckietown-shell-5.5.9/lib/dt_shell/cli.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/cli_options.py` & `duckietown-shell-5.5.9/lib/dt_shell/cli_options.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/col_logging.py` & `duckietown-shell-5.5.9/lib/dt_shell/col_logging.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/commands_.py` & `duckietown-shell-5.5.9/lib/dt_shell/commands_.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/config.py` & `duckietown-shell-5.5.9/lib/dt_shell/config.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/constants.py` & `duckietown-shell-5.5.9/lib/dt_shell/constants.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/dt_command_abs.py` & `duckietown-shell-5.5.9/lib/dt_shell/dt_command_abs.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/duckietown_tokens.py` & `duckietown-shell-5.5.9/lib/dt_shell/duckietown_tokens.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/env_checks.py` & `duckietown-shell-5.5.9/lib/dt_shell/env_checks.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/exceptions.py` & `duckietown-shell-5.5.9/lib/dt_shell/exceptions.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/logging.py` & `duckietown-shell-5.5.9/lib/dt_shell/logging.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/main.py` & `duckietown-shell-5.5.9/lib/dt_shell/main.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/package_version_check.py` & `duckietown-shell-5.5.9/lib/dt_shell/package_version_check.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/tokens_cli.py` & `duckietown-shell-5.5.9/lib/dt_shell/tokens_cli.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/update_utils.py` & `duckietown-shell-5.5.9/lib/dt_shell/update_utils.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/utils.py` & `duckietown-shell-5.5.9/lib/dt_shell/utils.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/dt_shell/version_check.py` & `duckietown-shell-5.5.9/lib/dt_shell/version_check.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/lib/duckietown_shell.egg-info/SOURCES.txt` & `duckietown-shell-5.5.9/lib/duckietown_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.8/setup.py` & `duckietown-shell-5.5.9/setup.py`

 * *Files identical despite different names*

