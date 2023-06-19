# Comparing `tmp/gw_eccentricity-1.0.1.tar.gz` & `tmp/gw_eccentricity-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gw_eccentricity-1.0.1.tar", last modified: Mon Apr 24 13:20:50 2023, max compression
+gzip compressed data, was "gw_eccentricity-1.0.2.tar", last modified: Mon Jun 19 13:15:28 2023, max compression
```

## Comparing `gw_eccentricity-1.0.1.tar` & `gw_eccentricity-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 vijay      (502) staff       (20)        0 2023-04-24 13:20:50.558048 gw_eccentricity-1.0.1/
--rw-r--r--   0 vijay      (502) staff       (20)     5128 2023-04-24 13:20:50.557856 gw_eccentricity-1.0.1/PKG-INFO
--rw-r--r--   0 vijay      (502) staff       (20)     3638 2023-02-24 09:47:49.000000 gw_eccentricity-1.0.1/README.md
-drwxr-xr-x   0 vijay      (502) staff       (20)        0 2023-04-24 13:20:50.554904 gw_eccentricity-1.0.1/gw_eccentricity/
--rw-r--r--   0 vijay      (502) staff       (20)      435 2023-02-11 16:46:41.000000 gw_eccentricity-1.0.1/gw_eccentricity/__init__.py
--rw-r--r--   0 vijay      (502) staff       (20)     4505 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/gw_eccentricity/compare_methods.py
--rw-r--r--   0 vijay      (502) staff       (20)   139591 2023-04-24 13:07:54.000000 gw_eccentricity-1.0.1/gw_eccentricity/eccDefinition.py
--rw-r--r--   0 vijay      (502) staff       (20)     1884 2022-09-20 13:37:08.000000 gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingAmplitude.py
--rw-r--r--   0 vijay      (502) staff       (20)     2545 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingAmplitudeFits.py
--rw-r--r--   0 vijay      (502) staff       (20)      810 2022-09-20 13:37:08.000000 gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingFrequency.py
--rw-r--r--   0 vijay      (502) staff       (20)    48055 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingFrequencyFits.py
--rw-r--r--   0 vijay      (502) staff       (20)     2184 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingResidualAmplitude.py
--rw-r--r--   0 vijay      (502) staff       (20)     1294 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingResidualFrequency.py
--rw-r--r--   0 vijay      (502) staff       (20)     3211 2022-06-16 18:35:52.000000 gw_eccentricity-1.0.1/gw_eccentricity/group_nr_waveforms.py
--rw-r--r--   0 vijay      (502) staff       (20)    18160 2023-04-24 13:18:54.000000 gw_eccentricity-1.0.1/gw_eccentricity/gw_eccentricity.py
--rw-r--r--   0 vijay      (502) staff       (20)    49274 2023-02-22 10:21:11.000000 gw_eccentricity-1.0.1/gw_eccentricity/load_data.py
--rw-r--r--   0 vijay      (502) staff       (20)     5846 2023-04-24 13:07:54.000000 gw_eccentricity-1.0.1/gw_eccentricity/plot_settings.py
--rw-r--r--   0 vijay      (502) staff       (20)     5299 2022-10-10 19:26:56.000000 gw_eccentricity-1.0.1/gw_eccentricity/truncate_waveform_by_flow.py
--rw-r--r--   0 vijay      (502) staff       (20)    12427 2023-02-22 10:21:11.000000 gw_eccentricity-1.0.1/gw_eccentricity/utils.py
-drwxr-xr-x   0 vijay      (502) staff       (20)        0 2023-04-24 13:20:50.556328 gw_eccentricity-1.0.1/gw_eccentricity.egg-info/
--rw-r--r--   0 vijay      (502) staff       (20)     5128 2023-04-24 13:20:50.000000 gw_eccentricity-1.0.1/gw_eccentricity.egg-info/PKG-INFO
--rw-r--r--   0 vijay      (502) staff       (20)      960 2023-04-24 13:20:50.000000 gw_eccentricity-1.0.1/gw_eccentricity.egg-info/SOURCES.txt
--rw-r--r--   0 vijay      (502) staff       (20)        1 2023-04-24 13:20:50.000000 gw_eccentricity-1.0.1/gw_eccentricity.egg-info/dependency_links.txt
--rw-r--r--   0 vijay      (502) staff       (20)       26 2023-04-24 13:20:50.000000 gw_eccentricity-1.0.1/gw_eccentricity.egg-info/requires.txt
--rw-r--r--   0 vijay      (502) staff       (20)       16 2023-04-24 13:20:50.000000 gw_eccentricity-1.0.1/gw_eccentricity.egg-info/top_level.txt
--rw-r--r--   0 vijay      (502) staff       (20)       38 2023-04-24 13:20:50.558096 gw_eccentricity-1.0.1/setup.cfg
--rw-r--r--   0 vijay      (502) staff       (20)     1393 2023-02-22 10:38:49.000000 gw_eccentricity-1.0.1/setup.py
-drwxr-xr-x   0 vijay      (502) staff       (20)        0 2023-04-24 13:20:50.557622 gw_eccentricity-1.0.1/test/
--rw-r--r--   0 vijay      (502) staff       (20)     1524 2023-02-22 10:21:11.000000 gw_eccentricity-1.0.1/test/test_example_notebooks.py
--rw-r--r--   0 vijay      (502) staff       (20)     2275 2022-11-24 23:10:42.000000 gw_eccentricity-1.0.1/test/test_interface.py
--rw-r--r--   0 vijay      (502) staff       (20)     9141 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/test/test_mks_vs_dimless_units.py
--rw-r--r--   0 vijay      (502) staff       (20)     2871 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/test/test_regression.py
--rw-r--r--   0 vijay      (502) staff       (20)     2498 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/test/test_time_convention.py
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 13:15:28.916770 gw_eccentricity-1.0.2/
+-rw-r--r--   0 arif      (1000) arif      (1000)     1084 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/LICENSE
+-rw-r--r--   0 arif      (1000) arif      (1000)     4390 2023-06-19 13:15:28.916770 gw_eccentricity-1.0.2/PKG-INFO
+-rw-r--r--   0 arif      (1000) arif      (1000)     3638 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/README.md
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 13:15:28.870770 gw_eccentricity-1.0.2/gw_eccentricity/
+-rw-r--r--   0 arif      (1000) arif      (1000)      435 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/__init__.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     4505 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/compare_methods.py
+-rw-r--r--   0 arif      (1000) arif      (1000)   140682 2023-06-19 06:13:53.000000 gw_eccentricity-1.0.2/gw_eccentricity/eccDefinition.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     1884 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingAmplitude.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     2545 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingAmplitudeFits.py
+-rw-r--r--   0 arif      (1000) arif      (1000)      810 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingFrequency.py
+-rw-r--r--   0 arif      (1000) arif      (1000)    47793 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingFrequencyFits.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     2184 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingResidualAmplitude.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     1294 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingResidualFrequency.py
+-rw-r--r--   0 arif      (1000) arif      (1000)    18175 2023-06-19 06:14:17.000000 gw_eccentricity-1.0.2/gw_eccentricity/gw_eccentricity.py
+-rw-r--r--   0 arif      (1000) arif      (1000)    49295 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/load_data.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     6103 2023-06-17 09:38:49.000000 gw_eccentricity-1.0.2/gw_eccentricity/plot_settings.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     5299 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/truncate_waveform_by_flow.py
+-rw-r--r--   0 arif      (1000) arif      (1000)    12416 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/utils.py
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 13:15:28.871770 gw_eccentricity-1.0.2/gw_eccentricity.egg-info/
+-rw-r--r--   0 arif      (1000) arif      (1000)     4390 2023-06-19 13:15:28.000000 gw_eccentricity-1.0.2/gw_eccentricity.egg-info/PKG-INFO
+-rw-r--r--   0 arif      (1000) arif      (1000)      930 2023-06-19 13:15:28.000000 gw_eccentricity-1.0.2/gw_eccentricity.egg-info/SOURCES.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)        1 2023-06-19 13:15:28.000000 gw_eccentricity-1.0.2/gw_eccentricity.egg-info/dependency_links.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)       26 2023-06-19 13:15:28.000000 gw_eccentricity-1.0.2/gw_eccentricity.egg-info/requires.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)       16 2023-06-19 13:15:28.000000 gw_eccentricity-1.0.2/gw_eccentricity.egg-info/top_level.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)       38 2023-06-19 13:15:28.916770 gw_eccentricity-1.0.2/setup.cfg
+-rw-r--r--   0 arif      (1000) arif      (1000)     1393 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/setup.py
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 13:15:28.915770 gw_eccentricity-1.0.2/test/
+-rw-r--r--   0 arif      (1000) arif      (1000)     1524 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/test/test_example_notebooks.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     2275 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/test/test_interface.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     9161 2023-06-19 06:13:53.000000 gw_eccentricity-1.0.2/test/test_mks_vs_dimless_units.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     2871 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/test/test_regression.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     2498 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/test/test_time_convention.py
```

### Comparing `gw_eccentricity-1.0.1/README.md` & `gw_eccentricity-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.1/gw_eccentricity/compare_methods.py` & `gw_eccentricity-1.0.2/gw_eccentricity/compare_methods.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.1/gw_eccentricity/eccDefinition.py` & `gw_eccentricity-1.0.2/gw_eccentricity/eccDefinition.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,25 +266,25 @@
 
     def truncate_dataDict_if_necessary(self,
                                        dataDict,
                                        num_orbits_to_exclude_before_merger,
                                        extra_kwargs):
         """Truncate dataDict if "num_orbits_to_exclude_before_merger" is not None.
 
-        parameters:
+        parameters
         ----------
         dataDict:
             Dictionary containing modes and times.
         num_orbits_to_exclude_before_merger: Number of orbits to exclude before
             merger to get the truncated dataDict.
         extra_kwargs:
             Extra kwargs passed to the measure eccentricity.
 
-        returns:
-        --------
+        Returns
+        -------
         dataDict:
             Truncated if num_orbits_to_exclude_before_merger is not None
             else the unchanged dataDict.
         t_merger:
             Merger time evaluated as the time of the global maximum of
             amplitude_using_all_modes. This is computed before the truncation.
         amp22_merger:
@@ -529,18 +529,20 @@
 
         It might happen that an extremum between two successive extrema is
         missed by the extrema finder, This would result in the two extrema
         being too far from each other and therefore a jump in extrema will be
         introduced.
 
         To detect if an extremum has been missed we do the following:
+
         - Compute the phase22 difference between i-th and (i+1)-th extrema:
           delta_phase22_extrema[i] = phase22_extrema[i+1] - phase22_extrema[i]
         - Compute the ratio of delta_phase22: r_delta_phase22_extrema[i] =
           delta_phase22_extrema[i+1]/delta_phase22_extrema[i]
+
         For correctly separated extrema, the ratio r_delta_phase22_extrema
         should be close to 1.
 
         Therefore if anywhere r_delta_phase22_extrema[i] >
         max_r_delta_phase22_extrema, where max_r_delta_phase22_extrema = 1.5 by
         default, then delta_phase22_extrema[i+1] is too large and implies that
         phase22 difference between (i+2)-th and (i+1)-th extrema is too large
@@ -866,93 +868,107 @@
         mode. We currently only allow time-domain, nonprecessing waveforms. We
         evaluate omega22(t) at pericenter times, t_pericenters, and build a
         spline interpolant omega22_pericenters(t) using those data
         points. Similarly, we build omega22_apocenters(t) using omega22(t) at
         the apocenter times, t_apocenters.
 
         Using omega22_pericenters(t) and omega22_apocenters(t), we first
-        compute e_omega22(t), as described in Eq.(4) of arXiv:2302.11257. We
+        compute e_omega22(t), as described in Eq.(4) of `arXiv:2302.11257`_. We
         then use e_omega22(t) to compute the eccentricity egw(t) using Eq.(8)
-        of arXiv:2302.11257. Mean anomaly is defined using t_pericenters, as
-        described in Eq.(10) of arXiv:2302.11257.
+        of `arXiv:2302.11257`_. Mean anomaly is defined using t_pericenters, as
+        described in Eq.(10) of `arXiv:2302.11257`_.
 
         To find t_pericenters/t_apocenters, one can look for extrema in
         different waveform data, like omega22(t) or Amp22(t), the amplitude of
         the (2, 2) mode. Pericenters correspond to the local maxima, while
         apocenters correspond to the local minima in the data. The method
         option (described below) lets the user pick which waveform data to use
         to find t_pericenters/t_apocenters.
 
-        parameters:
+        .. _arXiv:2302.11257: https://arxiv.org/abs/2302.11257
+
+        Parameters
         ----------
-        tref_in:
+        tref_in : array or float
             Input reference time at which to measure eccentricity and mean
-            anomaly.  Can be a single float or an array.
+            anomaly.
 
-        fref_in:
+        fref_in : array or float
             Input reference GW frequency at which to measure the eccentricity
-            and mean anomaly. Can be a single float or an array. Only one of
-            tref_in/fref_in should be provided.
+            and mean anomaly. Only one of *tref_in*/*fref_in* should be
+            provided.
 
-            Given an fref_in, we find the corresponding tref_in such that
-            omega22_average(tref_in) = 2 * pi * fref_in. Here,
-            omega22_average(t) is a monotonically increasing average frequency
-            obtained from the instantaneous omega22(t). omega22_average(t)
-            defaults to the orbit averaged omega22, but other options are
-            available (see omega22_averaging_method below).
+            Given an *fref_in*, we find the corresponding tref_in such that::
+
+                omega22_average(tref_in) = 2 * pi * fref_in
+
+            Here, omega22_average(t) is a monotonically increasing average
+            frequency obtained from the instantaneous
+            omega22(t). omega22_average(t) defaults to the orbit averaged
+            omega22, but other options are available (see
+            omega22_averaging_method below).
 
             Eccentricity and mean anomaly measurements are returned on a subset
-            of tref_in/fref_in, called tref_out/fref_out, which are described
-            below.  If dataDict is provided in dimensionless units, tref_in
-            should be in units of M and fref_in should be in units of
-            cycles/M. If dataDict is provided in MKS units, t_ref should be in
-            seconds and fref_in should be in Hz.
+            of *tref_in*/*fref_in*, called *tref_out*/*fref_out*, which are
+            described below.  If *dataDict* is provided in dimensionless units,
+            *tref_in* should be in units of M and *fref_in* should be in units
+            of cycles/M. If dataDict is provided in MKS units, *t_ref* should
+            be in seconds and *fref_in* should be in Hz.
 
-        returns:
-        --------
-        A dictionary containing the following keys
-        tref_out:
-            tref_out is the output reference time at which eccentricity and
-            mean anomaly are measured.
-            tref_out is included in the returned dictionary only when tref_in
-            is provided.
-            Units of tref_out are the same as that of tref_in.
-
-            tref_out is set as
-            tref_out = tref_in[tref_in >= tmin & tref_in <= tmax],
-            where tmax = min(t_pericenters[-1], t_apocenters[-1]) and
-                  tmin = max(t_pericenters[0], t_apocenters[0]),
-            As eccentricity measurement relies on the interpolants
-            omega22_pericenters(t) and omega22_apocenters(t), the above cutoffs
-            ensure that we only compute the eccentricity where both
-            omega22_pericenters(t) and omega22_apocenters(t) are within their
-            bounds.
-
-        fref_out:
-            fref_out is the output reference frequency at which eccentricity
-            and mean anomaly are measured.
-            fref_out is included in the returned dictionary only when fref_in
-            is provided.
-            Units of fref_out are the same as that of fref_in.
-
-            fref_out is set as
-            fref_out = fref_in[fref_in >= fref_min && fref_in <= fref_max],
-            where fref_min/fref_max are minimum/maximum allowed reference
-            frequency, with fref_min = omega22_average(tmin_for_fref)/2/pi
-            and fref_max = omega22_average(tmax_for_fref)/2/pi.
-            tmin_for_fref/tmax_for_fref are close to tmin/tmax, see
-            eccDefinition.get_fref_bounds() for details.
-
-        eccentricity:
-            Measured eccentricity at tref_out/fref_out. Same type as
-            tref_out/fref_out.
-
-        mean_anomaly:
-            Measured mean anomaly at tref_out/fref_out. Same type as
-            tref_out/fref_out.
+        Returns
+        -------
+        A dictionary with the following keys
+            tref_out
+                *tref_out* is the output reference time at which eccentricity
+                and mean anomaly are measured.  *tref_out* is included in the
+                returned dictionary only when *tref_in* is provided.  Units of
+                *tref_out* are the same as that of *tref_in*.
+
+                tref_out is set as::
+
+                    tref_out = tref_in[tref_in >= tmin & tref_in <= tmax],
+
+                where, ::
+
+                    tmax = min(t_pericenters[-1], t_apocenters[-1])
+                    tmin = max(t_pericenters[0], t_apocenters[0])
+
+                As eccentricity measurement relies on the interpolants
+                omega22_pericenters(t) and omega22_apocenters(t), the above
+                cutoffs ensure that we only compute the eccentricity where both
+                omega22_pericenters(t) and omega22_apocenters(t) are within
+                their bounds.
+
+            fref_out
+                *fref_out* is the output reference frequency at which
+                eccentricity and mean anomaly are measured.  *fref_out* is
+                included in the returned dictionary only when *fref_in* is
+                provided.  Units of *fref_out* are the same as that of
+                *fref_in*.
+
+                *fref_out* is set as::
+
+                    fref_out = fref_in[fref_in >= fref_min && fref_in <= fref_max]
+
+                where, fref_min/fref_max are minimum/maximum allowed reference
+                frequency, with::
+
+                    fref_min = omega22_average(tmin_for_fref)/2/pi
+                    fref_max = omega22_average(tmax_for_fref)/2/pi
+
+                tmin_for_fref/tmax_for_fref are close to tmin/tmax, see
+                :meth:`eccDefinition.get_fref_bounds()` for details.
+
+            eccentricity
+                Measured eccentricity at *tref_out*/*fref_out*. Same type as
+                *tref_out*/*fref_out*.
+
+            mean_anomaly
+                Measured mean anomaly at *tref_out*/*fref_out*. Same type as
+                *tref_out*/*fref_out*.
         """
         # Get the pericenters and apocenters
         pericenters = self.find_extrema("pericenters")
         original_pericenters = pericenters.copy()
         self.check_num_extrema(pericenters, "pericenters")
         # In some cases it is easier to find the pericenters than finding the
         # apocenters. For such cases, one can only find the pericenters and use
@@ -1099,21 +1115,21 @@
         else:
             return_dict.update({"tref_out": self.tref_out})
         return return_dict
 
     def et_from_ew22_0pn(self, ew22):
         """Get temporal eccentricity at Newtonian order.
 
-        Parameters:
-        -----------
+        Parameters
+        ----------
         ew22:
             eccentricity measured from the 22-mode frequency.
 
-        Returns:
-        --------
+        Returns
+        -------
         et:
             Temporal eccentricity at Newtonian order.
         """
         psi = np.arctan2(1. - ew22*ew22, 2.*ew22)
         et = np.cos(psi/3.) - np.sqrt(3) * np.sin(psi/3.)
 
         return et
@@ -1122,21 +1138,21 @@
         """
         Compute eccentricity at time t.
 
         Compute e_omega22 from the value of omega22_pericenters_interpolant and
         omega22_apocenters_interpolant at t using Eq.(4) in arXiv:2302.11257
         and then use Eq.(8) in arXiv:2302.11257 to compute e_gw from e_omega22.
 
-        Paramerers:
-        -----------
+        Paramerers
+        ----------
         t:
             Time to compute the eccentricity at. Could be scalar or an array.
 
-        Returns:
-        --------
+        Returns
+        -------
         Eccentricity at t.
         """
         # Check that t is within tmin and tmax to avoid extrapolation
         self.check_time_limits(t)
 
         omega22_pericenter_at_t = self.omega22_pericenters_interp(t)
         omega22_apocenter_at_t = self.omega22_apocenters_interp(t)
@@ -1146,24 +1162,24 @@
                              + np.sqrt(omega22_apocenter_at_t)))
         # get the  temporal eccentricity from e_omega22
         return self.et_from_ew22_0pn(self.e_omega22)
 
     def derivative_of_eccentricity(self, t, n=1):
         """Get time derivative of eccentricity.
 
-        Parameters:
-        -----------
-        t:
+        Parameters
+        ----------
+        t
             Times to get the derivative at.
-        n: int
+        n : int
             Order of derivative. Should be 1 or 2, since it uses
             cubic spine to get the derivatives.
 
-        Returns:
-        --------
+        Returns
+        -------
             nth order time derivative of eccentricity.
         """
         # Check that t is within tmin and tmax to avoid extrapolation
         self.check_time_limits(t)
 
         if self.ecc_for_checks is None:
             self.ecc_for_checks = self.compute_eccentricity(
@@ -1188,21 +1204,21 @@
         (n+1)th pericenter. Therefore, if we have N+1 pericenters, we collect,
         xVals = [tp_0, tp_1, tp_2, ..., tp_N]
         yVals = [0, 2pi, 4pi, ..., 2*pi*N]
         where tp_n is the time at the nth pericenter.
         Finally, we build a linear interpolant for y using these xVals and
         yVals.
 
-        Parameters:
-        -----------
+        Parameters
+        ----------
         t:
             Time to compute mean anomaly at. Could be scalar or an array.
 
-        Returns:
-        --------
+        Returns
+        -------
         Mean anomaly at t.
         """
         # Check that t is within tmin and tmax to avoid extrapolation
         self.check_time_limits(t)
 
         # Get the mean anomaly at the pericenters
         mean_ano_pericenters = np.arange(len(self.t_pericenters)) * 2 * np.pi
@@ -1241,21 +1257,21 @@
         executing the body if debug_level < 1, unless always_return=True.
 
         If calling this function externally from an instance of eccDefinition,
         you need to change self.debug_level to be >= 1 if you want to
         un-suppress the warnings. always_return=True is not sufficient to
         un-suppress the warnings.
 
-        parameters:
-        always_return:
+        Parameters
+        ----------
+        always_return : bool, default: False
             The return values of this function are used by some plotting
             functions, so if always_return=True, we execute the body and
             return values regardless of debug_level. However, the warnings
             will still be suppressed for debug_level < 1.
-            Default is False.
         """
 
         # This function only has checks with the flag important=False, which
         # means that warnings are suppressed when debug_level < 1.
         # We return without running the rest of the body to avoid unnecessary
         # computations, unless always_return=True.
         if self.debug_level < 1 and always_return is False:
@@ -1296,18 +1312,19 @@
                           self.debug_level, important=False)
         return orb_phase_diff, orb_phase_diff_ratio
 
     def check_monotonicity_and_convexity(self,
                                          check_convexity=False):
         """Check if measured eccentricity is a monotonic function of time.
 
-        parameters:
-        check_convexity:
+        Parameters
+        ----------
+        check_convexity : bool, default: False
             In addition to monotonicity, it will check for
-            convexity as well. Default is False.
+            convexity as well.
         """
         if self.decc_dt_for_checks is None:
             self.decc_dt_for_checks = self.derivative_of_eccentricity(
                 self.t_for_checks, n=1)
 
         # Is ecc(t) a monotonically decreasing function?
         if any(self.decc_dt_for_checks > 0):
@@ -1476,19 +1493,19 @@
         averaged omega22 calculated between ith and (i+1)th pericenter. That
         is, omega22_average((t[i] + t[i+1])/2) = int_t[i]^t[i+1] omega22(t) dt
         / (t[i+1] - t[i]), where t[i] is the time at the ith pericenter.  And
         similarly, we calculate the t_average_apocenters. We combine
         t_average_pericenters and t_average_apocenters, and sort them to obtain
         t_average.
 
-        Returns:
-        --------
-        t_for_orbit_averaged_omega22:
+        Returns
+        -------
+        t_for_orbit_averaged_omega22
             Times associated with orbit averaged omega22
-        sorted_idx_for_orbit_averaged_omega22:
+        sorted_idx_for_orbit_averaged_omega22
             Indices used to sort the times associated with orbit averaged
             omega22
         """
         # get the mid points between the pericenters as avg time for
         # pericenters
         self.t_average_pericenters \
             = 0.5 * (self.t[self.pericenters_location][:-1]
@@ -1504,73 +1521,82 @@
         sorted_idx_for_orbit_averaged_omega22 = np.argsort(
             t_for_orbit_averaged_omega22)
         t_for_orbit_averaged_omega22 = t_for_orbit_averaged_omega22[
             sorted_idx_for_orbit_averaged_omega22]
         return [t_for_orbit_averaged_omega22,
                 sorted_idx_for_orbit_averaged_omega22]
 
-    def get_orbit_averaged_omega22_at_pericenters(self):
+    def get_orbit_averaged_omega22_between_pericenters(self):
         """Get orbital average of omega22 between two consecutive pericenters.
 
+        Given N pericenters at times t[i], i=0...N-1, this function returns a
+        np.array of length N-1, where result[i] is the frequency averaged over
+        [t[i], t[i+1]]. result[i] is associated with the time at the temporal
+        midpoint between t[i] and t[i+1], i.e (t[i] + t[i+1])/2. See Eq.(12)
+        and Eq.(13) in arXiv:2302.11257 for details.
+
         Orbital average of omega22 between two consecutive pericenters
         i-th and (i+1)-th is given by
         <omega22>_i = (int_t[i]^t[i+1] omega22(t) dt)/(t[i+1] - t[i])
         t[i] is the time at the i-th extrema.
         Integration of omega22(t) from t[i] to t[i+1] is the same
         as taking the difference of phase22(t) between t[i] and t[i+1]
         <omega22>_i = (phase22[t[i+1]] - phase22[t[i]])/(t[i+1] - t[i])
         """
         return (np.diff(self.phase22[self.pericenters_location]) /
                 np.diff(self.t[self.pericenters_location]))
 
-    def get_orbit_averaged_omega22_at_apocenters(self):
+    def get_orbit_averaged_omega22_between_apocenters(self):
         """Get orbital average of omega22 between two consecutive apocenters.
 
-        The procedure to get the orbital average of omega22 at apocenters is
-        the same as that at pericenters. See documentation of
-        `get_orbit_averaged_omega22_at_pericenters` for details.
+        The procedure to get the orbital average of omega22 between apocenters
+        is the same as that between pericenters. See documentation of
+        `get_orbit_averaged_omega22_between_pericenters` for details.
         """
         return (np.diff(self.phase22[self.apocenters_location]) /
                 np.diff(self.t[self.apocenters_location]))
 
-    def compute_orbit_averaged_omega22_at_extrema(self, t):
-        """Compute reference frequency by orbital averaging omega22 at extrema.
+    def compute_orbit_averaged_omega22_between_extrema(self, t):
+        """Compute reference frequency by orbital averaging omega22 between extrema.
 
-        We compute the orbital average of omega22 at the pericenters
-        and the apocenters following:
+        We compute the orbital average of omega22 between two consecutive
+        extrema as following:
         <omega22>_i = (int_t[i]^t[i+1] omega22(t) dt) / (t[i+1] - t[i])
         where t[i] is the time of ith extrema and the suffix `i` stands for the
         i-th orbit between i-th and (i+1)-th extrema
         <omega22>_i is associated with the temporal midpoint between the i-th
         and (i+1)-th extrema,
         <t>_i = (t[i] + t[i+1]) / 2
+        See Eq.(12) and Eq.(13) in arXiv:2302.11257 for more details.
 
-        We do this averaging for pericenters and apocenters using the functions
-        `get_orbit_averaged_omega22_at_pericenters` and
-        `get_orbit_averaged_omega22_at_apocenters` and combine the results.
-        The combined array is then sorted using the sorting indices from
-        `get_t_average_for_orbit_averaged_omega22`.
+        We do this averaging between consecutive pericenters and consecutive
+        apocenters using the functions
+        `get_orbit_averaged_omega22_between_pericenters` and
+        `get_orbit_averaged_omega22_between_apocenters` and combine the
+        results. The combined array is then sorted using the sorting indices
+        from `get_t_average_for_orbit_averaged_omega22`.
 
         Finally we interpolate the data {<t>_i, <omega22>_i} and evaluate the
         interpolant at the input times `t`.
         """
         # get orbit averaged omega22 between consecutive pericenrers
-        # and apoceneters
+        # and consecutive apoceneters
         self.orbit_averaged_omega22_pericenters \
-            = self.get_orbit_averaged_omega22_at_pericenters()
+            = self.get_orbit_averaged_omega22_between_pericenters()
         self.orbit_averaged_omega22_apocenters \
-            = self.get_orbit_averaged_omega22_at_apocenters()
+            = self.get_orbit_averaged_omega22_between_apocenters()
         # check monotonicity of the omega22 average
         self.check_monotonicity_of_omega22_average(
             self.orbit_averaged_omega22_pericenters,
             "omega22 averaged [pericenter to pericenter]")
         self.check_monotonicity_of_omega22_average(
             self.orbit_averaged_omega22_apocenters,
             "omega22 averaged [apocenter to apocenter]")
-        # combine the average omega22 at pericenters and apocenters
+        # combine the average omega22 between consecutive pericenters and
+        # consecutive apocenters
         orbit_averaged_omega22 = np.append(
             self.orbit_averaged_omega22_apocenters,
             self.orbit_averaged_omega22_pericenters)
 
         # get the times associated to the orbit averaged omega22
         if not hasattr(self, "t_for_orbit_averaged_omega22"):
             self.t_for_orbit_averaged_omega22,\
@@ -1591,17 +1617,19 @@
             t, self.t_for_orbit_averaged_omega22, orbit_averaged_omega22)
 
     def check_monotonicity_of_omega22_average(self,
                                               omega22_average,
                                               description="omega22 average"):
         """Check that omega average is monotonically increasing.
 
-        omega22_average:
+        Parameters
+        ----------
+        omega22_average : array-like
             1d array of omega22 averages to check for monotonicity.
-        description:
+        description : str
             String to describe what the the which omega22 average we are
             looking at.
         """
         idx_non_monotonic = np.where(
             np.diff(omega22_average) <= 0)[0]
         if len(idx_non_monotonic) > 0:
             first_idx = idx_non_monotonic[0]
@@ -1693,39 +1721,39 @@
         return self.interp(
             t, self.t_zeroecc_shifted, self.omega22_zeroecc)
 
     def get_available_omega22_averaging_methods(self):
         """Return available omega22 averaging methods."""
         available_methods = {
             "mean_of_extrema_interpolants": self.compute_mean_of_extrema_interpolants,
-            "orbit_averaged_omega22": self.compute_orbit_averaged_omega22_at_extrema,
+            "orbit_averaged_omega22": self.compute_orbit_averaged_omega22_between_extrema,
             "omega22_zeroecc": self.compute_omega22_zeroecc
         }
         return available_methods
 
     def get_omega22_average(self, method=None):
         """Get times and corresponding values of omega22 average.
 
-        Parameters:
-        -----------
-        method: str
+        Parameters
+        ----------
+        method : str
             omega22 averaging method. Must be one of the following:
             - "mean_of_extrema_interpolants"
             - "orbit_averaged_omega22"
             - "omega22_zeroecc"
             See get_available_omega22_averaging_methods for available averaging
             methods and Sec.IID of arXiv:2302.11257 for more details.
             Default is None which uses the method provided in
             `self.extra_kwargs["omega22_averaging_method"]`
 
-        Returns:
-        --------
-        t_for_omega22_average:
+        Returns
+        -------
+        t_for_omega22_average : array-like
             Times associated with omega22_average.
-        omega22_average:
+        omega22_average : array-like
             omega22 average using given "method".
             These are data interpolated on the times t_for_omega22_average,
             where t_for_omega22_average is a subset of tref_in passed to the
             eccentricity measurement function.
 
             For the "orbit_averaged_omega22" method, the original
             omega22_average data points <omega22>_i are obtained by averaging
@@ -1733,34 +1761,36 @@
             associated <t>_i are obtained by taking the times at the midpoints
             between i-th and i+1-the extrema, i.e., <t>_i = (t_i + t_(i+1))/2.
 
             These original orbit averaged omega22 data points can be accessed
             using the gwecc_object with the following variables
 
             - orbit_averaged_omega22_apocenters: orbit averaged omega22 between
-              apocenters This is available when measuring eccentricity at
-              reference frequency.  If it is not available, it can be computed
-              using `get_orbit_averaged_omega22_at_apocenters`
+              apocenters. This is available when measuring eccentricity at
+              reference frequency. If it is not available, it can be computed
+              using `get_orbit_averaged_omega22_between_apocenters`
             - t_average_apocenters: temporal midpoints between
               apocenters. These are associated with
               `orbit_averaged_omega22_apocenters`
             - orbit_averaged_omega22_pericenters: orbit averaged omega22
-              between pericenters This is available when measuring eccentricity
-              at reference frequency.  If it is not available, it can be
-              computed using `get_orbit_averaged_omega22_at_pericenters`
+              between pericenters. This is available when measuring
+              eccentricity at reference frequency. If it is not available, it
+              can be computed using
+              `get_orbit_averaged_omega22_between_pericenters`
             - t_average_pericenters: temporal midpoints between
               pericenters. These are associated with
               `orbit_averaged_omega22_pericenters`
         """
         if method is None:
             method = self.extra_kwargs["omega22_averaging_method"]
         if method != "orbit_averaged_omega22":
             # the average frequencies are using interpolants that use omega22
             # values between tmin and tmax, therefore the min and max time for
-            # which omega22 average are the same as tmin and tmax, respectively.
+            # which omega22 average are the same as tmin and tmax,
+            # respectively.
             self.tmin_for_fref = self.tmin
             self.tmax_for_fref = self.tmax
         else:
             self.t_for_orbit_averaged_omega22, self.sorted_idx_for_orbit_averaged_omega22 = \
                 self.get_t_average_for_orbit_averaged_omega22()
             # for orbit averaged omega22, the associated times are obtained
             # using the temporal midpoints of the extrema, therefore we need to
@@ -1796,14 +1826,15 @@
         Where fref_min/fref_max is the minimum/maximum allowed reference
         frequency for the given omega22 averaging method. See get_fref_bounds
         for more details.
         Finally, we find the times where omega22_average(t) = 2*pi*fref_out,
         and set those to tref_in.
 
         omega22_average(t) could be calculated in the following ways
+
         - Mean of the omega22 given by the spline through the pericenters and
           the spline through the apocenters, we call this
           "mean_of_extrema_interpolants"
         - Orbital average at the extrema, we call this
           "orbit_averaged_omega22"
         - omega22 of the zero eccentricity waveform, called "omega22_zeroecc"
 
@@ -1863,46 +1894,46 @@
         therefore is not None, then it returns the minimum and maximum of that
         omega22_average and does not recompute the omega22_average using the
         input `method`. In other words, if omega22_average is already not None
         then input `method` is ignored and the existing omega22_average is
         used.  To force recomputation of omega22_average, for example, with a
         new method one need to set it to None first.
 
-        Parameters:
-        -----------
-        method:
+        Parameters
+        ----------
+        method : str
             Omega22 averaging method.  See
             get_available_omega22_averaging_methods for available methods.
             Default is None which will use the default method for omega22
             averaging using `extra_kwargs["omega22_averaging_method"]`
 
-        Returns:
+        Returns
+        -------
             Minimum allowed reference frequency, Maximum allowed reference
             frequency.
-        --------
         """
         if self.omega22_average is None:
             self.t_for_omega22_average, self.omega22_average = self.get_omega22_average(method)
         return [min(self.omega22_average)/2/np.pi,
                 max(self.omega22_average)/2/np.pi]
 
     def get_fref_out(self, fref_in, method):
         """Get fref_out from fref_in that falls within the valid average f22 range.
 
-        Parameters:
+        Parameters
         ----------
-        fref_in:
+        fref_in : array-like
             Input 22 mode reference frequency array.
 
-        method:
+        method : str
             method for getting average omega22
 
-        Returns:
+        Returns
         -------
-        fref_out:
+        fref_out : array-like
             Slice of fref_in that satisfies:
             fref_in >= fref_min && fref_in < fref_max
         """
         fref_min, fref_max = self.get_fref_bounds(method)
         fref_out = fref_in[
             np.logical_and(fref_in >= fref_min,
                            fref_in < fref_max)]
@@ -1930,14 +1961,15 @@
         """Make diagnostic plots for the eccDefinition method.
 
         We plot different quantities to asses how well our eccentricity
         measurement method is working. This could be seen as a diagnostic tool
         to check an implemented method.
 
         We plot the following quantities
+
         - The eccentricity vs vs time
         - decc/dt vs time, this is to test the monotonicity of eccentricity as
           a function of time
         - mean anomaly vs time
         - omega_22 vs time with the pericenters and apocenters shown. This
           would show if the method is missing any pericenters/apocenters or
           selecting one which is not a pericenter/apocenter
@@ -1950,59 +1982,61 @@
           `omega22_averaging_method` is plotted as a function of time.
           omega22_average is used to get the reference time for a given
           reference frequency. Therefore, it should be a strictly monotonic
           function of time.
 
         Additionally, we plot the following if data for zero eccentricity is
         provided and method is not residual method
+
         - residual amp22 vs time with the location of pericenters and
           apocenters shown.
         - residual omega22 vs time with the location of pericenters and
           apocenters shown.
+
         If the method itself uses residual data, then add one plot for
+
         - data that is not being used for finding extrema.
-        For example, if method is ResidualAmplitude
-        then plot residual omega and vice versa.
-        These two plots further help in understanding any unwanted feature
-        in the measured eccentricity vs time plot. For example, non smoothness
-        in the residual omega22 would indicate that the data in omega22 is not
-        good which might be causing glitches in the measured eccentricity plot.
+          For example, if method is ResidualAmplitude then plot residual omega
+          and vice versa.  These two plots further help in understanding any
+          unwanted feature in the measured eccentricity vs time plot. For
+          example, non smoothness in the residual omega22 would indicate that
+          the data in omega22 is not good which might be causing glitches in
+          the measured eccentricity plot.
 
         Finally, plot
+
         - data that is being used for finding extrema.
 
-        Parameters:
-        -----------
-        add_help_text:
+        Parameters
+        ----------
+        add_help_text : bool, default: True
             If True, add text to describe features in the plot.
-            Default is True.
-        usetex:
+        usetex : bool, default: False
             If True, use TeX to render texts.
-            Default is False.
-        style:
+        style : str
             Set font size, figure size suitable for particular use case. For
             example, to generate plot for "APS" journals, use style="APS".  For
             showing plots in a jupyter notebook, use "Notebook" so that plots
             are bigger and fonts are appropriately larger and so on.  See
             plot_settings.py for more details.  If None, then uses "Notebook"
             when twocol is False and uses "APS" if twocol is True.
             Default is None.
-        use_fancy_settings:
+        use_fancy_settings : bool, default: True
             Use fancy settings for matplotlib to make the plot look prettier.
             See plot_settings.py for more details.
-            Default is True.
-        twocol:
-            Use a two column grid layout. Default is False.
-        **kwargs:
+        twocol : bool, default: False
+            Use a two column grid layout.
+        **kwargs
             kwargs to be passed to plt.subplots()
 
-        Returns:
-        fig:
+        Returns
+        -------
+        fig
             Figure object.
-        axarr:
+        axarr
             Axes object.
         """
         # Make a list of plots we want to add
         list_of_plots = [self.plot_eccentricity,
                          self.plot_mean_anomaly,
                          self.plot_omega22,
                          self.plot_data_used_for_finding_extrema,
@@ -2381,15 +2415,15 @@
             fig=None,
             ax=None,
             add_help_text=True,
             usetex=False,
             style="Notebook",
             use_fancy_settings=True,
             plot_omega22=True,
-            plot_orbit_averaged_omega22_at_extrema=False,
+            plot_orbit_averaged_omega22_between_extrema=False,
             **kwargs):
         """Plot omega22_average.
 
         Parameters:
         -----------
         fig:
             Figure object to add the plot to. If None, initiates a new figure
@@ -2412,17 +2446,17 @@
             Default is Notebook.
         use_fancy_settings:
             Use fancy settings for matplotlib to make the plot look prettier.
             See plot_settings.py for more details.
             Default is True.
         plot_omega22: bool
             If True, plot omega22 also. Default is True.
-        plot_orbit_averaged_omega22_at_extrema: bool
+        plot_orbit_averaged_omega22_between_extrema: bool
             If True and method is orbit_averaged_omega22, plot the the orbit
-            averaged omega22 at the extrema as well. Default is False.
+            averaged omega22 between the extrema as well. Default is False.
 
         Returns:
         --------
         fig, ax
         """
         if fig is None or ax is None:
             figNew, ax = plt.subplots(figsize=(figWidthsTwoColDict[style], 4))
@@ -2440,15 +2474,15 @@
         if plot_omega22:
             ax.plot(self.t, self.omega22,
                     c='k',
                     alpha=0.4,
                     lw=0.5,
                     label=labelsDict["omega22"])
         if (self.extra_kwargs["omega22_averaging_method"] == "orbit_averaged_omega22" and
-            plot_orbit_averaged_omega22_at_extrema):
+            plot_orbit_averaged_omega22_between_extrema):
             ax.plot(self.t_average_apocenters,
                     self.orbit_averaged_omega22_apocenters,
                     c=colorsDict["apocenter"],
                     marker=".", ls="",
                     label=labelsDict["orbit_averaged_omega22_apocenters"])
             ax.plot(self.t_average_pericenters,
                     self.orbit_averaged_omega22_pericenters,
@@ -2489,42 +2523,39 @@
             use_fancy_settings=True,
             **kwargs):
         """Plot amp22, the locations of the apocenters and pericenters.
 
         This would show if the method is missing any pericenters/apocenters or
         selecting one which is not a pericenter/apocenter.
 
-        Parameters:
-        -----------
-        fig:
+        Parameters
+        ----------
+        fig :
             Figure object to add the plot to. If None, initiates a new figure
-            object.  Default is None.
-        ax:
+            object. Default is None.
+        ax :
             Axis object to add the plot to. If None, initiates a new axis
-            object.  Default is None.
-        add_help_text:
+            object. Default is None.
+        add_help_text : bool, default: True
             If True, add text to describe features in the plot.
-            Default is True.
-        usetex:
+        usetex : bool, default: False
             If True, use TeX to render texts.
-            Default is False.
-        style:
+        style : str, default: ``Notebook``
             Set font size, figure size suitable for particular use case. For
-            example, to generate plot for "APS" journals, use style="APS".  For
-            showing plots in a jupyter notebook, use "Notebook" so that plots
-            are bigger and fonts are appropriately larger and so on.  See
+            example, to generate plot for ``APS`` journals, use ``style='APS'``.
+            For showing plots in a jupyter notebook, use ``Notebook`` so that
+            plots are bigger and fonts are appropriately larger and so on.  See
             plot_settings.py for more details.
-            Default is Notebook.
-        use_fancy_settings:
+        use_fancy_settings : bool, default: True
             Use fancy settings for matplotlib to make the plot look prettier.
-            See plot_settings.py for more details.
-            Default is True.
+            See :py:func:`plot_settings.use_fancy_plotsettings` for more
+            details.
 
-        Returns:
-        --------
+        Returns
+        -------
         fig, ax
         """
         if fig is None or ax is None:
             figNew, ax = plt.subplots(figsize=(figWidthsTwoColDict[style], 4))
         if use_fancy_settings:
             use_fancy_plotsettings(usetex=usetex, style=style)
         ax.plot(self.t, self.amp22,
@@ -2793,16 +2824,17 @@
             style="Notebook",
             use_fancy_settings=True,
             add_vline_at_tref=True,
             **kwargs):
         """Plot the data that is being used.
 
         Also the locations of the apocenters and pericenters.
-        Parameters:
-        -----------
+
+        Parameters
+        ----------
         fig:
             Figure object to add the plot to. If None, initiates a new figure
             object.  Default is None.
         ax:
             Axis object to add the plot to. If None, initiates a new axis
             object.  Default is None.
         add_help_text:
@@ -2923,17 +2955,17 @@
         Thus it does not find the locations of the apocenters using pericenter
         finder at all. It is useful in situation where finding pericenters is
         easy but finding the apocenters in between is difficult. This is the
         case for highly eccentric systems where eccentricity approaches 1. For
         such systems the amp22/omega22 data between the pericenters is almost
         flat and hard to find the local minima.
 
-        returns:
-        ------
-        locations of apocenters
+        Returns
+        -------
+        locations of apocenters : array-like
         """
         # NOTE: Assuming uniform time steps.
         # TODO: Make it work for non
         # uniform time steps In the following we get the location of mid point
         # between ith pericenter and (i+1)th pericenter as (loc[i] +
         # loc[i+1])/2 where loc is the array that contains the pericenter
         # locations. This works because time steps are assumed to be uniform
@@ -2956,18 +2988,18 @@
         steps in the time array of the waveform data.  NOTE: As the function
         name mentions, this should be used only for dimensionless units. This
         is because the `width_for_unit_timestep` parameter refers to unit
         timestep in units of M. It is the fiducial width to use if the time
         step is 1M. If using time in seconds, this would depend on the total
         mass.
 
-        Parameters:
+        Parameters
         ----------
-        width_for_unit_timestep:
+        width_for_unit_timestep : int
             Width to use when the time step in the wavefrom data is 1.
 
-        Returns:
+        Returns
         -------
         width:
             Minimal width to separate consecutive peaks.
         """
         return int(width_for_unit_timestep / (self.t[1] - self.t[0]))
```

### Comparing `gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingAmplitude.py` & `gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingAmplitude.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingAmplitudeFits.py` & `gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingAmplitudeFits.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingFrequency.py` & `gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingFrequency.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingFrequencyFits.py` & `gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingFrequencyFits.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,18 @@
 
 class eccDefinitionUsingFrequencyFits(eccDefinition):
     """Measure eccentricity by finding extrema location using freq fits."""
 
     def __init__(self, *args, **kwargs):
         """Init for eccDefinitionUsingWithFrequencyFits class.
 
-        parameters:
+        Parameters
         ----------
-        dataDict: Dictionary containing the waveform data.
+        dataDict : dict
+            Dictionary containing the waveform data.
         """
         super().__init__(*args, **kwargs)
         self.data_str = "omega22"
         self.label_for_data_for_finding_extrema = labelsDict[self.data_str]
         self.label_for_fit_to_data_for_finding_extrema \
             = labelsDict[f"{self.data_str}_fit"]
         # Make a copy of omega22 and use it to set data_for_finding_extrema.
@@ -89,15 +90,16 @@
                 "data": self.data_for_finding_extrema,
                 "t": self.t
             }
 
     def get_default_kwargs_for_fits_methods(self):
         """Get default kwargs to be used for Fits methods.
 
-        The kwargs are:
+        The kwargs are
+
         - "nPN": The PN exponent to use in the fit function. It is
           inspired by the functional form of frequency/amplitude in
           the leading Post-Newtonian order ~(t - t_merger)^nPN
         - "fit_bounds_max_amp_factor": To set the upper bound on the
           Amplitude A of the fitting function of the form A(t-T)^n.
           The upper bound of A is set as f0*fit_bounds_max_amp_factor,
           where f0 is the mean of the first and the last values of data
@@ -154,21 +156,21 @@
         self.num_orbits_for_global_fit = self.kwargs_for_fits_methods[
             "num_orbits_for_global_fit"]
         self.return_diagnostic_data = self.kwargs_for_fits_methods["return_diagnostic_data"]
 
     def find_extrema(self, extrema_type="pericenters"):
         """Find the extrema in the data.
 
-        parameters:
-        -----------
+        Parameters
+        ----------
         extrema_type:
             Either "pericenters" or "apocenters".
 
-        returns:
-        ------
+        Returns
+        -------
         array of positions of extrema.
         """
         # STEP 0 - setup
 
         if extrema_type == "pericenters":
             sign = +1
         elif extrema_type == "apocenters":
@@ -474,93 +476,107 @@
         #         - if  number of extrema != N_extrema:
         #             goto (A)  [i.e. compute a larger/smaller data-interval
         #             with new K]
         #         - if |extrema - old_extrema| < tol:  break
         #         - old_extrema=extrema
         #         - update fitting_func by fit to extrema
 
-
     def FindExtremaNearIdxRef(self,
                               idx_ref,
                               sign, Nbefore, Nafter, K,
                               f_fit, p_initial, bounds,
                               TOL,
                               increase_idx_ref_if_needed=True,
                               refine_extrema=False,
                               verbose=False,
                               pp=None,
                               plot_info=""):
         """given a 22-GW mode (t, phase22, data), identify a stretch of data
         [idx_lo, idx_hi] centered roughly around the index idx_ref which
         satisfies the following properties:
+
           - The interval [idx_lo, idx_hi] contains Nbefore+Nafter maxima
             (if sign==+1) or minimia (if sign==-1)
             of trend-subtracted data, where Nbefore exrema are before idx_ref
             and Nafter extrema are after idx_ref
           - The trend-subtraction is specified by the fitting function
-            data_trend = f_fit(t, *p).
-            Its fitting parameters *p are self-consistently fitted to the
+            `data_trend = f_fit(t, *p)`.
+            Its fitting parameters `*p` are self-consistently fitted to the
             N_extrema extrema.
           - if increase_idx_ref_if_needed, idx_ref is allowed to increase in
             order to reach the desired Nbefore.
 
-        INPUT
-          - idx_ref   - the reference index, i.e. the approximate middle of the
-            interval of data to be sought
-          - sign      - if +1, look for maxima, if -1, look for minima
-          - Nbefore   - number of extrema to identify before idx_ref
-          - Nafter    - number of extrema to identify after idx_ref
-                          if Nafter=Nbefore-1, then the Nbefore'th extremum
-                          will be centered
-          - K         - an estimate for the periastron advance of the binary,
-                        i.e. the increase of phase22/4pi between two extrema
-          - f_fit     - fitting function f_fit(t, *p) to use for
-                        trend-subtraction
-          - p_initial - initial guesses for the best-fit parametes
-          - p_bounds  - bounds for the fit-parameters
-          - TOL       - iterate until the maximum change in any one data at an
-                        extremum is less tha this TOL
-          - increase_idx_ref_if_needed -- if true, allows to increase idx_ref
-                                          in order to achieve Nbefore extrema
-                                          between start of dataset and idx_ref
-                                          (idx_ref will never be decreased, in
-                                          order to preserve monotonicity to
-                                          help tracing out an inspiral)
-
-          - pp a PdfPages object for a diagnostic output plot
-          - plot_info -- string placed into the title of the diagnostic plot
-
-        RETURNS:
-              idx_extrema, p, K, idx_ref, extrema_refined
-        where
-          - idx_extrema -- the indices of the identified extrema
-                           USUALLY len(idx_extrema) == Nbefore+Nafter HOWEVER,
-                           if not enough extrema can be identified (e.g.  end
-                           of data), then a shorter or even empty list can be
-                           returned
-
-          - p -- the fitting parameters of the best fit through the extrema
-          - K -- an updated estimate of the periastron advance K (i.e. the
-                 average increase of phase22 between extrema divided by 4pi)
-          - idx_ref -- a (potentially increased) value of idx_ref, so that
-                       Nbefore extrema were found between the start of the data
-                       and idx_ref
-          - extrema_refined=(t_extrema_refined, data_extrema_refined,
-                 phase22_extrema_refined) information about the
-                 parabolic-fit-refined extrema.  If RefineExtrema==True, these
-                 arrays have same length as idx_extrema.  Otherwise, empty.
-
-
         ASSUMPTIONS & POSSIBLE FAILURE MODES
+
           - if increase_idx_ref_if_needed == False, and idx_lo cannot be
             reduced enough to reach Nbefore -> raise Exception
           - if fewer extrema are identified than requested, then the function
             will return normally, but with len(idx_extrema) **SMALLER** than
             Nbefore+Nafter. This signals that the end of the data is reached,
             and that the user should not press to even larger idx_ref.
+
+        Parameters
+        ----------
+        idx_ref
+            the reference index, i.e. the approximate middle of the
+            interval of data to be sought
+        sign
+            if +1, look for maxima, if -1, look for minima
+        Nbefore
+            Number of extrema to identify before idx_ref
+        Nafter
+            Number of extrema to identify after idx_ref
+            if Nafter=Nbefore-1, then the Nbefore'th extremum
+            will be centered
+        K
+            an estimate for the periastron advance of the binary,
+            i.e. the increase of phase22/4pi between two extrema
+        f_fit
+            fitting function :func:`f_fit(t, *p)` to use for trend-subtraction
+        p_initial
+            initial guesses for the best-fit parametes
+        p_bounds
+            bounds for the fit-parameters
+        TOL
+            Iterate until the maximum change in any one data at an
+            extremum is less tha this TOL
+        increase_idx_ref_if_needed
+            if true, allows to increase idx_ref in order to achieve Nbefore
+            extrema between start of dataset and idx_ref (idx_ref will never be
+            decreased, in order to preserve monotonicity to help tracing out an
+            inspiral)
+
+        pp
+            a PdfPages object for a diagnostic output plot
+        plot_info
+            string placed into the title of the diagnostic plot
+
+        Returns
+        -------
+        idx_extrema
+            the indices of the identified extrema USUALLY
+            len(idx_extrema) == Nbefore+Nafter HOWEVER,
+            if not enough extrema can be identified
+            (e.g.  end of data), then a shorter or even empty list can be
+            returned
+
+        p
+            the fitting parameters of the best fit through the extrema
+        K
+            an updated estimate of the periastron advance K (i.e. the
+                 average increase of phase22 between extrema divided by 4pi)
+        idx_ref
+            a (potentially increased) value of idx_ref, so that
+                       Nbefore extrema were found between the start of the data
+                       and idx_ref
+        extrema_refined
+            (t_extrema_refined, data_extrema_refined, phase22_extrema_refined)
+            information about the
+            parabolic-fit-refined extrema.  If RefineExtrema==True, these
+            arrays have same length as idx_extrema.  Otherwise, empty.
         """
         extrema_type = {+1: "pericenters", -1: "apocenters"}[sign]
         if verbose:
             print(f"FindExtremaNearIdxRef  idx_ref={idx_ref}, "
                   f"K_initial={K:5.3f}, "
                   f"p_initial={f_fit.format(*p_initial)}"
                   f", refine_extrema={refine_extrema}")
```

### Comparing `gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingResidualAmplitude.py` & `gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingResidualAmplitude.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingResidualFrequency.py` & `gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingResidualFrequency.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.1/gw_eccentricity/gw_eccentricity.py` & `gw_eccentricity-1.0.2/gw_eccentricity/gw_eccentricity.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 See our paper https://arxiv.org/abs/2302.11257 and
 https://pypi.org/project/gw_eccentricity for more details.
 """
 __copyright__ = "Copyright (C) 2023 Md Arif Shaikh, Vijay Varma, Harald Pfeiffer"
 __email__ = "arifshaikh.astro@gmail.com, vijay.varma392@gmail.com"
 __status__ = "testing"
 __author__ = "Md Arif Shaikh, Vijay Varma, Harald Pfeiffer"
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __license__ = """
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -83,21 +83,21 @@
     To find t_pericenters/t_apocenters, one can look for extrema in different
     waveform data, like omega22(t) or Amp22(t), the amplitude of the (2, 2)
     mode. Pericenters correspond to the local maxima, while apocenters
     correspond to the local minima in the data. The method option
     (described below) lets the user pick which waveform data to use to find
     t_pericenters/t_apocenters.
 
-    Parameters:
+    Parameters
     ----------
-    tref_in:
+    tref_in
         Input reference time at which to measure eccentricity and mean anomaly.
         Can be a single float or an array.
 
-    fref_in:
+    fref_in
         Input reference GW frequency at which to measure the eccentricity and
         mean anomaly. Can be a single float or an array. Only one of
         tref_in/fref_in should be provided.
 
         Given an fref_in, we find the corresponding tref_in such that
         omega22_average(tref_in) = 2 * pi * fref_in. Here, omega22_average(t)
         is a monotonically increasing average frequency obtained from the
@@ -108,16 +108,17 @@
         Eccentricity and mean anomaly measurements are returned on a subset of
         tref_in/fref_in, called tref_out/fref_out, which are described below.
         If dataDict is provided in dimensionless units, tref_in should be in
         units of M and fref_in should be in units of cycles/M. If dataDict is
         provided in MKS units, t_ref should be in seconds and fref_in should be
         in Hz.
 
-    method: str
+    method : str, default: ``Amplitude``
         Which waveform data to use for finding extrema. Options are:
+
         - "Amplitude": Finds extrema of Amp22(t).
         - "Frequency": Finds extrema of omega22(t).
         - "ResidualAmplitude": Finds extrema of resAmp22(t), the residual
           amplitude, obtained by subtracting the Amp22(t) of the quasicircular
           counterpart from the Amp22(t) of the eccentric waveform. The
           quasicircular counterpart is described in the documentation of
           dataDict below.
@@ -127,15 +128,15 @@
           waveform.
         - "AmplitudeFits": Uses Amp22(t) and iteratively subtracts a
           PN-inspired fit of the extrema of Amp22(t) from it, and finds extrema
           of the residual.
         - "FrequencyFits": Uses omega22(t) and iteratively subtracts a
           PN-inspired fit of the extrema of omega22(t) from it, and finds
           extrema of the residual.
-        Default is "Amplitude".
+
         The available list of methods can be also obtained from
         gw_eccentricity.get_available_methods().
         Detailed description of these methods can be found in Sec. III of
         arXiv:2302.11257.
 
         The Amplitude and Frequency methods can struggle for very small
         eccentricities, especially near the merger, as the
@@ -147,52 +148,60 @@
         finding extrema. However, methods that use the frequency for finding
         extrema (Frequency/ResidualFrequency/FrequencyFits) can be more
         sensitive to junk radiation in NR data.
 
         Therefore, the recommended methods are
         ResidualAmplitude/AmplitudeFits/Amplitude
 
-    dataDict:
+    dataDict : dict
         Dictionary containing waveform modes dict, time etc. Should follow the
-        format:
-        dataDict = {"t": time,
-                    "hlm": modeDict,
-                    "t_zeroecc": time,
-                    "hlm_zeroecc": modeDict,
-                   },
+        format::
+
+            dataDict = {"t": time,
+                       "hlm": modeDict,
+                       "t_zeroecc": time,
+                       "hlm_zeroecc": modeDict,
+                       }
+
         "t" and "hlm" are mandatory. "t_zeroecc" and "hlm_zeroecc" are only
         required for ResidualAmplitude and ResidualFrequency methods, but if
         provided, they are used for additional diagnostic plots, which can be
         helpful for all methods. Any other keys in dataDict will be ignored,
         with a warning.
 
         The recognized keys are:
-        - "t": 1d array of times.
+
+        - "t" : 1d array of times.
+
             - Should be uniformly sampled, with a small enough time step so
               that omega22(t) can be accurately computed. We use a 4th-order
               finite difference scheme. In dimensionless units, we recommend a
               time step of dtM = 0.1M to be conservative, but you may be able
               to get away with larger time steps like dtM = 1M. The
               corresponding time step in seconds would be
               dtM * M * lal.MTSUN_SI, where M is the total mass in Solar
               masses.
             - We do not require the waveform peak amplitude to occur at any
               specific time, but tref_in should follow the same convention for
               peak time as "t".
+
         - "hlm": Dictionary of waveform modes associated with "t".
-            - Should have the format:
+            Should have the format::
+
                 modeDict = {(l1, m1): h_{l1, m1},
                             (l2, m2): h_{l2, m2},
                             ...
-                           },
-                where h_{l, m} is a 1d complex array representing the (l, m)
-                waveform mode. Should contain at least the (2, 2) mode, but
-                more modes can be included, as indicated by the ellipsis '...'
-                above.
+                           }
+
+            where h_{l, m} is a 1d complex array representing the (l, m)
+            waveform mode. Should contain at least the (2, 2) mode, but
+            more modes can be included, as indicated by the ellipsis '...'
+            above.
         - "t_zeroecc" and "hlm_zeroecc":
+
             - Same as above, but for the quasicircular counterpart to the
               eccentric waveform. The quasicircular counterpart can be obtained
               by evaluating a waveform model by keeping the rest of the binary
               parameters fixed (same as the ones used to generate "hlm") but
               setting the eccentricity to zero. For NR, if such a quasicircular
               counterpart is not available, we recommend using quasicircular
               models like NRHybSur3dq8 or IMRPhenomT, depending on the mass
@@ -258,14 +267,15 @@
             debugging. When True, look for figures saved as
             `gwecc_{method}_*.pdf`.
             Default is False.
 
         omega22_averaging_method:
             Options for obtaining omega22_average(t) from the instantaneous
             omega22(t).
+
             - "orbit_averaged_omega22": First, orbit averages are obtained at
               each pericenter by averaging omega22(t) over the time from the
               current pericenter to the next one. This average value is
               associated with the time at midpoint between the current and the
               next pericenter. Similarly, orbit averages are computed at
               apocenters.  Finally, a spline interpolant is constructed between
               all of these orbit averages at extrema locations. However, the
@@ -275,14 +285,15 @@
               for details.
             - "mean_of_extrema_interpolants":
               The mean of omega22_pericenters(t) and omega22_apocenters(t) is
               used as a proxy for the average frequency.
             - "omega22_zeroecc": omega22(t) of the quasicircular counterpart
               is used as a proxy for the average frequency. This can only be
               used if "t_zeroecc" and "hlm_zeroecc" are provided in dataDict.
+
             See Sec. IID of arXiv:2302.11257 for a more detailed description of
             "omega22_average".
             Default is "orbit_averaged_omega22".
 
         treat_mid_points_between_pericenters_as_apocenters:
             If True, instead of trying to find apocenter locations by looking
             for local minima in the data, we simply find the midpoints between
@@ -293,28 +304,31 @@
 
         kwargs_for_fits_methods:
             Extra kwargs to be passed to FrequencyFits and AmplitudeFits
             methods. See
             eccDefinitionUsingFrequencyFits.get_default_kwargs_for_fits_methods
             for allowed keys.
 
-    Returns:
-    --------
+    Returns
+    -------
     A dictionary containing the following keys
     tref_out:
         tref_out is the output reference time at which eccentricity and mean
         anomaly are measured.
         tref_out is included in the returned dictionary only when tref_in is
         provided.
         Units of tref_out are the same as that of tref_in.
 
         tref_out is set as
         tref_out = tref_in[tref_in >= tmin & tref_in <= tmax],
-        where tmax = min(t_pericenters[-1], t_apocenters[-1]) and
-              tmin = max(t_pericenters[0], t_apocenters[0]),
+        where::
+
+            tmax = min(t_pericenters[-1], t_apocenters[-1])
+            tmin = max(t_pericenters[0], t_apocenters[0])
+
         As eccentricity measurement relies on the interpolants
         omega22_pericenters(t) and omega22_apocenters(t), the above cutoffs
         ensure that we only compute the eccentricity where both
         omega22_pericenters(t) and omega22_apocenters(t) are within their
         bounds.
 
     fref_out:
```

### Comparing `gw_eccentricity-1.0.1/gw_eccentricity/load_data.py` & `gw_eccentricity-1.0.2/gw_eccentricity/load_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,18 +149,19 @@
         sub_dict[kw] = super_dict[kw]
     return sub_dict
 
 
 def load_waveform(origin="LAL", **kwargs):
     """Load waveform.
 
-    parameters:
+    Parameters
     ----------
     origin: str
         The origin of the waveform to be generated/loaded. This can be one of
+
         - "LAL": Compute waveform by a call to the LAL-library.
             (see https://lscsoft.docs.ligo.org/lalsuite/lalsimulation/)
         - "SXSCatalog": Import waveform by reading a file in the SXS catalog
             format.
             (see https://data.black-holes.org/waveforms/documentation.html)
         - "LVCNR": Import waveform by reading a file in the LVCNR-data format.
             (see https://arxiv.org/abs/1703.01076)
@@ -171,16 +172,16 @@
         - "EMRI": Import EMRI waveform generated by Maarten.
 
     kwargs:
         Kwargs dictionary to be passed to the waveform loading functions.
         Allowed kwargs depend on origin. Run
         `load_data.get_load_waveform_defaults(origin)` to see
         allowed keys and defaults.
-    Returns:
-    --------
+    Returns
+    -------
     dataDict:
         Dictionary of time, modes etc. For detailed structure of the returned
         dataDict see gw_eccentricity.measure_eccentricity.
     """
     available_origins = get_available_waveform_origins(return_dict=True)
     if origin in available_origins:
         return available_origins[origin](**kwargs)
@@ -298,56 +299,58 @@
                           inclination=0, phi_ref=0., longAscNodes=0,
                           eccentricity=0, meanPerAno=0,
                           alignedSpin=True, lambda1=None, lambda2=None,
                           physicalUnits=False, M=None, D=None):
     """Generate waveform for a given approximant using LALSuite.
 
     Returns dimless time and dimless complex strain.
-    parameters:
+
+    Parameters
     ----------
-    approximant: str
+    approximant : str
         Name of approximant.
-    q: float
+    q : float
         Mass ratio q>=1.
-    chi1: array/list of len=3
+    chi1 : array/list of len=3
         Dimensionless spin vector of larger BH.
-    chi2: array/list of len=3
+    chi2 : array/list of len=3
         Dimensionless spin vector of smaller BH.
-    deltaTOverM: float
+    deltaTOverM : float
         Dimensionless time step size.
-    Momega0: float
+    Momega0 : float
         Dimensionless starting orbital frequency for waveform (rad/s).
-    inclination: float
+    inclination : float
         Inclination angle in radians.
-    phi_ref: float
+    phi_ref : float
         Lalsim stuff.
-    longAscNodes: float
+    longAscNodes : float
         Longiture of Ascending nodes.
-    eccentricity: float
+    eccentricity : float
         Eccentricity.
-    meanPerAno: float
+    meanPerAno : float
         Mean anomaly of periastron.
-    alignedSpin:
+    alignedSpin
         Assume aligned spin approximant.
-    lambda1:
+    lambda1
         Tidal parameter for larger BH.
-    lambda2:
+    lambda2
         Tidal parameter for smaller BH.
-    physicalUnits:
+    physicalUnits
         If True, return in physical units.
-    M:
+    M
         Total mass in units of solar mass. Required when physicalUnits is True.
-    D:
+    D
         Luminosity distance in units of mega parsec. Required when
         physicalUnits is True.
 
-    return:
-    t: array
+    Returns
+    -------
+    t : array
         Dimensionless time.
-    h: complex array
+    h : complex array
         Dimensionless complex strain h_{+} -i*h_{x}.
     """
     chi1 = np.array(chi1)
     chi2 = np.array(chi2)
 
     if alignedSpin:
         if np.sum(np.sqrt(chi1[:2]**2)) > 1e-5 or np.sum(
@@ -521,15 +524,15 @@
     Loading waveform modes from files in lvcnr format require the file
     `SEOBNRv4ROM_v2.0.hdf5` in `LAL_DATA_PATH`. This file can be downloaded
     from
     https://git.ligo.org/lscsoft/lalsuite-extra/-/blob/master/data/lalsimulation/SEOBNRv4ROM_v2.0.hdf5
     and the path can be set using `export
     LAL_DATA_PATH=/path/to/directory/containing/seobnrv4rom_file/`.
 
-    parameters:
+    Parameters
     ----------
     kwargs: Could be the following.
     Run `load_data.get_load_waveform_defaults('LVCNR')` to see allowed
     keys and defaults.
 
     filepath: str
         Path to lvcnr file in format described in arXiv:1703.01076.
@@ -553,15 +556,15 @@
     zero_ecc_approximant: str
         Waveform model to generate zero eccentricity waveform.
 
     num_orbits_to_remove_as_junk: float
         Number of orbits to throw away as junk from the beginning of the NR
         data.
 
-    returns:
+    Returns
     -------
         Dictionary of time and modes dictionary. Optionally the returned
         dictionary includes a dictionary of binary parameters, dictionary of
         zero eccentricity modes etc.
 
     t:
         Time array in dimensionless units. This already discards the first
@@ -704,15 +707,15 @@
     """Load modes from sxs waveform files in sxs catalog format.
 
     This function is intended for loading waveform modes from files in
     the sxs catalog format (see
     https://data.black-holes.org/waveforms/documentation.html).
     For loading lvcnr format files, see `load_lvcnr_waveform`.
 
-    parameters:
+    Parameters
     ----------
     kwargs: Dictionary with the following keys.
     Run `load_data.get_load_waveform_defaults('SXSCatalog')` to see allowed
     keys and defaults.
 
     filepath: str
         Path to waveform file in sxs catalog format. The file should
@@ -764,15 +767,15 @@
     mode_array: 1d array
         1d array of modes to load. Should have the format `[(l1, m1), (l2,
         m2),..]`
 
     extrap_order: int
         Extrapolation order to use for loading the waveform data.
 
-    returns:
+    Returns
     -------
     Returns a dictionary with the following quantities:
     t:
         1d array of times, in dimensionless units, with uniform time
         step `dt`, shifted such t=0 coincides with the peak waveform
         amplitude (obtained using all requested modes in
         mode_array). This already discards the first
@@ -984,24 +987,25 @@
     return {"t_zeroecc": t_zeroecc[start_zeroecc_idx:],
             "hlm_zeroecc": hlm_zeroecc}
 
 
 def reomve_junk_from_nr_data(t, modes_dict, num_orbits_to_remove_as_junk):
     """Remove junk from beginning of NR data.
 
-    Parameters:
+    Parameters
     ----------
     t:
         Time array for the NR data.
     modes_dict:
         Dictionary containing modes array.
     num_orbits_to_remove_as_junk:
         Number of orbits to remove as junk from the begining of NR data.
 
-    Returns:
+    Returns
+    -------
     t_clean:
         Time array corresponding to clean NR data.
     modes_dict_clean:
         modes_dict with `num_orbits_to_remove_as_junk` orbits removed from the
         begining of modes array.
     """
     phase22 = - np.unwrap(np.angle(modes_dict[(2, 2)]))
@@ -1121,15 +1125,15 @@
     or takes too long to load or loads only last few cycles.
 
     This is a simple hack to load the NR files using h5py and then
     interpolate the data. Also we only load 22 modes here for simiplicity.
     This function is mostly for testing measurement of eccentricity
     of NR waveforms.
 
-    parameters:
+    Parameters
     ----------
     kwargs: Could be the followings.
     Run `load_data.get_load_waveform_defaults('LVCNR_hack')` to see allowed
     keys and defaults.
 
     filepath: str
         Path to lvcnr file.
@@ -1144,15 +1148,15 @@
     include_params_dict: bool
         If True, returns a dictionary of binary parameters.
 
     num_orbits_to_remove_as_junk: float
         Number of orbits to throw away as junk from the begining of the NR
         data.
 
-    returns:
+    Returns
     -------
         Dictionary of modes dict, parameter dict and also zero ecc mode dict if
         include_zero_ecc is True.
 
     t:
         Time array.
     hlm:
```

### Comparing `gw_eccentricity-1.0.1/gw_eccentricity/plot_settings.py` & `gw_eccentricity-1.0.2/gw_eccentricity/plot_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 """Fancy settings for plots."""
 from matplotlib import rc
 from cycler import cycler
-from matplotlib import colormaps
+from packaging import version
 
-dark2 = colormaps["Dark2"].colors
+# Getting colormaps in matplotlib has changed from v3.5.0
+import matplotlib
+if version.parse(matplotlib.__version__) < version.parse("3.5.0"):
+    from matplotlib import cm
+    dark2 = cm.get_cmap("Dark2").colors
+else:
+    from matplotlib import colormaps
+    dark2 = colormaps["Dark2"].colors
 
 colorsDict = {
     "default": dark2[1],  # brown
     "apocenter": dark2[3],  # dark2[2],  # purple
     "pericenter": "tab:blue",  # dark2[0],  # turquoise
     "vline": dark2[3],  # pink
     "hline": dark2[5],  # orange
```

### Comparing `gw_eccentricity-1.0.1/gw_eccentricity/truncate_waveform_by_flow.py` & `gw_eccentricity-1.0.2/gw_eccentricity/truncate_waveform_by_flow.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.1/gw_eccentricity/utils.py` & `gw_eccentricity-1.0.2/gw_eccentricity/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 from scipy.interpolate import PchipInterpolator
 import warnings
 
 
 def amplitude_using_all_modes(mode_dict):
     """Get the amplitude using all the available modes.
 
-    Parameters:
+    Parameters
     ----------
     mode_dict:
         Dictionary containing waveform modes.
 
-    Returns:
+    Returns
+    -------
         Square root of the qudrature sum of the amplitudes of all the
         available modes in mode_dict.
     """
     amp = 0
     for mode in mode_dict.keys():
         amp += np.abs(mode_dict[mode])**2
     return np.sqrt(amp)
@@ -27,23 +28,23 @@
 def peak_time_via_quadratic_fit(t, func):
     """
     Find the peak time of a function quadratically.
 
     Fits the function to a quadratic over the 5 points closest to the argmax
     func.
 
-    Parameters:
-    -----------
+    Parameters
+    ----------
     t:
         An array of times.
     func:
         Array of function values.
 
-    Returns:
-    --------
+    Returns
+    -------
     tpeak:
         Time at peak of the function func.
     fpeak:
         Value of function func at tpeak.
     """
     # Find the time closest to the peak, making sure we have room on either
     # side
@@ -66,27 +67,27 @@
 
 def check_kwargs_and_set_defaults(user_kwargs=None,
                                   default_kwargs=None,
                                   name="user given kwargs",
                                   location=None):
     """Sanity check user given dicionary of kwargs and set default values.
 
-    Parameters:
+    Parameters
     ----------
     user_kwargs:
         Dictionary of kwargs by user.
     default_kwargs:
         Dictionary of default kwargs.
     name:
         string to represent the dictionary
     location:
         string pointing to where the defaults are defined
 
-    Returns:
-    --------
+    Returns
+    -------
     updated user_kwargs
     """
     # make user_kwargs iterable
     if user_kwargs is None:
         user_kwargs = {}
 
     for kw in user_kwargs.keys():
@@ -127,23 +128,23 @@
 
 def time_deriv_4thOrder(y, dt):
     """Fourth order accurate time derivative.
 
     Assuming constant time step.
     Tested for convergence up to 1e-12 level.
 
-    Parameters:
-    -----------
+    Parameters
+    ----------
     y:
         1d array to take time derivative of.
     dt:
         Time step.
 
-    Returns:
-    --------
+    Returns
+    -------
     dydt:
         Fourth order time derivative of y.
     """
     # Use a 5 point stencil
     res = 0*y
     # First do the interior
     res[2:-2] = (y[:-4] - 8*y[1:-3] + 8*y[3:-1] - y[4:])/12.
@@ -173,16 +174,16 @@
                 oldY,
                 allowExtrapolation=False,
                 interpolator="spline",
                 spline_kwargs=None,
                 check_kwargs=True):
     """Interpolate.
 
-    Parameters:
-    -----------
+    Parameters
+    ----------
     newX:
         Points where interpolant is to be evaluated.
     oldX:
         1d array of monotonically increasing real values.
     oldY:
         1d array of monotonically increasing real values.
     allowExtrapolation:
@@ -195,16 +196,16 @@
         "monotonic_spline":  Uses scipy.interpolate.PchipInterpolator.
         Default is "spline".
     spline_kwargs:
         See under get_interpolant.
     check_kwargs:
         Check spline_kwargs if check_kwargs is True. Default is True.
 
-    Returns:
-    --------
+    Returns
+    -------
     newY:
         Intepolated values at newX.
     """
     if len(oldY) != len(oldX):
         raise Exception("Lengths dont match.")
 
     if not allowExtrapolation:
@@ -229,16 +230,16 @@
                     oldY,
                     allowExtrapolation=False,
                     interpolator="spline",
                     spline_kwargs=None,
                     check_kwargs=True):
     """Create Interpolant.
 
-    Parameters:
-    -----------
+    Parameters
+    ----------
     oldX:
         1d array of monotonically increasing real values.
     oldY:
         1d array of monotonically increasing real values.
     allowExtrapolation:
         Bool. If True returns extrapolated values. Default is False.
         If False, an exception is raised if trying to extrapolate.
@@ -254,16 +255,16 @@
         spline function scipy.interpolate.InterpolatedUnivariateSpline and the
         defaults are set using gw_eccentricity.utils.get_default_spline_kwargs.
         Since we use allowExtraplotion arg separately, value of "ext" in
         extra_kwargs will be overridden by allowExtrapolation.
     check_kwargs:
         Check spline_kwargs if check_kwargs is True. Default is True.
 
-    Returns:
-    --------
+    Returns
+    -------
     Intepolatnt.
     """
     if not np.all(np.diff(oldX) > 0):
         raise Exception("oldX must have increasing values")
 
     if interpolator == "spline":
         if check_kwargs:
@@ -308,16 +309,16 @@
     return interpolant
 
 
 def debug_message(message, debug_level, important=True,
                   point_to_verbose_output=False):
     """Show message based on debug_level.
 
-    parameters:
-    -----------
+    parameters
+    ----------
     message: str
         Message to display.
 
     debug_level: int
         Indicator for level of debug message. Based on it, one of the
         following actions if performed:
         -1: No action is performed and hence no message is displayed.
```

### Comparing `gw_eccentricity-1.0.1/gw_eccentricity.egg-info/SOURCES.txt` & `gw_eccentricity-1.0.2/gw_eccentricity.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+LICENSE
 README.md
 setup.py
 gw_eccentricity/__init__.py
 gw_eccentricity/compare_methods.py
 gw_eccentricity/eccDefinition.py
 gw_eccentricity/eccDefinitionUsingAmplitude.py
 gw_eccentricity/eccDefinitionUsingAmplitudeFits.py
 gw_eccentricity/eccDefinitionUsingFrequency.py
 gw_eccentricity/eccDefinitionUsingFrequencyFits.py
 gw_eccentricity/eccDefinitionUsingResidualAmplitude.py
 gw_eccentricity/eccDefinitionUsingResidualFrequency.py
-gw_eccentricity/group_nr_waveforms.py
 gw_eccentricity/gw_eccentricity.py
 gw_eccentricity/load_data.py
 gw_eccentricity/plot_settings.py
 gw_eccentricity/truncate_waveform_by_flow.py
 gw_eccentricity/utils.py
 gw_eccentricity.egg-info/PKG-INFO
 gw_eccentricity.egg-info/SOURCES.txt
```

### Comparing `gw_eccentricity-1.0.1/setup.py` & `gw_eccentricity-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.1/test/test_example_notebooks.py` & `gw_eccentricity-1.0.2/test/test_example_notebooks.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.1/test/test_interface.py` & `gw_eccentricity-1.0.2/test/test_interface.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.1/test/test_mks_vs_dimless_units.py` & `gw_eccentricity-1.0.2/test/test_mks_vs_dimless_units.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,25 +120,25 @@
             np.unwrap(meanano_ref),
             np.unwrap(meanano_ref_MKS),
             err_msg=("Mean anomaly at dimensionless and MKS array of"
                      " times are different.\n"
                      "x = Dimensionless, y = MKS"))
 
         # Try evaluating at single dimensionless frequency
-        fref_in = gwecc_object.compute_orbit_averaged_omega22_at_extrema(
+        fref_in = gwecc_object.compute_orbit_averaged_omega22_between_extrema(
             dataDict["t"][idx]) / (2 * np.pi)
         gwecc_dict = measure_eccentricity(
             fref_in=fref_in,
             method=method,
             dataDict=dataDict)
         fref_out = gwecc_dict["fref_out"]
         ecc_ref = gwecc_dict["eccentricity"]
         meanano_ref = gwecc_dict["mean_anomaly"]
         # Try evaluating at single MKS frequency
-        fref_in = gwecc_object_MKS.compute_orbit_averaged_omega22_at_extrema(
+        fref_in = gwecc_object_MKS.compute_orbit_averaged_omega22_between_extrema(
             dataDictMKS["t"][idx]) / (2 * np.pi)
         gwecc_dict_MKS = measure_eccentricity(
             fref_in=fref_in,
             method=method,
             dataDict=dataDictMKS)
         fref_out_MKS = gwecc_dict_MKS["fref_out"]
         ecc_ref_MKS = gwecc_dict_MKS["eccentricity"]
@@ -161,25 +161,25 @@
             [meanano_ref],
             [meanano_ref_MKS],
             err_msg=("Mean anomaly at a single dimensionless and MKS"
                      " frequency gives different results.\n"
                      "x = Dimensionless, y = MKS"))
 
         # Try evaluating at an array of dimensionless frequencies
-        fref_in = gwecc_object.compute_orbit_averaged_omega22_at_extrema(
+        fref_in = gwecc_object.compute_orbit_averaged_omega22_between_extrema(
             dataDict["t"][idx: idx+500]) / (2 * np.pi)
         gwecc_dict = measure_eccentricity(
             fref_in=fref_in,
             method=method,
             dataDict=dataDict)
         fref_out = gwecc_dict["fref_out"]
         ecc_ref = gwecc_dict["eccentricity"]
         meanano_ref = gwecc_dict["mean_anomaly"]
         # Try evaluating at an array of MKS frequencies
-        fref_in = gwecc_object_MKS.compute_orbit_averaged_omega22_at_extrema(
+        fref_in = gwecc_object_MKS.compute_orbit_averaged_omega22_between_extrema(
             dataDictMKS["t"][idx: idx+500]) / (2 * np.pi)
         gwecc_dict_MKS = measure_eccentricity(
             fref_in=fref_in,
             method=method,
             dataDict=dataDictMKS)
         fref_out_MKS = gwecc_dict_MKS["fref_out"]
         ecc_ref_MKS = gwecc_dict_MKS["eccentricity"]
```

### Comparing `gw_eccentricity-1.0.1/test/test_regression.py` & `gw_eccentricity-1.0.2/test/test_regression.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.1/test/test_time_convention.py` & `gw_eccentricity-1.0.2/test/test_time_convention.py`

 * *Files identical despite different names*

