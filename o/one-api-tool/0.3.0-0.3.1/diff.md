# Comparing `tmp/one-api-tool-0.3.0.tar.gz` & `tmp/one-api-tool-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.3.0.tar", last modified: Mon Jun 19 08:27:18 2023, max compression
+gzip compressed data, was "one-api-tool-0.3.1.tar", last modified: Mon Jun 19 08:40:01 2023, max compression
```

## Comparing `one-api-tool-0.3.0.tar` & `one-api-tool-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:27:18.830935 one-api-tool-0.3.0/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.3.0/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     4172 2023-06-19 08:27:18.829641 one-api-tool-0.3.0/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     3616 2023-06-19 08:21:43.000000 one-api-tool-0.3.0/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:27:18.828302 one-api-tool-0.3.0/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     4172 2023-06-19 08:27:18.000000 one-api-tool-0.3.0/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-06-19 08:27:18.000000 one-api-tool-0.3.0/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-19 08:27:18.000000 one-api-tool-0.3.0/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-06-19 08:27:18.000000 one-api-tool-0.3.0/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-06-19 08:27:18.000000 one-api-tool-0.3.0/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-06-19 08:27:18.000000 one-api-tool-0.3.0/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:27:18.828872 one-api-tool-0.3.0/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.3.0/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:27:18.829250 one-api-tool-0.3.0/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.3.0/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-05-04 06:36:39.000000 one-api-tool-0.3.0/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    10837 2023-06-19 08:24:27.000000 one-api-tool-0.3.0/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-19 08:27:18.831198 one-api-tool-0.3.0/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-06-19 08:27:05.000000 one-api-tool-0.3.0/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:40:01.841620 one-api-tool-0.3.1/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.3.1/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4256 2023-06-19 08:40:01.841460 one-api-tool-0.3.1/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3700 2023-06-19 08:36:57.000000 one-api-tool-0.3.1/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:40:01.840786 one-api-tool-0.3.1/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4256 2023-06-19 08:40:01.000000 one-api-tool-0.3.1/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-06-19 08:40:01.000000 one-api-tool-0.3.1/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-19 08:40:01.000000 one-api-tool-0.3.1/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-06-19 08:40:01.000000 one-api-tool-0.3.1/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-06-19 08:40:01.000000 one-api-tool-0.3.1/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-06-19 08:40:01.000000 one-api-tool-0.3.1/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:40:01.841026 one-api-tool-0.3.1/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.3.1/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 08:40:01.841252 one-api-tool-0.3.1/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.3.1/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-05-04 06:36:39.000000 one-api-tool-0.3.1/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    10837 2023-06-19 08:24:27.000000 one-api-tool-0.3.1/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-19 08:40:01.841668 one-api-tool-0.3.1/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-06-19 08:39:54.000000 one-api-tool-0.3.1/setup.py
```

### Comparing `one-api-tool-0.3.0/LICENSE` & `one-api-tool-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.0/PKG-INFO` & `one-api-tool-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.3.0
+Version: 0.3.1
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -22,15 +22,15 @@
 
 ## Installation
 ```sh
 pip install -U one-api-tool
 ```
 
 ## Usage
-### 1. Usage with python.
+### 1. Using python.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
     "api_base": "https://api.openai.com/v1",
     "api_type": "open_ai"
@@ -50,19 +50,21 @@
     "api_key": "YOUR_API_KEY",
     "api_base": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 `api_key`: Obtain OpenAI API key from the [OpenAI website](https://platform.openai.com/account/api-keys) and Claude API key from the [Anthropic website](https://console.anthropic.com/account/keys).
 
-`api_base`: The base API used to send requests. You may also specify a proxy URL like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard. The API format is usually: `https://{your_organization}.openai.azure.com/`.
+`api_base`: This is the base API that is used to send requests. You can also specify a proxy URL, such as "https://your_proxy_domain/v1". For example, you can use Cloudflare workers to proxy the OpenAI site.
+
+If you are using Azure APIs, you can find relevant information on the Azure resource dashboard. The API format typically follows this pattern: `https://{your_organization}.openai.azure.com/`.
 
 `api_type`: Currently supported values are "open_ai", "azure", or "claude".
 
-Initialize the `OneAPITool` object from configuration:
+Here is a simple example:
 ```python
 from oneapi import OneAPITool
 # Two ways to initialize the OneAPITool object  
 # tool = OneAPITool.from_config(api_key, api_base, api_type)
 tool = OneAPITool.from_config_file("your_config_file.json")
 # Say hello to ChatGPT/Claude/GPT-4
 res = tool.simple_chat("Hello AI!")
@@ -70,15 +72,15 @@
 # Get embeddings of some sentences for further usage
 embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
 print(embeddings.shape)
 # Count the number of tokens
 print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
 **Note: Currently, `count_tokens` and `get_embeddings` only support OpenAI or Microsoft Azure API.**
-### 2. Usage with command line
+### 2. Using command line
 ```sh
 open-api --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "1+1=?" 
 ```
 <details open><summary>Output detail</summary>
```

### Comparing `one-api-tool-0.3.0/README.md` & `one-api-tool-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ## Installation
 ```sh
 pip install -U one-api-tool
 ```
 
 ## Usage
-### 1. Usage with python.
+### 1. Using python.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
     "api_base": "https://api.openai.com/v1",
     "api_type": "open_ai"
@@ -38,19 +38,21 @@
     "api_key": "YOUR_API_KEY",
     "api_base": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 `api_key`: Obtain OpenAI API key from the [OpenAI website](https://platform.openai.com/account/api-keys) and Claude API key from the [Anthropic website](https://console.anthropic.com/account/keys).
 
-`api_base`: The base API used to send requests. You may also specify a proxy URL like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard. The API format is usually: `https://{your_organization}.openai.azure.com/`.
+`api_base`: This is the base API that is used to send requests. You can also specify a proxy URL, such as "https://your_proxy_domain/v1". For example, you can use Cloudflare workers to proxy the OpenAI site.
+
+If you are using Azure APIs, you can find relevant information on the Azure resource dashboard. The API format typically follows this pattern: `https://{your_organization}.openai.azure.com/`.
 
 `api_type`: Currently supported values are "open_ai", "azure", or "claude".
 
-Initialize the `OneAPITool` object from configuration:
+Here is a simple example:
 ```python
 from oneapi import OneAPITool
 # Two ways to initialize the OneAPITool object  
 # tool = OneAPITool.from_config(api_key, api_base, api_type)
 tool = OneAPITool.from_config_file("your_config_file.json")
 # Say hello to ChatGPT/Claude/GPT-4
 res = tool.simple_chat("Hello AI!")
@@ -58,15 +60,15 @@
 # Get embeddings of some sentences for further usage
 embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
 print(embeddings.shape)
 # Count the number of tokens
 print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
 **Note: Currently, `count_tokens` and `get_embeddings` only support OpenAI or Microsoft Azure API.**
-### 2. Usage with command line
+### 2. Using command line
 ```sh
 open-api --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "1+1=?" 
 ```
 <details open><summary>Output detail</summary>
```

### Comparing `one-api-tool-0.3.0/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.3.1/one_api_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.3.0
+Version: 0.3.1
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -22,15 +22,15 @@
 
 ## Installation
 ```sh
 pip install -U one-api-tool
 ```
 
 ## Usage
-### 1. Usage with python.
+### 1. Using python.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
     "api_base": "https://api.openai.com/v1",
     "api_type": "open_ai"
@@ -50,19 +50,21 @@
     "api_key": "YOUR_API_KEY",
     "api_base": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 `api_key`: Obtain OpenAI API key from the [OpenAI website](https://platform.openai.com/account/api-keys) and Claude API key from the [Anthropic website](https://console.anthropic.com/account/keys).
 
-`api_base`: The base API used to send requests. You may also specify a proxy URL like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard. The API format is usually: `https://{your_organization}.openai.azure.com/`.
+`api_base`: This is the base API that is used to send requests. You can also specify a proxy URL, such as "https://your_proxy_domain/v1". For example, you can use Cloudflare workers to proxy the OpenAI site.
+
+If you are using Azure APIs, you can find relevant information on the Azure resource dashboard. The API format typically follows this pattern: `https://{your_organization}.openai.azure.com/`.
 
 `api_type`: Currently supported values are "open_ai", "azure", or "claude".
 
-Initialize the `OneAPITool` object from configuration:
+Here is a simple example:
 ```python
 from oneapi import OneAPITool
 # Two ways to initialize the OneAPITool object  
 # tool = OneAPITool.from_config(api_key, api_base, api_type)
 tool = OneAPITool.from_config_file("your_config_file.json")
 # Say hello to ChatGPT/Claude/GPT-4
 res = tool.simple_chat("Hello AI!")
@@ -70,15 +72,15 @@
 # Get embeddings of some sentences for further usage
 embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
 print(embeddings.shape)
 # Count the number of tokens
 print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
 **Note: Currently, `count_tokens` and `get_embeddings` only support OpenAI or Microsoft Azure API.**
-### 2. Usage with command line
+### 2. Using command line
 ```sh
 open-api --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "1+1=?" 
 ```
 <details open><summary>Output detail</summary>
```

### Comparing `one-api-tool-0.3.0/oneapi/commands/one_api_requst.py` & `one-api-tool-0.3.1/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.0/oneapi/one_api.py` & `one-api-tool-0.3.1/oneapi/one_api.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.0/setup.py` & `one-api-tool-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.3.0",
+    version="0.3.1",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

