# Comparing `tmp/langchain_wenxin-0.4.0.tar.gz` & `tmp/langchain_wenxin-0.5.0.tar.gz`

## Comparing `langchain_wenxin-0.4.0.tar` & `langchain_wenxin-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.4.0/src/langchain_wenxin/__about__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.4.0/src/langchain_wenxin/__init__.py
--rw-r--r--   0        0        0    14827 2020-02-02 00:00:00.000000 langchain_wenxin-0.4.0/src/langchain_wenxin/llms.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 langchain_wenxin-0.4.0/src/langchain_wenxin/retrievers.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 langchain_wenxin-0.4.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 langchain_wenxin-0.4.0/README.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 langchain_wenxin-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 langchain_wenxin-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/src/langchain_wenxin/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/src/langchain_wenxin/__init__.py
+-rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/src/langchain_wenxin/llms.py
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/src/langchain_wenxin/retrievers.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/README.md
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/PKG-INFO
```

### Comparing `langchain_wenxin-0.4.0/src/langchain_wenxin/llms.py` & `langchain_wenxin-0.5.0/src/langchain_wenxin/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
         self.access_token = ""
         self.access_token_expires = 0
 
     def completions_url(self, model: str) -> str:
         """Get the URL for the completions endpoint."""
         endpoint = "completions"
-        if model == "eb-instant":
+        if model in ["eb-instant", "ernie-bot-turbo"]:
             endpoint = "eb-instant"
         return self.WENXIN_CHAT_URL.format(endpoint=endpoint)
 
     def grant_token(self) -> str:
         """Grant access token from Baidu Cloud."""
         now_timestamp = int(time.time())
         if self.access_token and now_timestamp < self.access_token_expires:
@@ -144,29 +144,31 @@
             raise Exception(msg)
 
         return response
 
 
 class BaiduCommon(BaseModel):
     client: Any = None  #: :meta private:
-    model: str = "wenxin"
-    """Model name to use. supported models: wenxin/eb-instant"""
+    model: str = "ernie-bot"
+    """Model name to use. supported models: ernie-bot(wenxin)/ernie-bot-turbo(eb-instant)"""
 
     temperature: Optional[float] = None
-    """A non-negative float that tunes the degree of randomness in generation.
-    range: [0.0, 1.0]."""
+    """A non-negative float that tunes the degree of randomness in generation. Model default is 0.95.
+    range: (0.0, 1.0]."""
 
     penalty_score: Optional[float] = None
     """Repeating punishment involves penalizing already generated tokens to reduce the occurrence of repetition.
     The larger the value, the greater the punishment. Setting it too high can result in poorer text generation
-    for long texts. range: [1.0, 2.0]."""
+    for long texts. Model default is 1.0.
+    range: [1.0, 2.0]."""
 
     top_p: Optional[float] = None
     """Diversity influences the diversity of output text.
-    The larger the value, the stronger the diversity of the generated text. range: [0.0, 1.0]."""
+    The larger the value, the stronger the diversity of the generated text. Model default is 0.8.
+    range: (0.0, 1.0]."""
 
     streaming: bool = False
     """Whether to stream the results."""
 
     request_timeout: Optional[int] = 600
     """Timeout for requests to Baidu Wenxin Completion API. Default is 600 seconds."""
```

### Comparing `langchain_wenxin-0.4.0/.gitignore` & `langchain_wenxin-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.4.0/LICENSE.txt` & `langchain_wenxin-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.4.0/README.md` & `langchain_wenxin-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -27,23 +27,26 @@
 export BAIDU_SECRET_KEY="xxxxx"
 ```
 
 ```python3
 from langchain_wenxin.llms import Wenxin,ChatWenxin
 
 # Wenxin model
-llm = Wenxin(model="eb-instant")
+llm = Wenxin(model="ernie-bot-turbo")
 print(llm("你好"))
 
 # Wenxin chat model
 from langchain.schema import HumanMessage
 llm = ChatWenxin()
 print(llm([HumanMessage(content="你好")]))
 ```
 
 Support models:
-- wenxin: 文心一言
-- eb-instant: 文心 EB-Lite
+
+- ernie-bot: 标准模型，<https://cloud.baidu.com/doc/WENXINWORKSHOP/s/jlil56u11>
+    - Also named `wenxin` for compatibility.
+- ernie-bot-turbo: 快速模型，<https://cloud.baidu.com/doc/WENXINWORKSHOP/s/4lilb2lpf>
+    - Also named `eb-instant` for compatibility.
 
 ## License
 
 `langchain-wenxin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `langchain_wenxin-0.4.0/pyproject.toml` & `langchain_wenxin-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "langchain>=0.0.175",
   "requests",
   "sseclient-py",
+  "numpy",
 ]
 
 [project.urls]
 Documentation = "https://github.com/unknown/langchain-wenxin#readme"
 Issues = "https://github.com/unknown/langchain-wenxin/issues"
 Source = "https://github.com/unknown/langchain-wenxin"
```

### Comparing `langchain_wenxin-0.4.0/PKG-INFO` & `langchain_wenxin-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-wenxin
-Version: 0.4.0
+Version: 0.5.0
 Project-URL: Documentation, https://github.com/unknown/langchain-wenxin#readme
 Project-URL: Issues, https://github.com/unknown/langchain-wenxin/issues
 Project-URL: Source, https://github.com/unknown/langchain-wenxin
 Author-email: Tao Yang <swulling@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: langchain>=0.0.175
+Requires-Dist: numpy
 Requires-Dist: requests
 Requires-Dist: sseclient-py
 Description-Content-Type: text/markdown
 
 # langchain-wenxin - Langchain Baidu WENXINWORKSHOP wrapper
 
 [![PyPI - Version](https://img.shields.io/pypi/v/langchain-wenxin.svg)](https://pypi.org/project/langchain-wenxin)
@@ -51,23 +52,26 @@
 export BAIDU_SECRET_KEY="xxxxx"
 ```
 
 ```python3
 from langchain_wenxin.llms import Wenxin,ChatWenxin
 
 # Wenxin model
-llm = Wenxin(model="eb-instant")
+llm = Wenxin(model="ernie-bot-turbo")
 print(llm("你好"))
 
 # Wenxin chat model
 from langchain.schema import HumanMessage
 llm = ChatWenxin()
 print(llm([HumanMessage(content="你好")]))
 ```
 
 Support models:
-- wenxin: 文心一言
-- eb-instant: 文心 EB-Lite
+
+- ernie-bot: 标准模型，<https://cloud.baidu.com/doc/WENXINWORKSHOP/s/jlil56u11>
+    - Also named `wenxin` for compatibility.
+- ernie-bot-turbo: 快速模型，<https://cloud.baidu.com/doc/WENXINWORKSHOP/s/4lilb2lpf>
+    - Also named `eb-instant` for compatibility.
 
 ## License
 
 `langchain-wenxin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

