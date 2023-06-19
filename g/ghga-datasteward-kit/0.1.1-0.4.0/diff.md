# Comparing `tmp/ghga_datasteward_kit-0.1.1.tar.gz` & `tmp/ghga_datasteward_kit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_datasteward_kit-0.1.1.tar", last modified: Fri Jun  9 09:18:06 2023, max compression
+gzip compressed data, was "ghga_datasteward_kit-0.4.0.tar", last modified: Mon Jun 19 13:53:03 2023, max compression
```

## Comparing `ghga_datasteward_kit-0.1.1.tar` & `ghga_datasteward_kit-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:18:06.888794 ghga_datasteward_kit-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-09 09:18:06.888794 ghga_datasteward_kit-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:18:06.888794 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6557 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/batch_s3_upload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3301 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/catalog_accession_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23425 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/s3_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:18:06.888794 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-09 09:18:06.000000 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-09 09:18:06.000000 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:18:06.000000 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-09 09:18:06.000000 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:18:06.000000 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-09 09:18:06.000000 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-09 09:18:06.000000 ghga_datasteward_kit-0.1.1/ghga_datasteward_kit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-09 09:18:06.888794 ghga_datasteward_kit-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:18:06.888794 ghga_datasteward_kit-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:18:06.888794 ghga_datasteward_kit-0.1.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/tests/fixtures/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/tests/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/tests/test_s3_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-09 09:17:53.000000 ghga_datasteward_kit-0.1.1/tests/test_size_adjustment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:03.634051 ghga_datasteward_kit-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-19 13:53:03.634051 ghga_datasteward_kit-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:03.630051 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6589 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/batch_s3_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3327 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/catalog_accession_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:03.634051 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/cli/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/cli/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23226 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/s3_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:03.630051 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-19 13:53:03.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-19 13:53:03.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:53:03.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-19 13:53:03.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:53:03.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-19 13:53:03.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 13:53:03.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-19 13:53:03.638051 ghga_datasteward_kit-0.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:03.634051 ghga_datasteward_kit-0.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:03.634051 ghga_datasteward_kit-0.4.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/tests/fixtures/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/tests/fixtures/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/tests/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/tests/test_s3_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/tests/test_size_adjustment.py
```

### Comparing `ghga_datasteward_kit-0.1.1/LICENSE` & `ghga_datasteward_kit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.1.1/PKG-INFO` & `ghga_datasteward_kit-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_datasteward_kit
-Version: 0.1.1
+Version: 0.4.0
 Summary: GHGA Data Steward Kit - A utils package for GHGA data stewards.
 Home-page: https://github.com/ghga-de/ghga-datasteward-kit
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_datasteward_kit-0.1.1/README.md` & `ghga_datasteward_kit-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/__init__.py` & `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A utils package for GHGA data stewards."""
 
-__version__ = "0.1.1"
+__version__ = "0.4.0"
```

### Comparing `ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/__main__.py` & `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/batch_s3_upload.py` & `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/batch_s3_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from copy import copy
 from pathlib import Path
 from time import sleep
 from typing import Optional
 
 from pydantic import BaseModel
 
-from ghga_datasteward_kit.s3_upload import load_config_yaml
+from ghga_datasteward_kit.s3_upload import Config, load_config_yaml
 
 HERE = Path(__file__).parent
 
 
 class FileMetadata(BaseModel):
     """Container for storing metadata on files that shall be uploaded."""
 
@@ -191,15 +191,15 @@
     dry_run: bool,
 ):
     """
     Custom script to encrypt data using Crypt4GH and directly uploading it to S3
     objectstorage.
     """
 
-    config = load_config_yaml(config_path)
+    config = load_config_yaml(path=config_path, config_cls=Config)
     files = load_file_metadata(file_overview_tsv=file_overview_tsv)
 
     handle_file_uploads(
         files=files,
         output_dir=config.output_dir,
         config_path=config_path,
         parallel_processes=parallel_processes,
```

### Comparing `ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/catalog_accession_generator.py` & `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/catalog_accession_generator.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # limitations under the License.
 
 """Generate Accessions to be used in the Metadata Catalog."""
 
 
 from pathlib import Path
 
-from metldata.accession_registry.accession_handler import AccessionHandler
+from metldata.accession_registry.accession_registry import AccessionRegistry
 from metldata.accession_registry.accession_store import AccessionStore
 from metldata.accession_registry.config import Config
 
 BASE_PREFIX = "GHGAMC"
 
 RESOURCE_PREFIXES = {
     "file": "F",
@@ -41,29 +41,29 @@
     "individual": "I",
 }
 
 SUFFIX_LENGTH = 14
 
 
 def generate_accessions(
-    *, resource_type: str, number: int, accession_handler: AccessionHandler
+    *, resource_type: str, number: int, accession_registry: AccessionRegistry
 ) -> list[str]:
     """Generate Accessions to be used in the Metadata Catalog.
 
     Args:
         resource_type (str): The resource type for which to generate accessions.
         number (int): The number of accessions to generate.
-        accession_handler (AccessionHandler): The accession handler to use.
+        accession_registry (AccessionRegistry): The accession registry to use.
 
     Returns:
         list[str]: The generated accessions.
     """
 
     accessions = [
-        accession_handler.get_accession(resource_type=resource_type)
+        accession_registry.get_accession(resource_type=resource_type)
         for _ in range(number)
     ]
     return accessions
 
 
 def get_config(*, store_path: Path) -> Config:
     """Get the config."""
@@ -96,14 +96,16 @@
         raise ValueError(
             f"Unknown resource type '{resource_type}'. Please choose one of: "
             f"{list(RESOURCE_PREFIXES.keys())}"
         )
 
     config = get_config(store_path=store_path)
     accession_store = AccessionStore(config=config)
-    accession_handler = AccessionHandler(config=config, accession_store=accession_store)
+    accession_registry = AccessionRegistry(
+        config=config, accession_store=accession_store
+    )
 
     return generate_accessions(
         resource_type=resource_type,
         number=number,
-        accession_handler=accession_handler,
+        accession_registry=accession_registry,
     )
```

### Comparing `ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/config.py` & `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/cli/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,12 +9,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Collection of all config classes."""
+"""The command line interface of the package."""
 
-from ghga_datasteward_kit.s3_upload import Config as S3UploadConfig
-
-CONFIG_CLASSES = {"s3_upload": S3UploadConfig}
+from .main import cli  # noqa: F401
```

### Comparing `ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/main.py` & `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/main.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.1.1/ghga_datasteward_kit/s3_upload.py` & `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/s3_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,21 +36,22 @@
 from typing import Any, Generator
 from uuid import uuid4
 
 import crypt4gh.header  # type: ignore
 import crypt4gh.keys  # type: ignore
 import crypt4gh.lib  # type: ignore
 import requests  # type: ignore
-import yaml
 from ghga_connector.core.file_operations import read_file_parts
 from ghga_connector.core.session import RequestsSession
 from hexkit.providers.s3 import S3Config, S3ObjectStorage  # type: ignore
 from nacl.bindings import crypto_aead_chacha20poly1305_ietf_encrypt
 from pydantic import BaseSettings, Field, SecretStr, validator
 
+from ghga_datasteward_kit.utils import load_config_yaml
+
 
 def configure_session() -> requests.Session:
     """Configure session with exponential backoff retry"""
     RequestsSession.configure(6)
     return RequestsSession.session
 
 
@@ -587,22 +588,14 @@
 def check_output_path(output_path: Path):
     """Check if we accidentally try to overwrite an alread existing metadata file"""
     if output_path.exists():
         msg = f"Output file {output_path.resolve()} already exists and cannot be overwritten."
         handle_superficial_error(msg=msg)
 
 
-def load_config_yaml(path: Path) -> Config:
-    """Load config parameters from the specified YAML file."""
-
-    with open(path, "r", encoding="utf-8") as config_file:
-        config_dict = yaml.safe_load(config_file)
-    return Config(**config_dict)
-
-
 async def async_main(input_path: Path, alias: str, config: Config):
     """
     Run encryption, upload and validation.
     Prints metadata to <alias>.json in the specified output directory
     """
     if not input_path.exists():
         msg = f"No such file: {input_path.resolve()}"
@@ -650,9 +643,9 @@
 
 def main(input_path, alias: str, config_path: Path):
     """
     Custom script to encrypt data using Crypt4GH and directly uploading it to S3
     objectstorage.
     """
 
-    config = load_config_yaml(config_path)
+    config = load_config_yaml(config_path, Config)
     asyncio.run(async_main(input_path=input_path, alias=alias, config=config))
```

### Comparing `ghga_datasteward_kit-0.1.1/ghga_datasteward_kit.egg-info/PKG-INFO` & `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga-datasteward-kit
-Version: 0.1.1
+Version: 0.4.0
 Summary: GHGA Data Steward Kit - A utils package for GHGA data stewards.
 Home-page: https://github.com/ghga-de/ghga-datasteward-kit
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_datasteward_kit-0.1.1/ghga_datasteward_kit.egg-info/SOURCES.txt` & `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,23 +2,31 @@
 README.md
 setup.cfg
 setup.py
 ghga_datasteward_kit/__init__.py
 ghga_datasteward_kit/__main__.py
 ghga_datasteward_kit/batch_s3_upload.py
 ghga_datasteward_kit/catalog_accession_generator.py
-ghga_datasteward_kit/cli.py
 ghga_datasteward_kit/config.py
+ghga_datasteward_kit/loading.py
 ghga_datasteward_kit/main.py
+ghga_datasteward_kit/metadata.py
 ghga_datasteward_kit/s3_upload.py
+ghga_datasteward_kit/utils.py
 ghga_datasteward_kit.egg-info/PKG-INFO
 ghga_datasteward_kit.egg-info/SOURCES.txt
 ghga_datasteward_kit.egg-info/dependency_links.txt
 ghga_datasteward_kit.egg-info/entry_points.txt
 ghga_datasteward_kit.egg-info/not-zip-safe
 ghga_datasteward_kit.egg-info/requires.txt
 ghga_datasteward_kit.egg-info/top_level.txt
+ghga_datasteward_kit/cli/__init__.py
+ghga_datasteward_kit/cli/file.py
+ghga_datasteward_kit/cli/main.py
+ghga_datasteward_kit/cli/metadata.py
+tests/test_metadata.py
 tests/test_s3_upload.py
 tests/test_size_adjustment.py
 tests/fixtures/__init__.py
 tests/fixtures/config.py
+tests/fixtures/metadata.py
 tests/fixtures/utils.py
```

### Comparing `ghga_datasteward_kit-0.1.1/setup.cfg` & `ghga_datasteward_kit-0.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 	Topic :: Scientific/Engineering :: Bio-Informatics
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	hexkit[mongodb,s3]==0.9.2
+	hexkit[mongodb,s3]==0.10.0
 	httpx==0.23.3
-	ghga-connector==0.2.12
-	metldata==0.1.0
+	ghga-connector==0.3.3
+	metldata==0.2.3
 python_requires = >= 3.9
 
 [options.entry_points]
 console_scripts = 
 	ghga-datasteward-kit = ghga_datasteward_kit.__main__:run
 
 [options.extras_require]
```

### Comparing `ghga_datasteward_kit-0.1.1/setup.py` & `ghga_datasteward_kit-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.1.1/tests/fixtures/__init__.py` & `ghga_datasteward_kit-0.4.0/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.1.1/tests/fixtures/config.py` & `ghga_datasteward_kit-0.4.0/tests/fixtures/config.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.1.1/tests/fixtures/utils.py` & `ghga_datasteward_kit-0.4.0/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.1.1/tests/test_s3_upload.py` & `ghga_datasteward_kit-0.4.0/tests/test_s3_upload.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 """Testing the whole encryption, upload, validation flow"""
 
 import sys
 from pathlib import Path
 
 import pytest
-from ghga_service_chassis_lib.utils import big_temp_file  # type: ignore
+from ghga_service_commons.utils.temp_files import big_temp_file  # type: ignore
 from hexkit.providers.s3.testutils import (  # type: ignore
     config_from_localstack_container,
 )
 from pydantic import SecretStr
 from testcontainers.localstack import LocalStackContainer  # type: ignore
 
 from ghga_datasteward_kit.s3_upload import Config, async_main, objectstorage
```

### Comparing `ghga_datasteward_kit-0.1.1/tests/test_size_adjustment.py` & `ghga_datasteward_kit-0.4.0/tests/test_size_adjustment.py`

 * *Files identical despite different names*

