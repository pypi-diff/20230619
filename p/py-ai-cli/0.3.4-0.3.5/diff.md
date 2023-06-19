# Comparing `tmp/py-ai-cli-0.3.4.tar.gz` & `tmp/py-ai-cli-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ai-cli-0.3.4.tar", last modified: Wed May 31 09:09:44 2023, max compression
+gzip compressed data, was "py-ai-cli-0.3.5.tar", last modified: Mon Jun 19 07:35:20 2023, max compression
```

## Comparing `py-ai-cli-0.3.4.tar` & `py-ai-cli-0.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1830 2023-05-31 09:09:25.696531 py-ai-cli-0.3.4/CHANGELOG.md
--rw-r--r--   0        0        0     1092 2023-05-31 09:09:25.696531 py-ai-cli-0.3.4/LICENSE
--rw-r--r--   0        0        0     3363 2023-05-31 09:09:25.696531 py-ai-cli-0.3.4/README.md
--rw-r--r--   0        0        0     3940 2023-05-31 09:09:25.696531 py-ai-cli-0.3.4/README_ja.md
--rw-r--r--   0        0        0     2922 2023-05-31 09:09:25.696531 py-ai-cli-0.3.4/README_zh.md
--rw-r--r--   0        0        0     2021 2023-05-31 09:09:26.040537 py-ai-cli-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      680 2023-05-31 09:09:26.040537 py-ai-cli-0.3.4/src/ai_cli/__init__.py
--rw-r--r--   0        0        0     8380 2023-05-31 09:09:26.040537 py-ai-cli-0.3.4/src/ai_cli/bot/__init__.py
--rw-r--r--   0        0        0      195 2023-05-31 09:09:26.040537 py-ai-cli-0.3.4/src/ai_cli/bot/token.py
--rwxr-xr-x   0        0        0    13721 2023-05-31 09:09:26.040537 py-ai-cli-0.3.4/src/ai_cli/cli.py
--rw-r--r--   0        0        0     4474 2023-05-31 09:09:26.040537 py-ai-cli-0.3.4/src/ai_cli/git.py
--rw-r--r--   0        0        0     4400 2023-05-31 09:09:26.040537 py-ai-cli-0.3.4/src/ai_cli/setting.py
--rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 py-ai-cli-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1942 2023-06-19 07:35:01.198090 py-ai-cli-0.3.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1092 2023-06-19 07:35:01.198090 py-ai-cli-0.3.5/LICENSE
+-rw-r--r--   0        0        0     3363 2023-06-19 07:35:01.198090 py-ai-cli-0.3.5/README.md
+-rw-r--r--   0        0        0     3940 2023-06-19 07:35:01.198090 py-ai-cli-0.3.5/README_ja.md
+-rw-r--r--   0        0        0     2922 2023-06-19 07:35:01.198090 py-ai-cli-0.3.5/README_zh.md
+-rw-r--r--   0        0        0     2021 2023-06-19 07:35:01.602087 py-ai-cli-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      680 2023-06-19 07:35:01.602087 py-ai-cli-0.3.5/src/ai_cli/__init__.py
+-rw-r--r--   0        0        0     8388 2023-06-19 07:35:01.602087 py-ai-cli-0.3.5/src/ai_cli/bot/__init__.py
+-rw-r--r--   0        0        0      195 2023-06-19 07:35:01.602087 py-ai-cli-0.3.5/src/ai_cli/bot/token.py
+-rwxr-xr-x   0        0        0    14028 2023-06-19 07:35:01.602087 py-ai-cli-0.3.5/src/ai_cli/cli.py
+-rw-r--r--   0        0        0     4474 2023-06-19 07:35:01.602087 py-ai-cli-0.3.5/src/ai_cli/git.py
+-rw-r--r--   0        0        0     4400 2023-06-19 07:35:01.602087 py-ai-cli-0.3.5/src/ai_cli/setting.py
+-rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 py-ai-cli-0.3.5/PKG-INFO
```

### Comparing `py-ai-cli-0.3.4/CHANGELOG.md` & `py-ai-cli-0.3.5/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Release v0.3.5
+---------------------------
+
+- fix: EdgeGPT bot error
+- `commit` command add user-prompt option
+
 Release v0.3.4
 ---------------------------
 
 - fix: `commit` command error when delete file from git
 
 Release v0.3.2
 ---------------------------
```

### Comparing `py-ai-cli-0.3.4/LICENSE` & `py-ai-cli-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.4/README.md` & `py-ai-cli-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.4/README_ja.md` & `py-ai-cli-0.3.5/README_ja.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.4/README_zh.md` & `py-ai-cli-0.3.5/README_zh.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.4/pyproject.toml` & `py-ai-cli-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     "pysocks>=1.7.1",
     "pyperclip>=1.8.2",
     "EdgeGPT>=0.1.22.1",
     "tiktoken>=0.3.3",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.3.4"
+version = "0.3.5"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Repository = "https://github.com/yufeikang/ai-cli"
 Documentation = "https://github.com/yufeikang/ai-cli/blob/main/README.md"
```

### Comparing `py-ai-cli-0.3.4/src/ai_cli/__init__.py` & `py-ai-cli-0.3.5/src/ai_cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.4"
+__version__ = "0.3.5"
 
 import logging
 from logging.handlers import RotatingFileHandler
 from pathlib import Path
 
 HOME = Path.home()
```

### Comparing `py-ai-cli-0.3.4/src/ai_cli/bot/__init__.py` & `py-ai-cli-0.3.5/src/ai_cli/bot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from typing import Generator, Union
 from uuid import uuid4
 
 import openai
-from EdgeGPT import Chatbot, ConversationStyle
+from EdgeGPT.EdgeGPT import Chatbot, ConversationStyle
 
 from ai_cli.bot.token import get_token_count
 from ai_cli.setting import Setting
 
 logger = logging.getLogger(__name__)
```

### Comparing `py-ai-cli-0.3.4/src/ai_cli/cli.py` & `py-ai-cli-0.3.5/src/ai_cli/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -204,14 +204,22 @@
     "--message",
     "-m",
     dest="message",
     type=str,
     nargs="?",
     help="the extra message to add to the commit message",
 )
+commit_parser.add_argument(
+    "--user-prompt",
+    "-up",
+    dest="user_prompt",
+    type=str,
+    nargs="?",
+    help="enable user prompt mode, this will let you input the commit message",
+)
 
 args = parser.parse_args()
 
 init_logging(setting.log_level.get_value() if not args.debug else "DEBUG")
 
 logger = logging.getLogger(__name__)
 
@@ -404,15 +412,18 @@
         exit(0)
     diff_files = git.get_change_files("HEAD")
     if not diff_files or len(diff_files) == 0:
         console.print("[bold red]No diff files found")
         exit(0)
     console.print(f"[bold blue]Found {len(diff_files)} files changed[/bold blue]")
     diff = git.get_file_diff(diff_files, "HEAD")
-    message = f"{setting.commit_prompt.get_value()} \n\n {diff}"
+    prompt = setting.commit_prompt.get_value()
+    if args.user_prompt:
+        prompt = f"{prompt} \n\n user ask:{args.user_prompt} \n\n"
+    message = f"{prompt} \n\n {diff}"
     result = ask(message, stream=False).strip()
     if args.message:
         result = result + "\n\n" + args.message
     action = Prompt.ask(
         "[bold blue]Do you want to commit these changes?[/bold blue] [(Yes)y/(No)n/(Edit)e]",
         choices=["y", "n", "e"],
         show_choices=False,
```

### Comparing `py-ai-cli-0.3.4/src/ai_cli/git.py` & `py-ai-cli-0.3.5/src/ai_cli/git.py`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.4/src/ai_cli/setting.py` & `py-ai-cli-0.3.5/src/ai_cli/setting.py`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.4/PKG-INFO` & `py-ai-cli-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ai_cli
-Version: 0.3.4
+Version: 0.3.5
 Summary: This CLI tool allows you to easily chat with chatGPT in the command line. You can chat with it, ask questions, and even translate text. It also
 License: MIT
 Author-email: Yufei Kang <kou.uhi.x@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Documentation, https://github.com/yufeikang/ai-cli/blob/main/README.md
 Project-URL: Repository, https://github.com/yufeikang/ai-cli
 Description-Content-Type: text/markdown
```

