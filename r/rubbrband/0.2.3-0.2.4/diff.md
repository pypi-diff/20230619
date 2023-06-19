# Comparing `tmp/rubbrband-0.2.3.tar.gz` & `tmp/rubbrband-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubbrband-0.2.3.tar", last modified: Mon Jun 19 19:59:11 2023, max compression
+gzip compressed data, was "rubbrband-0.2.4.tar", last modified: Mon Jun 19 20:14:18 2023, max compression
```

## Comparing `rubbrband-0.2.3.tar` & `rubbrband-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-19 19:59:11.411768 rubbrband-0.2.3/
--rw-r--r--   0 llewyn     (501) staff       (20)    11357 2023-03-07 10:22:28.000000 rubbrband-0.2.3/LICENSE
--rw-r--r--   0 llewyn     (501) staff       (20)       48 2023-02-24 08:26:52.000000 rubbrband-0.2.3/MANIFEST.in
--rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-06-19 19:59:11.411820 rubbrband-0.2.3/PKG-INFO
--rw-r--r--   0 llewyn     (501) staff       (20)       54 2023-06-07 21:39:04.000000 rubbrband-0.2.3/README.md
--rw-r--r--   0 llewyn     (501) staff       (20)       93 2023-06-07 21:38:14.000000 rubbrband-0.2.3/pyproject.toml
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-19 19:59:11.411069 rubbrband-0.2.3/rubbrband/
--rw-r--r--   0 llewyn     (501) staff       (20)       61 2023-06-07 21:45:01.000000 rubbrband-0.2.3/rubbrband/__init__.py
--rw-r--r--   0 llewyn     (501) staff       (20)     1359 2023-06-19 19:56:51.000000 rubbrband-0.2.3/rubbrband/main.py
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-19 19:59:11.411659 rubbrband-0.2.3/rubbrband.egg-info/
--rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-06-19 19:59:11.000000 rubbrband-0.2.3/rubbrband.egg-info/PKG-INFO
--rw-r--r--   0 llewyn     (501) staff       (20)      267 2023-06-19 19:59:11.000000 rubbrband-0.2.3/rubbrband.egg-info/SOURCES.txt
--rw-r--r--   0 llewyn     (501) staff       (20)        1 2023-06-19 19:59:11.000000 rubbrband-0.2.3/rubbrband.egg-info/dependency_links.txt
--rw-r--r--   0 llewyn     (501) staff       (20)        9 2023-06-19 19:59:11.000000 rubbrband-0.2.3/rubbrband.egg-info/requires.txt
--rw-r--r--   0 llewyn     (501) staff       (20)       10 2023-06-19 19:59:11.000000 rubbrband-0.2.3/rubbrband.egg-info/top_level.txt
--rw-r--r--   0 llewyn     (501) staff       (20)      251 2023-06-19 19:59:11.412023 rubbrband-0.2.3/setup.cfg
--rw-r--r--   0 llewyn     (501) staff       (20)      172 2023-06-07 21:37:58.000000 rubbrband-0.2.3/setup.py
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-19 20:14:18.685233 rubbrband-0.2.4/
+-rw-r--r--   0 llewyn     (501) staff       (20)    11357 2023-03-07 10:22:28.000000 rubbrband-0.2.4/LICENSE
+-rw-r--r--   0 llewyn     (501) staff       (20)       48 2023-02-24 08:26:52.000000 rubbrband-0.2.4/MANIFEST.in
+-rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-06-19 20:14:18.685294 rubbrband-0.2.4/PKG-INFO
+-rw-r--r--   0 llewyn     (501) staff       (20)       54 2023-06-07 21:39:04.000000 rubbrband-0.2.4/README.md
+-rw-r--r--   0 llewyn     (501) staff       (20)       93 2023-06-07 21:38:14.000000 rubbrband-0.2.4/pyproject.toml
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-19 20:14:18.684397 rubbrband-0.2.4/rubbrband/
+-rw-r--r--   0 llewyn     (501) staff       (20)       61 2023-06-07 21:45:01.000000 rubbrband-0.2.4/rubbrband/__init__.py
+-rw-r--r--   0 llewyn     (501) staff       (20)     1357 2023-06-19 20:13:52.000000 rubbrband-0.2.4/rubbrband/main.py
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-19 20:14:18.685124 rubbrband-0.2.4/rubbrband.egg-info/
+-rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-06-19 20:14:18.000000 rubbrband-0.2.4/rubbrband.egg-info/PKG-INFO
+-rw-r--r--   0 llewyn     (501) staff       (20)      267 2023-06-19 20:14:18.000000 rubbrband-0.2.4/rubbrband.egg-info/SOURCES.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)        1 2023-06-19 20:14:18.000000 rubbrband-0.2.4/rubbrband.egg-info/dependency_links.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)        9 2023-06-19 20:14:18.000000 rubbrband-0.2.4/rubbrband.egg-info/requires.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)       10 2023-06-19 20:14:18.000000 rubbrband-0.2.4/rubbrband.egg-info/top_level.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)      251 2023-06-19 20:14:18.685521 rubbrband-0.2.4/setup.cfg
+-rw-r--r--   0 llewyn     (501) staff       (20)      172 2023-06-07 21:37:58.000000 rubbrband-0.2.4/setup.py
```

### Comparing `rubbrband-0.2.3/LICENSE` & `rubbrband-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rubbrband-0.2.3/rubbrband/main.py` & `rubbrband-0.2.4/rubbrband/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 def upload(image, prompt, metadata={}):
     if api_key is None:
         print("Provide an API key in the init function")
 
         return False
 
-    if type(image) == "PIL.PngImagePlugin.PngImageFile":
+    if type(image) == PIL.PngImagePlugin.PngImageFile:
         image = image_to_byte_array(image)
 
     metadata["prompt"] = prompt
     name = str(uuid.uuid4()) + ".jpg"
 
     response = requests.post(
         "https://block.rubbrband.com/upload_img?api_key=" + api_key,
```

