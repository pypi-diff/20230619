# Comparing `tmp/svgbit-0.2.8.tar.gz` & `tmp/svgbit-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgbit-0.2.8.tar", last modified: Thu Nov 24 12:03:52 2022, max compression
+gzip compressed data, was "svgbit-0.2.9.tar", last modified: Thu Nov 24 12:42:15 2022, max compression
```

## Comparing `svgbit-0.2.8.tar` & `svgbit-0.2.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 hongyz    (1001) hongyz    (1001)        0 2022-11-24 12:03:52.420859 svgbit-0.2.8/
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)    35149 2022-11-17 08:02:37.000000 svgbit-0.2.8/LICENSE
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)     8176 2022-11-24 12:03:52.420859 svgbit-0.2.8/PKG-INFO
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)     5915 2022-09-29 02:03:08.000000 svgbit-0.2.8/README.rst
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)       38 2022-11-24 12:03:52.420859 svgbit-0.2.8/setup.cfg
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)     1527 2022-11-17 08:05:53.000000 svgbit-0.2.8/setup.py
-drwxr-xr-x   0 hongyz    (1001) hongyz    (1001)        0 2022-11-24 12:03:52.420859 svgbit-0.2.8/svgbit/
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)      415 2022-11-24 06:20:19.000000 svgbit-0.2.8/svgbit/__init__.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)     3699 2022-09-29 02:03:08.000000 svgbit-0.2.8/svgbit/__main__.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)       22 2022-11-24 12:02:41.000000 svgbit-0.2.8/svgbit/_version.py
-drwxr-xr-x   0 hongyz    (1001) hongyz    (1001)        0 2022-11-24 12:03:52.420859 svgbit-0.2.8/svgbit/core/
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)    10096 2022-11-24 06:16:05.000000 svgbit-0.2.8/svgbit/core/STDataset.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)        0 2022-07-18 01:57:21.000000 svgbit-0.2.8/svgbit/core/__init__.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)     2157 2022-09-13 12:08:34.000000 svgbit-0.2.8/svgbit/core/cluster.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)     6410 2022-11-24 07:50:53.000000 svgbit-0.2.8/svgbit/core/combinations.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)     3977 2022-09-29 06:42:06.000000 svgbit-0.2.8/svgbit/core/density.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)     2674 2022-10-20 02:46:48.000000 svgbit-0.2.8/svgbit/core/filters.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)     6478 2022-11-24 10:48:58.000000 svgbit-0.2.8/svgbit/core/io.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)     6628 2022-09-29 02:03:08.000000 svgbit-0.2.8/svgbit/core/moran.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)     1501 2022-10-20 02:46:48.000000 svgbit-0.2.8/svgbit/core/normalizers.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)    10977 2022-10-27 07:22:32.000000 svgbit-0.2.8/svgbit/core/plot.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)      204 2022-07-22 02:04:42.000000 svgbit-0.2.8/svgbit/core/utils.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)      137 2022-08-08 01:21:33.000000 svgbit-0.2.8/svgbit/filters.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)       64 2022-09-13 12:08:34.000000 svgbit-0.2.8/svgbit/normalizers.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)      120 2022-09-13 12:08:34.000000 svgbit-0.2.8/svgbit/plot.py
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)     1063 2022-09-13 12:08:34.000000 svgbit-0.2.8/svgbit/run.py
-drwxr-xr-x   0 hongyz    (1001) hongyz    (1001)        0 2022-11-24 12:03:52.420859 svgbit-0.2.8/svgbit.egg-info/
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)     8176 2022-11-24 12:03:52.000000 svgbit-0.2.8/svgbit.egg-info/PKG-INFO
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)      588 2022-11-24 12:03:52.000000 svgbit-0.2.8/svgbit.egg-info/SOURCES.txt
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)        1 2022-11-24 12:03:52.000000 svgbit-0.2.8/svgbit.egg-info/dependency_links.txt
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)       49 2022-11-24 12:03:52.000000 svgbit-0.2.8/svgbit.egg-info/entry_points.txt
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)      102 2022-11-24 12:03:52.000000 svgbit-0.2.8/svgbit.egg-info/requires.txt
--rw-r--r--   0 hongyz    (1001) hongyz    (1001)        7 2022-11-24 12:03:52.000000 svgbit-0.2.8/svgbit.egg-info/top_level.txt
+drwxr-xr-x   0 hongyz    (1001) hongyz    (1001)        0 2022-11-24 12:42:15.516785 svgbit-0.2.9/
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)    35149 2022-11-17 08:02:37.000000 svgbit-0.2.9/LICENSE
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)     8176 2022-11-24 12:42:15.516785 svgbit-0.2.9/PKG-INFO
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)     5915 2022-09-29 02:03:08.000000 svgbit-0.2.9/README.rst
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)       38 2022-11-24 12:42:15.516785 svgbit-0.2.9/setup.cfg
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)     1527 2022-11-17 08:05:53.000000 svgbit-0.2.9/setup.py
+drwxr-xr-x   0 hongyz    (1001) hongyz    (1001)        0 2022-11-24 12:42:15.513452 svgbit-0.2.9/svgbit/
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)      415 2022-11-24 06:20:19.000000 svgbit-0.2.9/svgbit/__init__.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)     3699 2022-09-29 02:03:08.000000 svgbit-0.2.9/svgbit/__main__.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)       22 2022-11-24 12:41:55.000000 svgbit-0.2.9/svgbit/_version.py
+drwxr-xr-x   0 hongyz    (1001) hongyz    (1001)        0 2022-11-24 12:42:15.516785 svgbit-0.2.9/svgbit/core/
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)    10070 2022-11-24 12:40:45.000000 svgbit-0.2.9/svgbit/core/STDataset.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)        0 2022-07-18 01:57:21.000000 svgbit-0.2.9/svgbit/core/__init__.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)     2157 2022-09-13 12:08:34.000000 svgbit-0.2.9/svgbit/core/cluster.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)     6410 2022-11-24 07:50:53.000000 svgbit-0.2.9/svgbit/core/combinations.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)     3977 2022-09-29 06:42:06.000000 svgbit-0.2.9/svgbit/core/density.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)     2674 2022-10-20 02:46:48.000000 svgbit-0.2.9/svgbit/core/filters.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)     6478 2022-11-24 10:48:58.000000 svgbit-0.2.9/svgbit/core/io.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)     6628 2022-09-29 02:03:08.000000 svgbit-0.2.9/svgbit/core/moran.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)     1501 2022-10-20 02:46:48.000000 svgbit-0.2.9/svgbit/core/normalizers.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)    10977 2022-10-27 07:22:32.000000 svgbit-0.2.9/svgbit/core/plot.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)      204 2022-07-22 02:04:42.000000 svgbit-0.2.9/svgbit/core/utils.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)      137 2022-08-08 01:21:33.000000 svgbit-0.2.9/svgbit/filters.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)       64 2022-09-13 12:08:34.000000 svgbit-0.2.9/svgbit/normalizers.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)      120 2022-09-13 12:08:34.000000 svgbit-0.2.9/svgbit/plot.py
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)     1063 2022-09-13 12:08:34.000000 svgbit-0.2.9/svgbit/run.py
+drwxr-xr-x   0 hongyz    (1001) hongyz    (1001)        0 2022-11-24 12:42:15.513452 svgbit-0.2.9/svgbit.egg-info/
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)     8176 2022-11-24 12:42:15.000000 svgbit-0.2.9/svgbit.egg-info/PKG-INFO
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)      588 2022-11-24 12:42:15.000000 svgbit-0.2.9/svgbit.egg-info/SOURCES.txt
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)        1 2022-11-24 12:42:15.000000 svgbit-0.2.9/svgbit.egg-info/dependency_links.txt
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)       49 2022-11-24 12:42:15.000000 svgbit-0.2.9/svgbit.egg-info/entry_points.txt
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)      102 2022-11-24 12:42:15.000000 svgbit-0.2.9/svgbit.egg-info/requires.txt
+-rw-r--r--   0 hongyz    (1001) hongyz    (1001)        7 2022-11-24 12:42:15.000000 svgbit-0.2.9/svgbit.egg-info/top_level.txt
```

### Comparing `svgbit-0.2.8/LICENSE` & `svgbit-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `svgbit-0.2.8/PKG-INFO` & `svgbit-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: svgbit
-Version: 0.2.8
+Version: 0.2.9
 Summary: UNKNOWN
 Home-page: https://github.com/CPenglab/svgbit
 Author: CPenglab
 Author-email: chengpeng@ynu.edu.cn
 License: GPLv3
 Description: #################
         svgbit quickstart
```

### Comparing `svgbit-0.2.8/README.rst` & `svgbit-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `svgbit-0.2.8/setup.py` & `svgbit-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `svgbit-0.2.8/svgbit/__main__.py` & `svgbit-0.2.9/svgbit/__main__.py`

 * *Files identical despite different names*

### Comparing `svgbit-0.2.8/svgbit/core/STDataset.py` & `svgbit-0.2.9/svgbit/core/STDataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         results = cluster.cluster(
             self._hotspot_df,
             self._AI,
             n_svgs=n_svgs,
             n_svg_clusters=n_svg_clusters,
             threshold=threshold,
         )
-        self._svg_cluster = results[0].reindex(index=self.genes)
+        self._svg_cluster = results[0]
         self._spot_type = results[1].reindex(index=self.spots)
 
     @property
     def count_df(self) -> pd.DataFrame:
         """Expression matrix."""
         return self._count_df
```

### Comparing `svgbit-0.2.8/svgbit/core/cluster.py` & `svgbit-0.2.9/svgbit/core/cluster.py`

 * *Files identical despite different names*

### Comparing `svgbit-0.2.8/svgbit/core/combinations.py` & `svgbit-0.2.9/svgbit/core/combinations.py`

 * *Files identical despite different names*

### Comparing `svgbit-0.2.8/svgbit/core/density.py` & `svgbit-0.2.9/svgbit/core/density.py`

 * *Files identical despite different names*

### Comparing `svgbit-0.2.8/svgbit/core/filters.py` & `svgbit-0.2.9/svgbit/core/filters.py`

 * *Files identical despite different names*

### Comparing `svgbit-0.2.8/svgbit/core/io.py` & `svgbit-0.2.9/svgbit/core/io.py`

 * *Files identical despite different names*

### Comparing `svgbit-0.2.8/svgbit/core/moran.py` & `svgbit-0.2.9/svgbit/core/moran.py`

 * *Files identical despite different names*

### Comparing `svgbit-0.2.8/svgbit/core/normalizers.py` & `svgbit-0.2.9/svgbit/core/normalizers.py`

 * *Files identical despite different names*

### Comparing `svgbit-0.2.8/svgbit/core/plot.py` & `svgbit-0.2.9/svgbit/core/plot.py`

 * *Files identical despite different names*

### Comparing `svgbit-0.2.8/svgbit/run.py` & `svgbit-0.2.9/svgbit/run.py`

 * *Files identical despite different names*

### Comparing `svgbit-0.2.8/svgbit.egg-info/PKG-INFO` & `svgbit-0.2.9/svgbit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: svgbit
-Version: 0.2.8
+Version: 0.2.9
 Summary: UNKNOWN
 Home-page: https://github.com/CPenglab/svgbit
 Author: CPenglab
 Author-email: chengpeng@ynu.edu.cn
 License: GPLv3
 Description: #################
         svgbit quickstart
```

### Comparing `svgbit-0.2.8/svgbit.egg-info/SOURCES.txt` & `svgbit-0.2.9/svgbit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

