# Comparing `tmp/chainfury-0.1.0.tar.gz` & `tmp/chainfury-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainfury-0.1.0.tar", max compression
+gzip compressed data, was "chainfury-0.1.1.tar", max compression
```

## Comparing `chainfury-0.1.0.tar` & `chainfury-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,20 @@
--rw-r--r--   0        0        0    11351 2023-06-12 10:47:25.719426 chainfury-0.1.0/LICENSE
--rw-r--r--   0        0        0     7783 2023-06-12 10:47:25.719584 chainfury-0.1.0/README.md
--rw-r--r--   0        0        0      223 2023-06-19 10:26:36.047002 chainfury-0.1.0/chainfury/__init__.py
--rw-r--r--   0        0        0    12524 2023-06-19 10:21:46.091911 chainfury-0.1.0/chainfury/agent.py
--rw-r--r--   0        0        0    30518 2023-06-19 10:28:45.737597 chainfury-0.1.0/chainfury/base.py
--rw-r--r--   0        0        0      545 2023-06-19 10:42:02.929669 chainfury-0.1.0/chainfury/cli.py
--rw-r--r--   0        0        0      795 2023-06-19 10:20:57.258296 chainfury-0.1.0/chainfury/utils.py
--rw-r--r--   0        0        0      113 2023-06-19 10:27:02.042189 chainfury-0.1.0/chainfury/version.py
--rw-r--r--   0        0        0      628 2023-06-19 10:26:18.352503 chainfury-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8882 1970-01-01 00:00:00.000000 chainfury-0.1.0/setup.py
--rw-r--r--   0        0        0     8631 1970-01-01 00:00:00.000000 chainfury-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-06-12 10:47:25.719426 chainfury-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7783 2023-06-12 10:47:25.719584 chainfury-0.1.1/README.md
+-rw-r--r--   0        0        0      256 2023-06-19 19:54:10.712240 chainfury-0.1.1/chainfury/__init__.py
+-rw-r--r--   0        0        0    12524 2023-06-19 10:21:46.091911 chainfury-0.1.1/chainfury/agent.py
+-rw-r--r--   0        0        0    30518 2023-06-19 10:28:45.737597 chainfury-0.1.1/chainfury/base.py
+-rw-r--r--   0        0        0      996 2023-06-19 19:50:21.074486 chainfury-0.1.1/chainfury/cli.py
+-rw-r--r--   0        0        0     6035 2023-06-19 19:50:32.084245 chainfury-0.1.1/chainfury/client.py
+-rw-r--r--   0        0        0     1699 2023-06-12 14:13:15.392725 chainfury-0.1.1/chainfury/components/README.md
+-rw-r--r--   0        0        0      795 2023-06-19 19:58:00.971782 chainfury-0.1.1/chainfury/components/__init__.py
+-rw-r--r--   0        0        0     4187 2023-06-19 10:28:49.030833 chainfury-0.1.1/chainfury/components/ai_actions/__init__.py
+-rw-r--r--   0        0        0     2003 2023-06-19 10:28:44.950061 chainfury-0.1.1/chainfury/components/functional/__init__.py
+-rw-r--r--   0        0        0     2237 2023-06-19 10:28:44.907614 chainfury-0.1.1/chainfury/components/nbx/__init__.py
+-rw-r--r--   0        0        0     8981 2023-06-19 10:28:44.986884 chainfury-0.1.1/chainfury/components/openai/__init__.py
+-rw-r--r--   0        0        0       78 2023-06-19 19:54:19.450567 chainfury-0.1.1/chainfury/components/redis/__init__.py
+-rw-r--r--   0        0        0     9400 2023-06-19 10:28:44.949439 chainfury-0.1.1/chainfury/components/stability/__init__.py
+-rw-r--r--   0        0        0     1262 2023-06-19 19:53:04.579434 chainfury-0.1.1/chainfury/utils.py
+-rw-r--r--   0        0        0      113 2023-06-19 19:59:21.715065 chainfury-0.1.1/chainfury/version.py
+-rw-r--r--   0        0        0      628 2023-06-19 19:59:57.165966 chainfury-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9106 1970-01-01 00:00:00.000000 chainfury-0.1.1/setup.py
+-rw-r--r--   0        0        0     8631 1970-01-01 00:00:00.000000 chainfury-0.1.1/PKG-INFO
```

### Comparing `chainfury-0.1.0/LICENSE` & `chainfury-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chainfury-0.1.0/README.md` & `chainfury-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `chainfury-0.1.0/chainfury/agent.py` & `chainfury-0.1.1/chainfury/agent.py`

 * *Files identical despite different names*

### Comparing `chainfury-0.1.0/chainfury/base.py` & `chainfury-0.1.1/chainfury/base.py`

 * *Files identical despite different names*

### Comparing `chainfury-0.1.0/setup.py` & `chainfury-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['chainfury']
+['chainfury',
+ 'chainfury.components',
+ 'chainfury.components.ai_actions',
+ 'chainfury.components.functional',
+ 'chainfury.components.nbx',
+ 'chainfury.components.openai',
+ 'chainfury.components.redis',
+ 'chainfury.components.stability']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Jinja2==3.1.2', 'fire==0.5.0', 'jinja2schema==0.1.4']
 
 entry_points = \
 {'console_scripts': ['chainfury = chainfury.cli:main']}
 
 setup_kwargs = {
     'name': 'chainfury',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'ChainFury is a powerful tool that simplifies the creation and management of chains of prompts, making it easier to build complex chat applications using LLMs.',
     'long_description': '# 🦋 ChainFury\n\n[![linkcheck](https://img.shields.io/badge/Workflow-Passing-darkgreen)](https://github.com/NimbleBoxAI/ChainFury/actions)\n[![Downloads](https://static.pepy.tech/badge/chainfury)](https://pepy.tech/project/chainfury)\n[![linkcheck](https://img.shields.io/badge/Site-🦋ChainFury-lightblue)](https://chainfury.nbox.ai)\n[![License: Apache](https://img.shields.io/badge/License-Apache%20v2.0-red)](https://github.com/NimbleBoxAI/ChainFury/blob/main/LICENSE) \n[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/NimbleBoxAI.svg?style=social&label=Follow%20%40NimbleBoxAI)](https://twitter.com/NimbleBoxAI)\n[![](https://dcbadge.vercel.app/api/server/KhF38hrAJ2?compact=true&style=flat)](https://discord.com/invite/KhF38hrAJ2)\n\n<img src="./docs/1.png" align="center"/>\n\n🦋 Build complex chat apps using LLMs in 4 clicks ⚡️ [Try it out here](https://chainfury.nbox.ai/)\n\nChainFury is a powerful tool that simplifies the creation and management of chains of prompts, making it easier to build complex chat applications using LLMs. \n\nWith a simple GUI inspired by [LangFlow](https://github.com/logspace-ai/langflow), ChainFury enables you to chain components of [LangChain](https://github.com/hwchase17/langchain) together, allowing you to embed more complex chat applications with a simple JS snippet.\n\nChainFury supports a range of features, including but not limited to:\n\n- Recording all prompts and responses and storing them in a database\n- Collecting metrics like response latency\n- Querying OpenAI\'s API to obtain a rating for the response, which it stores in the database\n- Separate scoring mechanism per ChatBot to easily view performance in a dashboard\n- [Plugins](./server/plugins/) to extend the functionality of ChainFury with callbacks\n\n---\n\n<img src="./docs/2.png" align="center"/>\n\n---\nInstalling ChainFury is easy, with two methods available. We suggest using **the Docker method.**\n\n## Method 1: Docker\n\nThe easiest way to install ChainFury is to use Docker. You can use the following command to run ChainFury:\n\n```bash\ndocker build . -f Dockerfile -t chainfury:latest\n\ndocker run --env OPENAI_API_KEY=<your_key_here> -p 8000:8000 chainfury:latest\n```\n\nNow you can access the app on [localhost:8000](http://localhost:8000/ui/).\n\n<details>\n<summary>Optional environment variable for Database</summary>\nYou can also pass a Database URL to the docker container using the `DATABASE_URL` environment variable. If you do not pass a database URL, ChainFury will use a SQLite database.\n\nExample:\n\n```bash\ndocker run -it -E DATABASE_URL="mysql+pymysql://<user>:<password>@127.0.0.1:3306/<database>" -p 8000:8000 chainfury\n```\n</details>\n\n\n---\n## Method 2: Manual\n<details>\n<summary>For this, you will need to build the frontend and and then run the backend. The frontend can be built using the following command:</summary>\n\n```bash\ncd client\nyarn install\nyarn build\n```\n\nTo copy the frontend to the backend, run the following command:\n\n```bash\ncd ..\ncp -r client/dist/ server/static/\nmkdir -p ./server/templates\ncp ./client/dist/index.html ./server/templates/index.html\n```\n\nNow you can install the backend dependencies and run the server. We recommend using Python 3.9 virtual environment for this:\n\n```bash\npython3 -m venv venv\nsource venv/bin/activate\npip install -r requirements.txt\ncd server\npython3 -m uvicorn app:app --log-level=debug --host 0.0.0.0 --port 8000 --workers 1\n```\n</details>\n<!-- collapsable -->\n\n<details>\n<summary>How to run</summary>\n\nAssuming you are in `server` directory, you can run the server using the following command:\n\n```bash\npython3 server.py --port 8000 --config_plugins=\'["echo"]\'\n```\n</details>\n\nNow you can access the app on [localhost:8000](http://localhost:8000/ui/).\n\n---\n\n<img src="./docs/3.png" align="center"/>\n\n---\n\n1. Start the server by using the docker file provided or by using the manual method.\n\n2. Log into ChainFury by entering username = “admin” and password = “admin”\n\n3. Click on create chatbot\n\n4. Use one of the pre-configured chatbots or use the elements to create a custom chatbot.\n\n5. Save & create your chatbot and start chatting with it by clicking the chat on the bottom-right. You can see chatbot statistics and feedback metrics in your ChainFury dashboard.\n\n\n---\n\n<img src="./docs/5.png" align="center"/>\n\n---\n\nThere are six main areas that LangChain is designed to help with.\n\nChainFury consists of the same concepts to build LLM ChatBots. The components are, in increasing order of complexity:\n\n| Glossary | LangChain    | ChainFury    |\n| --- | --- | --- |\n| 📃 LLMs and Prompts | Prompt management, prompt optimization, generic interface for all LLMs, and common utilities for working with LLMs   | Easy prompt management with GUI elements\n| 🔗 Chains | Chains are sequences of calls (whether to an LLM or a different utility). LangChain provides a standard interface for chains, lots of integrations with other tools, and end-to-end chains for common applications | Easy chain management with GUI |\n| 📚 Data Augmented Generation | Data Augmented Generation involves specific types of chains that first interact with an external datasource to fetch data to use in the generation step. Examples of this include summarization of long pieces of text and question/answering over specific data sources | Coming soon |\n| 🤖 Agents | Agents involve an LLM making decisions about which Actions to take, taking that Action, seeing an Observation, and repeating that until done. LangChain provides a standard interface for agents, a selection of agents to choose from, and examples of end to end agents| Easy agent management with GUI |\n| 🧠 Memory | Memory is the concept of persisting state between calls of a chain/agent. LangChain provides a standard interface for memory, a collection of memory implementations, and examples of chains/agents that use memory | Memory modules are supported, persistant memory coming soon |\n| 🧐 Evaluation | [BETA] Generative models are notoriously hard to evaluate with traditional metrics. One new way of evaluating them is using language models themselves to do the evaluation. LangChain provides some prompts/chains for assisting in this | Auto evaluation of all prompts though OpenAI APIs |\n\n\n---\n\n<img src="./docs/4.png" align="center"/>\n\n---\nChainFury is an open-source project, and is currently in the alpha stage. We are open to contributions to the project in the form of features, infrastructure or documentation.\n\n- To contribute to this project, please follow a ["fork and pull request"](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) workflow. Please do not try to push directly to this repo unless you are maintainer.\n\n- Our [issues](https://github.com/NimbleBoxAI/ChainFury/issues) page is kept up to date with bugs, improvements, and feature requests.\n\n- If you\'re looking for help with your code, consider posting a question on the [GitHub Discussions board](https://github.com/NimbleBoxAI/ChainFury/discussions), so that more people can benefit from it.\n\n- **Describing your issue:** Try to provide as many details as possible. What exactly goes wrong? How is it failing? Is there an error? "XY doesn\'t work" usually isn\'t that helpful for tracking down problems. Always remember to include the code you ran and if possible, extract only the relevant parts and don\'t just dump your entire script. This will make it easier for us to reproduce the error.\n\n- **Sharing long blocks of code or logs:** If you need to include long code, logs or tracebacks, you can wrap them in `<details>` and `</details>`. This [collapses the content](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/details) so it only becomes visible on click, making the issue easier to read and follow.\n\n',
     'author': 'NimbleBox Engineering',
     'author_email': 'engineering@nimblebox.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/NimbleBoxAI/ChainFury',
```

### Comparing `chainfury-0.1.0/PKG-INFO` & `chainfury-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainfury
-Version: 0.1.0
+Version: 0.1.1
 Summary: ChainFury is a powerful tool that simplifies the creation and management of chains of prompts, making it easier to build complex chat applications using LLMs.
 Home-page: https://github.com/NimbleBoxAI/ChainFury
 License: Apache V2.0
 Author: NimbleBox Engineering
 Author-email: engineering@nimblebox.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

