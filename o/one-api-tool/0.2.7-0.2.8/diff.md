# Comparing `tmp/one-api-tool-0.2.7.tar.gz` & `tmp/one-api-tool-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.2.7.tar", last modified: Fri Apr 28 08:45:55 2023, max compression
+gzip compressed data, was "one-api-tool-0.2.8.tar", last modified: Mon Jun 19 07:09:07 2023, max compression
```

## Comparing `one-api-tool-0.2.7.tar` & `one-api-tool-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:45:55.401738 one-api-tool-0.2.7/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.7/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     2298 2023-04-28 08:45:55.401589 one-api-tool-0.2.7/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     1742 2023-04-27 13:04:23.000000 one-api-tool-0.2.7/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:45:55.400317 one-api-tool-0.2.7/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     2298 2023-04-28 08:45:55.000000 one-api-tool-0.2.7/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-04-28 08:45:55.000000 one-api-tool-0.2.7/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-28 08:45:55.000000 one-api-tool-0.2.7/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-04-28 08:45:55.000000 one-api-tool-0.2.7/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       60 2023-04-28 08:45:55.000000 one-api-tool-0.2.7/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-28 08:45:55.000000 one-api-tool-0.2.7/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:45:55.400718 one-api-tool-0.2.7/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.2.7/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:45:55.401205 one-api-tool-0.2.7/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.7/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-04-27 08:57:27.000000 one-api-tool-0.2.7/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     9512 2023-04-26 11:27:45.000000 one-api-tool-0.2.7/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-28 08:45:55.401787 one-api-tool-0.2.7/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1031 2023-04-28 08:45:48.000000 one-api-tool-0.2.7/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 07:09:07.178517 one-api-tool-0.2.8/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.8/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3947 2023-06-19 07:09:07.178367 one-api-tool-0.2.8/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3391 2023-06-05 02:51:55.000000 one-api-tool-0.2.8/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 07:09:07.177041 one-api-tool-0.2.8/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3947 2023-06-19 07:09:07.000000 one-api-tool-0.2.8/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-06-19 07:09:07.000000 one-api-tool-0.2.8/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-19 07:09:07.000000 one-api-tool-0.2.8/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-06-19 07:09:07.000000 one-api-tool-0.2.8/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-06-19 07:09:07.000000 one-api-tool-0.2.8/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-06-19 07:09:07.000000 one-api-tool-0.2.8/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 07:09:07.177414 one-api-tool-0.2.8/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.2.8/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 07:09:07.177873 one-api-tool-0.2.8/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.8/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-05-04 06:36:39.000000 one-api-tool-0.2.8/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    10251 2023-06-19 07:08:52.000000 one-api-tool-0.2.8/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-19 07:09:07.178569 one-api-tool-0.2.8/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-06-19 07:08:43.000000 one-api-tool-0.2.8/setup.py
```

### Comparing `one-api-tool-0.2.7/LICENSE` & `one-api-tool-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.7/oneapi/commands/one_api_requst.py` & `one-api-tool-0.2.8/oneapi/commands/one_api_requst.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                         required=True)
     parser.add_argument("-m",
                         "--model",
                         type=str,
                         default="",
                         help="evaluate model name, e.g., gpt-35-turbo, gpt-4",
                         required=False)
-    parser.add_argument("-tt",
+    parser.add_argument("-te",
                         "--temperature",
                         type=float,
                         default=0.1,
                         help="0-1, higher temperature more random result",
                         required=False)
     parser.add_argument("-mnt",
                         "--max_new_tokens",
```

### Comparing `one-api-tool-0.2.7/oneapi/one_api.py` & `one-api-tool-0.2.8/oneapi/one_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 from typing import Optional, Sequence, List
 import openai
 import anthropic
 from pydantic import BaseModel
 from abc import ABC, abstractmethod
 import sys
 import os
+import tiktoken
 sys.path.append(os.path.normpath(f"{os.path.dirname(os.path.abspath(__file__))}/.."))
 
-CLAUDE_TEMPLATE = "\n\nHuman: {prompt}\n\nAssistant: "
+CLAUDE_TEMPLATE = "\n\nHuman: {prompt}\n\nAssistant:"
 
 class ChatGPTMessage(BaseModel):
     role: str
     content: str
     
 class AbstrctMethod(BaseModel):
     api_key: str
@@ -150,14 +151,30 @@
     def get_embedding(self, text: str, engine="text-embedding-ada-002") -> List[float]:
         openai.api_key = self.method.api_key
         # replace newlines, which can negatively affect performance.
         text = text.replace("\n", " ")
 
         return openai.Embedding.create(input=[text], engine=engine)["data"][0]["embedding"]
 
+    @staticmethod
+    def count_tokens(list_of_text: List[str], encoding_name: str = 'cl100k_base') -> int:
+        """
+        Encoding name	OpenAI models
+        cl100k_base	    gpt-4, gpt-3.5-turbo, text-embedding-ada-002
+        p50k_base	    Codex models, text-davinci-002, text-davinci-003
+        r50k_base (or gpt2)	GPT-3 models like davinci
+        Args:
+            list_of_text (List[str]): [description]
+            encoding_name (str, optional): Defaults to 'cl100k_base'.
+        Returns:
+            int: [description]
+        """
+        encoder = tiktoken.get_encoding(encoding_name)
+        list_of_tokens = encoder.encode_batch(list_of_text)
+        return sum([len(tokens) for tokens in list_of_tokens])
 
 
 
 class ClaudeAITool(AbstractAPITool):
     """
     https://console.anthropic.com/claude
     https://github.com/anthropics/anthropic-sdk-python/blob/main/examples/basic_stream.py
```

### Comparing `one-api-tool-0.2.7/setup.py` & `one-api-tool-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.2.7",
+    version="0.2.8",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
         "httpx",
         "aiohttp",
+        "tiktoken",
         "tokenizers",
     ],
     entry_points={
         "console_scripts": [
             "one-api=oneapi.commands.one_api_requst:main"
         ]
     },
```

