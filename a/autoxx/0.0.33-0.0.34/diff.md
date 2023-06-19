# Comparing `tmp/autoxx-0.0.33.tar.gz` & `tmp/autoxx-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.33.tar", max compression
+gzip compressed data, was "autoxx-0.0.34.tar", max compression
```

## Comparing `autoxx-0.0.33.tar` & `autoxx-0.0.34.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.33/README.md
--rw-r--r--   0        0        0     7808 2023-06-14 07:11:34.884437 autoxx-0.0.33/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.33/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.33/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.33/autoxx/config/config.py
--rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.33/autoxx/setup.py
--rw-r--r--   0        0        0     7895 2023-06-15 10:14:04.414108 autoxx-0.0.33/autoxx/tools/knowledge_base/base.py
--rw-r--r--   0        0        0      409 2023-06-14 01:47:30.199685 autoxx-0.0.33/autoxx/tools/llm/base.py
--rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.33/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0    13277 2023-06-15 02:57:54.299087 autoxx-0.0.33/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0     1060 2023-06-15 03:38:02.463809 autoxx-0.0.33/autoxx/utils/base.py
--rw-r--r--   0        0        0     3197 2023-06-15 10:05:15.563247 autoxx-0.0.33/autoxx/utils/llm.py
--rw-r--r--   0        0        0     2271 2023-06-14 03:11:09.896898 autoxx-0.0.33/autoxx/utils/openai_models.py
--rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.33/autoxx/utils/processing_html.py
--rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.33/autoxx/utils/processing_text.py
--rw-r--r--   0        0        0     2631 2023-06-15 01:51:01.679558 autoxx-0.0.33/autoxx/utils/token_counter.py
--rw-r--r--   0        0        0      684 2023-06-15 10:15:09.470687 autoxx-0.0.33/pyproject.toml
--rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 autoxx-0.0.33/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.34/README.md
+-rw-r--r--   0        0        0     7808 2023-06-14 07:11:34.884437 autoxx-0.0.34/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.34/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.34/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.34/autoxx/config/config.py
+-rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.34/autoxx/setup.py
+-rw-r--r--   0        0        0     7667 2023-06-19 02:24:52.204933 autoxx-0.0.34/autoxx/tools/knowledge_base/base.py
+-rw-r--r--   0        0        0      409 2023-06-14 01:47:30.199685 autoxx-0.0.34/autoxx/tools/llm/base.py
+-rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.34/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0    13277 2023-06-15 02:57:54.299087 autoxx-0.0.34/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0     1060 2023-06-15 03:38:02.463809 autoxx-0.0.34/autoxx/utils/base.py
+-rw-r--r--   0        0        0     3197 2023-06-15 10:05:15.563247 autoxx-0.0.34/autoxx/utils/llm.py
+-rw-r--r--   0        0        0     2271 2023-06-14 03:11:09.896898 autoxx-0.0.34/autoxx/utils/openai_models.py
+-rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.34/autoxx/utils/processing_html.py
+-rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.34/autoxx/utils/processing_text.py
+-rw-r--r--   0        0        0     2631 2023-06-15 01:51:01.679558 autoxx-0.0.34/autoxx/utils/token_counter.py
+-rw-r--r--   0        0        0      684 2023-06-19 02:30:59.089507 autoxx-0.0.34/pyproject.toml
+-rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 autoxx-0.0.34/PKG-INFO
```

### Comparing `autoxx-0.0.33/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.34/autoxx/agent/babyagi/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.33/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.34/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.33/autoxx/agent/react/agent.py` & `autoxx-0.0.34/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.33/autoxx/config/config.py` & `autoxx-0.0.34/autoxx/config/config.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.33/autoxx/tools/knowledge_base/base.py` & `autoxx-0.0.34/autoxx/tools/knowledge_base/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,24 +137,19 @@
             print("Error:", e)
             raise Exception(f"failed to retrieve nodes: {str(e)}")
 
     def upsert_document(self, documents: List[Document]) -> None:
         self.index.docstore.add_documents(documents, allow_update=True)
         for document in documents:
             nodes = self.index.service_context.node_parser.get_nodes_from_documents([document])
-            print(nodes)
             self.index.insert_nodes(nodes)
 
     def delete_document(self, document_id: str) -> None:
         self.index.delete_ref_doc(document_id)
         self.index.docstore.delete_document(document_id)
-        try:
-            self.vector_store.delete(document_id, namespace=self.namespace)
-        except Exception as e:
-            print(f"failed to delete vector for document {document_id}: {str(e)}")
 
     def retrieve_document(self, document_ids: List[str]) ->  List[Document]:
         if document_ids is None or len(document_ids) == 0:
             return [doc for _, doc in self.index.docstore.docs.items()]
 
         documents = []
         for document_id in document_ids:
```

### Comparing `autoxx-0.0.33/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.34/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.33/autoxx/tools/web_search/search.py` & `autoxx-0.0.34/autoxx/tools/web_search/search.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.33/autoxx/utils/base.py` & `autoxx-0.0.34/autoxx/utils/base.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.33/autoxx/utils/llm.py` & `autoxx-0.0.34/autoxx/utils/llm.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.33/autoxx/utils/openai_models.py` & `autoxx-0.0.34/autoxx/utils/openai_models.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.33/autoxx/utils/processing_html.py` & `autoxx-0.0.34/autoxx/utils/processing_html.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.33/autoxx/utils/processing_text.py` & `autoxx-0.0.34/autoxx/utils/processing_text.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.33/autoxx/utils/token_counter.py` & `autoxx-0.0.34/autoxx/utils/token_counter.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.33/pyproject.toml` & `autoxx-0.0.34/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.33"
+version = "0.0.34"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -16,15 +16,15 @@
 bs4 = "0.0.1"
 webdriver_manager = "3.8.6"
 tiktoken = "0.3.3"
 playsound = "1.2.2"
 gTTS = "2.3.1"
 orjson = "3.8.10"
 spacy = ">=3.0.0,<4.0.0"
-llama-index = "^0.6.23"
+llama-index = "^0.6.27"
 google-api-python-client = "^2.86.0"
 pymongo = "^4.3.3"
 transformers = "^4.30.1"
 langchain = "^0.0.200"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `autoxx-0.0.33/PKG-INFO` & `autoxx-0.0.34/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.33
+Version: 0.0.34
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bs4 (==0.0.1)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: gTTS (==2.3.1)
 Requires-Dist: google-api-python-client (>=2.86.0,<3.0.0)
 Requires-Dist: langchain (>=0.0.200,<0.0.201)
-Requires-Dist: llama-index (>=0.6.23,<0.7.0)
+Requires-Dist: llama-index (>=0.6.27,<0.7.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: orjson (==3.8.10)
 Requires-Dist: pinecone-client (==2.2.1)
 Requires-Dist: playsound (==1.2.2)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: selenium (==4.9.0)
```

