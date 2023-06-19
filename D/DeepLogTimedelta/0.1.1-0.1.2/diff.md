# Comparing `tmp/DeepLogTimedelta-0.1.1.tar.gz` & `tmp/DeepLogTimedelta-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepLogTimedelta-0.1.1.tar", last modified: Mon Jun 19 13:42:37 2023, max compression
+gzip compressed data, was "DeepLogTimedelta-0.1.2.tar", last modified: Mon Jun 19 13:47:26 2023, max compression
```

## Comparing `DeepLogTimedelta-0.1.1.tar` & `DeepLogTimedelta-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 13:42:37.064954 DeepLogTimedelta-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-19 13:42:37.050810 DeepLogTimedelta-0.1.1/DeepLogTimedelta/
--rw-rw-rw-   0        0        0     1100 2023-06-19 13:31:46.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta/DeepLogTimedelta.py
--rw-rw-rw-   0        0        0        0 2023-06-19 12:37:56.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta/__init__.py
--rw-rw-rw-   0        0        0       97 2023-06-19 11:56:09.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta/main.py
--rw-rw-rw-   0        0        0     2311 2023-06-19 13:39:09.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta/preproccesing.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:42:37.061894 DeepLogTimedelta-0.1.1/DeepLogTimedelta.egg-info/
--rw-rw-rw-   0        0        0      207 2023-06-19 13:42:36.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-06-19 13:42:36.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 13:42:36.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-19 13:42:36.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      207 2023-06-19 13:42:37.063960 DeepLogTimedelta-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-19 13:42:37.064954 DeepLogTimedelta-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      335 2023-06-19 13:40:18.000000 DeepLogTimedelta-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:47:26.296082 DeepLogTimedelta-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-06-19 13:47:26.259357 DeepLogTimedelta-0.1.2/DeepLogTimedelta/
+-rw-rw-rw-   0        0        0     1100 2023-06-19 13:31:46.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta/DeepLogTimedelta.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:37:56.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta/__init__.py
+-rw-rw-rw-   0        0        0       97 2023-06-19 11:56:09.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta/main.py
+-rw-rw-rw-   0        0        0     2311 2023-06-19 13:46:57.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta/preproccesing.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:47:26.292900 DeepLogTimedelta-0.1.2/DeepLogTimedelta.egg-info/
+-rw-rw-rw-   0        0        0      207 2023-06-19 13:47:26.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-06-19 13:47:26.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 13:47:26.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-19 13:47:26.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      207 2023-06-19 13:47:26.295899 DeepLogTimedelta-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-19 13:47:26.297090 DeepLogTimedelta-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      335 2023-06-19 13:47:21.000000 DeepLogTimedelta-0.1.2/setup.py
```

### Comparing `DeepLogTimedelta-0.1.1/DeepLogTimedelta/DeepLogTimedelta.py` & `DeepLogTimedelta-0.1.2/DeepLogTimedelta/DeepLogTimedelta.py`

 * *Files identical despite different names*

### Comparing `DeepLogTimedelta-0.1.1/DeepLogTimedelta/preproccesing.py` & `DeepLogTimedelta-0.1.2/DeepLogTimedelta/preproccesing.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             lambda x: pd.Timestamp(pd.Timestamp(x).strftime('%Y-%m-%d %H:%M:%S')).timestamp())
         train.sort_values(by='timestamp', inplace=True, ignore_index=True)
 
         self.get_timediff(train)
         return train
 
     def sequence(self, data: pd.DataFrame):
-        train = self.initiliaze(data)
+        train = self.initialize(data)
         timedelta = train.timediff.values
         X, y = self.get_timediff_sequence(timedelta, self._length)
         X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.33, shuffle=False)
         X_train = torch.Tensor(X_train)
         X_test = torch.Tensor(X_test)
         y_train = torch.Tensor(y_train)
         y_test = torch.Tensor(y_test)
```

