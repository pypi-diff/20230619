# Comparing `tmp/shapedtw-1.0.1-py3-none-any.whl.zip` & `tmp/shapedtw-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 55843 bytes, number of entries: 12
--rw-rw-r--  2.0 unx      387 b- defN 23-Jun-19 09:57 shapedtw/__init__.py
--rw-rw-r--  2.0 unx    35037 b- defN 23-Jun-19 10:02 shapedtw/dtwPlot.py
--rw-rw-r--  2.0 unx    15488 b- defN 23-Jun-18 12:39 shapedtw/exceptions.py
--rw-rw-r--  2.0 unx    41850 b- defN 23-Jun-18 12:39 shapedtw/preprocessing.py
--rw-rw-r--  2.0 unx    19140 b- defN 23-Jun-18 12:39 shapedtw/shapeDescriptors.py
--rw-rw-r--  2.0 unx    60419 b- defN 23-Jun-19 10:03 shapedtw/shapedtw.py
--rw-rw-r--  2.0 unx     5752 b- defN 23-Jun-19 10:03 shapedtw/utils.py
--rw-rw-r--  2.0 unx    35149 b- defN 23-Jun-19 10:11 shapedtw-1.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx    24654 b- defN 23-Jun-19 10:11 shapedtw-1.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-19 10:11 shapedtw-1.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-19 10:11 shapedtw-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      946 b- defN 23-Jun-19 10:11 shapedtw-1.0.1.dist-info/RECORD
-12 files, 238923 bytes uncompressed, 54279 bytes compressed:  77.3%
+Zip file size: 55895 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      401 b- defN 23-Jun-19 18:49 shapedtw/__init__.py
+-rw-r--r--  2.0 unx    35037 b- defN 23-Jun-19 18:49 shapedtw/dtwPlot.py
+-rw-r--r--  2.0 unx    15488 b- defN 23-Jun-19 18:49 shapedtw/exceptions.py
+-rw-r--r--  2.0 unx    41850 b- defN 23-Jun-19 18:49 shapedtw/preprocessing.py
+-rw-r--r--  2.0 unx    19140 b- defN 23-Jun-19 18:49 shapedtw/shapeDescriptors.py
+-rw-r--r--  2.0 unx    60419 b- defN 23-Jun-19 18:49 shapedtw/shapedtw.py
+-rw-r--r--  2.0 unx     5752 b- defN 23-Jun-19 18:49 shapedtw/utils.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-19 18:49 shapedtw-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    26015 b- defN 23-Jun-19 18:49 shapedtw-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 18:49 shapedtw-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-19 18:49 shapedtw-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      946 b- defN 23-Jun-19 18:49 shapedtw-1.0.3.dist-info/RECORD
+12 files, 240298 bytes uncompressed, 54331 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: shapedtw/shapedtw.py
 Comment: 
 
 Filename: shapedtw/utils.py
 Comment: 
 
-Filename: shapedtw-1.0.1.dist-info/LICENSE
+Filename: shapedtw-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: shapedtw-1.0.1.dist-info/METADATA
+Filename: shapedtw-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: shapedtw-1.0.1.dist-info/WHEEL
+Filename: shapedtw-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: shapedtw-1.0.1.dist-info/top_level.txt
+Filename: shapedtw-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: shapedtw-1.0.1.dist-info/RECORD
+Filename: shapedtw-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shapedtw/__init__.py

```diff
@@ -1,12 +1,12 @@
 """
-Extension of the dtw-python package, implementing shape dtw variant of the algorithm.
+An extension to the dtw-python package, implementing a variant of the algorithm called 'shape dtw'.
 """
 
 __author__ = """Mikołaj Szafraniec"""
 __email__ = 'mikolaj.szafraniec.upds@gmail.com'
-__version__ = '1.0.1'
+__version__ = '1.0.3'
 
 # Imports which will be make after call 'from shapedtw import *'
 from shapedtw.shapedtw import shape_dtw
 from shapedtw.shapeDescriptors import *
 from shapedtw.dtwPlot import dtwPlot
```

## Comparing `shapedtw-1.0.1.dist-info/LICENSE` & `shapedtw-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `shapedtw-1.0.1.dist-info/METADATA` & `shapedtw-1.0.3.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: shapedtw
-Version: 1.0.1
-Summary: Extension of the dtw-python package, implementing shape dtw variant of the algorithm.
+Version: 1.0.3
+Summary: An extension to the dtw-python package, implementing a variant of the dtw algorithm called 'shape dtw'.
 Home-page: https://mikolajszafraniecupds.github.io/shapedtw-python/
 Author: Mikołaj Szafraniec
 Author-email: mikolaj.szafraniec.upds@gmail.com
 License: GNU General Public License v3
 Keywords: dtw,shapedtw,timeseries
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -126,15 +126,15 @@
         ts_x[:85]
     )
 ) + (randn(100)*distortion_factor)
 
 df = pd.DataFrame({"ts_x": ts_x, "ts_y": ts_y})
 df.plot()
 ```
-![Time series plot](docs/assets/img/readme_fig_1.png)
+![Time series plot](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_1.png)
 
 As a final step we will define shape descriptor and run the algorithm to obtain alignment path.
 We will use compound descriptor, consisting of slope descriptor (y-shift invariant) and PAA descriptor.
 
 ```python
 slope_descriptor = SlopeDescriptor(slope_window=5)
 paa_descriptor = PAADescriptor(piecewise_aggregation_window=5)
@@ -144,15 +144,15 @@
     y=ts_y,
     subsequence_width=20,
     shape_descriptor=compound_descriptor
 )
 
 dtwPlot(shape_dtw_results, plot_type="twoway", yoffset = 30)
 ```
-![Warping path produced by the shape dtw](docs/assets/img/readme_fig_2.png)
+![Warping path produced by the shape dtw](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_2.png)
 
 As we can see, despite the shift and distortion of the reference series, the shape dtw algorithm has reproduced
 the true alignment path almost completely correctly.
 
 Finally, we can retrieve a distances from *shape_dtw_results* object in the following way:
 
 ```python
@@ -355,20 +355,20 @@
 ```
 
 Differences between warping paths can be clearly seen at the *twoway* plots:
 
 ```python
 dtwPlot(shape_dtw_dependent_results, plot_type="twoway", xoffset=20)
 ```
-![Warping paths for multivariate, dependent variant](docs/assets/img/readme_fig_3.png)
+![Warping paths for multivariate, dependent variant](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_3.png)
 
 ```python
 dtwPlot(shape_dtw_independent_results, plot_type="twoway", xoffset=20)
 ```
-![Warping paths for multivariate, dependent variant](docs/assets/img/readme_fig_4.png)
+![Warping paths for multivariate, dependent variant](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_4.png)
 
 # DTW parameters
 For *shape dtw* we can use exactly the same additional parameters as for the *dtw* package. Below you can see
 see an example of specifying a sakoechiba window with a window size of 10:
 
 ```python
 import numpy as np
@@ -391,15 +391,15 @@
     window_type="sakoechiba",
     window_args={"window_size": 10},
     keep_internals=True
 )
 
 dtwPlot(shape_dtw_res, plot_type="density")
 ```
-![Warping paths for multivariate, dependent variant](docs/assets/img/readme_fig_5.png)
+![Warping paths for multivariate, dependent variant](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_5.png)
 
 # Plots
 We reused ploting mechanism from the *dtw* package in its core, however it was extended in order to
 allowing to plot multivariate shape dtw results as well. 
 
 In case of multivariate, dependent shape dtw the structure of both *alignment* and *density* plots 
 look the same as in univariate version. The reason is that there is a single warping path,
@@ -437,36 +437,36 @@
 ```
 
 Alignment plot shows the alignment path between time series indices:
 
 ```python
 dtwPlot(shape_dtw_res, plot_type="alignment")
 ```
-![Warping paths for multivariate, dependent variant](docs/assets/img/readme_fig_6.png)
+![Warping paths for multivariate, dependent variant](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_6.png)
 
 *twoway* plot displays time series values along with the alignment path:
 
 ```python
 dtwPlot(shape_dtw_res, plot_type="twoway", xoffset=20)
 ```
-![Warping paths for multivariate, dependent variant](docs/assets/img/readme_fig_7.png)
+![Warping paths for multivariate, dependent variant](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_7.png)
 
 *threeway* plot displays query and reference time serience values against their warping curve:
 
 ```python
 dtwPlot(shape_dtw_res, plot_type="threeway")
 ```
-![Warping paths for multivariate, dependent variant](docs/assets/img/readme_fig_8.png)
+![Warping paths for multivariate, dependent variant](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_8.png)
 
 *density* plot displays distance matrix in visual form together with warping curve:
 
 ```python
 dtwPlot(shape_dtw_res, plot_type="density")
 ```
-![Warping paths for multivariate, dependent variant](docs/assets/img/readme_fig_9.png)
+![Warping paths for multivariate, dependent variant](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_9.png)
 
 ### Plots - multivariate dependent variant
 
 Let's define random, multidimensional time series:
 
 ```python
 import numpy as np
@@ -493,37 +493,37 @@
 
 *alignment* plot looks exaclty the same as in case of univariate time series, since we've got one common
 warping path for all the dimensions:
 
 ```python
 dtwPlot(shape_dtw_res, plot_type="alignment")
 ```
-![Warping paths for multivariate, dependent variant](docs/assets/img/readme_fig_10.png)
+![Warping paths for multivariate, dependent variant](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_10.png)
 
 *twoway* plot shows all of time series dimensions and warping path:
 
 ```python
 dtwPlot(shape_dtw_res, plot_type="twoway", xoffset=20)
 ```
-![Warping paths for multivariate, dependent variant](docs/assets/img/readme_fig_11.png)
+![Warping paths for multivariate, dependent variant](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_11.png)
 
 *threeway* plot displays both dimensions of query and reference series against warping curve:
 
 ```python
 dtwPlot(shape_dtw_res, plot_type="threeway")
 ```
-![Warping paths for multivariate, dependent variant](docs/assets/img/readme_fig_12.png)
+![Warping paths for multivariate, dependent variant](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_12.png)
 
 *density* plot looks the same as in case of univariate time series, due to the fact that there is one
 common warping path:
 
 ```python
 dtwPlot(shape_dtw_res, plot_type="density")
 ```
-![Warping paths for multivariate, dependent variant](docs/assets/img/readme_fig_13.png)
+![Warping paths for multivariate, dependent variant](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_13.png)
 
 ### Plots - multivariate independent variant
 
 Let's define the same multidimensional time series as in previous example and calculate shape dtw
 results for them, but this time using independent multivariate version of the algorithm:
 
 ```python
@@ -550,37 +550,37 @@
 ```
 
 In this version *alignment* plot shows warping curves calculated for each dimension individually:
 
 ```python
 dtwPlot(shape_dtw_res, plot_type="alignment")
 ```
-![Warping paths for multivariate, dependent variant](docs/assets/img/readme_fig_14.png)
+![Warping paths for multivariate, dependent variant](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_14.png)
 
 Similarly as in dependent version, *twoway* plot shows values of all dimensions with
 warping paths. This time each alignment path is different:
 
 ```python
 dtwPlot(shape_dtw_res, plot_type="twoway", xoffset=20)
 ```
-![Warping paths for multivariate, dependent variant](docs/assets/img/readme_fig_15.png)
+![Warping paths for multivariate, dependent variant](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_15.png)
 
 *threeway* plot also looks similarly as in multivariate dependent case:
 
 ```python
 dtwPlot(shape_dtw_res, plot_type="threeway")
 ```
-![Warping paths for multivariate, dependent variant](docs/assets/img/readme_fig_16.png)
+![Warping paths for multivariate, dependent variant](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_16.png)
 
 *density* plot displays as many distance matrices and warping curves as many dimensions time series has:
 
 ```python
 dtwPlot(shape_dtw_res, plot_type="density")
 ```
-![Warping paths for multivariate, dependent variant](docs/assets/img/readme_fig_17.png)
+![Warping paths for multivariate, dependent variant](https://raw.githubusercontent.com/MikolajSzafraniecUPDS/shapedtw-python/master/docs/assets/img/readme_fig_17.png)
 
 # Applications
 Shape dtw algorithm can be used wherever standard dtw is used; according to experiments conducted and described
 by Zhao and Itti shape dtw outperforms standard dtw variant in almost all cases.
 
 As the author of this package, I think that the multidimensional version of shape dtw can be escpecially helpful for 
 financiers and investors using technical analysis in their work. Since the algorithm takes into account the
```

## Comparing `shapedtw-1.0.1.dist-info/RECORD` & `shapedtw-1.0.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-shapedtw/__init__.py,sha256=NUvXATOqkab301pvCyoO8fwuu9vV51M6-Y205zJo2Ng,387
+shapedtw/__init__.py,sha256=8yaQbIjhy5KL5eU4FDoGQ9g5epLqy0NZj3UbA56_gUk,401
 shapedtw/dtwPlot.py,sha256=hDs5zPjMh0c-wMOXW9upvX7KUU7fWQkZv0RGJ2AyNvI,35037
 shapedtw/exceptions.py,sha256=GRMrP9_Bo_uwQUqS0KYxBocV6SewHvzAL1eCNgMVWB0,15488
 shapedtw/preprocessing.py,sha256=_cRfA5dNmYmw9G7UeTx7E12VsC5tTPjTG7tbJJ1U9mA,41850
 shapedtw/shapeDescriptors.py,sha256=3WY1wuCSeVU8IN0yXNsyxxqwMYvNzS1FIhYWFjDCOmY,19140
 shapedtw/shapedtw.py,sha256=Dql3VxOQroxK5RkIFKOMXmg-NNpmp7IXJR2a-pMasC8,60419
 shapedtw/utils.py,sha256=nByVvdyE0jMr6djnjlBWCxoN8EnGq_GC3KJJ-19JZrE,5752
-shapedtw-1.0.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-shapedtw-1.0.1.dist-info/METADATA,sha256=-QV71sHjoHZIZHxhA_oLFaRiQebYq0T--P2Ra0JfqKQ,24654
-shapedtw-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-shapedtw-1.0.1.dist-info/top_level.txt,sha256=K1XU2NznMZntvyFX5WHHl0C5QzeBGgeXItowsvh3qsg,9
-shapedtw-1.0.1.dist-info/RECORD,,
+shapedtw-1.0.3.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+shapedtw-1.0.3.dist-info/METADATA,sha256=ndjRtE6hSfzbjCWz887I9CjiQQHDpNqEKWnbkE770dI,26015
+shapedtw-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+shapedtw-1.0.3.dist-info/top_level.txt,sha256=K1XU2NznMZntvyFX5WHHl0C5QzeBGgeXItowsvh3qsg,9
+shapedtw-1.0.3.dist-info/RECORD,,
```

