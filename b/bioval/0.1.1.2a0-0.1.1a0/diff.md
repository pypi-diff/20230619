# Comparing `tmp/bioval-0.1.1.2a0.tar.gz` & `tmp/bioval-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioval-0.1.1.2a0.tar", last modified: Mon Jun 19 18:53:03 2023, max compression
+gzip compressed data, was "bioval-0.1.1a0.tar", last modified: Mon Jun 19 17:27:25 2023, max compression
```

## Comparing `bioval-0.1.1.2a0.tar` & `bioval-0.1.1a0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwx---   0 bendidi   (5571) biofid   (50425)        0 2023-06-19 18:53:03.845339 bioval-0.1.1.2a0/
--rw-rw----   0 bendidi   (5571) biofid   (50425)     1073 2023-06-19 17:23:24.000000 bioval-0.1.1.2a0/LICENSE.txt
--rw-rw----   0 bendidi   (5571) biofid   (50425)     1019 2023-06-19 18:53:03.845339 bioval-0.1.1.2a0/PKG-INFO
-drwxrwx---   0 bendidi   (5571) biofid   (50425)        0 2023-06-19 18:53:03.845339 bioval-0.1.1.2a0/bioval.egg-info/
--rw-rw----   0 bendidi   (5571) biofid   (50425)     1019 2023-06-19 18:53:03.000000 bioval-0.1.1.2a0/bioval.egg-info/PKG-INFO
--rw-rw----   0 bendidi   (5571) biofid   (50425)      194 2023-06-19 18:53:03.000000 bioval-0.1.1.2a0/bioval.egg-info/SOURCES.txt
--rw-rw----   0 bendidi   (5571) biofid   (50425)        1 2023-06-19 18:53:03.000000 bioval-0.1.1.2a0/bioval.egg-info/dependency_links.txt
--rw-rw----   0 bendidi   (5571) biofid   (50425)       65 2023-06-19 18:53:03.000000 bioval-0.1.1.2a0/bioval.egg-info/requires.txt
--rw-rw----   0 bendidi   (5571) biofid   (50425)        7 2023-06-19 18:53:03.000000 bioval-0.1.1.2a0/bioval.egg-info/top_level.txt
--rw-rw----   0 bendidi   (5571) biofid   (50425)     1504 2023-06-19 18:47:57.000000 bioval-0.1.1.2a0/pyproject.toml
--rw-rw----   0 bendidi   (5571) biofid   (50425)       79 2023-06-19 18:53:03.849339 bioval-0.1.1.2a0/setup.cfg
--rw-rw----   0 bendidi   (5571) biofid   (50425)     1996 2023-06-19 18:52:31.000000 bioval-0.1.1.2a0/setup.py
+drwxrwx---   0 bendidi   (5571) biofid   (50425)        0 2023-06-19 17:27:25.080159 bioval-0.1.1a0/
+-rw-rw----   0 bendidi   (5571) biofid   (50425)     1073 2023-06-19 17:23:24.000000 bioval-0.1.1a0/LICENSE.txt
+-rw-rw----   0 bendidi   (5571) biofid   (50425)     1053 2023-06-19 17:27:25.080159 bioval-0.1.1a0/PKG-INFO
+-rw-rw----   0 bendidi   (5571) biofid   (50425)    10685 2023-06-19 17:23:24.000000 bioval-0.1.1a0/README.md
+drwxrwx---   0 bendidi   (5571) biofid   (50425)        0 2023-06-19 17:27:25.080159 bioval-0.1.1a0/bioval.egg-info/
+-rw-rw----   0 bendidi   (5571) biofid   (50425)     1053 2023-06-19 17:27:24.000000 bioval-0.1.1a0/bioval.egg-info/PKG-INFO
+-rw-rw----   0 bendidi   (5571) biofid   (50425)      204 2023-06-19 17:27:24.000000 bioval-0.1.1a0/bioval.egg-info/SOURCES.txt
+-rw-rw----   0 bendidi   (5571) biofid   (50425)        1 2023-06-19 17:27:24.000000 bioval-0.1.1a0/bioval.egg-info/dependency_links.txt
+-rw-rw----   0 bendidi   (5571) biofid   (50425)       65 2023-06-19 17:27:24.000000 bioval-0.1.1a0/bioval.egg-info/requires.txt
+-rw-rw----   0 bendidi   (5571) biofid   (50425)        7 2023-06-19 17:27:24.000000 bioval-0.1.1a0/bioval.egg-info/top_level.txt
+-rw-rw----   0 bendidi   (5571) biofid   (50425)     1460 2023-06-19 17:02:02.000000 bioval-0.1.1a0/pyproject.toml
+-rw-rw----   0 bendidi   (5571) biofid   (50425)       79 2023-06-19 17:27:25.084159 bioval-0.1.1a0/setup.cfg
+-rw-rw----   0 bendidi   (5571) biofid   (50425)     2078 2023-06-19 17:27:20.000000 bioval-0.1.1a0/setup.py
```

### Comparing `bioval-0.1.1.2a0/LICENSE.txt` & `bioval-0.1.1a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bioval-0.1.1.2a0/PKG-INFO` & `bioval-0.1.1a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bioval
-Version: 0.1.1.2a0
-Summary: Bioval is a Python package made to provide a wrapper and an easy access to a collection of evaluation metrics for comparing the similarity of two tensors, adapted to different evaluation processes of generative models applied to biological images.
+Version: 0.1.1a0
+Summary: Bioval is a Python package made to provide a wrapper and an easy access to a collection of evaluation metrics for comparing the similarity of two tensors, adapted to different evaluation processes of generative models applied to biological images, and by extension to natural images.
 Home-page: https://github.com/IhabBendidi/bioval
 Download-URL: https://github.com/IhabBendidi/bioval/archive/refs/tags/v0.1.1-alpha.tar.gz
 Author: Ihab Bendidi, Ethan Cohen, Auguste Genovesio
 Author-email: bendidiihab@gmail.Com
 License: MIT
 Keywords: biology,evaluation,generative models
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bioval-0.1.1.2a0/bioval.egg-info/PKG-INFO` & `bioval-0.1.1a0/bioval.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bioval
-Version: 0.1.1.2a0
-Summary: Bioval is a Python package made to provide a wrapper and an easy access to a collection of evaluation metrics for comparing the similarity of two tensors, adapted to different evaluation processes of generative models applied to biological images.
+Version: 0.1.1a0
+Summary: Bioval is a Python package made to provide a wrapper and an easy access to a collection of evaluation metrics for comparing the similarity of two tensors, adapted to different evaluation processes of generative models applied to biological images, and by extension to natural images.
 Home-page: https://github.com/IhabBendidi/bioval
 Download-URL: https://github.com/IhabBendidi/bioval/archive/refs/tags/v0.1.1-alpha.tar.gz
 Author: Ihab Bendidi, Ethan Cohen, Auguste Genovesio
 Author-email: bendidiihab@gmail.Com
 License: MIT
 Keywords: biology,evaluation,generative models
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bioval-0.1.1.2a0/pyproject.toml` & `bioval-0.1.1a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,10 @@
 torchvision = "*"
 Pillow = "*"
 nvidia-ml-py = "*"
 piq = "*"
 pot = "*"
 scikit-learn = "*"
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-packages = [
-    { include = "bioval" },
-]
```

### Comparing `bioval-0.1.1.2a0/setup.py` & `bioval-0.1.1a0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 setup(
   name = 'bioval',         # How you named your package folder (MyLib)
   packages = ['bioval'],   # Chose the same as "name"
-  version = '0.1.1.2-alpha',      # Start with a small number and increase it with every change you make
+  version = '0.1.1-alpha',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-  description = 'Bioval is a Python package made to provide a wrapper and an easy access to a collection of evaluation metrics for comparing the similarity of two tensors, adapted to different evaluation processes of generative models applied to biological images.',
+  description = 'Bioval is a Python package made to provide a wrapper and an easy access to a collection of evaluation metrics for comparing the similarity of two tensors, adapted to different evaluation processes of generative models applied to biological images, and by extension to natural images.',   # Give a short description about your library
   author = 'Ihab Bendidi, Ethan Cohen, Auguste Genovesio',                   # Type in your name
   author_email = 'bendidiihab@gmail.Com',      # Type in your E-Mail
   url = 'https://github.com/IhabBendidi/bioval',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/IhabBendidi/bioval/archive/refs/tags/v0.1.1-alpha.tar.gz',    # I explain this later on
   keywords = ['biology', 'evaluation', 'generative models',],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
         'numpy',
```

