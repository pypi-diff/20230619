# Comparing `tmp/one-api-tool-0.2.9.tar.gz` & `tmp/one-api-tool-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.2.9.tar", last modified: Mon Jun 19 08:07:50 2023, max compression
+gzip compressed data, was "one-api-tool-0.3.0.tar", last modified: Mon Jun 19 08:27:18 2023, max compression
```

## Comparing `one-api-tool-0.2.9.tar` & `one-api-tool-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:07:50.648841 one-api-tool-0.2.9/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.9/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     4183 2023-06-19 08:07:50.648695 one-api-tool-0.2.9/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     3591 2023-06-19 07:50:24.000000 one-api-tool-0.2.9/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:07:50.647117 one-api-tool-0.2.9/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     4183 2023-06-19 08:07:50.000000 one-api-tool-0.2.9/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-06-19 08:07:50.000000 one-api-tool-0.2.9/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-19 08:07:50.000000 one-api-tool-0.2.9/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-06-19 08:07:50.000000 one-api-tool-0.2.9/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-06-19 08:07:50.000000 one-api-tool-0.2.9/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-06-19 08:07:50.000000 one-api-tool-0.2.9/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:07:50.647671 one-api-tool-0.2.9/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.2.9/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:07:50.648145 one-api-tool-0.2.9/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.9/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-05-04 06:36:39.000000 one-api-tool-0.2.9/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    10802 2023-06-19 07:58:57.000000 one-api-tool-0.2.9/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-19 08:07:50.648893 one-api-tool-0.2.9/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-06-19 08:07:38.000000 one-api-tool-0.2.9/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:27:18.830935 one-api-tool-0.3.0/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.3.0/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4172 2023-06-19 08:27:18.829641 one-api-tool-0.3.0/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3616 2023-06-19 08:21:43.000000 one-api-tool-0.3.0/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:27:18.828302 one-api-tool-0.3.0/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4172 2023-06-19 08:27:18.000000 one-api-tool-0.3.0/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-06-19 08:27:18.000000 one-api-tool-0.3.0/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-19 08:27:18.000000 one-api-tool-0.3.0/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-06-19 08:27:18.000000 one-api-tool-0.3.0/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-06-19 08:27:18.000000 one-api-tool-0.3.0/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-06-19 08:27:18.000000 one-api-tool-0.3.0/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:27:18.828872 one-api-tool-0.3.0/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.3.0/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:27:18.829250 one-api-tool-0.3.0/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.3.0/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-05-04 06:36:39.000000 one-api-tool-0.3.0/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    10837 2023-06-19 08:24:27.000000 one-api-tool-0.3.0/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-19 08:27:18.831198 one-api-tool-0.3.0/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-06-19 08:27:05.000000 one-api-tool-0.3.0/setup.py
```

### Comparing `one-api-tool-0.2.9/LICENSE` & `one-api-tool-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.9/PKG-INFO` & `one-api-tool-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.9
+Version: 0.3.0
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -30,45 +28,45 @@
 ## Usage
 ### 1. Usage with python.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "https://api.openai.com/v1",
+    "api_base": "https://api.openai.com/v1",
     "api_type": "open_ai"
 }
 ```
 Azure OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "Replace with your Azure OpenAI resource's endpoint value.",
+    "api_base": "Replace with your Azure OpenAI resource's endpoint value.",
     "api_type": "azure"
 }
 ```
 Anthropic config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "https://api.anthropic.com",
+    "api_base": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 `api_key`: Obtain OpenAI API key from the [OpenAI website](https://platform.openai.com/account/api-keys) and Claude API key from the [Anthropic website](https://console.anthropic.com/account/keys).
 
-`api`: The base API used to send requests. You may also specify a proxy URL like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard. The API format is usually: `https://{your_organization}.openai.azure.com/`.
+`api_base`: The base API used to send requests. You may also specify a proxy URL like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard. The API format is usually: `https://{your_organization}.openai.azure.com/`.
 
 `api_type`: Currently supported values are "open_ai", "azure", or "claude".
 
 Initialize the `OneAPITool` object from configuration:
 ```python
 from oneapi import OneAPITool
 # Two ways to initialize the OneAPITool object  
-# tool = OneAPITool.from_config(api_key, api, api_type)
+# tool = OneAPITool.from_config(api_key, api_base, api_type)
 tool = OneAPITool.from_config_file("your_config_file.json")
 # Say hello to ChatGPT/Claude/GPT-4
 res = tool.simple_chat("Hello AI!")
 print(res)
 # Get embeddings of some sentences for further usage
 embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
 print(embeddings.shape)
@@ -115,8 +113,7 @@
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ## ToDo
 - [ ] Batch requests.
 - [ ] Token number counting.
 - [ ] Custom token budget.
-
```

### Comparing `one-api-tool-0.2.9/README.md` & `one-api-tool-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,45 +16,45 @@
 ## Usage
 ### 1. Usage with python.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "https://api.openai.com/v1",
+    "api_base": "https://api.openai.com/v1",
     "api_type": "open_ai"
 }
 ```
 Azure OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "Replace with your Azure OpenAI resource's endpoint value.",
+    "api_base": "Replace with your Azure OpenAI resource's endpoint value.",
     "api_type": "azure"
 }
 ```
 Anthropic config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "https://api.anthropic.com",
+    "api_base": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 `api_key`: Obtain OpenAI API key from the [OpenAI website](https://platform.openai.com/account/api-keys) and Claude API key from the [Anthropic website](https://console.anthropic.com/account/keys).
 
-`api`: The base API used to send requests. You may also specify a proxy URL like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard. The API format is usually: `https://{your_organization}.openai.azure.com/`.
+`api_base`: The base API used to send requests. You may also specify a proxy URL like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard. The API format is usually: `https://{your_organization}.openai.azure.com/`.
 
 `api_type`: Currently supported values are "open_ai", "azure", or "claude".
 
 Initialize the `OneAPITool` object from configuration:
 ```python
 from oneapi import OneAPITool
 # Two ways to initialize the OneAPITool object  
-# tool = OneAPITool.from_config(api_key, api, api_type)
+# tool = OneAPITool.from_config(api_key, api_base, api_type)
 tool = OneAPITool.from_config_file("your_config_file.json")
 # Say hello to ChatGPT/Claude/GPT-4
 res = tool.simple_chat("Hello AI!")
 print(res)
 # Get embeddings of some sentences for further usage
 embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
 print(embeddings.shape)
```

### Comparing `one-api-tool-0.2.9/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.3.0/one_api_tool.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.9
+Version: 0.3.0
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -30,45 +28,45 @@
 ## Usage
 ### 1. Usage with python.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "https://api.openai.com/v1",
+    "api_base": "https://api.openai.com/v1",
     "api_type": "open_ai"
 }
 ```
 Azure OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "Replace with your Azure OpenAI resource's endpoint value.",
+    "api_base": "Replace with your Azure OpenAI resource's endpoint value.",
     "api_type": "azure"
 }
 ```
 Anthropic config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "https://api.anthropic.com",
+    "api_base": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 `api_key`: Obtain OpenAI API key from the [OpenAI website](https://platform.openai.com/account/api-keys) and Claude API key from the [Anthropic website](https://console.anthropic.com/account/keys).
 
-`api`: The base API used to send requests. You may also specify a proxy URL like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard. The API format is usually: `https://{your_organization}.openai.azure.com/`.
+`api_base`: The base API used to send requests. You may also specify a proxy URL like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard. The API format is usually: `https://{your_organization}.openai.azure.com/`.
 
 `api_type`: Currently supported values are "open_ai", "azure", or "claude".
 
 Initialize the `OneAPITool` object from configuration:
 ```python
 from oneapi import OneAPITool
 # Two ways to initialize the OneAPITool object  
-# tool = OneAPITool.from_config(api_key, api, api_type)
+# tool = OneAPITool.from_config(api_key, api_base, api_type)
 tool = OneAPITool.from_config_file("your_config_file.json")
 # Say hello to ChatGPT/Claude/GPT-4
 res = tool.simple_chat("Hello AI!")
 print(res)
 # Get embeddings of some sentences for further usage
 embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
 print(embeddings.shape)
@@ -115,8 +113,7 @@
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ## ToDo
 - [ ] Batch requests.
 - [ ] Token number counting.
 - [ ] Custom token budget.
-
```

### Comparing `one-api-tool-0.2.9/oneapi/commands/one_api_requst.py` & `one-api-tool-0.3.0/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.9/oneapi/one_api.py` & `one-api-tool-0.3.0/oneapi/one_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,30 +211,30 @@
 
     @classmethod
     def from_config_file(cls, config_file):
         config = cls.load_json(config_file)
         api_type = config.get("api_type")
 
         if api_type == "claude":
-            return cls(ClaudeAITool(ClaudeMethod(api_key=config["api_key"], api_base=config["api"])))
+            return cls(ClaudeAITool(ClaudeMethod(api_key=config["api_key"], api_base=config["api_base"])))
         elif api_type == "azure":
-            return cls(OpenAITool(AzureMethod(api_key=config["api_key"], api_base=config["api"])))
+            return cls(OpenAITool(AzureMethod(api_key=config["api_key"], api_base=config["api_base"])))
         elif api_type == "open_ai":
-            return cls(OpenAITool(OpenAIMethod(api_key=config["api_key"], api_base=config["api"])))
+            return cls(OpenAITool(OpenAIMethod(api_key=config["api_key"], api_base=config["api_base"])))
         else:
             raise AssertionError(f"Couldn\'t find API type in config file: {config_file}. Please specify \"api_type\" as \"claude\", \"azure\", or \"open_ai\".")
 
     @classmethod
-    def from_config(cls, api_key, api, api_type):
+    def from_config(cls, api_key, api_base, api_type):
         if api_type == "claude":
-            return cls(ClaudeAITool(ClaudeMethod(api_key=api_key, api_base=api)))
+            return cls(ClaudeAITool(ClaudeMethod(api_key=api_key, api_base=api_base)))
         elif api_type == "azure":
-            return cls(OpenAITool(AzureMethod(api_key=api_key, api_base=api)))
+            return cls(OpenAITool(AzureMethod(api_key=api_key, api_base=api_base)))
         elif api_type == "open_ai":
-            return cls(OpenAITool(OpenAIMethod(api_key=api_key, api_base=api)))
+            return cls(OpenAITool(OpenAIMethod(api_key=api_key, api_base=api_base)))
         else:
             raise AssertionError(f"Couldn\'t find API type: {api_type}. Please specify \"api_type\" as \"claude\", \"azure\", or \"open_ai\".")
 
 
     @staticmethod
     def load_json(file_path):
         with open(file_path, "r") as f:
```

### Comparing `one-api-tool-0.2.9/setup.py` & `one-api-tool-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.2.9",
+    version="0.3.0",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

