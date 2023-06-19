# Comparing `tmp/spaces-0.2.1.tar.gz` & `tmp/spaces-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaces-0.2.1.tar", max compression
+gzip compressed data, was "spaces-0.3.0.tar", max compression
```

## Comparing `spaces-0.2.1.tar` & `spaces-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.2.1/README.md
--rw-r--r--   0        0        0     1426 2023-06-01 10:22:15.138220 spaces-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      168 2023-05-23 16:06:07.578194 spaces-0.2.1/spaces/__init__.py
--rw-r--r--   0        0        0       61 2023-05-23 12:16:01.390521 spaces-0.2.1/spaces/config.py
--rw-r--r--   0        0        0      259 2023-05-30 12:29:38.149333 spaces-0.2.1/spaces/gpu/__init__.py
--rw-r--r--   0        0        0     1577 2023-05-31 17:56:04.987325 spaces-0.2.1/spaces/gpu/client.py
--rw-r--r--   0        0        0     1142 2023-06-01 10:17:22.403085 spaces-0.2.1/spaces/gpu/decorator.py
--rw-r--r--   0        0        0     3579 2023-05-30 13:33:47.192592 spaces-0.2.1/spaces/gpu/torch.py
--rw-r--r--   0        0        0     6528 2023-05-31 15:42:07.658085 spaces-0.2.1/spaces/gpu/wrappers.py
--rw-r--r--   0        0        0     1147 2023-06-01 10:07:38.324798 spaces-0.2.1/spaces/gradio.py
--rw-r--r--   0        0        0     1386 2023-05-30 13:53:53.832283 spaces-0.2.1/spaces/utils.py
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 spaces-0.2.1/setup.py
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 spaces-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.3.0/README.md
+-rw-r--r--   0        0        0     1490 2023-06-19 14:28:05.760905 spaces-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-23 16:06:07.578194 spaces-0.3.0/spaces/__init__.py
+-rw-r--r--   0        0        0      453 2023-06-19 14:01:43.384427 spaces-0.3.0/spaces/config.py
+-rw-r--r--   0        0        0      259 2023-05-30 12:29:38.149333 spaces-0.3.0/spaces/gpu/__init__.py
+-rw-r--r--   0        0        0     1589 2023-06-19 13:46:27.461593 spaces-0.3.0/spaces/gpu/client.py
+-rw-r--r--   0        0        0      662 2023-06-19 13:47:01.122285 spaces-0.3.0/spaces/gpu/decorator.py
+-rw-r--r--   0        0        0     3555 2023-06-02 18:22:00.557437 spaces-0.3.0/spaces/gpu/torch.py
+-rw-r--r--   0        0        0     6753 2023-06-02 18:54:45.252087 spaces-0.3.0/spaces/gpu/wrappers.py
+-rw-r--r--   0        0        0      690 2023-06-01 15:35:22.446266 spaces-0.3.0/spaces/gradio.py
+-rw-r--r--   0        0        0     1332 2023-06-19 14:10:55.323758 spaces-0.3.0/spaces/utils.py
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 spaces-0.3.0/setup.py
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 spaces-0.3.0/PKG-INFO
```

### Comparing `spaces-0.2.1/pyproject.toml` & `spaces-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spaces"
-version = "0.2.1"
+version = "0.3.0"
 description = "Utilities for Hugging Face Spaces"
 authors = ["Charles Bensimon <charles@huggingface.co>"]
 readme = "README.md"
 homepage = "https://huggingface.co"
 repository = "https://github.com/huggingface/huggingface_hub"
 license = "Apache-2.0"
 
@@ -47,19 +47,20 @@
     "^\\s*if TYPE_CHECKING:\\s*$",
     "^\\s*\\.\\.\\.\\s*$",
 ]
 
 [tool.poe.tasks.test]
 shell = """set -e
     pyright
-    coverage run -m pytest
+    coverage run -m pytest tests/cpu
+    coverage run -m pytest tests/gpu
     coverage combine -q
+    coverage xml  || true
+    coverage html || true
     coverage report
-    coverage xml
-    coverage html
 """
 
 [tool.pyright]
 include = ["spaces", "tests"]
 pythonVersion = "3.9"
 
 [build-system]
```

### Comparing `spaces-0.2.1/spaces/gpu/client.py` & `spaces-0.3.0/spaces/gpu/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """
 """
 
-import os
 from http import HTTPStatus
 
 import requests
 from pydantic import BaseModel
 
 from .. import utils
+from ..config import Config
 
 
-NODE_IP = os.environ['NODE_IP'] # Fail if not defined
-BASE_URL = f"http://{NODE_IP}:8000"
 CGROUP_PATH = utils.self_cgroup_device_path()
 
 
 class ScheduleParams(BaseModel):
     cgroupPath: str
 
 class ScheduleResponse(BaseModel):
@@ -24,17 +22,21 @@
 
 class ReleaseParams(BaseModel):
     cgroupPath: str
     nvidiaIndex: int
     fail: bool
 
 
+def base_url() -> str:
+    assert Config.zero_device_api_url is not None
+    return Config.zero_device_api_url
+
+
 def post(path: str, params: BaseModel) -> requests.Response:
-    print(f'{params.dict()=}')
-    return requests.post(BASE_URL + path, params=params.dict())
+    return requests.post(base_url() + path, params=params.dict())
 
 
 def schedule() -> ScheduleResponse:
 
     res = post('/schedule', params=ScheduleParams(
         cgroupPath=CGROUP_PATH,
     ))
```

### Comparing `spaces-0.2.1/spaces/gpu/torch.py` & `spaces-0.3.0/spaces/gpu/torch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 """
 # pyright: reportPrivateImportUsage=false
 
 from __future__ import annotations
 
 import multiprocessing
+import os
 from concurrent.futures import ProcessPoolExecutor
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     import torch as Torch
 
 try:
@@ -72,26 +73,26 @@
     def _unpatch():
         torch.Tensor.to         = _tensor_to
         torch.Tensor.cuda       = _tensor_cuda
         torch._C._cuda_init     = _cuda_init
         torch.cuda.is_available = _cuda_available
 
     def _move(nvidia_index: int):
+        os.environ['CUDA_VISIBLE_DEVICES'] = str(nvidia_index)
         for op in to_ops:
             tensor, parsed_args = op
-            device, dtype, non_blocking, memory_format = parsed_args
-            device = torch.device(device.type, index=nvidia_index)
+            _, dtype, _, memory_format = parsed_args
             tensor.data = _tensor_to(tensor,
-                device=device,
+                device='cuda',
                 dtype=dtype,
                 memory_format=memory_format,
             ) # type: ignore
         for op in cuda_ops:
             tensor = op
-            tensor.data = _tensor_cuda(tensor, nvidia_index)
+            tensor.data = _tensor_cuda(tensor)
 
     def _is_in_bad_fork():
         with ProcessPoolExecutor(mp_context=multiprocessing.get_context('fork')) as e:
             f = e.submit(torch.cuda._is_in_bad_fork)
             return f.result()
 
     def _disable_cuda_intercept():
```

### Comparing `spaces-0.2.1/spaces/utils.py` & `spaces-0.3.0/spaces/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,33 +10,31 @@
 from typing import TypeVar
 
 from .config import Config
 
 
 T = TypeVar('T')
 
+CallableT = TypeVar("CallableT", bound=Callable)
+
 
 def is_zero_gpu() -> bool:
-    return str2bool(os.getenv(Config.zero_gpu_env, ""))
+    return Config.zero_gpu
 
 
 def self_cgroup_device_path() -> str:
     cgroup_content = Path('/proc/self/cgroup').read_text()
     for line in cgroup_content.strip().split('\n'):
         contents = line.split(':devices:')
         if len(contents) != 2:
             continue # pragma: no cover
         return contents[1]
     raise Exception # pragma: no cover
 
 
-def str2bool(v: str) -> bool:
-    return v.lower() in ("1", "t", "true")
-
-
 class SimpleQueue(_SimpleQueue[T]):
     def __init__(self, *args):
         super().__init__(*args, ctx=multiprocessing.get_context('fork'))
     def put(self, element: T):
         try:
             super().put(element)
         except PicklingError:
```

### Comparing `spaces-0.2.1/setup.py` & `spaces-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['psutil>=5.9.5,<6.0.0',
  'pydantic>=1.10.8,<2.0.0',
  'requests>=2.29.0,<3.0.0',
  'typing-extensions>=4.5.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'spaces',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': 'Utilities for Hugging Face Spaces',
     'long_description': '# Hugging Face Spaces\n\n## Installation\n\n`pip install spaces`\n',
     'author': 'Charles Bensimon',
     'author_email': 'charles@huggingface.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://huggingface.co',
```

### Comparing `spaces-0.2.1/PKG-INFO` & `spaces-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spaces
-Version: 0.2.1
+Version: 0.3.0
 Summary: Utilities for Hugging Face Spaces
 Home-page: https://huggingface.co
 License: Apache-2.0
 Author: Charles Bensimon
 Author-email: charles@huggingface.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

