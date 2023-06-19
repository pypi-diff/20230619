# Comparing `tmp/xlf-merge-0.1.2.tar.gz` & `tmp/xlf-merge-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlf-merge-0.1.2.tar", last modified: Tue Feb  8 17:48:35 2022, max compression
+gzip compressed data, was "xlf-merge-0.1.5.tar", last modified: Mon Jun 19 02:58:36 2023, max compression
```

## Comparing `xlf-merge-0.1.2.tar` & `xlf-merge-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-08 17:48:35.233866 xlf-merge-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)       69 2022-02-08 17:47:39.000000 xlf-merge-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2697 2022-02-08 17:48:35.233866 xlf-merge-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1105 2022-02-08 17:47:39.000000 xlf-merge-0.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-02-08 17:48:35.233866 xlf-merge-0.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1659 2022-02-08 17:47:39.000000 xlf-merge-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-08 17:48:35.233866 xlf-merge-0.1.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-08 17:47:39.000000 xlf-merge-0.1.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-08 17:48:35.233866 xlf-merge-0.1.2/xlf_merge/
--rw-rw-rw-   0 root         (0) root         (0)     5383 2022-02-08 17:47:39.000000 xlf-merge-0.1.2/xlf_merge/XlfParser.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-02-08 17:47:39.000000 xlf-merge-0.1.2/xlf_merge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2022-02-08 17:47:39.000000 xlf-merge-0.1.2/xlf_merge/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-08 17:48:35.233866 xlf-merge-0.1.2/xlf_merge/bin/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-08 17:47:39.000000 xlf-merge-0.1.2/xlf_merge/bin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5067 2022-02-08 17:47:39.000000 xlf-merge-0.1.2/xlf_merge/bin/xlf_merge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-08 17:48:35.233866 xlf-merge-0.1.2/xlf_merge.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2697 2022-02-08 17:48:35.000000 xlf-merge-0.1.2/xlf_merge.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      368 2022-02-08 17:48:35.000000 xlf-merge-0.1.2/xlf_merge.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-08 17:48:35.000000 xlf-merge-0.1.2/xlf_merge.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2022-02-08 17:48:35.000000 xlf-merge-0.1.2/xlf_merge.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-02-08 17:48:35.000000 xlf-merge-0.1.2/xlf_merge.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-02-08 17:48:35.000000 xlf-merge-0.1.2/xlf_merge.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 02:58:36.065025 xlf-merge-0.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)    35148 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2137 2023-06-19 02:58:36.065025 xlf-merge-0.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1105 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 02:58:36.065025 xlf-merge-0.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 02:58:36.065025 xlf-merge-0.1.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 02:58:36.065025 xlf-merge-0.1.5/xlf_merge/
+-rw-rw-rw-   0 root         (0) root         (0)     5383 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/xlf_merge/XlfParser.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/xlf_merge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/xlf_merge/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 02:58:36.065025 xlf-merge-0.1.5/xlf_merge/bin/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/xlf_merge/bin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5067 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/xlf_merge/bin/xlf_merge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 02:58:36.065025 xlf-merge-0.1.5/xlf_merge.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2137 2023-06-19 02:58:36.000000 xlf-merge-0.1.5/xlf_merge.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      376 2023-06-19 02:58:36.000000 xlf-merge-0.1.5/xlf_merge.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 02:58:36.000000 xlf-merge-0.1.5/xlf_merge.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-19 02:58:36.000000 xlf-merge-0.1.5/xlf_merge.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-19 02:58:36.000000 xlf-merge-0.1.5/xlf_merge.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-19 02:58:36.000000 xlf-merge-0.1.5/xlf_merge.egg-info/top_level.txt
```

### Comparing `xlf-merge-0.1.2/PKG-INFO` & `xlf-merge-0.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,16 @@
 Metadata-Version: 2.1
 Name: xlf-merge
-Version: 0.1.2
+Version: 0.1.5
 Summary: APP for merging xlf translation files
 Home-page: https://github.com/Salamek/xlf-merge
 Author: Adam Schubert
 Author-email: adam.schubert@sg1-game.net
 License: GPL-3.0 
 Project-URL: Release notes, https://github.com/Salamek/xlf-merge/releases
-Description: # xlf-merge
-        
-        Tool to merge XLF translation files.
-        And it can also find dupes in XLF files.
-        
-        
-        ## Installation
-        
-        ### Using PIP
-        
-        ```bash
-        pip install xlf-merge
-        ```
-        
-        ### Using package Debian/Archlinux package
-        
-        Go to https://repository.salamek.cz/ to see how to setup access to my public repository, then just do:
-        
-        debian
-        ```bash
-        apt update && apt install xlf-merge
-        ```
-        
-        archlinux
-        ```bash
-        pacman -Sy xlf-merge
-        ```
-        
-        ## Usage
-        
-        ### Merging
-        
-        ```bash
-        xlf-merge merge <old_translation_file> <new_translation_file> <output_file> --method='source/id'
-        ```
-        
-        Merge files by source:
-        
-        ```bash
-        xlf-merge merge messages.cs.xlf.old messages.xlf messages.cs.xlf --method='source'
-        ```
-        
-        Merge files by id:
-        
-        ```bash
-        xlf-merge merge messages.cs.xlf.old messages.xlf messages.cs.xlf --method='id'
-        ```
-        
-        ### Finding dupes
-        ```
-        xlf-merge dupes <file_to_check> --method='source/id/target'
-        ```
-        
-        Finding dupes by source:
-        
-        ```
-        xlf-merge dupes messages.cs.xlf --method='source'
-        ```
-        
-        Finding dupes by id:
-        
-        ```
-        xlf-merge dupes messages.cs.xlf --method='id'
-        ```
-        
-        Finding dupes by target:
-        
-        ```
-        xlf-merge dupes messages.cs.xlf --method='target'
-        ```
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -89,7 +18,79 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# xlf-merge
+
+Tool to merge XLF translation files.
+And it can also find dupes in XLF files.
+
+
+## Installation
+
+### Using PIP
+
+```bash
+pip install xlf-merge
+```
+
+### Using package Debian/Archlinux package
+
+Go to https://repository.salamek.cz/ to see how to setup access to my public repository, then just do:
+
+debian
+```bash
+apt update && apt install xlf-merge
+```
+
+archlinux
+```bash
+pacman -Sy xlf-merge
+```
+
+## Usage
+
+### Merging
+
+```bash
+xlf-merge merge <old_translation_file> <new_translation_file> <output_file> --method='source/id'
+```
+
+Merge files by source:
+
+```bash
+xlf-merge merge messages.cs.xlf.old messages.xlf messages.cs.xlf --method='source'
+```
+
+Merge files by id:
+
+```bash
+xlf-merge merge messages.cs.xlf.old messages.xlf messages.cs.xlf --method='id'
+```
+
+### Finding dupes
+```
+xlf-merge dupes <file_to_check> --method='source/id/target'
+```
+
+Finding dupes by source:
+
+```
+xlf-merge dupes messages.cs.xlf --method='source'
+```
+
+Finding dupes by id:
+
+```
+xlf-merge dupes messages.cs.xlf --method='id'
+```
+
+Finding dupes by target:
+
+```
+xlf-merge dupes messages.cs.xlf --method='target'
+```
```

### Comparing `xlf-merge-0.1.2/README.md` & `xlf-merge-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `xlf-merge-0.1.2/setup.py` & `xlf-merge-0.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='xlf-merge',
-    version='0.1.2',
+    version='0.1.5',
     packages=find_packages(exclude=['tests', 'tests.*']),
     package_data={'xlf_merge': ['py.typed']},
     install_requires=[
         'docopt',
         'lxml'
     ],
     url='https://github.com/Salamek/xlf-merge',
```

### Comparing `xlf-merge-0.1.2/xlf_merge/XlfParser.py` & `xlf-merge-0.1.5/xlf_merge/XlfParser.py`

 * *Files identical despite different names*

### Comparing `xlf-merge-0.1.2/xlf_merge/bin/xlf_merge.py` & `xlf-merge-0.1.5/xlf_merge/bin/xlf_merge.py`

 * *Files identical despite different names*

### Comparing `xlf-merge-0.1.2/xlf_merge.egg-info/PKG-INFO` & `xlf-merge-0.1.5/xlf_merge.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,16 @@
 Metadata-Version: 2.1
 Name: xlf-merge
-Version: 0.1.2
+Version: 0.1.5
 Summary: APP for merging xlf translation files
 Home-page: https://github.com/Salamek/xlf-merge
 Author: Adam Schubert
 Author-email: adam.schubert@sg1-game.net
 License: GPL-3.0 
 Project-URL: Release notes, https://github.com/Salamek/xlf-merge/releases
-Description: # xlf-merge
-        
-        Tool to merge XLF translation files.
-        And it can also find dupes in XLF files.
-        
-        
-        ## Installation
-        
-        ### Using PIP
-        
-        ```bash
-        pip install xlf-merge
-        ```
-        
-        ### Using package Debian/Archlinux package
-        
-        Go to https://repository.salamek.cz/ to see how to setup access to my public repository, then just do:
-        
-        debian
-        ```bash
-        apt update && apt install xlf-merge
-        ```
-        
-        archlinux
-        ```bash
-        pacman -Sy xlf-merge
-        ```
-        
-        ## Usage
-        
-        ### Merging
-        
-        ```bash
-        xlf-merge merge <old_translation_file> <new_translation_file> <output_file> --method='source/id'
-        ```
-        
-        Merge files by source:
-        
-        ```bash
-        xlf-merge merge messages.cs.xlf.old messages.xlf messages.cs.xlf --method='source'
-        ```
-        
-        Merge files by id:
-        
-        ```bash
-        xlf-merge merge messages.cs.xlf.old messages.xlf messages.cs.xlf --method='id'
-        ```
-        
-        ### Finding dupes
-        ```
-        xlf-merge dupes <file_to_check> --method='source/id/target'
-        ```
-        
-        Finding dupes by source:
-        
-        ```
-        xlf-merge dupes messages.cs.xlf --method='source'
-        ```
-        
-        Finding dupes by id:
-        
-        ```
-        xlf-merge dupes messages.cs.xlf --method='id'
-        ```
-        
-        Finding dupes by target:
-        
-        ```
-        xlf-merge dupes messages.cs.xlf --method='target'
-        ```
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -89,7 +18,79 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# xlf-merge
+
+Tool to merge XLF translation files.
+And it can also find dupes in XLF files.
+
+
+## Installation
+
+### Using PIP
+
+```bash
+pip install xlf-merge
+```
+
+### Using package Debian/Archlinux package
+
+Go to https://repository.salamek.cz/ to see how to setup access to my public repository, then just do:
+
+debian
+```bash
+apt update && apt install xlf-merge
+```
+
+archlinux
+```bash
+pacman -Sy xlf-merge
+```
+
+## Usage
+
+### Merging
+
+```bash
+xlf-merge merge <old_translation_file> <new_translation_file> <output_file> --method='source/id'
+```
+
+Merge files by source:
+
+```bash
+xlf-merge merge messages.cs.xlf.old messages.xlf messages.cs.xlf --method='source'
+```
+
+Merge files by id:
+
+```bash
+xlf-merge merge messages.cs.xlf.old messages.xlf messages.cs.xlf --method='id'
+```
+
+### Finding dupes
+```
+xlf-merge dupes <file_to_check> --method='source/id/target'
+```
+
+Finding dupes by source:
+
+```
+xlf-merge dupes messages.cs.xlf --method='source'
+```
+
+Finding dupes by id:
+
+```
+xlf-merge dupes messages.cs.xlf --method='id'
+```
+
+Finding dupes by target:
+
+```
+xlf-merge dupes messages.cs.xlf --method='target'
+```
```

