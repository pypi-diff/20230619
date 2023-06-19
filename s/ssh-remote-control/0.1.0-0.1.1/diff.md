# Comparing `tmp/ssh_remote_control-0.1.0.tar.gz` & `tmp/ssh_remote_control-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_remote_control-0.1.0.tar", last modified: Mon Jun 19 10:23:10 2023, max compression
+gzip compressed data, was "ssh_remote_control-0.1.1.tar", last modified: Mon Jun 19 13:11:15 2023, max compression
```

## Comparing `ssh_remote_control-0.1.0.tar` & `ssh_remote_control-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 10:23:10.842988 ssh_remote_control-0.1.0/
--rw-rw-rw-   0        0        0     1084 2023-06-19 04:51:08.000000 ssh_remote_control-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1428 2023-06-19 10:23:10.841986 ssh_remote_control-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      832 2023-06-19 10:07:10.000000 ssh_remote_control-0.1.0/README.md
--rw-rw-rw-   0        0        0      848 2023-06-19 09:17:43.000000 ssh_remote_control-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 10:23:10.842988 ssh_remote_control-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-19 10:23:10.757984 ssh_remote_control-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 10:23:10.787985 ssh_remote_control-0.1.0/src/ssh_remote_control/
--rw-rw-rw-   0        0        0    10774 2023-06-19 09:31:24.000000 ssh_remote_control-0.1.0/src/ssh_remote_control/__init__.py
--rw-rw-rw-   0        0        0     6656 2023-06-19 04:57:57.000000 ssh_remote_control-0.1.0/src/ssh_remote_control/command.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:23:10.838985 ssh_remote_control-0.1.0/src/ssh_remote_control/default_commands/
--rw-rw-rw-   0        0        0      111 2023-06-19 03:25:53.000000 ssh_remote_control-0.1.0/src/ssh_remote_control/default_commands/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-06-19 01:38:24.000000 ssh_remote_control-0.1.0/src/ssh_remote_control/default_commands/const.py
--rw-rw-rw-   0        0        0     3757 2023-06-19 10:12:42.000000 ssh_remote_control-0.1.0/src/ssh_remote_control/default_commands/linux.py
--rw-rw-rw-   0        0        0     3304 2023-06-19 10:13:12.000000 ssh_remote_control-0.1.0/src/ssh_remote_control/default_commands/windows_cmd.py
--rw-rw-rw-   0        0        0     3538 2023-06-19 10:14:03.000000 ssh_remote_control-0.1.0/src/ssh_remote_control/default_commands/windows_ps.py
--rw-rw-rw-   0        0        0      550 2023-06-19 03:37:58.000000 ssh_remote_control-0.1.0/src/ssh_remote_control/event.py
--rw-rw-rw-   0        0        0      159 2023-06-19 09:54:09.000000 ssh_remote_control-0.1.0/src/ssh_remote_control/helpers.py
--rw-rw-rw-   0        0        0     1313 2023-06-19 04:04:40.000000 ssh_remote_control-0.1.0/src/ssh_remote_control/locker.py
--rw-rw-rw-   0        0        0     6518 2023-06-19 04:58:47.000000 ssh_remote_control-0.1.0/src/ssh_remote_control/manager.py
--rw-rw-rw-   0        0        0     5891 2023-06-19 04:59:09.000000 ssh_remote_control-0.1.0/src/ssh_remote_control/sensor.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:23:10.827994 ssh_remote_control-0.1.0/src/ssh_remote_control.egg-info/
--rw-rw-rw-   0        0        0     1428 2023-06-19 10:23:10.000000 ssh_remote_control-0.1.0/src/ssh_remote_control.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-06-19 10:23:10.000000 ssh_remote_control-0.1.0/src/ssh_remote_control.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 10:23:10.000000 ssh_remote_control-0.1.0/src/ssh_remote_control.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-06-19 10:23:10.000000 ssh_remote_control-0.1.0/src/ssh_remote_control.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-19 10:23:10.000000 ssh_remote_control-0.1.0/src/ssh_remote_control.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 13:11:15.887416 ssh_remote_control-0.1.1/
+-rw-rw-rw-   0        0        0     1084 2023-06-19 04:51:08.000000 ssh_remote_control-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1428 2023-06-19 13:11:15.886417 ssh_remote_control-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      832 2023-06-19 10:07:10.000000 ssh_remote_control-0.1.1/README.md
+-rw-rw-rw-   0        0        0      848 2023-06-19 12:29:01.000000 ssh_remote_control-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 13:11:15.887416 ssh_remote_control-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 13:11:15.794908 ssh_remote_control-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 13:11:15.824911 ssh_remote_control-0.1.1/src/ssh_remote_control/
+-rw-rw-rw-   0        0        0    10774 2023-06-19 09:31:24.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/__init__.py
+-rw-rw-rw-   0        0        0     6656 2023-06-19 04:57:57.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/command.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:11:15.883419 ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/
+-rw-rw-rw-   0        0        0      111 2023-06-19 03:25:53.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-06-19 01:38:24.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/const.py
+-rw-rw-rw-   0        0        0     3757 2023-06-19 10:12:42.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/linux.py
+-rw-rw-rw-   0        0        0     3304 2023-06-19 10:13:12.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/windows_cmd.py
+-rw-rw-rw-   0        0        0     3538 2023-06-19 10:14:03.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/windows_ps.py
+-rw-rw-rw-   0        0        0      550 2023-06-19 03:37:58.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/event.py
+-rw-rw-rw-   0        0        0      159 2023-06-19 09:54:09.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/helpers.py
+-rw-rw-rw-   0        0        0     1313 2023-06-19 04:04:40.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/locker.py
+-rw-rw-rw-   0        0        0     6518 2023-06-19 04:58:47.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/manager.py
+-rw-rw-rw-   0        0        0     5891 2023-06-19 04:59:09.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/sensor.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:11:15.869406 ssh_remote_control-0.1.1/src/ssh_remote_control.egg-info/
+-rw-rw-rw-   0        0        0     1428 2023-06-19 13:11:15.000000 ssh_remote_control-0.1.1/src/ssh_remote_control.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-06-19 13:11:15.000000 ssh_remote_control-0.1.1/src/ssh_remote_control.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 13:11:15.000000 ssh_remote_control-0.1.1/src/ssh_remote_control.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-06-19 13:11:15.000000 ssh_remote_control-0.1.1/src/ssh_remote_control.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-19 13:11:15.000000 ssh_remote_control-0.1.1/src/ssh_remote_control.egg-info/top_level.txt
```

### Comparing `ssh_remote_control-0.1.0/LICENSE` & `ssh_remote_control-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.0/PKG-INFO` & `ssh_remote_control-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ssh_remote_control
-Version: 0.1.0
+Version: 0.1.1
 Summary: Control and monitor remote devices through SSH
 Author-email: zhbjsh <zhbjsh@outlook.com>
-Project-URL: Homepage, https://github.com/zhbjsh/ssh_remote_control
-Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh_remote_control/issues
+Project-URL: Homepage, https://github.com/zhbjsh/ssh-remote-control
+Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-remote-control/issues
 Keywords: ssh,command line,remote control
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ssh_remote_control-0.1.0/README.md` & `ssh_remote_control-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.0/pyproject.toml` & `ssh_remote_control-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_remote_control"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor remote devices through SSH"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -21,14 +21,14 @@
   "command line", 
   "remote control",
 ]
 dependencies = [
   "async-timeout >= 4.0.2",
   "icmplib >= 3.0.3",
   "paramiko >= 3.2.0",
-  "python-slugify >= 8.0.1",
+  "python-slugify >= 4.0.1",
   "wakeonlan >= 3.0.0",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/zhbjsh/ssh_remote_control"
-"Bug Tracker" = "https://github.com/zhbjsh/ssh_remote_control/issues"
+"Homepage" = "https://github.com/zhbjsh/ssh-remote-control"
+"Bug Tracker" = "https://github.com/zhbjsh/ssh-remote-control/issues"
```

### Comparing `ssh_remote_control-0.1.0/src/ssh_remote_control/__init__.py` & `ssh_remote_control-0.1.1/src/ssh_remote_control/__init__.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.0/src/ssh_remote_control/command.py` & `ssh_remote_control-0.1.1/src/ssh_remote_control/command.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.0/src/ssh_remote_control/default_commands/const.py` & `ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/const.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.0/src/ssh_remote_control/default_commands/linux.py` & `ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/linux.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.0/src/ssh_remote_control/default_commands/windows_cmd.py` & `ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/windows_cmd.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.0/src/ssh_remote_control/default_commands/windows_ps.py` & `ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/windows_ps.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.0/src/ssh_remote_control/event.py` & `ssh_remote_control-0.1.1/src/ssh_remote_control/event.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.0/src/ssh_remote_control/locker.py` & `ssh_remote_control-0.1.1/src/ssh_remote_control/locker.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.0/src/ssh_remote_control/manager.py` & `ssh_remote_control-0.1.1/src/ssh_remote_control/manager.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.0/src/ssh_remote_control/sensor.py` & `ssh_remote_control-0.1.1/src/ssh_remote_control/sensor.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.0/src/ssh_remote_control.egg-info/PKG-INFO` & `ssh_remote_control-0.1.1/src/ssh_remote_control.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ssh-remote-control
-Version: 0.1.0
+Version: 0.1.1
 Summary: Control and monitor remote devices through SSH
 Author-email: zhbjsh <zhbjsh@outlook.com>
-Project-URL: Homepage, https://github.com/zhbjsh/ssh_remote_control
-Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh_remote_control/issues
+Project-URL: Homepage, https://github.com/zhbjsh/ssh-remote-control
+Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-remote-control/issues
 Keywords: ssh,command line,remote control
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ssh_remote_control-0.1.0/src/ssh_remote_control.egg-info/SOURCES.txt` & `ssh_remote_control-0.1.1/src/ssh_remote_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

