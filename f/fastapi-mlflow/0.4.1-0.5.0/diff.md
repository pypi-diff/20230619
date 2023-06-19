# Comparing `tmp/fastapi_mlflow-0.4.1.tar.gz` & `tmp/fastapi_mlflow-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mlflow-0.4.1.tar", max compression
+gzip compressed data, was "fastapi_mlflow-0.5.0.tar", max compression
```

## Comparing `fastapi_mlflow-0.4.1.tar` & `fastapi_mlflow-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11352 2022-08-11 12:06:12.040233 fastapi_mlflow-0.4.1/LICENSE
--rw-r--r--   0        0        0     2650 2023-01-06 15:26:32.995842 fastapi_mlflow-0.4.1/README.md
--rw-r--r--   0        0        0       22 2022-08-10 14:33:30.741155 fastapi_mlflow-0.4.1/fastapi_mlflow/__init__.py
--rw-r--r--   0        0        0     1475 2023-04-14 15:44:22.195832 fastapi_mlflow-0.4.1/fastapi_mlflow/_mlflow_types.py
--rw-r--r--   0        0        0     1032 2023-04-17 13:06:21.593287 fastapi_mlflow-0.4.1/fastapi_mlflow/applications.py
--rw-r--r--   0        0        0      513 2023-04-17 12:52:44.792281 fastapi_mlflow-0.4.1/fastapi_mlflow/exceptions.py
--rw-r--r--   0        0        0     3326 2023-04-17 12:55:59.122998 fastapi_mlflow-0.4.1/fastapi_mlflow/predictors.py
--rw-r--r--   0        0        0      788 2023-04-17 14:46:18.364081 fastapi_mlflow-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 fastapi_mlflow-0.4.1/setup.py
--rw-r--r--   0        0        0     3484 1970-01-01 00:00:00.000000 fastapi_mlflow-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11352 2022-08-11 12:06:12.040233 fastapi_mlflow-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2650 2023-01-06 15:26:32.995842 fastapi_mlflow-0.5.0/README.md
+-rw-r--r--   0        0        0       22 2022-08-10 14:33:30.741155 fastapi_mlflow-0.5.0/fastapi_mlflow/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-14 15:44:22.195832 fastapi_mlflow-0.5.0/fastapi_mlflow/_mlflow_types.py
+-rw-r--r--   0        0        0     1032 2023-04-17 13:06:21.593287 fastapi_mlflow-0.5.0/fastapi_mlflow/applications.py
+-rw-r--r--   0        0        0      513 2023-04-17 12:52:44.792281 fastapi_mlflow-0.5.0/fastapi_mlflow/exceptions.py
+-rw-r--r--   0        0        0     3326 2023-04-17 12:55:59.122998 fastapi_mlflow-0.5.0/fastapi_mlflow/predictors.py
+-rw-r--r--   0        0        0      785 2023-06-09 14:10:16.093872 fastapi_mlflow-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3512 1970-01-01 00:00:00.000000 fastapi_mlflow-0.5.0/setup.py
+-rw-r--r--   0        0        0     3492 1970-01-01 00:00:00.000000 fastapi_mlflow-0.5.0/PKG-INFO
```

### Comparing `fastapi_mlflow-0.4.1/LICENSE` & `fastapi_mlflow-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_mlflow-0.4.1/README.md` & `fastapi_mlflow-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_mlflow-0.4.1/fastapi_mlflow/_mlflow_types.py` & `fastapi_mlflow-0.5.0/fastapi_mlflow/_mlflow_types.py`

 * *Files identical despite different names*

### Comparing `fastapi_mlflow-0.4.1/fastapi_mlflow/applications.py` & `fastapi_mlflow-0.5.0/fastapi_mlflow/applications.py`

 * *Files identical despite different names*

### Comparing `fastapi_mlflow-0.4.1/fastapi_mlflow/exceptions.py` & `fastapi_mlflow-0.5.0/fastapi_mlflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_mlflow-0.4.1/fastapi_mlflow/predictors.py` & `fastapi_mlflow-0.5.0/fastapi_mlflow/predictors.py`

 * *Files identical despite different names*

### Comparing `fastapi_mlflow-0.4.1/pyproject.toml` & `fastapi_mlflow-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "fastapi-mlflow"
-version = "0.4.1"
+version = "0.5.0"
 description = "Deploy mlflow models as JSON APIs with minimal new code."
 authors = ["John Harrison <john.harrison@autotrader.co.uk>"]
 readme = "README.md"
 repository = "https://github.com/autotraderuk/fastapi-mlflow"
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-mlflow = "^1.23.0"
-pydantic = "^1.9.0"
-fastapi = ">=0.73.0"
+mlflow = "^2.0.1"
+pydantic = "^1.10.0"
+fastapi = "^0.96.0"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=22"
-fastapi = {extras = ["all"], version = "^0.88.0"}
+fastapi = {extras = ["all"], version = ">=0.96.0"}
 flake8-bugbear = "^22.1.11"
 isort = "^5.10.1"
 pytest = "^6.2.5"
 pandas = "^1.2.0"
 pandas-stubs = "^1.2.0"
 numpy = "^1.22.1"
-mypy = ">=0.931"
+mypy = "^1.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.mypy]
```

### Comparing `fastapi_mlflow-0.4.1/setup.py` & `fastapi_mlflow-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['fastapi_mlflow']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fastapi>=0.73.0', 'mlflow>=1.23.0,<2.0.0', 'pydantic>=1.9.0,<2.0.0']
+['fastapi>=0.96.0,<0.97.0', 'mlflow>=2.0.1,<3.0.0', 'pydantic>=1.10.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'fastapi-mlflow',
-    'version': '0.4.1',
+    'version': '0.5.0',
     'description': 'Deploy mlflow models as JSON APIs with minimal new code.',
     'long_description': '# fastapi mlflow\n\nDeploy [mlflow](https://www.mlflow.org/) models as JSON APIs using [FastAPI](https://fastapi.tiangolo.com) with minimal new code.\n\n## Installation\n\n```shell\npip install fastapi-mlflow\n```\n\nFor running the app in production, you will also need an ASGI server, such as [Uvicorn](https://www.uvicorn.org) or [Hypercorn](https://gitlab.com/pgjones/hypercorn).\n\n## Install on Apple Silicon (ARM / M1)\n\nIf you experience problems installing on a newer generation Apple silicon based device, [this solution from StackOverflow](https://stackoverflow.com/a/67586301) before retrying install has been found to help.\n\n```shell\nbrew install openblas gfortran\nexport OPENBLAS="$(brew --prefix openblas)"\n```\n\n## License\n\nCopyright © 2022-23 Auto Trader Group plc.\n\n[Apache-2.0](https://www.apache.org/licenses/LICENSE-2.0)\n\n## Examples\n\n### Simple\n\n#### Create\n\nCreate a file `main.py` containing:\n\n```python\nfrom fastapi_mlflow.applications import build_app\nfrom mlflow.pyfunc import load_model\n\nmodel = load_model("/Users/me/path/to/local/model")\napp = build_app(model)\n```\n\n#### Run\n\nRun the server with:\n\n```shell\nuvicorn main:app\n```\n\n#### Check\n\nOpen your browser at <http://127.0.0.1:8000/docs>\n\nYou should see the automatically generated docs for your model, and be able to test it out using the `Try it out` button in the UI.\n\n### Serve multiple models\n\nIt should be possible to host multiple models (assuming that they have compatible dependencies...) by leveraging [FastAPIs Sub Applications](https://fastapi.tiangolo.com/advanced/sub-applications/#sub-applications-mounts):\n\n```python\nfrom fastapi import FastAPI\nfrom fastapi_mlflow.applications import build_app\nfrom mlflow.pyfunc import load_model\n\napp = FastAPI()\n\nmodel1 = load_model("/Users/me/path/to/local/model1")\nmodel1_app = build_app(model1)\napp.mount("/model1", model1_app)\n\nmodel2 = load_model("/Users/me/path/to/local/model2")\nmodel2_app = build_app(model2)\napp.mount("/model2", model2_app)\n```\n\n[Run](#run) and [Check](#check) as above.\n\n### Custom routing\n\nIf you want more control over where and how the prediction end-point is mounted in your API, you can build the predictor function directly and use it as you need:\n\n```python\nfrom inspect import signature\n\nfrom fastapi import FastAPI\nfrom fastapi_mlflow.predictors import build_predictor\nfrom mlflow.pyfunc import load_model\n\nmodel = load_model("/Users/me/path/to/local/model")\npredictor = build_predictor(model)\napp = FastAPI()\napp.add_api_route(\n    "/classify",\n    predictor,\n    response_model=signature(predictor).return_annotation,\n    methods=["POST"],\n)\n```\n\n[Run](#run) and [Check](#check) as above.\n',
     'author': 'John Harrison',
     'author_email': 'john.harrison@autotrader.co.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/autotraderuk/fastapi-mlflow',
```

### Comparing `fastapi_mlflow-0.4.1/PKG-INFO` & `fastapi_mlflow-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: fastapi-mlflow
-Version: 0.4.1
+Version: 0.5.0
 Summary: Deploy mlflow models as JSON APIs with minimal new code.
 Home-page: https://github.com/autotraderuk/fastapi-mlflow
 License: Apache-2.0
 Author: John Harrison
 Author-email: john.harrison@autotrader.co.uk
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi (>=0.73.0)
-Requires-Dist: mlflow (>=1.23.0,<2.0.0)
-Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: fastapi (>=0.96.0,<0.97.0)
+Requires-Dist: mlflow (>=2.0.1,<3.0.0)
+Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://github.com/autotraderuk/fastapi-mlflow
 Description-Content-Type: text/markdown
 
 # fastapi mlflow
 
 Deploy [mlflow](https://www.mlflow.org/) models as JSON APIs using [FastAPI](https://fastapi.tiangolo.com) with minimal new code.
```

