# Comparing `tmp/yud102023-0.0.4.tar.gz` & `tmp/yud102023-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yud102023-0.0.4.tar", last modified: Mon Jun 19 11:13:48 2023, max compression
+gzip compressed data, was "yud102023-0.0.5.tar", last modified: Mon Jun 19 12:05:28 2023, max compression
```

## Comparing `yud102023-0.0.4.tar` & `yud102023-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 11:13:48.460470 yud102023-0.0.4/
--rw-r--r--   0 tomereliel   (501) staff       (20)     1054 2023-06-18 22:55:32.000000 yud102023-0.0.4/LICENSE
--rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 11:13:48.460341 yud102023-0.0.4/PKG-INFO
--rw-r--r--   0 tomereliel   (501) staff       (20)       49 2023-06-18 22:56:17.000000 yud102023-0.0.4/README.md
--rw-r--r--   0 tomereliel   (501) staff       (20)      633 2023-06-19 11:13:41.000000 yud102023-0.0.4/pyproject.toml
--rw-r--r--   0 tomereliel   (501) staff       (20)       38 2023-06-19 11:13:48.460512 yud102023-0.0.4/setup.cfg
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 11:13:48.457886 yud102023-0.0.4/src/
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 11:13:48.459419 yud102023-0.0.4/src/yud102023/
--rw-r--r--   0 tomereliel   (501) staff       (20)    30029 2023-06-19 11:12:05.000000 yud102023-0.0.4/src/yud102023/goodbye.py
--rw-r--r--   0 tomereliel   (501) staff       (20)        0 2023-06-14 14:29:08.000000 yud102023-0.0.4/src/yud102023/init.py
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 11:13:48.460122 yud102023-0.0.4/src/yud102023.egg-info/
--rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 11:13:48.000000 yud102023-0.0.4/src/yud102023.egg-info/PKG-INFO
--rw-r--r--   0 tomereliel   (501) staff       (20)      263 2023-06-19 11:13:48.000000 yud102023-0.0.4/src/yud102023.egg-info/SOURCES.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)        1 2023-06-19 11:13:48.000000 yud102023-0.0.4/src/yud102023.egg-info/dependency_links.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)        9 2023-06-19 11:13:48.000000 yud102023-0.0.4/src/yud102023.egg-info/requires.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)       10 2023-06-19 11:13:48.000000 yud102023-0.0.4/src/yud102023.egg-info/top_level.txt
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 12:05:28.286959 yud102023-0.0.5/
+-rw-r--r--   0 tomereliel   (501) staff       (20)     1054 2023-06-18 22:55:32.000000 yud102023-0.0.5/LICENSE
+-rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 12:05:28.286798 yud102023-0.0.5/PKG-INFO
+-rw-r--r--   0 tomereliel   (501) staff       (20)       49 2023-06-18 22:56:17.000000 yud102023-0.0.5/README.md
+-rw-r--r--   0 tomereliel   (501) staff       (20)      633 2023-06-19 12:05:22.000000 yud102023-0.0.5/pyproject.toml
+-rw-r--r--   0 tomereliel   (501) staff       (20)       38 2023-06-19 12:05:28.287005 yud102023-0.0.5/setup.cfg
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 12:05:28.284318 yud102023-0.0.5/src/
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 12:05:28.285594 yud102023-0.0.5/src/yud102023/
+-rw-r--r--   0 tomereliel   (501) staff       (20)    30062 2023-06-19 12:04:41.000000 yud102023-0.0.5/src/yud102023/goodbye.py
+-rw-r--r--   0 tomereliel   (501) staff       (20)        0 2023-06-14 14:29:08.000000 yud102023-0.0.5/src/yud102023/init.py
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 12:05:28.286583 yud102023-0.0.5/src/yud102023.egg-info/
+-rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 12:05:28.000000 yud102023-0.0.5/src/yud102023.egg-info/PKG-INFO
+-rw-r--r--   0 tomereliel   (501) staff       (20)      263 2023-06-19 12:05:28.000000 yud102023-0.0.5/src/yud102023.egg-info/SOURCES.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)        1 2023-06-19 12:05:28.000000 yud102023-0.0.5/src/yud102023.egg-info/dependency_links.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)        9 2023-06-19 12:05:28.000000 yud102023-0.0.5/src/yud102023.egg-info/requires.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)       10 2023-06-19 12:05:28.000000 yud102023-0.0.5/src/yud102023.egg-info/top_level.txt
```

### Comparing `yud102023-0.0.4/LICENSE` & `yud102023-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yud102023-0.0.4/PKG-INFO` & `yud102023-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yud102023
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small creactive goodbye project for my students
 Author-email: Tomereliel <tomereliel.dev@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yud102023-0.0.4/pyproject.toml` & `yud102023-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "yud102023"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Tomereliel", email="tomereliel.dev@gmail.com" },
 ]
 description = "A small creactive goodbye project for my students"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `yud102023-0.0.4/src/yud102023/goodbye.py` & `yud102023-0.0.5/src/yud102023/goodbye.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,15 +411,15 @@
         sleep(1)
         print("Oh GREAT! it's you again....")
         sleep(3)
         clear()
         ans = input("IF YOU ARE REALLY MAGSHIMIM STUDENT - WHO IS THE BEST TEACHER YOU EVER MET?  \n")
         while ans.lower() != "tomer":
           clear()
-          if(ans.lower() == "Viki" or ans.lower() == "Vicki" or ans.lower() == "Vicky"):
+          if(ans.lower() == "viki" or ans.lower() == "vicki" or ans.lower() == "vicky"):
             ans = input("WRONG ANSWER!\nNice try... Vicky...\nI ASKED\nWHO IS THE BEST TEACHER\nYOU EVER MET?  \n")
           else:
             ans = input("WHAT YOU SAID?!?!?!  WRONG ANSWER!\nI ASKED\nWHO IS THE BEST TEACHER\nYOU EVER MET?  \n")
         clear()
         
         print("Very nice... very nice...\nTomer is the best indeed")
         sleep(5)
@@ -434,15 +434,15 @@
         student = input("\n\nWHO ARE YOU?\n")
         while student.lower() not in STUDENTS.keys():
           student = input("I SAID - WHO ARE YOU???  WHAT IS YOUR NAME????\n")
         clear()
         print("Ohh...")
         sleep(2)
         clear()
-        print("Is it really you "+student+"?")
+        print("Is it really you "+student[0].upper() + student[1:].lower()+"?")
         sleep(3)
         clear()
         print("I guess its time to say goodbye...")
         sleep(4)
         clear()
         #STUDENTS[student.lower()]()
         bless(student.lower())
```

### Comparing `yud102023-0.0.4/src/yud102023.egg-info/PKG-INFO` & `yud102023-0.0.5/src/yud102023.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yud102023
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small creactive goodbye project for my students
 Author-email: Tomereliel <tomereliel.dev@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

