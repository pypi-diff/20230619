# Comparing `tmp/AlgoMaster-0.0.6.tar.gz` & `tmp/AlgoMaster-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgoMaster-0.0.6.tar", last modified: Mon Jun 19 17:02:21 2023, max compression
+gzip compressed data, was "AlgoMaster-0.0.7.tar", last modified: Mon Jun 19 17:05:29 2023, max compression
```

## Comparing `AlgoMaster-0.0.6.tar` & `AlgoMaster-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 17:02:21.727487 AlgoMaster-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-06-19 17:02:21.654482 AlgoMaster-0.0.6/AlgoMaster/
--rw-rw-rw-   0        0        0       39 2023-06-19 16:54:03.000000 AlgoMaster-0.0.6/AlgoMaster/__init__.py
--rw-rw-rw-   0        0        0     8832 2023-06-19 17:00:11.000000 AlgoMaster-0.0.6/AlgoMaster/classifier.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:02:21.723486 AlgoMaster-0.0.6/AlgoMaster.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-19 17:02:21.000000 AlgoMaster-0.0.6/AlgoMaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-19 17:02:21.000000 AlgoMaster-0.0.6/AlgoMaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 17:02:21.000000 AlgoMaster-0.0.6/AlgoMaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-19 17:02:21.000000 AlgoMaster-0.0.6/AlgoMaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 17:02:21.000000 AlgoMaster-0.0.6/AlgoMaster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      534 2023-06-19 17:02:21.725487 AlgoMaster-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-17 16:12:45.000000 AlgoMaster-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 17:02:21.728487 AlgoMaster-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1329 2023-06-19 17:02:17.000000 AlgoMaster-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:05:29.361331 AlgoMaster-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-06-19 17:05:29.288234 AlgoMaster-0.0.7/AlgoMaster/
+-rw-rw-rw-   0        0        0       39 2023-06-19 16:54:03.000000 AlgoMaster-0.0.7/AlgoMaster/__init__.py
+-rw-rw-rw-   0        0        0     8850 2023-06-19 17:05:17.000000 AlgoMaster-0.0.7/AlgoMaster/classifier.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:05:29.355330 AlgoMaster-0.0.7/AlgoMaster.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-19 17:05:29.000000 AlgoMaster-0.0.7/AlgoMaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-19 17:05:29.000000 AlgoMaster-0.0.7/AlgoMaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 17:05:29.000000 AlgoMaster-0.0.7/AlgoMaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-19 17:05:29.000000 AlgoMaster-0.0.7/AlgoMaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 17:05:29.000000 AlgoMaster-0.0.7/AlgoMaster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      534 2023-06-19 17:05:29.359328 AlgoMaster-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-17 16:12:45.000000 AlgoMaster-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 17:05:29.361331 AlgoMaster-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1329 2023-06-19 17:05:24.000000 AlgoMaster-0.0.7/setup.py
```

### Comparing `AlgoMaster-0.0.6/AlgoMaster/classifier.py` & `AlgoMaster-0.0.7/AlgoMaster/classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,22 +47,24 @@
         roc = roc_auc_score(y_test_f, y_pred_f)
         f1 = f1_score(y_test_f, y_pred_f)
         recall = recall_score(y_test_f, y_pred_f)
         precision = precision_score(y_test_f, y_pred_f)
         return {'model name': model_name, 'accuracy': acc, 'confusion': confusion, 'roc': roc, 'f1': f1, 'recall': recall, 'precision': precision}
 
     def model_training(self):
+        model_results = []
         for model, model_name in zip(self.model, self.model_name):
             model.fit(self.X_train, self.Y_train)
             y_pred = model.predict(self.X_test)
             model_result = self.model_accuracy(self.Y_test, y_pred, model_name)
-            self.model_table = self.model_table.append(model_result, ignore_index=True)
+            model_results.append(model_result)
 
-        self.model_table = self.model_table.sort_values('accuracy', ascending=False)  # Sort table by accuracy
-        self.model_table.reset_index(drop=True, inplace=True)  # Reset index
+        self.model_table = pd.concat(model_results, ignore_index=True)
+        self.model_table = self.model_table.sort_values('accuracy', ascending=False)
+        self.model_table.reset_index(drop=True, inplace=True)
         return self.model_table
     
     def ensemble_prediction(self, count):
         top_models = nlargest(count, self.model_table.iterrows(), key=lambda x: x[1]['accuracy'])
         ensemble_predictions = []
         for _, model_row in top_models:
             model_index = self.model_name.index(model_row['model name'])
```

### Comparing `AlgoMaster-0.0.6/AlgoMaster.egg-info/PKG-INFO` & `AlgoMaster-0.0.7/AlgoMaster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgoMaster
-Version: 0.0.6
+Version: 0.0.7
 Summary: Learning models make simple
 Author: sajo sam
 Author-email: <sajosamambalakara@gmail.com>
 Keywords: python,classification,regression,machine learning models,hyper parameter turning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AlgoMaster-0.0.6/PKG-INFO` & `AlgoMaster-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgoMaster
-Version: 0.0.6
+Version: 0.0.7
 Summary: Learning models make simple
 Author: sajo sam
 Author-email: <sajosamambalakara@gmail.com>
 Keywords: python,classification,regression,machine learning models,hyper parameter turning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AlgoMaster-0.0.6/setup.py` & `AlgoMaster-0.0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Learning models make simple'
 # LONG_DESCRIPTION = '''
 #                                         Learning models
 #                                     (single-file, easy-to-use)'''
 
 # Setting up
 setup(
```

