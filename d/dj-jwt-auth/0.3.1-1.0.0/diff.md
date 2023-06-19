# Comparing `tmp/dj-jwt-auth-0.3.1.tar.gz` & `tmp/dj-jwt-auth-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-jwt-auth-0.3.1.tar", last modified: Thu May 25 14:31:59 2023, max compression
+gzip compressed data, was "dj-jwt-auth-1.0.0.tar", last modified: Mon Jun 19 09:03:45 2023, max compression
```

## Comparing `dj-jwt-auth-0.3.1.tar` & `dj-jwt-auth-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2023-05-25 14:31:59.669137 dj-jwt-auth-0.3.1/
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     2385 2023-05-25 14:31:59.669339 dj-jwt-auth-0.3.1/PKG-INFO
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     1444 2023-05-25 14:31:29.000000 dj-jwt-auth-0.3.1/README.md
-drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2023-05-25 14:31:59.661285 dj-jwt-auth-0.3.1/dj_jwt_auth.egg-info/
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     2385 2023-05-25 14:31:59.000000 dj-jwt-auth-0.3.1/dj_jwt_auth.egg-info/PKG-INFO
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      418 2023-05-25 14:31:59.000000 dj-jwt-auth-0.3.1/dj_jwt_auth.egg-info/SOURCES.txt
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        1 2023-05-25 14:31:59.000000 dj-jwt-auth-0.3.1/dj_jwt_auth.egg-info/dependency_links.txt
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)       63 2023-05-25 14:31:59.000000 dj-jwt-auth-0.3.1/dj_jwt_auth.egg-info/requires.txt
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)       17 2023-05-25 14:31:59.000000 dj-jwt-auth-0.3.1/dj_jwt_auth.egg-info/top_level.txt
-drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2023-05-25 14:31:59.665417 dj-jwt-auth-0.3.1/django_jwt/
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2022-10-13 11:25:09.000000 dj-jwt-auth-0.3.1/django_jwt/__init__.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     1111 2022-11-21 13:54:58.000000 dj-jwt-auth-0.3.1/django_jwt/jwt.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     1022 2022-10-27 12:06:32.000000 dj-jwt-auth-0.3.1/django_jwt/middleware.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      778 2022-10-14 14:12:54.000000 dj-jwt-auth-0.3.1/django_jwt/settings.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     1967 2022-10-24 09:36:32.000000 dj-jwt-auth-0.3.1/django_jwt/user.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      200 2022-12-07 14:39:32.000000 dj-jwt-auth-0.3.1/django_jwt/views.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      221 2022-10-24 09:36:12.000000 dj-jwt-auth-0.3.1/pyproject.toml
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      991 2023-05-25 14:31:59.670183 dj-jwt-auth-0.3.1/setup.cfg
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)       90 2022-10-24 09:36:32.000000 dj-jwt-auth-0.3.1/setup.py
-drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2023-05-25 14:31:59.668393 dj-jwt-auth-0.3.1/tests/
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2022-10-13 13:02:24.000000 dj-jwt-auth-0.3.1/tests/__init__.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      190 2022-10-14 08:57:49.000000 dj-jwt-auth-0.3.1/tests/models.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     3974 2022-10-24 09:36:56.000000 dj-jwt-auth-0.3.1/tests/test_middleware.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      212 2022-10-14 10:04:40.000000 dj-jwt-auth-0.3.1/tests/urls.py
+drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-06-19 09:03:45.184073 dj-jwt-auth-1.0.0/
+-rw-r--r--   0 seleznevk (984925890) 1002642239     2720 2023-06-19 09:03:45.184255 dj-jwt-auth-1.0.0/PKG-INFO
+-rw-r--r--   0 seleznevk (984925890) 1002642239     1779 2023-06-16 14:04:30.000000 dj-jwt-auth-1.0.0/README.md
+drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-06-19 09:03:45.175979 dj-jwt-auth-1.0.0/dj_jwt_auth.egg-info/
+-rw-r--r--   0 seleznevk (984925890) 1002642239     2720 2023-06-19 09:03:45.000000 dj-jwt-auth-1.0.0/dj_jwt_auth.egg-info/PKG-INFO
+-rw-r--r--   0 seleznevk (984925890) 1002642239      409 2023-06-19 09:03:45.000000 dj-jwt-auth-1.0.0/dj_jwt_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 seleznevk (984925890) 1002642239        1 2023-06-19 09:03:45.000000 dj-jwt-auth-1.0.0/dj_jwt_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 seleznevk (984925890) 1002642239       63 2023-06-19 09:03:45.000000 dj-jwt-auth-1.0.0/dj_jwt_auth.egg-info/requires.txt
+-rw-r--r--   0 seleznevk (984925890) 1002642239       17 2023-06-19 09:03:45.000000 dj-jwt-auth-1.0.0/dj_jwt_auth.egg-info/top_level.txt
+drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-06-19 09:03:45.180122 dj-jwt-auth-1.0.0/django_jwt/
+-rw-r--r--   0 seleznevk (984925890) 1002642239        0 2022-10-13 11:25:09.000000 dj-jwt-auth-1.0.0/django_jwt/__init__.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239     1092 2023-06-19 08:56:53.000000 dj-jwt-auth-1.0.0/django_jwt/middleware.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239      981 2023-06-16 14:04:30.000000 dj-jwt-auth-1.0.0/django_jwt/settings.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239     3064 2023-06-19 08:56:53.000000 dj-jwt-auth-1.0.0/django_jwt/user.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239     1482 2023-06-19 08:56:53.000000 dj-jwt-auth-1.0.0/django_jwt/utils.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239      200 2022-12-07 14:39:32.000000 dj-jwt-auth-1.0.0/django_jwt/views.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239      221 2022-10-24 09:36:12.000000 dj-jwt-auth-1.0.0/pyproject.toml
+-rw-r--r--   0 seleznevk (984925890) 1002642239      991 2023-06-19 09:03:45.185038 dj-jwt-auth-1.0.0/setup.cfg
+-rw-r--r--   0 seleznevk (984925890) 1002642239       90 2022-10-24 09:36:32.000000 dj-jwt-auth-1.0.0/setup.py
+drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-06-19 09:03:45.183215 dj-jwt-auth-1.0.0/tests/
+-rw-r--r--   0 seleznevk (984925890) 1002642239        0 2022-10-13 13:02:24.000000 dj-jwt-auth-1.0.0/tests/__init__.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239      251 2023-06-19 08:33:20.000000 dj-jwt-auth-1.0.0/tests/models.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239     5139 2023-06-19 08:55:20.000000 dj-jwt-auth-1.0.0/tests/test.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239      212 2022-10-14 10:04:40.000000 dj-jwt-auth-1.0.0/tests/urls.py
```

### Comparing `dj-jwt-auth-0.3.1/PKG-INFO` & `dj-jwt-auth-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-jwt-auth
-Version: 0.3.1
+Version: 1.0.0
 Summary: A Django package for JSON Web Token validation and verification. Using PyJWT.
 Home-page: https://www.example.com/
 Author: Konstantin Seleznev
 Author-email: k.seleznev@elsevier.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -43,38 +43,40 @@
         ...
         'django_jwt.middleware.JWTAuthMiddleware',
     ]
 ```
 
 ### Configuration:
 Required variables:
-- JWT_CERTS_URL - certificate endpoint, like `https://keyCloak/realms/h/protocol/openid-connect/certs`
+- OIDC_CERTS_URL - certificate endpoint, like `https://keyCloak/realms/h/.well-known/openid-configuration`
 
 Optional variables:
-- JWT_ALGORITHM - by default `ES256`
-- JWT_AUDIENCE - by default ["account", "broker"]
-- JWT_USER_UID - User model' unique identifier, by default `kc_id`
-
-- JWT_USER_MAPPING - mapping between JWT claims and user model fields, by default:
+- OIDC_AUDIENCE - by default ["account", "broker"]
+User retated variables:
+- OIDC_USER_UPDATE - if True, user model will be updated from userinfo endpoint if MODIFIED date has changed, by default True
+- OIDC_USER_MODIFIED_FIELD - user model field to store last modified date, by default `modified_timestamp`
+- OIDC_TOKEN_MODIFIED_FIELD - access token field to store last modified date, by default `updated_at`
+- OIDC_USER_UID - User model' unique identifier, by default `kc_id`
+- OIDC_USER_MAPPING - mapping between JWT claims and user model fields, by default:
 ```
-    JWT_USER_MAPPING = {
+    OIDC_USER_MAPPING = {
         'first_name': 'first_name',
         'last_name': 'last_name',
         'username': 'username',
     }
 ```
-- JWT_USER_DEFAULTS - default values for user model fields, by default:
+- OIDC_USER_DEFAULTS - default values for user model fields, by default:
 ```
-    JWT_USER_DEFAULTS = {
+    OIDC_USER_DEFAULTS = {
         'is_active': True,
     }
 ```
 
-- JWT_USER_ON_CREATE and JWT_USER_ON_UPDATE - functions to be called on user creation and update, by default:
+- OIDC_USER_ON_CREATE and OIDC_USER_ON_UPDATE - functions to be called on user creation and update, by default:
 ```
-    JWT_USER_ON_CREATE = None
-    JWT_USER_ON_UPDATE = None
+    OIDC_USER_ON_CREATE = None
+    OIDC_USER_ON_UPDATE = None
 ```
 These functions should accept two arguments: user and request.
 
 ### Testing:
 Run command `python runtests.py` to run tests.
```

### Comparing `dj-jwt-auth-0.3.1/README.md` & `dj-jwt-auth-1.0.0/dj_jwt_auth.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: dj-jwt-auth
+Version: 1.0.0
+Summary: A Django package for JSON Web Token validation and verification. Using PyJWT.
+Home-page: https://www.example.com/
+Author: Konstantin Seleznev
+Author-email: k.seleznev@elsevier.com
+License: MIT
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # Django-JWT
 
 This is a package to verify and validate JSON Web Tokens (JWT) in Django.
 
 ### Installation
 1. Install the package using pip.
 
@@ -19,38 +43,40 @@
         ...
         'django_jwt.middleware.JWTAuthMiddleware',
     ]
 ```
 
 ### Configuration:
 Required variables:
-- JWT_CERTS_URL - certificate endpoint, like `https://keyCloak/realms/h/protocol/openid-connect/certs`
+- OIDC_CERTS_URL - certificate endpoint, like `https://keyCloak/realms/h/.well-known/openid-configuration`
 
 Optional variables:
-- JWT_ALGORITHM - by default `ES256`
-- JWT_AUDIENCE - by default ["account", "broker"]
-- JWT_USER_UID - User model' unique identifier, by default `kc_id`
-
-- JWT_USER_MAPPING - mapping between JWT claims and user model fields, by default:
+- OIDC_AUDIENCE - by default ["account", "broker"]
+User retated variables:
+- OIDC_USER_UPDATE - if True, user model will be updated from userinfo endpoint if MODIFIED date has changed, by default True
+- OIDC_USER_MODIFIED_FIELD - user model field to store last modified date, by default `modified_timestamp`
+- OIDC_TOKEN_MODIFIED_FIELD - access token field to store last modified date, by default `updated_at`
+- OIDC_USER_UID - User model' unique identifier, by default `kc_id`
+- OIDC_USER_MAPPING - mapping between JWT claims and user model fields, by default:
 ```
-    JWT_USER_MAPPING = {
+    OIDC_USER_MAPPING = {
         'first_name': 'first_name',
         'last_name': 'last_name',
         'username': 'username',
     }
 ```
-- JWT_USER_DEFAULTS - default values for user model fields, by default:
+- OIDC_USER_DEFAULTS - default values for user model fields, by default:
 ```
-    JWT_USER_DEFAULTS = {
+    OIDC_USER_DEFAULTS = {
         'is_active': True,
     }
 ```
 
-- JWT_USER_ON_CREATE and JWT_USER_ON_UPDATE - functions to be called on user creation and update, by default:
+- OIDC_USER_ON_CREATE and OIDC_USER_ON_UPDATE - functions to be called on user creation and update, by default:
 ```
-    JWT_USER_ON_CREATE = None
-    JWT_USER_ON_UPDATE = None
+    OIDC_USER_ON_CREATE = None
+    OIDC_USER_ON_UPDATE = None
 ```
 These functions should accept two arguments: user and request.
 
 ### Testing:
-Run command `python runtests.py` to run tests.
+Run command `python runtests.py` to run tests.
```

### Comparing `dj-jwt-auth-0.3.1/django_jwt/user.py` & `dj-jwt-auth-1.0.0/django_jwt/user.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,45 @@
+import pytz
+from dateutil import parser
 from django.contrib.auth import get_user_model
 from django.http.request import HttpRequest
 
 from django_jwt import settings
+from django_jwt.utils import oidc_handler
+
+utc = pytz.UTC
 
 
 class UserHandler:
-    def __init__(self, payload: dict, request: HttpRequest):
+    def __init__(self, payload: dict, request: HttpRequest, access_token: str):
+        # payload of access token without user info
         # auth0_id should be available if auth0 added in Client Scopes in KeyCloak admin
-        self.kwargs = settings.JWT_USER_DEFAULTS.copy()
-        self.kwargs.update(
-            {ca_key: payload[kc_key] for kc_key, ca_key in settings.JWT_USER_MAPPING.items() if kc_key in payload}
-        )
-        self.kwargs["email"] = payload["email"].lower()
-        self.kwargs[settings.JWT_USER_UID] = payload.get("auth0_id", payload["sub"])
+        self.kwargs = settings.OIDC_USER_DEFAULTS.copy()
+        self.kwargs[settings.OIDC_USER_UID] = payload.get("auth0_id", payload["sub"])
+        modified_at = payload.get(settings.OIDC_TOKEN_MODIFIED_FIELD, None)
+        self.modified_at = utc.normalize(parser.parse(modified_at)) if modified_at else None
 
-        self.on_create = settings.JWT_USER_ON_CREATE
-        self.on_update = settings.JWT_USER_ON_UPDATE
+        self.on_create = settings.OIDC_USER_ON_CREATE
+        self.on_update = settings.OIDC_USER_ON_UPDATE
         self.request = request
+        self.access_token = access_token
+
+    def _collect_user_data(self):
+        """Collect user data from KeyCloak"""
+
+        if "email" not in self.kwargs:
+            user_data = oidc_handler.get_user_info(self.access_token)
+            self.kwargs["email"] = user_data["email"].lower()
+            self.kwargs.update(
+                {
+                    ca_key: user_data[kc_key]
+                    for kc_key, ca_key in settings.OIDC_USER_MAPPING.items()
+                    if kc_key in user_data
+                }
+            )
 
     def _update_user(self, user):
         """Update user fields if they are changed in KeyCloak"""
 
         is_changed = False
         for key, val in self.kwargs.items():
             if getattr(user, key) != val:
@@ -33,21 +52,28 @@
         """
         Get user from database by kc_id or email.
         If user is not found, create new user.
         Update user fields if they are changed in KeyCloak.
         """
         model = get_user_model()
         try:
-            user = model.objects.get(**{settings.JWT_USER_UID: self.kwargs[settings.JWT_USER_UID]})
+            user = model.objects.get(**{settings.OIDC_USER_UID: self.kwargs[settings.OIDC_USER_UID]})
         except model.DoesNotExist:
+            self._collect_user_data()
             try:
+                # if user is not found by kc_id, try to find by email
                 user = model.objects.get(email=self.kwargs["email"])
             except model.DoesNotExist:
+                # or just create new user
                 user = model.objects.create(**self.kwargs)
                 if self.on_create:
                     self.on_create(user, self.request)
                 return user
 
-        self._update_user(user)
-        if self.on_update:
-            self.on_update(user, self.request)
+        # update user fields if they are changed in KeyCloak
+        user_modified_at = getattr(user, settings.OIDC_USER_MODIFIED_FIELD)
+        if self.modified_at and utc.localize(user_modified_at) < self.modified_at:
+            self._collect_user_data()
+            self._update_user(user)
+            if self.on_update:
+                self.on_update(user, self.request)
         return user
```

### Comparing `dj-jwt-auth-0.3.1/setup.cfg` & `dj-jwt-auth-1.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj-jwt-auth
-version = 0.3.1
+version = 1.0.0
 description = A Django package for JSON Web Token validation and verification. Using PyJWT.
 long_description = file: README.md
 url = https://www.example.com/
 author = Konstantin Seleznev
 author_email = k.seleznev@elsevier.com
 license = MIT
 classifiers =
```

