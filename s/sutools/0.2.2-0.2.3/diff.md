# Comparing `tmp/sutools-0.2.2.tar.gz` & `tmp/sutools-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sutools-0.2.2.tar", last modified: Fri Jun  2 01:58:42 2023, max compression
+gzip compressed data, was "sutools-0.2.3.tar", last modified: Sun Jun 18 23:27:48 2023, max compression
```

## Comparing `sutools-0.2.2.tar` & `sutools-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:58:42.039376 sutools-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-02 01:58:20.000000 sutools-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-06-02 01:58:42.035376 sutools-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-06-02 01:58:20.000000 sutools-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-02 01:58:20.000000 sutools-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 01:58:42.039376 sutools-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-02 01:58:20.000000 sutools-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:58:42.035376 sutools-0.2.2/sutools/
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-02 01:58:20.000000 sutools-0.2.2/sutools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-02 01:58:20.000000 sutools-0.2.2/sutools/bench_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-02 01:58:20.000000 sutools-0.2.2/sutools/cli_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-02 01:58:20.000000 sutools-0.2.2/sutools/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-02 01:58:20.000000 sutools-0.2.2/sutools/meta_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:58:42.035376 sutools-0.2.2/sutools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-06-02 01:58:42.000000 sutools-0.2.2/sutools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-02 01:58:42.000000 sutools-0.2.2/sutools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:58:42.000000 sutools-0.2.2/sutools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 01:58:42.000000 sutools-0.2.2/sutools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:58:42.035376 sutools-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-02 01:58:20.000000 sutools-0.2.2/tests/test_bench_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-06-02 01:58:20.000000 sutools-0.2.2/tests/test_cli_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18499 2023-06-02 01:58:20.000000 sutools-0.2.2/tests/test_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-02 01:58:20.000000 sutools-0.2.2/tests/test_meta_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-02 01:58:20.000000 sutools-0.2.2/tests/test_sutools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:27:48.512372 sutools-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-18 23:27:27.000000 sutools-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-18 23:27:48.512372 sutools-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-18 23:27:27.000000 sutools-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-18 23:27:27.000000 sutools-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 23:27:48.512372 sutools-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-18 23:27:27.000000 sutools-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:27:48.512372 sutools-0.2.3/sutools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-18 23:27:27.000000 sutools-0.2.3/sutools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-18 23:27:27.000000 sutools-0.2.3/sutools/bench_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-18 23:27:27.000000 sutools-0.2.3/sutools/cli_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-18 23:27:27.000000 sutools-0.2.3/sutools/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-18 23:27:27.000000 sutools-0.2.3/sutools/meta_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:27:48.512372 sutools-0.2.3/sutools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-18 23:27:48.000000 sutools-0.2.3/sutools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-18 23:27:48.000000 sutools-0.2.3/sutools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 23:27:48.000000 sutools-0.2.3/sutools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 23:27:48.000000 sutools-0.2.3/sutools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:27:48.512372 sutools-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-18 23:27:27.000000 sutools-0.2.3/tests/test_bench_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-18 23:27:27.000000 sutools-0.2.3/tests/test_cli_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18499 2023-06-18 23:27:27.000000 sutools-0.2.3/tests/test_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-18 23:27:27.000000 sutools-0.2.3/tests/test_meta_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-18 23:27:27.000000 sutools-0.2.3/tests/test_sutools.py
```

### Comparing `sutools-0.2.2/LICENSE` & `sutools-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sutools-0.2.2/PKG-INFO` & `sutools-0.2.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: sutools
-Version: 0.2.2
-Summary: su (Super User) tools; per module utilities, designed to be lightweight, easy to configure, and reduce boilerplate code.
-Home-page: https://github.com/aastopher/sutools
-Author: Aaron Stopher
-Project-URL: Documentation, https://sutools.readthedocs.io
-Project-URL: Bug Tracker, https://github.com/aastopher/sutools/issues
-Keywords: logs,logger,logging,cli,utils,performance counter,benchmark
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Documentation Status](https://readthedocs.org/projects/sutools/badge/?version=latest)](https://sutools.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/aastopher/sutools/branch/master/graph/badge.svg?token=ZB0AX8D6JI)](https://codecov.io/gh/aastopher/sutools)
 [![PyPI version](https://badge.fury.io/py/sutools.svg)](https://badge.fury.io/py/sutools)
 [![DeepSource](https://deepsource.io/gh/aastopher/sutools.svg/?label=active+issues&show_trend=true&token=RVDa2T7M-E-YSg2DVFbr1ro-)](https://deepsource.io/gh/aastopher/sutools/?ref=repository-badge)
 
 ## Description
 
@@ -140,14 +124,64 @@
     -gr <class 'str'>, --greeting <class 'str'>
                             default: hello
     -fa <class 'str'>, --farewell <class 'str'>
                             default: goodbye
     -h, --help            Show this help message and exit.
 ```
 
+## CLI Using Variadic Functions
+
+Variadic functions are compatible with sutools cli utility. When calling kwargs from the cli; `key=value` should be used instead of `--` and `-`, these are reserved for default arguments.
+
+**NOTE:** since input is from `stdin` it will always be of type `<string>`, sutools will _not_ infer the data type you must infer your needed type within the function.
+
+```python
+"""This module does random stuff."""
+import sutools as su
+
+@su.register
+def variadic(*args, **kwargs):
+    
+    print("Positional arguments:")
+    for arg in args:
+        print(arg)
+
+    print("Keyword arguments:")
+    for key, value in kwargs.items():
+        print(f"{key} = {value}")
+
+    su.logger() # optional
+
+# module level function calls...
+
+if __name__ == '__main__':
+    # main code (will run even when using cli commands)...
+    su.cli(desc = __doc__)
+    # main code (will NOT run when using cli commands)...
+```
+
+**command usage:**
+
+```
+python module.py variadic 1 2 3 foo=1 bar=2
+```
+
+**output:**
+
+```
+Positional arguments:
+1
+2
+3
+Keyword arguments:
+foo = 1
+bar = 2
+```
+
+
 ## Logger Usage Examples
 
 </br>
  
  accessing defined loggers is done with a `log()` helper function. Note the use of `su.log()` in the below functions to access a specified logger before defining the log level and message.
 
 </br>
@@ -304,8 +338,8 @@
 **NOTE:** given an iterable for `arg`, `kwarg`, or `result` the object will be summarized in terms of vector length.
 
 ```
 {'function_name': [{'args': [{'type': 'arg_type', 'value': int}]
                     'benchmark': float,
                     'kwargs': {'kwarg_name': {'type': 'arg_type', 'length': int, }}
                     'result': {'type': 'arg_type', 'value': float}}]}
-```
+```
```

### Comparing `sutools-0.2.2/setup.py` & `sutools-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sutools",
-    version="0.2.2",
+    version="0.2.3",
     author="Aaron Stopher",
     packages=setuptools.find_packages(include=["sutools"]),
     description="su (Super User) tools; per module utilities, designed to be lightweight, easy to configure, and reduce boilerplate code.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aastopher/sutools",
     project_urls={
```

### Comparing `sutools-0.2.2/sutools/__init__.py` & `sutools-0.2.3/sutools/__init__.py`

 * *Files identical despite different names*

### Comparing `sutools-0.2.2/sutools/bench_handler.py` & `sutools-0.2.3/sutools/bench_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.2.2/sutools/cli_handler.py` & `sutools-0.2.3/sutools/cli_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,63 +30,77 @@
     def add_funcs(self, func_dict):
         """add registered functions to the cli"""
 
         self.func_dict = func_dict  # assign function dictionary property
 
         # iterate through registered functions
         for func_name, items in func_dict.items():
-            names = items[1]  # collect arg names
-            types = items[2]  # collect types of arg
+            names = items['names']  # collect arg names
+            types = items['types']  # collect types of arg
             arg_types = [types.get(name, None) for name in names]
-            defaults = items[3]  # collect default args
+            defaults = items['defaults']  # collect default args
 
             # init arg help and arg description
             ahelp = f"execute {func_name} function"
 
             # collect command description
-            signature = inspect.signature(func_dict[func_name][0])
+            signature = inspect.signature(func_dict[func_name]['func'])
+
+            # collect names and params for a given function
             params = []
             for name, param in signature.parameters.items():
+                
+                # check if function contains annotations
                 if param.annotation != inspect.Parameter.empty:
+                    # if default arg exists display in docs
                     if param.default != inspect.Parameter.empty:
                         params.append(
                             f"{name}: {param.annotation.__name__} = {param.default!r}"
                         )
                     else:
                         params.append(f"{name}: {param.annotation.__name__}")
                 else:
                     if param.default != inspect.Parameter.empty:
                         params.append(f"{name} = {param.default!r}")
                     else:
                         params.append(f"{name}")
+
+            # define return type if exists for docs
             if "return" in types:
-                adesc = f"{func_dict[func_name][0].__name__}({', '.join(params)}) -> {str(types['return'].__name__)}"
+                adesc = f"{func_dict[func_name]['func'].__name__}({', '.join(params)}) -> {str(types['return'].__name__)}"
             else:
-                adesc = f"{func_dict[func_name][0].__name__}({', '.join(params)})"
+                adesc = f"{func_dict[func_name]['func'].__name__}({', '.join(params)})"
 
-            # if docstring assign arg help
-            if items[-1] is not None:
-                ahelp = items[-1]
+            # define help string
+            if items['desc'] is not None:
+                ahelp = items['desc']
 
             # init sub parser
             subp = self.subparsers.add_parser(
                 func_name,
                 help=ahelp,
                 description=adesc,
                 argument_default=argparse.SUPPRESS,
                 add_help=False,
             )
 
+            # create abbreviations for named short name
             abbrevs = set()
             for name, atype in zip(names, arg_types):
+                # if arg is contains a default define a short name
                 if name in defaults:
+                    # default abbreviation is the first 2 characters
                     short_name = name[:2]
+                    # if space is taken define short name as just the list character
                     if short_name in abbrevs:
                         short_name = name[-1]
                     abbrevs.add(short_name)
+
+                    # if there exists a short name with the same first and 
+                    # last chars do not define one
                     try:
                         subp.add_argument(
                             f"-{short_name}",
                             f"--{name}",
                             metavar=str(atype) if atype is not None else None,
                             type=atype,
                             default=defaults[name],
@@ -97,44 +111,70 @@
                             f"--{name}",
                             metavar=str(atype) if atype is not None else None,
                             type=atype,
                             default=defaults[name],
                             help=f"default: {defaults[name]}",
                         )
                 else:
-                    subp.add_argument(
-                        name, type=atype, help=str(atype) if atype is not None else None
-                    )
+                    # if variadic allow any number of args
+                    if items['variadic']:
+                        subp.add_argument(
+                            name, nargs='*', type=atype, help=str(atype) if atype is not None else None
+                        )
+                    else:
+                        subp.add_argument(
+                            name, type=atype, help=str(atype) if atype is not None else None
+                        )
 
             # overide help & place at end of options
             subp.add_argument(
                 "-h", "--help", action="help", help="Show this help message and exit."
             )
 
     def parse(self):
         """initialize parsing args"""
 
         self.input = self.parser.parse_args()
 
         # if command in input namespace
         if self.input.command:
             # retrieve function and arg names for given command
-            func_tup = self.func_dict[self.input.command]
+            func_meta = self.func_dict[self.input.command]
+            args = []
+            kwargs = {}
+
+            # if variadic define args and kwargs
+            if func_meta['variadic']:
+                func = func_meta['func']
+                try:
+                    for arg in vars(self.input)['*args']:
+                        if '=' in arg:
+                            k,v = arg.split('=')
+                            kwargs[k] = v
+                        else:
+                            args.append(arg)
+                except KeyError:
+                    # pass because args & kwargs are already defined empty
+                    pass
+            else:
 
-            # unpack just the args and function
-            func, arg_names = (
-                func_tup[0],
-                func_tup[1],
-            )
-            # collect given args from namespace
-            args = [getattr(self.input, arg) for arg in arg_names]
+                # unpack just the args and function
+                func, arg_names = (
+                    func_meta['func'],
+                    func_meta['names'],
+                )
+            
+                # collect args from input namespace
+                args = [getattr(self.input, arg) for arg in arg_names]
             
             # run function with given args and collect any returns
             if asyncio.iscoroutinefunction(func):
-                returned = asyncio.run(func(*args))
+                returned = asyncio.run(func(*args, **kwargs))
             else:
-                returned = func(*args)
+                returned = func(*args, **kwargs)
 
             # print return if not None
             if returned:
                 print(returned)
-            sys.exit()  # exit the interpreter so the entire script is not run
+
+            # exit the interpreter so the entire script is not run
+            sys.exit()
```

### Comparing `sutools-0.2.2/sutools/log_handler.py` & `sutools-0.2.3/sutools/log_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.2.2/sutools/meta_handler.py` & `sutools-0.2.3/sutools/meta_handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,19 +11,40 @@
 
     def add_func(self, func):
         """registers a function to the function dictionary"""
         names = inspect.getfullargspec(func).args  # collect arg names
         types = inspect.getfullargspec(func).annotations  # collect types of args
         defaults = self._get_defaults(func)
         desc = None
+        variadic = False
 
+        # if docstring exists and no description defined set desc
         if func.__doc__:
             desc = func.__doc__
 
-        self.funcs.update({func.__name__: (func, names, types, defaults, desc)})
+        # collect function signature to check if variadic [args, kwargs]
+        signature = inspect.signature(func)
+        for name, param in signature.parameters.items():
+            param_kind = signature.parameters[name].kind
+            variadic = param_kind in [inspect.Parameter.VAR_POSITIONAL, inspect.Parameter.VAR_KEYWORD]
+            # correct names and types definition
+            if variadic:
+                names.append(str(param))
+                types = {}
+
+        # define function meta info
+        func_meta = {'func':func, 
+                    'names':names, 
+                    'types':types, 
+                    'defaults':defaults, 
+                    'desc':desc, 
+                    'variadic':variadic}
+        
+        # update function in store
+        self.funcs.update({func.__name__: func_meta})
 
     def add_cli(self, cli_obj):
         """adds a cli object to the store"""
         self.cli = cli_obj
 
     def add_log(self, log_obj):
         """adds a logger object to the store"""
```

### Comparing `sutools-0.2.2/sutools.egg-info/PKG-INFO` & `sutools-0.2.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sutools
-Version: 0.2.2
+Version: 0.2.3
 Summary: su (Super User) tools; per module utilities, designed to be lightweight, easy to configure, and reduce boilerplate code.
 Home-page: https://github.com/aastopher/sutools
 Author: Aaron Stopher
 Project-URL: Documentation, https://sutools.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/aastopher/sutools/issues
 Keywords: logs,logger,logging,cli,utils,performance counter,benchmark
 Classifier: Programming Language :: Python :: 3
@@ -140,14 +140,64 @@
     -gr <class 'str'>, --greeting <class 'str'>
                             default: hello
     -fa <class 'str'>, --farewell <class 'str'>
                             default: goodbye
     -h, --help            Show this help message and exit.
 ```
 
+## CLI Using Variadic Functions
+
+Variadic functions are compatible with sutools cli utility. When calling kwargs from the cli; `key=value` should be used instead of `--` and `-`, these are reserved for default arguments.
+
+**NOTE:** since input is from `stdin` it will always be of type `<string>`, sutools will _not_ infer the data type you must infer your needed type within the function.
+
+```python
+"""This module does random stuff."""
+import sutools as su
+
+@su.register
+def variadic(*args, **kwargs):
+    
+    print("Positional arguments:")
+    for arg in args:
+        print(arg)
+
+    print("Keyword arguments:")
+    for key, value in kwargs.items():
+        print(f"{key} = {value}")
+
+    su.logger() # optional
+
+# module level function calls...
+
+if __name__ == '__main__':
+    # main code (will run even when using cli commands)...
+    su.cli(desc = __doc__)
+    # main code (will NOT run when using cli commands)...
+```
+
+**command usage:**
+
+```
+python module.py variadic 1 2 3 foo=1 bar=2
+```
+
+**output:**
+
+```
+Positional arguments:
+1
+2
+3
+Keyword arguments:
+foo = 1
+bar = 2
+```
+
+
 ## Logger Usage Examples
 
 </br>
  
  accessing defined loggers is done with a `log()` helper function. Note the use of `su.log()` in the below functions to access a specified logger before defining the log level and message.
 
 </br>
```

### Comparing `sutools-0.2.2/tests/test_bench_handler.py` & `sutools-0.2.3/tests/test_bench_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.2.2/tests/test_cli_handler.py` & `sutools-0.2.3/tests/test_cli_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -216,7 +216,57 @@
     )
 
     cli_obj.parse()
 
     captured = capsys.readouterr()
 
     assert "pass" in captured.out
+
+def test_variadic_func(capsys, monkeypatch, mock_atexit_register):
+    def func_test(*args, **kwargs):
+        print('pass')
+
+    store = meta_handler.Store()
+    store.add_func(func_test)
+
+    log_obj = log_handler.Logger(
+        "test_logger",
+        list(store.funcs.keys()),
+        logging.INFO,
+        None,
+        None,
+        None,
+        None,
+        None,
+        None,
+        False,
+        logging.Formatter(
+            "%(asctime)s, %(msecs)d %(name)s %(levelname)s %(message)s",
+            datefmt="%H:%M:%S",
+        ),
+        logging.StreamHandler(sys.stdout),
+        stream=True,
+    )
+
+    cli_obj = cli_handler.CLI("description", False, log_obj=log_obj)
+    cli_obj.add_funcs(store.funcs)
+
+    monkeypatch.setattr(sys, "exit", lambda *args: None)
+
+    def run_cli_parse(namespace_dict):
+        namespace = argparse.Namespace(**namespace_dict)
+
+        monkeypatch.setattr(
+            cli_handler.argparse.ArgumentParser, "parse_args", lambda self: namespace
+        )
+
+        cli_obj.parse()
+
+        captured = capsys.readouterr()
+
+        assert "pass" in captured.out
+
+    # test variadic with args
+    run_cli_parse({'command': 'func_test', '*args': ['1', '2', '3', 'foo=1', 'bar=2']})
+
+    # test variadic without args
+    run_cli_parse({'command': 'func_test'})
```

### Comparing `sutools-0.2.2/tests/test_log_handler.py` & `sutools-0.2.3/tests/test_log_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.2.2/tests/test_meta_handler.py` & `sutools-0.2.3/tests/test_meta_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.2.2/tests/test_sutools.py` & `sutools-0.2.3/tests/test_sutools.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,16 +18,15 @@
     monkeypatch.setattr(su.log_handler.atexit, "register", mock_atexit_register)
     return mock_atexit_register
 
 
 ##### Methods
 
 # Test 1: this should test the register decorator from sutools
-# the result should be that the su.store contains a
-# none empty dictionary for the func property
+# the result should be that the su.store contains a dictionary for the functions meta info
 def test_register():
     def _get_defaults(func):
         """helper function to collect default func args"""
 
         # get the signature of the function
         sig = inspect.signature(func)
 
@@ -45,20 +44,71 @@
         return x + y
 
     names = inspect.getfullargspec(func_test).args  # collect arg names
     types = inspect.getfullargspec(func_test).annotations  # collect types of args
     defaults = _get_defaults(func_test)
     desc = func_test.__doc__
 
-    expected_dict = {func_test.__name__: (func_test, names, types, defaults, desc)}
+    expected_dict = {func_test.__name__: {'func':func_test, 
+                                        'names':names, 
+                                        'types':types, 
+                                        'defaults':defaults, 
+                                        'desc':desc, 
+                                        'variadic':False}}
 
     assert expected_dict == su.store.funcs
 
 
-# Test 2: this should test the cli from sutools
+# Test 2: this should test the register decorator from sutools
+# the result should be that the su.store contains a proper function dict for variadic functions
+def test_register_variadic():
+    def _get_meta(func):
+        '''helper function to collect default func args'''
+
+        # get the signature of the function
+        sig = inspect.signature(func)
+
+        # collect a dictionary of default argument values
+        defaults = {}
+        names = []
+        types = {}
+        variadic = False
+        for name, param in sig.parameters.items():
+            param_kind = param.kind
+            variadic = param_kind in [inspect.Parameter.VAR_POSITIONAL, inspect.Parameter.VAR_KEYWORD]
+
+            if param.default is not inspect.Parameter.empty:
+                defaults[name] = param.default
+
+            if variadic:
+                names.append(str(param))
+                types = {}
+
+        desc = func.__doc__
+
+        return names, types, defaults, desc, variadic
+
+    @su.register
+    def func_test(*args, **kwargs):
+        """this is a test function"""
+        return args, kwargs
+
+    names, types, defaults, desc, variadic = _get_meta(func_test)
+
+    expected_dict = {func_test.__name__: {'func':func_test, 
+                                        'names':names, 
+                                        'types':types, 
+                                        'defaults':defaults, 
+                                        'desc':desc, 
+                                        'variadic':variadic}}
+
+    assert expected_dict == su.store.funcs
+
+
+# Test 3: this should test the cli from sutools
 # the result should be that the cli property is not None in su.store
 # the cli object should contain commands for any registered functions
 def test_cli(mock_atexit_register, monkeypatch):
     # patch the input namespace with the desired command
     namespace = argparse.Namespace(command="", help=True)
 
     with patch(
@@ -68,15 +118,15 @@
         monkeypatch.setattr(sys, "exit", lambda *args: None)
 
         su.cli()
 
     assert su.store.cli is not None
 
 
-# Test 3: thisfunc_test should test the logger from sutools
+# Test 4: thisfunc_test should test the logger from sutools
 # the result should be that the log property is no None in su.store
 # the log object should also contain a property loggers with
 # the names of the loggers passed in to loggers property in the logger
 def test_logger(mock_atexit_register, monkeypatch):
     with patch("builtins.open", mock_open()) as mock_file:
         monkeypatch.setattr(su.os, "makedirs", lambda *args, **kwargs: None)
         su.logger(filepath="path")
@@ -117,15 +167,15 @@
             ),
         )
 
     assert su.store.log is not None
     assert all(name in vars(su.store.log.loggers) for name in expected)
 
 
-# Test 4: this should test the log helper function
+# Test 5: this should test the log helper function
 # the should return a namespace of loggers defined
 # in the log object in the su.store
 def test_log(mock_os, mock_atexit_register):
     @su.register
     def func_test():
         pass
 
@@ -137,15 +187,15 @@
         )
     assert "func_test" in vars(su.log()).keys()
 
 
 #### Integration
 
 
-# Test 5: this should test integrations for cli and logger compatibility
+# Test 6: this should test integrations for cli and logger compatibility
 # this should init both a logger and a cli as well as
 # at least one registered test function.
 # the result should be that the log statements in the cli are
 # logged if the cli has logs set to True
 def test_logger_cli(capsys, mock_os, mock_atexit_register, monkeypatch):
     expected_cli = "Test CLI"
     expected_log = "test log"
```

