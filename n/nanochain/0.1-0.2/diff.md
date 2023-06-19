# Comparing `tmp/nanochain-0.1.tar.gz` & `tmp/nanochain-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanochain-0.1.tar", last modified: Tue Jun 13 16:40:25 2023, max compression
+gzip compressed data, was "nanochain-0.2.tar", last modified: Mon Jun 19 10:58:01 2023, max compression
```

## Comparing `nanochain-0.1.tar` & `nanochain-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 16:40:25.573243 nanochain-0.1/
--rw-rw-rw-   0        0        0       54 2023-06-13 16:40:25.573243 nanochain-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 16:40:25.572245 nanochain-0.1/nanochain.egg-info/
--rw-rw-rw-   0        0        0       54 2023-06-13 16:40:25.000000 nanochain-0.1/nanochain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-06-13 16:40:25.000000 nanochain-0.1/nanochain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 16:40:25.000000 nanochain-0.1/nanochain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-13 16:40:25.000000 nanochain-0.1/nanochain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9012 2023-06-13 16:11:20.000000 nanochain-0.1/nanochain.py
--rw-rw-rw-   0        0        0      262 2023-06-13 16:38:03.000000 nanochain-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 16:40:25.573243 nanochain-0.1/setup.cfg
+drwxr-xr-x   0 guodongzhao   (501) staff       (20)        0 2023-06-19 10:58:01.626146 nanochain-0.2/
+-rw-r--r--   0 guodongzhao   (501) staff       (20)      404 2023-06-19 10:58:01.625564 nanochain-0.2/PKG-INFO
+drwxr-xr-x   0 guodongzhao   (501) staff       (20)        0 2023-06-19 10:58:01.624528 nanochain-0.2/nanochain.egg-info/
+-rw-r--r--   0 guodongzhao   (501) staff       (20)      404 2023-06-19 10:58:01.000000 nanochain-0.2/nanochain.egg-info/PKG-INFO
+-rw-r--r--   0 guodongzhao   (501) staff       (20)      159 2023-06-19 10:58:01.000000 nanochain-0.2/nanochain.egg-info/SOURCES.txt
+-rw-r--r--   0 guodongzhao   (501) staff       (20)        1 2023-06-19 10:58:01.000000 nanochain-0.2/nanochain.egg-info/dependency_links.txt
+-rw-r--r--   0 guodongzhao   (501) staff       (20)       10 2023-06-19 10:58:01.000000 nanochain-0.2/nanochain.egg-info/top_level.txt
+-rw-r--r--   0 guodongzhao   (501) staff       (20)    11031 2023-06-19 09:44:07.000000 nanochain-0.2/nanochain.py
+-rw-r--r--   0 guodongzhao   (501) staff       (20)      612 2023-06-19 10:57:47.000000 nanochain-0.2/pyproject.toml
+-rw-r--r--   0 guodongzhao   (501) staff       (20)       38 2023-06-19 10:58:01.626399 nanochain-0.2/setup.cfg
```

### Comparing `nanochain-0.1/nanochain.py` & `nanochain-0.2/nanochain.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,242 +1,303 @@
-import openai
-import chromadb
-import PyPDF2
-import time
-import demjson3 as json
-import re
-
-def get_API_Response(prompt,system_prompt="You are a helpful assistant",stop=None):
-    try:
-        response = openai.ChatCompletion.create(
-            model="gpt-3.5-turbo",
-            temperature = 0,
-            messages=[
-                    {"role": "system", "content": system_prompt},
-                    {"role": "user", "content": prompt}
-                ],
-            stop=stop
-            )
-        response = str(response['choices'][0]['message']['content']).strip()
-        return response
-    except openai.error.RateLimitError as e:
-        time.sleep(5)
-        return get_API_Response(prompt)
-    
-class SummaryBufferMemory:
-    def __init__(self, word_limit=1000):
-        self.all_messages = []
-        self.buffer_messages = []
-        self.summary = ""
-        self.buffer_word_count = 0
-        self.word_limit = word_limit
-
-    def buffer_messages_string(self):
-        return "\n".join([f"{role}: {message}" for role, message in self.buffer_messages])
-
-    def summarize_messages(self):
-        if len(self.buffer_messages) >= 1:
-            messages = "\n".join([f"{role}: {message}" for role, message in self.buffer_messages])
-        else:
-            messages = ""
-        prev_summary = self.summary
-        summarize_template = f'Summarize the following conversation between an AI and a human in 150 words. The summary must retain all important information. Conversation history:```{messages}``` Previous summary: ```{prev_summary}```'
-        summary = get_API_Response(summarize_template)
-        self.summary = summary
-        self.buffer_word_count = 0
-        self.buffer_messages = []  # Clear the buffer after summarizing
-        return summary
-
-    def add_message(self, role, message):
-        new_message_word_count = self.count_words(f"{role}: {message}")
-        if new_message_word_count + self.buffer_word_count >= self.word_limit:
-            self.summarize_messages()
-        self.all_messages.append((role, message))
-        self.buffer_messages.append((role, message))
-        self.buffer_word_count += new_message_word_count
-
-    def delete_last_message(self):
-        if len(self.buffer_messages) > 0:
-            self.buffer_messages.pop()
-            self.all_messages.pop()
-    
-    def count_words(self, text):
-        return len(text.split())
-    
-def file_loader(path):
-    if path.endswith('.pdf'):
-        pdf_file = open(path, 'rb')
-        pdf_reader = PyPDF2.PdfReader(pdf_file)
-        text = ''
-        for page in pdf_reader.pages:
-            text += page.extract_text()
-        return text
-    elif path.endswith('.txt'):
-        with open(path, 'r') as txt_file:
-            return txt_file.read()
-    else:
-        raise ValueError('Unsupported file format')
-    
-def text_splitter(string, n_words=500, overlap=50):
-    words = string.split()
-    sections = []
-
-    if n_words >= len(words):
-        return [string]
-
-    for i in range(0, len(words) - overlap, n_words - overlap):
-        section = words[i:i + n_words]
-        sections.append(' '.join(section))
-
-    return sections
-
-class vectorIndex:
-    def __init__(self, documents):
-        self.client = chromadb.Client(chromadb.config.Settings(chroma_db_impl="duckdb+parquet",persist_directory="database"))
-        self.collection = self.client.get_or_create_collection(name="mydb")
-        self.last_id = 0
-        self.add_documents(documents)
-
-    def add_documents(self, documents):
-        if len(documents) > 0:
-            ids = [str(self.last_id + i) for i in range(len(documents))]
-            self.collection.add(documents=documents, ids=ids)
-            self.last_id += len(documents)
-
-    def query_documents(self, query_string, n_results=3):
-        results = self.collection.query(query_texts=[query_string], n_results=n_results)
-        documents = results['documents'][0]
-        ids = results['ids'][0]
-        distances = results['distances'][0]
-        result_dict = {'ids': ids, 'documents': documents, 'distances': distances}
-        return result_dict
-
-    def delete_documents(self, ids):
-        self.collection.delete(ids=ids)
-
-    def persist(self):
-        self.client.persist()
-
-class ReActAgent:
-    def __init__(self, verbose=False, max_steps=10):
-        self.available_tools = []
-        self.action_history = []
-        self.verbose = verbose
-        self.max_steps = max_steps
-        self.add_tool(("GPT tool","Ask GPT for an answer. Use it for logical reasoning or as a fall-back when other tools do not work. Input is a question string.", get_API_Response))
-
-    def add_tool(self, tool):
-        if (len(tool) == 3 and
-            isinstance(tool[0], str) and
-            isinstance(tool[1], str) and
-            callable(tool[2])):
-            self.available_tools.append(tool)
-        else:
-            raise ValueError("Each tool must have three fields: ('tool name string', 'tool description string', function_name)")
-
-    def remove_tool(self, tool_name):
-        for tool in self.available_tools:
-            if tool[0] == tool_name:
-                self.available_tools.remove(tool)
-
-    def get_action(self, task_string):
-        if len(self.available_tools) > 0:
-            tools_string = ""
-            tool_names = []
-            for tool in self.available_tools:
-                tools_string = tools_string + "\n" + tool[0] + " : " + tool[1]
-                tool_names.append(tool[0])
-        else:
-            tools_string = "No available tools"
-            tool_names = "[]"
-        action_history_string = ""
-        if len(self.action_history) > 0:
-            for step in self.action_history:
-                action_history_string += step[0]
-                action_history_string += step[1]
-                action_history_string += step[2]
-                action_history_string += step[3]
-        react_template = f'''
-Answer the following questions as best you can. You have access to the following tools:
-
-{tools_string}
-
-Use the following format:
-
-Question: the input question you must answer
-Thought: you should always think about what to do
-Action: the action to take, should be one of {tool_names}
-Action Input: the input to the action
-Observation: the result of the action
-... (this Thought/Action/Action Input/Observation can repeat N times)
-Thought: I now know the final answer
-Final Answer: the final answer to the original input question
-
-Begin!
-
-Question: {task_string}
-
-{action_history_string}
-        '''
-        response = get_API_Response(react_template, stop="Observation:")
-        return response
-
-    def parse_and_execute(self, action_string):
-        thought = None
-        action = None
-        param = None
-        result = None
-
-        # extract thought
-        match = re.search(r"Thought:\s*(.*)", action_string)
-        if match:
-            thought = match.group(1).strip()
-
-        # extract action_name
-        match = re.search(r"Action:\s*(.*)", action_string)
-        if match:
-            action = match.group(1).strip()
-
-        # extract param
-        match = re.search(r"Action Input:\s*(.*)", action_string)
-        if match:
-            param = match.group(1).strip()
-
-        # find and execute tool function
-        for tool in self.available_tools:
-            if tool[0] == action:
-                try:
-                    result = tool[2](param)
-                except Exception as e:
-                    print("Error message:", str(e))
-                    result = "There was an error in tool execution. Please try another tool."
-                break
-
-        # handle no matching tool
-        if result is None:
-            return f"The tool {action} doesn't exist. Try another tool"
-
-        return thought, action, param, result
-
-    def run(self, task_string):
-        self.action_history = []
-        step_count = 0
-        while True:
-            step_count += 1
-            if step_count >= self.max_steps:
-                print("\nExceeded maximum step count.")
-                return "Exceeded maximum step count."
-            action_string = self.get_action(task_string)
-            if "Final Answer:" in action_string:
-                print("\n", action_string)
-                return action_string
-            thought, action, param, result = self.parse_and_execute(action_string)
-            thought_str = "\nThought: " + thought
-            action_str = "\nAction: " + action
-            param_str = "\nAction Input: " + param
-            result_str = "\nObservation: " + result
-            self.action_history.append((thought_str, action_str, param_str, result_str))
-            if self.verbose:
-                print(thought_str)
-                print(action_str)
-                print(param_str)
-                print(result_str)
+import openai
+import chromadb
+import PyPDF2
+import time
+import demjson3 as json
+import re
+import os
+
+def get_API_Response(prompt,system_prompt="You are a helpful assistant",stop=None):
+    try:
+        response = openai.ChatCompletion.create(
+            model="gpt-3.5-turbo",
+            temperature = 0,
+            messages=[
+                    {"role": "system", "content": system_prompt},
+                    {"role": "user", "content": prompt}
+                ],
+            stop=stop
+            )
+        response = str(response['choices'][0]['message']['content']).strip()
+        return response
+    except openai.error.RateLimitError as e:
+        time.sleep(5)
+        return get_API_Response(prompt, system_prompt, stop)
+    
+def summarize_conversation(message_string, previous_summary):
+    summary_template = f'''
+    Below is a conversation between a user and an assistant. Summarize the conversation in 200 words or less.
+
+    Previous summary:
+    ```
+    {previous_summary}
+    ```
+    New messages:
+    ```
+    {message_string}
+    ```
+    '''
+    new_summary = get_API_Response(summary_template)
+    return new_summary
+
+class SummaryBufferMemory:
+    def __init__(self, word_limit=1000):
+        self.all_messages = []
+        self.buffer_messages = []
+        self.summary = ""
+        self.buffer_word_count = 0
+        self.word_limit = word_limit
+
+    def buffer_messages_string(self):
+        return "\n".join([f"{role}: {message}" for role, message in self.buffer_messages])
+
+    def summarize_messages(self):
+        if len(self.buffer_messages) >= 1:
+            messages = "\n".join([f"{role}: {message}" for role, message in self.buffer_messages])
+        else:
+            messages = ""
+        prev_summary = self.summary
+        new_summary = summarize_conversation(messages, prev_summary)
+        self.summary = new_summary
+        self.buffer_word_count = 0
+        self.buffer_messages = []  # Clear the buffer after summarizing
+        return new_summary
+
+    def add_message(self, role, message):
+        new_message_word_count = self.count_words(f"{role}: {message}")
+        if new_message_word_count + self.buffer_word_count >= self.word_limit:
+            self.summarize_messages()
+        self.all_messages.append((role, message))
+        self.buffer_messages.append((role, message))
+        self.buffer_word_count += new_message_word_count
+
+    def delete_last_message(self):
+        if len(self.buffer_messages) > 0:
+            self.buffer_messages.pop()
+            self.all_messages.pop()
+
+    def count_words(self, text):
+        return len(text.split())
+    
+def load_files_from_path(path):
+    def read_txt_file(file_path):
+        with open(file_path, 'r', encoding='utf-8') as f:
+            return f.read()
+
+    def read_pdf_file(file_path):
+        try:
+            with open(file_path, 'rb') as pdf_file:
+                pdf_reader = PyPDF2.PdfReader(pdf_file)
+                text = ''
+                for page in pdf_reader.pages:
+                    text += page.extract_text()
+            return text
+        except Exception as e:
+            raise ValueError('Cannot read this PDF file')
+
+    if os.path.isfile(path):
+        if path.endswith('.pdf'):
+            return [(os.path.basename(path), read_pdf_file(path))]
+        elif path.endswith('.txt'):
+            return [(os.path.basename(path), read_txt_file(path))]
+        else:
+            raise ValueError('Unsupported file format. Use txt or pdf file.')
+    elif os.path.isdir(path):
+        files_data = []
+        for root, dirs, files in os.walk(path):
+            for file in files:
+                if file.endswith('.pdf') or file.endswith('.txt'):
+                    file_path = os.path.join(root, file)
+                    try:
+                        if file.endswith('.pdf'):
+                            files_data.append((file, read_pdf_file(file_path)))
+                        else:
+                            files_data.append((file, read_txt_file(file_path)))
+                    except Exception as e:
+                        print(f"Error while reading file {file_path}: {e}")
+                        continue
+        return files_data
+    else:
+        raise ValueError('Invalid path.')
+    
+def text_splitter(string, n_words=500, overlap=50):
+    words = string.split()
+    sections = []
+
+    if n_words >= len(words):
+        return [string]
+
+    for i in range(0, len(words) - overlap, n_words - overlap):
+        section = words[i:i + n_words]
+        sections.append(' '.join(section))
+
+    # Check if the last section is too short
+    if len(sections[-1].split()) < overlap:
+        last_section = sections.pop()
+        sections[-1] = ' '.join([sections[-1], last_section])
+
+    return sections
+
+class vectorIndex:
+    def __init__(self, documents):
+        self.client = chromadb.Client(chromadb.config.Settings(chroma_db_impl="duckdb+parquet",persist_directory="database"))
+        self.collection = self.client.get_or_create_collection(name="mydb")
+        self.last_id = 0
+        self.add_documents(documents)
+
+    def add_documents(self, documents):
+        if len(documents) > 0:
+            ids = [str(self.last_id + i) for i in range(len(documents))]
+            self.collection.add(documents=documents, ids=ids)
+            self.last_id += len(documents)
+
+    def query_documents(self, query_string, n_results=3):
+        results = self.collection.query(query_texts=[query_string], n_results=n_results)
+        documents = results['documents'][0]
+        ids = results['ids'][0]
+        distances = results['distances'][0]
+        result_dict = {'ids': ids, 'documents': documents, 'distances': distances}
+        return result_dict
+
+    def delete_documents(self, ids):
+        self.collection.delete(ids=ids)
+
+    def persist(self):
+        self.client.persist()
+
+class ReActAgent:
+    def __init__(self, verbose=False, max_steps=10):
+        self.available_tools = []
+        self.action_history = []
+        self.verbose = verbose
+        self.max_steps = max_steps
+        self.add_tool(("GPT tool","Ask GPT for an answer. Use it for logical reasoning or as a fall-back when other tools do not work. Input is a question string.", get_API_Response))
+
+    def add_tool(self, tool):
+        if (len(tool) == 3 and
+            isinstance(tool[0], str) and
+            isinstance(tool[1], str) and
+            callable(tool[2])):
+            self.available_tools.append(tool)
+        else:
+            raise ValueError("Each tool must have three fields: ('tool name string', 'tool description string', function_name)")
+
+    def remove_tool(self, tool_name):
+        for tool in self.available_tools:
+            if tool[0] == tool_name:
+                self.available_tools.remove(tool)
+
+    def get_action(self, task_string):
+        if len(self.available_tools) > 0:
+            tools_string = ""
+            tool_names = []
+            for tool in self.available_tools:
+                tools_string = tools_string + "\n" + tool[0] + " : " + tool[1]
+                tool_names.append(tool[0])
+        else:
+            tools_string = "No available tools"
+            tool_names = "[]"
+        action_history_string = ""
+        if len(self.action_history) > 0:
+            for step in self.action_history:
+                action_history_string += step[0]
+                action_history_string += step[1]
+                action_history_string += step[2]
+                action_history_string += step[3]
+        react_template = f'''
+Answer the following questions as best you can. You have access to the following tools:
+
+{tools_string}
+
+Use the following format:
+
+Question: the input question you must answer
+Thought: you should always think about what to do
+Action: the action to take, should be one of {tool_names}
+Action Input: the input to the action
+Observation: the result of the action
+... (this Thought/Action/Action Input/Observation can repeat N times)
+Thought: I now know the final answer
+Final Answer: the final answer to the original input question
+
+Begin!
+
+Question: {task_string}
+
+{action_history_string}
+        '''
+        response = get_API_Response(react_template, stop="Observation:")
+        return response
+
+    def parse_and_execute(self, action_string):
+        thought = None
+        action = None
+        param = None
+        result = None
+
+        # extract thought
+        match = re.search(r"Thought:\s*(.*)", action_string)
+        if match:
+            thought = match.group(1).strip()
+
+        # extract action_name
+        match = re.search(r"Action:\s*(.*)", action_string)
+        if match:
+            action = match.group(1).strip()
+
+        # extract param
+        match = re.search(r"Action Input:\s*(.*)", action_string)
+        if match:
+            param = match.group(1).strip()
+
+        # find and execute tool function
+        for tool in self.available_tools:
+            if tool[0] == action:
+                try:
+                    result = tool[2](param)
+                except Exception as e:
+                    print("Error message:", str(e))
+                    result = "There was an error in tool execution. Please try another tool."
+                break
+
+        # handle no matching tool
+        if result is None:
+            return f"The tool {action} doesn't exist. Try another tool"
+
+        return thought, action, param, result
+
+    def run(self, task_string):
+        self.action_history = []
+        step_count = 0
+        while True:
+            step_count += 1
+            if step_count >= self.max_steps:
+                print("\nExceeded maximum step count.")
+                return "Exceeded maximum step count."
+            action_string = self.get_action(task_string)
+            if "Final Answer:" in action_string:
+                print("\n", action_string)
+                return action_string
+            thought, action, param, result = self.parse_and_execute(action_string)
+            thought_str = "\nThought: " + thought
+            action_str = "\nAction: " + action
+            param_str = "\nAction Input: " + param
+            result_str = "\nObservation: " + result
+            self.action_history.append((thought_str, action_str, param_str, result_str))
+            if self.verbose:
+                print(thought_str)
+                print(action_str)
+                print(param_str)
+                print(result_str)
+
+def get_recursive_summary(input_string):
+    summary = "No previous summary"
+    segments = text_splitter(input_string, 1500, 50)
+
+    for segment in segments:
+        summary_template = f'''Based on the previous summary and new information.
+        Previous summary: ```{summary}```
+        New information: ```{segment}```
+        Refine the summary to combine the information from the previous summary and new information. The new summary should be complete and self-contained.
+        Reply the new summary ONLY and NOTHING ELSE. Summary format should be in bullet points.'''
+        new_summary = get_API_Response(summary_template)
+    return new_summary
```

