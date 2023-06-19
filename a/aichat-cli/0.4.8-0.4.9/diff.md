# Comparing `tmp/aichat-cli-0.4.8.tar.gz` & `tmp/aichat-cli-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aichat-cli-0.4.8.tar", last modified: Fri Jun 16 00:07:48 2023, max compression
+gzip compressed data, was "aichat-cli-0.4.9.tar", last modified: Mon Jun 19 19:10:46 2023, max compression
```

## Comparing `aichat-cli-0.4.8.tar` & `aichat-cli-0.4.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 00:07:48.537760 aichat-cli-0.4.8/
--rw-rw-rw-   0        0        0    35823 2023-05-23 15:04:57.000000 aichat-cli-0.4.8/LICENSE
--rw-rw-rw-   0        0        0     5229 2023-06-16 00:07:48.536754 aichat-cli-0.4.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 00:07:48.535680 aichat-cli-0.4.8/aichat_cli.egg-info/
--rw-rw-rw-   0        0        0     5229 2023-06-16 00:07:48.000000 aichat-cli-0.4.8/aichat_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-16 00:07:48.000000 aichat-cli-0.4.8/aichat_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 00:07:48.000000 aichat-cli-0.4.8/aichat_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-16 00:07:48.000000 aichat-cli-0.4.8/aichat_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 00:07:48.000000 aichat-cli-0.4.8/aichat_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 00:07:48.538760 aichat-cli-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1063 2023-06-16 00:07:36.000000 aichat-cli-0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 19:10:46.432538 aichat-cli-0.4.9/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 15:04:57.000000 aichat-cli-0.4.9/LICENSE
+-rw-rw-rw-   0        0        0     5240 2023-06-19 19:10:46.431538 aichat-cli-0.4.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 19:10:46.430541 aichat-cli-0.4.9/aichat_cli.egg-info/
+-rw-rw-rw-   0        0        0     5240 2023-06-19 19:10:46.000000 aichat-cli-0.4.9/aichat_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-19 19:10:46.000000 aichat-cli-0.4.9/aichat_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 19:10:46.000000 aichat-cli-0.4.9/aichat_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-19 19:10:46.000000 aichat-cli-0.4.9/aichat_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 19:10:46.000000 aichat-cli-0.4.9/aichat_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 19:10:46.433540 aichat-cli-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1063 2023-06-19 19:10:24.000000 aichat-cli-0.4.9/setup.py
```

### Comparing `aichat-cli-0.4.8/LICENSE` & `aichat-cli-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aichat-cli-0.4.8/PKG-INFO` & `aichat-cli-0.4.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 Metadata-Version: 2.1
 Name: aichat-cli
-Version: 0.4.8
+Version: 0.4.9
 Summary: A CLI app that allows you to have interactive conversations with different AI bots
 Home-page: https://github.com/TheLime1/aichat-cli
 Author: TheLime1
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ai Chat CLI
 
 [![PyPI version](https://img.shields.io/pypi/v/aichat-cli.svg)](https://pypi.org/project/aichat-cli/)
-[![Did i find a bad token today ?](https://github.com/TheLime1/gpt-cli/actions/workflows/bad_token.yml/badge.svg)](https://github.com/TheLime1/gpt-cli/actions/workflows/bad_token.yml)
 
 A command-line interface chatbot. It allows you to have interactive conversations with different bots, including GPT4 FOR FREE
 
 Check the web version [here](https://github.com/TheLime1/gptCensorFree) (WIP).
 
 Thanks to [@Lomusire](https://github.com/Lomusire) for providing premium tokens ❤️.
 
+We are in a race with poe.com devs baning our tokens, you can help by [generating tokens](https://krakenfiles.com/view/kUx2jPXcZ0/file.html). 
+
+Updated poe.com token list [here](https://raw.githubusercontent.com/TheLime1/online-proxy-list/main/poe_token_check/poe_tokens.txt).
+
 ## Features✨
 
 - Choose between different bots.
 - Input messages for the chatbot via command-line arguments or interactively.
 - Export the conversation to a .txt file for future reference.
 - Insert your clipboard for multiple-line messages.
 - Delete your messages to respect your privacy.
-- Automatic detection for bad tokens each day, [check this test !](https://github.com/TheLime1/gpt-cli/pull/18)
+- Updated tokens each day
 
 ## Prerequisites📋
 
 - Python 3.7 or higher installed on your system.
 
 ## Getting Started🚀
```

### Comparing `aichat-cli-0.4.8/aichat_cli.egg-info/PKG-INFO` & `aichat-cli-0.4.9/aichat_cli.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 Metadata-Version: 2.1
 Name: aichat-cli
-Version: 0.4.8
+Version: 0.4.9
 Summary: A CLI app that allows you to have interactive conversations with different AI bots
 Home-page: https://github.com/TheLime1/aichat-cli
 Author: TheLime1
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ai Chat CLI
 
 [![PyPI version](https://img.shields.io/pypi/v/aichat-cli.svg)](https://pypi.org/project/aichat-cli/)
-[![Did i find a bad token today ?](https://github.com/TheLime1/gpt-cli/actions/workflows/bad_token.yml/badge.svg)](https://github.com/TheLime1/gpt-cli/actions/workflows/bad_token.yml)
 
 A command-line interface chatbot. It allows you to have interactive conversations with different bots, including GPT4 FOR FREE
 
 Check the web version [here](https://github.com/TheLime1/gptCensorFree) (WIP).
 
 Thanks to [@Lomusire](https://github.com/Lomusire) for providing premium tokens ❤️.
 
+We are in a race with poe.com devs baning our tokens, you can help by [generating tokens](https://krakenfiles.com/view/kUx2jPXcZ0/file.html). 
+
+Updated poe.com token list [here](https://raw.githubusercontent.com/TheLime1/online-proxy-list/main/poe_token_check/poe_tokens.txt).
+
 ## Features✨
 
 - Choose between different bots.
 - Input messages for the chatbot via command-line arguments or interactively.
 - Export the conversation to a .txt file for future reference.
 - Insert your clipboard for multiple-line messages.
 - Delete your messages to respect your privacy.
-- Automatic detection for bad tokens each day, [check this test !](https://github.com/TheLime1/gpt-cli/pull/18)
+- Updated tokens each day
 
 ## Prerequisites📋
 
 - Python 3.7 or higher installed on your system.
 
 ## Getting Started🚀
```

### Comparing `aichat-cli-0.4.8/setup.py` & `aichat-cli-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 long_description = (base_path / "README.md").read_text(encoding="utf-8")
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="aichat-cli",
-    version="0.4.8",
+    version="0.4.9",
     author="TheLime1",
     license="GPLv3",
     description="A CLI app that allows you to have interactive conversations with different AI bots",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

