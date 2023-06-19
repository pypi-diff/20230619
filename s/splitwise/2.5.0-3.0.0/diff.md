# Comparing `tmp/splitwise-2.5.0.tar.gz` & `tmp/splitwise-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splitwise-2.5.0.tar", last modified: Sat Dec 10 23:08:17 2022, max compression
+gzip compressed data, was "splitwise-3.0.0.tar", last modified: Mon Jun 19 21:39:48 2023, max compression
```

## Comparing `splitwise-2.5.0.tar` & `splitwise-3.0.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 23:08:17.537402 splitwise-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2022-12-10 23:08:09.000000 splitwise-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20044 2022-12-10 23:08:17.537402 splitwise-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18837 2022-12-10 23:08:09.000000 splitwise-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 23:08:17.533402 splitwise-2.5.0/e2e-tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 23:08:09.000000 splitwise-2.5.0/e2e-tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2022-12-10 23:08:09.000000 splitwise-2.5.0/e2e-tests/test_expense.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2022-12-10 23:08:09.000000 splitwise-2.5.0/e2e-tests/test_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2022-12-10 23:08:17.537402 splitwise-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2022-12-10 23:08:09.000000 splitwise-2.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 23:08:17.533402 splitwise-2.5.0/splitwise/
--rw-r--r--   0 runner    (1001) docker     (123)    31318 2022-12-10 23:08:09.000000 splitwise-2.5.0/splitwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2022-12-10 23:08:09.000000 splitwise-2.5.0/splitwise/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2022-12-10 23:08:09.000000 splitwise-2.5.0/splitwise/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2022-12-10 23:08:09.000000 splitwise-2.5.0/splitwise/category.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2022-12-10 23:08:09.000000 splitwise-2.5.0/splitwise/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2022-12-10 23:08:09.000000 splitwise-2.5.0/splitwise/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2022-12-10 23:08:09.000000 splitwise-2.5.0/splitwise/debt.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2022-12-10 23:08:09.000000 splitwise-2.5.0/splitwise/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2022-12-10 23:08:09.000000 splitwise-2.5.0/splitwise/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    14324 2022-12-10 23:08:09.000000 splitwise-2.5.0/splitwise/expense.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2022-12-10 23:08:09.000000 splitwise-2.5.0/splitwise/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2022-12-10 23:08:09.000000 splitwise-2.5.0/splitwise/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2022-12-10 23:08:09.000000 splitwise-2.5.0/splitwise/picture.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2022-12-10 23:08:09.000000 splitwise-2.5.0/splitwise/receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2022-12-10 23:08:09.000000 splitwise-2.5.0/splitwise/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 23:08:17.533402 splitwise-2.5.0/splitwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20044 2022-12-10 23:08:17.000000 splitwise-2.5.0/splitwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2022-12-10 23:08:17.000000 splitwise-2.5.0/splitwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-10 23:08:17.000000 splitwise-2.5.0/splitwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-10 23:08:17.000000 splitwise-2.5.0/splitwise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-10 23:08:17.000000 splitwise-2.5.0/splitwise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 23:08:17.537402 splitwise-2.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_addUserToGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_createComment.py
--rw-r--r--   0 runner    (1001) docker     (123)    20966 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_createExpense.py
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_createGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_deleteExpense.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_deleteGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19960 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_getCategories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_getComments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_getCurrencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_getCurrentUser.py
--rw-r--r--   0 runner    (1001) docker     (123)    24676 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_getExpense.py
--rw-r--r--   0 runner    (1001) docker     (123)    18255 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_getExpenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_getFriends.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_getGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    20850 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_getGroups.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2375 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_getNotifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_getUser.py
--rw-r--r--   0 runner    (1001) docker     (123)    22096 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_updateExpense.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2022-12-10 23:08:09.000000 splitwise-2.5.0/tests/test_updateUser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:39:48.348048 splitwise-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-19 21:39:39.000000 splitwise-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20210 2023-06-19 21:39:48.348048 splitwise-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-06-19 21:39:39.000000 splitwise-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:39:48.344048 splitwise-3.0.0/e2e-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:39:39.000000 splitwise-3.0.0/e2e-tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-19 21:39:39.000000 splitwise-3.0.0/e2e-tests/test_expense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-19 21:39:39.000000 splitwise-3.0.0/e2e-tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-19 21:39:48.348048 splitwise-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-19 21:39:39.000000 splitwise-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:39:48.344048 splitwise-3.0.0/splitwise/
+-rw-r--r--   0 runner    (1001) docker     (123)    32905 2023-06-19 21:39:39.000000 splitwise-3.0.0/splitwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-19 21:39:39.000000 splitwise-3.0.0/splitwise/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-19 21:39:39.000000 splitwise-3.0.0/splitwise/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-19 21:39:39.000000 splitwise-3.0.0/splitwise/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-19 21:39:39.000000 splitwise-3.0.0/splitwise/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-19 21:39:39.000000 splitwise-3.0.0/splitwise/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-19 21:39:39.000000 splitwise-3.0.0/splitwise/debt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-19 21:39:39.000000 splitwise-3.0.0/splitwise/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-19 21:39:39.000000 splitwise-3.0.0/splitwise/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14324 2023-06-19 21:39:39.000000 splitwise-3.0.0/splitwise/expense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-19 21:39:39.000000 splitwise-3.0.0/splitwise/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-19 21:39:39.000000 splitwise-3.0.0/splitwise/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-19 21:39:39.000000 splitwise-3.0.0/splitwise/picture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-19 21:39:39.000000 splitwise-3.0.0/splitwise/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-06-19 21:39:39.000000 splitwise-3.0.0/splitwise/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:39:48.344048 splitwise-3.0.0/splitwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20210 2023-06-19 21:39:48.000000 splitwise-3.0.0/splitwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-19 21:39:48.000000 splitwise-3.0.0/splitwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:39:48.000000 splitwise-3.0.0/splitwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-19 21:39:48.000000 splitwise-3.0.0/splitwise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 21:39:48.000000 splitwise-3.0.0/splitwise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:39:48.348048 splitwise-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_addUserToGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_createComment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20859 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_createExpense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_createGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_deleteExpense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_deleteGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19892 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_getCategories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_getComments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_getCurrencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_getCurrentUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24608 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_getExpense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_getExpenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_getFriends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15625 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_getGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20782 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_getGroups.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2307 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_getNotifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_getUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22016 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_updateExpense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-19 21:39:39.000000 splitwise-3.0.0/tests/test_updateUser.py
```

### Comparing `splitwise-2.5.0/LICENSE` & `splitwise-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `splitwise-2.5.0/PKG-INFO` & `splitwise-3.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 Metadata-Version: 2.1
 Name: splitwise
-Version: 2.5.0
+Version: 3.0.0
 Summary: Splitwise Python SDK
 Home-page: https://github.com/namaggarwal/splitwise
-Download-URL: https://github.com/namaggarwal/splitwise/tarball/v2.5.0
+Download-URL: https://github.com/namaggarwal/splitwise/tarball/v3.0.0
 Author: Naman Aggarwal
 Author-email: aggarwal.nam@gmail.com
 License: MIT
 Project-URL: Documentation, https://splitwise.readthedocs.io
 Project-URL: Source, https://github.com/namaggarwal/splitwise
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Splitwise Python SDK
 
 ![](https://pepy.tech/badge/splitwise)
@@ -34,15 +30,15 @@
 ![](https://img.shields.io/pypi/wheel/splitwise.svg)
 ![](https://img.shields.io/pypi/pyversions/splitwise.svg)
 
 This is the python sdk for Splitwise APIs. Pull requests and bug reports are welcomed.
 
 ## Latest Version
 
-The latest version of splitwise SDK is Splitwise-2.5.0
+The latest version of splitwise SDK is Splitwise-3.0.0
 
 ## Docs
 
 The detailed docs are hosted at [readthedocs.org](https://readthedocs.org/projects/splitwise/)
 
 ## Installation
 
@@ -217,15 +213,15 @@
 sObj = Splitwise(Config.consumer_key,Config.consumer_secret)
 sObj.setAccessToken(session['access_token'])
 sObj.getGroup(43233)
 ```
 
 ### Get Expenses
 
-You can use ```getExpenses(offset,limit,group_id,friendship_id,dated_after,dated_before,updated_after,updated_before)``` to get all the expenses of the current user based on filter options. It returns a list of ```Expense``` objects.
+You can use ```getExpenses(offset,limit,group_id,friend_id,dated_after,dated_before,updated_after,updated_before,visible)``` to get all the expenses of the current user based on filter options. It returns a list of ```Expense``` objects.
 
 ```python
 sObj = Splitwise(Config.consumer_key,Config.consumer_secret)
 sObj.setAccessToken(session['access_token'])
 sObj.getExpenses()
 ```
 
@@ -371,14 +367,30 @@
 expense.setCost('10')
 expense.setDescription("Updated description")
 
 expense, errors = sObj.updateExpense(expense)
 print(expense.getId())
 ```
 
+or update the fetched expense
+
+
+```python
+from splitwise.expense import Expense
+
+sObj = Splitwise(Config.consumer_key,Config.consumer_secret)
+sObj.setAccessToken(session['access_token'])
+
+expense, error = sObj.getExpense(12345)
+expense.setDescription("Updated description")
+
+expense, errors = sObj.updateExpense(expense)
+print(expense.getDescription())
+```
+
 ### Delete expense
 You can use ```deleteExpense(expense_id)``` to delete an existing expense.
 
 ```python
 
 sObj = Splitwise(Config.consumer_key,Config.consumer_secret)
 sObj.setAccessToken(session['access_token'])
```

### Comparing `splitwise-2.5.0/README.md` & `splitwise-3.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ![](https://img.shields.io/pypi/wheel/splitwise.svg)
 ![](https://img.shields.io/pypi/pyversions/splitwise.svg)
 
 This is the python sdk for Splitwise APIs. Pull requests and bug reports are welcomed.
 
 ## Latest Version
 
-The latest version of splitwise SDK is Splitwise-2.5.0
+The latest version of splitwise SDK is Splitwise-3.0.0
 
 ## Docs
 
 The detailed docs are hosted at [readthedocs.org](https://readthedocs.org/projects/splitwise/)
 
 ## Installation
 
@@ -188,15 +188,15 @@
 sObj = Splitwise(Config.consumer_key,Config.consumer_secret)
 sObj.setAccessToken(session['access_token'])
 sObj.getGroup(43233)
 ```
 
 ### Get Expenses
 
-You can use ```getExpenses(offset,limit,group_id,friendship_id,dated_after,dated_before,updated_after,updated_before)``` to get all the expenses of the current user based on filter options. It returns a list of ```Expense``` objects.
+You can use ```getExpenses(offset,limit,group_id,friend_id,dated_after,dated_before,updated_after,updated_before,visible)``` to get all the expenses of the current user based on filter options. It returns a list of ```Expense``` objects.
 
 ```python
 sObj = Splitwise(Config.consumer_key,Config.consumer_secret)
 sObj.setAccessToken(session['access_token'])
 sObj.getExpenses()
 ```
 
@@ -342,14 +342,30 @@
 expense.setCost('10')
 expense.setDescription("Updated description")
 
 expense, errors = sObj.updateExpense(expense)
 print(expense.getId())
 ```
 
+or update the fetched expense
+
+
+```python
+from splitwise.expense import Expense
+
+sObj = Splitwise(Config.consumer_key,Config.consumer_secret)
+sObj.setAccessToken(session['access_token'])
+
+expense, error = sObj.getExpense(12345)
+expense.setDescription("Updated description")
+
+expense, errors = sObj.updateExpense(expense)
+print(expense.getDescription())
+```
+
 ### Delete expense
 You can use ```deleteExpense(expense_id)``` to delete an existing expense.
 
 ```python
 
 sObj = Splitwise(Config.consumer_key,Config.consumer_secret)
 sObj.setAccessToken(session['access_token'])
```

### Comparing `splitwise-2.5.0/e2e-tests/test_expense.py` & `splitwise-3.0.0/e2e-tests/test_expense.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,17 +24,52 @@
         expense.setGroupId(19571167)
         expense.setSplitEqually()
         expense.setReceipt(receipt)
         # create expense
         expense, error = self.sObj.createExpense(expense)
         self.assertIsNone(error)
         self.assertIsNotNone(expense.getId())
+        # update expense
+        expense.setDescription("I am now new expense")
+        expense, error = self.sObj.updateExpense(expense)
+        self.assertIsNone(error)
+        self.assertIsNotNone(expense.getId())
+        self.assertEqual(expense.getDescription(), "I am now new expense")
+        # delete expense
+        success, error = self.sObj.deleteExpense(expense.getId())
+        self.assertIsNone(error)
+        self.assertTrue(success)
+
+    def test_expense_update_independent_flow(self):
+        receipt = os.path.join(os.path.dirname(os.path.realpath(__file__)), "receipt.jpg")
+        expense = Expense()
+        expense.setDescription("End2EndTest")
+        expense.setCost('10')
+        expense.setGroupId(19571167)
+        expense.setSplitEqually()
+        expense.setReceipt(receipt)
+        # create expense
+        expense, error = self.sObj.createExpense(expense)
+        self.assertIsNone(error)
+        self.assertIsNotNone(expense.getId())
+        # update expense
+        newexpense = Expense()
+        newexpense.setId(expense.getId())
+        newexpense.setDescription("End2EndTestUpdated")
+        expense, error = self.sObj.updateExpense(newexpense)
+        self.assertIsNone(error)
+        self.assertIsNotNone(expense.getId())
+        self.assertEqual(expense.getDescription(), "End2EndTestUpdated")
         # delete expense
         success, error = self.sObj.deleteExpense(expense.getId())
         self.assertIsNone(error)
         self.assertTrue(success)
 
     def test_expense_invalidkeys_fail(self):
         sObj = Splitwise('consumerkey', 'consumersecret', {"oauth_token": "sdsd", "oauth_token_secret": "sdsdd"})
         expense = Expense()
         with self.assertRaises(SplitwiseUnauthorizedException):
             sObj.createExpense(expense)
+
+    def test_get_expenses_success(self):
+        expenses = self.sObj.getExpenses(limit=2, group_id=19571167)
+        self.assertEqual(len(expenses), 2)
```

### Comparing `splitwise-2.5.0/e2e-tests/test_group.py` & `splitwise-3.0.0/e2e-tests/test_group.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,12 +21,18 @@
         group.setName("Splitwise_test_case")
         # Create Group
         group, error = self.sObj.createGroup(group)
         self.assertIsNotNone(group.getId())
         # Delete Group
         self.sObj.deleteGroup(group.getId())
 
+    def test_get_group(self):
+        group_id = 19571167
+        group = self.sObj.getGroup(group_id)
+        self.assertIsNotNone(group.getId())
+        self.assertEqual(len(group.getMembers()), 2)
+
     def test_group_invalidkeys_fail(self):
         sObj = Splitwise('consumerkey', 'consumersecret', {"oauth_token": "sdsd", "oauth_token_secret": "sdsdd"})
         group = Group()
         with self.assertRaises(SplitwiseUnauthorizedException):
             sObj.createGroup(group)
```

### Comparing `splitwise-2.5.0/splitwise/__init__.py` & `splitwise-3.0.0/splitwise/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,21 +265,28 @@
 
         if auth is None:
             if self.auth:
                 auth = self.auth
             elif self.api_key:
                 headers = {'Authorization': 'Bearer {}'.format(self.api_key)}
 
+        data = Splitwise.__handleUppercaseBoolean(data)
+
         requestObj = Request(method=method, url=url, headers=headers, data=data, auth=auth, files=files)
 
         prep_req = requestObj.prepare()
 
         with sessions.Session() as session:
             response = session.send(prep_req)
 
+        content = self.__handleResponse(response)
+
+        return content
+
+    def __handleResponse(self, response):
         if response.status_code == 200:
             if (response.content and hasattr(response.content, "decode")):
                 return response.content.decode("utf-8")
             return response.content
 
         if response.status_code == 401:
             raise SplitwiseUnauthorizedException("Please check your token or consumer id and secret", response=response)
@@ -458,46 +465,51 @@
 
         return group
 
     def getExpenses(self,
                     offset=None,
                     limit=None,
                     group_id=None,
-                    friendship_id=None,
+                    friend_id=None,
                     dated_after=None,
                     dated_before=None,
                     updated_after=None,
-                    updated_before=None
+                    updated_before=None,
+                    visible=None
                     ):
         """ Gets the list of expenses given parameters.
 
         Args:
             offset(int, optional): Number of expenses to be skipped
             limit(int, optional): Number of expenses to be returned
             group_id(long, optional): GroupID of the expenses
-            friendship_id(long, optional): FriendshipID of the expenses
+            friend_id(long, optional): ID of the friend for which expenses are required
             dated_after(str, optional): ISO 8601 Date time. Return expenses later that this date
             dated_before(str, optional): ISO 8601 Date time. Return expenses earlier than this date
             updated_after(str, optional): ISO 8601 Date time. Return expenses updated after this date
             updated_before(str, optional): ISO 8601 Date time. Return expenses updated before this date
+            visible(bool, optional): Boolean to show only not deleted expenses
 
         Returns:
             :obj:`list` of :obj:`splitwise.expense.Expense`: List of Expense
         """
 
         options = {}
 
         # Copy of the locals is created as if I directly work on
         # locals and create variables in the loop a dictionary changed
         # error is thrown. Refer to bug #2 on Github
         localCopy = dict(locals())
         params = localCopy.keys()
         for param in params:
             if param != 'self' and param != 'options' and localCopy.get(param) is not None:
-                options[param] = localCopy.get(param)
+                paramVal = localCopy.get(param)
+                options[param] = paramVal
+                if isinstance(paramVal, bool):
+                    options[param] = str(paramVal).lower()
 
         url = Splitwise.GET_EXPENSES_URL
 
         url += self.__prepareOptionsUrl(options)
         content = self.__makeRequest(url)
         content = json.loads(content)
         expenses = []
@@ -554,14 +566,15 @@
             expense_data["category_id"] = category.getId()
             del expense_data["category"]
 
         receipt = expense.getReceiptPath()
         files = None
         if receipt:
             files = {"receipt":  io.open(receipt, "rb")}
+            del expense_data["receiptPath"]
 
         content = self.__makeRequest(
             Splitwise.CREATE_EXPENSE_URL, "POST", expense_data, files=files)
         content = json.loads(content)
         expense = None
         errors = None
 
@@ -615,14 +628,28 @@
             expense_data["category_id"] = category.getId()
             del expense_data["category"]
 
         receipt = expense.getReceiptPath()
         files = None
         if receipt:
             files = {"receipt":  io.open(receipt, "rb")}
+            del expense_data["receiptPath"]
+
+        expense_data.pop("created_by", None)
+        expense_data.pop("repayments", None)
+        expense_data.pop("next_repeat", None)
+        expense_data.pop("comments_count", None)
+        expense_data.pop("updated_by", None)
+        expense_data.pop("transaction_confirmed", None)
+        expense_data.pop("deleted_at", None)
+        expense_data.pop("friendship_id", None)
+        expense_data.pop("expense_bundle_id", None)
+        expense_data.pop("updated_at", None)
+        expense_data.pop("deleted_by", None)
+        expense_data.pop("created_at", None)
 
         content = self.__makeRequest(
             Splitwise.UPDATE_EXPENSE_URL+"/"+str(expense_id), "POST", expense_data, files=files)
         content = json.loads(content)
         expense = None
         errors = None
 
@@ -785,20 +812,36 @@
         if 'errors' in content:
             if len(content['errors']) != 0:
                 errors = SplitwiseError(content['errors'])
 
         return success, errors
 
     @staticmethod
+    def __handleUppercaseBoolean(data):
+        # convert the uppercase True/False to lower
+        # Splitwise server considers False as true value
+        try:
+            if data is not None:
+                for key, val in data.items():
+                    if isinstance(val, bool):
+                        data[key] = str(val).lower()
+        except Exception:
+            pass
+
+        return data
+
+    @staticmethod
     def setUserArray(users, user_array):
         for count, user in enumerate(users):
             user_dict = user.__dict__
             for key in user_dict:
                 if key == "id":
                     gen_key = "user_id"
+                elif key == "picture":
+                    continue
                 else:
                     gen_key = key
                 user_array["users__" +
                            str(count) + "__" + gen_key] = user_dict[key]
 
     def getComments(self, expense_id):
         """
```

### Comparing `splitwise-2.5.0/splitwise/balance.py` & `splitwise-3.0.0/splitwise/balance.py`

 * *Files identical despite different names*

### Comparing `splitwise-2.5.0/splitwise/category.py` & `splitwise-3.0.0/splitwise/category.py`

 * *Files identical despite different names*

### Comparing `splitwise-2.5.0/splitwise/comment.py` & `splitwise-3.0.0/splitwise/comment.py`

 * *Files identical despite different names*

### Comparing `splitwise-2.5.0/splitwise/currency.py` & `splitwise-3.0.0/splitwise/currency.py`

 * *Files identical despite different names*

### Comparing `splitwise-2.5.0/splitwise/debt.py` & `splitwise-3.0.0/splitwise/debt.py`

 * *Files identical despite different names*

### Comparing `splitwise-2.5.0/splitwise/error.py` & `splitwise-3.0.0/splitwise/error.py`

 * *Files identical despite different names*

### Comparing `splitwise-2.5.0/splitwise/exception.py` & `splitwise-3.0.0/splitwise/exception.py`

 * *Files identical despite different names*

### Comparing `splitwise-2.5.0/splitwise/expense.py` & `splitwise-3.0.0/splitwise/expense.py`

 * *Files identical despite different names*

### Comparing `splitwise-2.5.0/splitwise/group.py` & `splitwise-3.0.0/splitwise/group.py`

 * *Files identical despite different names*

### Comparing `splitwise-2.5.0/splitwise/notification.py` & `splitwise-3.0.0/splitwise/notification.py`

 * *Files identical despite different names*

### Comparing `splitwise-2.5.0/splitwise/picture.py` & `splitwise-3.0.0/splitwise/picture.py`

 * *Files identical despite different names*

### Comparing `splitwise-2.5.0/splitwise/receipt.py` & `splitwise-3.0.0/splitwise/receipt.py`

 * *Files identical despite different names*

### Comparing `splitwise-2.5.0/splitwise/user.py` & `splitwise-3.0.0/splitwise/user.py`

 * *Files identical despite different names*

### Comparing `splitwise-2.5.0/splitwise.egg-info/PKG-INFO` & `splitwise-3.0.0/splitwise.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 Metadata-Version: 2.1
 Name: splitwise
-Version: 2.5.0
+Version: 3.0.0
 Summary: Splitwise Python SDK
 Home-page: https://github.com/namaggarwal/splitwise
-Download-URL: https://github.com/namaggarwal/splitwise/tarball/v2.5.0
+Download-URL: https://github.com/namaggarwal/splitwise/tarball/v3.0.0
 Author: Naman Aggarwal
 Author-email: aggarwal.nam@gmail.com
 License: MIT
 Project-URL: Documentation, https://splitwise.readthedocs.io
 Project-URL: Source, https://github.com/namaggarwal/splitwise
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Splitwise Python SDK
 
 ![](https://pepy.tech/badge/splitwise)
@@ -34,15 +30,15 @@
 ![](https://img.shields.io/pypi/wheel/splitwise.svg)
 ![](https://img.shields.io/pypi/pyversions/splitwise.svg)
 
 This is the python sdk for Splitwise APIs. Pull requests and bug reports are welcomed.
 
 ## Latest Version
 
-The latest version of splitwise SDK is Splitwise-2.5.0
+The latest version of splitwise SDK is Splitwise-3.0.0
 
 ## Docs
 
 The detailed docs are hosted at [readthedocs.org](https://readthedocs.org/projects/splitwise/)
 
 ## Installation
 
@@ -217,15 +213,15 @@
 sObj = Splitwise(Config.consumer_key,Config.consumer_secret)
 sObj.setAccessToken(session['access_token'])
 sObj.getGroup(43233)
 ```
 
 ### Get Expenses
 
-You can use ```getExpenses(offset,limit,group_id,friendship_id,dated_after,dated_before,updated_after,updated_before)``` to get all the expenses of the current user based on filter options. It returns a list of ```Expense``` objects.
+You can use ```getExpenses(offset,limit,group_id,friend_id,dated_after,dated_before,updated_after,updated_before,visible)``` to get all the expenses of the current user based on filter options. It returns a list of ```Expense``` objects.
 
 ```python
 sObj = Splitwise(Config.consumer_key,Config.consumer_secret)
 sObj.setAccessToken(session['access_token'])
 sObj.getExpenses()
 ```
 
@@ -371,14 +367,30 @@
 expense.setCost('10')
 expense.setDescription("Updated description")
 
 expense, errors = sObj.updateExpense(expense)
 print(expense.getId())
 ```
 
+or update the fetched expense
+
+
+```python
+from splitwise.expense import Expense
+
+sObj = Splitwise(Config.consumer_key,Config.consumer_secret)
+sObj.setAccessToken(session['access_token'])
+
+expense, error = sObj.getExpense(12345)
+expense.setDescription("Updated description")
+
+expense, errors = sObj.updateExpense(expense)
+print(expense.getDescription())
+```
+
 ### Delete expense
 You can use ```deleteExpense(expense_id)``` to delete an existing expense.
 
 ```python
 
 sObj = Splitwise(Config.consumer_key,Config.consumer_secret)
 sObj.setAccessToken(session['access_token'])
```

### Comparing `splitwise-2.5.0/splitwise.egg-info/SOURCES.txt` & `splitwise-3.0.0/splitwise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splitwise-2.5.0/tests/test_addUserToGroup.py` & `splitwise-3.0.0/tests/test_addUserToGroup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from splitwise import Splitwise
 from splitwise.user import User
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class AddUserToGroupTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_createComment.py` & `splitwise-3.0.0/tests/test_createComment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from splitwise import Splitwise
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class CreateCommentTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_createExpense.py` & `splitwise-3.0.0/tests/test_createExpense.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import unittest
 
 from splitwise import Splitwise
 from splitwise.expense import Expense, ExpenseUser
-
-try:
-    from unittest.mock import MagicMock, patch
-except ImportError:  # Python 2
-    from mock import MagicMock, patch
+from unittest.mock import MagicMock, patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class CreateExpenseTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
@@ -25,15 +21,15 @@
         expense.setDescription("Testing")
         expense.setGroupId(19433671)
         expense.setSplitEqually()
         expense.setReceipt("temp.jpg")
         expenseRes, errors = self.sObj.createExpense(expense)
         mockMakeRequest.assert_called_with(
             "https://secure.splitwise.com/api/v3.0/create_expense", "POST",
-            {'cost': '10', 'description': 'Testing', 'group_id': 19433671, 'split_equally': True, 'receiptPath': 'temp.jpg'},
+            {'cost': '10', 'description': 'Testing', 'group_id': 19433671, 'split_equally': True},
             files={'receipt': mockFile})
         self.assertIsNone(errors)
         self.assertEqual(expenseRes.getId(), 1010906976)
         self.assertEqual(expenseRes.getGroupId(), 19433671)
         self.assertEqual(expenseRes.getFriendshipId(), None)
         self.assertEqual(expenseRes.getExpenseBundleId(), None)
         self.assertEqual(expenseRes.getDescription(), "Testing")
```

### Comparing `splitwise-2.5.0/tests/test_createGroup.py` & `splitwise-3.0.0/tests/test_createGroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from splitwise import Splitwise
 from splitwise.group import Group, FriendGroup
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class CreateGroupTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_deleteExpense.py` & `splitwise-3.0.0/tests/test_deleteExpense.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from splitwise import Splitwise
 from splitwise.exception import SplitwiseNotFoundException, SplitwiseNotAllowedException
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class DeleteExpenseTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_deleteGroup.py` & `splitwise-3.0.0/tests/test_deleteGroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from splitwise import Splitwise
 from splitwise.exception import SplitwiseNotFoundException, SplitwiseNotAllowedException
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class DeleteGroupTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_getCategories.py` & `splitwise-3.0.0/tests/test_getCategories.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from splitwise import Splitwise
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class GetCategoriesTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_getComments.py` & `splitwise-3.0.0/tests/test_getComments.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from splitwise import Splitwise
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class GetComments(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_getCurrencies.py` & `splitwise-3.0.0/tests/test_getCurrencies.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from splitwise import Splitwise
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class GetCurrenciesTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_getCurrentUser.py` & `splitwise-3.0.0/tests/test_getCurrentUser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from splitwise import Splitwise
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class GetCurrentUserTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_getExpense.py` & `splitwise-3.0.0/tests/test_getExpense.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from splitwise import Splitwise
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class GetExpenseTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_getExpenses.py` & `splitwise-3.0.0/tests/test_getExpenses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from splitwise import Splitwise
 import unittest
-try:
-    from unittest.mock import patch
-    from urllib.parse import parse_qs
-    import urllib.parse as urlparse
-except ImportError:  # Python 2
-    from mock import patch
-    from urlparse import parse_qs
-    import urlparse
+from unittest.mock import patch
+from urllib.parse import parse_qs
+import urllib.parse as urlparse
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class GetExpensesTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
@@ -155,15 +150,15 @@
         self.sObj.getExpenses(2, 3, "123", "1234", "2020-12-12", "2020-12-19", "2020-12-13", "2020-12-18")
         args, kwargs = mockMakeRequest.call_args
         parsed = urlparse.urlparse(args[0])
         qs = parse_qs(parsed.query)
         self.assertEqual(qs['offset'], ['2'])
         self.assertEqual(qs['limit'], ['3'])
         self.assertEqual(qs['group_id'], ['123'])
-        self.assertEqual(qs['friendship_id'], ['1234'])
+        self.assertEqual(qs['friend_id'], ['1234'])
         self.assertEqual(qs['dated_after'], ['2020-12-12'])
         self.assertEqual(qs['dated_before'], ['2020-12-19'])
         self.assertEqual(qs['updated_after'], ['2020-12-13'])
         self.assertEqual(qs['updated_before'], ['2020-12-18'])
 
     def test_getExpenses_exception(self, mockMakeRequest):
         mockMakeRequest.side_effect = Exception(
```

### Comparing `splitwise-2.5.0/tests/test_getFriends.py` & `splitwise-3.0.0/tests/test_getFriends.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from splitwise import Splitwise
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class GetFriendsTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_getGroup.py` & `splitwise-3.0.0/tests/test_getGroup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from splitwise import Splitwise
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class GetCategoriesTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_getGroups.py` & `splitwise-3.0.0/tests/test_getGroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from splitwise import Splitwise
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class GetGroupsTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_getNotifications.py` & `splitwise-3.0.0/tests/test_getNotifications.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from splitwise import Splitwise
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class GetNotifications(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_getUser.py` & `splitwise-3.0.0/tests/test_getUser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from splitwise import Splitwise
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class GetUserTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_updateExpense.py` & `splitwise-3.0.0/tests/test_updateExpense.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import unittest
 
 from splitwise import Splitwise, SplitwiseBadRequestException
 from splitwise.expense import Expense, ExpenseUser
-
-try:
-    from unittest.mock import MagicMock, patch
-except ImportError:  # Python 2
-    from mock import MagicMock, patch
+from unittest.mock import MagicMock, patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class UpdateExpenseTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

### Comparing `splitwise-2.5.0/tests/test_updateUser.py` & `splitwise-3.0.0/tests/test_updateUser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from splitwise import Splitwise
 from splitwise.user import User
 from splitwise.exception import SplitwiseBadRequestException
 import unittest
-try:
-    from unittest.mock import patch
-except ImportError:  # Python 2
-    from mock import patch
+from unittest.mock import patch
 
 
 @patch('splitwise.Splitwise._Splitwise__makeRequest')
 class UpdateUserTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sObj = Splitwise('consumerkey', 'consumersecret')
```

