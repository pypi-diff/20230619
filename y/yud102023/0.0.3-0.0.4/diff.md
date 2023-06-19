# Comparing `tmp/yud102023-0.0.3.tar.gz` & `tmp/yud102023-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yud102023-0.0.3.tar", last modified: Mon Jun 19 00:45:25 2023, max compression
+gzip compressed data, was "yud102023-0.0.4.tar", last modified: Mon Jun 19 11:13:48 2023, max compression
```

## Comparing `yud102023-0.0.3.tar` & `yud102023-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:45:25.636767 yud102023-0.0.3/
--rw-r--r--   0 tomereliel   (501) staff       (20)     1054 2023-06-18 22:55:32.000000 yud102023-0.0.3/LICENSE
--rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 00:45:25.636611 yud102023-0.0.3/PKG-INFO
--rw-r--r--   0 tomereliel   (501) staff       (20)       49 2023-06-18 22:56:17.000000 yud102023-0.0.3/README.md
--rw-r--r--   0 tomereliel   (501) staff       (20)      633 2023-06-19 00:45:13.000000 yud102023-0.0.3/pyproject.toml
--rw-r--r--   0 tomereliel   (501) staff       (20)       38 2023-06-19 00:45:25.636819 yud102023-0.0.3/setup.cfg
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:45:25.634178 yud102023-0.0.3/src/
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:45:25.635678 yud102023-0.0.3/src/yud102023/
--rw-r--r--   0 tomereliel   (501) staff       (20)    29940 2023-06-18 23:00:03.000000 yud102023-0.0.3/src/yud102023/goodbye.py
--rw-r--r--   0 tomereliel   (501) staff       (20)        0 2023-06-14 14:29:08.000000 yud102023-0.0.3/src/yud102023/init.py
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:45:25.636374 yud102023-0.0.3/src/yud102023.egg-info/
--rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 00:45:25.000000 yud102023-0.0.3/src/yud102023.egg-info/PKG-INFO
--rw-r--r--   0 tomereliel   (501) staff       (20)      263 2023-06-19 00:45:25.000000 yud102023-0.0.3/src/yud102023.egg-info/SOURCES.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)        1 2023-06-19 00:45:25.000000 yud102023-0.0.3/src/yud102023.egg-info/dependency_links.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)        9 2023-06-19 00:45:25.000000 yud102023-0.0.3/src/yud102023.egg-info/requires.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)       10 2023-06-19 00:45:25.000000 yud102023-0.0.3/src/yud102023.egg-info/top_level.txt
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 11:13:48.460470 yud102023-0.0.4/
+-rw-r--r--   0 tomereliel   (501) staff       (20)     1054 2023-06-18 22:55:32.000000 yud102023-0.0.4/LICENSE
+-rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 11:13:48.460341 yud102023-0.0.4/PKG-INFO
+-rw-r--r--   0 tomereliel   (501) staff       (20)       49 2023-06-18 22:56:17.000000 yud102023-0.0.4/README.md
+-rw-r--r--   0 tomereliel   (501) staff       (20)      633 2023-06-19 11:13:41.000000 yud102023-0.0.4/pyproject.toml
+-rw-r--r--   0 tomereliel   (501) staff       (20)       38 2023-06-19 11:13:48.460512 yud102023-0.0.4/setup.cfg
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 11:13:48.457886 yud102023-0.0.4/src/
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 11:13:48.459419 yud102023-0.0.4/src/yud102023/
+-rw-r--r--   0 tomereliel   (501) staff       (20)    30029 2023-06-19 11:12:05.000000 yud102023-0.0.4/src/yud102023/goodbye.py
+-rw-r--r--   0 tomereliel   (501) staff       (20)        0 2023-06-14 14:29:08.000000 yud102023-0.0.4/src/yud102023/init.py
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 11:13:48.460122 yud102023-0.0.4/src/yud102023.egg-info/
+-rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 11:13:48.000000 yud102023-0.0.4/src/yud102023.egg-info/PKG-INFO
+-rw-r--r--   0 tomereliel   (501) staff       (20)      263 2023-06-19 11:13:48.000000 yud102023-0.0.4/src/yud102023.egg-info/SOURCES.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)        1 2023-06-19 11:13:48.000000 yud102023-0.0.4/src/yud102023.egg-info/dependency_links.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)        9 2023-06-19 11:13:48.000000 yud102023-0.0.4/src/yud102023.egg-info/requires.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)       10 2023-06-19 11:13:48.000000 yud102023-0.0.4/src/yud102023.egg-info/top_level.txt
```

### Comparing `yud102023-0.0.3/LICENSE` & `yud102023-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yud102023-0.0.3/PKG-INFO` & `yud102023-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yud102023
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small creactive goodbye project for my students
 Author-email: Tomereliel <tomereliel.dev@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yud102023-0.0.3/pyproject.toml` & `yud102023-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "yud102023"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Tomereliel", email="tomereliel.dev@gmail.com" },
 ]
 description = "A small creactive goodbye project for my students"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `yud102023-0.0.3/src/yud102023/goodbye.py` & `yud102023-0.0.4/src/yud102023/goodbye.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,22 +94,23 @@
 
 HEB_BLESS = {"oren":'''
 אורן היקר,
 היה לי כיף ללמד אותך השנה.
 אתה אדם נעים וצנוע שכיף להיות לידו.
 
 עבדת קשה השנה וניכר שלמדת והתפתחת.
+תמשיך עם העבודה הקשה ואין לי ספק שבסוף תשתלם.
 המון בהצלחה בהמשך!
 
 תומר אליאל.
 רשתות, מגשימים, 2023.
 ''',
 'eliya':'''
 אליה היקרה,
-אין ספק שאת מוסיפה לכיתה גוון ייחודי והכרחי.
+אין ספק שאת מוסיפה לכיתה גוון ייחודי ויפה.
 הפרפקציוניזם שלך והמוטיבציה בשמיים מעוררים קנאה והשראה - תשמרי על תכונות אלו, אין ספק שהן יביאו אותך לגדולות.
 
 תישארי ייחודית וחריפה כמו שאת,
 דומיננטית ובולטת.
 בהערכה רבה,
 תומר אליאל.
 רשתות, מגשימים, 2023.
@@ -162,15 +163,15 @@
 המוטיבציה שלך מעוררת השראה - תשמרי עליה!
 בהערכה רבה והצלחה בהמשך,
 תומר אליאל.
 רשתות, מגשימים 2023.
 ''',
 'daniel':'''
 דניאל היקר!
-אין דבר שאני יותר אוהב מלהגיע לכיתה ולראות אותך מחכה לי שם או מגיע ביחד איתי ואז אנחנו מנהלים שיחה קצרה על איך הולך בלימודים ובתוכנית.
+אין דבר שאני יותר אוהב מלהגיע לכיתה ולראות אותך מחכה לי שם ראשון או מגיע ביחד איתי ואז אנחנו מנהלים שיחה קצרה על איך הולך בלימודים ובתוכנית.
 אתה חניך סופר חכם ועם זאת גם צנוע ומאוד נעים לבריות.
 אתה חבר טוב וברור לי שבגלל זה אתה אהוב בכיתה.
 
 הדרך השקטה בה אתה עושה דברים מעוררת הערצה - תמשיך כך!
 מאחל לך המון הצלחה בהמשך,
 תומר אליאל.
 רשתות, מגשימים 2023.
```

### Comparing `yud102023-0.0.3/src/yud102023.egg-info/PKG-INFO` & `yud102023-0.0.4/src/yud102023.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yud102023
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small creactive goodbye project for my students
 Author-email: Tomereliel <tomereliel.dev@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

