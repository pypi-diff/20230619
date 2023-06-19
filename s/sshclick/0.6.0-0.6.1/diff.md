# Comparing `tmp/sshclick-0.6.0.tar.gz` & `tmp/sshclick-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshclick-0.6.0.tar", max compression
+gzip compressed data, was "sshclick-0.6.1.tar", max compression
```

## Comparing `sshclick-0.6.0.tar` & `sshclick-0.6.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1068 2023-04-17 16:09:18.391084 sshclick-0.6.0/LICENSE
--rw-r--r--   0        0        0    17480 2023-05-20 18:57:10.639154 sshclick-0.6.0/README.md
--rw-r--r--   0        0        0     1065 2023-05-20 16:44:37.720951 sshclick-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-10 13:49:51.835727 sshclick-0.6.0/sshclick/__init__.py
--rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.6.0/sshclick/cmds/__init__.py
--rw-r--r--   0        0        0      455 2023-04-17 12:52:26.614177 sshclick-0.6.0/sshclick/cmds/cmd_config.py
--rw-r--r--   0        0        0      646 2022-08-10 20:50:38.844620 sshclick-0.6.0/sshclick/cmds/cmd_group.py
--rw-r--r--   0        0        0      732 2023-04-14 15:17:18.853394 sshclick-0.6.0/sshclick/cmds/cmd_host.py
--rw-r--r--   0        0        0        0 2023-04-17 12:48:49.004234 sshclick-0.6.0/sshclick/cmds/config/__init__.py
--rw-r--r--   0        0        0     1101 2023-04-17 12:59:37.314064 sshclick-0.6.0/sshclick/cmds/config/config_del.py
--rw-r--r--   0        0        0     1354 2023-04-17 12:59:34.824065 sshclick-0.6.0/sshclick/cmds/config/config_set.py
--rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.6.0/sshclick/cmds/group/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-14 13:48:55.874783 sshclick-0.6.0/sshclick/cmds/group/group_create.py
--rw-r--r--   0        0        0     2217 2023-04-14 13:45:08.024842 sshclick-0.6.0/sshclick/cmds/group/group_delete.py
--rw-r--r--   0        0        0     1068 2022-09-11 17:04:13.785725 sshclick-0.6.0/sshclick/cmds/group/group_list.py
--rw-r--r--   0        0        0     1196 2023-04-14 14:12:19.544415 sshclick-0.6.0/sshclick/cmds/group/group_rename.py
--rw-r--r--   0        0        0     2421 2023-04-14 13:49:04.844781 sshclick-0.6.0/sshclick/cmds/group/group_set.py
--rw-r--r--   0        0        0     2387 2023-04-17 09:36:07.926863 sshclick-0.6.0/sshclick/cmds/group/group_show.py
--rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.6.0/sshclick/cmds/host/__init__.py
--rw-r--r--   0        0        0     3970 2023-05-20 19:07:30.759013 sshclick-0.6.0/sshclick/cmds/host/host_create.py
--rw-r--r--   0        0        0     2458 2023-04-14 14:08:54.144468 sshclick-0.6.0/sshclick/cmds/host/host_delete.py
--rw-r--r--   0        0        0     1715 2023-04-17 09:39:36.716809 sshclick-0.6.0/sshclick/cmds/host/host_install_key.py
--rw-r--r--   0        0        0     4494 2023-04-30 10:40:52.857020 sshclick-0.6.0/sshclick/cmds/host/host_list.py
--rw-r--r--   0        0        0     1162 2023-04-14 14:12:44.404409 sshclick-0.6.0/sshclick/cmds/host/host_rename.py
--rw-r--r--   0        0        0     6579 2023-04-14 14:19:27.594303 sshclick-0.6.0/sshclick/cmds/host/host_set.py
--rw-r--r--   0        0        0     2997 2023-04-26 13:53:34.694329 sshclick-0.6.0/sshclick/cmds/host/host_show.py
--rw-r--r--   0        0        0     2699 2023-05-20 16:34:15.411092 sshclick-0.6.0/sshclick/cmds/host/host_test.py
--rw-r--r--   0        0        0      107 2023-04-17 12:21:37.064660 sshclick-0.6.0/sshclick/globals.py
--rw-r--r--   0        0        0     2535 2023-05-20 18:56:47.529159 sshclick-0.6.0/sshclick/main.py
--rw-r--r--   0        0        0     7832 2023-05-20 18:54:22.169193 sshclick-0.6.0/sshclick/main_tui.py
--rw-r--r--   0        0        0      411 2023-04-26 14:19:59.943911 sshclick-0.6.0/sshclick/sshc/__init__.py
--rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.6.0/sshclick/sshc/host_styles/__init__.py
--rw-r--r--   0        0        0     2312 2022-09-11 16:36:02.105733 sshclick-0.6.0/sshclick/sshc/host_styles/card.py
--rw-r--r--   0        0        0      363 2022-08-08 14:36:37.567084 sshclick-0.6.0/sshclick/sshc/host_styles/json.py
--rw-r--r--   0        0        0     2484 2023-04-17 09:57:40.316526 sshclick-0.6.0/sshclick/sshc/host_styles/panels.py
--rw-r--r--   0        0        0     2262 2022-09-11 16:56:01.465727 sshclick-0.6.0/sshclick/sshc/host_styles/simple.py
--rw-r--r--   0        0        0     1429 2022-08-08 14:36:37.567084 sshclick-0.6.0/sshclick/sshc/host_styles/table.py
--rw-r--r--   0        0        0     1780 2022-08-08 14:36:37.567084 sshclick-0.6.0/sshclick/sshc/host_styles/table2.py
--rw-r--r--   0        0        0    16709 2023-05-20 19:15:16.358913 sshclick-0.6.0/sshclick/sshc/ssh_config.py
--rw-r--r--   0        0        0     4516 2023-04-26 17:00:52.291382 sshclick-0.6.0/sshclick/sshc/ssh_graph.py
--rw-r--r--   0        0        0      434 2023-04-17 08:39:08.357758 sshclick-0.6.0/sshclick/sshc/ssh_group.py
--rw-r--r--   0        0        0     2627 2023-05-01 10:12:53.391675 sshclick-0.6.0/sshclick/sshc/ssh_host.py
--rw-r--r--   0        0        0     4555 2023-04-17 12:20:45.644673 sshclick-0.6.0/sshclick/sshc/ssh_parameters.py
--rw-r--r--   0        0        0     4842 2023-04-17 12:22:18.274649 sshclick-0.6.0/sshclick/sshc/sshutils.py
--rw-r--r--   0        0        0       17 2023-05-20 16:19:03.191299 sshclick-0.6.0/sshclick/version.py
--rw-r--r--   0        0        0    18324 1970-01-01 00:00:00.000000 sshclick-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-17 16:09:18.391084 sshclick-0.6.1/LICENSE
+-rw-r--r--   0        0        0    17532 2023-06-19 07:49:52.377342 sshclick-0.6.1/README.md
+-rw-r--r--   0        0        0     1065 2023-06-19 07:56:31.827277 sshclick-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-08-10 13:49:51.835727 sshclick-0.6.1/sshclick/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.6.1/sshclick/cmds/__init__.py
+-rw-r--r--   0        0        0      455 2023-04-17 12:52:26.614177 sshclick-0.6.1/sshclick/cmds/cmd_config.py
+-rw-r--r--   0        0        0      646 2022-08-10 20:50:38.844620 sshclick-0.6.1/sshclick/cmds/cmd_group.py
+-rw-r--r--   0        0        0      732 2023-04-14 15:17:18.853394 sshclick-0.6.1/sshclick/cmds/cmd_host.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:48:49.004234 sshclick-0.6.1/sshclick/cmds/config/__init__.py
+-rw-r--r--   0        0        0     1101 2023-04-17 12:59:37.314064 sshclick-0.6.1/sshclick/cmds/config/config_del.py
+-rw-r--r--   0        0        0     1354 2023-04-17 12:59:34.824065 sshclick-0.6.1/sshclick/cmds/config/config_set.py
+-rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.6.1/sshclick/cmds/group/__init__.py
+-rw-r--r--   0        0        0     1529 2023-06-15 14:23:03.562525 sshclick-0.6.1/sshclick/cmds/group/group_create.py
+-rw-r--r--   0        0        0     2217 2023-04-14 13:45:08.024842 sshclick-0.6.1/sshclick/cmds/group/group_delete.py
+-rw-r--r--   0        0        0     1068 2022-09-11 17:04:13.785725 sshclick-0.6.1/sshclick/cmds/group/group_list.py
+-rw-r--r--   0        0        0     1196 2023-04-14 14:12:19.544415 sshclick-0.6.1/sshclick/cmds/group/group_rename.py
+-rw-r--r--   0        0        0     2421 2023-04-14 13:49:04.844781 sshclick-0.6.1/sshclick/cmds/group/group_set.py
+-rw-r--r--   0        0        0     2387 2023-04-17 09:36:07.926863 sshclick-0.6.1/sshclick/cmds/group/group_show.py
+-rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.6.1/sshclick/cmds/host/__init__.py
+-rw-r--r--   0        0        0     4044 2023-06-15 14:29:32.038589 sshclick-0.6.1/sshclick/cmds/host/host_create.py
+-rw-r--r--   0        0        0     2458 2023-04-14 14:08:54.144468 sshclick-0.6.1/sshclick/cmds/host/host_delete.py
+-rw-r--r--   0        0        0     1715 2023-04-17 09:39:36.716809 sshclick-0.6.1/sshclick/cmds/host/host_install_key.py
+-rw-r--r--   0        0        0     4494 2023-04-30 10:40:52.857020 sshclick-0.6.1/sshclick/cmds/host/host_list.py
+-rw-r--r--   0        0        0     1162 2023-04-14 14:12:44.404409 sshclick-0.6.1/sshclick/cmds/host/host_rename.py
+-rw-r--r--   0        0        0     6579 2023-04-14 14:19:27.594303 sshclick-0.6.1/sshclick/cmds/host/host_set.py
+-rw-r--r--   0        0        0     2997 2023-04-26 13:53:34.694329 sshclick-0.6.1/sshclick/cmds/host/host_show.py
+-rw-r--r--   0        0        0     2699 2023-05-20 16:34:15.411092 sshclick-0.6.1/sshclick/cmds/host/host_test.py
+-rw-r--r--   0        0        0      107 2023-04-17 12:21:37.064660 sshclick-0.6.1/sshclick/globals.py
+-rw-r--r--   0        0        0     2535 2023-05-20 18:56:47.529159 sshclick-0.6.1/sshclick/main.py
+-rw-r--r--   0        0        0     7892 2023-06-19 07:49:16.677347 sshclick-0.6.1/sshclick/main_tui.py
+-rw-r--r--   0        0        0      411 2023-04-26 14:19:59.943911 sshclick-0.6.1/sshclick/sshc/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.6.1/sshclick/sshc/host_styles/__init__.py
+-rw-r--r--   0        0        0     2312 2022-09-11 16:36:02.105733 sshclick-0.6.1/sshclick/sshc/host_styles/card.py
+-rw-r--r--   0        0        0      363 2022-08-08 14:36:37.567084 sshclick-0.6.1/sshclick/sshc/host_styles/json.py
+-rw-r--r--   0        0        0     2484 2023-04-17 09:57:40.316526 sshclick-0.6.1/sshclick/sshc/host_styles/panels.py
+-rw-r--r--   0        0        0     2262 2022-09-11 16:56:01.465727 sshclick-0.6.1/sshclick/sshc/host_styles/simple.py
+-rw-r--r--   0        0        0     1429 2022-08-08 14:36:37.567084 sshclick-0.6.1/sshclick/sshc/host_styles/table.py
+-rw-r--r--   0        0        0     1780 2022-08-08 14:36:37.567084 sshclick-0.6.1/sshclick/sshc/host_styles/table2.py
+-rw-r--r--   0        0        0    16709 2023-06-15 14:23:09.902521 sshclick-0.6.1/sshclick/sshc/ssh_config.py
+-rw-r--r--   0        0        0     4516 2023-04-26 17:00:52.291382 sshclick-0.6.1/sshclick/sshc/ssh_graph.py
+-rw-r--r--   0        0        0      434 2023-04-17 08:39:08.357758 sshclick-0.6.1/sshclick/sshc/ssh_group.py
+-rw-r--r--   0        0        0     2627 2023-05-01 10:12:53.391675 sshclick-0.6.1/sshclick/sshc/ssh_host.py
+-rw-r--r--   0        0        0     4555 2023-04-17 12:20:45.644673 sshclick-0.6.1/sshclick/sshc/ssh_parameters.py
+-rw-r--r--   0        0        0     4842 2023-04-17 12:22:18.274649 sshclick-0.6.1/sshclick/sshc/sshutils.py
+-rw-r--r--   0        0        0       17 2023-06-19 07:56:50.407274 sshclick-0.6.1/sshclick/version.py
+-rw-r--r--   0        0        0    18376 1970-01-01 00:00:00.000000 sshclick-0.6.1/PKG-INFO
```

### Comparing `sshclick-0.6.0/LICENSE` & `sshclick-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/README.md` & `sshclick-0.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # SSH Click Config manager (sshclick)
 
-![splash_gif](tapes/splash.gif)
+![splash_gif](https://github.com/karlot/tapes/splash.gif)
 
 ## Links
 
 - [Intro](https://github.com/karlot/sshclick#intro)
 - [Why?](https://github.com/karlot/sshclick#why)
 - [What does it do](https://github.com/karlot/sshclick#what-does-it-do)
   - [Installation procedure](https://github.com/karlot/sshclick#installation-procedure)
@@ -31,15 +31,15 @@
 Backup your SSH config files before using!  
 SSHClick can be used with "show" and "list" commands for hosts, without modifying your SSH Config in any way!  
 
 **Only commands that modify configuration will edit and rewrite/restructure your SSH Config file. In that case, any added comment or infos that are not in form that SSHClick understand will be discarded, and configuration will be re-formatted to match SSHClick style. See below details to understand how SSH Click would keep your config organized**
 
 **NEW!** *Now comes with additional TUI that can be accessed via `sshc tui` or `ssht`.*  
 
-![splash_gif](tapes/sshc_tui_example.svg)
+![splash_gif](https://github.com/karlot/tapes/sshc_tui_example.svg)
 
 
 ## Why?
 
 * I need something that works fast and great in terminal, and does not require complex setup.
 * SSH config is the only config I need to backup.
 * SSH config is very feature-full with all options SSH client support, why inventing extra layer?
```

### Comparing `sshclick-0.6.0/pyproject.toml` & `sshclick-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # !!! Remember to update version here and in the code !!! 
 # (ಠ_ಠ)  -- I wish poetry could just read version from the package
 
 [tool.poetry]
 name = "sshclick"
 homepage = "https://github.com/karlot/sshclick"
-version = "0.6.0"
+version = "0.6.1"
 description = "SSH Config manager"
 authors = ["Karlo Tisaj <karlot@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
```

### Comparing `sshclick-0.6.0/sshclick/cmds/cmd_group.py` & `sshclick-0.6.1/sshclick/cmds/cmd_group.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/cmds/cmd_host.py` & `sshclick-0.6.1/sshclick/cmds/cmd_host.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/cmds/config/config_del.py` & `sshclick-0.6.1/sshclick/cmds/config/config_del.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/cmds/config/config_set.py` & `sshclick-0.6.1/sshclick/cmds/config/config_set.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/cmds/group/group_create.py` & `sshclick-0.6.1/sshclick/cmds/group/group_create.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 @click.option("-i", "--info", multiple=True, help=INFO_HELP)
 @click.argument("name")
 @click.pass_context
 def cmd(ctx, name, desc, info):
     config: SSH_Config = ctx.obj
 
     # Check if already group exists
-    if not config.check_group_by_name(name):
+    if config.check_group_by_name(name):
         print(f"Cannot create new group '{name}', as group already exists with this name")
         ctx.exit(1)
 
     new_group = SSH_Group(name, desc=desc, info=list(info))
 
     # Add new group to config and show newly created group
     config.groups.append(new_group)
```

### Comparing `sshclick-0.6.0/sshclick/cmds/group/group_delete.py` & `sshclick-0.6.1/sshclick/cmds/group/group_delete.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/cmds/group/group_list.py` & `sshclick-0.6.1/sshclick/cmds/group/group_list.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/cmds/group/group_rename.py` & `sshclick-0.6.1/sshclick/cmds/group/group_rename.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/cmds/group/group_set.py` & `sshclick-0.6.1/sshclick/cmds/group/group_set.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/cmds/group/group_show.py` & `sshclick-0.6.1/sshclick/cmds/group/group_show.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/cmds/host/host_create.py` & `sshclick-0.6.1/sshclick/cmds/host/host_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,27 +43,30 @@
     # Find group by name where to store config
     target_group_exists = config.check_group_by_name(target_group_name)
 
     if not target_group_exists and not force:
         print(f"Cannot create host '{name}' in group '{target_group_name}' since the group does not exist")
         print("Create group first, or use '--force' option to create it automatically!")
         ctx.exit(1)
+        # unreachable, but avoids issues with static checks
+        exit(1)
     elif not target_group_exists:
         target_group = SSH_Group(name=target_group_name)
         config.groups.append(target_group)
     else:
         target_group = config.get_group_by_name(target_group_name)
 
     # This is patter host
     target_type = "pattern" if "*" in name else "normal"
     new_host = SSH_Host(name=name, group=target_group_name, type=target_type, info=list(info))
 
     # Add all passed parameters to config
     for param, value in parameter:
-        param = param.lower()           # parametar keyword will be lowercased as they are case insensitive
+        # parametar keyword will be lowercased as they are case insensitive
+        param = param.lower()
         if not value or value.isspace():
             print(f"Cannot define empty value for parameter during host creation!")
             ctx.exit(1)
         if param in PARAMS_WITH_ALLOWED_MULTIPLE_VALUES:
             # We need to handle host parameter as "list"
             if not param in new_host.params:
                 new_host.params[param] = [ value ]
```

### Comparing `sshclick-0.6.0/sshclick/cmds/host/host_delete.py` & `sshclick-0.6.1/sshclick/cmds/host/host_delete.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/cmds/host/host_install_key.py` & `sshclick-0.6.1/sshclick/cmds/host/host_install_key.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/cmds/host/host_list.py` & `sshclick-0.6.1/sshclick/cmds/host/host_list.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/cmds/host/host_rename.py` & `sshclick-0.6.1/sshclick/cmds/host/host_rename.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/cmds/host/host_set.py` & `sshclick-0.6.1/sshclick/cmds/host/host_set.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/cmds/host/host_show.py` & `sshclick-0.6.1/sshclick/cmds/host/host_show.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/cmds/host/host_test.py` & `sshclick-0.6.1/sshclick/cmds/host/host_test.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/main.py` & `sshclick-0.6.1/sshclick/main.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/main_tui.py` & `sshclick-0.6.1/sshclick/main_tui.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     }
     """
 
     def __init__(self, sshconf=None):
         if isinstance(sshconf, SSH_Config):
             self.sshconf = sshconf
         else:
-            USER_SSH_CONFIG = USER_DEMO_CONFIG
+            # USER_SSH_CONFIG = USER_DEMO_CONFIG
             self.sshconf = SSH_Config(file=os.path.expanduser(USER_SSH_CONFIG)).read().parse()
         super().__init__()
 
     def compose(self) -> ComposeResult:
         yield Header(show_clock=True)
         with Container():
             ssh_tree = Tree(f"SSH Configuration ({len(self.sshconf.groups)} groups)", id="sshtree", data=None)
@@ -213,7 +213,11 @@
             driver.stop_application_mode()
             try:
                 subprocess.run(command, shell=True)
                 time.sleep(2)
             finally:
                 self.refresh()
                 driver.start_application_mode()
+
+## Entry for "ssht" command
+def tui():
+    SSHTui().run()
```

### Comparing `sshclick-0.6.0/sshclick/sshc/host_styles/card.py` & `sshclick-0.6.1/sshclick/sshc/host_styles/card.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/sshc/host_styles/panels.py` & `sshclick-0.6.1/sshclick/sshc/host_styles/panels.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/sshc/host_styles/simple.py` & `sshclick-0.6.1/sshclick/sshc/host_styles/simple.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/sshc/host_styles/table.py` & `sshclick-0.6.1/sshclick/sshc/host_styles/table.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/sshc/host_styles/table2.py` & `sshclick-0.6.1/sshclick/sshc/host_styles/table2.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/sshc/ssh_config.py` & `sshclick-0.6.1/sshclick/sshc/ssh_config.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/sshc/ssh_graph.py` & `sshclick-0.6.1/sshclick/sshc/ssh_graph.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/sshc/ssh_host.py` & `sshclick-0.6.1/sshclick/sshc/ssh_host.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/sshc/ssh_parameters.py` & `sshclick-0.6.1/sshclick/sshc/ssh_parameters.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/sshclick/sshc/sshutils.py` & `sshclick-0.6.1/sshclick/sshc/sshutils.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.6.0/PKG-INFO` & `sshclick-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sshclick
-Version: 0.6.0
+Version: 0.6.1
 Summary: SSH Config manager
 Home-page: https://github.com/karlot/sshclick
 License: MIT
 Author: Karlo Tisaj
 Author-email: karlot@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,15 @@
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: rich (>=13.3,<14.0)
 Requires-Dist: textual (>=0.26,<0.27)
 Description-Content-Type: text/markdown
 
 # SSH Click Config manager (sshclick)
 
-![splash_gif](tapes/splash.gif)
+![splash_gif](https://github.com/karlot/tapes/splash.gif)
 
 ## Links
 
 - [Intro](https://github.com/karlot/sshclick#intro)
 - [Why?](https://github.com/karlot/sshclick#why)
 - [What does it do](https://github.com/karlot/sshclick#what-does-it-do)
   - [Installation procedure](https://github.com/karlot/sshclick#installation-procedure)
@@ -55,15 +55,15 @@
 Backup your SSH config files before using!  
 SSHClick can be used with "show" and "list" commands for hosts, without modifying your SSH Config in any way!  
 
 **Only commands that modify configuration will edit and rewrite/restructure your SSH Config file. In that case, any added comment or infos that are not in form that SSHClick understand will be discarded, and configuration will be re-formatted to match SSHClick style. See below details to understand how SSH Click would keep your config organized**
 
 **NEW!** *Now comes with additional TUI that can be accessed via `sshc tui` or `ssht`.*  
 
-![splash_gif](tapes/sshc_tui_example.svg)
+![splash_gif](https://github.com/karlot/tapes/sshc_tui_example.svg)
 
 
 ## Why?
 
 * I need something that works fast and great in terminal, and does not require complex setup.
 * SSH config is the only config I need to backup.
 * SSH config is very feature-full with all options SSH client support, why inventing extra layer?
```

