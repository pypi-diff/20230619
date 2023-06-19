# Comparing `tmp/boundaryscheme-2.3.tar.gz` & `tmp/boundaryscheme-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/boundaryscheme-2.3.tar", last modified: Mon Jun 19 09:01:47 2023, max compression
+gzip compressed data, was "dist/boundaryscheme-2.4.tar", last modified: Mon Jun 19 09:40:49 2023, max compression
```

## Comparing `boundaryscheme-2.3.tar` & `boundaryscheme-2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-19 09:01:47.000000 boundaryscheme-2.3/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     4427 2023-06-19 09:01:47.000000 boundaryscheme-2.3/PKG-INFO
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-19 09:01:47.000000 boundaryscheme-2.3/tests/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 07:50:58.000000 boundaryscheme-2.3/tests/__init__.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       62 2023-06-14 13:22:07.000000 boundaryscheme-2.3/tests/test_import.py
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-19 09:01:47.000000 boundaryscheme-2.3/boundaryscheme.egg-info/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     4427 2023-06-19 09:01:47.000000 boundaryscheme-2.3/boundaryscheme.egg-info/PKG-INFO
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      522 2023-06-19 09:01:47.000000 boundaryscheme-2.3/boundaryscheme.egg-info/SOURCES.txt
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       29 2023-06-19 09:01:47.000000 boundaryscheme-2.3/boundaryscheme.egg-info/requires.txt
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       30 2023-06-19 09:01:47.000000 boundaryscheme-2.3/boundaryscheme.egg-info/top_level.txt
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        1 2023-06-19 09:01:47.000000 boundaryscheme-2.3/boundaryscheme.egg-info/dependency_links.txt
--rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     3327 2023-06-16 13:13:26.000000 boundaryscheme-2.3/README.md
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      940 2023-06-14 14:38:10.000000 boundaryscheme-2.3/setup.py
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-19 09:01:47.000000 boundaryscheme-2.3/examples/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-05-16 09:26:00.000000 boundaryscheme-2.3/examples/__init__.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1980 2023-06-19 08:52:55.000000 boundaryscheme-2.3/examples/draw_detKLcurve.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1385 2023-06-14 13:22:07.000000 boundaryscheme-2.3/examples/draw_nbrzerosdetKL.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      909 2023-06-14 13:22:07.000000 boundaryscheme-2.3/examples/draw_symbol.py
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-19 09:01:47.000000 boundaryscheme-2.3/boundaryscheme/
--rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     6390 2023-06-04 15:21:00.000000 boundaryscheme-2.3/boundaryscheme/boundaries.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      137 2023-06-19 09:01:27.000000 boundaryscheme-2.3/boundaryscheme/__init__.py
--rwxrwxrwx   0 pierrelebarbenchon   (501) staff       (20)    10942 2023-06-05 07:45:15.000000 boundaryscheme-2.3/boundaryscheme/utils.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)    19750 2023-06-14 13:22:07.000000 boundaryscheme-2.3/boundaryscheme/schemes.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     2605 2023-01-16 09:04:43.000000 boundaryscheme-2.3/boundaryscheme/complex_winding_number.py
--rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)    22478 2023-06-19 08:37:41.000000 boundaryscheme-2.3/boundaryscheme/pyplot.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       38 2023-06-19 09:01:47.000000 boundaryscheme-2.3/setup.cfg
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-19 09:40:49.000000 boundaryscheme-2.4/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     4427 2023-06-19 09:40:49.000000 boundaryscheme-2.4/PKG-INFO
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-19 09:40:49.000000 boundaryscheme-2.4/tests/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 07:50:58.000000 boundaryscheme-2.4/tests/__init__.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       62 2023-06-14 13:22:07.000000 boundaryscheme-2.4/tests/test_import.py
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-19 09:40:49.000000 boundaryscheme-2.4/boundaryscheme.egg-info/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     4427 2023-06-19 09:40:49.000000 boundaryscheme-2.4/boundaryscheme.egg-info/PKG-INFO
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      522 2023-06-19 09:40:49.000000 boundaryscheme-2.4/boundaryscheme.egg-info/SOURCES.txt
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       29 2023-06-19 09:40:49.000000 boundaryscheme-2.4/boundaryscheme.egg-info/requires.txt
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       30 2023-06-19 09:40:49.000000 boundaryscheme-2.4/boundaryscheme.egg-info/top_level.txt
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        1 2023-06-19 09:40:49.000000 boundaryscheme-2.4/boundaryscheme.egg-info/dependency_links.txt
+-rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     3327 2023-06-16 13:13:26.000000 boundaryscheme-2.4/README.md
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      940 2023-06-14 14:38:10.000000 boundaryscheme-2.4/setup.py
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-19 09:40:49.000000 boundaryscheme-2.4/examples/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-05-16 09:26:00.000000 boundaryscheme-2.4/examples/__init__.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     2054 2023-06-19 09:39:27.000000 boundaryscheme-2.4/examples/draw_detKLcurve.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1385 2023-06-14 13:22:07.000000 boundaryscheme-2.4/examples/draw_nbrzerosdetKL.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      909 2023-06-14 13:22:07.000000 boundaryscheme-2.4/examples/draw_symbol.py
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-19 09:40:49.000000 boundaryscheme-2.4/boundaryscheme/
+-rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     6390 2023-06-04 15:21:00.000000 boundaryscheme-2.4/boundaryscheme/boundaries.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      137 2023-06-19 09:40:12.000000 boundaryscheme-2.4/boundaryscheme/__init__.py
+-rwxrwxrwx   0 pierrelebarbenchon   (501) staff       (20)    10942 2023-06-05 07:45:15.000000 boundaryscheme-2.4/boundaryscheme/utils.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)    19750 2023-06-14 13:22:07.000000 boundaryscheme-2.4/boundaryscheme/schemes.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     2605 2023-01-16 09:04:43.000000 boundaryscheme-2.4/boundaryscheme/complex_winding_number.py
+-rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)    22484 2023-06-19 09:38:39.000000 boundaryscheme-2.4/boundaryscheme/pyplot.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       38 2023-06-19 09:40:49.000000 boundaryscheme-2.4/setup.cfg
```

### Comparing `boundaryscheme-2.3/PKG-INFO` & `boundaryscheme-2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boundaryscheme
-Version: 2.3
+Version: 2.4
 Summary: This library implements Kreiss-Lopatinskii determinant for numerical scheme with boundary
 Home-page: UNKNOWN
 Author: Pierre Le Barbenchon
 License: UNKNOWN
 Description: This is the architecture for the package "boundaryscheme" : https://pypi.org/project/boundaryscheme/
```

### Comparing `boundaryscheme-2.3/boundaryscheme.egg-info/PKG-INFO` & `boundaryscheme-2.4/boundaryscheme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boundaryscheme
-Version: 2.3
+Version: 2.4
 Summary: This library implements Kreiss-Lopatinskii determinant for numerical scheme with boundary
 Home-page: UNKNOWN
 Author: Pierre Le Barbenchon
 License: UNKNOWN
 Description: This is the architecture for the package "boundaryscheme" : https://pypi.org/project/boundaryscheme/
```

### Comparing `boundaryscheme-2.3/boundaryscheme.egg-info/SOURCES.txt` & `boundaryscheme-2.4/boundaryscheme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.3/README.md` & `boundaryscheme-2.4/README.md`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.3/setup.py` & `boundaryscheme-2.4/setup.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.3/examples/draw_detKLcurve.py` & `boundaryscheme-2.4/examples/draw_detKLcurve.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 
 if __name__ == "__main__":
     """plot the Kreiss-Lopatinskii determinant curve for BeamWarming and for lambda = 1.4"""
     # bsplt.detKLplot(BeamWarming, SILW(2,3), lamb = 1.4)
 
     """plot the Kreiss-Lopatinskii determinant curve for BeamWarming and for lambda in [1.4, 0.7, 1] with sigma = 0.4"""
-    bsplt.detKLplot(BeamWarming, SILW(2, 3), lamb=np.array([1.4, 0.7, 1]), sigma=0)
-
+    # bsplt.detKLplot(BeamWarming, SILW(2, 3), lamb=np.array([1.4, 0.7, 1]), sigma=0)
+    bsplt.nbrzerosdetKL(BeamWarming,[SILW(1,3),SILW(2,3)], nlambda = 50)
 
     """plot the Kreiss-Lopatinskii determinant curve for BeamWarming and for lambda = 1 with sigma in [-0.2, 0, 0.1,0.4]"""
     # bsplt.detKLplot(BeamWarming, SILW(2,3), lamb = 1, sigma = np.array([-0.2, 0, 0.1,0.4]))
 
     """plot the Kreiss-Lopatinskii determinant curve for BeamWarming and for lambda in [1.4, 0.7] with sigma in [-0.2, 0, 0.4]"""
     # bsplt.detKLplot(BeamWarming, SILW(2,3), lamb = [1.4, 0.7], sigma = np.array([-0.2, 0, 0.4]))
```

### Comparing `boundaryscheme-2.3/examples/draw_nbrzerosdetKL.py` & `boundaryscheme-2.4/examples/draw_nbrzerosdetKL.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.3/examples/draw_symbol.py` & `boundaryscheme-2.4/examples/draw_symbol.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.3/boundaryscheme/boundaries.py` & `boundaryscheme-2.4/boundaryscheme/boundaries.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.3/boundaryscheme/utils.py` & `boundaryscheme-2.4/boundaryscheme/utils.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.3/boundaryscheme/schemes.py` & `boundaryscheme-2.4/boundaryscheme/schemes.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.3/boundaryscheme/complex_winding_number.py` & `boundaryscheme-2.4/boundaryscheme/complex_winding_number.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.3/boundaryscheme/pyplot.py` & `boundaryscheme-2.4/boundaryscheme/pyplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,15 @@
                 WindingNumbers.append(Indice(Det))
             separator = []
             value = []
             for j in range(len(WindingNumbers) - 1):
                 if WindingNumbers[j] != WindingNumbers[j + 1]:
                     separator.append((lambdas[j] + lambdas[j + 1]) / 2)
                     value.append(S.r - WindingNumbers[j])
-            value.append(WindingNumbers[-1])
+            value.append(S.r - WindingNumbers[-1])
             if separator == []:
                 axs[i].text((lambmax + lambmin) / 2, 0.5, value[0], horizontalalignment="center", verticalalignment="center", fontsize=fontsize)
             else:
                 for j in range(len(separator) + 1):
                     if j == 0:
                         axs[i].plot([separator[j], separator[j]], [0, 1], color="black")
                         axs[i].text(separator[0] / 2, 0.5, value[j], horizontalalignment="center", verticalalignment="center", fontsize=fontsize)
```

