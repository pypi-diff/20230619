# Comparing `tmp/aio-pygo-1.0.1.tar.gz` & `tmp/aio-pygo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio-pygo-1.0.1.tar", last modified: Sun Jun 18 21:51:16 2023, max compression
+gzip compressed data, was "aio-pygo-1.0.2.tar", last modified: Sun Jun 18 22:39:10 2023, max compression
```

## Comparing `aio-pygo-1.0.1.tar` & `aio-pygo-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 gael       (501) staff       (20)        0 2023-06-18 21:51:16.832437 aio-pygo-1.0.1/
--rw-r--r--   0 gael       (501) staff       (20)    35149 2023-05-31 17:21:41.000000 aio-pygo-1.0.1/LICENSE
--rw-r--r--   0 gael       (501) staff       (20)     2874 2023-06-18 21:51:16.832284 aio-pygo-1.0.1/PKG-INFO
--rw-r--r--   0 gael       (501) staff       (20)     2403 2023-06-18 21:42:02.000000 aio-pygo-1.0.1/README.md
-drwxr-xr-x   0 gael       (501) staff       (20)        0 2023-06-18 21:51:16.829617 aio-pygo-1.0.1/aio_pygo.egg-info/
--rw-r--r--   0 gael       (501) staff       (20)     2874 2023-06-18 21:51:16.000000 aio-pygo-1.0.1/aio_pygo.egg-info/PKG-INFO
--rw-r--r--   0 gael       (501) staff       (20)      316 2023-06-18 21:51:16.000000 aio-pygo-1.0.1/aio_pygo.egg-info/SOURCES.txt
--rw-r--r--   0 gael       (501) staff       (20)        1 2023-06-18 21:51:16.000000 aio-pygo-1.0.1/aio_pygo.egg-info/dependency_links.txt
--rw-r--r--   0 gael       (501) staff       (20)        5 2023-06-18 21:51:16.000000 aio-pygo-1.0.1/aio_pygo.egg-info/top_level.txt
-drwxr-xr-x   0 gael       (501) staff       (20)        0 2023-06-18 21:51:16.832086 aio-pygo-1.0.1/pygo/
--rw-r--r--   0 gael       (501) staff       (20)      227 2023-06-18 21:48:05.000000 aio-pygo-1.0.1/pygo/__init__.py
--rw-r--r--   0 gael       (501) staff       (20)     1866 2023-06-04 10:53:21.000000 aio-pygo-1.0.1/pygo/chan.py
--rw-r--r--   0 gael       (501) staff       (20)     3896 2023-06-03 19:27:51.000000 aio-pygo-1.0.1/pygo/chan_test.py
--rw-r--r--   0 gael       (501) staff       (20)      100 2023-06-03 17:41:42.000000 aio-pygo-1.0.1/pygo/conftest.py
--rw-r--r--   0 gael       (501) staff       (20)      558 2023-06-03 19:33:52.000000 aio-pygo-1.0.1/pygo/defer.py
--rw-r--r--   0 gael       (501) staff       (20)      552 2023-06-03 19:36:11.000000 aio-pygo-1.0.1/pygo/defer_test.py
--rw-r--r--   0 gael       (501) staff       (20)      537 2023-06-03 20:09:47.000000 aio-pygo-1.0.1/pygo/go.py
--rw-r--r--   0 gael       (501) staff       (20)      590 2023-06-03 19:39:32.000000 aio-pygo-1.0.1/pygo/go_test.py
--rw-r--r--   0 gael       (501) staff       (20)      375 2023-06-18 19:59:45.000000 aio-pygo-1.0.1/pygo/time.py
--rw-r--r--   0 gael       (501) staff       (20)      336 2023-06-18 19:57:32.000000 aio-pygo-1.0.1/pygo/time_test.py
--rw-r--r--   0 gael       (501) staff       (20)      571 2023-06-18 21:48:27.000000 aio-pygo-1.0.1/pyproject.toml
--rw-r--r--   0 gael       (501) staff       (20)       38 2023-06-18 21:51:16.832483 aio-pygo-1.0.1/setup.cfg
+drwxr-xr-x   0 gael       (501) staff       (20)        0 2023-06-18 22:39:10.170075 aio-pygo-1.0.2/
+-rw-r--r--   0 gael       (501) staff       (20)    35149 2023-05-31 17:21:41.000000 aio-pygo-1.0.2/LICENSE
+-rw-r--r--   0 gael       (501) staff       (20)     3102 2023-06-18 22:39:10.169938 aio-pygo-1.0.2/PKG-INFO
+-rw-r--r--   0 gael       (501) staff       (20)     2631 2023-06-18 22:36:53.000000 aio-pygo-1.0.2/README.md
+drwxr-xr-x   0 gael       (501) staff       (20)        0 2023-06-18 22:39:10.168357 aio-pygo-1.0.2/aio_pygo.egg-info/
+-rw-r--r--   0 gael       (501) staff       (20)     3102 2023-06-18 22:39:10.000000 aio-pygo-1.0.2/aio_pygo.egg-info/PKG-INFO
+-rw-r--r--   0 gael       (501) staff       (20)      316 2023-06-18 22:39:10.000000 aio-pygo-1.0.2/aio_pygo.egg-info/SOURCES.txt
+-rw-r--r--   0 gael       (501) staff       (20)        1 2023-06-18 22:39:10.000000 aio-pygo-1.0.2/aio_pygo.egg-info/dependency_links.txt
+-rw-r--r--   0 gael       (501) staff       (20)        5 2023-06-18 22:39:10.000000 aio-pygo-1.0.2/aio_pygo.egg-info/top_level.txt
+drwxr-xr-x   0 gael       (501) staff       (20)        0 2023-06-18 22:39:10.169726 aio-pygo-1.0.2/pygo/
+-rw-r--r--   0 gael       (501) staff       (20)      228 2023-06-18 21:53:22.000000 aio-pygo-1.0.2/pygo/__init__.py
+-rw-r--r--   0 gael       (501) staff       (20)     1863 2023-06-18 22:31:26.000000 aio-pygo-1.0.2/pygo/chan.py
+-rw-r--r--   0 gael       (501) staff       (20)     3897 2023-06-18 22:31:26.000000 aio-pygo-1.0.2/pygo/chan_test.py
+-rw-r--r--   0 gael       (501) staff       (20)      100 2023-06-03 17:41:42.000000 aio-pygo-1.0.2/pygo/conftest.py
+-rw-r--r--   0 gael       (501) staff       (20)      558 2023-06-03 19:33:52.000000 aio-pygo-1.0.2/pygo/defer.py
+-rw-r--r--   0 gael       (501) staff       (20)      553 2023-06-18 22:31:26.000000 aio-pygo-1.0.2/pygo/defer_test.py
+-rw-r--r--   0 gael       (501) staff       (20)      537 2023-06-03 20:09:47.000000 aio-pygo-1.0.2/pygo/go.py
+-rw-r--r--   0 gael       (501) staff       (20)      590 2023-06-03 19:39:32.000000 aio-pygo-1.0.2/pygo/go_test.py
+-rw-r--r--   0 gael       (501) staff       (20)      375 2023-06-18 19:59:45.000000 aio-pygo-1.0.2/pygo/time.py
+-rw-r--r--   0 gael       (501) staff       (20)      336 2023-06-18 19:57:32.000000 aio-pygo-1.0.2/pygo/time_test.py
+-rw-r--r--   0 gael       (501) staff       (20)      603 2023-06-18 22:38:52.000000 aio-pygo-1.0.2/pyproject.toml
+-rw-r--r--   0 gael       (501) staff       (20)       38 2023-06-18 22:39:10.170114 aio-pygo-1.0.2/setup.cfg
```

### Comparing `aio-pygo-1.0.1/LICENSE` & `aio-pygo-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aio-pygo-1.0.1/PKG-INFO` & `aio-pygo-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: aio-pygo
-Version: 1.0.1
+Version: 1.0.2
 Summary: Write Python code in a Go-like fashion.
 Author: Gael Lz
 Project-URL: Homepage, https://github.com/GaelLnz/pygo
 Project-URL: Bug Tracker, https://github.com/GaelLnz/pygo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pygo
 
+[![PyPI version](https://badge.fury.io/py/aio-pygo.svg)](https://badge.fury.io/py/aio-pygo) [![codecov](https://codecov.io/gh/GaelLnz/pygo/branch/main/graph/badge.svg?token=PPVXA3VIQB)](https://codecov.io/gh/GaelLnz/pygo)
+
 Pygo is fully typed & zero dependency Python library that enables you to code in a Go-like fashion. It brings some of the key features from the Go programming language such as goroutines and channels.
 
 ## Features
 
 - **Goroutines**: Execute functions concurrently using asyncio coroutines.
 - **Channels**: Enable communication and synchronization between coroutines using channels.
 - **Select Statement**: Choose the first ready communication operation from multiple channels.
@@ -34,15 +36,15 @@
 
 ## Usage
 
 ### Goroutines
 
 ```python
 from asyncio import run
-from python-go import go
+from pygo import go
 
 async def worker():
     # some async operations
     ...
 
 async def main():
     # Start a goroutine
@@ -55,25 +57,25 @@
     run(main())
 ```
 
 ### Channels
 
 ```python
 from asyncio import run
-from python-go import Chan
+from pygo import Chan
 
 async def main():
     # Create a channel
     ch = Chan[str]()
 
     # Send data to the channel
-    ch.send("Hello, Pygo!")
+    await ch.send("Hello, Pygo!")
 
     # Receive data from the channel
-    data = ch.receive()
+    data, _ = await ch.receive()
     print(data)
 
 if __name__ == "__main__":
     run(main())
 ```
 
 ### And more
```

### Comparing `aio-pygo-1.0.1/README.md` & `aio-pygo-1.0.2/aio_pygo.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,25 @@
+Metadata-Version: 2.1
+Name: aio-pygo
+Version: 1.0.2
+Summary: Write Python code in a Go-like fashion.
+Author: Gael Lz
+Project-URL: Homepage, https://github.com/GaelLnz/pygo
+Project-URL: Bug Tracker, https://github.com/GaelLnz/pygo/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Pygo
 
+[![PyPI version](https://badge.fury.io/py/aio-pygo.svg)](https://badge.fury.io/py/aio-pygo) [![codecov](https://codecov.io/gh/GaelLnz/pygo/branch/main/graph/badge.svg?token=PPVXA3VIQB)](https://codecov.io/gh/GaelLnz/pygo)
+
 Pygo is fully typed & zero dependency Python library that enables you to code in a Go-like fashion. It brings some of the key features from the Go programming language such as goroutines and channels.
 
 ## Features
 
 - **Goroutines**: Execute functions concurrently using asyncio coroutines.
 - **Channels**: Enable communication and synchronization between coroutines using channels.
 - **Select Statement**: Choose the first ready communication operation from multiple channels.
@@ -20,15 +36,15 @@
 
 ## Usage
 
 ### Goroutines
 
 ```python
 from asyncio import run
-from python-go import go
+from pygo import go
 
 async def worker():
     # some async operations
     ...
 
 async def main():
     # Start a goroutine
@@ -41,25 +57,25 @@
     run(main())
 ```
 
 ### Channels
 
 ```python
 from asyncio import run
-from python-go import Chan
+from pygo import Chan
 
 async def main():
     # Create a channel
     ch = Chan[str]()
 
     # Send data to the channel
-    ch.send("Hello, Pygo!")
+    await ch.send("Hello, Pygo!")
 
     # Receive data from the channel
-    data = ch.receive()
+    data, _ = await ch.receive()
     print(data)
 
 if __name__ == "__main__":
     run(main())
 ```
 
 ### And more
@@ -87,8 +103,8 @@
 
 ## License
 
 Pygo is licensed under the GPL 3.0 License. See the [LICENSE](LICENSE) file for more details.
 
 ---
 
-Thank you for using Pygo. We hope this library enhances your concurrent and asynchronous programming experience in Python. Happy coding!
+Thank you for using Pygo. We hope this library enhances your concurrent and asynchronous programming experience in Python. Happy coding!
```

### Comparing `aio-pygo-1.0.1/aio_pygo.egg-info/PKG-INFO` & `aio-pygo-1.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-Metadata-Version: 2.1
-Name: aio-pygo
-Version: 1.0.1
-Summary: Write Python code in a Go-like fashion.
-Author: Gael Lz
-Project-URL: Homepage, https://github.com/GaelLnz/pygo
-Project-URL: Bug Tracker, https://github.com/GaelLnz/pygo/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Pygo
 
+[![PyPI version](https://badge.fury.io/py/aio-pygo.svg)](https://badge.fury.io/py/aio-pygo) [![codecov](https://codecov.io/gh/GaelLnz/pygo/branch/main/graph/badge.svg?token=PPVXA3VIQB)](https://codecov.io/gh/GaelLnz/pygo)
+
 Pygo is fully typed & zero dependency Python library that enables you to code in a Go-like fashion. It brings some of the key features from the Go programming language such as goroutines and channels.
 
 ## Features
 
 - **Goroutines**: Execute functions concurrently using asyncio coroutines.
 - **Channels**: Enable communication and synchronization between coroutines using channels.
 - **Select Statement**: Choose the first ready communication operation from multiple channels.
@@ -34,15 +22,15 @@
 
 ## Usage
 
 ### Goroutines
 
 ```python
 from asyncio import run
-from python-go import go
+from pygo import go
 
 async def worker():
     # some async operations
     ...
 
 async def main():
     # Start a goroutine
@@ -55,25 +43,25 @@
     run(main())
 ```
 
 ### Channels
 
 ```python
 from asyncio import run
-from python-go import Chan
+from pygo import Chan
 
 async def main():
     # Create a channel
     ch = Chan[str]()
 
     # Send data to the channel
-    ch.send("Hello, Pygo!")
+    await ch.send("Hello, Pygo!")
 
     # Receive data from the channel
-    data = ch.receive()
+    data, _ = await ch.receive()
     print(data)
 
 if __name__ == "__main__":
     run(main())
 ```
 
 ### And more
@@ -101,8 +89,8 @@
 
 ## License
 
 Pygo is licensed under the GPL 3.0 License. See the [LICENSE](LICENSE) file for more details.
 
 ---
 
-Thank you for using Pygo. We hope this library enhances your concurrent and asynchronous programming experience in Python. Happy coding!
+Thank you for using Pygo. We hope this library enhances your concurrent and asynchronous programming experience in Python. Happy coding!
```

### Comparing `aio-pygo-1.0.1/pygo/chan.py` & `aio-pygo-1.0.2/pygo/chan.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,12 @@
+from asyncio import sleep
 from asyncio.queues import Queue, QueueEmpty
-
 from typing import Any, Generic, TypeVar
 from uuid import uuid4
 
-from asyncio import sleep
-
-
 ChanType = TypeVar("ChanType")
 
 
 class Chan(Generic[ChanType]):
     class Empty(Exception):
         ...
```

### Comparing `aio-pygo-1.0.1/pygo/chan_test.py` & `aio-pygo-1.0.2/pygo/chan_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pytest import raises
+
 from pygo.chan import Chan, select
 from pygo.defer import deferrer
 from pygo.go import go
 
 
 class TestClose:
     async def test_close(self):
```

### Comparing `aio-pygo-1.0.1/pygo/defer.py` & `aio-pygo-1.0.2/pygo/defer.py`

 * *Files identical despite different names*

### Comparing `aio-pygo-1.0.1/pygo/defer_test.py` & `aio-pygo-1.0.2/pygo/defer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pytest import raises
+
 from pygo.defer import deferrer
 
 
 class TestDefer:
     async def test_defer(self):
         actual = []
         with deferrer() as d:
```

### Comparing `aio-pygo-1.0.1/pygo/go.py` & `aio-pygo-1.0.2/pygo/go.py`

 * *Files identical despite different names*

### Comparing `aio-pygo-1.0.1/pygo/go_test.py` & `aio-pygo-1.0.2/pygo/go_test.py`

 * *Files identical despite different names*

### Comparing `aio-pygo-1.0.1/pyproject.toml` & `aio-pygo-1.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aio-pygo"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Gael Lz" },
 ]
 description = "Write Python code in a Go-like fashion."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -17,8 +17,11 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/GaelLnz/pygo"
 "Bug Tracker" = "https://github.com/GaelLnz/pygo/issues"
 
 [tool.coverage.run]
-omit = ["*/*_test.py"]
+omit = ["*/*_test.py"]
+
+[tool.isort]
+profile = "black"
```

