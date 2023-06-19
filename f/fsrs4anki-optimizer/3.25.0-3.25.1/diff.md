# Comparing `tmp/fsrs4anki_optimizer-3.25.0.tar.gz` & `tmp/fsrs4anki_optimizer-3.25.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.25.0.tar", last modified: Sun Jun 18 15:19:45 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.25.1.tar", last modified: Mon Jun 19 06:20:32 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.25.0.tar` & `fsrs4anki_optimizer-3.25.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:19:45.202244 fsrs4anki_optimizer-3.25.0/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-18 15:19:45.202244 fsrs4anki_optimizer-3.25.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:19:45.202244 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-18 15:19:35.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-18 15:19:35.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43747 2023-06-18 15:19:35.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:19:45.202244 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-18 15:19:45.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-18 15:19:45.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:19:45.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-18 15:19:45.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 15:19:45.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-18 15:19:35.000000 fsrs4anki_optimizer-3.25.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 15:19:45.202244 fsrs4anki_optimizer-3.25.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 15:19:35.000000 fsrs4anki_optimizer-3.25.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:20:32.614370 fsrs4anki_optimizer-3.25.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 06:20:32.614370 fsrs4anki_optimizer-3.25.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:20:32.614370 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 06:20:23.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-19 06:20:23.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43832 2023-06-19 06:20:23.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:20:32.614370 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 06:20:32.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-19 06:20:32.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:20:32.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-19 06:20:32.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 06:20:32.000000 fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-19 06:20:23.000000 fsrs4anki_optimizer-3.25.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 06:20:32.614370 fsrs4anki_optimizer-3.25.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 06:20:23.000000 fsrs4anki_optimizer-3.25.1/setup.py
```

### Comparing `fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.25.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -610,15 +610,17 @@
             recall = percentage / 100
             time_list = np.zeros((d_range, index_len))
             time_list[:,:-1] = max_time
             for d in range(d_range, 0, -1):
                 s0 = init_stability(d)
                 s0_index = stability2index(s0)
                 diff = max_time
-                while diff > 1:
+                iteration = 0
+                while diff > 1 and iteration < 2e5:
+                    iteration += 1
                     total_time = time_list[d - 1].sum()
                     s_indices = np.arange(index_len - 2, -1, -1)
                     stabilities = stability_list[s_indices]
                     intervals = np.maximum(1, np.round(stabilities * np.log(recall) / np.log(0.9)))
                     p_recalls = np.power(0.9, intervals / stabilities)
                     recall_s = cal_next_recall_stability(stabilities, p_recalls, d, 1)
                     forget_d = np.minimum(d + d_offset, 10)
```

