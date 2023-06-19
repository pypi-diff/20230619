# Comparing `tmp/fsrs4anki_optimizer-3.25.1.tar.gz` & `tmp/fsrs4anki_optimizer-3.25.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.25.1.tar", last modified: Mon Jun 19 06:20:32 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.25.2.tar", last modified: Mon Jun 19 06:49:22 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.25.1.tar` & `fsrs4anki_optimizer-3.25.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:20:32.614370 fsrs4anki_optimizer-3.25.1/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 06:20:32.614370 fsrs4anki_optimizer-3.25.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:20:32.614370 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 06:20:23.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-19 06:20:23.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43832 2023-06-19 06:20:23.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:20:32.614370 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 06:20:32.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-19 06:20:32.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:20:32.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-19 06:20:32.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 06:20:32.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-19 06:20:23.000000 fsrs4anki_optimizer-3.25.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 06:20:32.614370 fsrs4anki_optimizer-3.25.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 06:20:23.000000 fsrs4anki_optimizer-3.25.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:49:22.470964 fsrs4anki_optimizer-3.25.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 06:49:22.470964 fsrs4anki_optimizer-3.25.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:49:22.470964 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 06:49:09.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-19 06:49:09.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43958 2023-06-19 06:49:09.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:49:22.470964 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 06:49:22.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-19 06:49:22.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:49:22.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-19 06:49:22.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 06:49:22.000000 fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-19 06:49:09.000000 fsrs4anki_optimizer-3.25.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 06:49:22.470964 fsrs4anki_optimizer-3.25.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 06:49:09.000000 fsrs4anki_optimizer-3.25.2/setup.py
```

### Comparing `fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.25.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,18 +126,21 @@
     def __init__(self, data_source: RevlogDataset, batch_size: int):
         self.data_source = data_source
         self.batch_size = batch_size
         lengths = np.array(data_source.seq_len)
         indices = np.argsort(lengths)
         full_batches, remainder = divmod(indices.size, self.batch_size)
         if full_batches > 0:
-            self.batch_indices = np.split(indices[:-remainder], full_batches)
+            if remainder == 0:
+                self.batch_indices = np.split(indices, full_batches)
+            else:
+                self.batch_indices = np.split(indices[:-remainder], full_batches)
         else:
             self.batch_indices = []
-        if remainder:
+        if remainder > 0:
             self.batch_indices.append(indices[-remainder:])
         self.batch_nums = len(self.batch_indices)
         # seed = int(torch.empty((), dtype=torch.int64).random_().item())
         seed = 2023
         self.generator = torch.Generator()
         self.generator.manual_seed(seed)
```

