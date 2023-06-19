# Comparing `tmp/selenium-recaptcha-solver-1.8.2.tar.gz` & `tmp/selenium-recaptcha-solver-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-recaptcha-solver-1.8.2.tar", last modified: Sun Jun  4 18:47:35 2023, max compression
+gzip compressed data, was "selenium-recaptcha-solver-1.8.3.tar", last modified: Mon Jun 19 11:30:09 2023, max compression
```

## Comparing `selenium-recaptcha-solver-1.8.2.tar` & `selenium-recaptcha-solver-1.8.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 18:47:35.298133 selenium-recaptcha-solver-1.8.2/
--rw-rw-rw-   0        0        0     1095 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.8.2/LICENSE
--rw-rw-rw-   0        0        0     3375 2023-06-04 18:47:35.297133 selenium-recaptcha-solver-1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     2949 2023-05-22 08:12:23.000000 selenium-recaptcha-solver-1.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 18:47:35.291133 selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver/
--rw-rw-rw-   0        0        0      170 2023-02-21 21:45:09.000000 selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver/__init__.py
--rw-rw-rw-   0        0        0      971 2023-04-12 10:28:50.000000 selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver/delay_config.py
--rw-rw-rw-   0        0        0       48 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver/exceptions.py
--rw-rw-rw-   0        0        0     7838 2023-02-11 09:55:38.000000 selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver/services.py
--rw-rw-rw-   0        0        0     8889 2023-06-04 18:41:48.000000 selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver/solver.py
-drwxrwxrwx   0        0        0        0 2023-06-04 18:47:35.296133 selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver.egg-info/
--rw-rw-rw-   0        0        0     3375 2023-06-04 18:47:35.000000 selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-06-04 18:47:35.000000 selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 18:47:35.000000 selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-06-04 18:47:35.000000 selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-06-04 18:47:35.000000 selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 18:47:35.298133 selenium-recaptcha-solver-1.8.2/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-06-04 18:47:23.000000 selenium-recaptcha-solver-1.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 18:47:35.296133 selenium-recaptcha-solver-1.8.2/tests/
--rw-rw-rw-   0        0        0     1220 2023-06-04 18:45:28.000000 selenium-recaptcha-solver-1.8.2/tests/test_api.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:30:09.397650 selenium-recaptcha-solver-1.8.3/
+-rw-rw-rw-   0        0        0     1095 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.8.3/LICENSE
+-rw-rw-rw-   0        0        0     3375 2023-06-19 11:30:09.397650 selenium-recaptcha-solver-1.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2949 2023-05-22 08:12:23.000000 selenium-recaptcha-solver-1.8.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 11:30:09.390397 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/
+-rw-rw-rw-   0        0        0      170 2023-02-21 21:45:09.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/__init__.py
+-rw-rw-rw-   0        0        0      971 2023-04-12 10:28:50.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/delay_config.py
+-rw-rw-rw-   0        0        0       48 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/exceptions.py
+-rw-rw-rw-   0        0        0     7838 2023-06-19 11:19:34.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/services.py
+-rw-rw-rw-   0        0        0     8889 2023-06-04 18:41:48.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/solver.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:30:09.394645 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver.egg-info/
+-rw-rw-rw-   0        0        0     3375 2023-06-19 11:30:09.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-06-19 11:30:09.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 11:30:09.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-06-19 11:30:09.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-19 11:30:09.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 11:30:09.397650 selenium-recaptcha-solver-1.8.3/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-06-19 11:28:41.000000 selenium-recaptcha-solver-1.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:30:09.395651 selenium-recaptcha-solver-1.8.3/tests/
+-rw-rw-rw-   0        0        0     1220 2023-06-19 11:24:15.000000 selenium-recaptcha-solver-1.8.3/tests/test_api.py
```

### Comparing `selenium-recaptcha-solver-1.8.2/LICENSE` & `selenium-recaptcha-solver-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.8.2/PKG-INFO` & `selenium-recaptcha-solver-1.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-recaptcha-solver
-Version: 1.8.2
+Version: 1.8.3
 Home-page: https://github.com/thicccat688/selenium-recaptcha-solver
 Download-URL: https://pypi.org/project/selenium-recaptcha-solver
 Author: Tomás Perestrelo
 Author-email: tomasperestrelo21@gmail.com
 License: MIT
 Keywords: python,captcha,speech recognition,selenium,web automation
 Description-Content-Type: text/markdown
```

### Comparing `selenium-recaptcha-solver-1.8.2/README.md` & `selenium-recaptcha-solver-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver/delay_config.py` & `selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/delay_config.py`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver/services.py` & `selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/services.py`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver/solver.py` & `selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/solver.py`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.8.2/selenium_recaptcha_solver.egg-info/PKG-INFO` & `selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-recaptcha-solver
-Version: 1.8.2
+Version: 1.8.3
 Home-page: https://github.com/thicccat688/selenium-recaptcha-solver
 Download-URL: https://pypi.org/project/selenium-recaptcha-solver
 Author: Tomás Perestrelo
 Author-email: tomasperestrelo21@gmail.com
 License: MIT
 Keywords: python,captcha,speech recognition,selenium,web automation
 Description-Content-Type: text/markdown
```

### Comparing `selenium-recaptcha-solver-1.8.2/setup.py` & `selenium-recaptcha-solver-1.8.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='selenium-recaptcha-solver',
-    version='1.8.2',
+    version='1.8.3',
     license='MIT',
     author='Tomás Perestrelo',
     author_email='tomasperestrelo21@gmail.com',
     packages=find_packages(exclude=('tests*', 'testing*')),
     url='https://github.com/thicccat688/selenium-recaptcha-solver',
     download_url='https://pypi.org/project/selenium-recaptcha-solver',
     keywords='python, captcha, speech recognition, selenium, web automation',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'selenium~=4.8.0',
         'pydub~=0.25.1',
-        'SpeechRecognition~=3.9.0',
-        'requests~=2.28.1',
+        'SpeechRecognition~=3.8.1',
+        'requests>=2.28.1,<2.32.0',
     ],
 )
```

### Comparing `selenium-recaptcha-solver-1.8.2/tests/test_api.py` & `selenium-recaptcha-solver-1.8.3/tests/test_api.py`

 * *Files identical despite different names*

