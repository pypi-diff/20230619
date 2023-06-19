# Comparing `tmp/pyvolsuggester-1.1.0.tar.gz` & `tmp/pyvolsuggester-1.1.1.tar.gz`

## Comparing `pyvolsuggester-1.1.0.tar` & `pyvolsuggester-1.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pyvolsuggester-1.1.0/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-1.1.0/License.txt
--rw-r--r--   0        0        0     9989 2020-02-02 00:00:00.000000 pyvolsuggester-1.1.0/README.md
--rw-r--r--   0        0        0     8537 2020-02-02 00:00:00.000000 pyvolsuggester-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    12414 2020-02-02 00:00:00.000000 pyvolsuggester-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pyvolsuggester-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-1.1.1/License.txt
+-rw-r--r--   0        0        0    10077 2020-02-02 00:00:00.000000 pyvolsuggester-1.1.1/README.md
+-rw-r--r--   0        0        0     8537 2020-02-02 00:00:00.000000 pyvolsuggester-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12498 2020-02-02 00:00:00.000000 pyvolsuggester-1.1.1/PKG-INFO
```

### Comparing `pyvolsuggester-1.1.0/License.txt` & `pyvolsuggester-1.1.1/License.txt`

 * *Files identical despite different names*

### Comparing `pyvolsuggester-1.1.0/README.md` & `pyvolsuggester-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,18 @@
 - In order to use this package, one need to ensure the following requirements:
     - Python 3.7 or later installed on your machine.
     - ffmpeg pacakge must be installed and its PATH must be added to Environment variables.
 
 ****
 
 ### 📌Package Usage
+This command will import the `PyVolSuggester` module.
+```
+import PyVolSuggester
+```
 This command will install all the uninstalled required libraries used in script.
 ```
 from PyVolSuggester import Suggester
 ```
 This will prompt user for input of `ffmpeg` path and audio file selection(.wav format).
 ```
 Suggester.main()
```

### Comparing `pyvolsuggester-1.1.0/pyproject.toml` & `pyvolsuggester-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 name = "PyVolSuggester"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.1.0"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
+version = "1.1.1"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Does audio feature extraction and suggest the feasible volumne for better feeling and experience."  # Optional ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is an optional longer description of your project that represents
```

### Comparing `pyvolsuggester-1.1.0/PKG-INFO` & `pyvolsuggester-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVolSuggester
-Version: 1.1.0
+Version: 1.1.1
 Summary: Does audio feature extraction and suggest the feasible volumne for better feeling and experience.
 Project-URL: Homepage, https://github.com/akash-rajak/PyVolSuggester
 Project-URL: Bug Reports, https://github.com/akash-rajak/PyVolSuggester/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, https://saythanks.io/to/aakashrajak02
 Project-URL: Source, https://github.com/akash-rajak/PyVolSuggester
 Author-email: Akash Rajak <aakashrajak02@gmail.com>
@@ -174,14 +174,18 @@
 - In order to use this package, one need to ensure the following requirements:
     - Python 3.7 or later installed on your machine.
     - ffmpeg pacakge must be installed and its PATH must be added to Environment variables.
 
 ****
 
 ### 📌Package Usage
+This command will import the `PyVolSuggester` module.
+```
+import PyVolSuggester
+```
 This command will install all the uninstalled required libraries used in script.
 ```
 from PyVolSuggester import Suggester
 ```
 This will prompt user for input of `ffmpeg` path and audio file selection(.wav format).
 ```
 Suggester.main()
```

