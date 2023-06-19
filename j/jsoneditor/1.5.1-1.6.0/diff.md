# Comparing `tmp/jsoneditor-1.5.1.tar.gz` & `tmp/jsoneditor-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsoneditor-1.5.1.tar", last modified: Thu Feb 17 22:21:11 2022, max compression
+gzip compressed data, was "jsoneditor-1.6.0.tar", last modified: Mon Jun 19 19:26:21 2023, max compression
```

## Comparing `jsoneditor-1.5.1.tar` & `jsoneditor-1.6.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 cheskel   (1000) cheskel   (1000)        0 2022-02-17 22:21:11.574922 jsoneditor-1.5.1/
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)       63 2021-11-25 05:03:12.000000 jsoneditor-1.5.1/MANIFEST.in
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)     6511 2022-02-17 22:21:11.574922 jsoneditor-1.5.1/PKG-INFO
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)     5152 2022-02-17 12:53:53.000000 jsoneditor-1.5.1/README.md
-drwxrwxr-x   0 cheskel   (1000) cheskel   (1000)        0 2022-02-17 22:21:11.570922 jsoneditor-1.5.1/jsoneditor/
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)       62 2022-02-17 22:20:58.000000 jsoneditor-1.5.1/jsoneditor/__init__.py
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)       58 2021-11-25 05:03:12.000000 jsoneditor-1.5.1/jsoneditor/__main__.py
-drwxrwxr-x   0 cheskel   (1000) cheskel   (1000)        0 2022-02-17 22:21:11.574922 jsoneditor-1.5.1/jsoneditor/files/
-drwxrwxr-x   0 cheskel   (1000) cheskel   (1000)        0 2022-02-17 22:21:11.574922 jsoneditor-1.5.1/jsoneditor/files/img/
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)      157 2021-11-25 05:03:12.000000 jsoneditor-1.5.1/jsoneditor/files/img/checkmark.svg
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)      278 2021-11-25 05:03:12.000000 jsoneditor-1.5.1/jsoneditor/files/img/close.svg
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)     1150 2021-11-25 05:03:12.000000 jsoneditor-1.5.1/jsoneditor/files/img/favicon.ico
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)    31482 2021-11-25 05:03:12.000000 jsoneditor-1.5.1/jsoneditor/files/img/jsoneditor-icons.svg
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)      168 2022-02-17 12:53:53.000000 jsoneditor-1.5.1/jsoneditor/files/index.css
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)      459 2022-02-17 12:53:53.000000 jsoneditor-1.5.1/jsoneditor/files/index.html
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)     2405 2022-02-17 12:53:53.000000 jsoneditor-1.5.1/jsoneditor/files/index.js
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)    35417 2022-02-17 12:53:53.000000 jsoneditor-1.5.1/jsoneditor/files/jsoneditor.min.css
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)   890746 2022-02-17 12:53:53.000000 jsoneditor-1.5.1/jsoneditor/files/jsoneditor.min.js
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)    13599 2022-02-17 22:16:22.000000 jsoneditor-1.5.1/jsoneditor/jsoneditor.py
-drwxrwxr-x   0 cheskel   (1000) cheskel   (1000)        0 2022-02-17 22:21:11.574922 jsoneditor-1.5.1/jsoneditor.egg-info/
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)     6511 2022-02-17 22:21:11.000000 jsoneditor-1.5.1/jsoneditor.egg-info/PKG-INFO
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)      617 2022-02-17 22:21:11.000000 jsoneditor-1.5.1/jsoneditor.egg-info/SOURCES.txt
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)        1 2022-02-17 22:21:11.000000 jsoneditor-1.5.1/jsoneditor.egg-info/dependency_links.txt
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)       48 2022-02-17 22:21:11.000000 jsoneditor-1.5.1/jsoneditor.egg-info/entry_points.txt
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)       19 2022-02-17 22:21:11.000000 jsoneditor-1.5.1/jsoneditor.egg-info/requires.txt
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)       11 2022-02-17 22:21:11.000000 jsoneditor-1.5.1/jsoneditor.egg-info/top_level.txt
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)       19 2021-11-25 05:03:12.000000 jsoneditor-1.5.1/requirements.txt
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)       38 2022-02-17 22:21:11.574922 jsoneditor-1.5.1/setup.cfg
--rw-rw-r--   0 cheskel   (1000) cheskel   (1000)     1158 2021-11-25 05:03:12.000000 jsoneditor-1.5.1/setup.py
+drwxr-xr-x   0 cheskeltwersky   (501) staff       (20)        0 2023-06-19 19:26:21.659388 jsoneditor-1.6.0/
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)     1072 2023-06-19 19:06:23.000000 jsoneditor-1.6.0/LICENSE
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)       63 2023-06-19 19:06:23.000000 jsoneditor-1.6.0/MANIFEST.in
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)     5871 2023-06-19 19:26:21.659269 jsoneditor-1.6.0/PKG-INFO
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)     5349 2023-06-19 19:26:00.000000 jsoneditor-1.6.0/README.md
+drwxr-xr-x   0 cheskeltwersky   (501) staff       (20)        0 2023-06-19 19:26:21.656599 jsoneditor-1.6.0/jsoneditor/
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)       62 2023-06-19 19:26:12.000000 jsoneditor-1.6.0/jsoneditor/__init__.py
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)       58 2023-06-19 19:06:23.000000 jsoneditor-1.6.0/jsoneditor/__main__.py
+drwxr-xr-x   0 cheskeltwersky   (501) staff       (20)        0 2023-06-19 19:26:21.658083 jsoneditor-1.6.0/jsoneditor/files/
+drwxr-xr-x   0 cheskeltwersky   (501) staff       (20)        0 2023-06-19 19:26:21.659072 jsoneditor-1.6.0/jsoneditor/files/img/
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)      157 2023-06-19 19:06:23.000000 jsoneditor-1.6.0/jsoneditor/files/img/checkmark.svg
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)      278 2023-06-19 19:06:23.000000 jsoneditor-1.6.0/jsoneditor/files/img/close.svg
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)     1150 2023-06-19 19:06:23.000000 jsoneditor-1.6.0/jsoneditor/files/img/favicon.ico
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)    31482 2023-06-19 19:06:23.000000 jsoneditor-1.6.0/jsoneditor/files/img/jsoneditor-icons.svg
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)      168 2023-06-19 19:06:23.000000 jsoneditor-1.6.0/jsoneditor/files/index.css
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)      459 2023-06-19 19:06:23.000000 jsoneditor-1.6.0/jsoneditor/files/index.html
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)     2405 2023-06-19 19:06:23.000000 jsoneditor-1.6.0/jsoneditor/files/index.js
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)    35417 2023-06-19 19:06:23.000000 jsoneditor-1.6.0/jsoneditor/files/jsoneditor.min.css
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)   890746 2023-06-19 19:06:23.000000 jsoneditor-1.6.0/jsoneditor/files/jsoneditor.min.js
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)    14354 2023-06-19 19:24:00.000000 jsoneditor-1.6.0/jsoneditor/jsoneditor.py
+drwxr-xr-x   0 cheskeltwersky   (501) staff       (20)        0 2023-06-19 19:26:21.657421 jsoneditor-1.6.0/jsoneditor.egg-info/
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)     5871 2023-06-19 19:26:21.000000 jsoneditor-1.6.0/jsoneditor.egg-info/PKG-INFO
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)      625 2023-06-19 19:26:21.000000 jsoneditor-1.6.0/jsoneditor.egg-info/SOURCES.txt
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)        1 2023-06-19 19:26:21.000000 jsoneditor-1.6.0/jsoneditor.egg-info/dependency_links.txt
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)       48 2023-06-19 19:26:21.000000 jsoneditor-1.6.0/jsoneditor.egg-info/entry_points.txt
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)       26 2023-06-19 19:26:21.000000 jsoneditor-1.6.0/jsoneditor.egg-info/requires.txt
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)       11 2023-06-19 19:26:21.000000 jsoneditor-1.6.0/jsoneditor.egg-info/top_level.txt
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)       26 2023-06-19 19:12:14.000000 jsoneditor-1.6.0/requirements.txt
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)       38 2023-06-19 19:26:21.659431 jsoneditor-1.6.0/setup.cfg
+-rw-r--r--   0 cheskeltwersky   (501) staff       (20)     1158 2023-06-19 19:06:23.000000 jsoneditor-1.6.0/setup.py
```

### Comparing `jsoneditor-1.5.1/PKG-INFO` & `jsoneditor-1.6.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,122 +1,108 @@
-Metadata-Version: 2.1
-Name: jsoneditor
-Version: 1.5.1
-Summary: Visualize and edit JSON
-Home-page: https://github.com/dermasmid/py-jsoneditor
-Author: Cheskel Twersky
-Author-email: twerskycheskel@gmail.com
-License: MIT
-Description: # 💥py-jsoneditor💥
-        Quickly View and Edit any JSON data.
-        
-        
-        # Why?
-        
-        When working with JSON data, You often need to get a structured view of the JSON in order to be able to work with it. There's an online tool [https://jsoneditoronline.org/](https://jsoneditoronline.org/) which I used for this, but copying/pasting all the time got frustrating pretty quickly, This is why I created this package which you can launch right from Python or from the command line.
-        
-        
-        # Screenshot
-        
-        ![](https://res.cloudinary.com/dermasmid/image/upload/v1624745064/Screenshot_from_2021-06-27_01-02-58_qymcrb.png)
-        
-        
-        # Installation
-        
-        ```bash
-        pip install jsoneditor
-        ```
-        
-        
-        # Python example
-        
-        In python you can simply import `jsoneditor` and call the `editjson` function, the first argument is going to be the data. See [Formats you can pass the JSON as](#formats-you-can-pass-the-json-as) for all the formats you can pass the JSON in. See [Python api](#python-api) for a full list of addtional arguments that you can pass to `editjson`.
-        ```python
-        import requests
-        import jsoneditor
-        
-        data = requests.get('https://jsonplaceholder.typicode.com/comments').json()
-        jsoneditor.editjson(data)
-        ```
-        
-        
-        # Command line example
-        
-        From the command line you can either pass the data as an argument as so:
-        ```bash
-        jsoneditor '{"Hey": "Hi"}'
-        ```
-        Or you can pipe it in like so:
-        ```bash
-        curl https://jsonplaceholder.typicode.com/comments | jsoneditor
-        ```
-        Or you can use what you have in your clipboard like so:
-        ```bash
-        jsoneditor -c
-        ```
-        See [Formats you can pass the JSON as](#formats-you-can-pass-the-json-as) for all the formats you can pass the JSON in.
-        
-        Refer to [CLI options](#cli-options) for a list of all cli options. Alternatively you can run `jsoneditor --help` from your terminal to see it.
-        
-        
-        ## <a></a>Formats you can pass the JSON as
-        
-        You can pass the json in any of the following formats:
-        * as valid json string. Example: `{"Hey": "Hi"}`
-        * as a python dict. Example: `{'Hey': 'hi'}`
-        * as a url the points to valid json. Example: `https://jsonplaceholder.typicode.com/comments`
-        * as a file path that is valid json. Example: `data.json`
-        
-        
-        ## <a></a>Python Api
-        
-        | parameter | type    | optional  |description                                                                  |
-        | --------- | ------- | -------- |-----------------------------------------------------------------------------|
-        | `data`    | `Any`     | ❌ |  The data in any of [these](#formats-you-can-pass-the-json-as) formats.       |
-        | `callback`| `callable`| ✔️ |  If you provide this argument you will have a ✅ button which will trigger this callback.|
-        | `options` | `dict`    | ✔️ | Options to pass the the jsoneditor object. See [here](https://github.com/josdejong/jsoneditor/blob/master/docs/api.md#configuration-options)|
-        | `additional_js`| `str`| ✔️ |  You can pass some JavaScript to run on the client side. You can interact with the editor by accessing the `window.editor` variable.|
-        | `keep_running`| `bool` | ✔️ | Whether to keep the server running. Defaults to `False`.                 |
-        | `run_in_thread`| `bool` | ✔️ | Whether to run the server in a separate thread. Defaults to `False`.    |
-        | `is_csv`| `bool` | ✔️ | Whether the data is csv data. Defaults to `False`.                             |
-        | `is_ndjson`| `bool` | ✔️ | Whether the data is Newline Delimited JSON  . Defaults to `False`.          |
-        | `is_js_object`| `bool` | ✔️ | Whether the data is a JavaScript Object. Defaults to `False`.            |
-        | `title`| `str` | ✔️ | A title to display in the browser.                                               |
-        | `port`| `int` | ✔️ | specify which port to use.                                                        |
-        
-        
-        ## <a></a>CLI options
-        
-        | parameter | description                                                           |
-        | --------- | ----------------------------------------------------------------------|
-        | `data`    | The data in any of [these](#formats-you-can-pass-the-json-as) formats |
-        | `-o`      | Add a button that will output the json back to the console            |
-        | `-b`      | Keep running in background                                            |
-        | `-c`      | Get JSON input from clipboard                                         |
-        | `-k`      | Keep alive                                                            |
-        | `-e`      | Edit mode                                                             |
-        | `-n`      | Don't launch browser                                                  |
-        | `-p`      | Server port                                                           |
-        | `--out`   | File to output when in edit mode                                      |
-        | `-t`      | Title to display in browser window                                    |
-        | `--csv`   | Input is CSV                                                          |
-        | `--js`    | Input is a JavaScript Object                                          |
-        | `--ndjson`| Input is Newline Delimited JSON                                       |
-        
-        
-        ## Build
-        
-        ```bash
-        python setup.py sdist
-        ```
-        
-        # Acknowledgements
-        
-        * [jsoneditor](https://github.com/josdejong/jsoneditor)
-        
-Keywords: python3 json jsoneditor api gui editor csv
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# 💥py-jsoneditor💥
+Quickly View and Edit any JSON data.
+
+
+# Why?
+
+When working with JSON data, You often need to get a structured view of the JSON in order to be able to work with it. There's an online tool [https://jsoneditoronline.org/](https://jsoneditoronline.org/) which I used for this, but copying/pasting all the time got frustrating pretty quickly, This is why I created this package which you can launch right from Python or from the command line.
+
+
+# Screenshot
+
+![](https://res.cloudinary.com/dermasmid/image/upload/v1624745064/Screenshot_from_2021-06-27_01-02-58_qymcrb.png)
+
+
+# Installation
+
+```bash
+pip install jsoneditor
+```
+
+
+# Python example
+
+In python you can simply import `jsoneditor` and call the `editjson` function, the first argument is going to be the data. See [Formats you can pass the JSON as](#formats-you-can-pass-the-json-as) for all the formats you can pass the JSON in. See [Python api](#python-api) for a full list of addtional arguments that you can pass to `editjson`.
+```python
+import requests
+import jsoneditor
+
+data = requests.get('https://jsonplaceholder.typicode.com/comments').json()
+jsoneditor.editjson(data)
+```
+
+
+# Command line example
+
+From the command line you can either pass the data as an argument as so:
+```bash
+jsoneditor '{"Hey": "Hi"}'
+```
+Or you can pipe it in like so:
+```bash
+curl https://jsonplaceholder.typicode.com/comments | jsoneditor
+```
+Or you can use what you have in your clipboard like so:
+```bash
+jsoneditor -c
+```
+See [Formats you can pass the JSON as](#formats-you-can-pass-the-json-as) for all the formats you can pass the JSON in.
+
+Refer to [CLI options](#cli-options) for a list of all cli options. Alternatively you can run `jsoneditor --help` from your terminal to see it.
+
+
+## <a></a>Formats you can pass the JSON as
+
+You can pass the json in any of the following formats:
+* as valid json string. Example: `{"Hey": "Hi"}`
+* as a python dict. Example: `{'Hey': 'hi'}`
+* as a url the points to valid json. Example: `https://jsonplaceholder.typicode.com/comments`
+* as a file path that is valid json. Example: `data.json`
+
+
+## <a></a>Python Api
+
+| parameter | type    | optional  |description                                                                  |
+| --------- | ------- | -------- |-----------------------------------------------------------------------------|
+| `data`    | `Any`     | ❌ |  The data in any of [these](#formats-you-can-pass-the-json-as) formats.       |
+| `callback`| `callable`| ✔️ |  If you provide this argument you will have a ✅ button which will trigger this callback.|
+| `options` | `dict`    | ✔️ | Options to pass the the jsoneditor object. See [here](https://github.com/josdejong/jsoneditor/blob/master/docs/api.md#configuration-options)|
+| `additional_js`| `str`| ✔️ |  You can pass some JavaScript to run on the client side. You can interact with the editor by accessing the `window.editor` variable.|
+| `keep_running`| `bool` | ✔️ | Whether to keep the server running. Defaults to `False`.                 |
+| `run_in_thread`| `bool` | ✔️ | Whether to run the server in a separate thread. Defaults to `False`.    |
+| `is_csv`| `bool` | ✔️ | Whether the data is csv data. Defaults to `False`.                             |
+| `is_yaml`| `bool` | ✔️ | Whether the data is yaml data. Defaults to `False`.                           |
+| `is_ndjson`| `bool` | ✔️ | Whether the data is Newline Delimited JSON  . Defaults to `False`.          |
+| `is_js_object`| `bool` | ✔️ | Whether the data is a JavaScript Object. Defaults to `False`.            |
+| `title`| `str` | ✔️ | A title to display in the browser.                                               |
+| `port`| `int` | ✔️ | specify which port to use.                                                        |
+
+
+## <a></a>CLI options
+
+| parameter | description                                                           |
+| --------- | ----------------------------------------------------------------------|
+| `data`    | The data in any of [these](#formats-you-can-pass-the-json-as) formats |
+| `-o`      | Add a button that will output the json back to the console            |
+| `-b`      | Keep running in background                                            |
+| `-c`      | Get JSON input from clipboard                                         |
+| `-k`      | Keep alive                                                            |
+| `-e`      | Edit mode                                                             |
+| `-n`      | Don't launch browser                                                  |
+| `-p`      | Server port                                                           |
+| `--out`   | File to output when in edit mode                                      |
+| `-t`      | Title to display in browser window                                    |
+| `--csv`   | Input is CSV                                                          |
+| `--yaml`  | Input is YAML                                                         |
+| `--js`    | Input is a JavaScript Object                                          |
+| `--ndjson`| Input is Newline Delimited JSON                                       |
+
+
+## Build
+
+```bash
+python setup.py sdist
+```
+
+# Acknowledgements
+
+* [jsoneditor](https://github.com/josdejong/jsoneditor)
```

### Comparing `jsoneditor-1.5.1/README.md` & `jsoneditor-1.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: jsoneditor
+Version: 1.6.0
+Summary: Visualize and edit JSON
+Home-page: https://github.com/dermasmid/py-jsoneditor
+Author: Cheskel Twersky
+Author-email: twerskycheskel@gmail.com
+License: MIT
+Keywords: python3 json jsoneditor api gui editor csv
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 💥py-jsoneditor💥
 Quickly View and Edit any JSON data.
 
 
 # Why?
 
 When working with JSON data, You often need to get a structured view of the JSON in order to be able to work with it. There's an online tool [https://jsoneditoronline.org/](https://jsoneditoronline.org/) which I used for this, but copying/pasting all the time got frustrating pretty quickly, This is why I created this package which you can launch right from Python or from the command line.
@@ -66,14 +83,15 @@
 | `data`    | `Any`     | ❌ |  The data in any of [these](#formats-you-can-pass-the-json-as) formats.       |
 | `callback`| `callable`| ✔️ |  If you provide this argument you will have a ✅ button which will trigger this callback.|
 | `options` | `dict`    | ✔️ | Options to pass the the jsoneditor object. See [here](https://github.com/josdejong/jsoneditor/blob/master/docs/api.md#configuration-options)|
 | `additional_js`| `str`| ✔️ |  You can pass some JavaScript to run on the client side. You can interact with the editor by accessing the `window.editor` variable.|
 | `keep_running`| `bool` | ✔️ | Whether to keep the server running. Defaults to `False`.                 |
 | `run_in_thread`| `bool` | ✔️ | Whether to run the server in a separate thread. Defaults to `False`.    |
 | `is_csv`| `bool` | ✔️ | Whether the data is csv data. Defaults to `False`.                             |
+| `is_yaml`| `bool` | ✔️ | Whether the data is yaml data. Defaults to `False`.                           |
 | `is_ndjson`| `bool` | ✔️ | Whether the data is Newline Delimited JSON  . Defaults to `False`.          |
 | `is_js_object`| `bool` | ✔️ | Whether the data is a JavaScript Object. Defaults to `False`.            |
 | `title`| `str` | ✔️ | A title to display in the browser.                                               |
 | `port`| `int` | ✔️ | specify which port to use.                                                        |
 
 
 ## <a></a>CLI options
@@ -87,20 +105,23 @@
 | `-k`      | Keep alive                                                            |
 | `-e`      | Edit mode                                                             |
 | `-n`      | Don't launch browser                                                  |
 | `-p`      | Server port                                                           |
 | `--out`   | File to output when in edit mode                                      |
 | `-t`      | Title to display in browser window                                    |
 | `--csv`   | Input is CSV                                                          |
+| `--yaml`  | Input is YAML                                                         |
 | `--js`    | Input is a JavaScript Object                                          |
 | `--ndjson`| Input is Newline Delimited JSON                                       |
 
 
 ## Build
 
 ```bash
 python setup.py sdist
 ```
 
 # Acknowledgements
 
 * [jsoneditor](https://github.com/josdejong/jsoneditor)
+
+
```

### Comparing `jsoneditor-1.5.1/jsoneditor/files/img/favicon.ico` & `jsoneditor-1.6.0/jsoneditor/files/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `jsoneditor-1.5.1/jsoneditor/files/img/jsoneditor-icons.svg` & `jsoneditor-1.6.0/jsoneditor/files/img/jsoneditor-icons.svg`

 * *Files identical despite different names*

### Comparing `jsoneditor-1.5.1/jsoneditor/files/index.js` & `jsoneditor-1.6.0/jsoneditor/files/index.js`

 * *Files identical despite different names*

### Comparing `jsoneditor-1.5.1/jsoneditor/files/jsoneditor.min.css` & `jsoneditor-1.6.0/jsoneditor/files/jsoneditor.min.css`

 * *Files identical despite different names*

### Comparing `jsoneditor-1.5.1/jsoneditor/files/jsoneditor.min.js` & `jsoneditor-1.6.0/jsoneditor/files/jsoneditor.min.js`

 * *Files identical despite different names*

### Comparing `jsoneditor-1.5.1/jsoneditor/jsoneditor.py` & `jsoneditor-1.6.0/jsoneditor/jsoneditor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import ast
 import csv
 import json
 import mimetypes
+import yaml
 import os
 import random
 import subprocess
 import sys
 import threading
 import webbrowser
 from collections.abc import Mapping
@@ -48,26 +49,28 @@
         data: Union[dict, str, list],
         callback: Callable[[dict], Any] = None,
         options: dict = None,
         additional_js: str = None,
         keep_running: bool = False,
         run_in_thread: bool = False,
         is_csv: bool = False,
+        is_yaml: bool = False,
         is_ndjson: bool = False,
         is_js_object: bool = False,
         title: str = None,
         port: int = None,
         no_browser: bool = False,
     ) -> None:
         self.callback = callback
         self.options = options
         self.additional_js = additional_js
         self.keep_running = keep_running
         self.run_in_thread = run_in_thread
         self.is_csv = is_csv
+        self.is_yaml = is_yaml
         self.is_ndjson = is_ndjson
         self.is_js_object = is_js_object
         self.title = title
         self.no_browser = no_browser
         self.get_random_port(port)
         self.data = self.get_json(data)
         self.server = None
@@ -125,25 +128,31 @@
     @staticmethod
     def is_file(source: str) -> bool:
         return os.path.exists(source)
 
     def detect_source_by_filename(self, source: str):
         if source.endswith(".csv"):
             self.is_csv = True
+        elif source.endswith(".yaml"):
+            self.is_yaml = True
         elif any(source.endswith(ext) for ext in [".ndjson", ".jsonl"]):
             self.is_ndjson = True
 
     def load_json(self, source):
         if self.is_csv:
             if isinstance(source, str):
                 # Throws an error if the input is not valid csv
                 csv.Sniffer().sniff(source[:1024], delimiters=",:;\t")
                 result = list(csv.DictReader(source.split("\n")))
             elif isinstance(source, TextIOWrapper):
                 result = list(csv.DictReader(source))
+        elif self.is_yaml:
+            result = list(filter(bool, yaml.load_all(source, Loader=yaml.UnsafeLoader)))
+            if len(result) == 1:
+                result = result[0]
         elif self.is_ndjson:
             if isinstance(source, str):
                 lines = source.splitlines()
             elif isinstance(source, TextIOWrapper):
                 lines = source.readlines()
             result = list(json.loads(line) for line in lines)
         elif self.is_js_object:
@@ -209,14 +218,18 @@
         # callback endpoint
         elif method == "POST":
             if path == "/callback":
                 request_body_size = int(environ["CONTENT_LENGTH"])
                 callback_data = json.loads(
                     environ["wsgi.input"].read(request_body_size).decode("utf-8")
                 )["data"]
+                # fix for edit mode with keep alive setting
+                # apply the recieved data to instance data
+                # without this a refresh doesn't reflect saved changes
+                self.data = callback_data
                 self.callback(callback_data)
                 self.send_response("200 OK", "text/plain", respond)
                 yield b""
 
     def start(self):
         # We might get an error if the port is in use.
         while True:
@@ -249,14 +262,15 @@
     data: Union[dict, str, list],
     callback: Callable[[dict], Any] = None,
     options: dict = None,
     additional_js: str = None,
     keep_running: bool = False,
     run_in_thread: bool = False,
     is_csv: bool = False,
+    is_yaml: bool = False,
     is_ndjson: bool = False,
     is_js_object: bool = False,
     title: str = None,
     port: int = None,
     no_browser: bool = False,
 ) -> Server:
     keep_running = keep_running or bool(callback)
@@ -265,14 +279,15 @@
         data,
         callback,
         options,
         additional_js,
         keep_running,
         run_in_thread,
         is_csv,
+        is_yaml,
         is_ndjson,
         is_js_object,
         title,
         port,
         no_browser,
     )
 
@@ -324,14 +339,15 @@
     parser.add_argument("-k", help="Keep alive", action="store_true")
     parser.add_argument("-e", help="Edit mode", action="store_true")
     parser.add_argument("-n", help="Don't launch browser", action="store_true")
     parser.add_argument("-p", help="Server port")
     parser.add_argument("--out", help="File to output when in edit mode")
     parser.add_argument("-t", help="Title to display in browser window")
     parser.add_argument("--csv", help="Input is CSV", action="store_true")
+    parser.add_argument("--yaml", help="Input is YAML", action="store_true")
     parser.add_argument(
         "--js", help="Input is a JavaScript Object", action="store_true"
     )
     parser.add_argument(
         "--ndjson", help="Input is Newline Delimited JSON", action="store_true"
     )
     args = parser.parse_args()
@@ -354,29 +370,32 @@
 
     if args.n:
         options["no_browser"] = True
 
     if args.csv:
         options["is_csv"] = True
 
+    if args.yaml:
+        options["is_yaml"] = True
+
     if args.js:
         options["is_js_object"] = True
 
     if args.ndjson:
         options["is_ndjson"] = True
 
     if not os.isatty(0):
         options["data"] = "".join(x for x in sys.stdin)
     else:
         if args.data:
             options["data"] = args.data
         elif args.c:
             options["data"] = pyperclip.paste()
         else:
-            raise ValueError("No data passed")
+            raise ValueError("No data passed.")
 
     if args.e:
 
         def edit_file(json_data: dict):
             file_path = None
             if args.out:
                 file_path = args.out
```

### Comparing `jsoneditor-1.5.1/jsoneditor.egg-info/PKG-INFO` & `jsoneditor-1.6.0/jsoneditor.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,122 +1,127 @@
 Metadata-Version: 2.1
 Name: jsoneditor
-Version: 1.5.1
+Version: 1.6.0
 Summary: Visualize and edit JSON
 Home-page: https://github.com/dermasmid/py-jsoneditor
 Author: Cheskel Twersky
 Author-email: twerskycheskel@gmail.com
 License: MIT
-Description: # 💥py-jsoneditor💥
-        Quickly View and Edit any JSON data.
-        
-        
-        # Why?
-        
-        When working with JSON data, You often need to get a structured view of the JSON in order to be able to work with it. There's an online tool [https://jsoneditoronline.org/](https://jsoneditoronline.org/) which I used for this, but copying/pasting all the time got frustrating pretty quickly, This is why I created this package which you can launch right from Python or from the command line.
-        
-        
-        # Screenshot
-        
-        ![](https://res.cloudinary.com/dermasmid/image/upload/v1624745064/Screenshot_from_2021-06-27_01-02-58_qymcrb.png)
-        
-        
-        # Installation
-        
-        ```bash
-        pip install jsoneditor
-        ```
-        
-        
-        # Python example
-        
-        In python you can simply import `jsoneditor` and call the `editjson` function, the first argument is going to be the data. See [Formats you can pass the JSON as](#formats-you-can-pass-the-json-as) for all the formats you can pass the JSON in. See [Python api](#python-api) for a full list of addtional arguments that you can pass to `editjson`.
-        ```python
-        import requests
-        import jsoneditor
-        
-        data = requests.get('https://jsonplaceholder.typicode.com/comments').json()
-        jsoneditor.editjson(data)
-        ```
-        
-        
-        # Command line example
-        
-        From the command line you can either pass the data as an argument as so:
-        ```bash
-        jsoneditor '{"Hey": "Hi"}'
-        ```
-        Or you can pipe it in like so:
-        ```bash
-        curl https://jsonplaceholder.typicode.com/comments | jsoneditor
-        ```
-        Or you can use what you have in your clipboard like so:
-        ```bash
-        jsoneditor -c
-        ```
-        See [Formats you can pass the JSON as](#formats-you-can-pass-the-json-as) for all the formats you can pass the JSON in.
-        
-        Refer to [CLI options](#cli-options) for a list of all cli options. Alternatively you can run `jsoneditor --help` from your terminal to see it.
-        
-        
-        ## <a></a>Formats you can pass the JSON as
-        
-        You can pass the json in any of the following formats:
-        * as valid json string. Example: `{"Hey": "Hi"}`
-        * as a python dict. Example: `{'Hey': 'hi'}`
-        * as a url the points to valid json. Example: `https://jsonplaceholder.typicode.com/comments`
-        * as a file path that is valid json. Example: `data.json`
-        
-        
-        ## <a></a>Python Api
-        
-        | parameter | type    | optional  |description                                                                  |
-        | --------- | ------- | -------- |-----------------------------------------------------------------------------|
-        | `data`    | `Any`     | ❌ |  The data in any of [these](#formats-you-can-pass-the-json-as) formats.       |
-        | `callback`| `callable`| ✔️ |  If you provide this argument you will have a ✅ button which will trigger this callback.|
-        | `options` | `dict`    | ✔️ | Options to pass the the jsoneditor object. See [here](https://github.com/josdejong/jsoneditor/blob/master/docs/api.md#configuration-options)|
-        | `additional_js`| `str`| ✔️ |  You can pass some JavaScript to run on the client side. You can interact with the editor by accessing the `window.editor` variable.|
-        | `keep_running`| `bool` | ✔️ | Whether to keep the server running. Defaults to `False`.                 |
-        | `run_in_thread`| `bool` | ✔️ | Whether to run the server in a separate thread. Defaults to `False`.    |
-        | `is_csv`| `bool` | ✔️ | Whether the data is csv data. Defaults to `False`.                             |
-        | `is_ndjson`| `bool` | ✔️ | Whether the data is Newline Delimited JSON  . Defaults to `False`.          |
-        | `is_js_object`| `bool` | ✔️ | Whether the data is a JavaScript Object. Defaults to `False`.            |
-        | `title`| `str` | ✔️ | A title to display in the browser.                                               |
-        | `port`| `int` | ✔️ | specify which port to use.                                                        |
-        
-        
-        ## <a></a>CLI options
-        
-        | parameter | description                                                           |
-        | --------- | ----------------------------------------------------------------------|
-        | `data`    | The data in any of [these](#formats-you-can-pass-the-json-as) formats |
-        | `-o`      | Add a button that will output the json back to the console            |
-        | `-b`      | Keep running in background                                            |
-        | `-c`      | Get JSON input from clipboard                                         |
-        | `-k`      | Keep alive                                                            |
-        | `-e`      | Edit mode                                                             |
-        | `-n`      | Don't launch browser                                                  |
-        | `-p`      | Server port                                                           |
-        | `--out`   | File to output when in edit mode                                      |
-        | `-t`      | Title to display in browser window                                    |
-        | `--csv`   | Input is CSV                                                          |
-        | `--js`    | Input is a JavaScript Object                                          |
-        | `--ndjson`| Input is Newline Delimited JSON                                       |
-        
-        
-        ## Build
-        
-        ```bash
-        python setup.py sdist
-        ```
-        
-        # Acknowledgements
-        
-        * [jsoneditor](https://github.com/josdejong/jsoneditor)
-        
 Keywords: python3 json jsoneditor api gui editor csv
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# 💥py-jsoneditor💥
+Quickly View and Edit any JSON data.
+
+
+# Why?
+
+When working with JSON data, You often need to get a structured view of the JSON in order to be able to work with it. There's an online tool [https://jsoneditoronline.org/](https://jsoneditoronline.org/) which I used for this, but copying/pasting all the time got frustrating pretty quickly, This is why I created this package which you can launch right from Python or from the command line.
+
+
+# Screenshot
+
+![](https://res.cloudinary.com/dermasmid/image/upload/v1624745064/Screenshot_from_2021-06-27_01-02-58_qymcrb.png)
+
+
+# Installation
+
+```bash
+pip install jsoneditor
+```
+
+
+# Python example
+
+In python you can simply import `jsoneditor` and call the `editjson` function, the first argument is going to be the data. See [Formats you can pass the JSON as](#formats-you-can-pass-the-json-as) for all the formats you can pass the JSON in. See [Python api](#python-api) for a full list of addtional arguments that you can pass to `editjson`.
+```python
+import requests
+import jsoneditor
+
+data = requests.get('https://jsonplaceholder.typicode.com/comments').json()
+jsoneditor.editjson(data)
+```
+
+
+# Command line example
+
+From the command line you can either pass the data as an argument as so:
+```bash
+jsoneditor '{"Hey": "Hi"}'
+```
+Or you can pipe it in like so:
+```bash
+curl https://jsonplaceholder.typicode.com/comments | jsoneditor
+```
+Or you can use what you have in your clipboard like so:
+```bash
+jsoneditor -c
+```
+See [Formats you can pass the JSON as](#formats-you-can-pass-the-json-as) for all the formats you can pass the JSON in.
+
+Refer to [CLI options](#cli-options) for a list of all cli options. Alternatively you can run `jsoneditor --help` from your terminal to see it.
+
+
+## <a></a>Formats you can pass the JSON as
+
+You can pass the json in any of the following formats:
+* as valid json string. Example: `{"Hey": "Hi"}`
+* as a python dict. Example: `{'Hey': 'hi'}`
+* as a url the points to valid json. Example: `https://jsonplaceholder.typicode.com/comments`
+* as a file path that is valid json. Example: `data.json`
+
+
+## <a></a>Python Api
+
+| parameter | type    | optional  |description                                                                  |
+| --------- | ------- | -------- |-----------------------------------------------------------------------------|
+| `data`    | `Any`     | ❌ |  The data in any of [these](#formats-you-can-pass-the-json-as) formats.       |
+| `callback`| `callable`| ✔️ |  If you provide this argument you will have a ✅ button which will trigger this callback.|
+| `options` | `dict`    | ✔️ | Options to pass the the jsoneditor object. See [here](https://github.com/josdejong/jsoneditor/blob/master/docs/api.md#configuration-options)|
+| `additional_js`| `str`| ✔️ |  You can pass some JavaScript to run on the client side. You can interact with the editor by accessing the `window.editor` variable.|
+| `keep_running`| `bool` | ✔️ | Whether to keep the server running. Defaults to `False`.                 |
+| `run_in_thread`| `bool` | ✔️ | Whether to run the server in a separate thread. Defaults to `False`.    |
+| `is_csv`| `bool` | ✔️ | Whether the data is csv data. Defaults to `False`.                             |
+| `is_yaml`| `bool` | ✔️ | Whether the data is yaml data. Defaults to `False`.                           |
+| `is_ndjson`| `bool` | ✔️ | Whether the data is Newline Delimited JSON  . Defaults to `False`.          |
+| `is_js_object`| `bool` | ✔️ | Whether the data is a JavaScript Object. Defaults to `False`.            |
+| `title`| `str` | ✔️ | A title to display in the browser.                                               |
+| `port`| `int` | ✔️ | specify which port to use.                                                        |
+
+
+## <a></a>CLI options
+
+| parameter | description                                                           |
+| --------- | ----------------------------------------------------------------------|
+| `data`    | The data in any of [these](#formats-you-can-pass-the-json-as) formats |
+| `-o`      | Add a button that will output the json back to the console            |
+| `-b`      | Keep running in background                                            |
+| `-c`      | Get JSON input from clipboard                                         |
+| `-k`      | Keep alive                                                            |
+| `-e`      | Edit mode                                                             |
+| `-n`      | Don't launch browser                                                  |
+| `-p`      | Server port                                                           |
+| `--out`   | File to output when in edit mode                                      |
+| `-t`      | Title to display in browser window                                    |
+| `--csv`   | Input is CSV                                                          |
+| `--yaml`  | Input is YAML                                                         |
+| `--js`    | Input is a JavaScript Object                                          |
+| `--ndjson`| Input is Newline Delimited JSON                                       |
+
+
+## Build
+
+```bash
+python setup.py sdist
+```
+
+# Acknowledgements
+
+* [jsoneditor](https://github.com/josdejong/jsoneditor)
+
+
```

### Comparing `jsoneditor-1.5.1/jsoneditor.egg-info/SOURCES.txt` & `jsoneditor-1.6.0/jsoneditor.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 jsoneditor/__init__.py
 jsoneditor/__main__.py
 jsoneditor/jsoneditor.py
```

### Comparing `jsoneditor-1.5.1/setup.py` & `jsoneditor-1.6.0/setup.py`

 * *Files identical despite different names*

