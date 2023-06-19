# Comparing `tmp/qps_limit-0.1.1-py3.8.egg` & `tmp/qps_limit-0.1.2-py3.8.egg`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7193 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      723 b- defN 23-Jun-18 23:37 EGG-INFO/PKG-INFO
--rw-rw-r--  2.0 unx      243 b- defN 23-Jun-18 23:37 EGG-INFO/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-18 23:37 EGG-INFO/dependency_links.txt
--rw-rw-r--  2.0 unx       11 b- defN 23-Jun-18 23:37 EGG-INFO/requires.txt
--rw-rw-r--  2.0 unx       10 b- defN 23-Jun-18 23:37 EGG-INFO/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-18 23:37 EGG-INFO/zip-safe
--rw-rw-r--  2.0 unx       77 b- defN 23-Jun-18 23:36 qps_limit/__init__.py
+Zip file size: 7660 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx     1620 b- defN 23-Jun-19 10:20 EGG-INFO/PKG-INFO
+-rw-rw-r--  2.0 unx      243 b- defN 23-Jun-19 10:20 EGG-INFO/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-19 10:20 EGG-INFO/dependency_links.txt
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jun-19 10:20 EGG-INFO/requires.txt
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jun-19 10:20 EGG-INFO/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-19 10:20 EGG-INFO/zip-safe
+-rw-rw-r--  2.0 unx       77 b- defN 23-Jun-19 10:16 qps_limit/__init__.py
 -rw-rw-r--  2.0 unx     7483 b- defN 23-Jun-18 23:36 qps_limit/wrapper.py
--rw-rw-r--  2.0 unx      229 b- defN 23-Jun-18 23:37 qps_limit/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--  2.0 unx     7692 b- defN 23-Jun-18 23:37 qps_limit/__pycache__/wrapper.cpython-38.pyc
-10 files, 16470 bytes uncompressed, 5899 bytes compressed:  64.2%
+-rw-rw-r--  2.0 unx      229 b- defN 23-Jun-19 10:20 qps_limit/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx     7692 b- defN 23-Jun-19 10:20 qps_limit/__pycache__/wrapper.cpython-38.pyc
+10 files, 17367 bytes uncompressed, 6366 bytes compressed:  63.3%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qps-limit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Run functions under any limited rate
 Home-page: https://github.com/antct/rate-limit
 Author: tt
 Author-email: 527892245@qq.com
 License: GPLv2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -12,7 +12,63 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
+Description-Content-Type: text/markdown
+
+## Rate Limit
+
+Run functions under any limited rate using `multiprocessing` + `asyncio`
+
+### Installation
+
+```bash
+pip install qps-limit
+```
+
+or install manually via git
+
+```bash
+git clone git://github.com/antct/rate-limit.git rate-limit
+cd rate-limit
+python setup.py install
+```
+
+### Example
+
+> 10 workers, each with a maximum qps of 10, to calculate the function value of `(1+1/n)^n`
+
+```python
+from qps_limit import MWrapper
+
+
+async def func(n: int):
+    return 1 + 1 / n, n
+
+
+def params():
+    for n in range(1, 1001):
+        yield (), {"n": n}
+
+
+def callback(r):
+    return r[0] ** r[1]
+
+
+engine = MWrapper(
+    func=func,
+    params=params(),
+    num_workers=10,
+    worker_max_qps=10,
+    streaming=False,
+    callback=callback,
+    progress=True
+)
+
+for i, r in engine.start():
+    print(i, r)
+```
+
+> elapsed time: 10.11s average qps: 98.96/100.00
```

## qps_limit/__init__.py

```diff
@@ -1,5 +1,5 @@
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 
 from .wrapper import MWrapper
 
 __all__ = ['MWrapper']
```

## qps_limit/__pycache__/__init__.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sun Jun 18 15:36:53 2023 UTC, .py size: 77 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,13 +1,13 @@
-00000000: 550d 0d0a 0000 0000 9524 8f64 4d00 0000  U........$.dM...
+00000000: 550d 0d0a 0000 0000 94ba 8f64 4d00 0000  U..........dM...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6403  Z.d.d.l.m.Z...d.
 00000040: 6701 5a03 6404 5300 2905 7a05 302e 312e  g.Z.d.S.).z.0.1.
-00000050: 31e9 0100 0000 2901 da08 4d57 7261 7070  1.....)...MWrapp
+00000050: 32e9 0100 0000 2901 da08 4d57 7261 7070  2.....)...MWrapp
 00000060: 6572 7202 0000 004e 2904 da0b 5f5f 7665  err....N)...__ve
 00000070: 7273 696f 6e5f 5fda 0777 7261 7070 6572  rsion__..wrapper
 00000080: 7202 0000 00da 075f 5f61 6c6c 5f5f a900  r......__all__..
 00000090: 7206 0000 0072 0600 0000 fa32 6275 696c  r....r.....2buil
 000000a0: 642f 6264 6973 742e 6c69 6e75 782d 7838  d/bdist.linux-x8
 000000b0: 365f 3634 2f65 6767 2f71 7073 5f6c 696d  6_64/egg/qps_lim
 000000c0: 6974 2f5f 5f69 6e69 745f 5f2e 7079 da08  it/__init__.py..
```

