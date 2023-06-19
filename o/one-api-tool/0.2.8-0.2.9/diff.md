# Comparing `tmp/one-api-tool-0.2.8.tar.gz` & `tmp/one-api-tool-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.2.8.tar", last modified: Mon Jun 19 07:09:07 2023, max compression
+gzip compressed data, was "one-api-tool-0.2.9.tar", last modified: Mon Jun 19 08:07:50 2023, max compression
```

## Comparing `one-api-tool-0.2.8.tar` & `one-api-tool-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 07:09:07.178517 one-api-tool-0.2.8/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.8/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     3947 2023-06-19 07:09:07.178367 one-api-tool-0.2.8/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     3391 2023-06-05 02:51:55.000000 one-api-tool-0.2.8/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 07:09:07.177041 one-api-tool-0.2.8/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     3947 2023-06-19 07:09:07.000000 one-api-tool-0.2.8/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-06-19 07:09:07.000000 one-api-tool-0.2.8/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-19 07:09:07.000000 one-api-tool-0.2.8/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-06-19 07:09:07.000000 one-api-tool-0.2.8/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-06-19 07:09:07.000000 one-api-tool-0.2.8/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-06-19 07:09:07.000000 one-api-tool-0.2.8/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 07:09:07.177414 one-api-tool-0.2.8/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.2.8/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 07:09:07.177873 one-api-tool-0.2.8/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.8/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-05-04 06:36:39.000000 one-api-tool-0.2.8/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    10251 2023-06-19 07:08:52.000000 one-api-tool-0.2.8/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-19 07:09:07.178569 one-api-tool-0.2.8/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-06-19 07:08:43.000000 one-api-tool-0.2.8/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:07:50.648841 one-api-tool-0.2.9/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.9/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4183 2023-06-19 08:07:50.648695 one-api-tool-0.2.9/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3591 2023-06-19 07:50:24.000000 one-api-tool-0.2.9/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:07:50.647117 one-api-tool-0.2.9/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4183 2023-06-19 08:07:50.000000 one-api-tool-0.2.9/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-06-19 08:07:50.000000 one-api-tool-0.2.9/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-19 08:07:50.000000 one-api-tool-0.2.9/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-06-19 08:07:50.000000 one-api-tool-0.2.9/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-06-19 08:07:50.000000 one-api-tool-0.2.9/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-06-19 08:07:50.000000 one-api-tool-0.2.9/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:07:50.647671 one-api-tool-0.2.9/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.2.9/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:07:50.648145 one-api-tool-0.2.9/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.9/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-05-04 06:36:39.000000 one-api-tool-0.2.9/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    10802 2023-06-19 07:58:57.000000 one-api-tool-0.2.9/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-19 08:07:50.648893 one-api-tool-0.2.9/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-06-19 08:07:38.000000 one-api-tool-0.2.9/setup.py
```

### Comparing `one-api-tool-0.2.8/LICENSE` & `one-api-tool-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.8/PKG-INFO` & `one-api-tool-0.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.8
+Version: 0.2.9
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -22,15 +24,15 @@
 
 ## Installation
 ```sh
 pip install -U one-api-tool
 ```
 
 ## Usage
-### 1. (Recommended method) Set your key information in the local configuration file.
+### 1. Usage with python.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.openai.com/v1",
     "api_type": "open_ai"
@@ -54,29 +56,31 @@
 ```
 `api_key`: Obtain OpenAI API key from the [OpenAI website](https://platform.openai.com/account/api-keys) and Claude API key from the [Anthropic website](https://console.anthropic.com/account/keys).
 
 `api`: The base API used to send requests. You may also specify a proxy URL like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard. The API format is usually: `https://{your_organization}.openai.azure.com/`.
 
 `api_type`: Currently supported values are "open_ai", "azure", or "claude".
 
-Initialize the `OneAPITool` object from a local configuration file:
+Initialize the `OneAPITool` object from configuration:
 ```python
 from oneapi import OneAPITool
-res = OneAPITool.from_config_file("your_config_file.json").simple_chat("Hello AI!")
+# Two ways to initialize the OneAPITool object  
+# tool = OneAPITool.from_config(api_key, api, api_type)
+tool = OneAPITool.from_config_file("your_config_file.json")
+# Say hello to ChatGPT/Claude/GPT-4
+res = tool.simple_chat("Hello AI!")
 print(res)
+# Get embeddings of some sentences for further usage
+embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
+print(embeddings.shape)
+# Count the number of tokens
+print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
-
-### 2. (Not recommended) Write the configuration directly into the code
-```python
-from oneapi import OneAPITool
-res = OneAPITool.from_config(api_key, api, api_type).simple_chat("Hello AI!")
-print(res)
-```
-
-### 3. Usage with command line
+**Note: Currently, `count_tokens` and `get_embeddings` only support OpenAI or Microsoft Azure API.**
+### 2. Usage with command line
 ```sh
 open-api --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "1+1=?" 
 ```
 <details open><summary>Output detail</summary>
 
@@ -111,7 +115,8 @@
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ## ToDo
 - [ ] Batch requests.
 - [ ] Token number counting.
 - [ ] Custom token budget.
+
```

### Comparing `one-api-tool-0.2.8/README.md` & `one-api-tool-0.2.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ## Installation
 ```sh
 pip install -U one-api-tool
 ```
 
 ## Usage
-### 1. (Recommended method) Set your key information in the local configuration file.
+### 1. Usage with python.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.openai.com/v1",
     "api_type": "open_ai"
@@ -42,29 +42,31 @@
 ```
 `api_key`: Obtain OpenAI API key from the [OpenAI website](https://platform.openai.com/account/api-keys) and Claude API key from the [Anthropic website](https://console.anthropic.com/account/keys).
 
 `api`: The base API used to send requests. You may also specify a proxy URL like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard. The API format is usually: `https://{your_organization}.openai.azure.com/`.
 
 `api_type`: Currently supported values are "open_ai", "azure", or "claude".
 
-Initialize the `OneAPITool` object from a local configuration file:
+Initialize the `OneAPITool` object from configuration:
 ```python
 from oneapi import OneAPITool
-res = OneAPITool.from_config_file("your_config_file.json").simple_chat("Hello AI!")
+# Two ways to initialize the OneAPITool object  
+# tool = OneAPITool.from_config(api_key, api, api_type)
+tool = OneAPITool.from_config_file("your_config_file.json")
+# Say hello to ChatGPT/Claude/GPT-4
+res = tool.simple_chat("Hello AI!")
 print(res)
+# Get embeddings of some sentences for further usage
+embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
+print(embeddings.shape)
+# Count the number of tokens
+print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
-
-### 2. (Not recommended) Write the configuration directly into the code
-```python
-from oneapi import OneAPITool
-res = OneAPITool.from_config(api_key, api, api_type).simple_chat("Hello AI!")
-print(res)
-```
-
-### 3. Usage with command line
+**Note: Currently, `count_tokens` and `get_embeddings` only support OpenAI or Microsoft Azure API.**
+### 2. Usage with command line
 ```sh
 open-api --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "1+1=?" 
 ```
 <details open><summary>Output detail</summary>
```

### Comparing `one-api-tool-0.2.8/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.2.9/one_api_tool.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.8
+Version: 0.2.9
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -22,15 +24,15 @@
 
 ## Installation
 ```sh
 pip install -U one-api-tool
 ```
 
 ## Usage
-### 1. (Recommended method) Set your key information in the local configuration file.
+### 1. Usage with python.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.openai.com/v1",
     "api_type": "open_ai"
@@ -54,29 +56,31 @@
 ```
 `api_key`: Obtain OpenAI API key from the [OpenAI website](https://platform.openai.com/account/api-keys) and Claude API key from the [Anthropic website](https://console.anthropic.com/account/keys).
 
 `api`: The base API used to send requests. You may also specify a proxy URL like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard. The API format is usually: `https://{your_organization}.openai.azure.com/`.
 
 `api_type`: Currently supported values are "open_ai", "azure", or "claude".
 
-Initialize the `OneAPITool` object from a local configuration file:
+Initialize the `OneAPITool` object from configuration:
 ```python
 from oneapi import OneAPITool
-res = OneAPITool.from_config_file("your_config_file.json").simple_chat("Hello AI!")
+# Two ways to initialize the OneAPITool object  
+# tool = OneAPITool.from_config(api_key, api, api_type)
+tool = OneAPITool.from_config_file("your_config_file.json")
+# Say hello to ChatGPT/Claude/GPT-4
+res = tool.simple_chat("Hello AI!")
 print(res)
+# Get embeddings of some sentences for further usage
+embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
+print(embeddings.shape)
+# Count the number of tokens
+print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
-
-### 2. (Not recommended) Write the configuration directly into the code
-```python
-from oneapi import OneAPITool
-res = OneAPITool.from_config(api_key, api, api_type).simple_chat("Hello AI!")
-print(res)
-```
-
-### 3. Usage with command line
+**Note: Currently, `count_tokens` and `get_embeddings` only support OpenAI or Microsoft Azure API.**
+### 2. Usage with command line
 ```sh
 open-api --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "1+1=?" 
 ```
 <details open><summary>Output detail</summary>
 
@@ -111,7 +115,8 @@
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ## ToDo
 - [ ] Batch requests.
 - [ ] Token number counting.
 - [ ] Custom token budget.
+
```

### Comparing `one-api-tool-0.2.8/oneapi/commands/one_api_requst.py` & `one-api-tool-0.2.9/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.8/oneapi/one_api.py` & `one-api-tool-0.2.9/oneapi/one_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -99,14 +99,15 @@
         raise NotImplementedError
         
 
 class OpenAITool(AbstractAPITool):
 
     def __init__(self,method : AbstrctMethod) -> None:
         self.method = method
+        self.encoder = None
         if isinstance(self.method, AzureMethod):
             openai.api_key = self.method.api_key
             openai.api_base = self.method.api_base
             openai.api_type = self.method.api_type
             openai.api_version = self.method.api_version
         else:
             openai.api_key = self.method.api_key
@@ -133,47 +134,44 @@
                 collected_messages.append(chunk_message)  # save the message
             full_reply_content = "".join([m.get("content", "") for m in collected_messages])
             return full_reply_content
         else:
             return completion.choices[0].message.get("content", "")
 
 
-    def get_embeddings(self, list_of_text: List[str], engine="text-embedding-ada-002") -> List[List[float]]:
-        assert len(list_of_text) <= 2048, "The batch size should not be larger than 2048."
-        openai.api_key = self.method.api_key
+    def get_embeddings(self, texts: List[str], engine="text-embedding-ada-002") -> List[List[float]]:
+        assert len(texts) <= 2048, "The batch size should not be larger than 2048."
         # replace newlines, which can negatively affect performance.
-        list_of_text = [text.replace("\n", " ") for text in list_of_text]
+        texts = [text.replace("\n", " ") for text in texts]
 
-        data = openai.Embedding.create(input=list_of_text, engine=engine).data
+        data = openai.Embedding.create(input=texts, engine=engine).data
         data = sorted(data, key=lambda x: x["index"])  # maintain the same order as input.
         return [d["embedding"] for d in data]
 
 
     def get_embedding(self, text: str, engine="text-embedding-ada-002") -> List[float]:
-        openai.api_key = self.method.api_key
         # replace newlines, which can negatively affect performance.
         text = text.replace("\n", " ")
-
         return openai.Embedding.create(input=[text], engine=engine)["data"][0]["embedding"]
 
-    @staticmethod
-    def count_tokens(list_of_text: List[str], encoding_name: str = 'cl100k_base') -> int:
+    def count_tokens(self, texts: List[str], encoding_name: str = 'cl100k_base') -> int:
         """
         Encoding name	OpenAI models
         cl100k_base	    gpt-4, gpt-3.5-turbo, text-embedding-ada-002
         p50k_base	    Codex models, text-davinci-002, text-davinci-003
         r50k_base (or gpt2)	GPT-3 models like davinci
         Args:
-            list_of_text (List[str]): [description]
+            texts (List[str]): [description]
             encoding_name (str, optional): Defaults to 'cl100k_base'.
         Returns:
             int: [description]
         """
-        encoder = tiktoken.get_encoding(encoding_name)
-        list_of_tokens = encoder.encode_batch(list_of_text)
+        if self.encoder is None:
+            self.encoder = tiktoken.get_encoding(encoding_name)
+        list_of_tokens = self.encoder.encode_batch(texts)
         return sum([len(tokens) for tokens in list_of_tokens])
 
 
 
 class ClaudeAITool(AbstractAPITool):
     """
     https://console.anthropic.com/claude
@@ -251,8 +249,20 @@
                 args = OpenAIDecodingArguments(messages=msgs, model=model if model else "gpt-3.5-turbo", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
         elif isinstance(self.tool, ClaudeAITool):
             args = ClaudeDecodingArguments(prompt=f"\n\nHuman: {prompt}\n\nAssistant:", model=model if model else "claude-v1.3", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
         else:
             raise AssertionError(f"Not supported api type: {type(self.tool)}")
 
         response = self.tool.simple_chat(args)
-        return response
+        return response
+
+    def get_embeddings(self, texts: List[str], engine="text-embedding-ada-002") -> List[List[float]]:
+        if isinstance(self.tool, OpenAITool):
+            return self.tool.get_embeddings(texts, engine)  
+        else:
+            raise AssertionError(f"Not supported api type for embeddings: {type(self.tool)}")
+    
+    def count_tokens(self, texts: List[str], encoding_name: str = 'cl100k_base') -> int:
+        if isinstance(self.tool, OpenAITool):
+            return self.tool.count_tokens(texts, encoding_name)
+        else:
+            raise AssertionError(f"Not supported api type for token counting: {type(self.tool)}")
```

### Comparing `one-api-tool-0.2.8/setup.py` & `one-api-tool-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.2.8",
+    version="0.2.9",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

