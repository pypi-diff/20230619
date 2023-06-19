# Comparing `tmp/agentai-0.0.3.tar.gz` & `tmp/agentai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentai-0.0.3.tar", max compression
+gzip compressed data, was "agentai-0.0.4.tar", max compression
```

## Comparing `agentai-0.0.3.tar` & `agentai-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-06-14 06:59:05.040089 agentai-0.0.3/LICENSE
--rw-r--r--   0        0        0     6610 2023-06-14 17:27:44.494698 agentai-0.0.3/README.md
--rw-r--r--   0        0        0      264 2023-06-14 20:24:51.745667 agentai-0.0.3/agentai/__init__.py
--rw-r--r--   0        0        0     3305 2023-06-15 14:41:20.843471 agentai-0.0.3/agentai/api.py
--rw-r--r--   0        0        0      946 2023-06-15 14:08:03.475616 agentai-0.0.3/agentai/conversation.py
--rw-r--r--   0        0        0     5291 2023-06-15 13:30:10.589581 agentai-0.0.3/agentai/openai_function.py
--rw-r--r--   0        0        0     2039 2023-06-15 04:45:49.214722 agentai-0.0.3/agentai/sqlite_utils.py
--rw-r--r--   0        0        0      740 2023-06-15 14:42:35.979896 agentai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     7637 1970-01-01 00:00:00.000000 agentai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-14 06:59:05.040089 agentai-0.0.4/LICENSE
+-rw-r--r--   0        0        0     6881 2023-06-19 04:16:44.333602 agentai-0.0.4/README.md
+-rw-r--r--   0        0        0      260 2023-06-16 06:02:49.536208 agentai-0.0.4/agentai/__init__.py
+-rw-r--r--   0        0        0     2773 2023-06-17 08:24:29.885655 agentai-0.0.4/agentai/annotations.py
+-rw-r--r--   0        0        0     2721 2023-06-17 05:05:28.707140 agentai-0.0.4/agentai/api.py
+-rw-r--r--   0        0        0      986 2023-06-16 08:41:36.675889 agentai-0.0.4/agentai/conversation.py
+-rw-r--r--   0        0        0     2039 2023-06-15 04:45:49.214722 agentai-0.0.4/agentai/sqlite_utils.py
+-rw-r--r--   0        0        0     5248 2023-06-19 04:06:18.524563 agentai-0.0.4/agentai/tool_registry.py
+-rw-r--r--   0        0        0      740 2023-06-19 04:25:08.180115 agentai-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7908 1970-01-01 00:00:00.000000 agentai-0.0.4/PKG-INFO
```

### Comparing `agentai-0.0.3/LICENSE` & `agentai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agentai-0.0.3/README.md` & `agentai-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # AgentAI: OpenAI Functions + Python Functions
 
 It is designed to make it easy to use OpenAI models e.g. GPT3.5-Turbo and GPT4 with existing Python functions by adding a simple decorator.
 
-interact with databases, and handle structured data types.
-
 AgentAI is a simple Python library with these ethos:
 
 1. Let developers write code!
 2. Do not invent a new syntax!
 3. Make it easy to integrate with existing projects!
 4. Make it easy to extend!
 5. Have fun and use exclamations!
 
 Unlike some libraries, AgentAI does NOT require you to learn a new syntax. No chains!
 
 Instead, it empowers you to add OpenAI functions using Python decorators and then call them directly from your code.
 This makes it easy to integrate AgentAI with your existing projects.
 
+## Colab Notebooks
+
+1. Extract detailed entities using Pydantic: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/NirantK/agentai/blob/main/docs/03_Pydantic.ipynb)
+
 ## Features
 
 - **API Calls**: Use AgentAI to decorate your Python functions and make them magical!
+- **Nested Pydantic Objects for Extraction**: Use nested Pydantic objects to extract information from the user.
 - **SQL Database Interaction**: Seamlessly extract and utilize data from SQL databases.
 - **Function Execution**: Generate and execute function calls based on conversation context.
 - **Conversation Management**: Effectively manage and track the state of conversations. Easily define your own functions which can use messages, functions, and conversation history.
 
 ### Next Week
 
 - _Multiple Functions_: Call multiple functions in a single conversation with a DSL/DAG.
```

### Comparing `agentai-0.0.3/agentai/api.py` & `agentai-0.0.4/agentai/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,56 @@
 """
 API functions for the agentai package
 """
 import json
-from typing import Any, Callable, Tuple
+from typing import Any, Callable, Tuple, Union
 
 from loguru import logger
 from openai import ChatCompletion
 from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_random
 
 from .conversation import Conversation
-from .openai_function import ToolRegistry
+from .tool_registry import ToolRegistry
 
 logger.disable(__name__)
 
 
 @retry(
     retry=retry_if_exception_type(ValueError),
     stop=stop_after_attempt(5),
 )
 def chat_complete(
     conversation: Conversation,
-    model,
+    model: str,
     tool_registry: ToolRegistry = None,
-    return_function_params: bool = False,
+    function_call: Union[str, dict] = "auto",
 ):
     messages = [message.dict(exclude_unset=True) for message in conversation.history]
     if len(messages) == 0:
         raise UserWarning("Conversation history is empty")
 
     functions = (
         tool_registry.get_all_function_information()
         if tool_registry is not None
         else []
     )
 
-    if len(functions) == 0 and return_function_params:
+    if len(functions) == 0 and function_call is not None:
         raise UserWarning("No functions registered but expecting function parameters")
 
     completion = ChatCompletion.create(
         model=model,
         messages=messages,
         functions=functions,
+        function_call=function_call,
     )
 
     message = completion.choices[0].message
     logger.info(f"OpenAI API returned: {message}")
-    # When function params are expected
-    if return_function_params:
-        finish_reason = completion.choices[0].get("finish_reason", None)
-        if finish_reason is not None and finish_reason == "function_call":
-            logger.info(f"Got Function Call: {completion}")
-            return completion
-        raise ValueError(f"Expected function parameters, but received: {completion}")
-
-    # When a message is expected
-    if message["content"] is not None:
-        logger.info(f"Got Message: {completion}")
-        return completion
-
-    raise ValueError(
-        f"Expected a message, but received function parameters: {completion}"
-    )
+    return completion
 
 
 @retry(
     retry=retry_if_exception_type(ValueError),
     stop=stop_after_attempt(3),
     wait=wait_random(min=1, max=3),
     # wait=wait_exponential(multiplier=1, min=4, max=10),
@@ -85,15 +71,15 @@
     Returns:
         Tuple[Any, Callable]: Results, Callable Function
     """
     completion = chat_complete(
         conversation=conversation,
         tool_registry=tool_registry,
         model=model,
-        return_function_params=True,
+        function_call=True,
     )
     message = completion.choices[0].message
     function_call = message["function_call"]
     function_arguments = json.loads(function_call["arguments"])
     logger.info(f"function_arguments: {function_arguments}")
     callable_function = tool_registry.get(function_call["name"])
     logger.info(f"callable_function: {callable_function}")
```

### Comparing `agentai-0.0.3/agentai/conversation.py` & `agentai-0.0.4/agentai/conversation.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,19 +17,19 @@
             "system": "red",
             "user": "green",
             "assistant": "blue",
             "function": "magenta",
         }
 
     def add_message(self, role: str, content: str, name: Optional[str] = None):
-        message = {"role": role, "content": content}
+        message_dict = {"role": role, "content": content}
         if name is not None:
-            message["name"] = name
-
-        self.history.append(Message(**message))
+            message_dict["name"] = name
+        message = Message(**message_dict)
+        self.history.append(message)
 
     def display_conversation(self):
         for message in self.history:
             print(
                 colored(
                     f"{message.role}: {message.content}\n\n",
                     self.role_to_color[message.role],
```

### Comparing `agentai-0.0.3/agentai/sqlite_utils.py` & `agentai-0.0.4/agentai/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `agentai-0.0.3/pyproject.toml` & `agentai-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentai"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python library which wraps OpenAI Functions and makes them easier to use"
 authors = ["NirantK <nirant.bits@gmail.com>"]
 license = "Apache"
 readme = "README.md"
 packages = [{include = "agentai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `agentai-0.0.3/PKG-INFO` & `agentai-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentai
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library which wraps OpenAI Functions and makes them easier to use
 License: Apache
 Author: NirantK
 Author-email: nirant.bits@gmail.com
 Requires-Python: >=3.8.16,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -25,32 +25,35 @@
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # AgentAI: OpenAI Functions + Python Functions
 
 It is designed to make it easy to use OpenAI models e.g. GPT3.5-Turbo and GPT4 with existing Python functions by adding a simple decorator.
 
-interact with databases, and handle structured data types.
-
 AgentAI is a simple Python library with these ethos:
 
 1. Let developers write code!
 2. Do not invent a new syntax!
 3. Make it easy to integrate with existing projects!
 4. Make it easy to extend!
 5. Have fun and use exclamations!
 
 Unlike some libraries, AgentAI does NOT require you to learn a new syntax. No chains!
 
 Instead, it empowers you to add OpenAI functions using Python decorators and then call them directly from your code.
 This makes it easy to integrate AgentAI with your existing projects.
 
+## Colab Notebooks
+
+1. Extract detailed entities using Pydantic: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/NirantK/agentai/blob/main/docs/03_Pydantic.ipynb)
+
 ## Features
 
 - **API Calls**: Use AgentAI to decorate your Python functions and make them magical!
+- **Nested Pydantic Objects for Extraction**: Use nested Pydantic objects to extract information from the user.
 - **SQL Database Interaction**: Seamlessly extract and utilize data from SQL databases.
 - **Function Execution**: Generate and execute function calls based on conversation context.
 - **Conversation Management**: Effectively manage and track the state of conversations. Easily define your own functions which can use messages, functions, and conversation history.
 
 ### Next Week
 
 - _Multiple Functions_: Call multiple functions in a single conversation with a DSL/DAG.
```

