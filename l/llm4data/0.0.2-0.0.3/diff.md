# Comparing `tmp/llm4data-0.0.2.tar.gz` & `tmp/llm4data-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4data-0.0.2.tar", max compression
+gzip compressed data, was "llm4data-0.0.3.tar", max compression
```

## Comparing `llm4data-0.0.2.tar` & `llm4data-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,34 @@
--rw-r--r--   0        0        0    30757 2023-05-26 17:27:00.950549 llm4data-0.0.2/LICENSE
--rw-r--r--   0        0        0     9149 2023-06-01 02:16:59.883937 llm4data-0.0.2/README.md
--rw-r--r--   0        0        0      289 2023-06-01 02:14:09.993471 llm4data-0.0.2/llm4data/__init__.py
--rw-r--r--   0        0        0     3005 2023-05-31 23:34:02.046844 llm4data-0.0.2/llm4data/configs.py
--rw-r--r--   0        0        0      243 2023-05-31 23:34:02.046957 llm4data-0.0.2/llm4data/embeddings/__init__.py
--rw-r--r--   0        0        0     3155 2023-05-31 23:34:02.047055 llm4data-0.0.2/llm4data/embeddings/base.py
--rw-r--r--   0        0        0      528 2023-05-31 23:34:02.047157 llm4data-0.0.2/llm4data/embeddings/docs.py
--rw-r--r--   0        0        0      796 2023-05-31 23:34:02.047256 llm4data-0.0.2/llm4data/embeddings/indicators.py
--rw-r--r--   0        0        0      803 2023-05-31 23:34:02.047356 llm4data-0.0.2/llm4data/embeddings/microdata.py
--rw-r--r--   0        0        0      170 2023-05-31 23:34:02.047500 llm4data-0.0.2/llm4data/index/index.py
--rw-r--r--   0        0        0     2356 2023-05-31 23:34:02.047613 llm4data-0.0.2/llm4data/index/qdrant.py
--rw-r--r--   0        0        0     5550 2023-05-27 17:39:27.522862 llm4data-0.0.2/llm4data/llm/indicators/wdi_sql.py
--rw-r--r--   0        0        0        0 2023-05-26 16:41:36.283163 llm4data-0.0.2/llm4data/llm/microdata/.gitkeep
--rw-r--r--   0        0        0     1407 2023-05-27 17:11:44.934021 llm4data-0.0.2/llm4data/prompts/base.py
--rw-r--r--   0        0        0     1663 2023-05-27 17:39:37.424246 llm4data-0.0.2/llm4data/prompts/indicators/templates.py
--rw-r--r--   0        0        0     3945 2023-05-27 17:39:32.427008 llm4data-0.0.2/llm4data/prompts/indicators/wdi.py
--rw-r--r--   0        0        0        0 2023-05-26 16:40:23.801226 llm4data-0.0.2/llm4data/prompts/microdata/.gitkeep
--rw-r--r--   0        0        0      352 2023-05-26 19:58:54.433048 llm4data-0.0.2/llm4data/prompts/utils.py
--rw-r--r--   0        0        0    11208 2023-05-30 17:15:25.960735 llm4data-0.0.2/llm4data/schema/docs/wbdocs.py
--rw-r--r--   0        0        0     3146 2023-05-27 00:12:24.551761 llm4data-0.0.2/llm4data/sources/indicators/wdi.py
--rw-r--r--   0        0        0        0 2023-05-26 16:41:22.772734 llm4data-0.0.2/llm4data/sources/microdata/.gitkeep
--rw-r--r--   0        0        0   117888 2023-05-24 15:43:46.011357 llm4data-0.0.2/llm4data/wdi2name.json
--rw-r--r--   0        0        0     1290 2023-06-01 02:14:09.985816 llm4data-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    10298 1970-01-01 00:00:00.000000 llm4data-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    30757 2023-05-26 17:27:00.950549 llm4data-0.0.3/LICENSE
+-rw-r--r--   0        0        0     9149 2023-06-05 20:17:16.274426 llm4data-0.0.3/README.md
+-rw-r--r--   0        0        0      289 2023-06-19 04:29:36.913046 llm4data-0.0.3/llm4data/__init__.py
+-rw-r--r--   0        0        0     3172 2023-06-15 20:16:00.899057 llm4data-0.0.3/llm4data/configs.py
+-rw-r--r--   0        0        0      243 2023-05-31 23:34:02.046957 llm4data-0.0.3/llm4data/embeddings/__init__.py
+-rw-r--r--   0        0        0     3186 2023-06-15 20:16:00.899273 llm4data-0.0.3/llm4data/embeddings/base.py
+-rw-r--r--   0        0        0      566 2023-06-15 20:16:00.899473 llm4data-0.0.3/llm4data/embeddings/docs.py
+-rw-r--r--   0        0        0      834 2023-06-15 20:16:00.899679 llm4data-0.0.3/llm4data/embeddings/indicators.py
+-rw-r--r--   0        0        0      841 2023-06-15 20:16:00.899898 llm4data-0.0.3/llm4data/embeddings/microdata.py
+-rw-r--r--   0        0        0      170 2023-06-15 20:16:00.900058 llm4data-0.0.3/llm4data/index/__init__.py
+-rw-r--r--   0        0        0     2680 2023-06-15 20:16:00.900299 llm4data-0.0.3/llm4data/index/qdrant.py
+-rw-r--r--   0        0        0     5838 2023-06-19 04:14:57.702274 llm4data-0.0.3/llm4data/llm/indicators/wdi_sql.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:41:36.283163 llm4data-0.0.3/llm4data/llm/microdata/.gitkeep
+-rw-r--r--   0        0        0     1780 2023-06-15 20:16:00.900797 llm4data-0.0.3/llm4data/prompts/base.py
+-rw-r--r--   0        0        0     2945 2023-06-18 23:29:06.835846 llm4data-0.0.3/llm4data/prompts/context.py
+-rw-r--r--   0        0        0     1663 2023-05-27 17:39:37.424246 llm4data-0.0.3/llm4data/prompts/indicators/templates.py
+-rw-r--r--   0        0        0     5065 2023-06-19 04:14:57.702708 llm4data-0.0.3/llm4data/prompts/indicators/wdi.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:40:23.801226 llm4data-0.0.3/llm4data/prompts/microdata/.gitkeep
+-rw-r--r--   0        0        0      352 2023-05-26 19:58:54.433048 llm4data-0.0.3/llm4data/prompts/utils.py
+-rw-r--r--   0        0        0     1030 2023-06-18 23:29:06.836040 llm4data-0.0.3/llm4data/schema/docs/migrate_wbdocs_metadata.py
+-rw-r--r--   0        0        0    24359 2023-06-15 20:16:00.901481 llm4data-0.0.3/llm4data/schema/docs/wbdocs.py
+-rw-r--r--   0        0        0     1647 2023-06-18 23:29:06.836205 llm4data-0.0.3/llm4data/schema/indicators/create_wdi_text.py
+-rw-r--r--   0        0        0     1130 2023-06-18 23:29:06.836396 llm4data-0.0.3/llm4data/schema/schema2info.py
+-rw-r--r--   0        0        0        0 2023-06-15 20:16:00.901705 llm4data-0.0.3/llm4data/scripts/__init__.py
+-rw-r--r--   0        0        0     1572 2023-06-19 04:14:57.702920 llm4data-0.0.3/llm4data/scripts/indexing/create_field_index.py
+-rw-r--r--   0        0        0     1684 2023-06-16 04:24:21.755270 llm4data-0.0.3/llm4data/scripts/indexing/docs/docs.py
+-rw-r--r--   0        0        0     3518 2023-06-15 20:16:00.902507 llm4data-0.0.3/llm4data/scripts/indexing/docs/load_docs.py
+-rw-r--r--   0        0        0      944 2023-06-18 23:29:06.836656 llm4data-0.0.3/llm4data/scripts/indexing/indicators/indicators.py
+-rw-r--r--   0        0        0     2789 2023-06-19 04:14:57.703168 llm4data-0.0.3/llm4data/scripts/indexing/indicators/load_indicators.py
+-rw-r--r--   0        0        0     3146 2023-05-27 00:12:24.551761 llm4data-0.0.3/llm4data/sources/indicators/wdi.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:41:22.772734 llm4data-0.0.3/llm4data/sources/microdata/.gitkeep
+-rw-r--r--   0        0        0   117888 2023-05-24 15:43:46.011357 llm4data-0.0.3/llm4data/wdi2name.json
+-rw-r--r--   0        0        0     1353 2023-06-19 04:29:36.903585 llm4data-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    10419 1970-01-01 00:00:00.000000 llm4data-0.0.3/PKG-INFO
```

### Comparing `llm4data-0.0.2/LICENSE` & `llm4data-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.2/README.md` & `llm4data-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.2/llm4data/configs.py` & `llm4data-0.0.3/llm4data/configs.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from dataclasses import dataclass
 
 
 # Define a data class for the database config
 @dataclass
 class WDIDBConfig:
     table_name: Optional[str] = os.getenv("WDI_DB_TABLE_NAME")
-    engine: Optional[str] = os.getenv("WDI_DB_ENGINE")
-    host: Optional[str] = os.getenv("WDI_DB_HOST")
-    port: Optional[str] = os.getenv("WDI_DB_PORT")
-    username: Optional[str] = os.getenv("WDI_DB_USERNAME")
-    password: Optional[str] = os.getenv("WDI_DB_PASSWORD")
+    engine: Optional[str] = os.getenv("DB_ENGINE")
+    host: Optional[str] = os.getenv("DB_HOST")
+    port: Optional[str] = os.getenv("DB_PORT")
+    username: Optional[str] = os.getenv("DB_USERNAME")
+    password: Optional[str] = os.getenv("DB_PASSWORD")
 
     @property
     def url(self):
         url = f"{self.engine}://{self.username}"
 
         if self.password:
             url += f":{self.password}"
@@ -39,33 +39,43 @@
 
     _exception_template = "`{dirvar}` environment variable is not set. Consider adding it to your .env file."
 
     def __post_init__(self):
         self.llm4data_dir = self._process_dir(self.llm4data_dir, "LLM4DATA_DIR")
 
         if not isinstance(self.llm4data_cache_dir, str):
-            raise ValueError("`LLM4DATA_CACHE_DIR` environment variable must be a string.")
+            raise ValueError(
+                "`LLM4DATA_CACHE_DIR` environment variable must be a string."
+            )
 
         if not isinstance(self.openai_payload_dir, str):
-            raise ValueError("`OPENAI_PAYLOAD_DIR` environment variable must be a string.")
+            raise ValueError(
+                "`OPENAI_PAYLOAD_DIR` environment variable must be a string."
+            )
 
         self.llm4data_cache_dir = self.llm4data_dir / self.llm4data_cache_dir
         self.openai_payload_dir = self.llm4data_dir / self.openai_payload_dir
 
-        self.llm4data_cache_dir = self._process_dir(self.llm4data_cache_dir, "LLM4DATA_CACHE_DIR")
-        self.openai_payload_dir = self._process_dir(self.openai_payload_dir, "OPENAI_PAYLOAD_DIR")
+        self.llm4data_cache_dir = self._process_dir(
+            self.llm4data_cache_dir, "LLM4DATA_CACHE_DIR"
+        )
+        self.openai_payload_dir = self._process_dir(
+            self.openai_payload_dir, "OPENAI_PAYLOAD_DIR"
+        )
 
     def _process_dir(self, dirname: Union[str, Path], dirvar: str) -> Path:
         if not dirname:
             raise ValueError(self._exception_template.format(dirvar=dirvar))
 
         dirname = Path(dirname).expanduser().resolve()
 
         if dirvar != "LLM4DATA_DIR" and self.llm4data_dir == dirname:
-            raise ValueError(f"{dirvar}={dirname} is the same as LLM4DATA_DIR={self.llm4data_dir}")
+            raise ValueError(
+                f"{dirvar}={dirname} is the same as LLM4DATA_DIR={self.llm4data_dir}"
+            )
 
         if not dirname.exists():
             warnings.warn(f"{dirvar}={dirname} does not exist. Creating it now...")
             dirname.mkdir(parents=True)
 
         return dirname
 
@@ -81,7 +91,10 @@
             )
 
 
 # Instantiate the config objects
 wdidb = WDIDBConfig()
 dirs = DirsConfig()  # NOTE: `dirs` is a reserved keyword in Python
 task_labels = TaskLabelsConfig()
+
+# Define the metadata key
+METADATA_KEY = "llm4data"
```

### Comparing `llm4data-0.0.2/llm4data/embeddings/base.py` & `llm4data-0.0.3/llm4data/embeddings/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from pydantic.main import ModelMetaclass
 from qdrant_client.http import models
 from pydantic.main import ModelMetaclass
 from dataclasses import dataclass, asdict
 
 
 # Make the model atomically available
-LOADED_MODELS = {}
+LOADED_MODELS: dict = {}
+
 
 @dataclass
 class BaseEmbeddingModel:
     model_size = {
         "instruct": 768,
         "all-MiniLM-L6-v2": 384,
         "multi-qa-mpnet-base-dot-v1": 768,
@@ -39,15 +40,14 @@
 
     def dict(self):
         return asdict(self)
 
 
 @dataclass
 class EmbeddingModel(BaseEmbeddingModel):
-
     def __post_init__(self):
         self._common_init()
         self._instruct_init()
         self._hf_init()
 
         self._create_embeddings()
 
@@ -76,27 +76,29 @@
             if not (self.embed_instruction and self.query_instruction):
                 raise ValueError(
                     "`embed_instruction` and `query_instruction` must be set if `is_instruct` is True."
                 )
             self.kwargs = {
                 **self.kwargs,
                 "embed_instruction": self.embed_instruction,
-                "query_instruction": self.query_instruction
+                "query_instruction": self.query_instruction,
             }
 
     def _hf_init(self):
         assert isinstance(self.kwargs, dict)
 
         if self.embedding_cls == "HuggingFaceEmbeddings":
             self.kwargs = {
                 **self.kwargs,
                 "model_name": self.model_name,
             }
 
-    def _create_embeddings(self) -> ModelMetaclass:
+    def _create_embeddings(self):
         if not isinstance(self.kwargs, dict):
             raise ValueError("`config.kwargs` must be a dict")
 
-        self.embeddings = getattr(langchain_embeddings, self.embedding_cls)(**self.kwargs)
+        self.embeddings = getattr(langchain_embeddings, self.embedding_cls)(
+            **self.kwargs
+        )
 
-        if self.max_tokens is None:
+        if self.max_tokens is None and self.embeddings:
             self.max_tokens = self.embeddings.client.max_seq_length
```

### Comparing `llm4data-0.0.2/llm4data/embeddings/docs.py` & `llm4data-0.0.3/llm4data/embeddings/docs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from typing import Optional
 from dataclasses import dataclass
 from llm4data.embeddings.base import EmbeddingModel
 
-DOCS_EMBEDDINGS: EmbeddingModel = None
+DOCS_EMBEDDINGS: Optional[EmbeddingModel] = None
 
 
 @dataclass
 class DocsEmbedding(EmbeddingModel):
     data_type: str = "docs"
```

### Comparing `llm4data-0.0.2/llm4data/embeddings/indicators.py` & `llm4data-0.0.3/llm4data/embeddings/indicators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from typing import Optional
 from dataclasses import dataclass
 from llm4data.embeddings.base import EmbeddingModel
 
-INDICATORS_EMBEDDINGS: EmbeddingModel = None
+INDICATORS_EMBEDDINGS: Optional[EmbeddingModel] = None
 
 
 @dataclass
 class IndicatorsEmbedding(EmbeddingModel):
     data_type: str = "indicators"
```

### Comparing `llm4data-0.0.2/llm4data/embeddings/microdata.py` & `llm4data-0.0.3/llm4data/embeddings/microdata.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from typing import Optional
 from dataclasses import dataclass
 from llm4data.embeddings.base import EmbeddingModel
 
-MICRODATA_EMBEDDINGS: EmbeddingModel = None
+MICRODATA_EMBEDDINGS: Optional[EmbeddingModel] = None
 
 
 @dataclass
 class MicrodataEmbedding(EmbeddingModel):
     data_type: str = "microdata"
```

### Comparing `llm4data-0.0.2/llm4data/index/qdrant.py` & `llm4data-0.0.3/llm4data/index/qdrant.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from typing import Optional, Union
 from langchain.vectorstores import Qdrant
 import qdrant_client
 from qdrant_client.http import models
 
 from ..embeddings.docs import get_docs_embeddings
 from ..embeddings.indicators import get_indicators_embeddings
 from ..embeddings.microdata import get_microdata_embeddings
@@ -11,55 +12,69 @@
 
 
 def collection_exists(collection_name: str) -> bool:
     colls = get_index_client().get_collections()
     return collection_name in [i.name for i in colls.collections]
 
 
-def get_index_client(path: str = None):
+def get_index_client(path: Optional[str] = None):
     global _CLIENT
     if _CLIENT is None:
-        if os.environ.get("QDRANT_URL") is not None:
-            url = os.environ.get("QDRANT_URL")
-            if os.environ.get("QDRANT_PORT") is not None:
-                url += f":{os.environ.get('QDRANT_PORT')}"
-            _CLIENT = qdrant_client.QdrantClient(url=url, prefer_grpc=False)
-        elif os.environ.get("QDRANT_PATH") is not None:
-            path = os.environ.get("QDRANT_PATH")
+        if path is not None:
             _CLIENT = qdrant_client.QdrantClient(path=path, prefer_grpc=True)
         else:
-            raise ValueError("QDRANT_URL or QDRANT_PATH not set in the environment")
+            url = os.environ.get("QDRANT_URL")
+            if url is not None:
+                port = os.environ.get("QDRANT_PORT")
+                if port is not None:
+                    url += f":{port}"
+                _CLIENT = qdrant_client.QdrantClient(url=url, prefer_grpc=False)
+            else:
+                path = os.environ.get("QDRANT_PATH")
+                if path is not None:
+                    _CLIENT = qdrant_client.QdrantClient(path=path, prefer_grpc=True)
+                else:
+                    raise ValueError("QDRANT_URL or QDRANT_PATH not set in the environment")
 
     return _CLIENT
 
 
-def get_index_collection(embeddings, path: str = None, recreate: bool = False):
+def get_index_collection(embeddings, path: Optional[str] = None, recreate: bool = False):
     client = get_index_client(path=path)
 
     if recreate:
         client.recreate_collection(
             collection_name=embeddings.collection_name,
-            vectors_config=models.VectorParams(size=embeddings.size, distance=embeddings.distance),
+            vectors_config=models.VectorParams(
+                size=embeddings.size, distance=embeddings.distance
+            ),
         )
 
     if not collection_exists(embeddings.collection_name):
         client.create_collection(
             collection_name=embeddings.collection_name,
-            vectors_config=models.VectorParams(size=embeddings.size, distance=embeddings.distance),
+            vectors_config=models.VectorParams(
+                size=embeddings.size, distance=embeddings.distance
+            ),
         )
 
     return Qdrant(
-        client=client, collection_name=embeddings.collection_name,
-        embeddings=embeddings.embeddings
+        client=client,
+        collection_name=embeddings.collection_name,
+        embeddings=embeddings.embeddings,
     )
 
 
-def get_docs_index(path: str = None, recreate: bool = False):
+def get_docs_index(path: Optional[str] = None, recreate: bool = False):
     return get_index_collection(get_docs_embeddings(), path=path, recreate=recreate)
 
 
-def get_indicators_index(path: str = None, recreate: bool = False):
-    return get_index_collection(get_indicators_embeddings(), path=path, recreate=recreate)
+def get_indicators_index(path: Optional[str] = None, recreate: bool = False):
+    return get_index_collection(
+        get_indicators_embeddings(), path=path, recreate=recreate
+    )
 
 
-def get_microdata_index(path: str = None, recreate: bool = False):
-    return get_index_collection(get_microdata_embeddings(), path=path, recreate=recreate)
+def get_microdata_index(path: Optional[str] = None, recreate: bool = False):
+    return get_index_collection(
+        get_microdata_embeddings(), path=path, recreate=recreate
+    )
```

### Comparing `llm4data-0.0.2/llm4data/llm/indicators/wdi_sql.py` & `llm4data-0.0.3/llm4data/llm/indicators/wdi_sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,28 +30,36 @@
         files and save them to an sqlite database.
 
         Structure is based on the output of `scripts/scrapers/indicators/wdi.py`.
 
         Do bulk insert.
         """
 
+        # Drop and recreate the table
+        cls.__table__.drop(engine, checkfirst=True)
+        Base.metadata.create_all(engine)
+
         wdi_jsons_dir = Path(wdi_jsons_dir)
 
         if not wdi_jsons_dir.exists() or not wdi_jsons_dir.is_dir():
             raise ValueError(f"Invalid wdi_jsons_dir: {wdi_jsons_dir}")
 
         wdi_jsons = list(wdi_jsons_dir.glob("*.json"))
         print(f"Found {len(wdi_jsons)} WDI JSON files.")
 
         wdi_jsons = sorted(wdi_jsons)
         for wdi_json in tqdm(wdi_jsons):
             wdi_objects = cls.from_indicator_json(wdi_json)
             session.bulk_save_objects(wdi_objects)
             session.commit()
 
+        # # Create an index on the indicator column
+        # psql -U postgres -d wdi
+        # CREATE INDEX indicator_index ON wdi USING hash (indicator);
+
     @classmethod
     def run_sql(
         cls,
         sql,
         params=None,
         pandas=True,
         as_dict=False,
@@ -185,15 +193,14 @@
         params=None,
         pandas=True,
         as_dict=False,
         to_markdown=False,
         drop_na=True,
         num_samples=20,
     ):
-
         if params is None:
             params = {}
 
         params["indicator"] = self.indicator_id
 
         return super().llm2sql_answer(
             prompt,
```

### Comparing `llm4data-0.0.2/llm4data/prompts/base.py` & `llm4data-0.0.3/llm4data/prompts/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -44,7 +44,23 @@
             api_kwargs=api_kwargs,
             **send_prompt_kwargs,
         )
 
     @abstractmethod
     def parse_response(self, response: dict, **kwargs: Any) -> Any:
         pass
+
+
+class APIPrompt(DatedPrompt):
+    task_label = "APIPrompt"
+    prompt_type = "zeros"
+    template = "Current date: {now}\n\n"
+
+    @abstractmethod
+    def parse_response(
+        self, response: dict, **kwargs: Any
+    ) -> Any:
+        pass
+
+    @abstractmethod
+    def send_prompt_get_sample(self, prompt: str, n_samples: int = 10, **kwargs: Any) -> dict:
+        pass
```

### Comparing `llm4data-0.0.2/llm4data/prompts/indicators/templates.py` & `llm4data-0.0.3/llm4data/prompts/indicators/templates.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.2/llm4data/prompts/indicators/wdi.py` & `llm4data-0.0.3/llm4data/prompts/indicators/wdi.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import json
+import requests
+import pandas as pd
 from typing import Any
 from urllib.parse import urlparse
 from openai_tools.parser import parse_misparsed
-from llm4data.prompts.base import DatedPrompt
+from llm4data.prompts.base import DatedPrompt, APIPrompt
 
 
 class WDISQLPrompt(DatedPrompt):
     task_label = "WDISQLPrompt"
 
     def __init__(self, input_variables=None, template=None):
         if template is None and input_variables is None:
             input_variables = ["now", "table", "fields"]
             template = (
                 "Current date: {now}\n\n"
                 "I have a database containing data from the WDI indicators."
                 " Write an SQL query for the prompt: ```{{{{user_content}}}}```\n\n"
                 "table: {table}\n"
                 "fields: {fields}\n\n"
-                " Use the convention `:param` and not `?`."
+                "Only the indicator can parameterized and you must fill the rest."
+                " Use the convention `:indicator` and not `?`."
                 " Use country_iso3 when querying, use country in the result.\n\n"
                 "Use the last 10 years if no year is specified."
                 " Drop rows with no value.\n\n"
                 "Return the entire row if useful for the prompt."
                 " If it will help in the analysis and if it makes sense, always add the year in the `SELECT` clause if it is not already there.\n\n"
                 """Return the output as JSON for json.loads: {{"query_string": <SQL>}}"""
             )
@@ -40,15 +43,15 @@
             query_string = content["query_string"]
         except json.JSONDecodeError:
             query_string = response["content"].strip()
 
         return query_string
 
 
-class WDIAPIPrompt(DatedPrompt):
+class WDIAPIPrompt(APIPrompt):
     """Context for generating a WDI API URL from a prompt.
 
     Example API URL:
         - https://api.worldbank.org/v2/country/PHL;IDN;MYS;SGP;THA;VNM/indicator/NY.GDP.MKTP.CD;EN.ATM.CO2E.KT?date=2013:2022&format=json&source=2
     """
 
     task_label = "WDIAPIPrompt"
@@ -70,14 +73,15 @@
                 "return: Your response must only be the completed and valid API URL: https://api.worldbank.org/v2/...&format=json\n\n"
                 "Always add `source=...` to the URL if multiple indicators are in the URL.\n\n"
                 "Do not explain."
             )
 
         super().__init__(input_variables=input_variables, template=template)
 
+    @staticmethod
     def get_indicator_code_from_url(url):
         """
         Get the indicator code from a WDI API URL.
         """
         parsed = urlparse(url)
         path = parsed.path
         path = path.split("/")
@@ -94,7 +98,40 @@
 
         if "None" in endpoint:
             endpoint = None
         else:
             endpoint = endpoint + f"&per_page={per_page}"
 
         return endpoint
+
+    def send_prompt_get_sample(self, prompt: str, n_samples: int = 10, **kwargs: Any) -> dict:
+        default = dict(
+            use_wdi=False,
+            wdi_api=None,
+            series_code=None,
+            data=None,
+        )
+
+        response = self.send_prompt(prompt=prompt)
+        endpoint = self.parse_response(response=response, **kwargs)
+
+        if endpoint is None:
+            return default
+
+        request = requests.get(endpoint)
+
+        if request.status_code != 200:
+            return default
+
+        try:
+            request_json = request.json()
+
+            data = pd.DataFrame(request_json[1]).sort_values("date", ascending=False)
+
+            return dict(
+                use_wdi=True,
+                wdi_api=endpoint,
+                series_code=self.get_indicator_code_from_url(endpoint),
+                sample=data.head(n_samples).to_dict(orient="records"),
+            )
+        except Exception as e:
+            return default
```

### Comparing `llm4data-0.0.2/llm4data/sources/indicators/wdi.py` & `llm4data-0.0.3/llm4data/sources/indicators/wdi.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.2/llm4data/wdi2name.json` & `llm4data-0.0.3/llm4data/wdi2name.json`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.2/pyproject.toml` & `llm4data-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm4data"
-version = "0.0.2"
+version = "0.0.3"
 description = "LLM4Data is a Python library designed to facilitate the application of large language models (LLMs) and artificial intelligence for development data and knowledge discovery."
 authors = ["Aivin V. Solatorio <avsolatorio@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.0.1"
@@ -16,14 +16,17 @@
 psycopg2-binary = "^2.9.6"
 python-dotenv = "^1.0.0"
 tiktoken = "^0.4.0"
 fire = "^0.5.0"
 qdrant-client = {version = "^1.2.0", python = ">=3.10,<3.12"}
 sentence-transformers = "^2.2.2"
 instructorembedding = "^1.0.1"
+pymupdf = "^1.22.3"
+metaschema = "0.0.3"
+pycountry = "^22.3.5"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 pytest-dotenv = "^0.5.2"
```

### Comparing `llm4data-0.0.2/PKG-INFO` & `llm4data-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: llm4data
-Version: 0.0.2
+Version: 0.0.3
 Summary: LLM4Data is a Python library designed to facilitate the application of large language models (LLMs) and artificial intelligence for development data and knowledge discovery.
 Author: Aivin V. Solatorio
 Author-email: avsolatorio@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: instructorembedding (>=1.0.1,<2.0.0)
 Requires-Dist: langchain (>=0.0.178,<0.0.179)
+Requires-Dist: metaschema (==0.0.3)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: openai-tools (==0.0.0.1.dev3)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
+Requires-Dist: pycountry (>=22.3.5,<23.0.0)
+Requires-Dist: pymupdf (>=1.22.3,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: qdrant-client (>=1.2.0,<2.0.0) ; python_version >= "3.10" and python_version < "3.12"
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.15,<3.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
```

