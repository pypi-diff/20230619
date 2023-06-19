# Comparing `tmp/py-ai-cli-0.3.5.tar.gz` & `tmp/py-ai-cli-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ai-cli-0.3.5.tar", last modified: Mon Jun 19 07:35:20 2023, max compression
+gzip compressed data, was "py-ai-cli-0.3.6.tar", last modified: Mon Jun 19 08:34:42 2023, max compression
```

## Comparing `py-ai-cli-0.3.5.tar` & `py-ai-cli-0.3.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1942 2023-06-19 07:35:01.198090 py-ai-cli-0.3.5/CHANGELOG.md
--rw-r--r--   0        0        0     1092 2023-06-19 07:35:01.198090 py-ai-cli-0.3.5/LICENSE
--rw-r--r--   0        0        0     3363 2023-06-19 07:35:01.198090 py-ai-cli-0.3.5/README.md
--rw-r--r--   0        0        0     3940 2023-06-19 07:35:01.198090 py-ai-cli-0.3.5/README_ja.md
--rw-r--r--   0        0        0     2922 2023-06-19 07:35:01.198090 py-ai-cli-0.3.5/README_zh.md
--rw-r--r--   0        0        0     2021 2023-06-19 07:35:01.602087 py-ai-cli-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      680 2023-06-19 07:35:01.602087 py-ai-cli-0.3.5/src/ai_cli/__init__.py
--rw-r--r--   0        0        0     8388 2023-06-19 07:35:01.602087 py-ai-cli-0.3.5/src/ai_cli/bot/__init__.py
--rw-r--r--   0        0        0      195 2023-06-19 07:35:01.602087 py-ai-cli-0.3.5/src/ai_cli/bot/token.py
--rwxr-xr-x   0        0        0    14028 2023-06-19 07:35:01.602087 py-ai-cli-0.3.5/src/ai_cli/cli.py
--rw-r--r--   0        0        0     4474 2023-06-19 07:35:01.602087 py-ai-cli-0.3.5/src/ai_cli/git.py
--rw-r--r--   0        0        0     4400 2023-06-19 07:35:01.602087 py-ai-cli-0.3.5/src/ai_cli/setting.py
--rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 py-ai-cli-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1942 2023-06-19 08:34:20.305378 py-ai-cli-0.3.6/CHANGELOG.md
+-rw-r--r--   0        0        0     1092 2023-06-19 08:34:20.305378 py-ai-cli-0.3.6/LICENSE
+-rw-r--r--   0        0        0     3363 2023-06-19 08:34:20.305378 py-ai-cli-0.3.6/README.md
+-rw-r--r--   0        0        0     3940 2023-06-19 08:34:20.305378 py-ai-cli-0.3.6/README_ja.md
+-rw-r--r--   0        0        0     2922 2023-06-19 08:34:20.305378 py-ai-cli-0.3.6/README_zh.md
+-rw-r--r--   0        0        0     2021 2023-06-19 08:34:20.709394 py-ai-cli-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      680 2023-06-19 08:34:20.709394 py-ai-cli-0.3.6/src/ai_cli/__init__.py
+-rw-r--r--   0        0        0     5509 2023-06-19 08:34:20.709394 py-ai-cli-0.3.6/src/ai_cli/bot/__init__.py
+-rw-r--r--   0        0        0     3071 2023-06-19 08:34:20.709394 py-ai-cli-0.3.6/src/ai_cli/bot/bing.py
+-rw-r--r--   0        0        0      195 2023-06-19 08:34:20.709394 py-ai-cli-0.3.6/src/ai_cli/bot/token.py
+-rwxr-xr-x   0        0        0    14028 2023-06-19 08:34:20.709394 py-ai-cli-0.3.6/src/ai_cli/cli.py
+-rw-r--r--   0        0        0     4474 2023-06-19 08:34:20.709394 py-ai-cli-0.3.6/src/ai_cli/git.py
+-rw-r--r--   0        0        0     4400 2023-06-19 08:34:20.709394 py-ai-cli-0.3.6/src/ai_cli/setting.py
+-rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 py-ai-cli-0.3.6/PKG-INFO
```

### Comparing `py-ai-cli-0.3.5/CHANGELOG.md` & `py-ai-cli-0.3.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.5/LICENSE` & `py-ai-cli-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.5/README.md` & `py-ai-cli-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.5/README_ja.md` & `py-ai-cli-0.3.6/README_ja.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.5/README_zh.md` & `py-ai-cli-0.3.6/README_zh.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.5/pyproject.toml` & `py-ai-cli-0.3.6/pyproject.toml`

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
-version = "0.3.5"
+version = "0.3.6"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Repository = "https://github.com/yufeikang/ai-cli"
 Documentation = "https://github.com/yufeikang/ai-cli/blob/main/README.md"
```

### Comparing `py-ai-cli-0.3.5/src/ai_cli/__init__.py` & `py-ai-cli-0.3.6/src/ai_cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.5"
+__version__ = "0.3.6"
 
 import logging
 from logging.handlers import RotatingFileHandler
 from pathlib import Path
 
 HOME = Path.home()
```

### Comparing `py-ai-cli-0.3.5/src/ai_cli/cli.py` & `py-ai-cli-0.3.6/src/ai_cli/cli.py`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.5/src/ai_cli/git.py` & `py-ai-cli-0.3.6/src/ai_cli/git.py`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.5/src/ai_cli/setting.py` & `py-ai-cli-0.3.6/src/ai_cli/setting.py`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.5/PKG-INFO` & `py-ai-cli-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ai_cli
-Version: 0.3.5
+Version: 0.3.6
 Summary: This CLI tool allows you to easily chat with chatGPT in the command line. You can chat with it, ask questions, and even translate text. It also
 License: MIT
 Author-email: Yufei Kang <kou.uhi.x@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Documentation, https://github.com/yufeikang/ai-cli/blob/main/README.md
 Project-URL: Repository, https://github.com/yufeikang/ai-cli
 Description-Content-Type: text/markdown
```

