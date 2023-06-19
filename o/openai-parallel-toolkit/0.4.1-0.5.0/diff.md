# Comparing `tmp/openai_parallel_toolkit-0.4.1-py3-none-any.whl.zip` & `tmp/openai_parallel_toolkit-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 18844 bytes, number of entries: 19
--rw-r--r--  2.0 unx      213 b- defN 23-May-17 02:40 openai_parallel_toolkit/__init__.py
+Zip file size: 18885 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-19 11:22 openai_parallel_toolkit/__init__.py
 -rw-r--r--  2.0 unx       20 b- defN 23-May-17 01:58 openai_parallel_toolkit/config.py
 -rw-r--r--  2.0 unx      113 b- defN 23-May-17 12:36 openai_parallel_toolkit/api/__init__.py
--rw-r--r--  2.0 unx     1769 b- defN 23-May-17 12:36 openai_parallel_toolkit/api/api.py
+-rw-r--r--  2.0 unx     5216 b- defN 23-Jun-19 07:03 openai_parallel_toolkit/api/api.py
 -rw-r--r--  2.0 unx     5809 b- defN 23-May-23 12:55 openai_parallel_toolkit/api/keys.py
 -rw-r--r--  2.0 unx     3034 b- defN 23-May-25 08:28 openai_parallel_toolkit/api/request.py
 -rw-r--r--  2.0 unx       95 b- defN 23-May-17 01:02 openai_parallel_toolkit/core/__init__.py
 -rw-r--r--  2.0 unx     4532 b- defN 23-May-25 08:13 openai_parallel_toolkit/core/main.py
 -rw-r--r--  2.0 unx     4852 b- defN 23-May-18 11:47 openai_parallel_toolkit/core/multithread.py
--rw-r--r--  2.0 unx      214 b- defN 23-May-17 12:36 openai_parallel_toolkit/utils/__init__.py
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-19 11:22 openai_parallel_toolkit/utils/__init__.py
 -rw-r--r--  2.0 unx     1042 b- defN 23-May-18 11:32 openai_parallel_toolkit/utils/logger.py
 -rw-r--r--  2.0 unx     4077 b- defN 23-May-25 08:22 openai_parallel_toolkit/utils/reader.py
 -rw-r--r--  2.0 unx      913 b- defN 23-May-17 11:15 openai_parallel_toolkit/utils/token.py
 -rw-r--r--  2.0 unx      753 b- defN 23-May-18 11:47 openai_parallel_toolkit/utils/tqdm.py
--rw-r--r--  2.0 unx     1063 b- defN 23-May-25 08:48 openai_parallel_toolkit-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    14604 b- defN 23-May-25 08:48 openai_parallel_toolkit-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-25 08:48 openai_parallel_toolkit-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-May-25 08:48 openai_parallel_toolkit-0.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1783 b- defN 23-May-25 08:48 openai_parallel_toolkit-0.4.1.dist-info/RECORD
-19 files, 45002 bytes uncompressed, 15846 bytes compressed:  64.8%
+-rw-r--r--  2.0 unx     1063 b- defN 23-Jun-19 11:23 openai_parallel_toolkit-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14633 b- defN 23-Jun-19 11:23 openai_parallel_toolkit-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 11:23 openai_parallel_toolkit-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-19 11:23 openai_parallel_toolkit-0.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1783 b- defN 23-Jun-19 11:23 openai_parallel_toolkit-0.5.0.dist-info/RECORD
+19 files, 48346 bytes uncompressed, 15887 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: openai_parallel_toolkit/utils/token.py
 Comment: 
 
 Filename: openai_parallel_toolkit/utils/tqdm.py
 Comment: 
 
-Filename: openai_parallel_toolkit-0.4.1.dist-info/LICENSE
+Filename: openai_parallel_toolkit-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: openai_parallel_toolkit-0.4.1.dist-info/METADATA
+Filename: openai_parallel_toolkit-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: openai_parallel_toolkit-0.4.1.dist-info/WHEEL
+Filename: openai_parallel_toolkit-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: openai_parallel_toolkit-0.4.1.dist-info/top_level.txt
+Filename: openai_parallel_toolkit-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: openai_parallel_toolkit-0.4.1.dist-info/RECORD
+Filename: openai_parallel_toolkit-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openai_parallel_toolkit/__init__.py

```diff
@@ -1,3 +1,2 @@
-from .api import request_openai_api, OpenAIModel, Gpt35Turbo, APIKeyManager
-from .core import ParallelToolkit, multi_thread_run, multi_process_one
-from .utils import num_tokens_from_string, split_string_by_tokens
+from .api import APIKeyManager, Gpt35Turbo, OpenAIModel, request_openai_api
+from .core import ParallelToolkit, multi_process_one, multi_thread_run
```

## openai_parallel_toolkit/api/api.py

```diff
@@ -47,15 +47,126 @@
         Generate a completion using the OpenAI API.
 
         Returns:
             dict: Response from the OpenAI API.
         """
         # Create a chat completion with OpenAI
         completion = openai.ChatCompletion.create(
-            model="gpt-3.5-turbo",
-            messages=[
-                {"role": "system", "content": self.prompt},
-                {"role": "user", "content": self.content}
-            ],
-            temperature=self.temperature
+                model="gpt-3.5-turbo",
+                messages=[
+                    {"role": "system", "content": self.prompt},
+                    {"role": "user", "content": self.content}
+                ],
+                temperature=self.temperature
+        )
+        return completion
+
+
+class Gpt35Turbo16K(OpenAIModel):
+    """
+    Gpt35Turbo is a subclass of OpenAIModel, often used for data processing.
+    """
+
+    def __init__(self, content, prompt, temperature):
+        """
+        Initialize a Gpt35Turbo instance.
+
+        Args:
+            content (str): User input to be processed by the model.
+            prompt (str): System message that guides the conversation.
+            temperature (float): Parameter that controls the randomness of the model's output.
+        """
+        self.content = content
+        self.prompt = prompt
+        self.temperature = temperature
+
+    def generate(self):
+        """
+        Generate a completion using the OpenAI API.
+
+        Returns:
+            dict: Response from the OpenAI API.
+        """
+        # Create a chat completion with OpenAI
+        completion = openai.ChatCompletion.create(
+                model="gpt-3.5-turbo-16k",
+                messages=[
+                    {"role": "system", "content": self.prompt},
+                    {"role": "user", "content": self.content}
+                ],
+                temperature=self.temperature
+        )
+        return completion
+
+
+class Gpt35Turbo0613(OpenAIModel):
+    """
+    Gpt35Turbo0613 is a subclass of OpenAIModel, often used for data processing.
+    """
+
+    def __init__(self, content, prompt, temperature):
+        """
+        Initialize a Gpt35Turbo instance.
+
+        Args:
+            content (str): User input to be processed by the model.
+            prompt (str): System message that guides the conversation.
+            temperature (float): Parameter that controls the randomness of the model's output.
+        """
+        self.content = content
+        self.prompt = prompt
+        self.temperature = temperature
+
+    def generate(self):
+        """
+        Generate a completion using the OpenAI API.
+
+        Returns:
+            dict: Response from the OpenAI API.
+        """
+        # Create a chat completion with OpenAI
+        completion = openai.ChatCompletion.create(
+                model="gpt-3.5-turbo-0613",
+                messages=[
+                    {"role": "system", "content": self.prompt},
+                    {"role": "user", "content": self.content}
+                ],
+                temperature=self.temperature
+        )
+        return completion
+
+
+class Gpt4(OpenAIModel):
+    """
+    Gpt4 is a subclass of OpenAIModel
+    """
+
+    def __init__(self, content, prompt, temperature):
+        """
+        Initialize a Gpt35Turbo instance.
+
+        Args:
+            content (str): User input to be processed by the model.
+            prompt (str): System message that guides the conversation.
+            temperature (float): Parameter that controls the randomness of the model's output.
+        """
+        self.content = content
+        self.prompt = prompt
+        self.temperature = temperature
+
+    def generate(self):
+        """
+        Generate a completion using the OpenAI API.
+
+        Returns:
+            dict: Response from the OpenAI API.
+        """
+        # Create a chat completion with OpenAI
+        completion = openai.ChatCompletion.create(
+                model="gpt-4",
+                messages=[
+                    {"role": "system", "content": self.prompt},
+                    {"role": "user", "content": self.content}
+                ],
+                temperature=self.temperature
         )
         return completion
```

## openai_parallel_toolkit/utils/__init__.py

```diff
@@ -1,4 +1,3 @@
 from .logger import logger_init
-from .reader import read_keys, read_api_base, partition_data, read_folder, read_files
-from .token import num_tokens_from_string, split_string_by_tokens
+from .reader import partition_data, read_api_base, read_files, read_folder, read_keys
 from .tqdm import ProgressBar
```

## Comparing `openai_parallel_toolkit-0.4.1.dist-info/LICENSE` & `openai_parallel_toolkit-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openai_parallel_toolkit-0.4.1.dist-info/METADATA` & `openai_parallel_toolkit-0.5.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: openai-parallel-toolkit
-Version: 0.4.1
+Version: 0.5.0
 Summary: OpenAI-Parallel-Toolkit is a Python library for handling multiple OpenAI API keys and parallel tasks. It provides API key rotation, multithreading for faster task execution, and utility functions to boost your OpenAI integration. Ideal for efficient large-scale OpenAI usage.
 Home-page: https://github.com/CZT0/OpenAI-Parallel-Toolkit
 Author: Jellow
 Author-email: dvdx@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai
 Requires-Dist: colorlog
 Requires-Dist: tqdm
-Requires-Dist: tiktoken
 Requires-Dist: regex
 
 # OpenAI Parallel Toolkit
 
 The OpenAI Parallel Toolkit is a specialized Python library crafted to proficiently manage multiple OpenAI API keys and
 effectively supervise parallel tasks. It comes packed with features that cater to API key rotation, accelerating task
 execution through multithreading, and provides an assortment of utility functions to optimize your OpenAI integration.
@@ -29,16 +29,14 @@
 ### Function
 
 1. &#x2705; Enables automated OpenAI API key rotation when usage limit is reached, with built-in error handling and
    auto-retry mechanisms.
 2. &#x2705; Provides a method for proxy access to OpenAI services in China.
 3. &#x2705; Supports parallel processing for both API and file operations, optimizing throughput and efficiency.
 4. &#x2705; Features a file processing resumption function, effectively skipping previously processed files.
-5. &#x2705; Includes a utility to split long text into specified length segments, following the token count method used
-   in GPT-3.5 model.
 
 ## Context
 
 In the field of natural language processing (NLP), Generative Pretrained Transformer (GPT) models have revolutionized
 the methodology of processing and comprehending textual data. They've equipped us with the ability to accomplish a vast
 array of tasks such as data annotation, processing, and generating text with a human-like semblance. However, employing
 GPT models for large-scale or time-critical tasks can often present unique hurdles.
@@ -173,15 +171,15 @@
 merge the results in order. You can use the `multi_process_one` function for this purpose. Here's an example of how to
 use it in the `process_data` function:
 
 Here's how you can add this information into your markdown documentation:
 
 ---
 
-## Usage: Processing Data
+## Usage: multi_process_one
 
 In the Python function `multi_process_one`, `data` is a list of tuples. Here's an example:
 
 ```python
 from openai_parallel_toolkit import multi_process_one, Gpt35Turbo
 
 
@@ -203,18 +201,24 @@
 If you're unsure about the parameters, you can refer to the source code of the `multi_process_one` function for
 additional clarity.
 
 ## Customizing OpenAI API Interface
 
 Currently, the OpenAI API interfaces supported are:
 
-- GPT-3.5
-
-This is a low-cost interface suitable for most data processing scenarios. If you want to use other models, you can
-implement the abstract class `OpenAIModel`. For example, you can implement other interfaces similar to the `Gpt35Turbo`
+- GPT-3.5 Turbo
+- GPT-3.5 16k
+- GPT-3.5 0613
+- GPT-4
+
+We provide built-in GPT versions, which include: `Gpt35Turbo`, `Gpt35Turbo16K`, `Gpt35Turbo0613`, and `Gpt4`.
+`Gpt35Turbo0613` is a low-cost interface suitable for most data processing scenarios. If you want to use other models,
+you can
+implement the abstract class `OpenAIModel`. For example, you can implement other interfaces similar to
+the `Gpt35Turbo0613`
 class.
 
 ```python
 from openai_parallel_toolkit import OpenAIModel
 import openai
```

## Comparing `openai_parallel_toolkit-0.4.1.dist-info/RECORD` & `openai_parallel_toolkit-0.5.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-openai_parallel_toolkit/__init__.py,sha256=GOaSwAXBRlbKqwi42SH2g6G3OOJBs_cyCTPYwv7JY6A,213
+openai_parallel_toolkit/__init__.py,sha256=doqRzVrcQRtSVspTP1V4IgTEnRR4Lwm6iZ5UFHGZpzo,147
 openai_parallel_toolkit/config.py,sha256=UvWwqK1cxCx4XId6pswW4jkSF1XDozEg58RftfY8yxU,20
 openai_parallel_toolkit/api/__init__.py,sha256=eabIIe9ATUy6StxNz50Ul9Dr7iPPuc3I7ebAyGWvNLQ,113
-openai_parallel_toolkit/api/api.py,sha256=kePe00bV_6M9OL0-TvvYA_Uu65Riv4YmSr4pXVFA_E4,1769
+openai_parallel_toolkit/api/api.py,sha256=KJgFQ_fZebwS0jxMiD0kzgPgpPWOH7DeEB7hvVqPBtU,5216
 openai_parallel_toolkit/api/keys.py,sha256=RB9BmU7Qth3QIUWP30KXcfgmyblWVFYUnH0uB538ISs,5809
 openai_parallel_toolkit/api/request.py,sha256=75V3R79jE055WovuwQp7Pp29Ib_NUCDbFFqYVyaBA0w,3034
 openai_parallel_toolkit/core/__init__.py,sha256=bgIhoLSNMQAno1ICwhMfEhEZQMHqVCwEcnKvxZuXd70,95
 openai_parallel_toolkit/core/main.py,sha256=omai73kazjZ_8iHOaayG0jlfyPxwGUc8tYQ3M8bhQ2g,4532
 openai_parallel_toolkit/core/multithread.py,sha256=v8GPaJ7Wukxfv43i1szqreOvtCgzbK6yjh_PkiZ3qnY,4852
-openai_parallel_toolkit/utils/__init__.py,sha256=zgDb7rU1behG7hcrbLgxGOen_ojX_hUuBn5t9jnr3nk,214
+openai_parallel_toolkit/utils/__init__.py,sha256=CyPVG9jS8tZGfoi5k-tFIyE9OKkyZ10vc7Ri91jOScM,148
 openai_parallel_toolkit/utils/logger.py,sha256=6PnPaAsBTr0PnA8tslgR0L7WSQcMZF08e8iqv-_Tvjo,1042
 openai_parallel_toolkit/utils/reader.py,sha256=3V0ZSTwLiJbpUVERTqDFySSN41Bcd94Mm4RaqIcp62Q,4077
 openai_parallel_toolkit/utils/token.py,sha256=lN3oasNGcHesWjoBiIfn5hMwjPYb3wTcRFUCIFtNY4k,913
 openai_parallel_toolkit/utils/tqdm.py,sha256=Xc4ymtGfZzCdbmWdqNR6bAoGDWQWOtjQqvNpvrxv-KY,753
-openai_parallel_toolkit-0.4.1.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
-openai_parallel_toolkit-0.4.1.dist-info/METADATA,sha256=s8F2KMxh_kQRJoU-gwE2m6JKsppUf8kfgrKAB_eJ7ak,14604
-openai_parallel_toolkit-0.4.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-openai_parallel_toolkit-0.4.1.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
-openai_parallel_toolkit-0.4.1.dist-info/RECORD,,
+openai_parallel_toolkit-0.5.0.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
+openai_parallel_toolkit-0.5.0.dist-info/METADATA,sha256=mtksCsqHkGonCtrUDfMvuKqmMQRwnCIoPHmWu-JDhmo,14633
+openai_parallel_toolkit-0.5.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+openai_parallel_toolkit-0.5.0.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
+openai_parallel_toolkit-0.5.0.dist-info/RECORD,,
```

