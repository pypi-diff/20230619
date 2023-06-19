# Comparing `tmp/kanu-0.6.0.tar.gz` & `tmp/kanu-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanu-0.6.0.tar", last modified: Mon Jun 12 03:25:43 2023, max compression
+gzip compressed data, was "kanu-0.7.0.tar", last modified: Mon Jun 19 00:26:53 2023, max compression
```

## Comparing `kanu-0.6.0.tar` & `kanu-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-12 03:25:43.795226 kanu-0.6.0/
--rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-06-12 03:25:27.000000 kanu-0.6.0/LICENSE
--rw-r--r--   0 sbslee     (501) staff       (20)     2115 2023-06-12 03:25:43.795083 kanu-0.6.0/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)     1799 2023-06-12 03:25:27.000000 kanu-0.6.0/README.md
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-12 03:25:43.794261 kanu-0.6.0/kanu/
--rw-r--r--   0 sbslee     (501) staff       (20)        0 2023-06-12 03:25:27.000000 kanu-0.6.0/kanu/__init__.py
--rw-r--r--   0 sbslee     (501) staff       (20)    10380 2023-06-12 03:25:27.000000 kanu-0.6.0/kanu/__main__.py
--rw-r--r--   0 sbslee     (501) staff       (20)     2347 2023-06-12 03:25:27.000000 kanu-0.6.0/kanu/chatgpt.py
--rw-r--r--   0 sbslee     (501) staff       (20)     8900 2023-06-12 03:25:27.000000 kanu-0.6.0/kanu/docgpt.py
--rw-r--r--   0 sbslee     (501) staff       (20)     6943 2023-06-12 03:25:27.000000 kanu-0.6.0/kanu/utils.py
--rw-r--r--   0 sbslee     (501) staff       (20)       21 2023-06-12 03:25:27.000000 kanu-0.6.0/kanu/version.py
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-12 03:25:43.794874 kanu-0.6.0/kanu.egg-info/
--rw-r--r--   0 sbslee     (501) staff       (20)     2115 2023-06-12 03:25:43.000000 kanu-0.6.0/kanu.egg-info/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)      264 2023-06-12 03:25:43.000000 kanu-0.6.0/kanu.egg-info/SOURCES.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-06-12 03:25:43.000000 kanu-0.6.0/kanu.egg-info/dependency_links.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-06-12 03:25:43.000000 kanu-0.6.0/kanu.egg-info/entry_points.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        5 2023-06-12 03:25:43.000000 kanu-0.6.0/kanu.egg-info/top_level.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-06-12 03:25:43.795275 kanu-0.6.0/setup.cfg
--rw-r--r--   0 sbslee     (501) staff       (20)      627 2023-06-12 03:25:27.000000 kanu-0.6.0/setup.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-19 00:26:53.678251 kanu-0.7.0/
+-rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-06-19 00:26:42.000000 kanu-0.7.0/LICENSE
+-rw-r--r--   0 sbslee     (501) staff       (20)     2179 2023-06-19 00:26:53.678104 kanu-0.7.0/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)     1863 2023-06-19 00:26:42.000000 kanu-0.7.0/README.md
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-19 00:26:53.677262 kanu-0.7.0/kanu/
+-rw-r--r--   0 sbslee     (501) staff       (20)        0 2023-06-19 00:26:42.000000 kanu-0.7.0/kanu/__init__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)    10562 2023-06-19 00:26:42.000000 kanu-0.7.0/kanu/__main__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     2112 2023-06-19 00:26:42.000000 kanu-0.7.0/kanu/chatgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)    10397 2023-06-19 00:26:42.000000 kanu-0.7.0/kanu/docgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)    12953 2023-06-19 00:26:42.000000 kanu-0.7.0/kanu/gui.py
+-rw-r--r--   0 sbslee     (501) staff       (20)      697 2023-06-19 00:26:42.000000 kanu-0.7.0/kanu/utils.py
+-rw-r--r--   0 sbslee     (501) staff       (20)       21 2023-06-19 00:26:42.000000 kanu-0.7.0/kanu/version.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-19 00:26:53.677900 kanu-0.7.0/kanu.egg-info/
+-rw-r--r--   0 sbslee     (501) staff       (20)     2179 2023-06-19 00:26:53.000000 kanu-0.7.0/kanu.egg-info/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)      276 2023-06-19 00:26:53.000000 kanu-0.7.0/kanu.egg-info/SOURCES.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-06-19 00:26:53.000000 kanu-0.7.0/kanu.egg-info/dependency_links.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-06-19 00:26:53.000000 kanu-0.7.0/kanu.egg-info/entry_points.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        5 2023-06-19 00:26:53.000000 kanu-0.7.0/kanu.egg-info/top_level.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-06-19 00:26:53.678303 kanu-0.7.0/setup.cfg
+-rw-r--r--   0 sbslee     (501) staff       (20)      627 2023-06-19 00:26:42.000000 kanu-0.7.0/setup.py
```

### Comparing `kanu-0.6.0/LICENSE` & `kanu-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kanu-0.6.0/PKG-INFO` & `kanu-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kanu
-Version: 0.6.0
+Version: 0.7.0
 Summary: A minimalistic Python-based GUI for various chatbots
 Home-page: https://github.com/sbslee/kanu
 Author: Seung-been "Steven" Lee
 Author-email: sbstevenlee@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -19,16 +19,17 @@
 There are currently two chatbots available in KANU:
 
 - [ChatGPT](#chatgpt) harnesses the power of ChatGPT, bringing it directly to your local computer
 - [DocGPT](#docgpt) allows you to effortlessly interact with your documents and ask questions about them
 
 Other features of KANU inclde:
 
-- Customize chat settings (e.g. font size and background color)
 - Customize chatbot parameters (e.g. prompt, temperature, and chunk size) by directly using the GUI or uploading a configuration file
+- Customize chat settings (e.g. font size and background color)
+- Display token counter and price monitor in chat window
 
 ## Installation
 
 The recommended way is via pip:
 
 ```
 $ pip install kanu
@@ -57,26 +58,21 @@
 ```
 
 <a id="docgpt"></a>
 ### DocGPT
 
 ![Alt Text](https://raw.githubusercontent.com/sbslee/kanu/main/images/docgpt.gif)
 
-The following document formats are supported by DocGPT:
-
-- .txt
-- .pdf
-- .doc and .docx
-- .csv
+DocGPT currently supports the following document formats: `.csv`, `.doc`, `.docx`, `.pdf`, and `.txt`.
 
 The following packages are required to run DocGPT:
 
 ```
 langchain    # Required.
-chromadb     # Required. 
+chromadb     # Required.
 tiktoken     # Required.
 pdfminer.six # Optional. Only required for .pdf documents.
 unstructured # Optional. Only required for .doc and .docx documents.
 tabulate     # Optional. Only required for .doc and .docx documents.
 ```
 
 ## Changelog
```

### Comparing `kanu-0.6.0/README.md` & `kanu-0.7.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 There are currently two chatbots available in KANU:
 
 - [ChatGPT](#chatgpt) harnesses the power of ChatGPT, bringing it directly to your local computer
 - [DocGPT](#docgpt) allows you to effortlessly interact with your documents and ask questions about them
 
 Other features of KANU inclde:
 
-- Customize chat settings (e.g. font size and background color)
 - Customize chatbot parameters (e.g. prompt, temperature, and chunk size) by directly using the GUI or uploading a configuration file
+- Customize chat settings (e.g. font size and background color)
+- Display token counter and price monitor in chat window
 
 ## Installation
 
 The recommended way is via pip:
 
 ```
 $ pip install kanu
@@ -45,26 +46,21 @@
 ```
 
 <a id="docgpt"></a>
 ### DocGPT
 
 ![Alt Text](https://raw.githubusercontent.com/sbslee/kanu/main/images/docgpt.gif)
 
-The following document formats are supported by DocGPT:
-
-- .txt
-- .pdf
-- .doc and .docx
-- .csv
+DocGPT currently supports the following document formats: `.csv`, `.doc`, `.docx`, `.pdf`, and `.txt`.
 
 The following packages are required to run DocGPT:
 
 ```
 langchain    # Required.
-chromadb     # Required. 
+chromadb     # Required.
 tiktoken     # Required.
 pdfminer.six # Optional. Only required for .pdf documents.
 unstructured # Optional. Only required for .doc and .docx documents.
 tabulate     # Optional. Only required for .doc and .docx documents.
 ```
 
 ## Changelog
```

### Comparing `kanu-0.6.0/kanu/__main__.py` & `kanu-0.7.0/kanu/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import configparser
 import tkinter as tk
+from tkinter import ttk
 from tkinter import filedialog
 import importlib.util
 
 from .version import __version__
-from .utils import Tooltip
+from .gui import Tooltip
 
+GPT_MODELS = ["gpt-3.5-turbo", "gpt-3.5-turbo-16k", "gpt-4", "gpt-4-32k"]
 CHATGPT_PROMPT = """You are a helpful assistant."""
 DOCGPT_PROMPT = """Use the following pieces of context to answer the question at the end. If you don't know the answer, just say that you don't know, don't try to make up an answer.
 
 {context}
 
 Question: {question}
 Helpful Answer:"""
 
 class KANU:
     def __init__(self, root):
         self.container = None
         self.root = root
         self.root.title(f"KANU ({__version__})")
-        self.root.geometry("600x620")
+        self.root.geometry("700x620")
         self.homepage()
 
     def homepage(self):
         if self.container is not None:
             self.container.pack_forget()
         self.container = tk.Frame(self.root)
         self.container.pack()
@@ -47,21 +49,19 @@
         m.grid(row=3, column=0, columnspan=2)
         b = tk.Button(self.container, text="Browse", command=self.parse_chatgpt_config)
         b.grid(row=4, column=0)
         b = tk.Button(self.container, text="Template", command=self.template_chatgpt_config)
         b.grid(row=4, column=1)
         m = tk.Message(self.container, width=300, text="Option 2. Configure manually")
         m.grid(row=5, column=0, columnspan=2)
-        self.model = tk.StringVar(self.container, value="gpt-3.5-turbo")
         l = tk.Label(self.container, text="Model:")
         l.grid(row=6, column=0, columnspan=2)
-        b = tk.Radiobutton(self.container, variable=self.model, text="gpt-3.5-turbo", value="gpt-3.5-turbo")
-        b.grid(row=7, column=0)
-        b = tk.Radiobutton(self.container, variable=self.model, text="gpt-4", value="gpt-4")
-        b.grid(row=7, column=1)
+        self.model = tk.StringVar(self.container, value="gpt-3.5-turbo")
+        om = ttk.OptionMenu(self.container, self.model, *GPT_MODELS)
+        om.grid(row=7, column=0, columnspan=2)
         l = tk.Label(self.container, text="System message ⓘ:")
         Tooltip(l, "The system message helps set the behavior of the chatbot.")
         l.grid(row=8, column=0, columnspan=2)
         self.prompt = tk.Text(self.container, height=9, width=42)
         sb = tk.Scrollbar(self.container, command=self.prompt.yview)
         self.prompt.insert("1.0", CHATGPT_PROMPT)
         self.prompt.grid(row=9, column=0, columnspan=2, sticky="nsew")
@@ -123,18 +123,16 @@
         b = tk.Button(self.container, text="Template", command=self.template_docgpt_config)
         b.grid(row=10, column=1)
         m = tk.Message(self.container, width=300, text="Option 2. Configure manually")
         m.grid(row=11, column=0, columnspan=2)
         self.model = tk.StringVar(self.container, value="gpt-3.5-turbo")
         l = tk.Label(self.container, text="Model:")
         l.grid(row=12, column=0, columnspan=2)
-        rb = tk.Radiobutton(self.container, variable=self.model, text="gpt-3.5-turbo", value="gpt-3.5-turbo")
-        rb.grid(row=13, column=0)
-        rb = tk.Radiobutton(self.container, variable=self.model, text="gpt-4", value="gpt-4")
-        rb.grid(row=13, column=1)
+        om = ttk.OptionMenu(self.container, self.model, *GPT_MODELS)
+        om.grid(row=13, column=0, columnspan=2)
         l = tk.Label(self.container, text="System message ⓘ:")
         Tooltip(l, "The system message helps set the behavior of the chatbot.")
         l.grid(row=14, column=0, columnspan=2)
         self.prompt = tk.Text(self.container, height=9, width=42)
         sb = tk.Scrollbar(self.container, command=self.prompt.yview)
         self.prompt.insert("1.0", DOCGPT_PROMPT)
         self.prompt.grid(row=15, column=0, columnspan=2, sticky="nsew")
@@ -157,23 +155,35 @@
 
     def parse_docgpt_config(self):
         config = configparser.ConfigParser()
         file_path = filedialog.askopenfilename()
         if not file_path:
             return
         config.read(file_path)
-        self.deploy_agent("DocGPT", config["USER"]["openai_key"], config["DEFAULT"]["model"], float(config["DEFAULT"]["temperature"]), config["DEFAULT"]["prompt"], config["DEFAULT"]["chunk_size"], config["DEFAULT"]["chunk_overlap"])
+        self.deploy_agent(
+            "DocGPT",
+            config["USER"]["openai_key"],
+            config["DEFAULT"]["model"],
+            float(config["DEFAULT"]["temperature"]),
+            config["DEFAULT"]["prompt"],
+            config["DEFAULT"]["chunk_size"],
+            config["DEFAULT"]["chunk_overlap"],
+            config["OPTIONAL"]["new_database_directory"],
+            config["OPTIONAL"]["document_directory"],
+            config["OPTIONAL"]["existing_database_directory"],
+        )
 
     def template_docgpt_config(self):
         file_path = filedialog.asksaveasfilename()
         if not file_path:
             return
         config = configparser.ConfigParser()
         config["DEFAULT"] = {"model": "gpt-3.5-turbo", "temperature": "0.5", "prompt": DOCGPT_PROMPT, "chunk_size": 1000, "chunk_overlap": 50}
         config["USER"] = {"openai_key": ""}
+        config["OPTIONAL"] = {"new_database_directory": "", "document_directory": "", "existing_database_directory": ""}
         with open(file_path, "w") as f:
             config.write(f)
 
     def deploy_agent(self, agent, *args, **kwargs):
         if agent == "ChatGPT":
             from .chatgpt import ChatGPT
             chatgpt = ChatGPT(self, *args, **kwargs)
```

### Comparing `kanu-0.6.0/kanu/docgpt.py` & `kanu-0.7.0/kanu/docgpt.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,47 +5,68 @@
 from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.vectorstores import Chroma
 from langchain.chat_models import ChatOpenAI
 from langchain.chains import ConversationalRetrievalChain
 from langchain.prompts import PromptTemplate
 from langchain.memory import ConversationBufferMemory
-
+from langchain.callbacks import get_openai_callback
 from langchain.document_loaders import (
     TextLoader,
     PDFMinerLoader,
     UnstructuredWordDocumentLoader,
     CSVLoader,
 )
 
-from .utils import Tooltip, Settings
+from .gui import Tooltip, Settings, Conversation
+from .utils import tokens2price, text2tokens
 
 DOCUMENT_LOADERS = {
     ".txt": (TextLoader, {"encoding": "utf8"}),
     ".pdf": (PDFMinerLoader, {}),
     ".doc": (UnstructuredWordDocumentLoader, {}),
     ".docx": (UnstructuredWordDocumentLoader, {}),
     ".csv": (CSVLoader, {}),
 }
 
 class DocGPT:
-    def __init__(self, kanu, openai_key, model, temperature, prompt, default_chunk_size, default_chunk_overlap):
+    def __init__(
+        self,
+        kanu,
+        openai_key,
+        model,
+        temperature,
+        prompt,
+        default_chunk_size,
+        default_chunk_overlap,
+        new_database_directory="",
+        document_directory="",
+        existing_database_directory="",
+    ):
         self.kanu = kanu
         self.model = model
         self.temperature = temperature
         self.prompt = prompt
         self.default_chunk_size = default_chunk_size
         self.default_chunk_overlap = default_chunk_overlap
         os.environ["OPENAI_API_KEY"] = openai_key
         self.settings = Settings(self)
+        self.conversation = Conversation(self)
+        self.tokens = 0
+        self.price = 0
+        self.new_database_directory = new_database_directory
+        self.document_directory = document_directory
+        self.existing_database_directory = existing_database_directory
 
     def run(self):
         self.kanu.container.pack_forget()
         self.kanu.container = tk.Frame(self.kanu.root)
         self.kanu.container.pack()
+        self.kanu.container.bind_all("<Return>", lambda event: self.send_message())
+        self.kanu.container.focus_set()
         l = tk.Label(self.kanu.container, text="DocGPT")
         l.grid(row=0, column=0, columnspan=3)
         b = tk.Button(self.kanu.container, text="Go back", command=lambda: self.kanu.config_docgpt())
         b.grid(row=1, column=0)
         b = tk.Button(self.kanu.container, text="Reload", command=lambda: self.run())
         b.grid(row=1, column=2)
         m = tk.Message(self.kanu.container, width=300, text="Option 1. Create a new database")
@@ -80,79 +101,90 @@
         self.option1_button.grid(row=7, column=0, columnspan=3)
         self.option1_button["state"] = tk.DISABLED
         m = tk.Message(self.kanu.container, width=300, text="Option 2. Use an existing database")
         m.grid(row=8, column=0, columnspan=3)
         l = tk.Label(self.kanu.container, text="Database ⓘ:")
         Tooltip(l, "Directory where the database is stored.")
         l.grid(row=9, column=0)
-        self.old_database_label = tk.Label(self.kanu.container, text="Not selected", fg="red")
-        self.old_database_label.grid(row=9, column=1)
-        b = tk.Button(self.kanu.container, text="Browse", command=self.specify_old_database_directory)
+        self.existing_database_label = tk.Label(self.kanu.container, text="Not selected", fg="red")
+        self.existing_database_label.grid(row=9, column=1)
+        b = tk.Button(self.kanu.container, text="Browse", command=self.specify_existing_database_directory)
         b.grid(row=9, column=2)
         self.option2_button = tk.Button(self.kanu.container, text="Go with Option 2", command=self.go_with_option2)
         self.option2_button.grid(row=10, column=0, columnspan=3)
         self.option2_button["state"] = tk.DISABLED
+        if self.new_database_directory:
+            self.new_database_label.configure(text=os.path.basename(self.new_database_directory), fg="lime green")
+        if self.document_directory:
+            self.document_label.configure(text=os.path.basename(self.document_directory), fg="lime green")
+        if self.new_database_label["text"] != "Not selected" and self.document_label["text"] != "Not selected":
+            self.option1_button["state"] = tk.NORMAL
+        if self.existing_database_directory:
+            self.existing_database_label.configure(text=os.path.basename(self.existing_database_directory), fg="lime green")
+            self.option2_button["state"] = tk.NORMAL
 
     def query(self):
         self.memory = ConversationBufferMemory(memory_key="chat_history", return_messages=True)
         self.db = Chroma(persist_directory=self.database_directory, embedding_function=OpenAIEmbeddings())
         self.qa = ConversationalRetrievalChain.from_llm(
             llm=ChatOpenAI(model_name=self.model, temperature=self.temperature),
             retriever=self.db.as_retriever(),
             memory=self.memory,
             chain_type="stuff",
             combine_docs_chain_kwargs={"prompt": PromptTemplate(template=self.prompt, input_variables=["context", "question"])}
         )
-        self.kanu.container.pack_forget()
-        self.kanu.container = tk.Frame(self.kanu.root)
-        self.kanu.container.pack()
-        l = tk.Label(self.kanu.container, text="DocGPT")
-        l.grid(row=0, column=0, columnspan=4)    
-        self.session = tk.Text(self.kanu.container, width=70, height=20)
-        self.session.grid(row=1, column=0, columnspan=4)
-        self.session.tag_config("user", **self.settings.get_user_kwargs())
-        self.session.tag_config("bot", **self.settings.get_bot_kwargs())
-        user_input = tk.Entry(self.kanu.container, width=54)
-        user_input.grid(row=2, column=0, columnspan=4)
-        b = tk.Button(self.kanu.container, text="Send", command=lambda: self.send_message(user_input))
-        b.grid(row=3, column=0)
-        b = tk.Button(self.kanu.container, text="Clear", command=lambda: self.clear_session())
-        b.grid(row=3, column=1)
-        b = tk.Button(self.kanu.container, text="Go back", command=lambda: self.run())
-        b.grid(row=3, column=2)
-        b = tk.Button(self.kanu.container, text="Settings", command=lambda: self.settings.page())
-        b.grid(row=3, column=3)
+        self.conversation.page()
 
-    def send_message(self, entry):
-        self.session.insert(tk.END, "You: " + entry.get() + "\n", "user")
-        response = self.qa(entry.get())["answer"]
-        self.session.insert(tk.END, "Bot: " + response + "\n", "bot")
-        entry.delete(0, tk.END)
+    def send_message(self):
+        self.session.insert(tk.END, "You: " + self.user_input.get() + "\n", "user")
+        with get_openai_callback() as cb:
+            response = self.qa(self.user_input.get())
+            usage = self.calculate_usage(cb)
+        self.session.insert(tk.END, "Bot: " + response["answer"] + "\n", "bot")
+        self.system.insert(tk.END, f"{usage}\n", "system")
+        self.chatbox.delete(0, tk.END)
+
+    def calculate_usage(self, cb):
+        prompt_price = tokens2price(self.model, "prompt", cb.prompt_tokens)
+        completion_price = tokens2price(self.model, "completion", cb.completion_tokens)
+        self.price += prompt_price + completion_price
+        self.tokens += cb.total_tokens
+        message = f"System: Used {cb.prompt_tokens:,} prompt + {cb.completion_tokens:,} completion = {cb.total_tokens:,} tokens (total: {self.tokens:,} or ${self.price:.6f})."
+        return message
 
     def go_with_option1(self):
+        self.database_directory = self.new_database_directory
+        self.tokens = self.price = 0
         documents = []
         for root, dirs, files in os.walk(self.document_directory):
             for file in files:
                 file_path = os.path.join(root, file)
                 file_ext = os.path.splitext(file_path)[1]
                 if file_ext not in DOCUMENT_LOADERS:
                     continue
                 loader_class, loader_kwargs = DOCUMENT_LOADERS[file_ext]
                 loader = loader_class(file_path, **loader_kwargs)
                 document = loader.load()
                 documents.extend(document)
         text_splitter = RecursiveCharacterTextSplitter(chunk_size=self.chunk_size.get(), chunk_overlap=self.chunk_overlap.get())
         texts = text_splitter.split_documents(documents)
-        db = Chroma.from_documents(texts, OpenAIEmbeddings(), persist_directory=self.database_directory)
+        for text in texts:
+            self.tokens += text2tokens("text-embedding-ada-002", text.page_content)
+        self.price = tokens2price("text-embedding-ada-002", "embedding", self.tokens)
+        db = Chroma.from_documents(texts, OpenAIEmbeddings(model="text-embedding-ada-002"), persist_directory=self.database_directory)
         db.add_documents(texts)
         db.persist()
         db = None
+        self.existing = False
         self.query()
 
     def go_with_option2(self):
+        self.database_directory = self.existing_database_directory
+        self.tokens = self.price = 0
+        self.existing = True
         self.query()
 
     def specify_document_directory(self):
         directory_path = filedialog.askdirectory()
         if not directory_path:
             return
         self.document_directory = directory_path
@@ -160,23 +192,24 @@
         if self.new_database_label["text"] != "Not selected":
             self.option1_button["state"] = tk.NORMAL
 
     def specify_new_database_directory(self):
         directory_path = filedialog.askdirectory()
         if not directory_path:
             return
-        self.database_directory = directory_path
+        self.new_database_directory = directory_path
         self.new_database_label.configure(text=os.path.basename(directory_path), fg="lime green")
         if self.document_label["text"] != "No file selected":
             self.option1_button["state"] = tk.NORMAL
 
-    def specify_old_database_directory(self):
+    def specify_existing_database_directory(self):
         directory_path = filedialog.askdirectory()
         if not directory_path:
             return
-        self.database_directory = directory_path
-        self.old_database_label.configure(text=os.path.basename(directory_path), fg="lime green")
+        self.existing_database_directory = directory_path
+        self.existing_database_label.configure(text=os.path.basename(directory_path), fg="lime green")
         self.option2_button["state"] = tk.NORMAL
 
     def clear_session(self):
-        self.session.delete(1.0, tk.END)
-
+        self.existing = True
+        self.tokens = self.price = 0
+        self.query()
```

### Comparing `kanu-0.6.0/kanu.egg-info/PKG-INFO` & `kanu-0.7.0/kanu.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kanu
-Version: 0.6.0
+Version: 0.7.0
 Summary: A minimalistic Python-based GUI for various chatbots
 Home-page: https://github.com/sbslee/kanu
 Author: Seung-been "Steven" Lee
 Author-email: sbstevenlee@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -19,16 +19,17 @@
 There are currently two chatbots available in KANU:
 
 - [ChatGPT](#chatgpt) harnesses the power of ChatGPT, bringing it directly to your local computer
 - [DocGPT](#docgpt) allows you to effortlessly interact with your documents and ask questions about them
 
 Other features of KANU inclde:
 
-- Customize chat settings (e.g. font size and background color)
 - Customize chatbot parameters (e.g. prompt, temperature, and chunk size) by directly using the GUI or uploading a configuration file
+- Customize chat settings (e.g. font size and background color)
+- Display token counter and price monitor in chat window
 
 ## Installation
 
 The recommended way is via pip:
 
 ```
 $ pip install kanu
@@ -57,26 +58,21 @@
 ```
 
 <a id="docgpt"></a>
 ### DocGPT
 
 ![Alt Text](https://raw.githubusercontent.com/sbslee/kanu/main/images/docgpt.gif)
 
-The following document formats are supported by DocGPT:
-
-- .txt
-- .pdf
-- .doc and .docx
-- .csv
+DocGPT currently supports the following document formats: `.csv`, `.doc`, `.docx`, `.pdf`, and `.txt`.
 
 The following packages are required to run DocGPT:
 
 ```
 langchain    # Required.
-chromadb     # Required. 
+chromadb     # Required.
 tiktoken     # Required.
 pdfminer.six # Optional. Only required for .pdf documents.
 unstructured # Optional. Only required for .doc and .docx documents.
 tabulate     # Optional. Only required for .doc and .docx documents.
 ```
 
 ## Changelog
```

### Comparing `kanu-0.6.0/setup.py` & `kanu-0.7.0/setup.py`

 * *Files identical despite different names*

