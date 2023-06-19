# Comparing `tmp/pytest_xdist_worker_stats-0.1.1.tar.gz` & `tmp/pytest_xdist_worker_stats-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_xdist_worker_stats-0.1.1.tar", max compression
+gzip compressed data, was "pytest_xdist_worker_stats-0.1.2.tar", max compression
```

## Comparing `pytest_xdist_worker_stats-0.1.1.tar` & `pytest_xdist_worker_stats-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-06-15 08:53:33.817321 pytest_xdist_worker_stats-0.1.1/LICENSE
--rw-r--r--   0        0        0     2004 2023-06-15 08:57:34.823044 pytest_xdist_worker_stats-0.1.1/README.md
--rw-r--r--   0        0        0     2831 2023-06-15 08:57:22.904206 pytest_xdist_worker_stats-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       75 2023-06-15 08:57:22.908206 pytest_xdist_worker_stats-0.1.1/pytest_xdist_worker_stats/__init__.py
--rw-r--r--   0        0        0      937 2023-06-15 08:53:33.821321 pytest_xdist_worker_stats-0.1.1/pytest_xdist_worker_stats/options.py
--rw-r--r--   0        0        0     2372 2023-06-15 08:53:33.822321 pytest_xdist_worker_stats-0.1.1/pytest_xdist_worker_stats/plugin.py
--rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 pytest_xdist_worker_stats-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-15 08:53:33.817321 pytest_xdist_worker_stats-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2004 2023-06-15 08:57:34.823044 pytest_xdist_worker_stats-0.1.2/README.md
+-rw-r--r--   0        0        0     2831 2023-06-19 16:09:38.510823 pytest_xdist_worker_stats-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-06-19 16:09:38.510823 pytest_xdist_worker_stats-0.1.2/pytest_xdist_worker_stats/__init__.py
+-rw-r--r--   0        0        0      937 2023-06-15 08:53:33.821321 pytest_xdist_worker_stats-0.1.2/pytest_xdist_worker_stats/options.py
+-rw-r--r--   0        0        0     2333 2023-06-19 16:09:38.510823 pytest_xdist_worker_stats-0.1.2/pytest_xdist_worker_stats/plugin.py
+-rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 pytest_xdist_worker_stats-0.1.2/PKG-INFO
```

### Comparing `pytest_xdist_worker_stats-0.1.1/LICENSE` & `pytest_xdist_worker_stats-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.1/README.md` & `pytest_xdist_worker_stats-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.1/pyproject.toml` & `pytest_xdist_worker_stats-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-xdist-worker-stats"
-version = "0.1.1"
+version = "0.1.2"
 description = "A pytest plugin to list worker statistics after a xdist run."
 authors = ["Mikuláš Poul <mikulaspoul@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pytest_xdist_worker_stats"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `pytest_xdist_worker_stats-0.1.1/pytest_xdist_worker_stats/options.py` & `pytest_xdist_worker_stats-0.1.2/pytest_xdist_worker_stats/options.py`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.1/pytest_xdist_worker_stats/plugin.py` & `pytest_xdist_worker_stats-0.1.2/pytest_xdist_worker_stats/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,17 @@
 
 SHARED_WORKER_INFO = "worker_info"
 
 
 class XdistWorkerStatsPlugin:
     def __init__(self, config):
         self.config = config
-        self.is_primary = self.is_primary()
         self.test_stats = {}
         self.worker_test_times = {}
 
-    def is_primary(self):
-        return not hasattr(self.config, "workerinput")
-
     def add(self, name):
         self.test_stats[name] = self.test_stats.get(name) or {}
         return self.test_stats[name]
 
     def pytest_runtest_setup(self, item):
         self.add(item.nodeid)["start"] = time.time()
 
@@ -47,19 +43,22 @@
                 worker_times = self.worker_test_times[worker]
                 tr._tw.line(f"worker {worker: <5}: {len(worker_times): >4} tests {sum(worker_times):10.2f}s runtime")
 
     def pytest_testnodedown(self, node, error):
         """
         Get statistic about worker usage for test cases from xdist nodes and merge to primary stats.
         """
-        if (node_worker_stats := node.workeroutput.get(SHARED_WORKER_INFO)) is not None:
+        if (
+            hasattr(node, "workeroutput")
+            and (node_worker_stats := node.workeroutput.get(SHARED_WORKER_INFO)) is not None
+        ):
             self.worker_test_times.update(dict(node_worker_stats))
 
     @pytest.hookimpl(hookwrapper=True, trylast=True)
     def pytest_sessionfinish(self, session, exitstatus):
         """
         Dump worker usage statistics to `workeroutput`.
         Executed once per node if with xdist and will gen from primary node.
         """
         yield
-        if not self.is_primary:
+        if hasattr(self.config, "workeroutput"):
             self.config.workeroutput[SHARED_WORKER_INFO] = self.worker_test_times
```

### Comparing `pytest_xdist_worker_stats-0.1.1/PKG-INFO` & `pytest_xdist_worker_stats-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-xdist-worker-stats
-Version: 0.1.1
+Version: 0.1.2
 Summary: A pytest plugin to list worker statistics after a xdist run.
 Home-page: https://github.com/mikicz/pytest-xdist-worker-stats
 License: MIT
 Keywords: pytest,xdist,pytest-xdist
 Author: Mikuláš Poul
 Author-email: mikulaspoul@gmail.com
 Requires-Python: >=3.10,<4.0
```

