# Comparing `tmp/s2stools-0.1.0.tar.gz` & `tmp/s2stools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2stools-0.1.0.tar", last modified: Mon Aug 22 11:29:54 2022, max compression
+gzip compressed data, was "s2stools-0.2.0.tar", last modified: Mon Jun 19 14:47:27 2023, max compression
```

## Comparing `s2stools-0.1.0.tar` & `s2stools-0.2.0.tar`

### file list

```diff
@@ -1,63 +1,18 @@
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2022-08-22 11:29:54.000000 s2stools-0.1.0/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)        0 2021-12-03 09:27:43.000000 s2stools-0.1.0/LICENSE.txt
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)        0 2022-08-22 09:46:36.000000 s2stools-0.1.0/MANIFEST.in
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      554 2022-08-22 11:29:54.000000 s2stools-0.1.0/PKG-INFO
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2148 2022-08-22 11:04:43.000000 s2stools-0.1.0/README.md
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2022-08-22 11:29:54.000000 s2stools-0.1.0/s2stools/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       68 2022-08-22 09:23:32.000000 s2stools-0.1.0/s2stools/__init__.py
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2022-08-22 11:29:54.000000 s2stools-0.1.0/s2stools/clim/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       30 2021-12-03 09:27:43.000000 s2stools-0.1.0/s2stools/clim/__init__.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     6392 2022-08-22 09:23:32.000000 s2stools-0.1.0/s2stools/clim/_deseasonalize.py
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2022-08-22 11:29:54.000000 s2stools-0.1.0/s2stools/download/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      825 2021-12-20 10:29:27.000000 s2stools-0.1.0/s2stools/download/S2SDownloader.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       61 2022-04-13 10:18:03.000000 s2stools-0.1.0/s2stools/download/__init__.py
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2022-08-22 11:29:54.000000 s2stools-0.1.0/s2stools/download/ecmwf/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     6259 2022-07-20 10:23:17.000000 s2stools-0.1.0/s2stools/download/ecmwf/S2SDownloaderECMWF.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       33 2021-12-03 09:27:44.000000 s2stools-0.1.0/s2stools/download/ecmwf/__init__.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2430 2021-12-03 09:27:44.000000 s2stools-0.1.0/s2stools/download/ecmwf/model_setup.py
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2022-08-22 11:29:54.000000 s2stools-0.1.0/s2stools/events/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    23381 2022-08-22 09:23:32.000000 s2stools-0.1.0/s2stools/events/EventComposite.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      302 2022-04-13 10:18:03.000000 s2stools-0.1.0/s2stools/events/__init__.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     8822 2021-12-20 10:29:27.000000 s2stools-0.1.0/s2stools/events/_extreme_prob.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     6979 2022-08-22 09:23:32.000000 s2stools-0.1.0/s2stools/events/_find_events.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2185 2022-02-22 15:49:33.000000 s2stools-0.1.0/s2stools/events/_infer_metadata.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1171 2021-12-20 10:29:27.000000 s2stools-0.1.0/s2stools/events/_infer_statistics.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1317 2022-08-17 15:00:33.000000 s2stools-0.1.0/s2stools/events/_leadtime_lagtime_conversion.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2538 2022-07-29 13:16:47.000000 s2stools-0.1.0/s2stools/events/_manage.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3371 2022-04-13 10:18:03.000000 s2stools-0.1.0/s2stools/events/_process_events.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      736 2022-04-13 10:18:03.000000 s2stools-0.1.0/s2stools/events/_ssw_compendium.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3313 2022-04-13 10:18:03.000000 s2stools-0.1.0/s2stools/events/_utils.py
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2022-08-22 11:29:54.000000 s2stools-0.1.0/s2stools/plot/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      117 2022-08-22 09:23:32.000000 s2stools-0.1.0/s2stools/plot/__init__.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      821 2022-02-22 15:49:34.000000 s2stools-0.1.0/s2stools/plot/_composite.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1237 2022-08-22 09:24:43.000000 s2stools-0.1.0/s2stools/plot/_format.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      305 2022-08-22 09:23:32.000000 s2stools-0.1.0/s2stools/plot/_utils.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2166 2022-08-22 09:27:59.000000 s2stools-0.1.0/s2stools/plot/_xarray.py
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2022-08-22 11:29:54.000000 s2stools-0.1.0/s2stools/process/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      174 2022-08-22 09:46:36.000000 s2stools-0.1.0/s2stools/process/__init__.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      604 2022-05-11 07:33:37.000000 s2stools-0.1.0/s2stools/process/_computing.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     8468 2022-08-22 09:23:32.000000 s2stools-0.1.0/s2stools/process/_open.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1340 2022-08-22 09:23:32.000000 s2stools-0.1.0/s2stools/process/_process_utils.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1678 2022-08-22 09:25:58.000000 s2stools-0.1.0/s2stools/process/_save.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     5060 2022-08-22 09:27:40.000000 s2stools-0.1.0/s2stools/process/_spectral.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3372 2022-08-17 14:40:13.000000 s2stools-0.1.0/s2stools/process/_transform_timedelta64_dimensions.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1799 2022-08-22 09:27:58.000000 s2stools-0.1.0/s2stools/process/_utils.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1272 2022-08-22 09:23:32.000000 s2stools-0.1.0/s2stools/process/_validtime.py
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2022-08-22 11:29:54.000000 s2stools-0.1.0/s2stools/tests/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)        0 2021-12-03 09:27:44.000000 s2stools-0.1.0/s2stools/tests/__init__.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      688 2021-12-03 09:27:44.000000 s2stools-0.1.0/s2stools/tests/test_clim.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3337 2022-04-13 10:18:03.000000 s2stools-0.1.0/s2stools/tests/test_download.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3350 2022-07-20 10:23:18.000000 s2stools-0.1.0/s2stools/tests/test_events.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      191 2022-07-20 10:23:18.000000 s2stools-0.1.0/s2stools/tests/test_plot.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3235 2022-07-28 07:32:17.000000 s2stools-0.1.0/s2stools/tests/test_process.py
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2022-08-22 11:29:54.000000 s2stools-0.1.0/s2stools/utils/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       22 2021-12-03 09:27:44.000000 s2stools-0.1.0/s2stools/utils/__init__.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2459 2022-02-22 15:51:51.000000 s2stools-0.1.0/s2stools/utils/_utils.py
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2022-08-22 11:29:54.000000 s2stools-0.1.0/s2stools.egg-info/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      554 2022-08-22 11:29:52.000000 s2stools-0.1.0/s2stools.egg-info/PKG-INFO
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1481 2022-08-22 11:29:53.000000 s2stools-0.1.0/s2stools.egg-info/SOURCES.txt
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)        1 2022-08-22 11:29:52.000000 s2stools-0.1.0/s2stools.egg-info/dependency_links.txt
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       30 2022-08-22 11:29:52.000000 s2stools-0.1.0/s2stools.egg-info/requires.txt
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)        9 2022-08-22 11:29:52.000000 s2stools-0.1.0/s2stools.egg-info/top_level.txt
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       38 2022-08-22 11:29:54.000000 s2stools-0.1.0/setup.cfg
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1213 2022-08-22 11:27:04.000000 s2stools-0.1.0/setup.py
+drwxr-xr-x   0 Jonas.Spaeth   (503) staff       (20)        0 2023-06-19 14:47:27.405931 s2stools-0.2.0/
+-rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)     1053 2023-04-20 15:07:18.000000 s2stools-0.2.0/LICENSE
+-rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)      265 2023-06-19 14:47:27.405319 s2stools-0.2.0/PKG-INFO
+-rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)     2372 2023-04-20 15:07:18.000000 s2stools-0.2.0/README.md
+drwxr-xr-x   0 Jonas.Spaeth   (503) staff       (20)        0 2023-06-19 14:47:27.401924 s2stools-0.2.0/s2stools/
+-rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)      107 2023-05-04 12:00:27.000000 s2stools-0.2.0/s2stools/__init__.py
+-rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)     5911 2023-05-04 12:12:47.000000 s2stools-0.2.0/s2stools/clim.py
+-rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)     1974 2023-05-04 12:07:19.000000 s2stools-0.2.0/s2stools/events.py
+-rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)     3145 2023-05-04 12:12:47.000000 s2stools-0.2.0/s2stools/plot.py
+-rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)     4182 2023-05-04 12:12:47.000000 s2stools-0.2.0/s2stools/process.py
+drwxr-xr-x   0 Jonas.Spaeth   (503) staff       (20)        0 2023-06-19 14:47:27.404723 s2stools-0.2.0/s2stools.egg-info/
+-rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)      265 2023-06-19 14:47:27.000000 s2stools-0.2.0/s2stools.egg-info/PKG-INFO
+-rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)      279 2023-06-19 14:47:27.000000 s2stools-0.2.0/s2stools.egg-info/SOURCES.txt
+-rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)        1 2023-06-19 14:47:27.000000 s2stools-0.2.0/s2stools.egg-info/dependency_links.txt
+-rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)       36 2023-06-19 14:47:27.000000 s2stools-0.2.0/s2stools.egg-info/requires.txt
+-rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)        9 2023-06-19 14:47:27.000000 s2stools-0.2.0/s2stools.egg-info/top_level.txt
+-rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)       38 2023-06-19 14:47:27.406157 s2stools-0.2.0/setup.cfg
+-rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)      926 2023-06-19 10:34:06.000000 s2stools-0.2.0/setup.py
```

### Comparing `s2stools-0.1.0/s2stools/clim/_deseasonalize.py` & `s2stools-0.2.0/s2stools/clim.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,183 +1,178 @@
 import numpy as np
 import xarray as xr
+import xarray.core.groupby
+from tqdm.autonotebook import tqdm
 
 
-def deseasonalize(
+def climatology(
         data,
         window_size=15,
-        standardize=False,
+        mean_or_std="mean",
         ndays_clim_filter=7,
-        hide_print=True,
-        hide_plot=True,
         hide_warnings=False,
-        return_clim_lists=False,
+        groupby="validtime",
 ):
     """
     Compute anomalies from the climatological mean. Deseasonalization is based on hindcasts.
 
     Parameters
     ----------
     data : xr.Dataset or xr.DataArray
         The raw data.
     window_size : int
         The mean is constructed using all reftimes within this plus-minus-day-interval.
-    standardize : boolean
-        If True, compute standardized anomalies.
+    mean_or_std : str
+        either 'mean' or 'std'
     ndays_clim_filter : int
         Apply running mean to the climatology.
-    hide_print : boolean
-        If False, print how many reftimes are used for each climatology. Defaults to True.
-    hide_plot : boolean
-        If False, plot the climatology.
     hide_warnings : boolean
         ???
-    return_clim_lists : boolean
-        If True, also return the constructed climatologies. If False, only return anomalies.
+    groupby : str
+        must be 'leadtime' or 'validtime'
 
     Returns
     -------
     xr.Dataset or xr.DataArray
-        Anomalies If return_clim_lists=True, return tuple anom, clim_list, climstd_list.
+        xr.DataArray | xr.Dataset
 
     Warnings
     --------
     If reftimes +- time window are not available then anomalies are still computed, but climatology is less robust.
 
     Notes
     -----
     There my be use cases where only one reftime and no running mean should be used, e.g., for computing anomalies of
     forecast variance.
 
     """
-    data_by_reftime_list = []
+    if mean_or_std == "mean":
+        aggregation_func = xarray.core.groupby.DataArrayGroupByAggregations.mean
+        aggregation_dim = "stacked_reftime_leadtime"
+    elif mean_or_std == "std":
+        aggregation_func = xarray.core.groupby.DataArrayGroupByAggregations.std
+        aggregation_dim = ["stacked_reftime_leadtime", "hc_year"]
+    else:
+        raise ValueError(f"mean_or_std must be 'mean' or 'std', not '{mean_or_std}'")
+
     clim_list = []
-    climstd_list = []
 
-    for reftime in data.reftime:
+    for reftime in tqdm(data.reftime, desc="iterating reftimes"):
+
+        # collect all reftimes within time window
         reftime = reftime.values.astype("datetime64[D]")
+
         window = np.arange(reftime - window_size, reftime + window_size)
-        hc_reftimes_in_window = (
-            data.sel(reftime=np.in1d(data.reftime.values, window))
-                .sel(hc_year=-1)
-                .dropna("reftime", how="all")
-                .reftime.values
-        )
 
-        # ***** COMPUTE CLIMATOLOGY *****
-        clim_stacked = (
-            data.sel(reftime=hc_reftimes_in_window, hc_year=(data.hc_year != 0))
-                .mean(["hc_year", "number"])
-                .stack(date=("reftime", "leadtime"))
+        hc_reftimes_in_window = (
+            data.sel(reftime=data.reftime.isin(window))
+            .drop_sel(hc_year=0)
+            .isel(hc_year=0)
+            .reftime
         )
 
-        clim = (
-            clim_stacked.assign_coords(
-                days_since_reftime_init=(
-                    "date",
-                    (
-                            clim_stacked.reftime.values - reftime + clim_stacked.leadtime.values
-                    ).astype("timedelta64[D]")
-                    ,
+        # stacked forecasts from hindcast years
+        clim_stacked = data.sel(
+            reftime=hc_reftimes_in_window, hc_year=(data.hc_year != 0)
+        ).stack(date=("reftime", "leadtime"))
+        if mean_or_std == "mean":
+            clim_stacked = clim_stacked.mean(["hc_year", "number"])
+        elif mean_or_std == "std":
+            clim_stacked = clim_stacked.sel(number=0)
+
+        # compute climatology
+        if groupby == "validtime":
+            clim = (
+                (
+                    clim_stacked.assign_coords(
+                        days_since_reftime_init=(
+                            "date",
+                            (
+                                    clim_stacked.reftime.values
+                                    - reftime
+                                    + clim_stacked.leadtime.values
+                            ).astype("timedelta64[D]"),
+                        )
+                    )  # days_since_reftime_init measures timedelta relative to initialization
+                    .unstack()
+                    .groupby("days_since_reftime_init")
+                    .apply(
+                        aggregation_func, dim=aggregation_dim
+                    )  # average or standardize all days that have validtime, e.g., reftime + 2D
+                    .rolling(
+                        days_since_reftime_init=ndays_clim_filter,
+                        center=True,
+                        min_periods=1,
+                    )
+                    .mean()  # rolling mean
+                    .sel(
+                        days_since_reftime_init=slice(
+                            np.timedelta64(0, "D"), data.leadtime[-1]
+                        )
+                    )  # cut climatology to length of forecast
+                    .rename(days_since_reftime_init="leadtime")
                 )
+                .assign_coords(reftime=reftime)
+                .expand_dims("reftime")
             )
-                .unstack()
-                .groupby("days_since_reftime_init")
-                .mean()
-                .rolling(
-                days_since_reftime_init=ndays_clim_filter, center=True, min_periods=1
+
+        ### remove
+        # compute climatology 2
+        if groupby == "leadtime":
+            if mean_or_std == "mean":
+                aggregation_dim = "reftime"
+            elif mean_or_std == "std":
+                aggregation_dim = ["reftime", "hc_year"]
+
+            clim = (
+                (
+                    clim_stacked.unstack()
+                    .groupby("leadtime")
+                    .apply(
+                        aggregation_func, dim=aggregation_dim
+                    )  # average or standardize all days that have validtime, e.g., reftime + 2D
+                    .rolling(
+                        leadtime=ndays_clim_filter,
+                        center=True,
+                        min_periods=1,
+                    )
+                    .mean()  # rolling mean
+                    .sel(
+                        leadtime=slice(np.timedelta64(0, "D"), data.leadtime[-1])
+                    )  # cut climatology to length of forecast
+                )
+                .assign_coords(reftime=reftime)
+                .expand_dims("reftime")
             )
-                .mean()
-                .sel(days_since_reftime_init=slice(np.timedelta64(0, "D"), data.leadtime[-1]))
-                .rename(days_since_reftime_init="leadtime")
-        )
+        ###
+
         if len(clim.leadtime) != len(data.leadtime):
             if not hide_warnings:
                 print(
                     "WARNING: no climatology available for {} days of reftime {}. Applying interpolation.".format(
                         len(data.leadtime) - len(clim.leadtime), reftime
                     )
                 )
             clim = clim.interp(
                 leadtime=data.leadtime,
                 kwargs={"fill_value": "extrapolate"},
             )
 
-        if not hide_print:
-            print(
-                "climatology for reftime {}: n refs = {}".format(
-                    reftime, len(hc_reftimes_in_window)
-                )
-            )
-        if not hide_plot:
-            clim.plot(label=reftime)
-
-        if standardize:
-            # ***** COMPUTE STD CLIMATOLOGY *****
-
-            climstd_stacked = (
-                data.sel(reftime=hc_reftimes_in_window, hc_year=(data.hc_year != 0))
-                    .sel(number=0)
-                    .stack(date=("reftime", "leadtime"))
-            )
-
-            climstd = (
-                climstd_stacked.assign_coords(
-                    days_since_reftime_init=(
-                        "date",
-                        (
-                                climstd_stacked.reftime.values.astype(
-                                    "datetime64[D]") - reftime + climstd_stacked.leadtime.values
-                        ).astype("timedelta64[D]")
-                        ,
-                    )
-                )
-                    .unstack()
-                    .groupby("days_since_reftime_init")
-                    .std(["stacked_reftime_leadtime", "hc_year"])
-                    .rolling(
-                    days_since_reftime_init=ndays_clim_filter,
-                    center=True,
-                    min_periods=1,
-                )
-                    .mean()
-                    .sel(days_since_reftime_init=slice(np.timedelta64(0, "D"), data.leadtime[-1]))
-                    .rename(days_since_reftime_init="leadtime")
-            )
-
-            if len(climstd.leadtime) != len(data.leadtime):
-                if not hide_warnings:
-                    print(
-                        "WARNING: no std climatology available for {} days of reftime {}. Applying interpolation.".format(
-                            len(data.leadtime) - len(climstd.leadtime),
-                            reftime,
-                        )
-                    )
-                climstd = climstd.interp(
-                    leadtime=data.leadtime,
-                    kwargs={"fill_value": "extrapolate"},
-                )
+        clim_list.append(clim)
 
-            data_anomstd_oneref = (data.sel(reftime=reftime) - clim) / climstd
-            data_by_reftime_list.append(data_anomstd_oneref)
-            climstd_list.append(climstd)
-
-        else:
-            data_anom_oneref = data.sel(reftime=reftime) - clim
-            data_by_reftime_list.append(data_anom_oneref)
+    clim_list = xr.concat(clim_list, dim="reftime")
+    return clim_list
 
-        clim_list.append(clim)
 
-    anom = xr.concat(data_by_reftime_list, dim="reftime").transpose(*data.dims)
+def nam(dataarray):
+    """
+    Not implemented.
 
-    if return_clim_lists:
-        return anom, clim_list, climstd_list
-    else:
-        return anom
+    Parameters
+    ----------
+    dataarray : xr.DataArray
 
+    Returns
+    -------
 
-def nam(z):
-    z_sel = z.sortby("latitude").sel(latitude=slice(65, 90))
-    weights = np.cos(np.deg2rad(z.latitude))
-    avg = (z_sel * weights).mean(["longitude", "latitude"])
-    res = -1 * deseasonalize(avg, standardize=True)
-    return res
+    """
+    print("Not Implemented")
```

### Comparing `s2stools-0.1.0/setup.py` & `s2stools-0.2.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from setuptools import setup
+from setuptools import find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.2.0'
 DESCRIPTION = 'python tools for handling s2s forecast data'
-LONG_DESCRIPTION = 'python tools for handling s2s forecast data.' \
-                   'Including submodules: ' \
-                   '<download> for retreiving s2s forecasts, ' \
-                   '<clim> for deseasonalization, ' \
-                   '<events> for creating event composites, ' \
-                   '<plot> for matplotlib utilities, ' \
-                   '<process> for handling data structures, ' \
-                   '<utils> for further utilities and <tests>'
+LONG_DESCRIPTION = 'python tools for handling s2s forecast data.'
 
 setup(
     name='s2stools',
     version=VERSION,
     author='Jonas Spaeth',
     author_email='jonas.spaeth@physik.uni-muenchen.de',
-    packages=['s2stools', 's2stools.clim', "s2stools.download", "s2stools.download.ecmwf", "s2stools.events",
-              "s2stools.plot", "s2stools.process", "s2stools.tests", "s2stools.utils"],
+    # packages=['s2stools', 's2stools.clim', "s2stools.download", "s2stools.download.ecmwf", "s2stools.events",
+    #           "s2stools.plot", "s2stools.process", "s2stools.tests", "s2stools.utils"],
+    packages=['s2stools'],
+    # packages=find_packages(),
     scripts=[],  # ['bin/script1','bin/script2'],
     # url='http://pypi.python.org/pypi/PackageName/',
     license='LICENSE.txt',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     install_requires=[
         "numpy",
         "xarray",
-        "ecmwf-api-client"
+        "tqdm",
+        "pandas",
+        "matplotlib"
     ],
 )
```

