# Comparing `tmp/matplotlib_venn_wordcloud-0.2.5.tar.gz` & `tmp/matplotlib_venn_wordcloud-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/matplotlib_venn_wordcloud-0.2.5.tar", last modified: Tue May  5 12:18:25 2020, max compression
+gzip compressed data, was "matplotlib_venn_wordcloud-0.2.6.tar", last modified: Mon Jun 19 09:42:20 2023, max compression
```

## Comparing `matplotlib_venn_wordcloud-0.2.5.tar` & `matplotlib_venn_wordcloud-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2020-05-05 12:18:25.000000 matplotlib_venn_wordcloud-0.2.5/
--rwxrwxrwx   0 paul      (1000) paul      (1000)     1366 2018-02-27 15:26:05.000000 matplotlib_venn_wordcloud-0.2.5/README.md
--rw-rw-r--   0 paul      (1000) paul      (1000)     1124 2020-05-05 11:52:09.000000 matplotlib_venn_wordcloud-0.2.5/setup.py
--rw-r--r--   0 paul      (1000) paul      (1000)      851 2020-05-05 12:18:25.000000 matplotlib_venn_wordcloud-0.2.5/PKG-INFO
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2020-05-05 12:18:25.000000 matplotlib_venn_wordcloud-0.2.5/matplotlib_venn_wordcloud/
--rwxrwxrwx   0 paul      (1000) paul      (1000)     2697 2020-05-05 11:52:31.000000 matplotlib_venn_wordcloud-0.2.5/matplotlib_venn_wordcloud/__init__.py
--rwxrwxr-x   0 paul      (1000) paul      (1000)     6372 2020-04-21 13:09:10.000000 matplotlib_venn_wordcloud-0.2.5/matplotlib_venn_wordcloud/examples.py
--rwxrwxr-x   0 paul      (1000) paul      (1000)    18972 2020-05-05 11:43:52.000000 matplotlib_venn_wordcloud-0.2.5/matplotlib_venn_wordcloud/_main.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2020-05-05 12:18:25.000000 matplotlib_venn_wordcloud-0.2.5/matplotlib_venn_wordcloud.egg-info/
--rwxrwxrwx   0 paul      (1000) paul      (1000)      383 2020-05-05 12:18:25.000000 matplotlib_venn_wordcloud-0.2.5/matplotlib_venn_wordcloud.egg-info/SOURCES.txt
--rwxrwxrwx   0 paul      (1000) paul      (1000)       26 2020-05-05 12:18:25.000000 matplotlib_venn_wordcloud-0.2.5/matplotlib_venn_wordcloud.egg-info/top_level.txt
--rwxrwxrwx   0 paul      (1000) paul      (1000)      851 2020-05-05 12:18:25.000000 matplotlib_venn_wordcloud-0.2.5/matplotlib_venn_wordcloud.egg-info/PKG-INFO
--rwxrwxrwx   0 paul      (1000) paul      (1000)       43 2020-05-05 12:18:25.000000 matplotlib_venn_wordcloud-0.2.5/matplotlib_venn_wordcloud.egg-info/requires.txt
--rwxrwxrwx   0 paul      (1000) paul      (1000)        1 2020-05-05 12:18:25.000000 matplotlib_venn_wordcloud-0.2.5/matplotlib_venn_wordcloud.egg-info/dependency_links.txt
--rwxrwxrwx   0 paul      (1000) paul      (1000)       79 2020-05-05 12:18:25.000000 matplotlib_venn_wordcloud-0.2.5/setup.cfg
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-06-19 09:42:20.800259 matplotlib_venn_wordcloud-0.2.6/
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     1058 2017-04-04 11:37:08.000000 matplotlib_venn_wordcloud-0.2.6/LICENSE
+-rw-rw-r--   0 paul      (1000) paul      (1000)      835 2023-06-19 09:42:20.800259 matplotlib_venn_wordcloud-0.2.6/PKG-INFO
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     1456 2023-06-19 09:34:15.000000 matplotlib_venn_wordcloud-0.2.6/README.md
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-06-19 09:42:20.796259 matplotlib_venn_wordcloud-0.2.6/matplotlib_venn_wordcloud/
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     2697 2023-06-19 09:34:53.000000 matplotlib_venn_wordcloud-0.2.6/matplotlib_venn_wordcloud/__init__.py
+-rwxrwxr-x   0 paul      (1000) paul      (1000)    18974 2023-06-19 08:58:02.000000 matplotlib_venn_wordcloud-0.2.6/matplotlib_venn_wordcloud/_main.py
+-rwxrwxr-x   0 paul      (1000) paul      (1000)     6372 2020-04-21 13:09:10.000000 matplotlib_venn_wordcloud-0.2.6/matplotlib_venn_wordcloud/examples.py
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-06-19 09:42:20.800259 matplotlib_venn_wordcloud-0.2.6/matplotlib_venn_wordcloud.egg-info/
+-rwxrwxrwx   0 paul      (1000) paul      (1000)      835 2023-06-19 09:42:20.000000 matplotlib_venn_wordcloud-0.2.6/matplotlib_venn_wordcloud.egg-info/PKG-INFO
+-rwxrwxrwx   0 paul      (1000) paul      (1000)      391 2023-06-19 09:42:20.000000 matplotlib_venn_wordcloud-0.2.6/matplotlib_venn_wordcloud.egg-info/SOURCES.txt
+-rwxrwxrwx   0 paul      (1000) paul      (1000)        1 2023-06-19 09:42:20.000000 matplotlib_venn_wordcloud-0.2.6/matplotlib_venn_wordcloud.egg-info/dependency_links.txt
+-rwxrwxrwx   0 paul      (1000) paul      (1000)       43 2023-06-19 09:42:20.000000 matplotlib_venn_wordcloud-0.2.6/matplotlib_venn_wordcloud.egg-info/requires.txt
+-rwxrwxrwx   0 paul      (1000) paul      (1000)       26 2023-06-19 09:42:20.000000 matplotlib_venn_wordcloud-0.2.6/matplotlib_venn_wordcloud.egg-info/top_level.txt
+-rwxrwxrwx   0 paul      (1000) paul      (1000)       79 2023-06-19 09:42:20.800259 matplotlib_venn_wordcloud-0.2.6/setup.cfg
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1124 2023-06-19 09:34:28.000000 matplotlib_venn_wordcloud-0.2.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `matplotlib_venn_wordcloud-0.2.5/README.md` & `matplotlib_venn_wordcloud-0.2.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -33,17 +33,21 @@
     sets.append(set(words))
 
 # create visualisation
 venn2_wordcloud(sets)
 ```
 You can also run [examples.py](./matplotlib_venn_wordcloud/examples.py) as main.
 
-``` 
+```
     python examples.py
 ```
 ## Installation
 
 Easiest via pip:
 
 ``` shell
 pip install matplotlib_venn_wordcloud
 ```
+
+## Recent changes
+
+- 0.2.6 Fixed bug that occurred due to numpy's deprecation of np.float
```

### Comparing `matplotlib_venn_wordcloud-0.2.5/setup.py` & `matplotlib_venn_wordcloud-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name = 'matplotlib_venn_wordcloud',
-    version = '0.2.5',
+    version = '0.2.6',
     description = 'Create a Venn diagram with word clouds corresponding to each subset.',
     author = 'Paul Brodersen',
     author_email = 'paulbrodersen+matplotlib_venn_wordcloud@gmail.com',
     url = 'https://github.com/paulbrodersen/matplotlib_venn_wordcloud',
     download_url = 'https://github.com/paulbrodersen/matplotlib_venn_wordcloud/archive/0.2.4.tar.gz',
     keywords = ['matplotlib', 'venn', 'wordcloud'],
     classifiers = [ # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
```

### Comparing `matplotlib_venn_wordcloud-0.2.5/PKG-INFO` & `matplotlib_venn_wordcloud-0.2.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: matplotlib_venn_wordcloud
-Version: 0.2.5
+Version: 0.2.6
 Summary: Create a Venn diagram with word clouds corresponding to each subset.
 Home-page: https://github.com/paulbrodersen/matplotlib_venn_wordcloud
+Download-URL: https://github.com/paulbrodersen/matplotlib_venn_wordcloud/archive/0.2.4.tar.gz
 Author: Paul Brodersen
 Author-email: paulbrodersen+matplotlib_venn_wordcloud@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/paulbrodersen/matplotlib_venn_wordcloud/archive/0.2.4.tar.gz
-Description: UNKNOWN
 Keywords: matplotlib,venn,wordcloud
 Platform: Platform Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Visualization
+License-File: LICENSE
```

### Comparing `matplotlib_venn_wordcloud-0.2.5/matplotlib_venn_wordcloud/__init__.py` & `matplotlib_venn_wordcloud-0.2.6/matplotlib_venn_wordcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,8 +66,8 @@
 # create visualisation
 venn_wordcloud.venn2_wordcloud(sets)
 
 """
 
 from matplotlib_venn_wordcloud._main import venn2_wordcloud, venn3_wordcloud
 __all__ = ['venn2_wordcloud', 'venn3_wordcloud']
-__version__ = '0.2.5'
+__version__ = '0.2.6'
```

### Comparing `matplotlib_venn_wordcloud-0.2.5/matplotlib_venn_wordcloud/examples.py` & `matplotlib_venn_wordcloud-0.2.6/matplotlib_venn_wordcloud/examples.py`

 * *Files identical despite different names*

### Comparing `matplotlib_venn_wordcloud-0.2.5/matplotlib_venn_wordcloud/_main.py` & `matplotlib_venn_wordcloud-0.2.6/matplotlib_venn_wordcloud/_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,15 +512,15 @@
         # determine pixel coordinates
         x = np.linspace(xlim[0], xlim[1], self.x_resolution)
         y = np.linspace(ylim[0], ylim[1], self.y_resolution)
         xgrid, ygrid = np.meshgrid(x, y)
         self.pixel_coordinates = np.c_[xgrid.ravel(), ygrid.ravel()]
 
         # initialise pixel array
-        self.rgba = np.zeros((self.y_resolution, self.x_resolution, 4), dtype=np.float)
+        self.rgba = np.zeros((self.y_resolution, self.x_resolution, 4), dtype=np.float64)
 
 
     def imshow(self, **imshow_kwargs):
         # create a new axis on top of existing axis
         bbox = self.ax.get_position() # in figure coordinates
         fig = self.ax.get_figure()
         subax = fig.add_axes(bbox, facecolor=None)
```

### Comparing `matplotlib_venn_wordcloud-0.2.5/matplotlib_venn_wordcloud.egg-info/PKG-INFO` & `matplotlib_venn_wordcloud-0.2.6/matplotlib_venn_wordcloud.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: matplotlib-venn-wordcloud
-Version: 0.2.5
+Version: 0.2.6
 Summary: Create a Venn diagram with word clouds corresponding to each subset.
 Home-page: https://github.com/paulbrodersen/matplotlib_venn_wordcloud
+Download-URL: https://github.com/paulbrodersen/matplotlib_venn_wordcloud/archive/0.2.4.tar.gz
 Author: Paul Brodersen
 Author-email: paulbrodersen+matplotlib_venn_wordcloud@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/paulbrodersen/matplotlib_venn_wordcloud/archive/0.2.4.tar.gz
-Description: UNKNOWN
 Keywords: matplotlib,venn,wordcloud
 Platform: Platform Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Visualization
+License-File: LICENSE
```

