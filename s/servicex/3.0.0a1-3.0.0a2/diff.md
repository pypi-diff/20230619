# Comparing `tmp/servicex-3.0.0a1.tar.gz` & `tmp/servicex-3.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicex-3.0.0a1.tar", max compression
+gzip compressed data, was "servicex-3.0.0a2.tar", max compression
```

## Comparing `servicex-3.0.0a1.tar` & `servicex-3.0.0a2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1499 2023-06-16 21:24:27.546614 servicex-3.0.0a1/LICENSE
--rw-r--r--   0        0        0     2574 2023-06-16 21:24:27.546614 servicex-3.0.0a1/README.md
--rw-r--r--   0        0        0     1070 2023-06-16 21:25:15.907111 servicex-3.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     1535 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/__init__.py
--rw-r--r--   0        0        0       96 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/_version.py
--rw-r--r--   0        0        0     1535 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/app/__init__.py
--rw-r--r--   0        0        0     3157 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/app/cache.py
--rw-r--r--   0        0        0     1776 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/app/cli_options.py
--rw-r--r--   0        0        0     2643 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/app/main.py
--rw-r--r--   0        0        0     5414 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/app/transforms.py
--rw-r--r--   0        0        0     3362 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/configuration.py
--rw-r--r--   0        0        0    15385 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/dataset.py
--rw-r--r--   0        0        0     1984 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/dataset_group.py
--rw-r--r--   0        0        0     2700 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/dataset_identifier.py
--rw-r--r--   0        0        0     1535 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/func_adl/__init__.py
--rw-r--r--   0        0        0     9275 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/func_adl/func_adl_dataset.py
--rw-r--r--   0        0        0     4013 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/func_adl/util.py
--rw-r--r--   0        0        0     4184 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/minio_adpater.py
--rw-r--r--   0        0        0     4410 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/models.py
--rw-r--r--   0        0        0     3111 2023-06-16 21:24:27.550614 servicex-3.0.0a1/servicex_client/python_dataset.py
--rw-r--r--   0        0        0     4405 2023-06-16 21:24:27.550614 servicex-3.0.0a1/servicex_client/query_cache.py
--rw-r--r--   0        0        0     5374 2023-06-16 21:24:27.550614 servicex-3.0.0a1/servicex_client/servicex_adapter.py
--rw-r--r--   0        0        0     5031 2023-06-16 21:24:27.550614 servicex-3.0.0a1/servicex_client/servicex_client.py
--rw-r--r--   0        0        0     1692 2023-06-16 21:24:27.550614 servicex-3.0.0a1/servicex_client/types.py
--rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 servicex-3.0.0a1/setup.py
--rw-r--r--   0        0        0     3648 1970-01-01 00:00:00.000000 servicex-3.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1499 2023-06-19 14:46:52.495569 servicex-3.0.0a2/LICENSE
+-rw-r--r--   0        0        0     4890 2023-06-19 14:46:52.495569 servicex-3.0.0a2/README.md
+-rw-r--r--   0        0        0     1187 2023-06-19 14:47:30.391655 servicex-3.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1535 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/__init__.py
+-rw-r--r--   0        0        0       96 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/_version.py
+-rw-r--r--   0        0        0     1535 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/app/__init__.py
+-rw-r--r--   0        0        0     3157 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/app/cache.py
+-rw-r--r--   0        0        0     1776 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/app/cli_options.py
+-rw-r--r--   0        0        0     2643 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/app/main.py
+-rw-r--r--   0        0        0     5414 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/app/transforms.py
+-rw-r--r--   0        0        0     3721 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/configuration.py
+-rw-r--r--   0        0        0    17500 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/dataset.py
+-rw-r--r--   0        0        0     2674 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/dataset_group.py
+-rw-r--r--   0        0        0     3410 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/dataset_identifier.py
+-rw-r--r--   0        0        0     1535 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/func_adl/__init__.py
+-rw-r--r--   0        0        0     4013 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/func_adl/util.py
+-rw-r--r--   0        0        0    11894 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/func_adl_dataset.py
+-rw-r--r--   0        0        0     4184 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/minio_adpater.py
+-rw-r--r--   0        0        0     5130 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/models.py
+-rw-r--r--   0        0        0     3111 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/python_dataset.py
+-rw-r--r--   0        0        0     4405 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/query_cache.py
+-rw-r--r--   0        0        0     5424 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/servicex_adapter.py
+-rw-r--r--   0        0        0     8042 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/servicex_client.py
+-rw-r--r--   0        0        0     1692 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/types.py
+-rw-r--r--   0        0        0     6278 1970-01-01 00:00:00.000000 servicex-3.0.0a2/setup.py
+-rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 servicex-3.0.0a2/PKG-INFO
```

### Comparing `servicex-3.0.0a1/LICENSE` & `servicex-3.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a1/pyproject.toml` & `servicex-3.0.0a2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servicex"
-version = "3.0.0-alpha.1"
+version = "3.0.0-alpha.2"
 description = ""
 authors = ["Ben Galewsky <bengal1@illinois.edu>", "Gordon Watts <gwatts@uw.edu>"]
 readme = "README.md"
 packages = [{include = "servicex_client"}]
 
 [tool.poetry.scripts]
 servicex = "servicex_client.app.main:app"
@@ -23,28 +23,30 @@
 PyYAML = "^6.0"
 types-PyYAML = "^6.0"
 
 pandas = {version = "^2.0.2", optional = true}
 pyarrow = {version = "^12.0.0", optional = true}
 fastparquet = {version="^2023.4.0", optional = true}
 
+sphinx = {version="^7.0.1", optional = true}
+furo = {version="^2023.5.20", optional = true}
+
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
 flake8 = "^5.0.4"
 mypy = "^0.981"
 pytest-asyncio ="^0.21.0"
 asyncmock = "^0.4.2"
 
 
 
 [tool.poetry.extras]
 pandas = ["pandas", "pyarrow", "fastparquet"]
-
-
+docs = ["sphinx", "furo"]
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `servicex-3.0.0a1/servicex_client/__init__.py` & `servicex-3.0.0a2/servicex_client/__init__.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a1/servicex_client/app/__init__.py` & `servicex-3.0.0a2/servicex_client/app/__init__.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a1/servicex_client/app/cache.py` & `servicex-3.0.0a2/servicex_client/app/cache.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a1/servicex_client/app/cli_options.py` & `servicex-3.0.0a2/servicex_client/app/cli_options.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a1/servicex_client/app/main.py` & `servicex-3.0.0a2/servicex_client/app/main.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a1/servicex_client/app/transforms.py` & `servicex-3.0.0a2/servicex_client/app/transforms.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a1/servicex_client/configuration.py` & `servicex-3.0.0a2/servicex_client/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,14 +50,22 @@
         allow_population_by_field_name = True
 
     def endpoint_dict(self) -> Dict[str, Endpoint]:
         return {endpoint.name: endpoint for endpoint in self.api_endpoints}
 
     @classmethod
     def read(cls, config_path: Optional[str] = None):
+        r"""
+        Read configuration from .servicex file.
+
+        :param config_path: If provided, use this as the path to the .servicex file.
+                            Otherwise, search, starting from the current working directory
+                            and look in enclosing directories
+        :return: Populated configuraton object
+        """
         if config_path:
             yaml_config = cls._add_from_path(Path(config_path), walk_up_tree=False)
         else:
             yaml_config = cls._add_from_path(walk_up_tree=True)
 
         if yaml_config:
             return Configuration(**yaml_config)
```

### Comparing `servicex-3.0.0a1/servicex_client/dataset.py` & `servicex-3.0.0a2/servicex_client/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,30 @@
             sx_adapter: ServiceXAdapter = None,
             config: Configuration = None,
             query_cache: QueryCache = None,
             servicex_polling_interval: int = 10,
             minio_polling_interval: int = 5,
             result_format: ResultFormat = None
     ):
+        r"""
+        This is the main class for constructing transform requests and receiving the
+        results in a format of your choice. It can be run synchronously or asynchronously.
+
+        :param dataset_identifier: Either a Rucio DID or a list of files
+        :param title: Human readable title for this transform
+        :param codegen: Name of the code generator
+        :param sx_adapter:
+        :param config:
+        :param query_cache:
+        :param servicex_polling_interval: How many seconds between polling for
+                                          transform status?
+        :param minio_polling_interval:  How many seconds between polling the minio bucket
+                                        for new files?
+        :param result_format:
+        """
         super(Dataset, self).__init__()
         self.servicex = sx_adapter
         self.configuration = config
         self.cache = query_cache
 
         self.dataset_identifier = dataset_identifier
         self.codegen = codegen
@@ -111,23 +127,33 @@
             selection=self.generate_selection_string()
         )
         # Transfer the DID into the transform request
         self.dataset_identifier.populate_transform_request(sx_request)
         return sx_request
 
     def set_result_format(self, result_format: ResultFormat):
+        r"""
+        Set the result format - required at constructor time or as part of the query
+        chain of methods
+        :param result_format:
+        :return: self to allow you to chain together query and setup methods
+        """
         self.result_format = result_format
         return self
 
     async def submit_and_download(self, signed_urls_only: bool = False) -> TransformedResults:
         """
         Submit the transform request to ServiceX. Poll the transform status to see when
         the transform completes and to get the number of files in the dataset along with
         current progress and failed file count.
-        :return:
+
+        :param signed_urls_only: Set to true to skip actually downloading the files and
+                                 just return pre-signed urls
+        :return: Transform results object which contains the list of files downlaoded
+                 or the list of pre-signed urls
         """
         download_files_task = None
         loop = asyncio.get_running_loop()
 
         def transform_complete(task: Task):
             """
             Called when the Monitor task completes. This could be because of exception or
@@ -337,25 +363,47 @@
                     (self.current_status and self.current_status.status == Status.complete):
                 break
 
         # Now just wait until all of our tasks complete
         await asyncio.gather(*download_tasks)
         return result_uris
 
-    async def as_parquet_files(self) -> TransformedResults:
-        self.result_format = ResultFormat.parquet
+    async def as_files_async(self) -> TransformedResults:
+        r"""
+        Submit the transform and request all the resulting files to be downloaded
+        :return: TransformResult instance with the list of complete paths to the downloaded files
+        """
         return await self.submit_and_download()
 
-    async def as_root_files(self):
-        self.result_format = ResultFormat.root_file
-        return await self.submit_and_download()
+    def as_files(self) -> TransformedResults:
+        r"""
+        Submit the transform and request all the resulting files to be downloaded
+        :return: TransformResult instance with the list of complete paths to the downloaded files
+        """
+        return asyncio.run(self.submit_and_download())
 
-    async def as_files(self):
-        return await self.submit_and_download()
+    async def as_pandas_async(self):
+        r"""
+        Return a pandas dataframe containing the results. This only works if you've
+        installed pandas extra
 
-    async def as_pandas(self):
-        transformed_result = await self.as_parquet_files()
+        :return: Pandas Dataframe
+        """
+        self.result_format = ResultFormat.parquet
+        transformed_result = await self.as_files_async()
         dataframes = pd.concat([pandas.read_parquet(p) for p in transformed_result.file_list])
         return dataframes
 
-    async def as_signed_urls(self):
+    def as_pandas(self):
+        r"""
+        Synchronous version of as_pandas_asynch
+        :return:
+        """
+        return asyncio.run(self.as_pandas_async())
+
+    async def as_signed_urls(self) -> TransformedResults:
+        r"""
+        Presign URLs for each of the transformed files
+
+        :return: TransformedResults object with the presigned_urls list populated
+        """
         return await self.submit_and_download(signed_urls_only=True)
```

### Comparing `servicex-3.0.0a1/servicex_client/dataset_group.py` & `servicex-3.0.0a2/servicex_client/func_adl/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,22 +21,7 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-import asyncio
-from typing import Coroutine, List
-
-from servicex_client.models import TransformedResults
-
-
-class DatasetGroup:
-    def __init__(self, datasets: List[Coroutine]):
-        self.datasets = datasets
-
-    async def gather_results_async(self) -> List[TransformedResults]:
-        return await asyncio.gather(*self.datasets)
-
-    def gather_results(self) -> List[TransformedResults]:
-        return asyncio.run(self.gather_results_async())
```

### Comparing `servicex-3.0.0a1/servicex_client/dataset_identifier.py` & `servicex-3.0.0a2/servicex_client/dataset_identifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 from typing import List, Union
 
 from servicex_client.models import TransformRequest
 
 
 class DataSetIdentifier:
+    r"""
+    Base class for specifying the dataset to transform. This can either be a list of
+    xRootD URIs or a rucio DID
+    """
     def __init__(self, scheme: str, dataset: str, num_files: int = None):
         self.scheme = scheme
         self.dataset = dataset
         self.num_files = num_files
 
     @property
     def did(self):
@@ -44,19 +48,34 @@
     def populate_transform_request(self, transform_request: TransformRequest) -> None:
         transform_request.did = self.did
         transform_request.file_list = None
 
 
 class RucioDatasetIdentifier(DataSetIdentifier):
     def __init__(self, dataset: str, num_files: int = None):
+        r"""
+        Rucio Dataset - this will be looked up using the Rucio data management
+        service.
+
+        :param dataset: The rucio DID - this can be a dataset or a container of datasets.
+        :param num_files: Maximum number of files to return. This is useful during development
+            to perform quick runs. ServiceX is careful to make sure it always
+            returns the same subset of files.
+
+        """
         super().__init__("rucio", dataset, num_files=num_files)
 
 
 class FileListDataset:
     def __init__(self, files: Union[List[str], str]):
+        r"""
+        Dataset specified as a list of XRootD URIs.
+
+        :param files: Either a list of URIs or a single URI string
+        """
         if type(files) == str:
             self.files = [files]
         else:
             self.files = files
 
     def populate_transform_request(self, transform_request: TransformRequest) -> None:
         transform_request.file_list = self.files
```

### Comparing `servicex-3.0.0a1/servicex_client/func_adl/__init__.py` & `servicex-3.0.0a2/servicex_client/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,7 +21,12 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+from typing import Union
+
+from servicex_client.dataset_identifier import DataSetIdentifier, FileListDataset
+
+DID = Union[DataSetIdentifier, FileListDataset]
```

### Comparing `servicex-3.0.0a1/servicex_client/func_adl/func_adl_dataset.py` & `servicex-3.0.0a2/servicex_client/func_adl_dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 from servicex_client.servicex_adapter import ServiceXAdapter
 from servicex_client.types import DID
 
 T = TypeVar("T")
 
 
 class FuncADLDataset(Dataset, EventDataset[T]):
+    r"""
+    ServiceX Dataset class that uses func_adl query syntax.
+    """
     # These are methods that are translated locally
     _execute_locally = ["ResultPandasDF", "ResultAwkwardArray"]
 
     async def execute_result_async(self, a: ast.AST, title: Optional[str] = None) -> Any:
         pass
 
     def check_data_format_request(self, f_name: str):
@@ -75,14 +78,15 @@
     def clone_with_new_ast(self, new_ast: ast.AST, new_type: typing.Any):
         """
         Override the method from ObjectStream - We need to be careful because the query
         cache is a tinyDB database that holds an open file pointer. We are not allowed
         to clone an open file handle, so for this property we will copy by reference
         and share it between the clones. Turns out ast class is also picky about copies,
         so we set that explicitly.
+
         :param new_ast:
         :param new_type:
         :return:
         """
         clone = copy.copy(self)
         for attr, value in vars(self).items():
             if type(value) == QueryCache:
@@ -94,33 +98,101 @@
 
         clone._item_type = new_type
         return clone
 
     def SelectMany(
         self, func: Union[str, ast.Lambda, Callable[[T], Iterable[S]]]
     ) -> FuncADLDataset[S]:
+        r"""
+        Given the current stream's object type is an array or other iterable, return
+        the items in this objects type, one-by-one. This has the effect of flattening a
+        nested array.
+
+        Arguments:
+
+            func:   The function that should be applied to this stream's objects to return
+                    an iterable. Each item of the iterable is now the stream of objects.
+
+        Returns:
+            The Dataset with the SelectMany operator applied
+
+        Notes:
+            - The function can be a `lambda`, the name of a one-line function, a string that
+              contains a lambda definition, or a python `ast` of type `ast.Lambda`.
+        """
         return super().SelectMany(func)
 
     def Select(self, f: Union[str, ast.Lambda, Callable[[T], S]]) -> FuncADLDataset[S]:
+        r"""
+        Apply a transformation function to each object in the stream, yielding a new type of
+        object. There is a one-to-one correspondence between the input objects and output objects.
+
+        Arguments:
+            f:      selection function (lambda)
+
+        Returns:
+            The Dataset with the Select operator applied
+
+        Notes:
+            - The function can be a `lambda`, the name of a one-line function, a string that
+              contains a lambda definition, or a python `ast` of type `ast.Lambda`.
+        """
+
         return super().Select(f)
 
     def generate_selection_string(self) -> str:
         return self.generate_qastle(self.query_ast)
 
     def Where(self, filter: Union[str, ast.Lambda, Callable[[T], bool]]) -> FuncADLDataset[T]:
+        r"""
+        Filter the object stream, allowing only items for which `filter` evaluates as true through.
+
+        Arguments:
+
+            filter      A filter lambda that returns True/False.
+
+        Returns:
+
+            The Dataset with the Where operator applied
+
+        Notes:
+            - The function can be a `lambda`, the name of a one-line function, a string that
+              contains a lambda definition, or a python `ast` of type `ast.Lambda`.
+        """
+
         return super().Where(filter)
 
     def MetaData(self, metadata: Dict[str, Any]) -> FuncADLDataset[T]:
+        r"""Add metadata to the current object stream. The metadata is an arbitrary set of string
+        key-value pairs. The backend must be able to properly interpret the metadata.
+
+        Returns:
+            The Dataset with the MetaData operator applied
+        """
+
         return super().MetaData(metadata)
 
     def QMetaData(self, metadata: Dict[str, Any]) -> FuncADLDataset[T]:
+        r"""Add query metadata to the current object stream.
+
+        - Metadata is never transmitted to any back end
+        - Metadata is per-query, not per sample.
+
+        Warnings are issued if metadata is overwriting metadata.
+
+        Args:
+            metadata (Dict[str, Any]): Metadata to be used later
+
+        Returns:
+            The Dataset with the QMetaData operator applied
+        """
         return super().QMetaData(metadata)
 
     def generate_qastle(self, a: ast.AST) -> str:
-        """Generate the qastle from the ast of the query.
+        r"""Generate the qastle from the ast of the query.
 
         1. The top level function is already marked as being "ok"
         1. If the top level function is something we have to process locally,
            then we strip it off.
 
         Args:
             a (ast.AST): The complete AST of the request.
@@ -213,8 +285,14 @@
                     keywords=[],
                 )
                 source = c
 
         return python_ast_to_text_ast(source)
 
     def as_qastle(self):
+        r"""
+        Generate Qastle from this AST
+
+        :returns:
+            Qastle representation of the target's AST
+        """
         return self.value()
```

### Comparing `servicex-3.0.0a1/servicex_client/func_adl/util.py` & `servicex-3.0.0a2/servicex_client/func_adl/util.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a1/servicex_client/minio_adpater.py` & `servicex-3.0.0a2/servicex_client/minio_adpater.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a1/servicex_client/models.py` & `servicex-3.0.0a2/servicex_client/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,54 +30,75 @@
 from enum import Enum
 
 from pydantic import BaseModel, Field, validator
 from typing import List, Optional
 
 
 class ResultDestination(str, Enum):
+    r"""
+    Direct the output to object store or posix volume
+    """
     object_store = 'object-store'
     volume = 'volume'
 
 
 class ResultFormat(str, Enum):
+    r"""
+    Specify the file format for the generated output
+    """
     parquet = "parquet",
     root_file = "root-file"
 
 
 class Status(str, Enum):
+    r"""
+    Status of a sumbittied transform
+    """
     complete = "Complete",
     fatal = "Fatal",
     canceled = "Canceled",
     submitted = "Submitted",
     running = "Running"
 
 
 class TransformRequest(BaseModel):
+    r"""
+    Transform request sent to ServiceX
+    """
     title: Optional[str] = None
     did: Optional[str] = None
     file_list: Optional[List[str]] = Field(None, alias='file-list')
     selection: str
     image: Optional[str] = None
     codegen: str
     tree_name: Optional[str] = Field(None, alias='tree-name')
     result_destination: ResultDestination = Field(alias="result-destination")
     result_format: ResultFormat = Field(alias="result-format")
 
     class Config:
         allow_population_by_field_name = True
 
     def compute_hash(self):
+        r"""
+        Compute a hash for this submission. Only include properties that imapact the result
+        so we have maximal ability to reuse transforms
+
+        :return: SHA256 hash of request
+        """
         sha = hashlib.sha256(str([self.did, self.selection, self.tree_name,
                                   self.codegen, self.image,
                                   self.result_format.name, self.file_list]).
                              encode("utf-8"))
         return sha.hexdigest()
 
 
 class TransformStatus(BaseModel):
+    r"""
+    Status object returned by servicex
+    """
     request_id: str
     did: str
     selection: str
     tree_name: Optional[str] = Field(alias="tree-name")
     image: str
     result_destination: ResultDestination = Field(alias="result-destination")
     result_format: ResultFormat = Field(alias="result-format")
@@ -100,20 +121,27 @@
     def parse_finish_time(cls, v):
         if isinstance(v, str) and v == "None":
             return None
         return v
 
 
 class ResultFile(BaseModel):
+    r"""
+    Record reporting the properties of a tranformed file result
+    """
     filename: str
     size: int
     extension: str
 
 
 class TransformedResults(BaseModel):
+    r"""
+    Returned for a submission. Gives you everything you need to know about a completed
+    transform.
+    """
     hash: str
     title: str
     codegen: str
     request_id: str
     submit_time: datetime
     data_dir: str
     file_list: List[str]
```

### Comparing `servicex-3.0.0a1/servicex_client/python_dataset.py` & `servicex-3.0.0a2/servicex_client/python_dataset.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a1/servicex_client/query_cache.py` & `servicex-3.0.0a2/servicex_client/query_cache.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a1/servicex_client/servicex_adapter.py` & `servicex-3.0.0a2/servicex_client/servicex_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 import os
 from datetime import datetime
-from typing import Optional, Dict
+from typing import Optional, Dict, List
 
 import httpx
 from google.auth import jwt
 
 from servicex_client.models import TransformRequest, TransformStatus
 
 
@@ -75,15 +75,15 @@
 
         now = datetime.utcnow().timestamp()
         if not self.token or \
                 float(jwt.decode(self.token, verify=False)["exp"]) - now < 0:
             await self._get_token(client)
         return {"Authorization": f"Bearer {self.token}"}
 
-    async def get_transforms(self):
+    async def get_transforms(self) -> List[TransformStatus]:
         async with httpx.AsyncClient() as client:
             headers = await self._get_authorization(client)
             r = await client.get(url=f"{self.url}/servicex/transformation",
                                  headers=headers)
             if r.status_code == 401:
                 raise AuthorizationError(f"Not authorized to access serviceX at {self.url}")
 
@@ -107,15 +107,15 @@
                                   json=transform_request.dict(by_alias=True,
                                                               exclude_none=True))
             if r.status_code == 401:
                 raise AuthorizationError(
                     f"Not authorized to access serviceX at {self.url}")
         return r.json()['request_id']
 
-    async def get_transform_status(self, request_id: str):
+    async def get_transform_status(self, request_id: str) -> TransformStatus:
         async with httpx.AsyncClient() as client:
             headers = await self._get_authorization(client)
             r = await client.get(url=f"{self.url}/servicex/transformation/{request_id}",
                                  headers=headers)
             if r.status_code == 401:
                 raise AuthorizationError(f"Not authorized to access serviceX at {self.url}")
             if r.status_code == 404:
```

### Comparing `servicex-3.0.0a1/setup.py` & `servicex-3.0.0a2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,26 +17,27 @@
  'qastle>=0.16,<0.17',
  'requests>=2.31,<3.0',
  'tinydb>=4.7,<5.0',
  'typer[all]>=0.9.0,<0.10.0',
  'types-PyYAML>=6.0,<7.0']
 
 extras_require = \
-{'pandas': ['pandas>=2.0.2,<3.0.0',
+{'docs': ['sphinx>=7.0.1,<8.0.0', 'furo>=2023.5.20,<2024.0.0'],
+ 'pandas': ['pandas>=2.0.2,<3.0.0',
             'pyarrow>=12.0.0,<13.0.0',
             'fastparquet>=2023.4.0,<2024.0.0']}
 
 entry_points = \
 {'console_scripts': ['servicex = servicex_client.app.main:app']}
 
 setup_kwargs = {
     'name': 'servicex',
-    'version': '3.0.0a1',
+    'version': '3.0.0a2',
     'description': '',
-    'long_description': '# servicex_client\nPython SDK and CLI Client for ServiceX\n\n## Configuration\nThe client relies on a YAML file to obtain the URLs of different servicex\ndeployments, as well as tokens to authenticate with the service. The file \nshould be named `.servicex` and the format of this file is as follows:\n```yaml\napi_endpoints:\n  - endpoint: http://localhost:5000\n    name: localhost\n\n  - endpoint: https://servicex-release-testing-4.servicex.ssl-hep.org\n    name: testing4\n    token: ...\n\ndefault_endpoint: testing4\n\ncache_path: /tmp/ServiceX_Client/cache-dir\n```\nThe `default_endpoint` will be used if otherwise not specified. The cache \ndatabase and downloaded files will be stored in the directory specified by \n`cache_path`.\n\nThe library will search for this file in the current working directory and then\nstart looking in parent directories until a file is found.\n\n## Command Line Interface\nWhen installed, the client provides a new command in your shell, `servicex`.\nThis command uses a series of subcommands to work with various functions of\nserviceX.\n\nCommon command line arguments:\n\n| Flag | Long Flag | What it does                                         |\n|------|-----------|------------------------------------------------------|\n| -u   | --url     | The url of the serviceX ingress                      |\n| -b   | --backend | Named backend from the .servicex file endpoints list |\n\nIf neither url nor backend are specified then the client will attempt to use the\n`default_endpoint` value to determine who to talk to.\n\n### codegens \nThis command will list the code generators deployed.\n\n### transforms\nThese commands interact with transforms that have been run\n\n#### list\nList transforms associated with the current user. Add the `--complete` flag to\nonly show transforms that have completed.\n\n#### files\nList the files along with their size generated by a transform. Specify the \ntransform request id with the `-t` or `--transform-id` flag\n\n#### download\nDownload the files from a transform to a local directory. Specify the transform\nrequest id with `-t` and the directory to download to with `-d`. Defaults to\ndownloading files to the current working directory.\n\n### cache\nThese commands allow you to work with the query cache maintained by the serviceX\nclient.\n\n#### list\nShow all of the cached transforms along with the run time, code generator, and \nnumber of resulting files\n\n#### delete\nDelete a specific transform from the cache. Provide the transform request ID \nwith the `-t` or `--transform-id` arg.\n\n#### clear\nClear all of the transforms from the cache.\n\n',
+    'long_description': "# servicex_client\nPython SDK and CLI Client for ServiceX\n\n## Configuration\nThe client relies on a YAML file to obtain the URLs of different servicex\ndeployments, as well as tokens to authenticate with the service. The file \nshould be named `.servicex` and the format of this file is as follows:\n```yaml\napi_endpoints:\n  - endpoint: http://localhost:5000\n    name: localhost\n\n  - endpoint: https://servicex-release-testing-4.servicex.ssl-hep.org\n    name: testing4\n    token: ...\n\ndefault_endpoint: testing4\n\ncache_path: /tmp/ServiceX_Client/cache-dir\nshortened_downloaded_filename: true\n\n```\nThe `default_endpoint` will be used if otherwise not specified. The cache \ndatabase and downloaded files will be stored in the directory specified by \n`cache_path`.\n\nThe `shortened_downloaded_filename` property controls whether downloaded files\nwill have their names shortened for convenience. Setting to false preserves\nthe full filename from the dataset.\n`\n\nThe library will search for this file in the current working directory and then\nstart looking in parent directories until a file is found.\n\n## Command Line Interface\nWhen installed, the client provides a new command in your shell, `servicex`.\nThis command uses a series of subcommands to work with various functions of\nserviceX.\n\nCommon command line arguments:\n\n| Flag | Long Flag | What it does                                         |\n|------|-----------|------------------------------------------------------|\n| -u   | --url     | The url of the serviceX ingress                      |\n| -b   | --backend | Named backend from the .servicex file endpoints list |\n\nIf neither url nor backend are specified then the client will attempt to use the\n`default_endpoint` value to determine who to talk to.\n\n### codegens \nThis command will list the code generators deployed.\n\n### transforms\nThese commands interact with transforms that have been run\n\n#### list\nList transforms associated with the current user. Add the `--complete` flag to\nonly show transforms that have completed.\n\n#### files\nList the files along with their size generated by a transform. Specify the \ntransform request id with the `-t` or `--transform-id` flag\n\n#### download\nDownload the files from a transform to a local directory. Specify the transform\nrequest id with `-t` and the directory to download to with `-d`. Defaults to\ndownloading files to the current working directory.\n\n### cache\nThese commands allow you to work with the query cache maintained by the serviceX\nclient.\n\n#### list\nShow all of the cached transforms along with the run time, code generator, and \nnumber of resulting files\n\n#### delete\nDelete a specific transform from the cache. Provide the transform request ID \nwith the `-t` or `--transform-id` arg.\n\n#### clear\nClear all of the transforms from the cache. Add `-y` to force the operation \nwithout confirming with the console.\n\n## Python SDK\nEntry to the SDK starts with constructing an instance of ServiceXClient.  The \nconstructor accepts `backend` argument to specify a named backend from the\n`.servicex` file, or `url` for the direct URL to a serviceX server. With the \nURL option you can't provide a token from `.servicex` so it must either be an\nunsecured endpoint, or the token must be provided via the WLCG standard of a \nfile pointed to by `BEARER_TOKEN_FILE` environment variable.\n\nWith an instance of ServiceXClient you can \n- List the code generators deployed with the ServiceX instance\n- List the transformers that have been run\n- Get the current status of a specific transform\n\n### Create a Dataset Instance to Run Transforms\nThe ServiceX client also can create a `Dataset` instance that \nallows you to specify a query, provide a dataset identifier,\nand retrieve the results of the resulting transform request.\n\nThere are two types of datasets\n- func_adl_dataset\n- Python Function dataset\n\n### Dataset Identifiers\nBefore we get too deeply into the dataset classes, we should look\nat how to specify a dataset.\n- RucioDatasetIdentifier - for retrieving data files registered with Rucio\n- FileListDataset - A list of URIs for accessing files using xRootd\n\n### FuncADL Dataset\nThis dataset is controlled by the func_adl language. The dataset\nsupports the `Select`, `SelectMany`, `Where`, `MetaData`, and `QMetaData` \noperators from func_adl.\n\n\n### Datasets\nThis is the abstract class for requesting data from ServiceX. You have to \nspecify the dataset identifier you want data from and provide some sort of \nselection query. You can set the result format with the `set_result_format` \noperator (it's also a factory method arg for the dataset).\n\nOperators that cause the client to interact with the server: These terminal \noperators will call out to the serviceX server and process results. They\nare all implemented as asynchronous coroutines, but they also come with \nsynchronous versions to make it easy to do easy things.\n\n\n#### \n\n",
     'author': 'Ben Galewsky',
     'author_email': 'bengal1@illinois.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

