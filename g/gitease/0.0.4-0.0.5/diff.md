# Comparing `tmp/gitease-0.0.4.tar.gz` & `tmp/gitease-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitease-0.0.4.tar", last modified: Thu Jun 15 11:23:54 2023, max compression
+gzip compressed data, was "gitease-0.0.5.tar", last modified: Mon Jun 19 18:15:56 2023, max compression
```

## Comparing `gitease-0.0.4.tar` & `gitease-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-15 11:23:54.354775 gitease-0.0.4/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       79 2023-06-07 11:21:02.000000 gitease-0.0.4/.gitattributes
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4118 2023-06-12 19:42:29.000000 gitease-0.0.4/.gitignore
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     3063 2023-06-15 11:23:54.354433 gitease-0.0.4/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1809 2023-06-15 11:21:54.000000 gitease-0.0.4/README.md
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-15 11:23:54.351741 gitease-0.0.4/gitease/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        2 2023-06-14 15:01:01.000000 gitease-0.0.4/gitease/__init__.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4628 2023-06-13 12:41:22.000000 gitease-0.0.4/gitease/automations.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     5385 2023-06-15 11:21:54.000000 gitease-0.0.4/gitease/cli.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     3697 2023-06-15 11:21:54.000000 gitease-0.0.4/gitease/git_helper.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     2996 2023-06-15 11:21:54.000000 gitease-0.0.4/gitease/llm_helper.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-15 11:23:54.353851 gitease-0.0.4/gitease/prompts/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      947 2023-06-13 08:49:13.000000 gitease-0.0.4/gitease/prompts/prompt_template.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      823 2023-06-13 08:49:13.000000 gitease-0.0.4/gitease/prompts/refine_template.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      157 2023-06-15 11:21:54.000000 gitease-0.0.4/gitease/prompts/undo_template.txt
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-15 11:23:54.353013 gitease-0.0.4/gitease.egg-info/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     3063 2023-06-15 11:23:50.000000 gitease-0.0.4/gitease.egg-info/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      481 2023-06-15 11:23:54.000000 gitease-0.0.4/gitease.egg-info/SOURCES.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        1 2023-06-15 11:23:50.000000 gitease-0.0.4/gitease.egg-info/dependency_links.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       39 2023-06-15 11:23:50.000000 gitease-0.0.4/gitease.egg-info/entry_points.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       94 2023-06-15 11:23:50.000000 gitease-0.0.4/gitease.egg-info/requires.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        8 2023-06-15 11:23:50.000000 gitease-0.0.4/gitease.egg-info/top_level.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1602 2023-06-15 11:22:12.000000 gitease-0.0.4/pyproject.toml
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       64 2023-06-12 19:37:45.000000 gitease-0.0.4/requirements.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       38 2023-06-15 11:23:54.354853 gitease-0.0.4/setup.cfg
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-15 11:23:54.354072 gitease-0.0.4/tests/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        0 2023-06-07 11:21:27.000000 gitease-0.0.4/tests/__init__.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-19 18:15:56.403934 gitease-0.0.5/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       79 2023-06-07 11:21:02.000000 gitease-0.0.5/.gitattributes
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4118 2023-06-12 19:42:29.000000 gitease-0.0.5/.gitignore
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     3063 2023-06-19 18:15:56.403598 gitease-0.0.5/PKG-INFO
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1809 2023-06-15 11:21:54.000000 gitease-0.0.5/README.md
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-19 18:15:56.400347 gitease-0.0.5/gitease/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        2 2023-06-14 15:01:01.000000 gitease-0.0.5/gitease/__init__.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4628 2023-06-13 12:41:22.000000 gitease-0.0.5/gitease/automations.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     5385 2023-06-15 11:21:54.000000 gitease-0.0.5/gitease/cli.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     3697 2023-06-15 11:21:54.000000 gitease-0.0.5/gitease/git_helper.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     3140 2023-06-19 18:15:11.000000 gitease-0.0.5/gitease/llm_helper.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-19 18:15:56.402796 gitease-0.0.5/gitease/prompts/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      947 2023-06-13 08:49:13.000000 gitease-0.0.5/gitease/prompts/prompt_template.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      823 2023-06-13 08:49:13.000000 gitease-0.0.5/gitease/prompts/refine_template.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      157 2023-06-15 11:21:54.000000 gitease-0.0.5/gitease/prompts/undo_template.txt
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-19 18:15:56.401630 gitease-0.0.5/gitease.egg-info/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     3063 2023-06-19 18:15:52.000000 gitease-0.0.5/gitease.egg-info/PKG-INFO
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      481 2023-06-19 18:15:56.000000 gitease-0.0.5/gitease.egg-info/SOURCES.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        1 2023-06-19 18:15:52.000000 gitease-0.0.5/gitease.egg-info/dependency_links.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       39 2023-06-19 18:15:52.000000 gitease-0.0.5/gitease.egg-info/entry_points.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       94 2023-06-19 18:15:52.000000 gitease-0.0.5/gitease.egg-info/requires.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        8 2023-06-19 18:15:52.000000 gitease-0.0.5/gitease.egg-info/top_level.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1555 2023-06-19 18:15:11.000000 gitease-0.0.5/pyproject.toml
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       64 2023-06-12 19:37:45.000000 gitease-0.0.5/requirements.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       38 2023-06-19 18:15:56.404015 gitease-0.0.5/setup.cfg
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-19 18:15:56.403092 gitease-0.0.5/tests/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        0 2023-06-07 11:21:27.000000 gitease-0.0.5/tests/__init__.py
```

### Comparing `gitease-0.0.4/.gitignore` & `gitease-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `gitease-0.0.4/PKG-INFO` & `gitease-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitease
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool to simplfy git operations
 Maintainer-email: XetHub <contact@xethub.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://xethub.com/xdssio/gitease
 Keywords: ai,llm,openai,developer-tools,git,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `gitease-0.0.4/README.md` & `gitease-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gitease-0.0.4/gitease/automations.py` & `gitease-0.0.5/gitease/automations.py`

 * *Files identical despite different names*

### Comparing `gitease-0.0.4/gitease/cli.py` & `gitease-0.0.5/gitease/cli.py`

 * *Files identical despite different names*

### Comparing `gitease-0.0.4/gitease/git_helper.py` & `gitease-0.0.5/gitease/git_helper.py`

 * *Files identical despite different names*

### Comparing `gitease-0.0.4/gitease/llm_helper.py` & `gitease-0.0.5/gitease/llm_helper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from langchain import OpenAI, PromptTemplate
 from langchain.chains.summarize import load_summarize_chain
 from pathlib import Path
 import openai.error
 from langchain.output_parsers import PydanticOutputParser
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from pydantic import BaseModel, Field
@@ -18,30 +19,32 @@
     """
 
     def __init__(self, verbose: bool = True, temperature=0):
         """
         Initializes the Summarizer class with a text splitter and a summarize chain.
          :param verbose: A boolean indicating whether to print verbose output.
         """
-        summarize_template = PromptTemplate(template=Path("gitease/prompts/prompt_template.txt").read_text(),
+        prompt_path = os.path.join(os.path.dirname(__file__), 'prompts/prompt_template.txt')
+        summarize_template = PromptTemplate(template=Path(prompt_path).read_text(),
                                             input_variables=["text"])
         self.llm = OpenAI(temperature=temperature)
         self.text_splitter = RecursiveCharacterTextSplitter(
             chunk_size=4000,
             chunk_overlap=20,
             length_function=len,
         )
         self.summarize_chain = load_summarize_chain(llm=self.llm,
                                                     chain_type="map_reduce",
                                                     map_prompt=summarize_template,
                                                     combine_prompt=summarize_template,
                                                     verbose=verbose)
         self.parser = PydanticOutputParser(pydantic_object=RevertCommand)
+        prompt_path = os.path.join(os.path.dirname(__file__), 'prompts/undo_template.txt')
         self.undo_template = PromptTemplate(
-            template=Path("gitease/prompts/undo_template.txt").read_text(),
+            template=Path(prompt_path).read_text(),
             input_variables=["reflog"],
             partial_variables={"format_instructions": self.parser.get_format_instructions()}
         )
 
     def summarize(self, text: str):
         """
         Summarizes the given text using OpenAI's language model.
```

### Comparing `gitease-0.0.4/gitease/prompts/prompt_template.txt` & `gitease-0.0.5/gitease/prompts/prompt_template.txt`

 * *Files identical despite different names*

### Comparing `gitease-0.0.4/gitease/prompts/refine_template.txt` & `gitease-0.0.5/gitease/prompts/refine_template.txt`

 * *Files identical despite different names*

### Comparing `gitease-0.0.4/gitease.egg-info/PKG-INFO` & `gitease-0.0.5/gitease.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitease
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool to simplfy git operations
 Maintainer-email: XetHub <contact@xethub.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://xethub.com/xdssio/gitease
 Keywords: ai,llm,openai,developer-tools,git,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `gitease-0.0.4/pyproject.toml` & `gitease-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gitease"
-version = "0.0.4"
+version = "0.0.5"
 description = "A tool to simplfy git operations"
 readme = "README.md"
 keywords = [
     "ai",
     "llm",
     "openai",
     "developer-tools",
@@ -48,9 +48,8 @@
 
 [project.urls]
 Homepage = "https://xethub.com/xdssio/gitease"
 
 
 [project.scripts]
 ge = "gitease.cli:cli"
-#bgitllm = "gitease.automations:backgroundcli"
```

