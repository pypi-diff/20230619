# Comparing `tmp/dfsync-0.3.7.tar.gz` & `tmp/dfsync-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfsync-0.3.7.tar", last modified: Fri Jul 16 06:17:12 2021, max compression
+gzip compressed data, was "dfsync-0.3.8.tar", last modified: Mon Aug  9 17:21:41 2021, max compression
```

## Comparing `dfsync-0.3.7.tar` & `dfsync-0.3.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       22 2021-03-27 05:46:27.532800 dfsync-0.3.7/dfsync/__init__.py
--rw-r--r--   0        0        0       64 2021-04-06 10:05:47.667270 dfsync-0.3.7/dfsync/backends/__init__.py
--rw-r--r--   0        0        0    21020 2021-07-16 06:12:03.542397 dfsync-0.3.7/dfsync/backends/kube.py
--rwxr-xr-x   0        0        0     1307 2021-03-15 10:10:49.575860 dfsync-0.3.7/dfsync/backends/kube_exec.py
--rw-r--r--   0        0        0     4780 2021-07-15 05:23:26.792307 dfsync-0.3.7/dfsync/backends/rsync.py
--rw-r--r--   0        0        0      475 2021-05-23 23:31:09.551867 dfsync-0.3.7/dfsync/char_ui.py
--rw-r--r--   0        0        0      125 2021-03-17 16:28:00.884270 dfsync-0.3.7/dfsync/cli.py
--rw-r--r--   0        0        0     3241 2021-03-30 12:50:07.393669 dfsync-0.3.7/dfsync/exp.py
--rw-r--r--   0        0        0     5225 2021-05-24 01:03:50.413273 dfsync-0.3.7/dfsync/filters.py
--rw-r--r--   0        0        0     6445 2021-07-15 10:38:01.962557 dfsync-0.3.7/dfsync/monitor.py
--rw-r--r--   0        0        0     3350 2021-04-28 13:06:18.000000 dfsync-0.3.7/dfsync/transactions.py
--rw-r--r--   0        0        0      436 2021-07-16 06:12:35.210708 dfsync-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      785 2021-07-16 06:17:12.551708 dfsync-0.3.7/setup.py
--rw-r--r--   0        0        0      503 2021-07-16 06:17:12.552019 dfsync-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0       22 2021-03-27 05:46:27.532800 dfsync-0.3.8/dfsync/__init__.py
+-rw-r--r--   0        0        0       64 2021-04-06 10:05:47.667270 dfsync-0.3.8/dfsync/backends/__init__.py
+-rw-r--r--   0        0        0    21420 2021-08-09 17:18:08.988648 dfsync-0.3.8/dfsync/backends/kube.py
+-rwxr-xr-x   0        0        0     1600 2021-08-09 16:54:53.225674 dfsync-0.3.8/dfsync/backends/kube_exec.py
+-rw-r--r--   0        0        0     4780 2021-07-15 05:23:26.792307 dfsync-0.3.8/dfsync/backends/rsync.py
+-rw-r--r--   0        0        0      475 2021-05-23 23:31:09.551867 dfsync-0.3.8/dfsync/char_ui.py
+-rw-r--r--   0        0        0      125 2021-03-17 16:28:00.884270 dfsync-0.3.8/dfsync/cli.py
+-rw-r--r--   0        0        0     3241 2021-03-30 12:50:07.393669 dfsync-0.3.8/dfsync/exp.py
+-rw-r--r--   0        0        0     5225 2021-05-24 01:03:50.413273 dfsync-0.3.8/dfsync/filters.py
+-rw-r--r--   0        0        0     6610 2021-08-09 17:19:30.466837 dfsync-0.3.8/dfsync/monitor.py
+-rw-r--r--   0        0        0     3350 2021-04-28 13:06:18.000000 dfsync-0.3.8/dfsync/transactions.py
+-rw-r--r--   0        0        0      436 2021-08-09 17:20:34.624075 dfsync-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      785 2021-08-09 17:21:42.324396 dfsync-0.3.8/setup.py
+-rw-r--r--   0        0        0      503 2021-08-09 17:21:42.324673 dfsync-0.3.8/PKG-INFO
```

### Comparing `dfsync-0.3.7/dfsync/backends/kube.py` & `dfsync-0.3.8/dfsync/backends/kube.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,17 +143,14 @@
 
 
 def get_selected_kubernetes(kube_host=None):
     contexts, active_context = config.list_kube_config_contexts()
     if not contexts:
         raise ValueError("Cannot find any kubernetes contexts in kube-config file")
 
-    # TODO: remove this statement once kube_exec has been updated to work with an arbitrary context
-    kube_host = None
-
     context_apis = []
     selected_context = None
     selected_context_api = None
     active_context_api = None
     multiple_matches = False
     for c in contexts:
         ctx_client = client.CoreV1Api(api_client=config.new_client_from_config(context=c["name"]))
@@ -183,38 +180,43 @@
 
             if len(tags) > 0:
                 tags_str = ",".join(tags)
                 print(f"  * {c['name']} on {ctx_api_host} [{tags_str}]")
             else:
                 print(f"  * {c['name']} on {ctx_api_host}")
         if kube_host is None:
-            print(f"Use 'kubectl config set current-context <name>' to set the current context\n")
+            ctx_api_host = active_context_api.api_client.configuration.host
+            print(
+                f"Add --kube-host={ctx_api_host} to use a specific kubernetes API host\n"
+                f"Alternatively, use 'kubectl config set current-context <name>' to set the current context"
+            )
 
     if kube_host is not None and selected_context is None:
         raise ValueError(f"None of the kubernetes contexts match '{kube_host}'")
 
     if selected_context is None:
         selected_context = active_context
         selected_context_api = active_context_api
     return selected_context, selected_context_api
 
 
 class KubeReDeployer:
-    def __init__(self, kube_host=None, **kwargs):
+    def __init__(self, kube_host=None, pod_timeout=30, **kwargs):
         config.load_kube_config()
 
         selected_context, selected_context_api = get_selected_kubernetes(kube_host)
 
         self.context_name = selected_context["name"]
         self.api = selected_context_api
         self.apps_api = client.AppsV1Api(api_client=config.new_client_from_config(context=self.context_name))
 
         print(f"Using cluster: {self.context_name} on {self.api.api_client.configuration.host}")
         self.rsync_backend_instance = rsync_backend()
         self._image_distro = None
+        self.pod_timeout = pod_timeout
 
     def supervisor_install(self, pod, spec, status):
         if self._is_supervised(pod, spec, status):
             return
 
         command = self._image_distro.get_supervise_command()
         deployments = self._set_deployment_command(pod, spec, status, command)
@@ -350,14 +352,15 @@
 
     def get_exec_command(self, namespace, pod_name, container_name):
         py_path = os.path.abspath(sys.executable)
         backends_dir, _ = os.path.split(os.path.abspath(__file__))
         cmd = [py_path, os.path.join(backends_dir, "kube_exec.py")]
         env = {
             **os.environ,
+            "KUBEEXEC_CONTEXT": self.context_name,
             "KUBEEXEC_POD": pod_name,
             "KUBEEXEC_NAMESPACE": namespace,
             "KUBEEXEC_CONTAINER": container_name,
         }
         return " ".join(cmd), env
 
     def list_deployments(self, namespace, image_base):
@@ -541,29 +544,33 @@
         if not len(pods):
             print("None of the deployment containers match the given image")
             return
 
         please_wait()
         w = watch.Watch()
         cleanup_started = False
-        for event in w.stream(self.api.list_pod_for_all_namespaces, timeout_seconds=30):
+        for event in w.stream(self.api.list_pod_for_all_namespaces, timeout_seconds=self.pod_timeout):
             pod = event["object"]
             if pod.metadata.name not in pods:
                 continue
 
             if event["type"] == "DELETED":
                 del pods[pod.metadata.name]
             elif event["type"] != "ADDED" and not cleanup_started:
                 please_wait("Cleaning up")
                 cleanup_started = True
 
             if len(pods) == 0:
                 w.stop()
         if len(pods) > 0:
-            print("Time-out waiting for pods: {}".format(", ".join(pods.keys())))
+            pod_keys = ", ".join(pods.keys())
+            print(
+                f"Time-out ({self.pod_timeout}s) waiting for pods: {pod_keys}\n"
+                f"Increasing the pod reconfiguration timeout using --pod-timeout={self.pod_timeout+60} might help"
+            )
 
     def on_monitor_start(
         self, src_file_paths: list = None, destination_dir: str = None, supervisor: bool = True, **kwargs
     ):
         image_base, _ = self.split_destination(destination_dir)
         if supervisor:
             self.stabilize_deployments(image_base)
```

### Comparing `dfsync-0.3.7/dfsync/backends/kube_exec.py` & `dfsync-0.3.8/dfsync/backends/kube_exec.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,19 +3,23 @@
 import os.path
 import subprocess
 import sys
 
 from kubernetes import client, config
 
 
-def get_kubectl_exec_command(namespace, pod_name, container_name):
+def get_kubectl_exec_command(namespace, pod_name, container_name, kube_config=None, kube_context=None):
+    kubeconfig = [f"--kubeconfig={kube_config}"] if kube_config else []
+    context = [f"--context={kube_context}"] if kube_context else []
+
     ns = ["-n", "{}".format(namespace)] if namespace else []
     pod_name = ["{}".format(pod_name)]
     ctnr = ["-c", "{}".format(container_name)] if container_name else []
-    return ["kubectl", "exec", *pod_name, "-i", *ns, *ctnr, "--"]
+
+    return ["kubectl", *kubeconfig, *context, "exec", *pod_name, "-i", *ns, *ctnr, "--"]
 
 
 def get_container_command():
     clean_args = []
     for arg in sys.argv[1:]:
         if len(clean_args) == 0 and (not arg or len(arg.strip()) == 0):
             # remove any spaces or empty values from the beginning of sys.argv
@@ -29,14 +33,16 @@
     if not pod_name:
         raise ValueError("Expecting pod name in 'KUBEEXEC_POD' env. variable")
 
     kubectl_cmd = get_kubectl_exec_command(
         os.environ.get("KUBEEXEC_NAMESPACE"),
         pod_name,
         os.environ.get("KUBEEXEC_CONTAINER"),
+        os.environ.get("KUBEEXEC_KUBECONFIG"),
+        os.environ.get("KUBEEXEC_CONTEXT"),
     )
 
     container_cmd = get_container_command()
     cmd = [*kubectl_cmd, *container_cmd]
     subprocess.check_call(cmd)
     # print("MIHAI\n\n", file=sys.stderr)
     # print(subprocess.check_output(cmd), file=sys.stderr)
```

### Comparing `dfsync-0.3.7/dfsync/backends/rsync.py` & `dfsync-0.3.8/dfsync/backends/rsync.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.3.7/dfsync/exp.py` & `dfsync-0.3.8/dfsync/exp.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.3.7/dfsync/filters.py` & `dfsync-0.3.8/dfsync/filters.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.3.7/dfsync/monitor.py` & `dfsync-0.3.8/dfsync/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,16 @@
 
 
 @click.command()
 @click.argument("source", nargs=-1)
 @click.argument("destination", default="", nargs=1)
 @click.option("--supervisor/--no-supervisor", default=False, help="Try to install supervisor in container", type=bool)
 @click.option("--kube-host", default=None, help="Kubernetes api host server address/hostname", type=str)
-def main(source, destination, supervisor, kube_host):
+@click.option("--pod-timeout", default=30, help="Pod reconfiguration timeout (default is 30 seconds)", type=int)
+def main(source, destination, supervisor, kube_host, pod_timeout):
     """
     Watches a folder for changes and propagates all file changes to a destination.
 
     SOURCE is a path to the folder that dfsync will monitor for changes (or current dir if missing)
 
     DESTINATION is a destination path / psuedo-url
 
@@ -152,15 +153,17 @@
 
     paths = ["."] if len(source) == 0 else source
     destination_dir = destination
 
     backend, destination_dir = split_destination(destination_dir)
     click.echo("Destination, {}: '{}'".format(backend, destination_dir))
 
-    backend_options = dict(destination_dir=destination_dir, supervisor=supervisor, kube_host=kube_host)
+    backend_options = dict(
+        destination_dir=destination_dir, supervisor=supervisor, kube_host=kube_host, pod_timeout=pod_timeout
+    )
     backend_engine_factory = BACKENDS.get(backend)
     backend_engine = backend_engine_factory(**backend_options)
     if backend_engine is None:
         raise ValueError("Backend not found: {}".format(backend))
 
     handlers = []
     observer = Observer()
```

### Comparing `dfsync-0.3.7/dfsync/transactions.py` & `dfsync-0.3.8/dfsync/transactions.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.3.7/setup.py` & `dfsync-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'watchdog>=2.0.2,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['dfsync = dfsync.cli:dfsync']}
 
 setup_kwargs = {
     'name': 'dfsync',
-    'version': '0.3.7',
+    'version': '0.3.8',
     'description': '',
     'long_description': None,
     'author': 'Mihai Balint',
     'author_email': 'balint.mihai@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

