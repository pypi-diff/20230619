# Comparing `tmp/dargus-1.0.2.tar.gz` & `tmp/dargus-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/dapregi/dev/argus/dist/.tmp-3c59htmw/dargus-1.0.2.tar", last modified: Thu Apr 13 08:44:33 2023, max compression
+gzip compressed data, was "/home/dapregi/dev/argus/dist/.tmp-6fj1dhkr/dargus-1.1.0.tar", last modified: Mon Jun 19 16:05:29 2023, max compression
```

## Comparing `dargus-1.0.2.tar` & `dargus-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-04-13 08:44:33.000000 dargus-1.0.2/
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)    11357 2020-07-29 10:38:30.000000 dargus-1.0.2/LICENSE
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-04-13 08:44:33.000000 dargus-1.0.2/PKG-INFO
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)       73 2023-02-17 13:43:50.000000 dargus-1.0.2/README.md
-drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus/
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)        0 2020-07-29 10:38:30.000000 dargus-1.0.2/dargus/__init__.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13228 2023-04-13 08:40:53.000000 dargus-1.0.2/dargus/argus.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1940 2023-04-11 13:10:00.000000 dargus-1.0.2/dargus/argus_cli.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     2350 2023-04-13 08:40:53.000000 dargus-1.0.2/dargus/argus_config.py
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)       43 2020-07-29 10:38:30.000000 dargus-1.0.2/dargus/argus_exceptions.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      928 2023-02-06 09:28:40.000000 dargus-1.0.2/dargus/commons.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1567 2023-02-06 09:22:09.000000 dargus-1.0.2/dargus/utils.py
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)      889 2020-07-29 10:38:30.000000 dargus-1.0.2/dargus/validation_result.py
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)     7118 2023-02-21 14:33:18.000000 dargus-1.0.2/dargus/validator.py
-drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus.egg-info/
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus.egg-info/PKG-INFO
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      410 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus.egg-info/SOURCES.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        1 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus.egg-info/dependency_links.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       49 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus.egg-info/entry_points.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       29 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus.egg-info/requires.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        7 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus.egg-info/top_level.txt
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)     1042 2023-04-13 08:43:59.000000 dargus-1.0.2/pyproject.toml
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       38 2023-04-13 08:44:33.000000 dargus-1.0.2/setup.cfg
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)       92 2023-02-17 14:07:57.000000 dargus-1.0.2/setup.py
+drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-06-19 16:05:29.000000 dargus-1.1.0/
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)    11357 2020-07-29 10:38:30.000000 dargus-1.1.0/LICENSE
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-06-19 16:05:29.000000 dargus-1.1.0/PKG-INFO
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       73 2023-06-01 15:53:34.000000 dargus-1.1.0/README.md
+drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus/
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        0 2023-06-01 15:53:34.000000 dargus-1.1.0/dargus/__init__.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13373 2023-06-19 16:04:17.000000 dargus-1.1.0/dargus/argus.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1940 2023-06-01 15:53:34.000000 dargus-1.1.0/dargus/argus_cli.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     2350 2023-06-01 15:53:34.000000 dargus-1.1.0/dargus/argus_config.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       43 2023-06-01 15:53:34.000000 dargus-1.1.0/dargus/argus_exceptions.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      928 2023-06-01 15:53:34.000000 dargus-1.1.0/dargus/commons.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1577 2023-06-19 16:04:17.000000 dargus-1.1.0/dargus/utils.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      889 2023-06-01 15:53:34.000000 dargus-1.1.0/dargus/validation_result.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     7180 2023-06-19 16:04:17.000000 dargus-1.1.0/dargus/validator.py
+drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus.egg-info/
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus.egg-info/PKG-INFO
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      410 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus.egg-info/SOURCES.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        1 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus.egg-info/dependency_links.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       49 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus.egg-info/entry_points.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       29 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus.egg-info/requires.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        7 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus.egg-info/top_level.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1042 2023-06-19 16:04:17.000000 dargus-1.1.0/pyproject.toml
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       38 2023-06-19 16:05:29.000000 dargus-1.1.0/setup.cfg
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       92 2023-06-01 15:53:34.000000 dargus-1.1.0/setup.py
```

### Comparing `dargus-1.0.2/LICENSE` & `dargus-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dargus-1.0.2/PKG-INFO` & `dargus-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargus
-Version: 1.0.2
+Version: 1.1.0
 Summary: A Python engine for testing and benchmarking REST web services
 Author-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 Maintainer-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `dargus-1.0.2/dargus/argus.py` & `dargus-1.1.0/dargus/argus.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 import json
 from itertools import product
 from datetime import datetime
 
 from dargus.validator import Validator
 from dargus.validation_result import ValidationResult
-from dargus.utils import get_item, create_url
+from dargus.utils import get_item_from_json, create_url
 from dargus.commons import query
 
 
 class _Suite:
     def __init__(self, id_, base_url=None, tests=None):
         self.id_ = id_
         self.base_url = base_url
@@ -90,31 +90,31 @@
             val_name = val_fname[:-3] if val_fname.endswith('.py') else val_fname
             cls_name = ''.join(x.title() for x in val_name.split('_'))
             spec = importlib.util.spec_from_file_location(cls_name, val_path)
             foo = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(foo)
             validator_class = getattr(foo, cls_name)
             self.validator = validator_class(
-                validation=self.config.get('validation')
+                config=self.config, token=self.token
             )
         else:
             self.validator = Validator(
-                validation=self.config.get('validation')
+                config=self.config, token=self.token
             )
 
     def _generate_headers(self):
         if 'rest' in self.config and self.config['rest'] is not None and self.config['rest']['headers']:
             self.headers = self.config['rest']['headers']
 
     @staticmethod
     def _login(auth, field):
         url = create_url(auth['url'], auth.get('pathParams'),
                          auth.get('queryParams'))
         response = query(url, method=auth.get('method'), headers=auth.get('headers'), body=auth.get('body'))
-        return get_item(response.json(), field)
+        return get_item_from_json(response.json(), field)
 
     def _generate_token(self):
         if 'authentication' in self.config and self.config['authentication'] is not None:
             auth = self.config['authentication']
             token_func = re.findall(r'^(.+)\((.+)\)$', auth['token'])
             if token_func:
                 if token_func[0][0] == 'env':
@@ -147,14 +147,17 @@
         self.suite_ids.append(id_)
 
         # Filtering suites to run
         if 'suites' in self.config and self.config['suites'] is not None:
             if id_ not in self.config['suites']:
                 return None
 
+        # Getting base URL
+        if suite.get('baseUrl') is None and 'baseUrl' in self.config:
+            suite['baseUrl'] = self.config['baseUrl']
         base_url = suite.get('baseUrl')
 
         tests = list(filter(
             None, [self._parse_test(test) for test in suite.get('tests')]
         ))
 
         suite = _Suite(id_=id_, base_url=base_url, tests=tests)
@@ -319,15 +322,15 @@
             for test in suite.tests:
                 self.current.tests = [test]
                 for task in test.tasks:
                     self.current.tests[0].tasks = [task]
                     self.query_task()
                     if not self.current.tests[0].async_:
                         res = self.validator.validate(
-                            self.response, self.current.tests[0].tasks[0]
+                            self.response, self.current
                         )
                         vr = ValidationResult(
                             current=self.current,
                             url=self.url,
                             response=self.response,
                             validation=res,
                             headers=self.headers,
```

### Comparing `dargus-1.0.2/dargus/argus_cli.py` & `dargus-1.1.0/dargus/argus_cli.py`

 * *Files identical despite different names*

### Comparing `dargus-1.0.2/dargus/argus_config.py` & `dargus-1.1.0/dargus/argus_config.py`

 * *Files identical despite different names*

### Comparing `dargus-1.0.2/dargus/commons.py` & `dargus-1.1.0/dargus/commons.py`

 * *Files identical despite different names*

### Comparing `dargus-1.0.2/dargus/utils.py` & `dargus-1.1.0/dargus/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import requests
 
 
-def get_item(json_dict, field):
+def get_item_from_json(json_dict, field):
     for item in field.split('.'):
         items = list(filter(None, re.split(r'[\[\]]', item)))
         key, indexes = items[0], map(int, items[1:])
         json_dict = json_dict[key]
         if indexes:
             for i in indexes:
                 json_dict = json_dict[i]
```

### Comparing `dargus-1.0.2/dargus/validation_result.py` & `dargus-1.1.0/dargus/validation_result.py`

 * *Files identical despite different names*

### Comparing `dargus-1.0.2/dargus/validator.py` & `dargus-1.1.0/dargus/validator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,86 +1,69 @@
 import re
 
-from dargus.utils import get_item, dot2python, num_compare
+from dargus.utils import get_item_from_json, dot2python, num_compare
 from dargus.argus_exceptions import ValidationError
 
 
 class Validator:
-    def __init__(self, validation=None):
-        self.validation = self.get_default_validation()
-        if validation is not None:
-            self.validation.update(validation)
-
+    def __init__(self, config, token=None):
+        self._config = config
         self._rest_response = None
         self._rest_response_json = None
+        self._current = None
         self._task = None
-        self._async_jobs = []
+        self._stored_values = {}
+        self._token = token
+
+        self.validation = self.get_default_validation()
+        if self._config.get('validation') is not None:
+            self.validation.update(config.get('validation'))
 
     @staticmethod
     def get_default_validation():
         validation = {
             'timeDeviation': 100,
             'asyncRetryTime': 10,
             'ignore_time': False,
             'ignore_headers': [],
             'ignore_results': [],
             'fail_on_first': False
         }
         return validation
 
-    @property
-    def rest_response(self):
-        return self._rest_response
-
-    @rest_response.setter
-    def rest_response(self, rest_response):
-        self._rest_response = rest_response
-        self._rest_response_json = rest_response.json()
-
-    @property
-    def async_jobs(self):
-        return self._async_jobs
-
-    @async_jobs.setter
-    def async_jobs(self, async_jobs):
-        self._async_jobs = async_jobs
-
-    @property
-    def task(self):
-        return self._task
-
-    @task.setter
-    def task(self, task):
-        self._task = task
-
     def get_item(self, field):
-        field_value = get_item(self._rest_response_json, field)
+        if field.startswith('<'):
+            variable_name = field.split('.')[0].lstrip('<').rstrip('>')
+            field = '.'.join(field.split('.')[1:])
+            field_value = get_item_from_json(self._stored_values[variable_name], field)
+        else:
+            field_value = get_item_from_json(self._rest_response_json, field)
         return field_value
 
     def compare(self, field, value, operator='eq'):
-        field_value = get_item(self._rest_response_json, field)
+        field_value = self.get_item(field)
         return num_compare(field_value, value, operator)
 
     def match(self, field, regex):
-        field_value = get_item(self._rest_response_json, field)
+        field_value = self.get_item(field)
         return any(re.findall(regex, field_value))
 
     def empty(self, field):
         try:
-            field_value = get_item(self._rest_response_json, field)
+            field_value = self.get_item(field)
         except (TypeError, KeyError, IndexError):
             return False
         return not field_value
 
     def list_length(self, field, value, operator='eq'):
-        field_value = get_item(self._rest_response_json, field)
+        field_value = self.get_item(field)
         return num_compare(len(field_value), value, operator)
 
     def list_contains(self, field, value, expected=True):
-        field_value = get_item(self._rest_response_json, field)
+        field_value = self.get_item(field)
         if expected:
             return value in field_value
         else:
             return value not in field_value
 
     @staticmethod
     def _to_python_lambda(value):
@@ -94,42 +77,47 @@
         # Internal variables (e.g. "$QUERY_PARAMS")
         value = value.replace('$QUERY_PARAMS', 'self.task.query_params')
 
         value = 'lambda ' + value.replace('->', ':')
         return value
 
     def list_apply(self, field, value, all_=False):
-        field_value = get_item(self._rest_response_json, field)
+        field_value = self.get_item(field)
         lambda_function = self._to_python_lambda(value)
         res = [eval(lambda_function, {'self': self})(i) for i in field_value]
         if all_:
             return all(res)
         else:
             return any(res)
 
     def list_equals(self, field, value, is_sorted=True):
-        field_value = get_item(self._rest_response_json, field)
+        field_value = self.get_item(field)
         if len(field) != len(value):
             return False
         if is_sorted:
             return field_value == value
         else:
             return sorted(field_value) == sorted(value)
 
     def list_sorted(self, field, reverse=False):
-        field_value = get_item(self._rest_response_json, field)
+        field_value = self.get_item(field)
         return field_value == sorted(field_value, reverse=reverse)
 
     def dict_equals(self, field, value):
-        field_value = get_item(self._rest_response_json, field)
+        field_value = self.get_item(field)
         if len(field) != len(value):
             return False
         else:
             return field_value == value
 
+    def store(self, field, variable_name):
+        field_value = self.get_item(field)
+        self._stored_values[variable_name] = field_value
+        return True
+
     def _is_defined(self, method_name):
         return method_name in dir(self)
 
     def _validate_results(self, methods, exclude=None):
         results = []
         for method in methods:
             method_parts = re.search(r'^(.+?)\((.*)\)$', method)
@@ -147,72 +135,78 @@
 
             # Raise error if fail_on_first is True
             if self.validation['fail_on_first'] and not result:
                 msg = 'Validation function "{}" returned False'
                 raise ValidationError(msg.format(method))
 
             results.append({'function': method, 'result': result})
+
+        # Empty stored values
+        self._stored_values = {}
+
         return results
 
     def validate_time(self, task_time):
         request_time = self._rest_response.elapsed.total_seconds()
         time_deviation = self.validation['timeDeviation']
         max_time = task_time + task_time*time_deviation/100
         min_time = task_time - task_time*time_deviation/100
         if not min_time < request_time < max_time:
             return False
         return True
 
     def validate_headers(self, task_headers, exclude=None):
         for key in task_headers.keys():
             if key not in exclude and (
-                    key not in self.rest_response.headers.keys() or
-                    self.rest_response.headers[key] != task_headers[key]
+                    key not in self._rest_response.headers.keys() or
+                    self._rest_response.headers[key] != task_headers[key]
             ):
                 return False
         return True
 
     def validate_status_code(self, task_status_code):
-        if not task_status_code == self.rest_response.status_code:
+        if not task_status_code == self._rest_response.status_code:
             return False
         return True
 
-    def validate(self, response, task):
-        self.rest_response = response
-        self.task = task
+    def validate(self, response, current):
+        self._rest_response = response
+        self._rest_response_json = response.json()
+        self._current = current
+        self._task = self._current.tests[0].tasks[0]
         results = []
 
         # Time
-        if 'time' in task.validation and not self.validation['ignore_time']:
+        if 'time' in self._task.validation and not self.validation['ignore_time']:
             results.append(
                 {'function': 'validate_time',
-                 'result': self.validate_time(task.validation['time'])}
+                 'result': self.validate_time(self._task.validation['time'])}
             )
 
         # Headers
-        if 'headers' in task.validation:
+        if 'headers' in self._task.validation:
             result_headers = self.validate_headers(
-                task.validation['headers'],
+                self._task.validation['headers'],
                 exclude=self.validation['ignore_headers']
             )
             results.append({'function': 'validate_headers',
                             'result': result_headers})
 
         # Status code
-        task_status_code = task.validation.get('status_code') \
-            if 'status_code' in task.validation else 200
+        task_status_code = self._task.validation.get('status_code') \
+            if 'status_code' in self._task.validation else 200
         results.append(
             {'function': 'validate_status_code',
              'result': self.validate_status_code(task_status_code)}
         )
 
         # Results
-        if 'results' in task.validation:
+        if 'results' in self._task.validation:
             results += self._validate_results(
-                task.validation['results'],
+                self._task.validation['results'],
                 exclude=self.validation['ignore_results']
             )
 
         return results
 
     def validate_async(self, async_jobs):
         pass
```

### Comparing `dargus-1.0.2/dargus.egg-info/PKG-INFO` & `dargus-1.1.0/dargus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargus
-Version: 1.0.2
+Version: 1.1.0
 Summary: A Python engine for testing and benchmarking REST web services
 Author-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 Maintainer-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `dargus-1.0.2/pyproject.toml` & `dargus-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["dargus"]
 
 [project]
 name = "dargus"
-version = "1.0.2"
+version = "1.1.0"
 description = "A Python engine for testing and benchmarking REST web services"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 authors = [
   {name="Daniel Perez-Gil", email="daniel.perez@zettagenomics.com"}
 ]
```

