# Comparing `tmp/sai-airflow-plugins-0.1.9.tar.gz` & `tmp/sai-airflow-plugins-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sai-airflow-plugins-0.1.9.tar", last modified: Mon Sep  5 14:42:31 2022, max compression
+gzip compressed data, was "sai-airflow-plugins-0.2.0.tar", last modified: Mon Jun 19 13:17:34 2023, max compression
```

## Comparing `sai-airflow-plugins-0.1.9.tar` & `sai-airflow-plugins-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:42:31.886773 sai-airflow-plugins-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-09-05 14:42:31.886773 sai-airflow-plugins-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:42:31.882773 sai-airflow-plugins-0.1.9/sai_airflow_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:42:31.886773 sai-airflow-plugins-0.1.9/sai_airflow_plugins/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4407 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins/hooks/fabric_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)     5125 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins/hooks/mattermost_webhook_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:42:31.886773 sai-airflow-plugins-0.1.9/sai_airflow_plugins/operators/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2159 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins/operators/conditional_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)     4280 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins/operators/conditional_skip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)    13371 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins/operators/fabric_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4010 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins/operators/mattermost_webhook_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:42:31.886773 sai-airflow-plugins-0.1.9/sai_airflow_plugins/sensors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins/sensors/conditional_sensors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins/sensors/fabric_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:42:31.886773 sai-airflow-plugins-0.1.9/sai_airflow_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-09-05 14:42:31.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-09-05 14:42:31.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 14:42:31.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-05 14:42:31.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-05 14:42:31.000000 sai-airflow-plugins-0.1.9/sai_airflow_plugins.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-09-05 14:42:31.886773 sai-airflow-plugins-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:42:31.886773 sai-airflow-plugins-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/tests/mocked_fabric_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)     4009 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/tests/test_conditional_skip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     4625 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/tests/test_fabric_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)     7749 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/tests/test_fabric_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/tests/test_fabric_sensor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2541 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/tests/test_mattermost_webhook_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-09-05 14:42:21.000000 sai-airflow-plugins-0.1.9/tests/test_mattermost_webhook_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:34.777865 sai-airflow-plugins-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-19 13:17:34.777865 sai-airflow-plugins-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:34.773865 sai-airflow-plugins-0.2.0/sai_airflow_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:34.773865 sai-airflow-plugins-0.2.0/sai_airflow_plugins/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/hooks/fabric_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/hooks/mattermost_webhook_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:34.777865 sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/conditional_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/conditional_skip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/fabric_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/mattermost_webhook_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:34.777865 sai-airflow-plugins-0.2.0/sai_airflow_plugins/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/sensors/conditional_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins/sensors/fabric_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:34.773865 sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-19 13:17:34.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-19 13:17:34.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:17:34.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-19 13:17:34.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 13:17:34.000000 sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-19 13:17:34.777865 sai-airflow-plugins-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:34.777865 sai-airflow-plugins-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/mocked_fabric_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/test_conditional_skip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/test_fabric_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/test_fabric_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/test_fabric_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/test_mattermost_webhook_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-19 13:17:25.000000 sai-airflow-plugins-0.2.0/tests/test_mattermost_webhook_operator.py
```

### Comparing `sai-airflow-plugins-0.1.9/LICENSE` & `sai-airflow-plugins-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.1.9/PKG-INFO` & `sai-airflow-plugins-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: sai-airflow-plugins
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python package with various operators, hooks and utilities for Apache Airflow
 Home-page: https://github.com/Slimmer-AI/sai-airflow-plugins
 Author: Slimmer.AI
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: System :: Monitoring
 Provides-Extra: docs
 Provides-Extra: tests
 License-File: LICENSE
 
 sai-airflow-plugins
```

### Comparing `sai-airflow-plugins-0.1.9/README.rst` & `sai-airflow-plugins-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.1.9/sai_airflow_plugins/hooks/fabric_hook.py` & `sai-airflow-plugins-0.2.0/sai_airflow_plugins/hooks/fabric_hook.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.1.9/sai_airflow_plugins/hooks/mattermost_webhook_hook.py` & `sai-airflow-plugins-0.2.0/sai_airflow_plugins/hooks/mattermost_webhook_hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     :param http_conn_id: connection that optionally has a Mattermost webhook token in the extra field
     :param webhook_token: Mattermost webhook token. If http_conn_id isn't supplied this should be the full webhook url.
     :param message: The message you want to send on Mattermost
     :param attachments: The attachments to send on Mattermost. Should be a list of dictionaries representing
                         Mattermost attachments.
     :param props: The props to send on Mattermost. Should be a dictionary representing Mattermost props.
     :param post_type: Sets an optional Mattermost post type, mainly for use by plugins. If supplied, must begin with
-                      "custom_"
+                      ``custom_``
     :param channel: The channel the message should be posted to
     :param username: The username to post with
     :param icon_emoji: The emoji to use as icon for the user posting to Mattermost
     :param icon_url: The icon image URL string to use in place of the default icon.
     :param proxy: Proxy to use to make the Mattermost webhook call
     :param extra_options: Extra options for http hook
     """
```

### Comparing `sai-airflow-plugins-0.1.9/sai_airflow_plugins/operators/conditional_operators.py` & `sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/conditional_operators.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.1.9/sai_airflow_plugins/operators/conditional_skip_mixin.py` & `sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/conditional_skip_mixin.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.1.9/sai_airflow_plugins/operators/fabric_operator.py` & `sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/fabric_operator.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,16 +24,21 @@
                         provided. (templated)
     :param remote_host: remote host to connect. (templated) Nullable. If provided, it will replace the `remote_host`
                         which was defined in `fabric_hook` or predefined in the connection of `ssh_conn_id`.
     :param command: command to execute on remote host. (templated)
     :param use_sudo: uses Fabric's sudo function instead of run. Because this function automatically adds a responder
                      for the password prompt, parameter `add_sudo_password_responder` will be ignored. It uses the
                      SSH connection's password as reply.
-    :param sudo_user: If `use_sudo` is `True`, run the command as this user. If not supplied it will run as root.
-                      This parameter is ignored if `use_sudo` is `False`.
+    :param use_sudo_shell: wraps the command in a sudo shell. The difference with `use_sudo` is that Fabric's sudo
+                           function only executes a single command as sudo. Within a sudo shell a full script can be
+                           run, e.g. a templated script file. This does *not* automatically add a sudo responder
+                           for the password prompt. Use `add_sudo_password_responder` as necessary.
+                           This parameter can't be used at the same time as `use_sudo`.
+    :param sudo_user: If `use_sudo` or `use_sudo_shell` is `True`, run the command as this user. If not supplied it will
+                      run as root. This parameter is ignored if `use_sudo` and `use_sudo_shell` are `False`.
     :param watchers: Watchers for responding to specific command output. This is a list of dicts specifying a class
                      of type ``StreamWatcher`` and its arguments. For each dict the corresponding object is created
                      and added to Fabric's run function. It's done this way because arguments to an operator are
                      pickled and StreamWatcher objects are derived from thread.local which can't be pickled.
                      Example:
                      >>> {"watchers": [{"class": Responder, "pattern": r"Continue\\?", "response": "yes\\n"}]}
                      See also: http://docs.pyinvoke.org/en/latest/concepts/watchers.html
@@ -72,14 +77,15 @@
     @apply_defaults
     def __init__(self,
                  fabric_hook: Optional[FabricHook] = None,
                  ssh_conn_id: Optional[str] = None,
                  remote_host: Optional[str] = None,
                  command: str = None,
                  use_sudo: Optional[bool] = False,
+                 use_sudo_shell: Optional[bool] = False,
                  sudo_user: Optional[str] = None,
                  watchers: Optional[List[Dict[str, Any]]] = None,
                  add_sudo_password_responder: Optional[bool] = False,
                  add_generic_password_responder: Optional[bool] = False,
                  add_unknown_host_key_responder: Optional[bool] = False,
                  connect_timeout: Optional[int] = 10,
                  environment: Optional[Dict[str, Any]] = None,
@@ -92,14 +98,15 @@
                  **kwargs):
         super().__init__(*args, **kwargs)
         self.fabric_hook = fabric_hook
         self.ssh_conn_id = ssh_conn_id
         self.remote_host = remote_host
         self.command = command
         self.use_sudo = use_sudo
+        self.use_sudo_shell = use_sudo_shell
         self.sudo_user = sudo_user
         self.watchers = watchers or []
         self.add_sudo_password_responder = False if self.use_sudo else add_sudo_password_responder
         self.add_generic_password_responder = add_generic_password_responder
         self.add_unknown_host_key_responder = add_unknown_host_key_responder
         self.connect_timeout = connect_timeout
         self.environment = environment or {}
@@ -110,15 +117,15 @@
         self.keepalive = keepalive
 
     def execute(self, context: Dict):
         """
         Executes ``self.command`` over the configured SSH connection.
 
         :param context: Context dict provided by airflow
-        :return: True or the connection's stdout if ``self.do_xcom_push`` is True.
+        :return: True if the command executed correctly.
                  On an error, raises AirflowException.
         """
         result = self.execute_fabric_command()
 
         if result.exited == 0:
             # Push the output to an XCom if requested
             if self.xcom_push_key and result.stdout:
@@ -162,14 +169,17 @@
 
             else:
                 raise AirflowException("Cannot operate without fabric_hook or ssh_conn_id.")
 
             if not self.command:
                 raise AirflowException("SSH command not specified. Aborting.")
 
+            if self.use_sudo and self.use_sudo_shell:
+                raise AirflowException("Cannot use use_sudo and use_sudo_shell at the same time. Aborting.")
+
             conn = self.fabric_hook.get_fabric_conn()
 
             # Create watcher objects, using the provided dictionary to instantiate the class and supply its kwargs
             watchers = []
             for watcher_dict in self.watchers:
                 try:
                     watcher_class = watcher_dict.pop("class")
@@ -191,33 +201,42 @@
 
             if self.add_generic_password_responder:
                 watchers.append(self.fabric_hook.get_generic_pass_responder())
 
             if self.add_unknown_host_key_responder:
                 watchers.append(self.fabric_hook.get_unknown_host_key_responder())
 
+            # Wrap command in sudo shell if requested
+            if self.use_sudo_shell:
+                sudo_params = f"-su {self.sudo_user}" if self.sudo_user else "-s"
+                command = f"sudo {sudo_params} -- <<'__end_of_sudo_shell__'\n" \
+                          f"{self.command}\n" \
+                          f"__end_of_sudo_shell__"
+            else:
+                command = self.command
+
             if self.use_sudo:
                 if self.sudo_user:
-                    self.log.info(f"Running sudo command as '{self.sudo_user}': {self.command}")
+                    self.log.info(f"Running sudo command as '{self.sudo_user}': {command}")
                 else:
-                    self.log.info(f"Running sudo command: {self.command}")
+                    self.log.info(f"Running sudo command: {command}")
             else:
-                self.log.info(f"Running command: {self.command}")
+                self.log.info(f"Running command: {command}")
 
             if self.environment:
                 formatted_env_msg = "\n".join(f"{k}={v}" for k, v in self.environment.items())
                 self.log.info(f"With environment variables:\n{formatted_env_msg}")
 
             # Open connection and set transport-specific options
             conn.open()
             conn.transport.set_keepalive(self.keepalive)
 
             # Set up runtime options and run the command
             run_kwargs = dict(
-                command=self.command,
+                command=command,
                 pty=self.get_pty,
                 env=self.environment,
                 watchers=watchers,
                 warn=True  # don't directly raise an UnexpectedExit when the exit code is non-zero
             )
 
             if self.use_sudo:
```

### Comparing `sai-airflow-plugins-0.1.9/sai_airflow_plugins/operators/mattermost_webhook_operator.py` & `sai-airflow-plugins-0.2.0/sai_airflow_plugins/operators/mattermost_webhook_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     :param http_conn_id: connection that optionally has a Mattermost webhook token in the extra field
     :param webhook_token: Mattermost webhook token. If http_conn_id isn't supplied this should be the full webhook url.
     :param message: The message you want to send on Mattermost
     :param attachments: The attachments to send on Mattermost. Should be a list of dictionaries representing
                         Mattermost attachments.
     :param props: The props to send on Mattermost. Should be a dictionary representing Mattermost props.
     :param post_type: Sets an optional Mattermost post type, mainly for use by plugins. If supplied, must begin with
-                      "custom_"
+                      ``custom_``
     :param channel: The channel the message should be posted to
     :param username: The username to post with
     :param icon_emoji: The emoji to use as icon for the user posting to Mattermost
     :param icon_url: The icon image URL string to use in place of the default icon.
     :param proxy: Proxy to use to make the Mattermost webhook call
     :param extra_options: Extra options for http hook
     """
```

### Comparing `sai-airflow-plugins-0.1.9/sai_airflow_plugins/sensors/conditional_sensors.py` & `sai-airflow-plugins-0.2.0/sai_airflow_plugins/sensors/conditional_sensors.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.1.9/sai_airflow_plugins/sensors/fabric_sensor.py` & `sai-airflow-plugins-0.2.0/sai_airflow_plugins/sensors/fabric_sensor.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.1.9/sai_airflow_plugins.egg-info/PKG-INFO` & `sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: sai-airflow-plugins
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python package with various operators, hooks and utilities for Apache Airflow
 Home-page: https://github.com/Slimmer-AI/sai-airflow-plugins
 Author: Slimmer.AI
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: System :: Monitoring
 Provides-Extra: docs
 Provides-Extra: tests
 License-File: LICENSE
 
 sai-airflow-plugins
```

### Comparing `sai-airflow-plugins-0.1.9/sai_airflow_plugins.egg-info/SOURCES.txt` & `sai-airflow-plugins-0.2.0/sai_airflow_plugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.1.9/setup.py` & `sai-airflow-plugins-0.2.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 
 requirements = [
     "apache-airflow[ssh]>=1.10",
     "fabric>=2.5"
 ]
 
 requirements_docs = [
-    "sphinx>=3.5,<4",
+    "sphinx>=5,<6",
     "sphinx-rtd-theme",
     "sphinx-autodoc-typehints",
-    "sphinx-versions==1.0.1"
+    "sphinx-versions==1.0.1",
+    "click<8"  # Prevents `AttributeError: module 'click' has no attribute 'get_os_args'` on Python 3.11
 ]
 
 requirements_tests = [
     "pytest",
     "faker"
 ]
 
@@ -45,17 +46,18 @@
         # Development status
         "Development Status :: 5 - Production/Stable",
 
         # Environments
         "Environment :: Plugins",
 
         # Supported Python versions
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
 
         # License
         "License :: OSI Approved :: Apache Software License",
 
         # Topic
         "Topic :: System :: Monitoring"
     ]
```

### Comparing `sai-airflow-plugins-0.1.9/tests/mocked_fabric_hook.py` & `sai-airflow-plugins-0.2.0/tests/mocked_fabric_hook.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.1.9/tests/test_conditional_skip_mixin.py` & `sai-airflow-plugins-0.2.0/tests/test_conditional_skip_mixin.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.1.9/tests/test_fabric_hook.py` & `sai-airflow-plugins-0.2.0/tests/test_fabric_hook.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.1.9/tests/test_fabric_operator.py` & `sai-airflow-plugins-0.2.0/tests/test_fabric_operator.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,14 +83,49 @@
                             use_sudo=True, sudo_user=sudo_user)
 
         res = op.execute_fabric_command()
         res.conn.open.assert_called()
         res.conn.sudo.assert_called_with(command=command, pty=pty, env=env, watchers=[], warn=True,
                                          password=self.hook.password, user=sudo_user)
 
+    def test_fabric_operator_use_sudo_shell(self):
+        """
+        Test that parameter use_sudo_shell wraps the command in a sudo shell
+        """
+        command = faker.text()
+        env = faker.pydict()
+        pty = faker.pybool()
+        op = FabricOperator(task_id=TEST_TASK_ID, fabric_hook=self.hook, command=command, environment=env, get_pty=pty,
+                            use_sudo_shell=True)
+
+        res = op.execute_fabric_command()
+
+        expected_command = f"sudo -s -- <<'__end_of_sudo_shell__'\n{command}\n__end_of_sudo_shell__"
+
+        res.conn.open.assert_called()
+        res.conn.run.assert_called_with(command=expected_command, pty=pty, env=env, watchers=[], warn=True)
+
+    def test_fabric_operator_use_sudo_shell_with_user(self):
+        """
+        Test that parameter use_sudo_shell wraps the command in a sudo shell for the specified user
+        """
+        command = faker.text()
+        env = faker.pydict()
+        pty = faker.pybool()
+        sudo_user = faker.user_name()
+        op = FabricOperator(task_id=TEST_TASK_ID, fabric_hook=self.hook, command=command, environment=env, get_pty=pty,
+                            use_sudo_shell=True, sudo_user=sudo_user)
+
+        res = op.execute_fabric_command()
+
+        expected_command = f"sudo -su {sudo_user} -- <<'__end_of_sudo_shell__'\n{command}\n__end_of_sudo_shell__"
+
+        res.conn.open.assert_called()
+        res.conn.run.assert_called_with(command=expected_command, pty=pty, env=env, watchers=[], warn=True)
+
     def test_fabric_operator_execute_non_zero_exit(self):
         """
         Test that execution with a non-zero exit code fails and the exit code is logged
         """
         self.hook.exit_code = faker.pyint(min_value=1)
         op = FabricOperator(task_id=TEST_TASK_ID, fabric_hook=self.hook, command="ls")
```

### Comparing `sai-airflow-plugins-0.1.9/tests/test_fabric_sensor.py` & `sai-airflow-plugins-0.2.0/tests/test_fabric_sensor.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.1.9/tests/test_mattermost_webhook_hook.py` & `sai-airflow-plugins-0.2.0/tests/test_mattermost_webhook_hook.py`

 * *Files identical despite different names*

### Comparing `sai-airflow-plugins-0.1.9/tests/test_mattermost_webhook_operator.py` & `sai-airflow-plugins-0.2.0/tests/test_mattermost_webhook_operator.py`

 * *Files identical despite different names*

