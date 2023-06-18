# Comparing `tmp/networkcalculator-1.3.2.tar.gz` & `tmp/networkcalculator-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networkcalculator-1.3.2.tar", last modified: Sun Jun 18 23:08:25 2023, max compression
+gzip compressed data, was "networkcalculator-1.3.3.tar", last modified: Sun Jun 18 23:24:51 2023, max compression
```

## Comparing `networkcalculator-1.3.2.tar` & `networkcalculator-1.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 23:08:25.059551 networkcalculator-1.3.2/
--rw-rw-rw-   0        0        0     1094 2023-06-18 18:29:24.000000 networkcalculator-1.3.2/LICENSE
--rw-rw-rw-   0        0        0      687 2023-06-18 23:08:25.058550 networkcalculator-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    12602 2023-06-18 21:13:54.000000 networkcalculator-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 23:08:25.058550 networkcalculator-1.3.2/networkcalculator.egg-info/
--rw-rw-rw-   0        0        0      687 2023-06-18 23:08:25.000000 networkcalculator-1.3.2/networkcalculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-18 23:08:25.000000 networkcalculator-1.3.2/networkcalculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 23:08:25.000000 networkcalculator-1.3.2/networkcalculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 23:08:25.000000 networkcalculator-1.3.2/networkcalculator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 23:08:25.059551 networkcalculator-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-06-18 23:07:49.000000 networkcalculator-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 23:24:51.706348 networkcalculator-1.3.3/
+-rw-rw-rw-   0        0        0     1094 2023-06-18 18:29:24.000000 networkcalculator-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0      739 2023-06-18 23:24:51.705349 networkcalculator-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    12602 2023-06-18 21:13:54.000000 networkcalculator-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 23:24:51.704350 networkcalculator-1.3.3/networkcalculator.egg-info/
+-rw-rw-rw-   0        0        0      739 2023-06-18 23:24:51.000000 networkcalculator-1.3.3/networkcalculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-18 23:24:51.000000 networkcalculator-1.3.3/networkcalculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 23:24:51.000000 networkcalculator-1.3.3/networkcalculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 23:24:51.000000 networkcalculator-1.3.3/networkcalculator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 23:24:51.706348 networkcalculator-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      892 2023-06-18 23:24:48.000000 networkcalculator-1.3.3/setup.py
```

### Comparing `networkcalculator-1.3.2/LICENSE` & `networkcalculator-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `networkcalculator-1.3.2/PKG-INFO` & `networkcalculator-1.3.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: networkcalculator
-Version: 1.3.2
+Version: 1.3.3
 Author: Ray Bernard
 Author-email: ray.bernard@outlook.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Network calculator is a Python library that allows you to calculate the bandwidth and subnets
```

### Comparing `networkcalculator-1.3.2/README.md` & `networkcalculator-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `networkcalculator-1.3.2/networkcalculator.egg-info/PKG-INFO` & `networkcalculator-1.3.3/networkcalculator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: networkcalculator
-Version: 1.3.2
+Version: 1.3.3
 Author: Ray Bernard
 Author-email: ray.bernard@outlook.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Network calculator is a Python library that allows you to calculate the bandwidth and subnets
```

### Comparing `networkcalculator-1.3.2/setup.py` & `networkcalculator-1.3.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from setuptools import setup, find_packages
 
-
-
-
 setup(
     name='networkcalculator',
-    version='1.3.2',
+    version='1.3.3',
     author='Ray Bernard',
     author_email='ray.bernard@outlook.com',
     packages=find_packages(),
     long_description='Network calculator is a Python library that allows you to calculate the bandwidth and subnets',
     long_description_content_type='text/x-rst',
     setup_requires=['wheel'],
 
@@ -17,10 +14,12 @@
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+
         'Operating System :: OS Independent',
     ],
 )
```

