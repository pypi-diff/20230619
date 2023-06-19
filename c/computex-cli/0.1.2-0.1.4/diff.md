# Comparing `tmp/computex_cli-0.1.2.tar.gz` & `tmp/computex_cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computex_cli-0.1.2.tar", max compression
+gzip compressed data, was "computex_cli-0.1.4.tar", max compression
```

## Comparing `computex_cli-0.1.2.tar` & `computex_cli-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      613 2023-06-13 21:08:54.631293 computex_cli-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-12 13:32:24.984013 computex_cli-0.1.2/cxcli/__init__.py
--rw-r--r--   0        0        0     6085 2023-06-14 16:12:11.890803 computex_cli-0.1.2/cxcli/cli.py
--rw-r--r--   0        0        0      911 2023-06-13 21:08:54.632830 computex_cli-0.1.2/cxcli/config.py
--rw-r--r--   0        0        0      161 2023-06-13 21:08:54.633286 computex_cli-0.1.2/cxcli/exc.py
--rw-r--r--   0        0        0        0 2023-06-13 21:08:54.633381 computex_cli-0.1.2/cxcli/services/__init__.py
--rw-r--r--   0        0        0      950 2023-06-13 21:08:54.634140 computex_cli-0.1.2/cxcli/services/auth.py
--rw-r--r--   0        0        0     1485 2023-06-13 21:08:54.634576 computex_cli-0.1.2/cxcli/services/deployments.py
--rw-r--r--   0        0        0     1912 2023-06-13 21:08:54.635101 computex_cli-0.1.2/cxcli/services/service.py
--rw-r--r--   0        0        0     1236 2023-06-13 21:08:54.635947 computex_cli-0.1.2/cxcli/services/users.py
--rw-r--r--   0        0        0      727 2023-06-14 16:12:11.880449 computex_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 computex_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      613 2023-06-19 17:17:45.415196 computex_cli-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 18:28:28.160718 computex_cli-0.1.4/cxcli/__init__.py
+-rw-r--r--   0        0        0     6522 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/cli.py
+-rw-r--r--   0        0        0      911 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/config.py
+-rw-r--r--   0        0        0      161 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/exc.py
+-rw-r--r--   0        0        0        0 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/services/__init__.py
+-rw-r--r--   0        0        0      950 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/services/auth.py
+-rw-r--r--   0        0        0     2075 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/services/deployments.py
+-rw-r--r--   0        0        0     1912 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/services/service.py
+-rw-r--r--   0        0        0     1236 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/services/users.py
+-rw-r--r--   0        0        0      727 2023-06-19 17:18:00.035243 computex_cli-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 computex_cli-0.1.4/PKG-INFO
```

### Comparing `computex_cli-0.1.2/README.md` & `computex_cli-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.2/cxcli/cli.py` & `computex_cli-0.1.4/cxcli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -107,45 +107,47 @@
     update_core_api_credentials(
         login_response.access_token, login_response.refresh_token
     )
     click.echo("Successfully logged in. Welcome to CX.")
 
 
 @cli.command()
-@click.option("--app-name", help="Your app's name.")
+@click.option("--app", help="Your app's name.")
 @click.option(
-    "--container-image", help="A container image name that has been pushed to ComputeX."
+    "--image", help="A container image name that has been pushed to ComputeX."
 )
 @click.option("--num-cpu-cores", default=4, help="Number of CPU cores.")
 @click.option("--num-gpu", default=1, help="Number of GPUs.")
 @click.option(
-    "--gpu-sku", default="A40", help="The type of GPU you'd like to use."
+    "--gpu", default="A40", help="The type of GPU you'd like to use."
 )  # TODO: Add listing of SKUs
 # @click.option(
-#     "--cpu-sku", default="intel_xeon_v3", help="The type of CPU you'd like to use."
+#     "--cpu", default="intel_xeon_v3", help="The type of CPU you'd like to use."
 # )
 @click.option("--memory", default=4, help="Memory in GB to allocate.")
 @click.option("--replicas", default=1, help="Number of replicas to use.")
 @refresh_credentials
 def deploy(
-    app_name,
-    container_image,
+    app,
+    image,
     num_cpu_cores,
     num_gpu,
-    gpu_sku,
-    # cpu_sku,
+    gpu,
+    # cpu,
     memory,
     replicas,
 ):
+    # TODO: Verify that image exists before deployment.
+    r = UserServiceV1().get_registry_credentials()
     r = DeployRequest(
-        app_name=app_name,
-        container_image=container_image,
+        app_name=app,
+        container_image=f"{r.registry_host}/{r.registry_namespace}/{image}",
         num_cpu_cores=num_cpu_cores,
         num_gpu=num_gpu,
-        gpu_sku=gpu_sku,
+        gpu=gpu,
         # cpu_sku=cpu_sku,
         memory=memory,
         replicas=replicas,
     )
     DeploymentServiceV1().deploy(r)
     click.echo("Your app has successfully deployed.")
 
@@ -154,18 +156,18 @@
 @refresh_credentials
 def list_deployments():
     deployments = DeploymentServiceV1().list()
     click.echo(json.dumps(deployments.dict(), indent=4))
 
 
 @cli.command()
-@click.option("--app-name", help="Your app's name.")
+@click.option("--app", help="Your app's name.")
 @refresh_credentials
-def delete_deployment(app_name):
-    r = DeploymentServiceV1().delete(app_name)
+def delete_deployment(app):
+    r = DeploymentServiceV1().delete(app)
     click.echo(json.dumps(r.dict(), indent=4))
 
 
 @cli.command()
 @click.argument("image")
 @refresh_credentials
 def push(image):
@@ -176,9 +178,26 @@
         password=r.registry_password,
         registry=r.registry_host,
     )
     client.images.tag(image, f"{r.registry_host}/{r.registry_namespace}/{image}")
     client.images.push(f"{r.registry_host}/{r.registry_namespace}/{image}")
 
 
+@cli.command()
+@click.option("--app")
+@refresh_credentials
+def logs(app):
+    r = DeploymentServiceV1().logs(app)
+    click.echo(json.dumps(r.json(), indent=4))
+
+
+@cli.command()
+@click.option("--app")
+@click.option("--data")
+@refresh_credentials
+def predict(app, data):
+    r = DeploymentServiceV1().predict(app, data)
+    click.echo(json.dumps(r.dict(), indent=4))
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `computex_cli-0.1.2/cxcli/config.py` & `computex_cli-0.1.4/cxcli/config.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.2/cxcli/services/auth.py` & `computex_cli-0.1.4/cxcli/services/auth.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.2/cxcli/services/deployments.py` & `computex_cli-0.1.4/cxcli/services/deployments.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 class DeployRequest(BaseModel):
     app_name: str
     container_image: str
     num_cpu_cores: int
     num_gpu: int
     # TODO: Share SKU enums from main repo.
-    gpu_sku: str
-    # cpu_sku: str
+    gpu: str
+    # cpu: str
     memory: int
     replicas: int
 
 
 class DeployResponse(BaseModel):
     app_name: str
 
@@ -26,14 +26,22 @@
     status: dict
 
 
 class ListDeploymentsResponse(BaseModel):
     deployments: List[str]
 
 
+class LogsResponse(BaseModel):
+    logs: dict
+
+
+class PredictResponse(BaseModel):
+    result: dict
+
+
 class DeploymentServiceV1(CoreApiService):
     base_path: str = "/api/v1/deployments"
 
     def deploy(self, deploy_request: DeployRequest) -> DeployResponse:
         r = self._post("/deploy", json=deploy_request.dict())
         # TODO: Add better status checks and failed login reporting.
         r.raise_for_status()
@@ -49,7 +57,20 @@
 
     def delete(self, app_name: str):
         r = self._delete(f"/{app_name}")
         # TODO: Add better status checks and failed login reporting.
         r.raise_for_status()
         j = r.json()
         return DeleteResponse(status=j["status"])
+
+    def logs(self, app_name: str):
+        r = self._get(f"/{app_name}/logs")
+        # TODO: Add better status checks and failed login reporting.
+        r.raise_for_status()
+        j = r.json()
+        return LogsResponse(logs=j["logs"])
+
+    def predict(self, app_name: str, data: dict):
+        r = self._post(f"/{app_name}/predict", json=data)
+        # TODO: Add better status checks and failed login reporting.
+        r.raise_for_status()
+        return PredictResponse(result=r.json())
```

### Comparing `computex_cli-0.1.2/cxcli/services/service.py` & `computex_cli-0.1.4/cxcli/services/service.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.2/cxcli/services/users.py` & `computex_cli-0.1.4/cxcli/services/users.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.2/pyproject.toml` & `computex_cli-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "computex-cli"
-version = "0.1.2"
+version = "0.1.4"
 description = "ComputeX CLI tool"
 authors = ["Abate De Mey <abate@computex.ai>"]
 readme = "README.md"
 packages = [{include = "cxcli"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `computex_cli-0.1.2/PKG-INFO` & `computex_cli-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computex-cli
-Version: 0.1.2
+Version: 0.1.4
 Summary: ComputeX CLI tool
 Author: Abate De Mey
 Author-email: abate@computex.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

