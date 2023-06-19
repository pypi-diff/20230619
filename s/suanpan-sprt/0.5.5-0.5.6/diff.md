# Comparing `tmp/suanpan-sprt-0.5.5.tar.gz` & `tmp/suanpan-sprt-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/suanpan-sprt-0.5.5.tar", last modified: Fri Jun 16 07:39:57 2023, max compression
+gzip compressed data, was "dist/suanpan-sprt-0.5.6.tar", last modified: Mon Jun 19 06:23:27 2023, max compression
```

## Comparing `suanpan-sprt-0.5.5.tar` & `suanpan-sprt-0.5.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-16 07:39:57.000000 suanpan-sprt-0.5.5/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-16 07:39:57.000000 suanpan-sprt-0.5.5/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.5/README.md
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-06-16 07:39:57.000000 suanpan-sprt-0.5.5/setup.cfg
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.5/setup.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-16 07:39:57.000000 suanpan-sprt-0.5.5/sprt/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-03-13 09:36:01.000000 suanpan-sprt-0.5.5/sprt/__init__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5072 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.5/sprt/__main__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.5/sprt/arguments.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1280 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.5/sprt/envs.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.5/sprt/exceptions.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4321 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.5/sprt/loader.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2069 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.5/sprt/log.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.5/sprt/master.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5000 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.5/sprt/server.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6456 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.5/sprt/storage.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3448 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.5/sprt/testing.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.5/sprt/utils.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-06-16 07:39:57.000000 suanpan-sprt-0.5.5/sprt/version.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-16 07:39:57.000000 suanpan-sprt-0.5.5/suanpan_sprt.egg-info/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-16 07:39:57.000000 suanpan-sprt-0.5.5/suanpan_sprt.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-06-16 07:39:57.000000 suanpan-sprt-0.5.5/suanpan_sprt.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-06-16 07:39:57.000000 suanpan-sprt-0.5.5/suanpan_sprt.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-06-16 07:39:57.000000 suanpan-sprt-0.5.5/suanpan_sprt.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-06-16 07:39:57.000000 suanpan-sprt-0.5.5/suanpan_sprt.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-06-16 07:39:57.000000 suanpan-sprt-0.5.5/suanpan_sprt.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.6/README.md
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/setup.cfg
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.6/setup.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/sprt/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-03-13 09:36:01.000000 suanpan-sprt-0.5.6/sprt/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5190 2023-06-19 06:23:26.000000 suanpan-sprt-0.5.6/sprt/__main__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.6/sprt/arguments.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1280 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.6/sprt/envs.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.6/sprt/exceptions.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4321 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.6/sprt/loader.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2069 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.6/sprt/log.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.6/sprt/master.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5229 2023-06-19 06:23:26.000000 suanpan-sprt-0.5.6/sprt/server.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6456 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.6/sprt/storage.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3448 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.6/sprt/testing.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.6/sprt/utils.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-06-19 06:23:26.000000 suanpan-sprt-0.5.6/sprt/version.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/suanpan_sprt.egg-info/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/suanpan_sprt.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/suanpan_sprt.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/suanpan_sprt.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/suanpan_sprt.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/suanpan_sprt.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/suanpan_sprt.egg-info/top_level.txt
```

### Comparing `suanpan-sprt-0.5.5/setup.py` & `suanpan-sprt-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.5/sprt/__main__.py` & `suanpan-sprt-0.5.6/sprt/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 
 
 @click.command()
 @click.option('-h', '--host', default='localhost', envvar='RT_HOST', help='Runtime host')
 @click.option('-p', '--port', default=9988, envvar='RT_PORT', help='Runtime port')
 @click.option('-l', '--log-level', default='debug', envvar='RT_LOG_LEVEL', help='runtime logging level')
 @click.option('-f', '--log-file', default='runtime.log', envvar='RT_LOG_FILE', help='runtime logging file')
+@click.option('--new-log', default=False, envvar='RT_NEW_LOG', help='component with new log')
 @click.option('-w', '--working-dir', default='.', envvar='RT_WORKING_DIR', help='working dir')
-def main(host, port, log_level: str, log_file: str, working_dir: str):
+def main(host, port, log_level: str, log_file: str, new_log: bool, working_dir: str):
     if log_level.upper() in ('CRITICAL', 'FATAL', 'ERROR', 'WARN', 'WARNING', 'INFO', 'DEBUG'):
         dictConfig({
             'version': 1,
             'root': {
                 'level': log_level.upper(),
                 'handlers': ['console']
             },
@@ -65,15 +66,15 @@
                     'propagate': False
                 }
             },
         })
 
     signal.signal(signal.SIGTERM, receive_signal)
     signal.signal(signal.SIGINT, receive_signal)
-    app = server.create_app(working_dir, log_file)
+    app = server.create_app(working_dir, log_file, new_log)
 
     config = Config()
     config.bind = [f'{host}:{port}']
     app.logger.info(f'python runtime running on {host}:{port}')
     asyncio.run(serve(app, config))
```

### Comparing `suanpan-sprt-0.5.5/sprt/arguments.py` & `suanpan-sprt-0.5.6/sprt/arguments.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.5/sprt/envs.py` & `suanpan-sprt-0.5.6/sprt/envs.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.5/sprt/loader.py` & `suanpan-sprt-0.5.6/sprt/loader.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.5/sprt/log.py` & `suanpan-sprt-0.5.6/sprt/log.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.5/sprt/master.py` & `suanpan-sprt-0.5.6/sprt/master.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.5/sprt/server.py` & `suanpan-sprt-0.5.6/sprt/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,25 +53,30 @@
     resource = acquire_resource(*args, **kwargs)
     try:
         yield resource
     finally:
         release_resource(resource)
 
 
-def create_app(working_dir='.', log_file=''):
+def create_app(working_dir='.', log_file='', new_log=False):
     log_path = pathlib.Path(log_file).parent
+    filename = pathlib.Path(log_file).name
+    logfile_prefix = filename.split('-')[0:2]
     app = Quart(__name__)
     QuartSchema(app)
 
     @app.post("/")
     @validate_request(FunctionParams)
     @validate_response(FunctionResponse)
     async def handle_post(data: FunctionParams) -> FunctionResponse:
         node_id = data.context.node_id
-        log_name = log_path / node_id
+        if new_log:
+            log_name = log_path / f'{logfile_prefix[0]}-{logfile_prefix[1]}-{node_id}'
+        else:
+            log_name = log_path / node_id
         if utils.should_log_rollover(str(log_name)):
             utils.do_log_rollover(str(log_name))
         with open(log_path / node_id, 'a', encoding='utf8') as f:
             with redirect_stdout(f), redirect_stderr(f), node_context(node_id):
                 function = None
                 try:
                     logging.debug(f'event: {data.context.args}')
```

### Comparing `suanpan-sprt-0.5.5/sprt/storage.py` & `suanpan-sprt-0.5.6/sprt/storage.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.5/sprt/testing.py` & `suanpan-sprt-0.5.6/sprt/testing.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.5/sprt/utils.py` & `suanpan-sprt-0.5.6/sprt/utils.py`

 * *Files identical despite different names*

