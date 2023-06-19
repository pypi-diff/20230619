# Comparing `tmp/fsrs4anki_optimizer-3.25.2.tar.gz` & `tmp/fsrs4anki_optimizer-3.25.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.25.2.tar", last modified: Mon Jun 19 06:49:22 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.25.3.tar", last modified: Mon Jun 19 07:13:50 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.25.2.tar` & `fsrs4anki_optimizer-3.25.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:49:22.470964 fsrs4anki_optimizer-3.25.2/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 06:49:22.470964 fsrs4anki_optimizer-3.25.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:49:22.470964 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 06:49:09.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-19 06:49:09.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43958 2023-06-19 06:49:09.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:49:22.470964 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 06:49:22.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-19 06:49:22.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:49:22.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-19 06:49:22.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 06:49:22.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-19 06:49:09.000000 fsrs4anki_optimizer-3.25.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 06:49:22.470964 fsrs4anki_optimizer-3.25.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 06:49:09.000000 fsrs4anki_optimizer-3.25.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:50.439204 fsrs4anki_optimizer-3.25.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 07:13:50.439204 fsrs4anki_optimizer-3.25.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:50.435204 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 07:13:36.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-19 07:13:36.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44249 2023-06-19 07:13:36.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:50.439204 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 07:13:50.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-19 07:13:50.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:13:50.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-19 07:13:50.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 07:13:50.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-19 07:13:36.000000 fsrs4anki_optimizer-3.25.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 07:13:50.439204 fsrs4anki_optimizer-3.25.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 07:13:36.000000 fsrs4anki_optimizer-3.25.3/setup.py
```

### Comparing `fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -461,14 +461,19 @@
     def train(self, lr: float = 4e-2, n_epoch: int = 3, n_splits: int = 3, batch_size: int = 512, verbose: bool = True):
         """Step 4"""
         self.dataset = pd.read_csv("./revlog_history.tsv", sep='\t', index_col=None, dtype={'r_history': str ,'t_history': str} )
         self.dataset = self.dataset[(self.dataset['i'] > 1) & (self.dataset['delta_t'] > 0) & (self.dataset['t_history'].str.count(',0') == 0)]
         self.dataset['tensor'] = self.dataset.progress_apply(lambda x: lineToTensor(list(zip([x['t_history']], [x['r_history']]))[0]), axis=1)
         self.dataset['group'] = self.dataset['r_history'] + self.dataset['t_history']
         print("Tensorized!")
+        
+        n_pre_train_groups = len(self.dataset[self.dataset['i'] == 2]['group'].unique())
+        if n_pre_train_groups < n_splits:
+            print("Not enough groups for pre-training. Splitting into {} folds.".format(n_pre_train_groups))
+            n_splits = n_pre_train_groups
 
         w = []
         plots = []
         if n_splits > 1:
             sgkf = StratifiedGroupKFold(n_splits=n_splits)
             for train_index, test_index in sgkf.split(self.dataset, self.dataset['i'], self.dataset['group']):
                 print("TRAIN:", len(train_index), "TEST:",  len(test_index))
```

