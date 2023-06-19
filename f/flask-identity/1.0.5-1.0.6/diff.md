# Comparing `tmp/flask_identity-1.0.5.tar.gz` & `tmp/flask_identity-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_identity-1.0.5.tar", max compression
+gzip compressed data, was "flask_identity-1.0.6.tar", max compression
```

## Comparing `flask_identity-1.0.5.tar` & `flask_identity-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1119 2023-05-29 12:41:30.306646 flask_identity-1.0.5/LICENSE.rst
--rw-r--r--   0        0        0     2604 2023-05-29 12:45:53.285419 flask_identity-1.0.5/README.rst
--rw-r--r--   0        0        0      905 2023-05-31 01:12:45.393303 flask_identity-1.0.5/flask_identity/__init__.py
--rw-r--r--   0        0        0     2225 2023-06-02 15:57:07.213555 flask_identity-1.0.5/flask_identity/_hash_context.py
--rw-r--r--   0        0        0     3325 2023-06-02 15:57:20.326013 flask_identity-1.0.5/flask_identity/_token_context.py
--rw-r--r--   0        0        0     1243 2023-05-31 01:12:45.379734 flask_identity-1.0.5/flask_identity/babels.py
--rw-r--r--   0        0        0      840 2023-05-31 01:12:45.404196 flask_identity-1.0.5/flask_identity/compats.py
--rw-r--r--   0        0        0    10558 2023-06-03 13:49:39.379245 flask_identity-1.0.5/flask_identity/config.py
--rw-r--r--   0        0        0    18255 2023-06-02 15:51:11.741304 flask_identity-1.0.5/flask_identity/core.py
--rw-r--r--   0        0        0    14348 2023-06-02 16:01:44.758996 flask_identity-1.0.5/flask_identity/datastore.py
--rw-r--r--   0        0        0     7825 2023-06-03 13:28:19.267568 flask_identity-1.0.5/flask_identity/decorators.py
--rw-r--r--   0        0        0     3944 2023-06-02 15:50:19.098559 flask_identity-1.0.5/flask_identity/forms.py
--rw-r--r--   0        0        0     5413 2023-06-02 16:07:32.388007 flask_identity-1.0.5/flask_identity/mixins.py
--rw-r--r--   0        0        0      823 2023-05-29 12:41:30.313443 flask_identity-1.0.5/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo
--rw-r--r--   0        0        0     1269 2023-05-29 12:41:30.313585 flask_identity-1.0.5/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po
--rw-r--r--   0        0        0     1076 2023-05-29 12:41:30.313677 flask_identity-1.0.5/flask_identity/translations/flask_identity.pot
--rw-r--r--   0        0        0      814 2023-05-29 12:41:30.313893 flask_identity-1.0.5/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.mo
--rw-r--r--   0        0        0     1264 2023-05-29 12:41:30.314002 flask_identity-1.0.5/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.po
--rw-r--r--   0        0        0    10158 2023-06-03 13:42:18.463471 flask_identity-1.0.5/flask_identity/utils.py
--rw-r--r--   0        0        0     6204 2023-06-02 15:59:26.317960 flask_identity-1.0.5/flask_identity/views.py
--rw-r--r--   0        0        0     1743 2023-06-14 03:34:34.840779 flask_identity-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 flask_identity-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1119 2023-05-29 12:41:30.306646 flask_identity-1.0.6/LICENSE.rst
+-rw-r--r--   0        0        0     2604 2023-05-29 12:45:53.285419 flask_identity-1.0.6/README.rst
+-rw-r--r--   0        0        0      905 2023-05-31 01:12:45.393303 flask_identity-1.0.6/flask_identity/__init__.py
+-rw-r--r--   0        0        0     2562 2023-06-19 02:23:03.039513 flask_identity-1.0.6/flask_identity/_hash_context.py
+-rw-r--r--   0        0        0     3325 2023-06-02 15:57:20.326013 flask_identity-1.0.6/flask_identity/_token_context.py
+-rw-r--r--   0        0        0     1243 2023-05-31 01:12:45.379734 flask_identity-1.0.6/flask_identity/babels.py
+-rw-r--r--   0        0        0      840 2023-05-31 01:12:45.404196 flask_identity-1.0.6/flask_identity/compats.py
+-rw-r--r--   0        0        0    10558 2023-06-03 13:49:39.379245 flask_identity-1.0.6/flask_identity/config.py
+-rw-r--r--   0        0        0    18255 2023-06-02 15:51:11.741304 flask_identity-1.0.6/flask_identity/core.py
+-rw-r--r--   0        0        0    14348 2023-06-02 16:01:44.758996 flask_identity-1.0.6/flask_identity/datastore.py
+-rw-r--r--   0        0        0     7825 2023-06-03 13:28:19.267568 flask_identity-1.0.6/flask_identity/decorators.py
+-rw-r--r--   0        0        0     3944 2023-06-02 15:50:19.098559 flask_identity-1.0.6/flask_identity/forms.py
+-rw-r--r--   0        0        0     5413 2023-06-02 16:07:32.388007 flask_identity-1.0.6/flask_identity/mixins.py
+-rw-r--r--   0        0        0      823 2023-05-29 12:41:30.313443 flask_identity-1.0.6/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo
+-rw-r--r--   0        0        0     1269 2023-05-29 12:41:30.313585 flask_identity-1.0.6/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po
+-rw-r--r--   0        0        0     1076 2023-05-29 12:41:30.313677 flask_identity-1.0.6/flask_identity/translations/flask_identity.pot
+-rw-r--r--   0        0        0      814 2023-05-29 12:41:30.313893 flask_identity-1.0.6/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.mo
+-rw-r--r--   0        0        0     1264 2023-05-29 12:41:30.314002 flask_identity-1.0.6/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.po
+-rw-r--r--   0        0        0    10158 2023-06-03 13:42:18.463471 flask_identity-1.0.6/flask_identity/utils.py
+-rw-r--r--   0        0        0     6204 2023-06-02 15:59:26.317960 flask_identity-1.0.6/flask_identity/views.py
+-rw-r--r--   0        0        0     1743 2023-06-19 02:24:53.194196 flask_identity-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 flask_identity-1.0.6/PKG-INFO
```

### Comparing `flask_identity-1.0.5/LICENSE.rst` & `flask_identity-1.0.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/README.rst` & `flask_identity-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/__init__.py` & `flask_identity-1.0.6/flask_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/_hash_context.py` & `flask_identity-1.0.6/flask_identity/_hash_context.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,17 @@
     Hash Context of Flask-Identity
 
     :author: solardiax <solardiax@hotmail.com>
     :copyright: (c) 2020 by DreamEx Works.
     :license: MIT, see LICENSE for more details.
 """
 
-
+import base64
+import hmac
+import hashlib
 from passlib.context import CryptContext
 
 
 class HashContext(object):
     """
     | Class to generate/verify hash securitied string.
     | Hashed string can be used to store context or any unencrypt context.
@@ -28,41 +30,46 @@
 
         if secret_key is None:
             raise SystemError("Config setting SECRET_KEY or IDENTITY_HASH_SALT is missing.")
 
         schemes = app.config.get("IDENTITY_HASH_SCHEMES", ["bcrypt"])
         schemes_keywords = app.config.get("IDENTITY_HASH_OPTIONS", {})
 
+        self._secret_key: str = secret_key
         # Create a passlib CryptContext
-        self.crypt_context = CryptContext(schemes, **schemes_keywords)
+        self._crypt_context = CryptContext(schemes, **schemes_keywords)
 
-    def hash_context(self, context: str) -> str:
+    def hash_context(self, plaintext: str) -> str:
         """
-        Hash plaintext ``context`` using the ``IDENTITY_HASH_SCHEMES`` specified in the app config.
-        :param context: Plaintext string that the user types in.
+        Hash plaintext ``plaintext`` using the ``IDENTITY_HASH_SCHEMES`` specified in the app config.
+        :param plaintext: Plaintext string that the user types in.
         :return: hashed context.
 
         Example:
             ``user.context = hash_context("mycontext")``
         """
 
         # Use passlib's CryptContext to hash a context
-        context_hash = self.crypt_context.encrypt(context)
+        context_hash = self._crypt_context.encrypt(self._get_hmac_str(plaintext))
 
         return context_hash
 
-    def verify_context(self, context: str, context_hash: str) -> bool:
+    def verify_context(self, plaintext: str, plaintext_hash: str) -> bool:
         """
         Verify plaintext ``context`` against ``hashed context``.
-        :param context: Plaintext context that the user types in.
-        :param context_hash: context hash generated by a previous call to ``hash_context()``.
+        :param plaintext: Plaintext context that the user types in.
+        :param plaintext_hash: context hash generated by a previous call to ``hash_context()``.
         :return:
-            | True when ``context`` matches ``context_hash``.
+            | True when ``content`` matches ``context_hash``.
             | False otherwise.
 
         Example:
             ::
-                if verify_context("mycontext", user.context):
+                if verify_context("mycontext", user.content):
                     login_user(user)
         """
         # Use passlib's CryptContext to verify a context
-        return self.crypt_context.verify(context, context_hash)
+        return self._crypt_context.verify(plaintext, plaintext_hash)
+
+    def _get_hmac_str(self, plaintext: str) -> str:
+        h = hmac.new(self._secret_key.encode("utf-8"), plaintext.encode("utf-8"), hashlib.sha512)
+        return base64.b64encode(h.digest()).decode("ascii")
```

### Comparing `flask_identity-1.0.5/flask_identity/_token_context.py` & `flask_identity-1.0.6/flask_identity/_token_context.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/babels.py` & `flask_identity-1.0.6/flask_identity/babels.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/compats.py` & `flask_identity-1.0.6/flask_identity/compats.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/config.py` & `flask_identity-1.0.6/flask_identity/config.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/core.py` & `flask_identity-1.0.6/flask_identity/core.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/datastore.py` & `flask_identity-1.0.6/flask_identity/datastore.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/decorators.py` & `flask_identity-1.0.6/flask_identity/decorators.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/forms.py` & `flask_identity-1.0.6/flask_identity/forms.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/mixins.py` & `flask_identity-1.0.6/flask_identity/mixins.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo` & `flask_identity-1.0.6/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po` & `flask_identity-1.0.6/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/translations/flask_identity.pot` & `flask_identity-1.0.6/flask_identity/translations/flask_identity.pot`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.mo` & `flask_identity-1.0.6/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.mo`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.po` & `flask_identity-1.0.6/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.po`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/utils.py` & `flask_identity-1.0.6/flask_identity/utils.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/flask_identity/views.py` & `flask_identity-1.0.6/flask_identity/views.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.5/pyproject.toml` & `flask_identity-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple/"
 priority = "supplemental"
 
 [tool.poetry]
 name = "Flask-Identity"
-version = "1.0.5"
+version = "1.0.6"
 description = "A lightweight extension & library to security Flask applications quickly and simply."
 authors = ["SolardiaX <solardiax@hotmail.com>"]
 maintainers = ["SolardiaX <solardiax@hotmail.com>"]
 license = "MIT"
 readme="README.rst"
 repository="https://github.com/SolardiaX/flask-identity"
 homepage="https://github.com/SolardiaX/flask-identity"
```

### Comparing `flask_identity-1.0.5/PKG-INFO` & `flask_identity-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-identity
-Version: 1.0.5
+Version: 1.0.6
 Summary: A lightweight extension & library to security Flask applications quickly and simply.
 Home-page: https://github.com/SolardiaX/flask-identity
 License: MIT
 Author: SolardiaX
 Author-email: solardiax@hotmail.com
 Maintainer: SolardiaX
 Maintainer-email: solardiax@hotmail.com
```

