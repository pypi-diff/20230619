# Comparing `tmp/signal-slot-mp-1.0.3.tar.gz` & `tmp/signal-slot-mp-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal-slot-mp-1.0.3.tar", last modified: Tue Aug 30 09:13:04 2022, max compression
+gzip compressed data, was "signal-slot-mp-1.0.5.tar", last modified: Mon Jun 19 04:31:39 2023, max compression
```

## Comparing `signal-slot-mp-1.0.3.tar` & `signal-slot-mp-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2022-08-30 09:13:04.428145 signal-slot-mp-1.0.3/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1073 2022-07-21 08:56:03.000000 signal-slot-mp-1.0.3/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     1980 2022-08-30 09:13:04.428145 signal-slot-mp-1.0.3/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1351 2022-08-30 09:11:54.000000 signal-slot-mp-1.0.3/README.md
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2022-08-30 09:13:04.428145 signal-slot-mp-1.0.3/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1230 2022-08-30 09:11:02.000000 signal-slot-mp-1.0.3/setup.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2022-08-30 09:13:04.428145 signal-slot-mp-1.0.3/signal_slot/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-07-21 08:56:45.000000 signal-slot-mp-1.0.3/signal_slot/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3251 2022-07-21 09:23:41.000000 signal-slot-mp-1.0.3/signal_slot/queue_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    19024 2022-08-30 09:12:56.000000 signal-slot-mp-1.0.3/signal_slot/signal_slot.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      973 2022-08-22 02:00:14.000000 signal-slot-mp-1.0.3/signal_slot/utils.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2022-08-30 09:13:04.428145 signal-slot-mp-1.0.3/signal_slot_mp.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1980 2022-08-30 09:13:04.000000 signal-slot-mp-1.0.3/signal_slot_mp.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      380 2022-08-30 09:13:04.000000 signal-slot-mp-1.0.3/signal_slot_mp.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2022-08-30 09:13:04.000000 signal-slot-mp-1.0.3/signal_slot_mp.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       78 2022-08-30 09:13:04.000000 signal-slot-mp-1.0.3/signal_slot_mp.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       18 2022-08-30 09:13:04.000000 signal-slot-mp-1.0.3/signal_slot_mp.egg-info/top_level.txt
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2022-08-30 09:13:04.428145 signal-slot-mp-1.0.3/tests/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-07-21 08:57:23.000000 signal-slot-mp-1.0.3/tests/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5327 2022-08-30 09:12:56.000000 signal-slot-mp-1.0.3/tests/test_signal_slot.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 04:31:39.752252 signal-slot-mp-1.0.5/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1073 2023-02-28 06:09:03.000000 signal-slot-mp-1.0.5/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6918 2023-06-19 04:31:39.752252 signal-slot-mp-1.0.5/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6289 2023-06-19 04:19:46.000000 signal-slot-mp-1.0.5/README.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-19 04:31:39.752252 signal-slot-mp-1.0.5/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1279 2023-06-19 04:07:11.000000 signal-slot-mp-1.0.5/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 04:31:39.752252 signal-slot-mp-1.0.5/signal_slot/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 06:09:03.000000 signal-slot-mp-1.0.5/signal_slot/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3168 2023-02-28 06:09:35.000000 signal-slot-mp-1.0.5/signal_slot/queue_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    19024 2023-02-28 06:09:03.000000 signal-slot-mp-1.0.5/signal_slot/signal_slot.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      973 2023-02-28 06:09:03.000000 signal-slot-mp-1.0.5/signal_slot/utils.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 04:31:39.752252 signal-slot-mp-1.0.5/signal_slot_mp.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6918 2023-06-19 04:31:39.000000 signal-slot-mp-1.0.5/signal_slot_mp.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      406 2023-06-19 04:31:39.000000 signal-slot-mp-1.0.5/signal_slot_mp.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-19 04:31:39.000000 signal-slot-mp-1.0.5/signal_slot_mp.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-06-19 04:31:39.000000 signal-slot-mp-1.0.5/signal_slot_mp.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       18 2023-06-19 04:31:39.000000 signal-slot-mp-1.0.5/signal_slot_mp.egg-info/top_level.txt
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 04:31:39.752252 signal-slot-mp-1.0.5/tests/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 06:09:03.000000 signal-slot-mp-1.0.5/tests/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7586 2023-02-28 09:08:55.000000 signal-slot-mp-1.0.5/tests/test_signal_slot.py
```

### Comparing `signal-slot-mp-1.0.3/LICENSE` & `signal-slot-mp-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `signal-slot-mp-1.0.3/setup.py` & `signal-slot-mp-1.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
+import os
+
 import setuptools
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
     descr_lines = long_description.split("\n")
     long_description = "\n".join(descr_lines)
 
 
+queue_deps = ["faster-fifo>=1.4.4,<2.0"] if os.name != "nt" else []
+
+
 setup(
     # Information
     name="signal-slot-mp",
     description="Fast and compact framework for communication between threads and processes in Python using event loops, signals and slots.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.0.3",
+    version="1.0.5",
     url="https://github.com/alex-petrenko/signal-slot",
     author="Aleksei Petrenko",
     license="MIT",
     keywords="asynchronous multithreading multiprocessing queue faster-fifo signal slot event loop",
     project_urls={
         "Github": "https://github.com/alex-petrenko/signal-slot",
         "Sample Factory": "https://github.com/alex-petrenko/sample-factory",
     },
-    install_requires=[
-        "faster-fifo>=1.4.2,<2.0",
-    ],
+    install_requires=queue_deps,
     extras_require={
         "dev": ["black", "isort", "pytest<8.0", "flake8", "pre-commit", "twine"],
     },
     package_dir={"": "./"},
     packages=setuptools.find_packages(where="./", include="signal_slot*"),
     include_package_data=True,
     python_requires=">=3.8",
```

### Comparing `signal-slot-mp-1.0.3/signal_slot/queue_utils.py` & `signal-slot-mp-1.0.5/signal_slot/queue_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,14 @@
         return get_mp_queue(buffer_size_bytes)
 
 
 def get_mp_queue(buffer_size_bytes=1_000_000):
     if os.name == "nt":
         MpQueue = MpQueueWrapper
     else:
-        # noinspection PyUnresolvedReferences
-        import faster_fifo_reduction
         from faster_fifo import Queue as MpQueue
 
     return MpQueue(max_size_bytes=buffer_size_bytes)
 
 
 class QueueWrapper(Queue):
     def get_many(self, block=True, timeout=float(1e3), max_messages_to_get=int(1e9)):
```

### Comparing `signal-slot-mp-1.0.3/signal_slot/signal_slot.py` & `signal-slot-mp-1.0.5/signal_slot/signal_slot.py`

 * *Files identical despite different names*

### Comparing `signal-slot-mp-1.0.3/signal_slot/utils.py` & `signal-slot-mp-1.0.5/signal_slot/utils.py`

 * *Files identical despite different names*

### Comparing `signal-slot-mp-1.0.3/tests/test_signal_slot.py` & `signal-slot-mp-1.0.5/tests/test_signal_slot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import datetime
 import logging
 import multiprocessing
+import time
+from queue import Empty
 
 import pytest
 
+from signal_slot.queue_utils import get_mp_queue
 from signal_slot.signal_slot import EventLoop, EventLoopObject, EventLoopProcess, Timer, log, process_name, signal
 
 logging.basicConfig(level=logging.NOTSET)
 
 
 class C1(EventLoopObject):
     def __init__(self, event_loop, object_id):
@@ -197,7 +200,87 @@
     # emitting lots of signals before starting the event loop - this should lead to queue overflow
     # most of these signals are lost because of queue overflow, but we should not crash
     lots_of_data = [42] * 100000
     for i in range(100):
         emitter.foo_signal.emit(lots_of_data)
     for i in range(5000):
         emitter.foo_signal.emit(i)
+
+
+now = datetime.datetime.now
+
+
+# classes derived from EventLoopObject define signals and slots (actually any method can be a slot)
+class A(EventLoopObject):
+    @signal
+    def signal_a(self):
+        ...
+
+    def on_signal_b(self, msg: str):
+        print(f"{now()} {self.object_id} received signal_b: {msg}")
+        time.sleep(1)
+        self.signal_a.emit("hello from A", 42)
+
+
+class B(EventLoopObject):
+    @signal
+    def signal_b(self):
+        ...
+
+    def on_signal_a(self, msg: str, other_data: int):
+        print(f"{now()} {self.object_id} received signal_a: {msg} {other_data}")
+        time.sleep(1)
+        self.signal_b.emit("hello from B")
+
+
+def test_usage_example():
+    # create main event loop and object of type A
+    main_event_loop = EventLoop("main_loop")
+    a = A(main_event_loop, "object: a")
+
+    # create a background process with a separate event loop and object b that lives on that event loop
+    bg_process = EventLoopProcess(unique_process_name="background_process")
+    b = B(bg_process.event_loop, "object: b")
+
+    # connect signals and slots
+    a.signal_a.connect(b.on_signal_a)
+    b.signal_b.connect(a.on_signal_b)
+
+    # emit signal from a to kick off the communication
+    a.signal_a.emit("Initial hello from A", 1337)
+
+    # create a timer that will stop our system after 10 seconds
+    stop_timer = Timer(main_event_loop, 10.0, single_shot=True)
+    stop_timer.start()
+
+    # connect the stop method of the event loop to the timeout signal of the timer
+    stop_timer.timeout.connect(main_event_loop.stop)
+    stop_timer.timeout.connect(bg_process.stop)  # stops the event loop of the background process
+
+    # start the background process
+    bg_process.start()
+
+    # start the main event loop
+    main_event_loop.exec()
+
+    # if we get here, the main event loop has stopped
+    # wait for the background process to finish
+    bg_process.join()
+
+    print(f"{now()} Done!")
+
+
+def test_queue_get_many():
+    q = get_mp_queue()
+
+    q.put(1)
+    q.put(2)
+    q.put(3)
+
+    msgs = []
+    while True:
+        try:
+            msgs.extend(q.get_many_nowait())
+        except Empty:
+            break
+
+    assert msgs == [1, 2, 3]
```

