# Comparing `tmp/dccmd-0.4.2.tar.gz` & `tmp/dccmd-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dccmd-0.4.2.tar", max compression
+gzip compressed data, was "dccmd-0.4.3.tar", max compression
```

## Comparing `dccmd-0.4.2.tar` & `dccmd-0.4.3.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0    11343 2022-04-03 15:12:02.723336 dccmd-0.4.2/LICENSE
--rw-r--r--   0        0        0    15516 2023-03-09 19:14:33.534717 dccmd-0.4.2/README.md
--rw-r--r--   0        0        0    37897 2023-05-26 18:40:10.713334 dccmd-0.4.2/dccmd/__init__.py
--rw-r--r--   0        0        0        0 2022-03-12 18:48:32.479928 dccmd-0.4.2/dccmd/main/__init__.py
--rw-r--r--   0        0        0     2693 2022-10-24 16:43:51.513342 dccmd-0.4.2/dccmd/main/auth/__init__.py
--rw-r--r--   0        0        0     1971 2022-04-03 16:01:57.710024 dccmd-0.4.2/dccmd/main/auth/client.py
--rw-r--r--   0        0        0     2434 2022-04-02 13:57:48.676773 dccmd-0.4.2/dccmd/main/auth/credentials.py
--rw-r--r--   0        0        0    10257 2023-03-09 19:14:33.534717 dccmd-0.4.2/dccmd/main/auth/util.py
--rw-r--r--   0        0        0     3645 2022-07-16 13:22:43.136443 dccmd-0.4.2/dccmd/main/crypto/__init__.py
--rw-r--r--   0        0        0     1846 2022-07-16 13:22:43.136443 dccmd-0.4.2/dccmd/main/crypto/keys.py
--rw-r--r--   0        0        0     1769 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/crypto/util.py
--rw-r--r--   0        0        0     8669 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/download/__init__.py
--rw-r--r--   0        0        0     1516 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/models/__init__.py
--rw-r--r--   0        0        0     1158 2022-07-16 12:51:12.543170 dccmd-0.4.2/dccmd/main/models/errors.py
--rw-r--r--   0        0        0    11768 2023-05-26 18:40:10.716667 dccmd-0.4.2/dccmd/main/rooms/__init__.py
--rw-r--r--   0        0        0      118 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/rooms/models.py
--rw-r--r--   0        0        0    10440 2023-05-26 18:40:10.716667 dccmd-0.4.2/dccmd/main/rooms/permissions.py
--rw-r--r--   0        0        0     3128 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/rooms/print.py
--rw-r--r--   0        0        0    11512 2023-05-26 18:53:37.146674 dccmd-0.4.2/dccmd/main/upload/__init__.py
--rw-r--r--   0        0        0     4423 2022-10-24 16:43:51.516675 dccmd-0.4.2/dccmd/main/users/__init__.py
--rw-r--r--   0        0        0     9731 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/users/manage.py
--rw-r--r--   0        0        0     1902 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/users/print.py
--rw-r--r--   0        0        0     4747 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/util/__init__.py
--rw-r--r--   0        0        0      652 2023-05-26 18:40:10.716667 dccmd-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    17052 1970-01-01 00:00:00.000000 dccmd-0.4.2/setup.py
--rw-r--r--   0        0        0    16237 1970-01-01 00:00:00.000000 dccmd-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-05-25 12:01:39.464522 dccmd-0.4.3/LICENSE
+-rw-r--r--   0        0        0    15516 2023-05-25 12:01:39.464639 dccmd-0.4.3/README.md
+-rw-r--r--   0        0        0    37888 2023-06-19 13:05:04.175852 dccmd-0.4.3/dccmd/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 12:01:39.464919 dccmd-0.4.3/dccmd/main/__init__.py
+-rw-r--r--   0        0        0     2693 2023-05-25 12:01:39.465040 dccmd-0.4.3/dccmd/main/auth/__init__.py
+-rw-r--r--   0        0        0     1971 2023-05-25 12:01:39.465106 dccmd-0.4.3/dccmd/main/auth/client.py
+-rw-r--r--   0        0        0     2434 2023-05-25 12:01:39.465168 dccmd-0.4.3/dccmd/main/auth/credentials.py
+-rw-r--r--   0        0        0    10257 2023-05-25 12:01:39.465249 dccmd-0.4.3/dccmd/main/auth/util.py
+-rw-r--r--   0        0        0     3645 2023-05-25 12:01:39.465356 dccmd-0.4.3/dccmd/main/crypto/__init__.py
+-rw-r--r--   0        0        0     1846 2023-05-25 12:01:39.465418 dccmd-0.4.3/dccmd/main/crypto/keys.py
+-rw-r--r--   0        0        0     1769 2023-05-25 12:01:39.465480 dccmd-0.4.3/dccmd/main/crypto/util.py
+-rw-r--r--   0        0        0     8669 2023-05-25 12:01:39.465613 dccmd-0.4.3/dccmd/main/download/__init__.py
+-rw-r--r--   0        0        0     1516 2023-05-25 12:01:39.465708 dccmd-0.4.3/dccmd/main/models/__init__.py
+-rw-r--r--   0        0        0     1158 2023-05-25 12:01:39.465779 dccmd-0.4.3/dccmd/main/models/errors.py
+-rw-r--r--   0        0        0    11768 2023-05-25 12:01:39.465890 dccmd-0.4.3/dccmd/main/rooms/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-25 12:01:39.465948 dccmd-0.4.3/dccmd/main/rooms/models.py
+-rw-r--r--   0        0        0    10440 2023-05-25 12:01:39.466033 dccmd-0.4.3/dccmd/main/rooms/permissions.py
+-rw-r--r--   0        0        0     3128 2023-05-25 12:01:39.466094 dccmd-0.4.3/dccmd/main/rooms/print.py
+-rw-r--r--   0        0        0    11441 2023-06-15 05:48:05.441018 dccmd-0.4.3/dccmd/main/upload/__init__.py
+-rw-r--r--   0        0        0     4423 2023-05-25 12:01:39.466348 dccmd-0.4.3/dccmd/main/users/__init__.py
+-rw-r--r--   0        0        0     9731 2023-05-25 12:01:39.466455 dccmd-0.4.3/dccmd/main/users/manage.py
+-rw-r--r--   0        0        0     1902 2023-05-25 12:01:39.466517 dccmd-0.4.3/dccmd/main/users/print.py
+-rw-r--r--   0        0        0     4747 2023-05-25 12:01:39.466617 dccmd-0.4.3/dccmd/main/util/__init__.py
+-rw-r--r--   0        0        0      652 2023-06-19 13:06:49.264462 dccmd-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    16237 1970-01-01 00:00:00.000000 dccmd-0.4.3/PKG-INFO
```

### Comparing `dccmd-0.4.2/LICENSE` & `dccmd-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/README.md` & `dccmd-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/__init__.py` & `dccmd-0.4.3/dccmd/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 DRACOON Commander
 A CLI DRACOON client
 
 """
 
-__version__ = "0.4.2-SNAPSHOT"
+__version__ = "0.4.3"
 
 # std imports
 import sys
 import os
 import asyncio
 
 # external imports
```

### Comparing `dccmd-0.4.2/dccmd/main/auth/__init__.py` & `dccmd-0.4.3/dccmd/main/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/auth/client.py` & `dccmd-0.4.3/dccmd/main/auth/client.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/auth/credentials.py` & `dccmd-0.4.3/dccmd/main/auth/credentials.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/auth/util.py` & `dccmd-0.4.3/dccmd/main/auth/util.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/crypto/__init__.py` & `dccmd-0.4.3/dccmd/main/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/crypto/keys.py` & `dccmd-0.4.3/dccmd/main/crypto/keys.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/crypto/util.py` & `dccmd-0.4.3/dccmd/main/crypto/util.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/download/__init__.py` & `dccmd-0.4.3/dccmd/main/download/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/models/__init__.py` & `dccmd-0.4.3/dccmd/main/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/models/errors.py` & `dccmd-0.4.3/dccmd/main/models/errors.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/rooms/__init__.py` & `dccmd-0.4.3/dccmd/main/rooms/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/rooms/permissions.py` & `dccmd-0.4.3/dccmd/main/rooms/permissions.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/rooms/print.py` & `dccmd-0.4.3/dccmd/main/rooms/print.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/upload/__init__.py` & `dccmd-0.4.3/dccmd/main/upload/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,19 +172,15 @@
     """check if OS is Windows"""
     return platform.system() == "Windows"
 
 
 async def create_folder_struct(source: str, target: str, dracoon: DRACOON, velocity: int = 2):
     """create all necessary folders for a recursive folder upload"""
 
-    if velocity > 10:
-        velocity = 10
-    elif velocity < 1:
-        velocity = 1
-
+    velocity = max(1, min(velocity, 10)) # refactor to one line
     async def process_batch(batch):
         """process a batch of folders to create"""
 
         path = target.rstrip('/') + '/' + batch[0].parent_path.lstrip('/')
         parent_node = await dracoon.nodes.get_node_from_path(path)
 
         if parent_node is None:
@@ -269,18 +265,15 @@
 
     for file in file_list.ignored_files:
         dracoon.logger.info(f"Ignoring file: {file.dir_path}")
 
     file_list.sort_by_size()
     transfer_list = DCTransferList(total=file_list.total_size, file_count=file_list.file_count)
 
-    if velocity > 10:
-        velocity = 10
-    elif velocity < 1:
-        velocity = 1
+    velocity = max(1, min(velocity, 10))
 
     concurrent_reqs = velocity * 5
 
     upload_reqs = []
 
     for item in file_list.file_list:
         upload_job = DCTransfer(transfer=transfer_list)
@@ -291,14 +284,15 @@
             file_path=item.dir_path,
             target_path=(target_path),
             resolution_strategy=resolution_strategy,
             callback_fn=upload_job.update
         )
         upload_reqs.append(asyncio.ensure_future(req))
 
+
     for batch in dracoon.batch_process(
             coro_list=upload_reqs, batch_size=concurrent_reqs
         ):
         try:
             # get fresh token per batch (avoid rate limiting)
             await dracoon.connect(connection_type=OAuth2ConnectionType.refresh_token)
             await asyncio.gather(*batch)
```

### Comparing `dccmd-0.4.2/dccmd/main/users/__init__.py` & `dccmd-0.4.3/dccmd/main/users/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/users/manage.py` & `dccmd-0.4.3/dccmd/main/users/manage.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/users/print.py` & `dccmd-0.4.3/dccmd/main/users/print.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/dccmd/main/util/__init__.py` & `dccmd-0.4.3/dccmd/main/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.2/pyproject.toml` & `dccmd-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dccmd"
-version = "0.4.2"
+version = "0.4.3"
 description = "DRACOON Commander – CLI client for DRACOON Cloud (dracoon.com)"
 authors = ["Octavio Simone <70800577+unbekanntes-pferd@users.noreply.github.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dccmd-0.4.2/setup.py` & `dccmd-0.4.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,466 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dccmd
+Version: 0.4.3
+Summary: DRACOON Commander – CLI client for DRACOON Cloud (dracoon.com)
+License: Apache-2.0
+Author: Octavio Simone
+Author-email: 70800577+unbekanntes-pferd@users.noreply.github.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: SecretStorage (>=3.3.1,<4.0.0)
+Requires-Dist: dracoon (>=1.10.0,<2.0.0)
+Requires-Dist: keyring (>=23.6.0,<24.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: typer (>=0.4.0,<0.5.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['dccmd',
- 'dccmd.main',
- 'dccmd.main.auth',
- 'dccmd.main.crypto',
- 'dccmd.main.download',
- 'dccmd.main.models',
- 'dccmd.main.rooms',
- 'dccmd.main.upload',
- 'dccmd.main.users',
- 'dccmd.main.util']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['SecretStorage>=3.3.1,<4.0.0',
- 'dracoon>=1.10.0,<2.0.0',
- 'keyring>=23.6.0,<24.0.0',
- 'tqdm>=4.65.0,<5.0.0',
- 'typer>=0.4.0,<0.5.0']
-
-entry_points = \
-{'console_scripts': ['dccmd = dccmd:app']}
-
-setup_kwargs = {
-    'name': 'dccmd',
-    'version': '0.4.2',
-    'description': 'DRACOON Commander – CLI client for DRACOON Cloud (dracoon.com)',
-    'long_description': '<h1 align="center">DRACOON Commander</h1>\n\n\n## Table of Contents\n\n* [About the Project](#about-the-project)\n  * [Built With](#built-with)\n* [Getting Started](#getting-started)\n  * [Prerequisites](#prerequisites)\n  * [Installation](#installation)\n* [Usage](#usage)\n* [Configuration](#configuration)\n* [License](#license)\n\n\n## About the project\n_Disclaimer: This is an unofficial client and is not supported by DRACOON._<br>\nThis client is a CLI tool to perform basic commands in DRACOON and comes with the following functionalities:\n\n* Full support for S3 direct up- / download\n    * Chunked up- and downloads\n* Full support for DRACOON end-to-end encryption\n* Optimized for concurrent requests\n* Store credentials in OS-specific secure location\n    * Linux: Freedesktop Secret Service (secretstorage)\n    * macOS: Keychain\n    * Windows: Windows Credential Locker\n\n### Built With\n* [typer](https://typer.tiangolo.com)\n* [keyring](https://pypi.org/project/keyring)\n* [dracoon](https://github.com/unbekanntes-pferd/dracoon-python-api)\n    * [httpx](https://www.python-httpx.org/)\n* [poetry](https://python-poetry.org/)\n\nA full dependency list can be viewed in\n* [pyproject.toml](/pyproject.toml) - list of dependencies and project info\n* [poetry.lock](/poetry.lock)\n\nDRACOON Commander is built with typer as the CLI framework and uses keyring to store all credentials (OAuth2 tokens, client credentials and encryption password). \nThe tool is built on top of dracoon, an async API wrapper for DRACOON based on httpx.\nThe project is managed with poetry (dependencies, release build and publishing).\n\n## Getting Started\nIn order to get started, download the latest tarball from Github or install dccmd from pip:\n[Releases]()\n\n### Prerequisites\nYou need a working Python 3.10 installation – dccmd makes use of type annotations and uses 3.10 features.\nGet the latest Python version from: [python.org](https://python.org).\n\n```bash\npython3 --version\n```\n\nIn order to get going, you can install dccmd either in a virtual environment or globally.\n\n### Installation\n\nTo install a version, use `pip` and install the `dccmd` package.\n\n#### In a virtual environment\n```bash\nvirtualenv <DIR>\nsource <DIR>/bin/activate \npython3 -m pip install dccmd\n```\n#### Globally\n```bash\npython3 -m pip install dccmd\n```\n\n#### Set PATH\nIn order for the script to work, you might need to add the relevant script path to your PATH.\nWhen installing with pip, the output will already indicate if the path is present or not.\nIf you do not add the correct directory to PATH, you will *not* be able to use the `dccmd` command in your preferred shell.\n\n##### Windows\nIn Windows, just add the script path by editing the environment variables for your account:\nLook for an entry called \'Path\' and install the script directory from the `pip install` output.\n\n##### Unix\nOn Linux or macOS you can add a path to PATH by using the following command:<br>\n`export PATH="/your/directory/see/install/output:$PATH"`<br>\n\n\n## Usage\n\n### Display commands\n\nIn order to see all available commands, arguments and options, use the --help flag:\n```bash\ndccmd --help\n```\n\n```\nUsage: dccmd [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --install-completion [bash|zsh|fish|powershell|pwsh]\n                                  Install completion for the specified shell.\n  --show-completion [bash|zsh|fish|powershell|pwsh]\n                                  Show completion for the specified shell, to\n                                  copy it or customize the installation.\n  --help                          Show this message and exit.\n\nCommands:\n  auth\n  client\n  crypto\n  download  Download a file from DRACOON by providing a source path and a...\n  ls        List all nodes in a DRACOON path\n  mkdir     Create a folder in a DRACOON parent path\n  mkroom    Create a room (inherit permissions) in a DRACOON parent path\n  rm        Delete a file / folder / room in DRACOON\n  upload    Upload a file into DRACOON by providing a source path and a...\n```\nAll commands display their own help message, e.g. \n`dccmd upload --help`.\n\n### Client registration and authentication\n\nBefore you can perform any command, you must authenticate and set up the client.\nIf you enter any command which requires authentication (e.g. `dccmd ls your.dracoon.domain.com/`), you will be prompted first for a client configuration:\n* client id\n* client secret\n\n#### Client \nBefore you can use `dccmd` you need to generate a client in your DRACOON instance (config manager role required).\n1. Create a client with a client id and client secret.\nPlease make sure you have the following settings active:\n* Authorization code \n* Redirect URI is set to `https://your.dracoon.domain.com/oauth/callback`\n* Optional: If you wish to use the CLI mode (enter password and username via CLI), you can activate password flow \n\n2. Copy client id and client secret and use any command (e.g. `dccmd ls your.dracoon.domain.com/`).\n\n3. Enter client id and client secret – the information will be securely stored in your OS-specific secret container.\n\n#### Authentication\nOnce the client is set up, you will receive a link to authenticate via OAuth2 authorization code flow – you will then receive a code which you need to enter into the terminal.\nWhen completed, you will be prompted to store credentials securely (OS-specific).\n\nAdditionally, you can skip the authorization code flow and provide credentials directly, e.g. for the `dccmd ls` command:\n\n```bash\ndccmd ls your-dracoon.domain.com/ --cli-mode username@mail.com topsecret123!\n```\n\n### Upload\n\n**Important: if you use Windows, you need to provide the path with \'/\' instead of \'\\\\\'!**\n\nYou can upload single files using the upload command:\n\n```bash\ndccmd upload /path/to/file.pdf your-dracoon.domain.com/\n```\nIn order to upload a directory, use the `--recursive` (`-r`) flag:\n\n```bash\ndccmd upload -r /path/to/folder your-dracoon.domain.com/\n```\n\n#### Conflict resolution\nIf you upload a file which already exists (based on file name), the upload will be rejected.<br> \nIn order to force an overwrite, use the `--overwrite` flag:\n\n```bash\ndccmd upload /path/to/file.pdf your-dracoon.domain.com/ --overwrite\n```\n\nIf you wish to auto-rename the file if it already exists, use the `auto-rename`flag:\n\n```bash\ndccmd upload /path/to/file.pdf your-dracoon.domain.com/ --auto-rename\n```\n\n#### Advanced usage\nIf you upload folders recursively, you might encounter performance issues, specifically when uploading many small files. \nYou can therefore adjust concurrent file uploads via the `--velocity` (`-v`) flag:\n\n```bash\ndccmd upload -r /path/to/folder your-dracoon.domain.com/ -v 3\n```\nThe default value is 2 - it does not coincide with real request value.<br>\nMaximum (although not recommended) value is 10. Entering higher numbers will result in max value use.<br>\nMinimum value is 1 - this will not upload a folder per file but is the minimum concurrent request value. Entering lower numbers will result in min value use.\n\nIf you need to understand why uploads fail, you can also run the command using the `--debug` flag:\n\n```bash\ndccmd upload -r /path/to/folder your-dracoon.domain.com/ --debug\n```\n*Note: This will have impact on performance as the log will be streamed to terminal and the log level will be increased to DEBUG.*\n\n### Create folder\n\nIf you wish to create a folder, use the `mkdir` command:\n\n```bash\ndccmd mkdir your-dracoon.domain.com/parent/newfolder\n```\nJust enter the full new path to create a folder. \nYou will need *create* permission to do so.\n\n\n### Create room\n\nIf you wish to create a room, use the `mkroom` command:\n\n```bash\ndccmd mkroom your-dracoon.domain.com/parent/newroom\n```\nJust enter the full new path to create a room. \nThe room will be created as a room with inherited permissions from the parent.\nYou will need *manage* permission to do so.\n\nTo create a room on the root level (\'/\'), you need to provide an admin user using \nthe corresponding option (`-au` or `--admin-user`):\n\n```bash\ndccmd mkroom -au "admin.username" your-dracoon.domain.com/newroom\n```\n*Note: In order to use the username of an OIDC user, you need to escape the `\\`, meaning you need to enter multiple slashes like so: `OIDC\\\\\\user.name`*\n\nTo create a room on any level that does *not* inherit permissions, use the `-au` (`--admin-user`) flag and provide the room admin when creating the room as with root level rooms:\n\n```bash\ndccmd mkroom -au "admin.username" your-dracoon.domain.com/parent-room/newroom\n```\n\n### Delete node\n\nIf you wish to delete a node, use the `rm` command:\n\n```bash\ndccmd rm your-dracoon.domain.com/parent/somefile.pdf\n```\nIn order to delete a container (room, folder) you need to use the `--recursive` (`r`) flag:\n\n```bash\ndccmd rm your-dracoon.domain.com/parent/folder/to/delete\n```\n**Warning: Deleting rooms cannot be undone!**\n\n### List nodes\n\nIn order to list all nodes, use the `ls` command:\n\n```bash\ndccmd ls your-dracoon.domain.com/\n```\n*Note: In order to list the root node, you need to provide a trailing `/`*\nFor a specific container (room or folder), use the path:\n```bash\ndccmd ls your-dracoon.domain.com/your/room\n```\n\n#### Displaying additional information\nUsing the `ls` command by default only provides node names.\nIn order to display more information, use relevant flags:\n\n* Display all information (size, last updated, last update user): `--long` (`-l`)\n    * Display sizes in human readable format (B, KB..): `--human-readable` (`-h`)\n* Display node id: `--inode` (`-i`)\n\nExample displaying full information:\n\n```bash\ndccmd ls -h -i -l your-dracoon.domain.com/your/room\n```\n### Download\n\nTo download a file, use the `download` command:\n\n```bash\ndccmd download your-dracoon.domain.com/your/cool-file.mp4 /target/directory\n```\n\nTo download a room or a folder, use the `download` command with `--recursive` (`-r`) flag:\n\n```bash\ndccmd download -r your-dracoon.domain.com/your/cool-folder /target/directory\n```\n\n#### Advanced usage\nIf you download folders recursively, you might encounter performance issues, specifically when downloading many small files. \nYou can therefore adjust concurrent file uploads via the `--velocity` (`-v`) flag:\n\n```bash\ndccmd upload -r /path/to/folder your-dracoon.domain.com/ -v 3\n```\nThe default value is 2 - it does not coincide with real request value.<br>\nMaximum (although not recommended) value is 10. Entering higher numbers will result in max value use.<br>\nMinimum value is 1 - this will not download a folder per file but is the minimum concurrent request value. Entering lower numbers will result in min value use.\n\n### User operations\n\nYou can list, edit and import users with relevant `dccmd users` command:\n\n* csv-import  Add a list of users to DRACOON from a CSV file\n* ls          Get a list of users in DRACOON\n* rm          Delete a user\n\n#### Importing users\n\nYou can import users by using the `csv-import` command and providing a path to the csv file:\n\n```bash\ndccmd users csv-import /path/to/users.csv your-dracoon.domain.com/\n```\n\nThe csv file must contain a header and should include the following attributes:\n\n* first name\n* last name\n* email \n* login (optional)\n\nBy default, local users are created - if you want to import oidc users, you need pass the oidc config id:\n\n```bash\n#example with OIDC config 5\ndccmd users csv-import /path/to/users.csv your-dracoon.domain.com/ 5\n```\n\n#### Listing users\n\nYou can list all users using the `ls` command:\n\n```bash\ndccmd users ls your-dracoon.domain.com/\n```\n\nYou can get all users also as csv format by using the `--csv` flag:\n\n```bash\ndccmd users ls your-dracoon.domain.com/ --csv > users.csv\n```\n\nTo find a user, you can pass a search string to search for either first name, last name or user name (search string applies to all):\n\n```bash\n# will return all users with either first name, last name or user name containing \'yourname\'\ndccmd users ls your-dracoon.domain.com/ yourname\n```\n\n#### Deleting users\n\nYou can delete a user by providing the username:\n```bash\ndccmd users rm your-dracoon.domain.com/ user123\n```\n\n### Room permissions management\n\nFor an overview of the available commands use \n\n```bash\ndccmd rooms --help\n```\n\n#### List user / group permissions in a room\n\nTo list user permissions in a room, use the `list-users` command:\n\n```bash\ndccmd rooms list-users your-dracoon.domain.com/your-room\n```\nYou need minimum `read` permissions to list users.\n\nTo list group permissions in a room, use the `list-groups` command:\n\n```bash\ndccmd rooms list-groups your-dracoon.domain.com/your-room\n```\nYou need minimum `read` permissions to list groups.\n\nAs with other commands, you can use the `--csv` flag to get a csv export for the room\npermissions (users and groups).\n\n#### Add user / group to a room\n\nCurrently, the following templates are available:\n- read: read-only perrmissions for a room \n- edit: edit permissions for a room\n- admin: room admin permissions\n\nThe permissions coincide with the templates in use of the official DRACOON Web App.\n\nYou need `manage` permissions (room admin) to add users / groups.\n\nTo add a user, use the `add-user` command and provide the user and permission template (`-u` and `-p`):\n\n```bash\ndccmd rooms add-user -u "user.name" -p admin your-dracoon.domain.com/your-room\n```\n\nTo add a group, use the `add-group` command and provide the group and permission template (`-g` and `-p`):\n\n```bash\ndccmd rooms add-group -g "group.name" -p admin your-dracoon.domain.com/your-room\n```\n\n#### Remove user / group from a room\n\nYou need `manage` permissions (room admin) to remove users / groups.\n\nTo add a user, use the `remove-user` command and provide the user (`-u`):\n\n```bash\ndccmd rooms remove-user -u "user.name" your-dracoon.domain.com/your-room\n```\n\nTo add a group, use the `remove-group` command and provide the group (`-g`):\n\n```bash\ndccmd rooms remove-group -g "group.name" your-dracoon.domain.com/your-room\n```\n\n## Configuration / administration\n\nYou can view / manage the configuration for `dccmd` using the relevant commands:\n\n* `dccmd auth` - manage credentials\n    * `dccmd auth ls your.dracoon.domain.com` will display if a refresh token has been stored for the provided domain\n    * `dccmd auth rm your-dracoon.domain.com` will remove stored credentials for the provided domain\n* `dccmd client` - manage client\n    * `dccmd client register your.dracoon.domain.com` will start the registration process for a client and given domain\n    * `dccmd client ls your.dracoon.domain.com` will display client information for the provided domain\n    * `dccmd client rm your-dracoon.domain.com` will remove the stored client config for the provided domain\n* `dccmd crypto` - manage encryption\n    * `dccmd crypto ls your.dracoon.domain.com` will display if encryption password is stored for the provided domain\n    * `dccmd crypto rm your-dracoon.domain.com` will remove the encryption password for the provided domain\n    * `dccmd crypto distribute your-dracoon.domain.com/` will generate file keys available to distribute - if providing a specific path (`dccmd crypto distribute your-dracoon.domain.com/some/path`), only keys for provided parent room will be generated.\n\n### Logging \nWhen using a command, a log will be created in the current working directory.\nCurrently it is not possible to configure a default path for a log.\n\nYou can stream the log to stdout by using the `--debug` flag with any DRACOON-specific command (`upload`, `download`, `ls`, `rm`, `mkdir`, `mkroom`).\n\n\n## License\nDistributed under the Apache License. See [LICENSE](/LICENSE) for more information.\n',
-    'author': 'Octavio Simone',
-    'author_email': '70800577+unbekanntes-pferd@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+<h1 align="center">DRACOON Commander</h1>
 
 
-setup(**setup_kwargs)
+## Table of Contents
+
+* [About the Project](#about-the-project)
+  * [Built With](#built-with)
+* [Getting Started](#getting-started)
+  * [Prerequisites](#prerequisites)
+  * [Installation](#installation)
+* [Usage](#usage)
+* [Configuration](#configuration)
+* [License](#license)
+
+
+## About the project
+_Disclaimer: This is an unofficial client and is not supported by DRACOON._<br>
+This client is a CLI tool to perform basic commands in DRACOON and comes with the following functionalities:
+
+* Full support for S3 direct up- / download
+    * Chunked up- and downloads
+* Full support for DRACOON end-to-end encryption
+* Optimized for concurrent requests
+* Store credentials in OS-specific secure location
+    * Linux: Freedesktop Secret Service (secretstorage)
+    * macOS: Keychain
+    * Windows: Windows Credential Locker
+
+### Built With
+* [typer](https://typer.tiangolo.com)
+* [keyring](https://pypi.org/project/keyring)
+* [dracoon](https://github.com/unbekanntes-pferd/dracoon-python-api)
+    * [httpx](https://www.python-httpx.org/)
+* [poetry](https://python-poetry.org/)
+
+A full dependency list can be viewed in
+* [pyproject.toml](/pyproject.toml) - list of dependencies and project info
+* [poetry.lock](/poetry.lock)
+
+DRACOON Commander is built with typer as the CLI framework and uses keyring to store all credentials (OAuth2 tokens, client credentials and encryption password). 
+The tool is built on top of dracoon, an async API wrapper for DRACOON based on httpx.
+The project is managed with poetry (dependencies, release build and publishing).
+
+## Getting Started
+In order to get started, download the latest tarball from Github or install dccmd from pip:
+[Releases]()
+
+### Prerequisites
+You need a working Python 3.10 installation – dccmd makes use of type annotations and uses 3.10 features.
+Get the latest Python version from: [python.org](https://python.org).
+
+```bash
+python3 --version
+```
+
+In order to get going, you can install dccmd either in a virtual environment or globally.
+
+### Installation
+
+To install a version, use `pip` and install the `dccmd` package.
+
+#### In a virtual environment
+```bash
+virtualenv <DIR>
+source <DIR>/bin/activate 
+python3 -m pip install dccmd
+```
+#### Globally
+```bash
+python3 -m pip install dccmd
+```
+
+#### Set PATH
+In order for the script to work, you might need to add the relevant script path to your PATH.
+When installing with pip, the output will already indicate if the path is present or not.
+If you do not add the correct directory to PATH, you will *not* be able to use the `dccmd` command in your preferred shell.
+
+##### Windows
+In Windows, just add the script path by editing the environment variables for your account:
+Look for an entry called 'Path' and install the script directory from the `pip install` output.
+
+##### Unix
+On Linux or macOS you can add a path to PATH by using the following command:<br>
+`export PATH="/your/directory/see/install/output:$PATH"`<br>
+
+
+## Usage
+
+### Display commands
+
+In order to see all available commands, arguments and options, use the --help flag:
+```bash
+dccmd --help
+```
+
+```
+Usage: dccmd [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --install-completion [bash|zsh|fish|powershell|pwsh]
+                                  Install completion for the specified shell.
+  --show-completion [bash|zsh|fish|powershell|pwsh]
+                                  Show completion for the specified shell, to
+                                  copy it or customize the installation.
+  --help                          Show this message and exit.
+
+Commands:
+  auth
+  client
+  crypto
+  download  Download a file from DRACOON by providing a source path and a...
+  ls        List all nodes in a DRACOON path
+  mkdir     Create a folder in a DRACOON parent path
+  mkroom    Create a room (inherit permissions) in a DRACOON parent path
+  rm        Delete a file / folder / room in DRACOON
+  upload    Upload a file into DRACOON by providing a source path and a...
+```
+All commands display their own help message, e.g. 
+`dccmd upload --help`.
+
+### Client registration and authentication
+
+Before you can perform any command, you must authenticate and set up the client.
+If you enter any command which requires authentication (e.g. `dccmd ls your.dracoon.domain.com/`), you will be prompted first for a client configuration:
+* client id
+* client secret
+
+#### Client 
+Before you can use `dccmd` you need to generate a client in your DRACOON instance (config manager role required).
+1. Create a client with a client id and client secret.
+Please make sure you have the following settings active:
+* Authorization code 
+* Redirect URI is set to `https://your.dracoon.domain.com/oauth/callback`
+* Optional: If you wish to use the CLI mode (enter password and username via CLI), you can activate password flow 
+
+2. Copy client id and client secret and use any command (e.g. `dccmd ls your.dracoon.domain.com/`).
+
+3. Enter client id and client secret – the information will be securely stored in your OS-specific secret container.
+
+#### Authentication
+Once the client is set up, you will receive a link to authenticate via OAuth2 authorization code flow – you will then receive a code which you need to enter into the terminal.
+When completed, you will be prompted to store credentials securely (OS-specific).
+
+Additionally, you can skip the authorization code flow and provide credentials directly, e.g. for the `dccmd ls` command:
+
+```bash
+dccmd ls your-dracoon.domain.com/ --cli-mode username@mail.com topsecret123!
+```
+
+### Upload
+
+**Important: if you use Windows, you need to provide the path with '/' instead of '\\'!**
+
+You can upload single files using the upload command:
+
+```bash
+dccmd upload /path/to/file.pdf your-dracoon.domain.com/
+```
+In order to upload a directory, use the `--recursive` (`-r`) flag:
+
+```bash
+dccmd upload -r /path/to/folder your-dracoon.domain.com/
+```
+
+#### Conflict resolution
+If you upload a file which already exists (based on file name), the upload will be rejected.<br> 
+In order to force an overwrite, use the `--overwrite` flag:
+
+```bash
+dccmd upload /path/to/file.pdf your-dracoon.domain.com/ --overwrite
+```
+
+If you wish to auto-rename the file if it already exists, use the `auto-rename`flag:
+
+```bash
+dccmd upload /path/to/file.pdf your-dracoon.domain.com/ --auto-rename
+```
+
+#### Advanced usage
+If you upload folders recursively, you might encounter performance issues, specifically when uploading many small files. 
+You can therefore adjust concurrent file uploads via the `--velocity` (`-v`) flag:
+
+```bash
+dccmd upload -r /path/to/folder your-dracoon.domain.com/ -v 3
+```
+The default value is 2 - it does not coincide with real request value.<br>
+Maximum (although not recommended) value is 10. Entering higher numbers will result in max value use.<br>
+Minimum value is 1 - this will not upload a folder per file but is the minimum concurrent request value. Entering lower numbers will result in min value use.
+
+If you need to understand why uploads fail, you can also run the command using the `--debug` flag:
+
+```bash
+dccmd upload -r /path/to/folder your-dracoon.domain.com/ --debug
+```
+*Note: This will have impact on performance as the log will be streamed to terminal and the log level will be increased to DEBUG.*
+
+### Create folder
+
+If you wish to create a folder, use the `mkdir` command:
+
+```bash
+dccmd mkdir your-dracoon.domain.com/parent/newfolder
+```
+Just enter the full new path to create a folder. 
+You will need *create* permission to do so.
+
+
+### Create room
+
+If you wish to create a room, use the `mkroom` command:
+
+```bash
+dccmd mkroom your-dracoon.domain.com/parent/newroom
+```
+Just enter the full new path to create a room. 
+The room will be created as a room with inherited permissions from the parent.
+You will need *manage* permission to do so.
+
+To create a room on the root level ('/'), you need to provide an admin user using 
+the corresponding option (`-au` or `--admin-user`):
+
+```bash
+dccmd mkroom -au "admin.username" your-dracoon.domain.com/newroom
+```
+*Note: In order to use the username of an OIDC user, you need to escape the `\`, meaning you need to enter multiple slashes like so: `OIDC\\\user.name`*
+
+To create a room on any level that does *not* inherit permissions, use the `-au` (`--admin-user`) flag and provide the room admin when creating the room as with root level rooms:
+
+```bash
+dccmd mkroom -au "admin.username" your-dracoon.domain.com/parent-room/newroom
+```
+
+### Delete node
+
+If you wish to delete a node, use the `rm` command:
+
+```bash
+dccmd rm your-dracoon.domain.com/parent/somefile.pdf
+```
+In order to delete a container (room, folder) you need to use the `--recursive` (`r`) flag:
+
+```bash
+dccmd rm your-dracoon.domain.com/parent/folder/to/delete
+```
+**Warning: Deleting rooms cannot be undone!**
+
+### List nodes
+
+In order to list all nodes, use the `ls` command:
+
+```bash
+dccmd ls your-dracoon.domain.com/
+```
+*Note: In order to list the root node, you need to provide a trailing `/`*
+For a specific container (room or folder), use the path:
+```bash
+dccmd ls your-dracoon.domain.com/your/room
+```
+
+#### Displaying additional information
+Using the `ls` command by default only provides node names.
+In order to display more information, use relevant flags:
+
+* Display all information (size, last updated, last update user): `--long` (`-l`)
+    * Display sizes in human readable format (B, KB..): `--human-readable` (`-h`)
+* Display node id: `--inode` (`-i`)
+
+Example displaying full information:
+
+```bash
+dccmd ls -h -i -l your-dracoon.domain.com/your/room
+```
+### Download
+
+To download a file, use the `download` command:
+
+```bash
+dccmd download your-dracoon.domain.com/your/cool-file.mp4 /target/directory
+```
+
+To download a room or a folder, use the `download` command with `--recursive` (`-r`) flag:
+
+```bash
+dccmd download -r your-dracoon.domain.com/your/cool-folder /target/directory
+```
+
+#### Advanced usage
+If you download folders recursively, you might encounter performance issues, specifically when downloading many small files. 
+You can therefore adjust concurrent file uploads via the `--velocity` (`-v`) flag:
+
+```bash
+dccmd upload -r /path/to/folder your-dracoon.domain.com/ -v 3
+```
+The default value is 2 - it does not coincide with real request value.<br>
+Maximum (although not recommended) value is 10. Entering higher numbers will result in max value use.<br>
+Minimum value is 1 - this will not download a folder per file but is the minimum concurrent request value. Entering lower numbers will result in min value use.
+
+### User operations
+
+You can list, edit and import users with relevant `dccmd users` command:
+
+* csv-import  Add a list of users to DRACOON from a CSV file
+* ls          Get a list of users in DRACOON
+* rm          Delete a user
+
+#### Importing users
+
+You can import users by using the `csv-import` command and providing a path to the csv file:
+
+```bash
+dccmd users csv-import /path/to/users.csv your-dracoon.domain.com/
+```
+
+The csv file must contain a header and should include the following attributes:
+
+* first name
+* last name
+* email 
+* login (optional)
+
+By default, local users are created - if you want to import oidc users, you need pass the oidc config id:
+
+```bash
+#example with OIDC config 5
+dccmd users csv-import /path/to/users.csv your-dracoon.domain.com/ 5
+```
+
+#### Listing users
+
+You can list all users using the `ls` command:
+
+```bash
+dccmd users ls your-dracoon.domain.com/
+```
+
+You can get all users also as csv format by using the `--csv` flag:
+
+```bash
+dccmd users ls your-dracoon.domain.com/ --csv > users.csv
+```
+
+To find a user, you can pass a search string to search for either first name, last name or user name (search string applies to all):
+
+```bash
+# will return all users with either first name, last name or user name containing 'yourname'
+dccmd users ls your-dracoon.domain.com/ yourname
+```
+
+#### Deleting users
+
+You can delete a user by providing the username:
+```bash
+dccmd users rm your-dracoon.domain.com/ user123
+```
+
+### Room permissions management
+
+For an overview of the available commands use 
+
+```bash
+dccmd rooms --help
+```
+
+#### List user / group permissions in a room
+
+To list user permissions in a room, use the `list-users` command:
+
+```bash
+dccmd rooms list-users your-dracoon.domain.com/your-room
+```
+You need minimum `read` permissions to list users.
+
+To list group permissions in a room, use the `list-groups` command:
+
+```bash
+dccmd rooms list-groups your-dracoon.domain.com/your-room
+```
+You need minimum `read` permissions to list groups.
+
+As with other commands, you can use the `--csv` flag to get a csv export for the room
+permissions (users and groups).
+
+#### Add user / group to a room
+
+Currently, the following templates are available:
+- read: read-only perrmissions for a room 
+- edit: edit permissions for a room
+- admin: room admin permissions
+
+The permissions coincide with the templates in use of the official DRACOON Web App.
+
+You need `manage` permissions (room admin) to add users / groups.
+
+To add a user, use the `add-user` command and provide the user and permission template (`-u` and `-p`):
+
+```bash
+dccmd rooms add-user -u "user.name" -p admin your-dracoon.domain.com/your-room
+```
+
+To add a group, use the `add-group` command and provide the group and permission template (`-g` and `-p`):
+
+```bash
+dccmd rooms add-group -g "group.name" -p admin your-dracoon.domain.com/your-room
+```
+
+#### Remove user / group from a room
+
+You need `manage` permissions (room admin) to remove users / groups.
+
+To add a user, use the `remove-user` command and provide the user (`-u`):
+
+```bash
+dccmd rooms remove-user -u "user.name" your-dracoon.domain.com/your-room
+```
+
+To add a group, use the `remove-group` command and provide the group (`-g`):
+
+```bash
+dccmd rooms remove-group -g "group.name" your-dracoon.domain.com/your-room
+```
+
+## Configuration / administration
+
+You can view / manage the configuration for `dccmd` using the relevant commands:
+
+* `dccmd auth` - manage credentials
+    * `dccmd auth ls your.dracoon.domain.com` will display if a refresh token has been stored for the provided domain
+    * `dccmd auth rm your-dracoon.domain.com` will remove stored credentials for the provided domain
+* `dccmd client` - manage client
+    * `dccmd client register your.dracoon.domain.com` will start the registration process for a client and given domain
+    * `dccmd client ls your.dracoon.domain.com` will display client information for the provided domain
+    * `dccmd client rm your-dracoon.domain.com` will remove the stored client config for the provided domain
+* `dccmd crypto` - manage encryption
+    * `dccmd crypto ls your.dracoon.domain.com` will display if encryption password is stored for the provided domain
+    * `dccmd crypto rm your-dracoon.domain.com` will remove the encryption password for the provided domain
+    * `dccmd crypto distribute your-dracoon.domain.com/` will generate file keys available to distribute - if providing a specific path (`dccmd crypto distribute your-dracoon.domain.com/some/path`), only keys for provided parent room will be generated.
+
+### Logging 
+When using a command, a log will be created in the current working directory.
+Currently it is not possible to configure a default path for a log.
+
+You can stream the log to stdout by using the `--debug` flag with any DRACOON-specific command (`upload`, `download`, `ls`, `rm`, `mkdir`, `mkroom`).
+
+
+## License
+Distributed under the Apache License. See [LICENSE](/LICENSE) for more information.
+
```

