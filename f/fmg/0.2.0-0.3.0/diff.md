# Comparing `tmp/fmg-0.2.0.tar.gz` & `tmp/fmg-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmg-0.2.0.tar", last modified: Tue May 23 02:53:33 2023, max compression
+gzip compressed data, was "fmg-0.3.0.tar", last modified: Mon Jun 19 08:49:29 2023, max compression
```

## Comparing `fmg-0.2.0.tar` & `fmg-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 02:53:33.194414 fmg-0.2.0/
--rw-rw-rw-   0        0        0     1060 2019-08-27 18:29:08.000000 fmg-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 fmg-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      770 2023-05-23 02:53:33.194414 fmg-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-05-23 02:07:31.000000 fmg-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 02:53:33.164577 fmg-0.2.0/fmg/
--rw-rw-rw-   0        0        0      180 2023-05-23 01:58:56.000000 fmg-0.2.0/fmg/__init__.py
--rw-rw-rw-   0        0        0       63 2023-05-23 02:53:21.000000 fmg-0.2.0/fmg/__version__.py
--rw-rw-rw-   0        0        0     8864 2023-05-23 02:51:34.000000 fmg-0.2.0/fmg/core.py
-drwxrwxrwx   0        0        0        0 2023-05-23 02:53:33.194414 fmg-0.2.0/fmg.egg-info/
--rw-rw-rw-   0        0        0      770 2023-05-23 02:53:33.000000 fmg-0.2.0/fmg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-23 02:53:33.000000 fmg-0.2.0/fmg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 02:53:33.000000 fmg-0.2.0/fmg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-23 02:53:33.000000 fmg-0.2.0/fmg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-23 02:53:33.000000 fmg-0.2.0/fmg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 02:53:33.194414 fmg-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     3791 2023-05-23 02:53:21.000000 fmg-0.2.0/setup.py
+drwxrwxrwx   0 khtao     (1000) khtao     (1000)        0 2023-06-19 08:49:29.921433 fmg-0.3.0/
+-rwxrwxrwx   0 khtao     (1000) khtao     (1000)     1060 2019-08-27 18:29:08.000000 fmg-0.3.0/LICENSE
+-rwxrwxrwx   0 khtao     (1000) khtao     (1000)       26 2019-08-27 18:29:08.000000 fmg-0.3.0/MANIFEST.in
+-rwxrwxrwx   0 khtao     (1000) khtao     (1000)      768 2023-06-19 08:49:29.921075 fmg-0.3.0/PKG-INFO
+-rwxrwxrwx   0 khtao     (1000) khtao     (1000)      120 2023-05-23 02:07:31.000000 fmg-0.3.0/README.md
+drwxrwxrwx   0 khtao     (1000) khtao     (1000)        0 2023-06-19 08:49:29.914315 fmg-0.3.0/fmg/
+-rwxrwxrwx   0 khtao     (1000) khtao     (1000)      180 2023-05-23 01:58:56.000000 fmg-0.3.0/fmg/__init__.py
+-rwxrwxrwx   0 khtao     (1000) khtao     (1000)       63 2023-06-19 08:47:07.000000 fmg-0.3.0/fmg/__version__.py
+-rwxrwxrwx   0 khtao     (1000) khtao     (1000)     8949 2023-06-19 02:47:47.000000 fmg-0.3.0/fmg/core.py
+drwxrwxrwx   0 khtao     (1000) khtao     (1000)        0 2023-06-19 08:49:29.919805 fmg-0.3.0/fmg.egg-info/
+-rwxrwxrwx   0 khtao     (1000) khtao     (1000)      768 2023-06-19 08:49:29.000000 fmg-0.3.0/fmg.egg-info/PKG-INFO
+-rwxrwxrwx   0 khtao     (1000) khtao     (1000)      219 2023-06-19 08:49:29.000000 fmg-0.3.0/fmg.egg-info/SOURCES.txt
+-rwxrwxrwx   0 khtao     (1000) khtao     (1000)        1 2023-06-19 08:49:29.000000 fmg-0.3.0/fmg.egg-info/dependency_links.txt
+-rwxrwxrwx   0 khtao     (1000) khtao     (1000)       32 2023-06-19 08:49:29.000000 fmg-0.3.0/fmg.egg-info/requires.txt
+-rwxrwxrwx   0 khtao     (1000) khtao     (1000)        4 2023-06-19 08:49:29.000000 fmg-0.3.0/fmg.egg-info/top_level.txt
+-rwxrwxrwx   0 khtao     (1000) khtao     (1000)       38 2023-06-19 08:49:29.921606 fmg-0.3.0/setup.cfg
+-rwxrwxrwx   0 khtao     (1000) khtao     (1000)     3791 2023-06-19 02:48:42.000000 fmg-0.3.0/setup.py
```

### Comparing `fmg-0.2.0/LICENSE` & `fmg-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fmg-0.2.0/PKG-INFO` & `fmg-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-Metadata-Version: 2.1
-Name: fmg
-Version: 0.2.0
-Summary: Fast Memory Graphics for big image, use like OpenSlide
-Home-page: https://github.com/khtao/fmg
-Author: khtao
-Author-email: khtao@live.cn
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# Fast Memory Graphics for big image
-
-Fast Memory Graphics is a big image type based on lmdb and can use like OpenSlide
+Metadata-Version: 2.1
+Name: fmg
+Version: 0.3.0
+Summary: Fast Memory Graphics for big image, use like OpenSlide
+Home-page: https://github.com/khtao/fmg
+Author: khtao
+Author-email: khtao@live.cn
+License: MIT
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# Fast Memory Graphics for big image
+
+Fast Memory Graphics is a big image type based on lmdb and can use like OpenSlide
+
+
```

### Comparing `fmg-0.2.0/fmg/core.py` & `fmg-0.3.0/fmg/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,30 +85,29 @@
     def __init__(self, filename, mode='r'):
         """Open a whole-slide image."""
         AbstractSlide.__init__(self)
         self._filename = filename
         self._mode = mode
         if mode == 'r':
             self._osr = json.load(open(filename))
-            self._data = [lmdb.open(os.path.join(self._filename[:-4], 'level' + str(i)))
+            self._data = [lmdb.open(os.path.join(self._filename[:-4], 'level' + str(i))).begin()
                           for i in range(self.level_count)]
-            self.check_data()
+            # self.check_data()
         elif mode == 'w':
-
             pass
 
-    def check_data(self):
-        for i in range(self.level_count):
-            txn = self._data[i].begin()
-            dimension = txn.get(key='dimension'.encode())
-            if dimension is not None:
-                dimension_w = dimension.decode()
-                dimension_r = str(self.level_dimensions[i])
-                if dimension_r != dimension_w:
-                    print('warning: read size %s does not match write size %s' % (dimension_w, dimension_r))
+    # def check_data(self):
+    #     for i in range(self.level_count):
+    #         txn = self._data[i].begin()
+    #         dimension = txn.get(key='dimension'.encode())
+    #         if dimension is not None:
+    #             dimension_w = dimension.decode()
+    #             dimension_r = str(self.level_dimensions[i])
+    #             if dimension_r != dimension_w:
+    #                 print('warning: read size %s does not match write size %s' % (dimension_w, dimension_r))
 
     def __repr__(self):
         return f'{self.__class__.__name__}({self._filename!r})'
 
     def close(self):
         """Close the OpenSlide object."""
         for dd in self._data:
@@ -137,33 +136,35 @@
     def properties(self):
         """Metadata about the image.
 
         This is a map: property name -> property value."""
         return self._osr
 
     def read_region(self, location, level, size):
+
         """Return a PIL.Image containing the contents of the region.
 
         location: (x, y) tuple giving the top left pixel in the level 0
                   reference frame.
         level:    the level number.
         size:     (width, height) tuple giving the region size.
 
         Unlike in the C interface, the image data returned by this
         function is not premultiplied."""
+        assert self._mode == 'r', 'must be in read mode!'
         x_start, y_start = location
         x_end, y_end = x_start + size[0], y_start + size[1]
         dimension = self.level_dimensions[level]
         step = self._osr['patch_size']
         x_min = math.floor(x_start / step) * step
         y_min = math.floor(y_start / step) * step
         x_max = math.ceil(x_end / step) * step
         y_max = math.ceil(y_end / step) * step
         image = np.zeros((y_max - y_min, x_max - x_min, 3), dtype=np.uint8)
-        txn = self._data[level].begin()
+        txn = self._data[level]
         for w in range(x_min, min(x_max, dimension[0]), step):
             for h in range(y_min, min(y_max, dimension[1]), step):
                 w_max = min(w + step, dimension[0])
                 h_max = min(h + step, dimension[1])
                 buff = txn.get(key=str((w, h, w_max, h_max)).encode())
                 buff = np.frombuffer(buff, dtype=np.uint8)
                 buff = cv2.imdecode(buff, cv2.IMREAD_COLOR)
@@ -173,36 +174,36 @@
 
     def save_from_numpy(self, data, ext='.jpg',
                         params=[cv2.IMWRITE_JPEG_QUALITY, 90],
                         pyramid=False, mpp=None, patch_size=256):
         assert self._mode == 'w'
         w, h, c = data.shape
         level_count = 1
-        level_dimensions = [(h, w)]
-        level_downsamples = [(1.0, 1.0)]
+        level_dimensions = [[h, w]]
+        level_downsamples = [[1.0, 1.0]]
         level_data = [data]
         if pyramid:
             level_dimension = [h, w]
             while True:
                 if 256 <= level_dimension[0] <= 512 or 256 <= level_dimension[1] <= 512:
                     break
                 else:
                     level_dimension[0] = level_dimension[0] // 2
                     level_dimension[1] = level_dimension[1] // 2
                     level_count += 1
-                    level_downsamples.append((h / level_dimension[0], w / level_dimension[1]))
-                    level_dimensions.append((level_dimension[0], level_dimension[1]))
+                    level_downsamples.append([h / level_dimension[0], w / level_dimension[1]])
+                    level_dimensions.append([level_dimension[0], level_dimension[1]])
                     level_data.append(level_data[-1][::2, ::2, :])
 
         properties = {}
         properties['level_count'] = level_count
         properties['level_dimensions'] = level_dimensions
         properties['dimension'] = level_dimensions[0]
         properties['level_downsamples'] = level_downsamples
-        properties['mpp'] = mpp
+        properties['mpp'] = float(mpp)
         properties['ext'] = ext
         properties['params'] = params
         properties['patch_size'] = patch_size
         self._osr = properties
         if os.path.exists(self._filename[:-4]):
             shutil.rmtree(self._filename[:-4])
         os.makedirs(self._filename[:-4])
```

### Comparing `fmg-0.2.0/fmg.egg-info/PKG-INFO` & `fmg-0.3.0/fmg.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-Metadata-Version: 2.1
-Name: fmg
-Version: 0.2.0
-Summary: Fast Memory Graphics for big image, use like OpenSlide
-Home-page: https://github.com/khtao/fmg
-Author: khtao
-Author-email: khtao@live.cn
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# Fast Memory Graphics for big image
-
-Fast Memory Graphics is a big image type based on lmdb and can use like OpenSlide
+Metadata-Version: 2.1
+Name: fmg
+Version: 0.3.0
+Summary: Fast Memory Graphics for big image, use like OpenSlide
+Home-page: https://github.com/khtao/fmg
+Author: khtao
+Author-email: khtao@live.cn
+License: MIT
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# Fast Memory Graphics for big image
+
+Fast Memory Graphics is a big image type based on lmdb and can use like OpenSlide
+
+
```

### Comparing `fmg-0.2.0/setup.py` & `fmg-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'fmg'
 DESCRIPTION = 'Fast Memory Graphics for big image, use like OpenSlide'
 URL = 'https://github.com/khtao/fmg'
 EMAIL = 'khtao@live.cn'
 AUTHOR = 'khtao'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.0'
+VERSION = '0.3.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'lmdb', 'opencv-python', 'numpy', 'pillow'
 ]
 
 # What packages are optional?
```

