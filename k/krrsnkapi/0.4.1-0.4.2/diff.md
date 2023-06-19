# Comparing `tmp/krrsnkapi-0.4.1.tar.gz` & `tmp/krrsnkapi-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krrsnkapi-0.4.1.tar", last modified: Mon Jun 19 20:08:21 2023, max compression
+gzip compressed data, was "krrsnkapi-0.4.2.tar", last modified: Mon Jun 19 20:18:19 2023, max compression
```

## Comparing `krrsnkapi-0.4.1.tar` & `krrsnkapi-0.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 20:08:21.646414 krrsnkapi-0.4.1/
--rw-rw-rw-   0        0        0     1087 2023-04-13 13:12:53.000000 krrsnkapi-0.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0      619 2023-06-19 20:08:21.648414 krrsnkapi-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1569 2023-04-13 12:53:07.000000 krrsnkapi-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 20:08:21.622413 krrsnkapi-0.4.1/krrsnkapi/
--rw-rw-rw-   0        0        0       52 2023-06-19 20:08:00.000000 krrsnkapi-0.4.1/krrsnkapi/__init__.py
--rw-rw-rw-   0        0        0     2519 2023-06-19 20:00:30.000000 krrsnkapi-0.4.1/krrsnkapi/krrsnkapi.py
-drwxrwxrwx   0        0        0        0 2023-06-19 20:08:21.644414 krrsnkapi-0.4.1/krrsnkapi.egg-info/
--rw-rw-rw-   0        0        0      619 2023-06-19 20:08:20.000000 krrsnkapi-0.4.1/krrsnkapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-06-19 20:08:21.000000 krrsnkapi-0.4.1/krrsnkapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 20:08:20.000000 krrsnkapi-0.4.1/krrsnkapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-19 20:08:20.000000 krrsnkapi-0.4.1/krrsnkapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-19 20:08:20.000000 krrsnkapi-0.4.1/krrsnkapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-19 20:08:21.650415 krrsnkapi-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1447 2023-06-19 20:08:10.000000 krrsnkapi-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:18:19.108087 krrsnkapi-0.4.2/
+-rw-rw-rw-   0        0        0     1087 2023-04-13 13:12:53.000000 krrsnkapi-0.4.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      621 2023-06-19 20:18:19.109087 krrsnkapi-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1569 2023-04-13 12:53:07.000000 krrsnkapi-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 20:18:19.090086 krrsnkapi-0.4.2/krrsnkapi/
+-rw-rw-rw-   0        0        0       52 2023-06-19 20:08:00.000000 krrsnkapi-0.4.2/krrsnkapi/__init__.py
+-rw-rw-rw-   0        0        0     2556 2023-06-19 20:14:35.000000 krrsnkapi-0.4.2/krrsnkapi/krrsnkapi.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:18:19.105087 krrsnkapi-0.4.2/krrsnkapi.egg-info/
+-rw-rw-rw-   0        0        0      621 2023-06-19 20:18:18.000000 krrsnkapi-0.4.2/krrsnkapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-06-19 20:18:18.000000 krrsnkapi-0.4.2/krrsnkapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 20:18:18.000000 krrsnkapi-0.4.2/krrsnkapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-19 20:18:18.000000 krrsnkapi-0.4.2/krrsnkapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-19 20:18:18.000000 krrsnkapi-0.4.2/krrsnkapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-19 20:18:19.111087 krrsnkapi-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1449 2023-06-19 20:17:17.000000 krrsnkapi-0.4.2/setup.py
```

### Comparing `krrsnkapi-0.4.1/LICENSE.txt` & `krrsnkapi-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.4.1/PKG-INFO` & `krrsnkapi-0.4.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krrsnkapi
-Version: 0.4.1
+Version: 0.4.2
 Summary: Module for easy use of my api | info on GitHub: https://github.com/kararasenok-gd/krrsnkapi
 Home-page: https://github.com/kararasenok-gd/krrsnkapi
-Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.4.tar.gz
+Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.4.2.tar.gz
 Author: kararasenok_gd
 Author-email: murzikkurzikpro@gmail.com
 License: MIT
 Keywords: api
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krrsnkapi-0.4.1/README.md` & `krrsnkapi-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.4.1/krrsnkapi/krrsnkapi.py` & `krrsnkapi-0.4.2/krrsnkapi/krrsnkapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,11 +93,12 @@
 
 class r34:
 	def __init__(self, apikey):
 		self.apikey = apikey
 
 	def get_url(self, keyword, page = 0):
 		self.keyword = keyword
+		self.page = page
 
-		self.response = requests.post(f"https://kararasenok.ueuo.com/api/v1/r34/?keyword={self.keyword}&apikey={self.apikey}")
+		self.response = requests.post(f"https://kararasenok.ueuo.com/api/v1/r34/?keyword={self.keyword}&apikey={self.apikey}&page={self.page}")
 
 		return self.response.text
```

### Comparing `krrsnkapi-0.4.1/krrsnkapi.egg-info/PKG-INFO` & `krrsnkapi-0.4.2/krrsnkapi.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krrsnkapi
-Version: 0.4.1
+Version: 0.4.2
 Summary: Module for easy use of my api | info on GitHub: https://github.com/kararasenok-gd/krrsnkapi
 Home-page: https://github.com/kararasenok-gd/krrsnkapi
-Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.4.tar.gz
+Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.4.2.tar.gz
 Author: kararasenok_gd
 Author-email: murzikkurzikpro@gmail.com
 License: MIT
 Keywords: api
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krrsnkapi-0.4.1/setup.py` & `krrsnkapi-0.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 # ver = input("version: ")
 
 setup(
   name = 'krrsnkapi',         # How you named your package folder (MyLib)
   packages = ['krrsnkapi'],   # Chose the same as "name"
-  version = "0.4.1",      # Start with a small number and increase it with every change you make
+  version = "0.4.2",      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Module for easy use of my api | info on GitHub: https://github.com/kararasenok-gd/krrsnkapi',   # Give a short description about your library
   author = 'kararasenok_gd',                   # Type in your name
   author_email = 'murzikkurzikpro@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/kararasenok-gd/krrsnkapi',   # Provide either the link to your github or to your website
-  download_url = f'https://github.com/kararasenok-gd/krrsnkapi/archive/v0.4.tar.gz',    # I explain this later on
+  download_url = f'https://github.com/kararasenok-gd/krrsnkapi/archive/v0.4.2.tar.gz',    # I explain this later on
   keywords = ["api"],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests'
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Topic :: Software Development :: Build Tools',
```

