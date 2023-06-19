# Comparing `tmp/OpenAIAuth-1.0.2.tar.gz` & `tmp/OpenAIAuth-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenAIAuth-1.0.2.tar", last modified: Sat May 27 02:21:47 2023, max compression
+gzip compressed data, was "OpenAIAuth-1.0.3.tar", last modified: Mon Jun 19 08:27:42 2023, max compression
```

## Comparing `OpenAIAuth-1.0.2.tar` & `OpenAIAuth-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:21:47.687727 OpenAIAuth-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-27 02:21:22.000000 OpenAIAuth-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-27 02:21:47.687727 OpenAIAuth-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-27 02:21:22.000000 OpenAIAuth-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 02:21:47.687727 OpenAIAuth-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-27 02:21:22.000000 OpenAIAuth-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:21:47.687727 OpenAIAuth-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:21:47.687727 OpenAIAuth-1.0.2/src/OpenAIAuth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-27 02:21:47.000000 OpenAIAuth-1.0.2/src/OpenAIAuth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-27 02:21:47.000000 OpenAIAuth-1.0.2/src/OpenAIAuth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:21:47.000000 OpenAIAuth-1.0.2/src/OpenAIAuth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-27 02:21:47.000000 OpenAIAuth-1.0.2/src/OpenAIAuth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 02:21:47.000000 OpenAIAuth-1.0.2/src/OpenAIAuth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-05-27 02:21:22.000000 OpenAIAuth-1.0.2/src/OpenAIAuth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:27:42.662939 OpenAIAuth-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-19 08:27:19.000000 OpenAIAuth-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-19 08:27:42.662939 OpenAIAuth-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-19 08:27:19.000000 OpenAIAuth-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 08:27:42.662939 OpenAIAuth-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-19 08:27:19.000000 OpenAIAuth-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:27:42.662939 OpenAIAuth-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:27:42.662939 OpenAIAuth-1.0.3/src/OpenAIAuth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-19 08:27:42.000000 OpenAIAuth-1.0.3/src/OpenAIAuth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-19 08:27:42.000000 OpenAIAuth-1.0.3/src/OpenAIAuth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:27:42.000000 OpenAIAuth-1.0.3/src/OpenAIAuth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 08:27:42.000000 OpenAIAuth-1.0.3/src/OpenAIAuth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 08:27:42.000000 OpenAIAuth-1.0.3/src/OpenAIAuth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-19 08:27:19.000000 OpenAIAuth-1.0.3/src/OpenAIAuth.py
```

### Comparing `OpenAIAuth-1.0.2/LICENSE` & `OpenAIAuth-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenAIAuth-1.0.2/setup.py` & `OpenAIAuth-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="OpenAIAuth",
-    version="1.0.2",
+    version="1.0.3",
     license="MIT",
     author="pengzhile",
     author_email="acheong@student.dalat.org",
     description="OpenAI Authentication Reverse Engineered",
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=["OpenAIAuth"],
```

### Comparing `OpenAIAuth-1.0.2/src/OpenAIAuth.py` & `OpenAIAuth-1.0.3/src/OpenAIAuth.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,24 @@
         self,
         email: str,
         password: str,
         proxy: str = None,
         use_cache: bool = True,
         mfa: str = None,
     ):
+        """
+        Initializes an instance of the Auth0 class.
+
+        Args:
+        - email (str): The email address of the user.
+        - password (str): The password of the user.
+        - proxy (str, optional): The proxy server to use for requests. Defaults to None.
+        - use_cache (bool, optional): Flag indicating whether to use cache for access token. Defaults to True.
+        - mfa (str, optional): The multi-factor authentication method. Defaults to None.
+        """
         self.session_token = None
         self.email = email
         self.password = password
         self.use_cache = use_cache
         self.mfa = mfa
         self.session = requests.Session()
         self.req_kwargs = {
@@ -45,14 +55,21 @@
 
     @staticmethod
     def __check_email(email: str):
         regex = r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b"
         return re.fullmatch(regex, email)
 
     def auth(self) -> str:
+        """
+        Authenticates the user and returns the access token.
+
+        Returns:
+        - str: The access token.
+        """
+
         if (
             self.use_cache
             and self.access_token
             and self.expires
             and self.expires > dt.now()
         ):
             return self.access_token
```

