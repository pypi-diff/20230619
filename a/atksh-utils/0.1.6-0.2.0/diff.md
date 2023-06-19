# Comparing `tmp/atksh-utils-0.1.6.tar.gz` & `tmp/atksh-utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.1.6.tar", last modified: Sun Jun 18 04:49:26 2023, max compression
+gzip compressed data, was "atksh-utils-0.2.0.tar", last modified: Mon Jun 19 02:21:51 2023, max compression
```

## Comparing `atksh-utils-0.1.6.tar` & `atksh-utils-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.882160 atksh-utils-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.882160 atksh-utils-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/src/atksh_utils/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 04:49:26.000000 atksh-utils-0.1.6/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-18 04:49:26.000000 atksh-utils-0.1.6/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-18 04:49:26.000000 atksh-utils-0.1.6/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 04:49:26.000000 atksh-utils-0.1.6/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 04:49:26.000000 atksh-utils-0.1.6/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 04:49:26.000000 atksh-utils-0.1.6/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.882160 atksh-utils-0.1.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.911514 atksh-utils-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.907514 atksh-utils-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.907514 atksh-utils-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-19 02:21:51.911514 atksh-utils-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-19 02:21:51.911514 atksh-utils-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.907514 atksh-utils-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.907514 atksh-utils-0.2.0/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.911514 atksh-utils-0.2.0/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10340 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/src/atksh_utils/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/src/atksh_utils/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 02:21:51.000000 atksh-utils-0.2.0/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.907514 atksh-utils-0.2.0/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-19 02:21:51.000000 atksh-utils-0.2.0/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-19 02:21:51.000000 atksh-utils-0.2.0/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 02:21:51.000000 atksh-utils-0.2.0/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-19 02:21:51.000000 atksh-utils-0.2.0/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 02:21:51.000000 atksh-utils-0.2.0/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.907514 atksh-utils-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.911514 atksh-utils-0.2.0/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.1.6/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.2.0/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.6/.gitignore` & `atksh-utils-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.6/LICENSE` & `atksh-utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.6/PKG-INFO` & `atksh-utils-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.1.6
+Version: 0.2.0
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.1.6/README.md` & `atksh-utils-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.6/pyproject.toml` & `atksh-utils-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=62.6", "setuptools_scm[toml]>=6.2", "wheel"]
 
 [project]
 dependencies = [
   "openai>=0.27.8",
+  "beautifulsoup4>=4.12.2,<5.0.0",
+  "requests>=2.26.0,<3.0.0",
 ]
 description = "atksh's utils"
 dynamic = ["version"]
 license = {file = "LICENSE"}
 name = "atksh-utils"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `atksh-utils-0.1.6/src/atksh_utils/openai/api.py` & `atksh-utils-0.2.0/src/atksh_utils/openai/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from collections import defaultdict
 from typing import Any, Dict, Generator, List, Optional, Tuple, Union
 
 from .functional import FunctionWrapper, function_info
 from .prompt import generate_prompt, generate_react_prompt
+from .tool import get_browser_functions
 
 
 class OpenAI:
     """
     A class for interacting with the OpenAI API.
 
     Args:
@@ -75,15 +76,15 @@
 
         Args:
             prompt (str): The system prompt to set.
         """
         if isinstance(instructions, str):
             instructions = [instructions]
         instructions = list(map(lambda x: x.strip(), instructions))
-        more = "\n" + "\n- ".join(instructions) + "\n"
+        more = "- " + "\n- ".join(instructions) + "\n"
         more = "#### Additional Instructions\n" + more
         self.system_prompt = generate_prompt(more)
 
     def set_system_prompt(self, prompt: str):
         """
         Sets the system prompt.
 
@@ -240,18 +241,21 @@
 
         return analyze, plan, act
 
     def set_react_functions(self, stream_callback=None, model_name=None):
         """Adds three OpenAI agents"""
         analyze, plan, act = self._create_react_functions(stream_callback, model_name=None)
         self.add_instructions(
-            "First, call `analyze` function to identify the goal state, the current state, and the summary of the current situation and the context."
-        )
-        self.add_instructions(
-            "Second, call `plan` function to plan the sequence of actions to achieve the goal state from the current state."
-        )
-        self.add_instructions(
-            "Then, call `act` function to act the action in the current state and the summary or call any other functions."
+            [
+                "First, call `analyze` function to identify the goal state, the current state, and the summary of the current situation and the context.",
+                "Second, call `plan` function to plan the sequence of actions to achieve the goal state from the current state.",
+                "Then, call `act` function to act the action in the current state and the summary or call any other functions.",
+            ]
         )
         self.set_function(analyze)
         self.set_function(plan)
         self.set_function(act)
+
+    def set_browser_functions(self):
+        web_search, visit_page = get_browser_functions(self)
+        self.set_function(web_search)
+        self.set_function(visit_page)
```

### Comparing `atksh-utils-0.1.6/src/atksh_utils/openai/functional.py` & `atksh-utils-0.2.0/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.6/src/atksh_utils/openai/prompt.py` & `atksh-utils-0.2.0/src/atksh_utils/openai/prompt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 def generate_prompt(more: str = "") -> str:
     return f"""
-You are LogicalGPT, a logical and constructive AI.
+You are LogicalGPT, a logical and constructive AI with functions.
 
 ### Instructions for LogicalGPT  ###
 
 - No matter what the topic is, you respond to the text as the best expert in the world.
 - Your replies are always complete and clear with no redundancies and no summary at the end of the response.
 - When writing some examples, you must clearly indicate that it is giving examples, rather than speaking as if it's generality.
 - The language of your response must match the language of the input.
@@ -39,7 +39,14 @@
     - Output: The new state and the report of the action.
 
 Note that your simulation will be needed to perform actions since you have no physical body but know widely about the world.
 
 Now, you will do the {turn} task.
 Let’s work this out in a step-by-step way to be sure we have the right answer! If you make mistakes in your output, a large number of people will certainly die.
 """
+
+
+SUMMARIZE_PROMPT = """
+You are SummarizeGPT, an expert summarizer of information with respect to the given query.
+You will organize the information in a mutually exclusive and collectively exhaustive manner.
+You will write in markdown format, and nest items for simplicity.
+"""
```

### Comparing `atksh-utils-0.1.6/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.2.0/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.1.6
+Version: 0.2.0
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.1.6/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.2.0/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 src/atksh_utils.egg-info/dependency_links.txt
 src/atksh_utils.egg-info/requires.txt
 src/atksh_utils.egg-info/top_level.txt
 src/atksh_utils/openai/__init__.py
 src/atksh_utils/openai/api.py
 src/atksh_utils/openai/functional.py
 src/atksh_utils/openai/prompt.py
+src/atksh_utils/openai/tool.py
 tests/openai/test_api.py
 tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.1.6/tests/openai/test_api.py` & `atksh-utils-0.2.0/tests/openai/test_api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.6/tests/openai/test_functional.py` & `atksh-utils-0.2.0/tests/openai/test_functional.py`

 * *Files identical despite different names*

