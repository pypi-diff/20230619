# Comparing `tmp/wasmpy-0.1.0a2.tar.gz` & `tmp/wasmpy-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wasmpy-0.1.0a2.tar", last modified: Sun Nov  8 22:41:13 2020, max compression
+gzip compressed data, was "dist\wasmpy-0.1.0a3.tar", last modified: Mon Dec 14 17:36:31 2020, max compression
```

## Comparing `wasmpy-0.1.0a2.tar` & `wasmpy-0.1.0a3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2020-11-08 22:41:13.278238 wasmpy-0.1.0a2/
--rw-rw-rw-   0        0        0     1944 2020-11-08 22:41:13.278238 wasmpy-0.1.0a2/PKG-INFO
--rw-rw-rw-   0        0        0      867 2020-11-05 18:16:47.000000 wasmpy-0.1.0a2/README.md
--rw-rw-rw-   0        0        0       42 2020-11-08 22:41:13.278238 wasmpy-0.1.0a2/setup.cfg
--rw-rw-rw-   0        0        0      915 2020-11-08 22:40:16.000000 wasmpy-0.1.0a2/setup.py
-drwxrwxrwx   0        0        0        0 2020-11-08 22:41:13.028183 wasmpy-0.1.0a2/wasmpy/
--rw-rw-rw-   0        0        0      107 2020-11-04 21:55:34.000000 wasmpy-0.1.0a2/wasmpy/__init__.py
--rw-rw-rw-   0        0        0     1425 2020-11-04 22:01:23.000000 wasmpy-0.1.0a2/wasmpy/hooks.py
--rw-rw-rw-   0        0        0    13069 2020-11-01 13:00:45.000000 wasmpy-0.1.0a2/wasmpy/instructions.py
--rw-rw-rw-   0        0        0     2239 2020-10-30 18:29:36.000000 wasmpy-0.1.0a2/wasmpy/module.py
--rw-rw-rw-   0        0        0     5335 2020-10-30 18:30:06.000000 wasmpy-0.1.0a2/wasmpy/sections.py
--rw-rw-rw-   0        0        0     2440 2020-10-30 18:24:54.000000 wasmpy-0.1.0a2/wasmpy/types.py
--rw-rw-rw-   0        0        0     2017 2020-11-05 17:20:20.000000 wasmpy-0.1.0a2/wasmpy/values.py
-drwxrwxrwx   0        0        0        0 2020-11-08 22:41:13.215733 wasmpy-0.1.0a2/wasmpy.egg-info/
--rw-rw-rw-   0        0        0     1944 2020-11-08 22:41:12.000000 wasmpy-0.1.0a2/wasmpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2020-11-08 22:41:12.000000 wasmpy-0.1.0a2/wasmpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-11-08 22:41:12.000000 wasmpy-0.1.0a2/wasmpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2020-11-08 22:41:12.000000 wasmpy-0.1.0a2/wasmpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2020-12-14 17:36:31.141759 wasmpy-0.1.0a3/
+-rw-rw-rw-   0        0        0     1944 2020-12-14 17:36:31.139746 wasmpy-0.1.0a3/PKG-INFO
+-rw-rw-rw-   0        0        0      867 2020-11-05 18:16:47.000000 wasmpy-0.1.0a3/README.md
+-rw-rw-rw-   0        0        0       42 2020-12-14 17:36:31.142740 wasmpy-0.1.0a3/setup.cfg
+-rw-rw-rw-   0        0        0      915 2020-12-14 17:35:25.000000 wasmpy-0.1.0a3/setup.py
+drwxrwxrwx   0        0        0        0 2020-12-14 17:36:31.099748 wasmpy-0.1.0a3/wasmpy/
+-rw-rw-rw-   0        0        0      107 2020-11-04 21:55:34.000000 wasmpy-0.1.0a3/wasmpy/__init__.py
+-rw-rw-rw-   0        0        0     1380 2020-12-13 19:02:16.000000 wasmpy-0.1.0a3/wasmpy/hooks.py
+-rw-rw-rw-   0        0        0    13675 2020-12-14 17:27:49.000000 wasmpy-0.1.0a3/wasmpy/instructions.py
+-rw-rw-rw-   0        0        0     2239 2020-10-30 18:29:36.000000 wasmpy-0.1.0a3/wasmpy/module.py
+-rw-rw-rw-   0        0        0     5316 2020-12-14 17:27:49.000000 wasmpy-0.1.0a3/wasmpy/sections.py
+-rw-rw-rw-   0        0        0     2440 2020-12-14 16:55:31.000000 wasmpy-0.1.0a3/wasmpy/types.py
+-rw-rw-rw-   0        0        0     2105 2020-12-14 17:27:49.000000 wasmpy-0.1.0a3/wasmpy/values.py
+drwxrwxrwx   0        0        0        0 2020-12-14 17:36:31.136754 wasmpy-0.1.0a3/wasmpy.egg-info/
+-rw-rw-rw-   0        0        0     1944 2020-12-14 17:36:30.000000 wasmpy-0.1.0a3/wasmpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2020-12-14 17:36:30.000000 wasmpy-0.1.0a3/wasmpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-12-14 17:36:30.000000 wasmpy-0.1.0a3/wasmpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2020-12-14 17:36:30.000000 wasmpy-0.1.0a3/wasmpy.egg-info/top_level.txt
```

### Comparing `wasmpy-0.1.0a2/PKG-INFO` & `wasmpy-0.1.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasmpy
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: Interactions between WebAssembly and Python
 Home-page: https://github.com/r-james-dev/wasmpy
 Author: James Ryan
 Author-email: r.james.dev@gmail.com
 License: MIT
 Description: # WasmPy
         Interacting with WebAssembly code from python.
```

### Comparing `wasmpy-0.1.0a2/README.md` & `wasmpy-0.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.0a2/setup.py` & `wasmpy-0.1.0a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fp:
     description = fp.read()
 
 setuptools.setup(
     name="wasmpy",
-    version="0.1.0a2",
+    version="0.1.0a3",
     author="James Ryan",
     author_email="r.james.dev@gmail.com",
     description="Interactions between WebAssembly and Python",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/r-james-dev/wasmpy",
     packages=["wasmpy"],
```

### Comparing `wasmpy-0.1.0a2/wasmpy/hooks.py` & `wasmpy-0.1.0a3/wasmpy/hooks.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from .module import read_module
-import os, sys, types
-
-class WebAssemblyBinaryLoader(object):
-    """WebAssembly binary import hook.
-    This hook is registered automatically with `import wasmpy`.
-    After the initial import a WebAssembly binary format file (.wasm) can
-    be loaded with the import statement eg:
-    |- mymodule
-    |  |- mymodule_2.wasm
-    |
-    |- mymodule_1.wasm
-    |- example.py
-    in example.py:
-    ```
-    import wasmpy
-    import mymodule_1
-    from mymodule import mymodule_2
-    ``` Will load both binary files.
-    """
-    def find_module(self, fullname, path=None):
-        fname = fullname.split(".")[-1] + ".wasm"
-        if path is not None and len(path):
-            for p in path:
-                if os.path.isfile(os.path.join(p, fname)):
-                    self.fname = os.path.join(p, fname)
-                    return self
-
-        elif len(fullname.split(".")) < 2 and os.path.isfile(fname):
-            self.fname = os.path.abspath(fname)
-            return self
-
-    def load_module(self, fullname):
-        if fullname in sys.modules:
-            return
-
-        mod = types.ModuleType(fullname)
-        mod.__file__ = self.fname
-        mod.__name__ = fullname
-        mod.__loader__ = self
-        sys.modules[fullname] = mod
-        with open(self.fname, "rb") as fp:
-            mod.module = read_module(fp)
-
-        return mod
+from .module import read_module
+import os, sys, types
+
+class WebAssemblyBinaryLoader(object):
+    """WebAssembly binary import hook.
+    This hook is registered automatically with `import wasmpy`.
+    After the initial import a WebAssembly binary format file (.wasm) can
+    be loaded with the import statement eg:
+    |- mymodule
+    |  |- mymodule_2.wasm
+    |
+    |- mymodule_1.wasm
+    |- example.py
+    in example.py:
+    ```
+    import wasmpy
+    import mymodule_1
+    from mymodule import mymodule_2
+    ``` Will load both binary files.
+    """
+    def find_module(self, fullname, path=None):
+        fname = fullname.split(".")[-1] + ".wasm"
+        if path is not None and len(path):
+            for p in path:
+                if os.path.isfile(os.path.join(p, fname)):
+                    self.fname = os.path.join(p, fname)
+                    return self
+
+        elif len(fullname.split(".")) < 2 and os.path.isfile(fname):
+            self.fname = os.path.abspath(fname)
+            return self
+
+    def load_module(self, fullname):
+        if fullname in sys.modules:
+            return
+
+        mod = types.ModuleType(fullname)
+        mod.__file__ = self.fname
+        mod.__name__ = fullname
+        mod.__loader__ = self
+        sys.modules[fullname] = mod
+        with open(self.fname, "rb") as fp:
+            mod.module = read_module(fp)
+
+        return mod
```

### Comparing `wasmpy-0.1.0a2/wasmpy/instructions.py` & `wasmpy-0.1.0a3/wasmpy/instructions.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,35 +37,62 @@
     if data == b"\0":
         return "unreachable"
 
     if data == b"\x01":
         return "nop"
 
     if data == b"\x02":
-        rt = read_valtype(buffer)
+        try:
+            rt = read_valtype(buffer)
+
+        except TypeError:
+            buffer.seek(-1, 1)
+            if buffer.read(1)[0] != 64:
+                raise TypeError("Invalid blocktype.")
+
+            rt = None
+
         in_ = []
         instruction = read_instruction(buffer)
         while instruction != "end":
             in_.append(instruction)
             instruction = read_instruction(buffer)
 
         return "block", rt, tuple(in_), "end"
 
     if data == b"\x03":
-        rt = read_valtype(buffer)
+        try:
+            rt = read_valtype(buffer)
+
+        except TypeError:
+            buffer.seek(-1, 1)
+            if buffer.read(1)[0] != 64:
+                raise TypeError("Invalid blocktype.")
+
+            rt = None
+
         in_ = []
         instruction = read_instruction(buffer)
         while instruction != "end":
             in_.append(instruction)
             instruction = read_instruction(buffer)
 
         return "loop", rt, tuple(in_), "end"
 
     if data == b"\x04":
-        rt = read_valtype(buffer)
+        try:
+            rt = read_valtype(buffer)
+
+        except TypeError:
+            buffer.seek(-1, 1)
+            if buffer.read(1)[0] != 64:
+                raise TypeError("Invalid blocktype.")
+
+            rt = None
+
         in1 = []
         instruction = read_instruction(buffer)
         while instruction not in ["end", "else"]:
             in1.append(instruction)
             instruction = read_instruction(buffer)
 
         in1 = tuple(in1)
@@ -208,15 +235,15 @@
 
     # Numeric instructions
     # https://www.w3.org/TR/wasm-core-1/#numeric-instructions%E2%91%A6
     if data == b"\x41":
         return "i32.const", read_sint(buffer, 32)
 
     if data == b"\x42":
-        return "i64.const", read_sint(buffer, 32)
+        return "i64.const", read_sint(buffer, 64)
 
     if data == b"\x43":
         return "f32.const", read_f32(buffer)
 
     if data == b"\x44":
         return "f64.const", read_f64(buffer)
```

### Comparing `wasmpy-0.1.0a2/wasmpy/module.py` & `wasmpy-0.1.0a3/wasmpy/module.py`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.0a2/wasmpy/sections.py` & `wasmpy-0.1.0a3/wasmpy/sections.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         for _ in range(get_vec_len(buffer)):
             size = read_uint(buffer, 32)
             start = buffer.tell()
 
             t = ()
             for _ in range(get_vec_len(buffer)):
                 n = read_uint(buffer, 32)
-                t += tuple(read_valtype(buffer) for _ in range(n))
+                t += ((read_valtype(buffer),),)
 
             concat_t = ()
             for locals in t:
                 concat_t += locals
 
             code += ((concat_t, read_expr(buffer)),)
             end = buffer.tell()
```

### Comparing `wasmpy-0.1.0a2/wasmpy/types.py` & `wasmpy-0.1.0a3/wasmpy/types.py`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.0a2/wasmpy/values.py` & `wasmpy-0.1.0a3/wasmpy/values.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,28 +33,30 @@
 
     return result
 
 
 def read_sint(buffer, bits):
     """Read a signed integer stored in LEB128 format."""
     # https://www.w3.org/TR/wasm-core-1/#integers%E2%91%A4
-    shift = 0
-    byte = buffer.read(1)[0]
-    result = byte & 127
-    consumed_bytes = 1
-
-    byte = buffer.read(1)[0]
-    while byte >> 7:
-        consumed_bytes += 1
-        assert consumed_bytes <= math.ceil(bits / 7), "Invalid integer"
-        result |= (byte & 127) << shift
-        shift += 7
+    try:
         byte = buffer.read(1)[0]
+        consumed_bytes = 1
+        result = byte & 127
+        shift = 7
+        while byte >> 7:
+            byte = buffer.read(1)[0]
+            consumed_bytes += 1
+            assert consumed_bytes <= math.ceil(bits / 7)
+            result |= (byte & 127) << shift
+            shift += 7
 
-    if shift < bits and (byte >> 6) & 1:
+    except (AssertionError, IndexError):
+        raise TypeError("Invalid integer.")
+
+    if result >> consumed_bytes * 7 - 1:
         result |= ~0 << shift
 
     return result
 
 
 def read_f32(buffer):
     """Read a single precision float from buffer."""
```

### Comparing `wasmpy-0.1.0a2/wasmpy.egg-info/PKG-INFO` & `wasmpy-0.1.0a3/wasmpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasmpy
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: Interactions between WebAssembly and Python
 Home-page: https://github.com/r-james-dev/wasmpy
 Author: James Ryan
 Author-email: r.james.dev@gmail.com
 License: MIT
 Description: # WasmPy
         Interacting with WebAssembly code from python.
```

