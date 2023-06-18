# Comparing `tmp/vanoma_api_utils-0.97.0.tar.gz` & `tmp/vanoma_api_utils-0.98.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanoma_api_utils-0.97.0.tar", max compression
+gzip compressed data, was "vanoma_api_utils-0.98.0.tar", max compression
```

## Comparing `vanoma_api_utils-0.97.0.tar` & `vanoma_api_utils-0.98.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      785 2023-05-20 07:52:34.467544 vanoma_api_utils-0.97.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-11-20 15:41:36.379982 vanoma_api_utils-0.97.0/vanoma_api_utils/__init__.py
--rw-r--r--   0        0        0     1042 2023-05-05 23:43:21.324482 vanoma_api_utils-0.97.0/vanoma_api_utils/auth_api.py
--rw-r--r--   0        0        0     1871 2023-05-19 12:29:43.606502 vanoma_api_utils-0.97.0/vanoma_api_utils/communication_api.py
--rw-r--r--   0        0        0      256 2021-12-21 21:17:43.572975 vanoma_api_utils-0.97.0/vanoma_api_utils/constants.py
--rw-r--r--   0        0        0        0 2021-11-23 16:02:21.945089 vanoma_api_utils-0.97.0/vanoma_api_utils/django/__init__.py
--rw-r--r--   0        0        0     2847 2023-01-09 12:46:03.473102 vanoma_api_utils-0.97.0/vanoma_api_utils/django/fields.py
--rw-r--r--   0        0        0      511 2023-01-10 10:59:21.300355 vanoma_api_utils-0.97.0/vanoma_api_utils/django/functions.py
--rw-r--r--   0        0        0     1328 2022-12-28 22:45:38.576188 vanoma_api_utils-0.97.0/vanoma_api_utils/django/middlewares.py
--rw-r--r--   0        0        0      648 2023-05-10 22:06:02.068641 vanoma_api_utils-0.97.0/vanoma_api_utils/django/request.py
--rw-r--r--   0        0        0     3087 2023-05-20 07:52:27.593007 vanoma_api_utils-0.97.0/vanoma_api_utils/django/settings.py
--rw-r--r--   0        0        0     1138 2023-03-03 14:56:46.353080 vanoma_api_utils-0.97.0/vanoma_api_utils/django/tests.py
--rw-r--r--   0        0        0      564 2021-11-29 19:45:24.704407 vanoma_api_utils-0.97.0/vanoma_api_utils/django/validators.py
--rw-r--r--   0        0        0      359 2021-11-29 17:39:47.918553 vanoma_api_utils-0.97.0/vanoma_api_utils/django/views.py
--rw-r--r--   0        0        0      460 2022-11-12 13:53:13.472533 vanoma_api_utils-0.97.0/vanoma_api_utils/exceptions.py
--rw-r--r--   0        0        0     2149 2023-05-10 23:46:49.793790 vanoma_api_utils-0.97.0/vanoma_api_utils/http.py
--rw-r--r--   0        0        0      731 2022-09-29 11:16:04.699469 vanoma_api_utils-0.97.0/vanoma_api_utils/jwt.py
--rw-r--r--   0        0        0      334 2023-05-06 12:11:25.362324 vanoma_api_utils-0.97.0/vanoma_api_utils/mini_huey/__init__.py
--rw-r--r--   0        0        0      302 2023-05-06 12:03:55.443246 vanoma_api_utils-0.97.0/vanoma_api_utils/mini_huey/apps.py
--rw-r--r--   0        0        0      745 2023-03-03 10:18:23.340558 vanoma_api_utils-0.97.0/vanoma_api_utils/misc.py
--rw-r--r--   0        0        0      719 2023-05-10 19:49:19.660911 vanoma_api_utils-0.97.0/vanoma_api_utils/phone_numbers.py
--rw-r--r--   0        0        0        0 2021-11-21 15:05:33.075892 vanoma_api_utils-0.97.0/vanoma_api_utils/py.typed
--rw-r--r--   0        0        0      165 2023-05-06 01:16:45.565915 vanoma_api_utils-0.97.0/vanoma_api_utils/request.py
--rw-r--r--   0        0        0        0 2021-11-23 15:40:52.590038 vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/__init__.py
--rw-r--r--   0        0        0      480 2022-11-12 13:23:20.002099 vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/exceptions.py
--rw-r--r--   0        0        0      142 2022-05-30 10:26:27.381278 vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/filters.py
--rw-r--r--   0        0        0     1144 2022-10-10 09:49:31.420992 vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/generics.py
--rw-r--r--   0        0        0     1424 2023-05-01 23:39:19.933610 vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/pagination.py
--rw-r--r--   0        0        0      547 2023-05-05 23:10:22.453470 vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/parsers.py
--rw-r--r--   0        0        0      853 2023-05-05 23:57:44.470179 vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/renderers.py
--rw-r--r--   0        0        0      291 2022-10-18 18:19:28.688546 vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/responses.py
--rw-r--r--   0        0        0     6379 2023-01-17 11:33:02.221744 vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/serializers.py
--rw-r--r--   0        0        0      215 2022-10-18 18:19:00.551261 vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/tests.py
--rw-r--r--   0        0        0     3168 2023-01-08 23:09:08.723575 vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/views.py
--rw-r--r--   0        0        0      314 2021-11-24 10:01:52.245853 vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/viewsets.py
--rw-r--r--   0        0        0      338 2021-11-28 15:16:26.130594 vanoma_api_utils-0.97.0/vanoma_api_utils/sentry.py
--rw-r--r--   0        0        0      612 2023-05-06 12:07:34.271756 vanoma_api_utils-0.97.0/vanoma_api_utils/tests.py
--rw-r--r--   0        0        0     1238 1970-01-01 00:00:00.000000 vanoma_api_utils-0.97.0/setup.py
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 vanoma_api_utils-0.97.0/PKG-INFO
+-rw-r--r--   0        0        0      812 2023-06-18 22:14:20.954499 vanoma_api_utils-0.98.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-11-20 15:41:36.379982 vanoma_api_utils-0.98.0/vanoma_api_utils/__init__.py
+-rw-r--r--   0        0        0     1042 2023-05-05 23:43:21.324482 vanoma_api_utils-0.98.0/vanoma_api_utils/auth_api.py
+-rw-r--r--   0        0        0     1871 2023-05-19 12:29:43.606502 vanoma_api_utils-0.98.0/vanoma_api_utils/communication_api.py
+-rw-r--r--   0        0        0      256 2021-12-21 21:17:43.572975 vanoma_api_utils-0.98.0/vanoma_api_utils/constants.py
+-rw-r--r--   0        0        0        0 2021-11-23 16:02:21.945089 vanoma_api_utils-0.98.0/vanoma_api_utils/django/__init__.py
+-rw-r--r--   0        0        0     2847 2023-01-09 12:46:03.473102 vanoma_api_utils-0.98.0/vanoma_api_utils/django/fields.py
+-rw-r--r--   0        0        0      511 2023-01-10 10:59:21.300355 vanoma_api_utils-0.98.0/vanoma_api_utils/django/functions.py
+-rw-r--r--   0        0        0     1328 2022-12-28 22:45:38.576188 vanoma_api_utils-0.98.0/vanoma_api_utils/django/middlewares.py
+-rw-r--r--   0        0        0      648 2023-05-10 22:06:02.068641 vanoma_api_utils-0.98.0/vanoma_api_utils/django/request.py
+-rw-r--r--   0        0        0     3177 2023-06-18 22:08:24.144734 vanoma_api_utils-0.98.0/vanoma_api_utils/django/settings.py
+-rw-r--r--   0        0        0     1138 2023-03-03 14:56:46.353080 vanoma_api_utils-0.98.0/vanoma_api_utils/django/tests.py
+-rw-r--r--   0        0        0      564 2021-11-29 19:45:24.704407 vanoma_api_utils-0.98.0/vanoma_api_utils/django/validators.py
+-rw-r--r--   0        0        0      359 2021-11-29 17:39:47.918553 vanoma_api_utils-0.98.0/vanoma_api_utils/django/views.py
+-rw-r--r--   0        0        0      460 2022-11-12 13:53:13.472533 vanoma_api_utils-0.98.0/vanoma_api_utils/exceptions.py
+-rw-r--r--   0        0        0     2149 2023-05-10 23:46:49.793790 vanoma_api_utils-0.98.0/vanoma_api_utils/http.py
+-rw-r--r--   0        0        0      731 2022-09-29 11:16:04.699469 vanoma_api_utils-0.98.0/vanoma_api_utils/jwt.py
+-rw-r--r--   0        0        0      334 2023-05-06 12:11:25.362324 vanoma_api_utils-0.98.0/vanoma_api_utils/mini_huey/__init__.py
+-rw-r--r--   0        0        0      302 2023-05-06 12:03:55.443246 vanoma_api_utils-0.98.0/vanoma_api_utils/mini_huey/apps.py
+-rw-r--r--   0        0        0      745 2023-03-03 10:18:23.340558 vanoma_api_utils-0.98.0/vanoma_api_utils/misc.py
+-rw-r--r--   0        0        0      719 2023-05-10 19:49:19.660911 vanoma_api_utils-0.98.0/vanoma_api_utils/phone_numbers.py
+-rw-r--r--   0        0        0        0 2021-11-21 15:05:33.075892 vanoma_api_utils-0.98.0/vanoma_api_utils/py.typed
+-rw-r--r--   0        0        0      165 2023-05-06 01:16:45.565915 vanoma_api_utils-0.98.0/vanoma_api_utils/request.py
+-rw-r--r--   0        0        0        0 2021-11-23 15:40:52.590038 vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/__init__.py
+-rw-r--r--   0        0        0      480 2022-11-12 13:23:20.002099 vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/exceptions.py
+-rw-r--r--   0        0        0      142 2022-05-30 10:26:27.381278 vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/filters.py
+-rw-r--r--   0        0        0     1144 2022-10-10 09:49:31.420992 vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/generics.py
+-rw-r--r--   0        0        0     1424 2023-05-01 23:39:19.933610 vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/pagination.py
+-rw-r--r--   0        0        0      547 2023-05-05 23:10:22.453470 vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/parsers.py
+-rw-r--r--   0        0        0      853 2023-05-05 23:57:44.470179 vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/renderers.py
+-rw-r--r--   0        0        0      291 2022-10-18 18:19:28.688546 vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/responses.py
+-rw-r--r--   0        0        0     2535 2023-06-18 22:14:00.287477 vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/serializers.py
+-rw-r--r--   0        0        0      215 2022-10-18 18:19:00.551261 vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/tests.py
+-rw-r--r--   0        0        0     3168 2023-01-08 23:09:08.723575 vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/views.py
+-rw-r--r--   0        0        0      314 2021-11-24 10:01:52.245853 vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/viewsets.py
+-rw-r--r--   0        0        0      338 2021-11-28 15:16:26.130594 vanoma_api_utils-0.98.0/vanoma_api_utils/sentry.py
+-rw-r--r--   0        0        0      612 2023-05-06 12:07:34.271756 vanoma_api_utils-0.98.0/vanoma_api_utils/tests.py
+-rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 vanoma_api_utils-0.98.0/setup.py
+-rw-r--r--   0        0        0     1262 1970-01-01 00:00:00.000000 vanoma_api_utils-0.98.0/PKG-INFO
```

### Comparing `vanoma_api_utils-0.97.0/pyproject.toml` & `vanoma_api_utils-0.98.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vanoma-api-utils"
-version = "0.97.0"
+version = "0.98.0"
 description = "Python utils for vanoma APIs"
 authors = ["Vanoma <contact@vanoma.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 django = "^4.2"
 djangorestframework = "^3.14.0"
@@ -20,14 +20,15 @@
 Faker = "^9.9.1"
 psycopg2 = "^2.9.3"
 django-storages = "^1.13.1"
 boto3 = "^1.24.89"
 shortuuid = "^1.0.9"
 babel = "^2.12.1"
 huey = "^2.4.5"
+drf-flex-fields = "^1.0.2"
 
 [tool.poetry.dev-dependencies]
 black = "^22.8.0"
 pre-commit = "^2.15.0"
 pytest = "6.2.5"
 
 [build-system]
```

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/auth_api.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/auth_api.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/communication_api.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/communication_api.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/django/fields.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/django/fields.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/django/middlewares.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/django/middlewares.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/django/request.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/django/request.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/django/settings.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/django/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def resolve_logging() -> Dict[str, Any]:
     if resolve_environment() == "testing":
         return {
             "version": 1,
             "root": {
-                "level": "CRITICAL", # Use a higher-level to disable logs in tests. Can't find a way to easily disable the root logger.
+                "level": "CRITICAL",  # Use a higher-level to disable logs in tests. Can't find a way to easily disable the root logger.
             },
         }
 
     return {
         "version": 1,
         "disable_existing_loggers": False,
         "formatters": {
@@ -95,7 +95,12 @@
         "djangorestframework_camel_case.parser.CamelCaseJSONParser",
     ),
     "TEST_REQUEST_DEFAULT_FORMAT": "json",
     "EXCEPTION_HANDLER": "vanoma_api_utils.rest_framework.views.exception_handler",
     "DEFAULT_VERSIONING_CLASS": "rest_framework.versioning.NamespaceVersioning",
     "DEFAULT_PAGINATION_CLASS": "vanoma_api_utils.rest_framework.pagination.PageNumberPagination",
 }
+
+BASE_REST_FLEX_FIELDS = {
+    "EXPAND_PARAM": "include",
+    "OMIT_PARAM": "exclude",
+}
```

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/django/tests.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/django/tests.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/django/validators.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/django/validators.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/http.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/http.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/jwt.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/jwt.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/misc.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/misc.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/phone_numbers.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/phone_numbers.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/generics.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/generics.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/pagination.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/pagination.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/parsers.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/parsers.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/renderers.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/renderers.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/rest_framework/views.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/rest_framework/views.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/vanoma_api_utils/tests.py` & `vanoma_api_utils-0.98.0/vanoma_api_utils/tests.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.97.0/setup.py` & `vanoma_api_utils-0.98.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,26 +17,27 @@
  'boto3>=1.24.89,<2.0.0',
  'dj-database-url>=0.5.0,<0.6.0',
  'django-filter>=21.1,<22.0',
  'django-storages>=1.13.1,<2.0.0',
  'django>=4.2,<5.0',
  'djangorestframework-camel-case>=1.2.0,<2.0.0',
  'djangorestframework>=3.14.0,<4.0.0',
+ 'drf-flex-fields>=1.0.2,<2.0.0',
  'huey>=2.4.5,<3.0.0',
  'phonenumbers>=8.12.37,<9.0.0',
  'psycopg2>=2.9.3,<3.0.0',
  'pyhumps>=3.5.3,<4.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'requests>=2.27.1,<3.0.0',
  'sentry-sdk>=1.12.1,<2.0.0',
  'shortuuid>=1.0.9,<2.0.0']
 
 setup_kwargs = {
     'name': 'vanoma-api-utils',
-    'version': '0.97.0',
+    'version': '0.98.0',
     'description': 'Python utils for vanoma APIs',
     'long_description': 'None',
     'author': 'Vanoma',
     'author_email': 'contact@vanoma.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `vanoma_api_utils-0.97.0/PKG-INFO` & `vanoma_api_utils-0.98.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanoma-api-utils
-Version: 0.97.0
+Version: 0.98.0
 Summary: Python utils for vanoma APIs
 Author: Vanoma
 Author-email: contact@vanoma.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,14 +16,15 @@
 Requires-Dist: boto3 (>=1.24.89,<2.0.0)
 Requires-Dist: dj-database-url (>=0.5.0,<0.6.0)
 Requires-Dist: django (>=4.2,<5.0)
 Requires-Dist: django-filter (>=21.1,<22.0)
 Requires-Dist: django-storages (>=1.13.1,<2.0.0)
 Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
 Requires-Dist: djangorestframework-camel-case (>=1.2.0,<2.0.0)
+Requires-Dist: drf-flex-fields (>=1.0.2,<2.0.0)
 Requires-Dist: huey (>=2.4.5,<3.0.0)
 Requires-Dist: phonenumbers (>=8.12.37,<9.0.0)
 Requires-Dist: psycopg2 (>=2.9.3,<3.0.0)
 Requires-Dist: pyhumps (>=3.5.3,<4.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: sentry-sdk (>=1.12.1,<2.0.0)
```

