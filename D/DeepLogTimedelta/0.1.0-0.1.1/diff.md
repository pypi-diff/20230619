# Comparing `tmp/DeepLogTimedelta-0.1.0.tar.gz` & `tmp/DeepLogTimedelta-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepLogTimedelta-0.1.0.tar", last modified: Mon Jun 19 13:29:04 2023, max compression
+gzip compressed data, was "DeepLogTimedelta-0.1.1.tar", last modified: Mon Jun 19 13:42:37 2023, max compression
```

## Comparing `DeepLogTimedelta-0.1.0.tar` & `DeepLogTimedelta-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 13:29:04.601192 DeepLogTimedelta-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-19 13:29:04.575687 DeepLogTimedelta-0.1.0/DeepLogTimedelta/
--rw-rw-rw-   0        0        0     1100 2023-06-19 13:11:20.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta/DeepLogTimedelta.py
--rw-rw-rw-   0        0        0        0 2023-06-19 12:37:56.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta/__init__.py
--rw-rw-rw-   0        0        0       97 2023-06-19 11:56:09.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta/main.py
--rw-rw-rw-   0        0        0     2309 2023-06-19 13:28:17.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta/preproccesing.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:29:04.598003 DeepLogTimedelta-0.1.0/DeepLogTimedelta.egg-info/
--rw-rw-rw-   0        0        0      207 2023-06-19 13:29:04.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-06-19 13:29:04.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 13:29:04.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-19 13:29:04.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      207 2023-06-19 13:29:04.600188 DeepLogTimedelta-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-19 13:29:04.601192 DeepLogTimedelta-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      335 2023-06-19 13:29:01.000000 DeepLogTimedelta-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:42:37.064954 DeepLogTimedelta-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-19 13:42:37.050810 DeepLogTimedelta-0.1.1/DeepLogTimedelta/
+-rw-rw-rw-   0        0        0     1100 2023-06-19 13:31:46.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta/DeepLogTimedelta.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:37:56.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta/__init__.py
+-rw-rw-rw-   0        0        0       97 2023-06-19 11:56:09.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta/main.py
+-rw-rw-rw-   0        0        0     2311 2023-06-19 13:39:09.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta/preproccesing.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:42:37.061894 DeepLogTimedelta-0.1.1/DeepLogTimedelta.egg-info/
+-rw-rw-rw-   0        0        0      207 2023-06-19 13:42:36.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-06-19 13:42:36.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 13:42:36.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-19 13:42:36.000000 DeepLogTimedelta-0.1.1/DeepLogTimedelta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      207 2023-06-19 13:42:37.063960 DeepLogTimedelta-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-19 13:42:37.064954 DeepLogTimedelta-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      335 2023-06-19 13:40:18.000000 DeepLogTimedelta-0.1.1/setup.py
```

### Comparing `DeepLogTimedelta-0.1.0/DeepLogTimedelta/DeepLogTimedelta.py` & `DeepLogTimedelta-0.1.1/DeepLogTimedelta/DeepLogTimedelta.py`

 * *Files identical despite different names*

### Comparing `DeepLogTimedelta-0.1.0/DeepLogTimedelta/preproccesing.py` & `DeepLogTimedelta-0.1.1/DeepLogTimedelta/preproccesing.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     def initialize(self, data: pd.DataFrame):
         need_columns = ['event_id', '@timestamp']
         train = data[need_columns]
         train = train.rename(columns={'event_id': 'event', '@timestamp': 'timestamp'})
         train['timestamp'] = train['timestamp'].apply(
             lambda x: pd.Timestamp(pd.Timestamp(x).strftime('%Y-%m-%d %H:%M:%S')).timestamp())
         train.sort_values(by='timestamp', inplace=True, ignore_index=True)
+
         self.get_timediff(train)
         return train
 
     def sequence(self, data: pd.DataFrame):
         train = self.initiliaze(data)
         timedelta = train.timediff.values
         X, y = self.get_timediff_sequence(timedelta, self._length)
```

