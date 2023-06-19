# Comparing `tmp/cligpt-2.7.2.tar.gz` & `tmp/cligpt-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cligpt-2.7.2.tar", last modified: Wed Mar 15 20:07:43 2023, max compression
+gzip compressed data, was "cligpt-2.8.tar", last modified: Mon Jun 19 10:23:46 2023, max compression
```

## Comparing `cligpt-2.7.2.tar` & `cligpt-2.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ramdrop    (501) staff       (20)        0 2023-03-15 20:07:43.793457 cligpt-2.7.2/
--rw-r--r--   0 ramdrop    (501) staff       (20)     1073 2023-03-08 18:32:27.000000 cligpt-2.7.2/LICENSE
--rw-r--r--   0 ramdrop    (501) staff       (20)       26 2023-03-09 20:58:46.000000 cligpt-2.7.2/MANIFEST.in
--rw-r--r--   0 ramdrop    (501) staff       (20)     1871 2023-03-15 20:07:43.793269 cligpt-2.7.2/PKG-INFO
--rw-r--r--   0 ramdrop    (501) staff       (20)     1382 2023-03-15 18:53:16.000000 cligpt-2.7.2/README.md
--rw-r--r--   0 ramdrop    (501) staff       (20)       84 2023-03-08 18:32:34.000000 cligpt-2.7.2/pyproject.toml
--rw-r--r--   0 ramdrop    (501) staff       (20)       38 2023-03-15 20:07:43.793510 cligpt-2.7.2/setup.cfg
--rw-r--r--   0 ramdrop    (501) staff       (20)      979 2023-03-15 20:07:24.000000 cligpt-2.7.2/setup.py
-drwxr-xr-x   0 ramdrop    (501) staff       (20)        0 2023-03-15 20:07:43.789218 cligpt-2.7.2/src/
-drwxr-xr-x   0 ramdrop    (501) staff       (20)        0 2023-03-15 20:07:43.791537 cligpt-2.7.2/src/cligpt/
--rw-r--r--   0 ramdrop    (501) staff       (20)        0 2023-03-09 18:13:11.000000 cligpt-2.7.2/src/cligpt/__init__.py
--rw-r--r--   0 ramdrop    (501) staff       (20)       60 2023-03-14 18:25:28.000000 cligpt-2.7.2/src/cligpt/__main__.py
--rw-r--r--   0 ramdrop    (501) staff       (20)     1621 2023-03-15 18:40:58.000000 cligpt-2.7.2/src/cligpt/cli.py
--rw-r--r--   0 ramdrop    (501) staff       (20)     7649 2023-03-15 20:06:34.000000 cligpt-2.7.2/src/cligpt/cligpt.py
--rw-r--r--   0 ramdrop    (501) staff       (20)      250 2023-03-10 12:27:51.000000 cligpt-2.7.2/src/cligpt/config.json
-drwxr-xr-x   0 ramdrop    (501) staff       (20)        0 2023-03-15 20:07:43.792890 cligpt-2.7.2/src/cligpt.egg-info/
--rw-r--r--   0 ramdrop    (501) staff       (20)     1871 2023-03-15 20:07:43.000000 cligpt-2.7.2/src/cligpt.egg-info/PKG-INFO
--rw-r--r--   0 ramdrop    (501) staff       (20)      380 2023-03-15 20:07:43.000000 cligpt-2.7.2/src/cligpt.egg-info/SOURCES.txt
--rw-r--r--   0 ramdrop    (501) staff       (20)        1 2023-03-15 20:07:43.000000 cligpt-2.7.2/src/cligpt.egg-info/dependency_links.txt
--rw-r--r--   0 ramdrop    (501) staff       (20)       43 2023-03-15 20:07:43.000000 cligpt-2.7.2/src/cligpt.egg-info/entry_points.txt
--rw-r--r--   0 ramdrop    (501) staff       (20)       12 2023-03-15 20:07:43.000000 cligpt-2.7.2/src/cligpt.egg-info/requires.txt
--rw-r--r--   0 ramdrop    (501) staff       (20)        7 2023-03-15 20:07:43.000000 cligpt-2.7.2/src/cligpt.egg-info/top_level.txt
-drwxr-xr-x   0 ramdrop    (501) staff       (20)        0 2023-03-15 20:07:43.793073 cligpt-2.7.2/test/
--rw-r--r--   0 ramdrop    (501) staff       (20)        0 2023-03-09 20:14:27.000000 cligpt-2.7.2/test/test.py
+drwxr-xr-x   0 ramdrop    (501) staff       (20)        0 2023-06-19 10:23:46.475017 cligpt-2.8/
+-rw-r--r--   0 ramdrop    (501) staff       (20)     1073 2023-03-08 18:32:27.000000 cligpt-2.8/LICENSE
+-rw-r--r--   0 ramdrop    (501) staff       (20)       26 2023-03-09 20:58:46.000000 cligpt-2.8/MANIFEST.in
+-rw-r--r--   0 ramdrop    (501) staff       (20)     1884 2023-06-19 10:23:46.474852 cligpt-2.8/PKG-INFO
+-rw-r--r--   0 ramdrop    (501) staff       (20)     1397 2023-06-19 10:22:05.000000 cligpt-2.8/README.md
+-rw-r--r--   0 ramdrop    (501) staff       (20)       84 2023-03-08 18:32:34.000000 cligpt-2.8/pyproject.toml
+-rw-r--r--   0 ramdrop    (501) staff       (20)       38 2023-06-19 10:23:46.475058 cligpt-2.8/setup.cfg
+-rw-r--r--   0 ramdrop    (501) staff       (20)      990 2023-03-16 11:20:28.000000 cligpt-2.8/setup.py
+drwxr-xr-x   0 ramdrop    (501) staff       (20)        0 2023-06-19 10:23:46.467353 cligpt-2.8/src/
+drwxr-xr-x   0 ramdrop    (501) staff       (20)        0 2023-06-19 10:23:46.469935 cligpt-2.8/src/cligpt/
+-rw-r--r--   0 ramdrop    (501) staff       (20)        0 2023-03-09 18:13:11.000000 cligpt-2.8/src/cligpt/__init__.py
+-rw-r--r--   0 ramdrop    (501) staff       (20)       60 2023-03-14 18:25:28.000000 cligpt-2.8/src/cligpt/__main__.py
+-rw-r--r--   0 ramdrop    (501) staff       (20)     2277 2023-03-16 11:19:54.000000 cligpt-2.8/src/cligpt/cli.py
+-rw-r--r--   0 ramdrop    (501) staff       (20)     7469 2023-03-15 21:42:42.000000 cligpt-2.8/src/cligpt/cligpt.py
+-rw-r--r--   0 ramdrop    (501) staff       (20)      250 2023-03-10 12:27:51.000000 cligpt-2.8/src/cligpt/config.json
+drwxr-xr-x   0 ramdrop    (501) staff       (20)        0 2023-06-19 10:23:46.474428 cligpt-2.8/src/cligpt.egg-info/
+-rw-r--r--   0 ramdrop    (501) staff       (20)     1884 2023-06-19 10:23:46.000000 cligpt-2.8/src/cligpt.egg-info/PKG-INFO
+-rw-r--r--   0 ramdrop    (501) staff       (20)      380 2023-06-19 10:23:46.000000 cligpt-2.8/src/cligpt.egg-info/SOURCES.txt
+-rw-r--r--   0 ramdrop    (501) staff       (20)        1 2023-06-19 10:23:46.000000 cligpt-2.8/src/cligpt.egg-info/dependency_links.txt
+-rw-r--r--   0 ramdrop    (501) staff       (20)       43 2023-06-19 10:23:46.000000 cligpt-2.8/src/cligpt.egg-info/entry_points.txt
+-rw-r--r--   0 ramdrop    (501) staff       (20)       22 2023-06-19 10:23:46.000000 cligpt-2.8/src/cligpt.egg-info/requires.txt
+-rw-r--r--   0 ramdrop    (501) staff       (20)        7 2023-06-19 10:23:46.000000 cligpt-2.8/src/cligpt.egg-info/top_level.txt
+drwxr-xr-x   0 ramdrop    (501) staff       (20)        0 2023-06-19 10:23:46.474644 cligpt-2.8/test/
+-rw-r--r--   0 ramdrop    (501) staff       (20)        0 2023-03-09 20:14:27.000000 cligpt-2.8/test/test.py
```

### Comparing `cligpt-2.7.2/LICENSE` & `cligpt-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cligpt-2.7.2/PKG-INFO` & `cligpt-2.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,84 @@
 Metadata-Version: 2.1
 Name: cligpt
-Version: 2.7.2
+Version: 2.8
 Summary: A handy CLI interface for ChatGPT
 Home-page: http://www.example.com/~cschultz/bvote/
 Author: skvn
 Author-email: xxx@gmail.com
 Project-URL: Bug Tracker, http://bitbucket.org/tarek/distribute/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Command Line Inferface for ChatGPT
 
-### Installation 
+## Installation
+
 ```shell
 pip install --upgrade cligpt
 ```
 
-### Getting Started
+## Getting Started
+
 ```shell
 # Fill in your OpenAI API key
 export OPENAI_API_KEY=[sk-xxxx]
 
 # Launch
 cligpt
 
 # Switch roles (you may use abbreviations as long as they do not clash with other roles)
 @revise (or @revis | @revi | @rev | @re | @r)
 ```
 
-### Advanced Options
+## Advanced Options
 
 - Customize your roles
-    
+
     Edit the configuration file:
-    ```
+
+    ```shell
     vim ~/.cligpt/config.json
     ```
 
 - Turn on/off Auto-copy (default=on)
-    
+
     `cligpt` automatically copies the last response to your clipboard. To enable/disable it, launch `cligpt` with the following command:
-    ```
+
+    ```shell
     cligpt --no_auto_copy
     ```
+
 - Adjust context length (default=6)
-    
+
     Context length refers to the number of prompts+responses `cligpt` should remember. For example, if you want it to remember the last 3 prompts + 3 responses, launch `cligpt` with the following command:
-    ```
+
+    ```shell
     cligpt --context_length=6
     ```
 
 - Turn on/off stream mode (default=on)
 
     Stream mode displays words popping up one by one. To enable/disable it, launch `cligpt` with the following command:
-    ```
+
+    ```shell
     cligpt --no_stream
     ```
+
 - Proxy (default=None)
 
     Use a proxy for the OpenAI API:
 
-    ```
+    ```shell
     cligpt --proxy=http:127.0.0.1:9000
     ```
 
+## Uninstallation
 
-
-### Uninstallation
 ```shell
 pip uninstall cligpt
 (rm -rf ~/.cligpt)
 ```
```

### Comparing `cligpt-2.7.2/README.md` & `cligpt-2.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,69 @@
 # Command Line Inferface for ChatGPT
 
-### Installation 
+## Installation
+
 ```shell
 pip install --upgrade cligpt
 ```
 
-### Getting Started
+## Getting Started
+
 ```shell
 # Fill in your OpenAI API key
 export OPENAI_API_KEY=[sk-xxxx]
 
 # Launch
 cligpt
 
 # Switch roles (you may use abbreviations as long as they do not clash with other roles)
 @revise (or @revis | @revi | @rev | @re | @r)
 ```
 
-### Advanced Options
+## Advanced Options
 
 - Customize your roles
-    
+
     Edit the configuration file:
-    ```
+
+    ```shell
     vim ~/.cligpt/config.json
     ```
 
 - Turn on/off Auto-copy (default=on)
-    
+
     `cligpt` automatically copies the last response to your clipboard. To enable/disable it, launch `cligpt` with the following command:
-    ```
+
+    ```shell
     cligpt --no_auto_copy
     ```
+
 - Adjust context length (default=6)
-    
+
     Context length refers to the number of prompts+responses `cligpt` should remember. For example, if you want it to remember the last 3 prompts + 3 responses, launch `cligpt` with the following command:
-    ```
+
+    ```shell
     cligpt --context_length=6
     ```
 
 - Turn on/off stream mode (default=on)
 
     Stream mode displays words popping up one by one. To enable/disable it, launch `cligpt` with the following command:
-    ```
+
+    ```shell
     cligpt --no_stream
     ```
+
 - Proxy (default=None)
 
     Use a proxy for the OpenAI API:
 
-    ```
+    ```shell
     cligpt --proxy=http:127.0.0.1:9000
     ```
 
+## Uninstallation
 
-
-### Uninstallation
 ```shell
 pip uninstall cligpt
 (rm -rf ~/.cligpt)
 ```
```

### Comparing `cligpt-2.7.2/setup.py` & `cligpt-2.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cligpt",
-    version="2.7.2",
+    version="2.8",
     author="skvn",
     author_email="xxx@gmail.com",
     description="A handy CLI interface for ChatGPT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://www.example.com/~cschultz/bvote/",
     project_urls={
@@ -20,13 +20,13 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     python_requires=">=3.6",
-    install_requires=['openai', 'rich'],
+    install_requires=['openai', 'rich', 'pyperclip'],
     package_data={"": ["*.json"]},
     entry_points={
         "console_scripts": ["cligpt = cligpt.cli:main"],
     },
 )
```

### Comparing `cligpt-2.7.2/src/cligpt/cligpt.py` & `cligpt-2.8/src/cligpt/cligpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,14 @@
 from rich.panel import Panel
 from rich.logging import RichHandler
 import logging
 import pyperclip
 from rich.prompt import Prompt
 import readline
 
-logger = logging.getLogger(__name__)
-handler = RichHandler()
-
-# Set the logging level and add the handler to the logger
-logger.setLevel(logging.INFO)
-logger.addHandler(handler)
 
 
 c = Console(color_system="truecolor", soft_wrap=True)
 
 
 class CLIGPT:
     def __init__(self, openai_api_key, config_file, stream=True, proxy=None, context_length=6, auto_copy=True):
@@ -114,15 +108,15 @@
                                                                 messages=[{
                                                                     "role": "system",
                                                                     "content": f"{self.configs[self.roles[self.default_role_index]]}"
                                                                 }, {
                                                                     "role": "user",
                                                                     "content": f"{user_input}"
                                                                 }], stream=self.stream)
-                    c.print(f"[bold deep_sky_blue3]@GPT: ", end="")
+                    c.print(f"[bold bright_cyan]@GPT: ", end="")
                     if self.stream == True:
                         answer = '\n'
 
                         # # comment because markdown doesn't support soft wrap
                         # md = Markdown("")
                         # parser = MarkdownIt().enable("strikethrough")
                         # with Live(md, auto_refresh=False) as lv:
```

### Comparing `cligpt-2.7.2/src/cligpt.egg-info/PKG-INFO` & `cligpt-2.8/src/cligpt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,84 @@
 Metadata-Version: 2.1
 Name: cligpt
-Version: 2.7.2
+Version: 2.8
 Summary: A handy CLI interface for ChatGPT
 Home-page: http://www.example.com/~cschultz/bvote/
 Author: skvn
 Author-email: xxx@gmail.com
 Project-URL: Bug Tracker, http://bitbucket.org/tarek/distribute/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Command Line Inferface for ChatGPT
 
-### Installation 
+## Installation
+
 ```shell
 pip install --upgrade cligpt
 ```
 
-### Getting Started
+## Getting Started
+
 ```shell
 # Fill in your OpenAI API key
 export OPENAI_API_KEY=[sk-xxxx]
 
 # Launch
 cligpt
 
 # Switch roles (you may use abbreviations as long as they do not clash with other roles)
 @revise (or @revis | @revi | @rev | @re | @r)
 ```
 
-### Advanced Options
+## Advanced Options
 
 - Customize your roles
-    
+
     Edit the configuration file:
-    ```
+
+    ```shell
     vim ~/.cligpt/config.json
     ```
 
 - Turn on/off Auto-copy (default=on)
-    
+
     `cligpt` automatically copies the last response to your clipboard. To enable/disable it, launch `cligpt` with the following command:
-    ```
+
+    ```shell
     cligpt --no_auto_copy
     ```
+
 - Adjust context length (default=6)
-    
+
     Context length refers to the number of prompts+responses `cligpt` should remember. For example, if you want it to remember the last 3 prompts + 3 responses, launch `cligpt` with the following command:
-    ```
+
+    ```shell
     cligpt --context_length=6
     ```
 
 - Turn on/off stream mode (default=on)
 
     Stream mode displays words popping up one by one. To enable/disable it, launch `cligpt` with the following command:
-    ```
+
+    ```shell
     cligpt --no_stream
     ```
+
 - Proxy (default=None)
 
     Use a proxy for the OpenAI API:
 
-    ```
+    ```shell
     cligpt --proxy=http:127.0.0.1:9000
     ```
 
+## Uninstallation
 
-
-### Uninstallation
 ```shell
 pip uninstall cligpt
 (rm -rf ~/.cligpt)
 ```
```

