# Comparing `tmp/simpleaichat-0.1.1.tar.gz` & `tmp/simpleaichat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleaichat-0.1.1.tar", last modified: Fri Jun  9 04:06:19 2023, max compression
+gzip compressed data, was "simpleaichat-0.2.0.tar", last modified: Mon Jun 19 02:40:51 2023, max compression
```

## Comparing `simpleaichat-0.1.1.tar` & `simpleaichat-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-09 04:06:19.235172 simpleaichat-0.1.1/
--rw-r--r--   0 root         (0) staff       (20)     1066 2023-02-18 01:00:20.000000 simpleaichat-0.1.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)    15867 2023-06-09 04:06:19.234935 simpleaichat-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)    15430 2023-06-08 14:46:39.000000 simpleaichat-0.1.1/README.md
--rw-r--r--   0 root         (0) staff       (20)       38 2023-06-09 04:06:19.235248 simpleaichat-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      972 2023-06-09 04:05:24.000000 simpleaichat-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-09 04:06:19.232926 simpleaichat-0.1.1/simpleaichat/
--rw-r--r--   0 root         (0) staff       (20)       46 2023-06-05 04:46:22.000000 simpleaichat-0.1.1/simpleaichat/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    11175 2023-06-08 02:34:09.000000 simpleaichat-0.1.1/simpleaichat/chatgpt.py
--rw-r--r--   0 root         (0) staff       (20)      549 2023-06-08 03:28:41.000000 simpleaichat-0.1.1/simpleaichat/cli.py
--rw-r--r--   0 root         (0) staff       (20)     3052 2023-06-03 05:30:50.000000 simpleaichat-0.1.1/simpleaichat/models.py
--rw-r--r--   0 root         (0) staff       (20)    12175 2023-06-08 01:27:02.000000 simpleaichat-0.1.1/simpleaichat/simpleaichat.py
--rw-r--r--   0 root         (0) staff       (20)     2364 2023-06-03 03:44:43.000000 simpleaichat-0.1.1/simpleaichat/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-09 04:06:19.234612 simpleaichat-0.1.1/simpleaichat.egg-info/
--rw-r--r--   0 root         (0) staff       (20)    15867 2023-06-09 04:06:18.000000 simpleaichat-0.1.1/simpleaichat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      387 2023-06-09 04:06:19.000000 simpleaichat-0.1.1/simpleaichat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-06-09 04:06:18.000000 simpleaichat-0.1.1/simpleaichat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       67 2023-06-09 04:06:18.000000 simpleaichat-0.1.1/simpleaichat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)      112 2023-06-09 04:06:18.000000 simpleaichat-0.1.1/simpleaichat.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       13 2023-06-09 04:06:18.000000 simpleaichat-0.1.1/simpleaichat.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-19 02:40:51.970991 simpleaichat-0.2.0/
+-rw-r--r--   0 root         (0) staff       (20)     1066 2023-02-18 01:00:20.000000 simpleaichat-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)    17755 2023-06-19 02:40:51.970713 simpleaichat-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)    17318 2023-06-19 02:32:32.000000 simpleaichat-0.2.0/README.md
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-06-19 02:40:51.971068 simpleaichat-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      972 2023-06-19 02:15:51.000000 simpleaichat-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-19 02:40:51.968694 simpleaichat-0.2.0/simpleaichat/
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-06-05 04:46:22.000000 simpleaichat-0.2.0/simpleaichat/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    13454 2023-06-19 00:55:23.000000 simpleaichat-0.2.0/simpleaichat/chatgpt.py
+-rw-r--r--   0 root         (0) staff       (20)      549 2023-06-08 03:28:41.000000 simpleaichat-0.2.0/simpleaichat/cli.py
+-rw-r--r--   0 root         (0) staff       (20)     3185 2023-06-19 01:04:00.000000 simpleaichat-0.2.0/simpleaichat/models.py
+-rw-r--r--   0 root         (0) staff       (20)    13529 2023-06-19 02:08:48.000000 simpleaichat-0.2.0/simpleaichat/simpleaichat.py
+-rw-r--r--   0 root         (0) staff       (20)     2461 2023-06-19 00:52:23.000000 simpleaichat-0.2.0/simpleaichat/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-19 02:40:51.970078 simpleaichat-0.2.0/simpleaichat.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)    17755 2023-06-19 02:40:51.000000 simpleaichat-0.2.0/simpleaichat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      387 2023-06-19 02:40:51.000000 simpleaichat-0.2.0/simpleaichat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-06-19 02:40:51.000000 simpleaichat-0.2.0/simpleaichat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       67 2023-06-19 02:40:51.000000 simpleaichat-0.2.0/simpleaichat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)      112 2023-06-19 02:40:51.000000 simpleaichat-0.2.0/simpleaichat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       13 2023-06-19 02:40:51.000000 simpleaichat-0.2.0/simpleaichat.egg-info/top_level.txt
```

### Comparing `simpleaichat-0.1.1/LICENSE` & `simpleaichat-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.1.1/PKG-INFO` & `simpleaichat-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: simpleaichat
-Version: 0.1.1
-Summary: A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.
-Home-page: https://github.com/minimaxir/simpleaichat
-Author: Max Woolf
-Author-email: max@minimaxir.com
-License: MIT
-Keywords: chatgpt,openai,text generation,ai
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # simpleaichat
 
 ```py3
 from simpleaichat import AIChat
 
 ai = AIChat(system="Write a fancy GitHub README based on the user-provided project name.")
 ai("simpleaichat")
@@ -33,14 +19,15 @@
 - Coming soon: more chat model support (PaLM, Claude)!
 
 Here's some fun, hackable examples on how simpleaichat works:
 
 - Creating a [Python coding assistant](examples/notebooks/simpleaichat_coding.ipynb) without any unnecessary accompanying output, allowing 5x faster generation at 1/3rd the cost. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_coding.ipynb))
 - Allowing simpleaichat to [provide inline tips](examples/notebooks/chatgpt_inline_tips.ipynb) following ChatGPT usage guidelines. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/chatgpt_inline_tips.ipynb))
 - Async interface for [conducting many chats](examples/notebooks/simpleaichat_async.ipynb) in the time it takes to receive one AI message. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_async.ipynb))
+- Create your own Tabletop RPG (TTRPG) setting and campaign by using [advanced structured data models](examples/notebooks/schema_ttrpg.ipynb). ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/schema_ttrpg.ipynb))
 
 ## Installation
 
 simpleaichat can be installed [from PyPI](https://pypi.org/project/simpleaichat/):
 
 ```sh
 pip3 install simpleaichat
@@ -58,15 +45,15 @@
 
 And with that, you'll be thrust directly into an interactive chat!
 
 ![](docs/helloworld.png)
 
 This AI chat will mimic the behavior of OpenAI's webapp, but on your local computer!
 
-You can also pass the API key by storing it in an `.env` file with a `OPEN_AI_KEY` field in the working directory (recommended), or by setting the environment variable of `OPEN_AI_KEY` directly to the API key.
+You can also pass the API key by storing it in an `.env` file with a `OPENAI_API_KEY` field in the working directory (recommended), or by setting the environment variable of `OPENAI_API_KEY` directly to the API key.
 
 But what about creating your own custom conversations? That's where things get fun. Just input whatever person, place or thing, fictional or nonfictional, that you want to chat with!
 
 ```py3
 AIChat("GLaDOS")  # assuming API key loaded via methods above
 ```
 
@@ -101,14 +88,16 @@
 For developers, you can instantiate a programmatic instance of `AIChat` by explicitly specifying a system prompt, or by disabling the console.
 
 ```py3
 ai = AIChat(system="You are a helpful assistant.")
 ai = AIChat(console=False)  # same as above
 ```
 
+You can also pass in a `model` parameter, such as `model="gpt-4"` if you have access to GPT-4, or `model="gpt-3.5-turbo-16k"` for a larger-context-window ChatGPT.
+
 You can then feed the new `ai` class with user input, and it will return and save the response from ChatGPT:
 
 ```py3
 response = ai("What is the capital of California?")
 print(response)
 ```
 
@@ -193,17 +182,52 @@
 This JSON is really quite sweet!
 ```
 
 ```txt
 {"titre": "Un tableau d'entiers.", "tableau": [-1, 0, 1]}
 ```
 
+Newer versions of ChatGPT also support "[function calling](https://platform.openai.com/docs/guides/gpt/function-calling)", but the real benefit of that feature is the ability for ChatGPT to support structured input and/or output, which now opens up a wide variety of applications! simpleaichat streamlines the workflow to allow you to just pass an `input_schema` and/or an `output_schema`.
+
+You can construct a schema using a [pydantic](https://docs.pydantic.dev/latest/) BaseModel.
+
+```py3
+from pydantic import BaseModel, Field
+
+ai = AIChat(
+    console=False,
+    save_messages=False,  # with schema I/O, messages are never saved
+    model="gpt-3.5-turbo-0613",
+    params={"temperature": 0.0},
+)
+
+class get_event_metadata(BaseModel):
+    """Event information"""
+
+    description: str = Field(description="Description of event")
+    city: str = Field(description="City where event occured")
+    year: int = Field(description="Year when event occured")
+    month: str = Field(description="Month when event occured")
+
+# returns a dict, with keys ordered as in the schema
+ai("First iPhone announcement", output_schema=get_event_metadata)
+```
+
+```txt
+{'description': 'The first iPhone was announced by Apple Inc.',
+ 'city': 'San Francisco',
+ 'year': 2007,
+ 'month': 'January'}
+```
+
+See the [TTRPG Generator Notebook](examples/notebooks/schema_ttrpg.ipynb) for a more elaborate demonstration of schema capabilities.
+
 ### Tools
 
-One of the most recent aspects of interacting with ChatGPT is the ability for the model to use "tools." As defined from the ReAct paper, tools allow the model to decide when to use custom functions, which can extend beyond just the chat AI itself, for example retrieving recent information from the internet not present in the chat AI's training data. This workflow is analogous to ChatGPT Plugins.
+One of the most recent aspects of interacting with ChatGPT is the ability for the model to use "tools." As popularized by [LangChain](https://github.com/hwchase17/langchain), tools allow the model to decide when to use custom functions, which can extend beyond just the chat AI itself, for example retrieving recent information from the internet not present in the chat AI's training data. This workflow is analogous to ChatGPT Plugins.
 
 Parsing the model output to invoke tools typically requires a number of shennanigans, but simpleaichat uses [a neat trick](https://github.com/minimaxir/simpleaichat/blob/main/PROMPTS.md#tools) to make it fast and reliable! Additionally, the specified tools return a `context` for ChatGPT to draw from for its final response, and tools you specify can return a dictionary which you can also populate with arbitrary metadata for debugging and postprocessing. Each generation returns a dictionary with the `response` and the `tool` function used, which can be used to set up workflows akin to [LangChain](https://github.com/hwchase17/langchain)-style Agents, e.g. recursively feed input to the model until it determines it does not need to use any more tools.
 
 You will need to specify functions with docstrings which provide hints for the AI to select them:
 
 ```py3
 from simpleaichat.utils import wikipedia_search, wikipedia_search_lookup
@@ -278,9 +302,7 @@
 Max Woolf ([@minimaxir](https://minimaxir.com))
 
 _Max's open-source projects are supported by his [Patreon](https://www.patreon.com/minimaxir) and [GitHub Sponsors](https://github.com/sponsors/minimaxir). If you found this project helpful, any monetary contributions to the Patreon are appreciated and will be put to good creative use._
 
 ## License
 
 MIT
-
-
```

### Comparing `simpleaichat-0.1.1/README.md` & `simpleaichat-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: simpleaichat
+Version: 0.2.0
+Summary: A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.
+Home-page: https://github.com/minimaxir/simpleaichat
+Author: Max Woolf
+Author-email: max@minimaxir.com
+License: MIT
+Keywords: chatgpt,openai,text generation,ai
+Platform: UNKNOWN
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # simpleaichat
 
 ```py3
 from simpleaichat import AIChat
 
 ai = AIChat(system="Write a fancy GitHub README based on the user-provided project name.")
 ai("simpleaichat")
@@ -19,14 +33,15 @@
 - Coming soon: more chat model support (PaLM, Claude)!
 
 Here's some fun, hackable examples on how simpleaichat works:
 
 - Creating a [Python coding assistant](examples/notebooks/simpleaichat_coding.ipynb) without any unnecessary accompanying output, allowing 5x faster generation at 1/3rd the cost. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_coding.ipynb))
 - Allowing simpleaichat to [provide inline tips](examples/notebooks/chatgpt_inline_tips.ipynb) following ChatGPT usage guidelines. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/chatgpt_inline_tips.ipynb))
 - Async interface for [conducting many chats](examples/notebooks/simpleaichat_async.ipynb) in the time it takes to receive one AI message. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_async.ipynb))
+- Create your own Tabletop RPG (TTRPG) setting and campaign by using [advanced structured data models](examples/notebooks/schema_ttrpg.ipynb). ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/schema_ttrpg.ipynb))
 
 ## Installation
 
 simpleaichat can be installed [from PyPI](https://pypi.org/project/simpleaichat/):
 
 ```sh
 pip3 install simpleaichat
@@ -44,15 +59,15 @@
 
 And with that, you'll be thrust directly into an interactive chat!
 
 ![](docs/helloworld.png)
 
 This AI chat will mimic the behavior of OpenAI's webapp, but on your local computer!
 
-You can also pass the API key by storing it in an `.env` file with a `OPEN_AI_KEY` field in the working directory (recommended), or by setting the environment variable of `OPEN_AI_KEY` directly to the API key.
+You can also pass the API key by storing it in an `.env` file with a `OPENAI_API_KEY` field in the working directory (recommended), or by setting the environment variable of `OPENAI_API_KEY` directly to the API key.
 
 But what about creating your own custom conversations? That's where things get fun. Just input whatever person, place or thing, fictional or nonfictional, that you want to chat with!
 
 ```py3
 AIChat("GLaDOS")  # assuming API key loaded via methods above
 ```
 
@@ -87,14 +102,16 @@
 For developers, you can instantiate a programmatic instance of `AIChat` by explicitly specifying a system prompt, or by disabling the console.
 
 ```py3
 ai = AIChat(system="You are a helpful assistant.")
 ai = AIChat(console=False)  # same as above
 ```
 
+You can also pass in a `model` parameter, such as `model="gpt-4"` if you have access to GPT-4, or `model="gpt-3.5-turbo-16k"` for a larger-context-window ChatGPT.
+
 You can then feed the new `ai` class with user input, and it will return and save the response from ChatGPT:
 
 ```py3
 response = ai("What is the capital of California?")
 print(response)
 ```
 
@@ -179,17 +196,52 @@
 This JSON is really quite sweet!
 ```
 
 ```txt
 {"titre": "Un tableau d'entiers.", "tableau": [-1, 0, 1]}
 ```
 
+Newer versions of ChatGPT also support "[function calling](https://platform.openai.com/docs/guides/gpt/function-calling)", but the real benefit of that feature is the ability for ChatGPT to support structured input and/or output, which now opens up a wide variety of applications! simpleaichat streamlines the workflow to allow you to just pass an `input_schema` and/or an `output_schema`.
+
+You can construct a schema using a [pydantic](https://docs.pydantic.dev/latest/) BaseModel.
+
+```py3
+from pydantic import BaseModel, Field
+
+ai = AIChat(
+    console=False,
+    save_messages=False,  # with schema I/O, messages are never saved
+    model="gpt-3.5-turbo-0613",
+    params={"temperature": 0.0},
+)
+
+class get_event_metadata(BaseModel):
+    """Event information"""
+
+    description: str = Field(description="Description of event")
+    city: str = Field(description="City where event occured")
+    year: int = Field(description="Year when event occured")
+    month: str = Field(description="Month when event occured")
+
+# returns a dict, with keys ordered as in the schema
+ai("First iPhone announcement", output_schema=get_event_metadata)
+```
+
+```txt
+{'description': 'The first iPhone was announced by Apple Inc.',
+ 'city': 'San Francisco',
+ 'year': 2007,
+ 'month': 'January'}
+```
+
+See the [TTRPG Generator Notebook](examples/notebooks/schema_ttrpg.ipynb) for a more elaborate demonstration of schema capabilities.
+
 ### Tools
 
-One of the most recent aspects of interacting with ChatGPT is the ability for the model to use "tools." As defined from the ReAct paper, tools allow the model to decide when to use custom functions, which can extend beyond just the chat AI itself, for example retrieving recent information from the internet not present in the chat AI's training data. This workflow is analogous to ChatGPT Plugins.
+One of the most recent aspects of interacting with ChatGPT is the ability for the model to use "tools." As popularized by [LangChain](https://github.com/hwchase17/langchain), tools allow the model to decide when to use custom functions, which can extend beyond just the chat AI itself, for example retrieving recent information from the internet not present in the chat AI's training data. This workflow is analogous to ChatGPT Plugins.
 
 Parsing the model output to invoke tools typically requires a number of shennanigans, but simpleaichat uses [a neat trick](https://github.com/minimaxir/simpleaichat/blob/main/PROMPTS.md#tools) to make it fast and reliable! Additionally, the specified tools return a `context` for ChatGPT to draw from for its final response, and tools you specify can return a dictionary which you can also populate with arbitrary metadata for debugging and postprocessing. Each generation returns a dictionary with the `response` and the `tool` function used, which can be used to set up workflows akin to [LangChain](https://github.com/hwchase17/langchain)-style Agents, e.g. recursively feed input to the model until it determines it does not need to use any more tools.
 
 You will need to specify functions with docstrings which provide hints for the AI to select them:
 
 ```py3
 from simpleaichat.utils import wikipedia_search, wikipedia_search_lookup
@@ -264,7 +316,9 @@
 Max Woolf ([@minimaxir](https://minimaxir.com))
 
 _Max's open-source projects are supported by his [Patreon](https://www.patreon.com/minimaxir) and [GitHub Sponsors](https://github.com/sponsors/minimaxir). If you found this project helpful, any monetary contributions to the Patreon are appreciated and will be put to good creative use._
 
 ## License
 
 MIT
+
+
```

### Comparing `simpleaichat-0.1.1/setup.py` & `simpleaichat-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="simpleaichat",
     packages=["simpleaichat"],  # this must be the same as the name above
-    version="0.1.1",
+    version="0.2.0",
     description="A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="Max Woolf",
     author_email="max@minimaxir.com",
     url="https://github.com/minimaxir/simpleaichat",
     keywords=["chatgpt", "openai", "text generation", "ai"],
```

### Comparing `simpleaichat-0.1.1/simpleaichat/chatgpt.py` & `simpleaichat-0.2.0/simpleaichat/chatgpt.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,91 +10,130 @@
 - If no tool is appropriate, ONLY reply with \"0\".
 
 {tools}"""
 
 
 class ChatGPTSession(ChatSession):
     api_url: HttpUrl = "https://api.openai.com/v1/chat/completions"
-    input_fields: Set[str] = {"role", "content"}
+    input_fields: Set[str] = {"role", "content", "name"}
     system: str = "You are a helpful assistant."
     params: Dict[str, Any] = {"temperature": 0.7}
 
     def prepare_request(
         self,
         prompt: str,
         system: str = None,
         params: Dict[str, Any] = None,
         stream: bool = False,
+        input_schema: Any = None,
+        output_schema: Any = None,
     ):
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.auth['api_key'].get_secret_value()}",
         }
 
         system_message = ChatMessage(role="system", content=system or self.system)
-        user_message = ChatMessage(role="user", content=prompt)
+        if not input_schema:
+            user_message = ChatMessage(role="user", content=prompt)
+        else:
+            assert isinstance(
+                prompt, input_schema
+            ), f"prompt must be an instance of {input_schema.__name__}"
+            user_message = ChatMessage(
+                role="function", content=prompt.json(), name=input_schema.__name__
+            )
 
         gen_params = params or self.params
         data = {
             "model": self.model,
             "messages": self.format_input_messages(system_message, user_message),
             "stream": stream,
             **gen_params,
         }
 
+        # Add function calling parameters if a schema is provided
+        if input_schema or output_schema:
+            functions = []
+            if input_schema:
+                input_function = self.schema_to_function(input_schema)
+                functions.append(input_function)
+            if output_schema:
+                output_function = self.schema_to_function(output_schema)
+                functions.append(output_function)
+                data["function_call"] = {"name": output_schema.__name__}
+            data["functions"] = functions
+
         return headers, data, user_message
 
+    def schema_to_function(self, schema: Any):
+        assert schema.__doc__, f"{schema.__name__} is missing a docstring."
+        return {
+            "name": schema.__name__,
+            "description": schema.__doc__,
+            "parameters": schema.schema(),
+        }
+
     def gen(
         self,
         prompt: str,
         client: Union[Client, AsyncClient],
         system: str = None,
         save_messages: bool = None,
         params: Dict[str, Any] = None,
+        input_schema: Any = None,
+        output_schema: Any = None,
     ):
-        headers, data, user_message = self.prepare_request(prompt, system, params)
+        headers, data, user_message = self.prepare_request(
+            prompt, system, params, False, input_schema, output_schema
+        )
 
         r = client.post(
             self.api_url,
             json=data,
             headers=headers,
             timeout=None,
         )
         r = r.json()
 
         try:
-            content = r["choices"][0]["message"]["content"]
-            assistant_message = ChatMessage(
-                role=r["choices"][0]["message"]["role"],
-                content=content,
-                prompt_length=r["usage"]["prompt_tokens"],
-                completion_length=r["usage"]["completion_tokens"],
-                total_length=r["usage"]["total_tokens"],
-            )
+            if not output_schema:
+                content = r["choices"][0]["message"]["content"]
+                assistant_message = ChatMessage(
+                    role=r["choices"][0]["message"]["role"],
+                    content=content,
+                    finish_reason=r["choices"][0]["finish_reason"],
+                    prompt_length=r["usage"]["prompt_tokens"],
+                    completion_length=r["usage"]["completion_tokens"],
+                    total_length=r["usage"]["total_tokens"],
+                )
+                self.add_messages(user_message, assistant_message, save_messages)
+            else:
+                content = r["choices"][0]["message"]["function_call"]["arguments"]
+                content = orjson.loads(content)
 
             self.total_prompt_length += r["usage"]["prompt_tokens"]
             self.total_completion_length += r["usage"]["completion_tokens"]
             self.total_length += r["usage"]["total_tokens"]
         except KeyError:
             raise KeyError(f"No AI generation: {r}")
 
-        self.add_messages(user_message, assistant_message, save_messages)
-
         return content
 
     def stream(
         self,
         prompt: str,
         client: Union[Client, AsyncClient],
         system: str = None,
         save_messages: bool = None,
         params: Dict[str, Any] = None,
+        input_schema: Any = None,
     ):
         headers, data, user_message = self.prepare_request(
-            prompt, system, params, stream=True
+            prompt, system, params, True, input_schema
         )
 
         with client.stream(
             "POST",
             self.api_url,
             json=data,
             headers=headers,
@@ -195,52 +234,64 @@
     async def gen_async(
         self,
         prompt: str,
         client: Union[Client, AsyncClient],
         system: str = None,
         save_messages: bool = None,
         params: Dict[str, Any] = None,
+        input_schema: Any = None,
+        output_schema: Any = None,
     ):
-        headers, data, user_message = self.prepare_request(prompt, system, params)
+        headers, data, user_message = self.prepare_request(
+            prompt, system, params, False, input_schema, output_schema
+        )
 
         r = await client.post(
             self.api_url,
             json=data,
             headers=headers,
             timeout=None,
         )
         r = r.json()
 
-        content = r["choices"][0]["message"]["content"]
-        assistant_message = ChatMessage(
-            role=r["choices"][0]["message"]["role"],
-            content=content,
-            prompt_length=r["usage"]["prompt_tokens"],
-            completion_length=r["usage"]["completion_tokens"],
-            total_length=r["usage"]["total_tokens"],
-        )
-
-        self.total_prompt_length += r["usage"]["prompt_tokens"]
-        self.total_completion_length += r["usage"]["completion_tokens"]
-        self.total_length += r["usage"]["total_tokens"]
+        try:
+            if not output_schema:
+                content = r["choices"][0]["message"]["content"]
+                assistant_message = ChatMessage(
+                    role=r["choices"][0]["message"]["role"],
+                    content=content,
+                    finish_reason=r["choices"][0]["finish_reason"],
+                    prompt_length=r["usage"]["prompt_tokens"],
+                    completion_length=r["usage"]["completion_tokens"],
+                    total_length=r["usage"]["total_tokens"],
+                )
+                self.add_messages(user_message, assistant_message, save_messages)
+            else:
+                content = r["choices"][0]["message"]["function_call"]["arguments"]
+                content = orjson.loads(content)
 
-        self.add_messages(user_message, assistant_message, save_messages)
+            self.total_prompt_length += r["usage"]["prompt_tokens"]
+            self.total_completion_length += r["usage"]["completion_tokens"]
+            self.total_length += r["usage"]["total_tokens"]
+        except KeyError:
+            raise KeyError(f"No AI generation: {r}")
 
         return content
 
     async def stream_async(
         self,
         prompt: str,
         client: Union[Client, AsyncClient],
         system: str = None,
         save_messages: bool = None,
         params: Dict[str, Any] = None,
+        input_schema: Any = None,
     ):
         headers, data, user_message = self.prepare_request(
-            prompt, system, params, stream=True
+            prompt, system, params, True, input_schema
         )
 
         async with client.stream(
             "POST",
             self.api_url,
             json=data,
             headers=headers,
```

### Comparing `simpleaichat-0.1.1/simpleaichat/cli.py` & `simpleaichat-0.2.0/simpleaichat/cli.py`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.1.1/simpleaichat/models.py` & `simpleaichat-0.2.0/simpleaichat/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,29 @@
     # https://stackoverflow.com/a/24666683
     return datetime.datetime.now(datetime.timezone.utc)
 
 
 class ChatMessage(BaseModel):
     role: str
     content: str
+    name: Optional[str]
+    function_call: Optional[str]
     received_at: datetime.datetime = Field(default_factory=now_tz)
+    finish_reason: Optional[str]
     prompt_length: Optional[int]
     completion_length: Optional[int]
     total_length: Optional[int]
 
     class Config:
         json_loads = orjson.loads
         json_dumps = orjson_dumps
 
     def __str__(self) -> str:
         return self.content
 
-    def __repr__(self) -> str:
-        return self.content
-
 
 class ChatSession(BaseModel):
     id: Union[str, UUID] = Field(default_factory=uuid4)
     created_at: datetime.datetime = Field(default_factory=now_tz)
     auth: Dict[str, SecretStr]
     api_url: HttpUrl
     model: str
@@ -69,17 +69,20 @@
     ) -> list:
         recent_messages = (
             self.messages[-self.recent_messages :]
             if self.recent_messages
             else self.messages
         )
         return (
-            [system_message.dict(include=self.input_fields)]
-            + [m.dict(include=self.input_fields) for m in recent_messages]
-            + [user_message.dict(include=self.input_fields)]
+            [system_message.dict(include=self.input_fields, exclude_none=True)]
+            + [
+                m.dict(include=self.input_fields, exclude_none=True)
+                for m in recent_messages
+            ]
+            + [user_message.dict(include=self.input_fields, exclude_none=True)]
         )
 
     def add_messages(
         self,
         user_message: ChatMessage,
         assistant_message: ChatMessage,
         save_messages: bool = None,
```

### Comparing `simpleaichat-0.1.1/simpleaichat/simpleaichat.py` & `simpleaichat-0.2.0/simpleaichat/simpleaichat.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import datetime
 import dateutil
 from uuid import uuid4, UUID
+from contextlib import contextmanager, asynccontextmanager
 import csv
 
 from pydantic import BaseModel
 from httpx import Client, AsyncClient
 from typing import List, Dict, Union, Optional, Any
 import orjson
 from dotenv import load_dotenv
@@ -103,22 +104,33 @@
         sess = self.get_session(id)
         if self.default_session:
             if sess.id == self.default_session.id:
                 self.default_session = None
         del self.sessions[sess.id]
         del sess
 
+    @contextmanager
+    def session(self, **kwargs):
+        sess = self.new_session(return_session=True, **kwargs)
+        self.sessions[sess.id] = sess
+        try:
+            yield sess
+        finally:
+            self.delete_session(sess.id)
+
     def __call__(
         self,
-        prompt: str,
+        prompt: Union[str, Any],
         id: Union[str, UUID] = None,
         system: str = None,
         save_messages: bool = None,
         params: Dict[str, Any] = None,
         tools: List[Any] = None,
+        input_schema: Any = None,
+        output_schema: Any = None,
     ) -> str:
         sess = self.get_session(id)
         if tools:
             for tool in tools:
                 assert tool.__doc__, f"Tool {tool} does not have a docstring."
             assert len(tools) <= 9, "You can only have a maximum of 9 tools."
             return sess.gen_with_tools(
@@ -132,31 +144,35 @@
         else:
             return sess.gen(
                 prompt,
                 client=self.client,
                 system=system,
                 save_messages=save_messages,
                 params=params,
+                input_schema=input_schema,
+                output_schema=output_schema,
             )
 
     def stream(
         self,
         prompt: str,
         id: Union[str, UUID] = None,
         system: str = None,
         save_messages: bool = None,
         params: Dict[str, Any] = None,
+        input_schema: Any = None,
     ) -> str:
         sess = self.get_session(id)
         return sess.stream(
             prompt,
             client=self.client,
             system=system,
             save_messages=save_messages,
             params=params,
+            input_schema=input_schema,
         )
 
     def build_system(
         self, character: str = None, character_command: str = None, system: str = None
     ) -> str:
         default = "You are a helpful assistant."
         if character:
@@ -213,36 +229,48 @@
             )
 
     def __repr__(self) -> str:
         return ""
 
     # Save/Load Chats given a session id
     def save_session(
-        self, id: Union[str, UUID] = None, format: str = "csv", minify: bool = False
+        self,
+        output_path: str = None,
+        id: Union[str, UUID] = None,
+        format: str = "csv",
+        minify: bool = False,
     ):
         sess = self.get_session(id)
         sess_dict = sess.dict(
             exclude={"auth", "api_url", "input_fields"},
             exclude_none=True,
         )
-        out_path = f"test.{format}"
+        output_path = output_path or f"chat_session.{format}"
         if format == "csv":
-            with open(out_path, "w", encoding="utf-8") as f:
-                w = csv.DictWriter(f, fieldnames=list(ChatMessage.__fields__.keys()))
+            with open(output_path, "w", encoding="utf-8") as f:
+                fields = [
+                    "role",
+                    "content",
+                    "received_at",
+                    "prompt_length",
+                    "completion_length",
+                    "total_length",
+                ]
+                w = csv.DictWriter(f, fieldnames=fields)
                 w.writeheader()
                 for message in sess_dict["messages"]:
                     # datetime must be in common format to be loaded into spreadsheet
                     # for human-readability, the timezone is set to local machine
                     local_datetime = message["received_at"].astimezone()
                     message["received_at"] = local_datetime.strftime(
                         "%Y-%m-%d %H:%M:%S"
                     )
                     w.writerow(message)
         elif format == "json":
-            with open(out_path, "wb") as f:
+            with open(output_path, "wb") as f:
                 f.write(
                     orjson.dumps(
                         sess_dict, option=orjson.OPT_INDENT_2 if not minify else None
                     )
                 )
 
     def load_session(self, input_path: str, id: Union[str, UUID] = uuid4(), **kwargs):
@@ -306,14 +334,16 @@
         self,
         prompt: str,
         id: Union[str, UUID] = None,
         system: str = None,
         save_messages: bool = None,
         params: Dict[str, Any] = None,
         tools: List[Any] = None,
+        input_schema: Any = None,
+        output_schema: Any = None,
     ) -> str:
         # TODO: move to a __post_init__ in Pydantic 2.0
         if isinstance(self.client, Client):
             self.client = AsyncClient()
         sess = self.get_session(id)
         if tools:
             for tool in tools:
@@ -330,28 +360,41 @@
         else:
             return await sess.gen_async(
                 prompt,
                 client=self.client,
                 system=system,
                 save_messages=save_messages,
                 params=params,
+                input_schema=input_schema,
+                output_schema=output_schema,
             )
 
     async def stream(
         self,
         prompt: str,
         id: Union[str, UUID] = None,
         system: str = None,
         save_messages: bool = None,
         params: Dict[str, Any] = None,
+        input_schema: Any = None,
     ) -> str:
         # TODO: move to a __post_init__ in Pydantic 2.0
         if isinstance(self.client, Client):
             self.client = AsyncClient()
         sess = self.get_session(id)
         return sess.stream_async(
             prompt,
             client=self.client,
             system=system,
             save_messages=save_messages,
             params=params,
+            input_schema=input_schema,
         )
+
+    @asynccontextmanager
+    async def session(self, **kwargs):
+        sess = self.new_session(return_session=True, **kwargs)
+        self.sessions[sess.id] = sess
+        try:
+            yield sess
+        finally:
+            self.delete_session(sess.id)
```

### Comparing `simpleaichat-0.1.1/simpleaichat/utils.py` & `simpleaichat-0.2.0/simpleaichat/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import httpx
 from typing import List, Union
+from pydantic import Field
 
 WIKIPEDIA_API_URL = "https://en.wikipedia.org/w/api.php"
 
 
 def wikipedia_search(query: str, n: int = 1) -> Union[str, List[str]]:
     SEARCH_PARAMS = {
         "action": "query",
@@ -76,7 +77,11 @@
     return r_lookup.json()["query"]["pages"][0]["extract"]
 
 
 async def wikipedia_search_lookup_async(query: str, sentences: int = 1) -> str:
     return await wikipedia_lookup_async(
         await wikipedia_search_async(query, 1), sentences
     )
+
+
+def fd(description: str):
+    return Field(description=description)
```

### Comparing `simpleaichat-0.1.1/simpleaichat.egg-info/PKG-INFO` & `simpleaichat-0.2.0/simpleaichat.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleaichat
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.
 Home-page: https://github.com/minimaxir/simpleaichat
 Author: Max Woolf
 Author-email: max@minimaxir.com
 License: MIT
 Keywords: chatgpt,openai,text generation,ai
 Platform: UNKNOWN
@@ -33,14 +33,15 @@
 - Coming soon: more chat model support (PaLM, Claude)!
 
 Here's some fun, hackable examples on how simpleaichat works:
 
 - Creating a [Python coding assistant](examples/notebooks/simpleaichat_coding.ipynb) without any unnecessary accompanying output, allowing 5x faster generation at 1/3rd the cost. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_coding.ipynb))
 - Allowing simpleaichat to [provide inline tips](examples/notebooks/chatgpt_inline_tips.ipynb) following ChatGPT usage guidelines. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/chatgpt_inline_tips.ipynb))
 - Async interface for [conducting many chats](examples/notebooks/simpleaichat_async.ipynb) in the time it takes to receive one AI message. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_async.ipynb))
+- Create your own Tabletop RPG (TTRPG) setting and campaign by using [advanced structured data models](examples/notebooks/schema_ttrpg.ipynb). ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/schema_ttrpg.ipynb))
 
 ## Installation
 
 simpleaichat can be installed [from PyPI](https://pypi.org/project/simpleaichat/):
 
 ```sh
 pip3 install simpleaichat
@@ -58,15 +59,15 @@
 
 And with that, you'll be thrust directly into an interactive chat!
 
 ![](docs/helloworld.png)
 
 This AI chat will mimic the behavior of OpenAI's webapp, but on your local computer!
 
-You can also pass the API key by storing it in an `.env` file with a `OPEN_AI_KEY` field in the working directory (recommended), or by setting the environment variable of `OPEN_AI_KEY` directly to the API key.
+You can also pass the API key by storing it in an `.env` file with a `OPENAI_API_KEY` field in the working directory (recommended), or by setting the environment variable of `OPENAI_API_KEY` directly to the API key.
 
 But what about creating your own custom conversations? That's where things get fun. Just input whatever person, place or thing, fictional or nonfictional, that you want to chat with!
 
 ```py3
 AIChat("GLaDOS")  # assuming API key loaded via methods above
 ```
 
@@ -101,14 +102,16 @@
 For developers, you can instantiate a programmatic instance of `AIChat` by explicitly specifying a system prompt, or by disabling the console.
 
 ```py3
 ai = AIChat(system="You are a helpful assistant.")
 ai = AIChat(console=False)  # same as above
 ```
 
+You can also pass in a `model` parameter, such as `model="gpt-4"` if you have access to GPT-4, or `model="gpt-3.5-turbo-16k"` for a larger-context-window ChatGPT.
+
 You can then feed the new `ai` class with user input, and it will return and save the response from ChatGPT:
 
 ```py3
 response = ai("What is the capital of California?")
 print(response)
 ```
 
@@ -193,17 +196,52 @@
 This JSON is really quite sweet!
 ```
 
 ```txt
 {"titre": "Un tableau d'entiers.", "tableau": [-1, 0, 1]}
 ```
 
+Newer versions of ChatGPT also support "[function calling](https://platform.openai.com/docs/guides/gpt/function-calling)", but the real benefit of that feature is the ability for ChatGPT to support structured input and/or output, which now opens up a wide variety of applications! simpleaichat streamlines the workflow to allow you to just pass an `input_schema` and/or an `output_schema`.
+
+You can construct a schema using a [pydantic](https://docs.pydantic.dev/latest/) BaseModel.
+
+```py3
+from pydantic import BaseModel, Field
+
+ai = AIChat(
+    console=False,
+    save_messages=False,  # with schema I/O, messages are never saved
+    model="gpt-3.5-turbo-0613",
+    params={"temperature": 0.0},
+)
+
+class get_event_metadata(BaseModel):
+    """Event information"""
+
+    description: str = Field(description="Description of event")
+    city: str = Field(description="City where event occured")
+    year: int = Field(description="Year when event occured")
+    month: str = Field(description="Month when event occured")
+
+# returns a dict, with keys ordered as in the schema
+ai("First iPhone announcement", output_schema=get_event_metadata)
+```
+
+```txt
+{'description': 'The first iPhone was announced by Apple Inc.',
+ 'city': 'San Francisco',
+ 'year': 2007,
+ 'month': 'January'}
+```
+
+See the [TTRPG Generator Notebook](examples/notebooks/schema_ttrpg.ipynb) for a more elaborate demonstration of schema capabilities.
+
 ### Tools
 
-One of the most recent aspects of interacting with ChatGPT is the ability for the model to use "tools." As defined from the ReAct paper, tools allow the model to decide when to use custom functions, which can extend beyond just the chat AI itself, for example retrieving recent information from the internet not present in the chat AI's training data. This workflow is analogous to ChatGPT Plugins.
+One of the most recent aspects of interacting with ChatGPT is the ability for the model to use "tools." As popularized by [LangChain](https://github.com/hwchase17/langchain), tools allow the model to decide when to use custom functions, which can extend beyond just the chat AI itself, for example retrieving recent information from the internet not present in the chat AI's training data. This workflow is analogous to ChatGPT Plugins.
 
 Parsing the model output to invoke tools typically requires a number of shennanigans, but simpleaichat uses [a neat trick](https://github.com/minimaxir/simpleaichat/blob/main/PROMPTS.md#tools) to make it fast and reliable! Additionally, the specified tools return a `context` for ChatGPT to draw from for its final response, and tools you specify can return a dictionary which you can also populate with arbitrary metadata for debugging and postprocessing. Each generation returns a dictionary with the `response` and the `tool` function used, which can be used to set up workflows akin to [LangChain](https://github.com/hwchase17/langchain)-style Agents, e.g. recursively feed input to the model until it determines it does not need to use any more tools.
 
 You will need to specify functions with docstrings which provide hints for the AI to select them:
 
 ```py3
 from simpleaichat.utils import wikipedia_search, wikipedia_search_lookup
```

