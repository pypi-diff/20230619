# Comparing `tmp/stackdiac-0.0.1.dev29.tar.gz` & `tmp/stackdiac-0.0.1.dev30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackdiac-0.0.1.dev29.tar", max compression
+gzip compressed data, was "stackdiac-0.0.1.dev30.tar", max compression
```

## Comparing `stackdiac-0.0.1.dev29.tar` & `stackdiac-0.0.1.dev30.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1066 2023-06-13 16:32:22.736846 stackdiac-0.0.1.dev29/LICENSE
--rw-r--r--   0        0        0     1415 2023-06-13 16:32:22.736846 stackdiac-0.0.1.dev29/README.md
--rw-r--r--   0        0        0      616 2023-06-13 16:32:44.909069 stackdiac-0.0.1.dev29/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-13 16:32:22.736846 stackdiac-0.0.1.dev29/stackdiac/__init__.py
--rw-r--r--   0        0        0       23 2023-06-13 16:32:22.736846 stackdiac-0.0.1.dev29/stackdiac/api/__init__.py
--rw-r--r--   0        0        0     1179 2023-06-13 16:32:22.736846 stackdiac-0.0.1.dev29/stackdiac/api/server.py
--rw-r--r--   0        0        0     1800 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/cli/__init__.py
--rw-r--r--   0        0        0      729 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/cli/build.py
--rw-r--r--   0        0        0     1594 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/cli/create.py
--rw-r--r--   0        0        0      464 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/cli/ui.py
--rw-r--r--   0        0        0      381 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/models/__init__.py
--rw-r--r--   0        0        0     1145 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/models/backend.py
--rw-r--r--   0        0        0     2582 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/models/binary.py
--rw-r--r--   0        0        0    12716 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/models/cluster.py
--rw-r--r--   0        0        0     2769 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/models/config.py
--rw-r--r--   0        0        0     2325 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/models/operation.py
--rw-r--r--   0        0        0      161 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/models/provider.py
--rw-r--r--   0        0        0     5276 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/models/repo.py
--rw-r--r--   0        0        0      411 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/models/secret.py
--rw-r--r--   0        0        0     1716 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/models/spec.py
--rw-r--r--   0        0        0    12767 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/models/stack.py
--rw-r--r--   0        0        0      108 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/stackd/__init__.py
--rw-r--r--   0        0        0      193 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/stackd/filters.py
--rw-r--r--   0        0        0      297 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/stackd/sdmod.py
--rw-r--r--   0        0        0    11901 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/stackd/stackd.py
--rw-r--r--   0        0        0   164360 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/ui/4753c5ba57962b4d7bf8.woff
--rw-r--r--   0        0        0   121340 2023-06-13 16:32:22.740846 stackdiac-0.0.1.dev29/stackdiac/ui/6d63d0501e5ed7b79dab.woff2
--rw-r--r--   0        0        0  2216513 2023-06-13 16:32:22.756846 stackdiac-0.0.1.dev29/stackdiac/ui/bundle.js
--rw-r--r--   0        0        0     3087 2023-06-13 16:32:22.756846 stackdiac-0.0.1.dev29/stackdiac/ui/bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      415 2023-06-13 16:32:22.756846 stackdiac-0.0.1.dev29/stackdiac/ui/index.html
--rw-r--r--   0        0        0        0 2023-06-13 16:32:22.756846 stackdiac-0.0.1.dev29/stackdiac/views/__init__.py
--rw-r--r--   0        0        0      780 2023-06-13 16:32:22.756846 stackdiac-0.0.1.dev29/stackdiac/views/module.py
--rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 stackdiac-0.0.1.dev29/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/LICENSE
+-rw-r--r--   0        0        0     1415 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/README.md
+-rw-r--r--   0        0        0      616 2023-06-19 07:21:04.916380 stackdiac-0.0.1.dev30/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/api/__init__.py
+-rw-r--r--   0        0        0     1179 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/api/server.py
+-rw-r--r--   0        0        0     1789 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/cli/__init__.py
+-rw-r--r--   0        0        0      729 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/cli/build.py
+-rw-r--r--   0        0        0     1594 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/cli/create.py
+-rw-r--r--   0        0        0      464 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/cli/ui.py
+-rw-r--r--   0        0        0      381 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/__init__.py
+-rw-r--r--   0        0        0     1145 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/backend.py
+-rw-r--r--   0        0        0     2582 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/binary.py
+-rw-r--r--   0        0        0    12716 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/cluster.py
+-rw-r--r--   0        0        0     2769 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/config.py
+-rw-r--r--   0        0        0     2594 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/operation.py
+-rw-r--r--   0        0        0      161 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/provider.py
+-rw-r--r--   0        0        0     5276 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/repo.py
+-rw-r--r--   0        0        0      411 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/secret.py
+-rw-r--r--   0        0        0     1716 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/spec.py
+-rw-r--r--   0        0        0    13166 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/stack.py
+-rw-r--r--   0        0        0      108 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/stackd/__init__.py
+-rw-r--r--   0        0        0      193 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/stackd/filters.py
+-rw-r--r--   0        0        0      297 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/stackd/sdmod.py
+-rw-r--r--   0        0        0    11931 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/stackd/stackd.py
+-rw-r--r--   0        0        0   164360 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/ui/4753c5ba57962b4d7bf8.woff
+-rw-r--r--   0        0        0   121340 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/ui/6d63d0501e5ed7b79dab.woff2
+-rw-r--r--   0        0        0  2216513 2023-06-19 07:20:35.971693 stackdiac-0.0.1.dev30/stackdiac/ui/bundle.js
+-rw-r--r--   0        0        0     3087 2023-06-19 07:20:35.971693 stackdiac-0.0.1.dev30/stackdiac/ui/bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      415 2023-06-19 07:20:35.971693 stackdiac-0.0.1.dev30/stackdiac/ui/index.html
+-rw-r--r--   0        0        0        0 2023-06-19 07:20:35.971693 stackdiac-0.0.1.dev30/stackdiac/views/__init__.py
+-rw-r--r--   0        0        0      780 2023-06-19 07:20:35.971693 stackdiac-0.0.1.dev30/stackdiac/views/module.py
+-rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 stackdiac-0.0.1.dev30/PKG-INFO
```

### Comparing `stackdiac-0.0.1.dev29/LICENSE` & `stackdiac-0.0.1.dev30/LICENSE`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/README.md` & `stackdiac-0.0.1.dev30/README.md`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/pyproject.toml` & `stackdiac-0.0.1.dev30/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stackdiac"
-version = "0.0.1-dev29"
+version = "0.0.1-dev30"
 description = ""
 authors = ["sysr9 <38893296+sysr9@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `stackdiac-0.0.1.dev29/stackdiac/api/server.py` & `stackdiac-0.0.1.dev30/stackdiac/api/server.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/stackdiac/cli/__init__.py` & `stackdiac-0.0.1.dev30/stackdiac/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,12 +62,11 @@
     
 cli.add_command(tg)
 
 @click.command(context_settings={"ignore_unknown_options": True}, name="op")
 @click.option("-b", "--build", is_flag=True, help="deprecated, always building")
 @click.argument("target")
 def op(target, build:bool, **kwargs):
-    sd.configure()
-    sd.build()
+    sd.configure()    
     sd.run_operation(target=target, **kwargs)
 
 cli.add_command(op)
```

### Comparing `stackdiac-0.0.1.dev29/stackdiac/cli/build.py` & `stackdiac-0.0.1.dev30/stackdiac/cli/build.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/stackdiac/cli/create.py` & `stackdiac-0.0.1.dev30/stackdiac/cli/create.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/stackdiac/models/backend.py` & `stackdiac-0.0.1.dev30/stackdiac/models/backend.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/stackdiac/models/binary.py` & `stackdiac-0.0.1.dev30/stackdiac/models/binary.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/stackdiac/models/cluster.py` & `stackdiac-0.0.1.dev30/stackdiac/models/cluster.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/stackdiac/models/config.py` & `stackdiac-0.0.1.dev30/stackdiac/models/config.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/stackdiac/models/operation.py` & `stackdiac-0.0.1.dev30/stackdiac/models/operation.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,23 +21,26 @@
     modules: list[str]
     command: str | list[str] = "plan"
 
 class PipelineStep(BaseModel):
     module: str
     title: str | None = None
     command: str | list[str] = "apply"
+    vars: dict[str, Any] = {}
 
-    def run(self, sd, cluster, cluster_stack, **kwargs):
+    def run(self, sd, cluster, cluster_stack, stack, operation, **kwargs):
         if self.title is None:
             self.title = f"run {self.command} on {self.module}"
             
         if self.command is not list:
             self.command = self.command.split(" ")
         
-        
+        cluster_stack.build(cluster=cluster, sd=sd, extra_vars=self.vars,
+                                                    **kwargs)
+        logger.info(f"builded {self.title} step with extra vars {self.vars}")
         sd.terragrunt(target=cluster_stack.stack.modules[self.module].built_vars["build_path"], 
                       terragrunt_options=self.command, 
                       cluster=cluster, **kwargs)
         logger.info(f"finished running step <{self.title}>")
 
 
 class Operation(BaseModel):    
@@ -49,15 +52,15 @@
     
 
     def run(self, sd, target, cluster, cluster_stack, **kwargs):
         logger.info(f"{self} running {len(self.pipeline)} steps pipeline")
 
         for step in self.pipeline:
             logger.info(f"running step {step}")
-            step.run(sd, cluster, cluster_stack, **kwargs)
+            step.run(sd, cluster, cluster_stack, operation=self, **kwargs)
 
 
     def run_old(self, sd, target, cluster, stack, **kwargs):
         op = self.configurations[self.configuration]
         dest = os.path.join(sd.builddir, cluster.name, stack.name)
         args = ["run-all"]
         for module in op.modules:
```

### Comparing `stackdiac-0.0.1.dev29/stackdiac/models/repo.py` & `stackdiac-0.0.1.dev30/stackdiac/models/repo.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/stackdiac/models/spec.py` & `stackdiac-0.0.1.dev30/stackdiac/models/spec.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/stackdiac/models/stack.py` & `stackdiac-0.0.1.dev30/stackdiac/models/stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,20 @@
 
 class ModuleDependency(BaseModel):
     name: str
     path: str
     abspath: str
     module_name: str
     stack_name: str
+    alias: str | None = None
 
     @property
     def varname(self) -> str:
+        if self.alias:
+            return self.alias
         return f"{self.stack_name}_{self.module_name}".replace("-", "_")
 
 class ModuleSecretStatus(Enum):
     UNKNOWN = "unknown"
     NOT_EXISTS = "not_exists"
     EXISTS = "exists"
     VALID   = "valid"
@@ -77,15 +80,15 @@
     source: str | None = None
     src: str | None = None
     vars: dict[str, Any] = {}
     module_vars: dict[str, Any] = {}
     built_vars: dict[str, Any] = {}
     providers: list[str] = []
     provider_overrides: dict[str, Any] = {}
-    inputs: list[str] = []
+    inputs: Any = []
     deps: list[str] = []
     tf_state_key: str | None = None
     tf_state_bucket: str | None = None
     tf_state_bucket_region: str | None = None
     tf_backend: str = "s3"
     tf_backend_config: dict[str, Any] = {}
     backend: Backend | None = None
@@ -124,30 +127,39 @@
         vars_file = self.build_vars_file(sd, cluster_stack, cluster)
         if os.path.exists(vars_file):
             return yaml.load(open(vars_file), Loader=yaml.FullLoader)
         else:
             return {}
    
 
-    def build_deps(self, stack, module, cluster, deps:list[str], sd, **kwargs) -> list[ModuleDependency]:
-        for d in deps:
+    def build_deps(self, stack, module, cluster, deps, sd, **kwargs) -> list[ModuleDependency]:
+        if type(deps) is list:
+            _deps = { d: None for d in deps }
+        elif type(deps) is dict:
+            _deps = deps
+        else:
+            raise Exception(f"invalid deps type {type(deps)}")
+        
+        for d, alias in _deps.items():            
             parts = [x for x in d.split("/") if x]
             if len(parts) == 2:
                 stack_name, module_name = parts
             elif len(parts) == 1:
                 module_name = parts[0]
                 stack_name = stack.name
             else:
                 raise Exception(f"invalid module dep {d}")
+           
             yield ModuleDependency(
                 name=d,
                 path=d,
                 abspath=os.path.join(sd.builddir, cluster.name, stack_name, module_name),
                 module_name=module_name,
-                stack_name=stack_name
+                stack_name=stack_name,
+                alias=alias
             )
 
     @property
     def charts_root(self) -> str:
         from stackdiac.stackd import sd
         return os.path.join(sd.root, "charts")
 
@@ -210,15 +222,15 @@
         """
         return f"{os.path.dirname(self.abssrc)}//{os.path.basename(self.abssrc)}"
 
     def get_build_dir(self, cluster, stack):
         from stackdiac.stackd import sd
         return os.path.join(sd.root, "build", cluster.name, stack.name, self.name)
 
-    def build(self, cluster, cluster_stack, stack, sd, **kwargs):
+    def build(self, cluster, cluster_stack, stack, sd, extra_vars={}, **kwargs):
         #from stackdiac.stackd import sd
         path = sd.resolve_module_path(self.src)
         dest = self.get_build_dir(cluster, stack)
         os.makedirs(dest, exist_ok=True)
         _vars = {
             'build_path': dest,
             'module_path': path,
@@ -238,15 +250,16 @@
 
         for v in [
                 self.vars,
                 sd.conf.vars,
                 cluster.vars,
                 cluster_stack.vars,
                 cluster_stack.module_vars.get(self.name, {}),
-                self.module_vars
+                self.module_vars,
+                extra_vars
                 ]:
             always_merger.merge(_vars, deepcopy(v))
 
         self.built_vars = deepcopy(_vars)
 
         exclude_list = [
             "vault_address",
```

### Comparing `stackdiac-0.0.1.dev29/stackdiac/stackd/stackd.py` & `stackdiac-0.0.1.dev30/stackdiac/stackd/stackd.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,14 +305,16 @@
 
     def run_operation(self, target, **kwargs):
         """
         target is in form <cluster>/<stack>/<operation>
         running  self.terragrunt with configured module path
     
         """
+        self.build()
         cluster, stack, operation = target.split("/")
         self.clusters[cluster].stacks[stack].build(cluster=self.clusters[cluster], sd=self, **kwargs)
+        
         self.clusters[cluster].stacks[stack].stack.operations[operation].run(target=target, sd=self, 
             cluster=self.clusters[cluster],
             stack=self.clusters[cluster].stacks[stack],
             cluster_stack=self.clusters[cluster].stacks[stack], # < more logical name
             **kwargs)
```

### Comparing `stackdiac-0.0.1.dev29/stackdiac/ui/4753c5ba57962b4d7bf8.woff` & `stackdiac-0.0.1.dev30/stackdiac/ui/4753c5ba57962b4d7bf8.woff`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/stackdiac/ui/6d63d0501e5ed7b79dab.woff2` & `stackdiac-0.0.1.dev30/stackdiac/ui/6d63d0501e5ed7b79dab.woff2`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/stackdiac/ui/bundle.js` & `stackdiac-0.0.1.dev30/stackdiac/ui/bundle.js`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/stackdiac/ui/bundle.js.LICENSE.txt` & `stackdiac-0.0.1.dev30/stackdiac/ui/bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/stackdiac/views/module.py` & `stackdiac-0.0.1.dev30/stackdiac/views/module.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev29/PKG-INFO` & `stackdiac-0.0.1.dev30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackdiac
-Version: 0.0.1.dev29
+Version: 0.0.1.dev30
 Summary: 
 License: MIT
 Author: sysr9
 Author-email: 38893296+sysr9@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

