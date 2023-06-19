# Comparing `tmp/cfr-0.5.3.tar.gz` & `tmp/cfr-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-0.5.3.tar", last modified: Mon May 29 23:40:25 2023, max compression
+gzip compressed data, was "cfr-0.6.0.tar", last modified: Mon Jun 19 02:43:55 2023, max compression
```

## Comparing `cfr-0.5.3.tar` & `cfr-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 23:40:25.535761 cfr-0.5.3/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-0.5.3/LICENSE
--rw-r--r--   0 fengzhu    (502) staff       (20)     1771 2023-05-29 23:40:25.535558 cfr-0.5.3/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)     1207 2023-05-29 21:16:00.000000 cfr-0.5.3/README.md
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 23:40:25.524985 cfr-0.5.3/bin/
--rw-r--r--   0 fengzhu    (502) staff       (20)     3905 2022-07-04 04:11:55.000000 cfr-0.5.3/bin/cfr
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 23:40:25.530969 cfr-0.5.3/cfr/
--rw-r--r--   0 fengzhu    (502) staff       (20)      640 2023-03-24 23:03:50.000000 cfr-0.5.3/cfr/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-0.5.3/cfr/climate.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 23:40:25.534929 cfr-0.5.3/cfr/da/
--rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-0.5.3/cfr/da/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-0.5.3/cfr/da/enkf.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-0.5.3/cfr/gcm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-0.5.3/cfr/ml.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    63265 2023-05-29 21:16:00.000000 cfr-0.5.3/cfr/proxy.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    44993 2023-05-29 21:16:00.000000 cfr-0.5.3/cfr/psm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    49995 2023-05-29 21:16:00.000000 cfr-0.5.3/cfr/reconjob.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     2311 2023-03-27 02:39:30.000000 cfr-0.5.3/cfr/reconres.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-05-29 21:16:00.000000 cfr-0.5.3/cfr/ts.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    26581 2023-05-29 21:16:00.000000 cfr-0.5.3/cfr/utils.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    54810 2023-04-17 19:25:37.000000 cfr-0.5.3/cfr/visual.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 23:40:25.534067 cfr-0.5.3/cfr.egg-info/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1771 2023-05-29 23:40:25.000000 cfr-0.5.3/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-05-29 23:40:25.000000 cfr-0.5.3/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-05-29 23:40:25.000000 cfr-0.5.3/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-0.5.3/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu    (502) staff       (20)      203 2023-05-29 23:40:25.000000 cfr-0.5.3/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-05-29 23:40:25.000000 cfr-0.5.3/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-05-29 23:40:25.535820 cfr-0.5.3/setup.cfg
--rw-r--r--   0 fengzhu    (502) staff       (20)     1414 2023-05-29 23:40:02.000000 cfr-0.5.3/setup.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-19 02:43:55.064572 cfr-0.6.0/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-0.6.0/LICENSE
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-19 02:43:55.064401 cfr-0.6.0/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1207 2023-05-29 21:16:00.000000 cfr-0.6.0/README.md
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-19 02:43:55.056204 cfr-0.6.0/bin/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     5163 2023-06-19 02:34:42.000000 cfr-0.6.0/bin/cfr
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-19 02:43:55.060887 cfr-0.6.0/cfr/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      640 2023-03-24 23:03:50.000000 cfr-0.6.0/cfr/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-0.6.0/cfr/climate.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-19 02:43:55.064046 cfr-0.6.0/cfr/da/
+-rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-0.6.0/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-0.6.0/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-0.6.0/cfr/gcm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-0.6.0/cfr/ml.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    63286 2023-06-17 21:42:44.000000 cfr-0.6.0/cfr/proxy.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    44993 2023-05-29 21:16:00.000000 cfr-0.6.0/cfr/psm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    54926 2023-06-19 02:39:39.000000 cfr-0.6.0/cfr/reconjob.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     2311 2023-03-27 02:39:30.000000 cfr-0.6.0/cfr/reconres.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-05-29 21:16:00.000000 cfr-0.6.0/cfr/ts.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    26581 2023-05-29 21:16:00.000000 cfr-0.6.0/cfr/utils.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    54810 2023-04-17 19:25:37.000000 cfr-0.6.0/cfr/visual.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-19 02:43:55.063376 cfr-0.6.0/cfr.egg-info/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-19 02:43:55.000000 cfr-0.6.0/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-06-19 02:43:55.000000 cfr-0.6.0/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-19 02:43:55.000000 cfr-0.6.0/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-0.6.0/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu    (502) staff       (20)      203 2023-06-19 02:43:55.000000 cfr-0.6.0/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-06-19 02:43:55.000000 cfr-0.6.0/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-19 02:43:55.064622 cfr-0.6.0/setup.cfg
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1413 2023-06-17 21:43:24.000000 cfr-0.6.0/setup.py
```

### Comparing `cfr-0.5.3/LICENSE` & `cfr-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-0.5.3/PKG-INFO` & `cfr-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.5.3
-Summary: cfr: the Python package for Climate Field Reconstruction
+Version: 0.6.0
+Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
-Keywords: paleocliamte reconstruction
+Keywords: climate field reconstruction
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: psm
 Provides-Extra: ml
 Provides-Extra: graphem
```

### Comparing `cfr-0.5.3/README.md` & `cfr-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cfr-0.5.3/cfr/__init__.py` & `cfr-0.6.0/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.3/cfr/climate.py` & `cfr-0.6.0/cfr/climate.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.3/cfr/da/enkf.py` & `cfr-0.6.0/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.3/cfr/gcm.py` & `cfr-0.6.0/cfr/gcm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.3/cfr/ml.py` & `cfr-0.6.0/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.3/cfr/proxy.py` & `cfr-0.6.0/cfr/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1043,19 +1043,19 @@
         new.refresh()
         return new
 
     def filter(self, by, keys, mode='fuzzy'):
         ''' Filter the proxy database according to given ptype list.
 
         Args:
-            by (str): filter by a keyword {'ptype', 'pid', 'lat', 'lon', 'loc', 'tag'}
+            by (str): filter by a keyword {'ptype', 'pid', 'dt', 'lat', 'lon', 'loc', 'tag'}
             keys (set): a set of keywords
 
                 * For `by = 'ptype' or 'pid'`, keys take a fuzzy match
-                * For `by = 'lat' or 'lon'`, keys = (lat_min, lat_max) or (lon_min, lon_max)
+                * For `by = 'dt' or 'lat' or 'lon'`, keys = (min, max)
                 * For `by = 'loc-squre'`, keys = (lat_min, lat_max, lon_min, lon_max)
                 * For `by = 'loc-circle'`, keys = (center_lat, center_lon, distance)
                 * For `by = 'tag'`, keys should be a list of tags
 
             mode (str): 'fuzzy' or 'exact' search when `by = 'ptype' or 'pid'`
 
         '''
@@ -1063,29 +1063,30 @@
 
         new_db = ProxyDatabase()
         pobjs = []
         for pid, pobj in self.records.items():
             target = {
                 'ptype': pobj.ptype,
                 'pid': pobj.pid,
+                'dt': pobj.dt,
                 'lat': pobj.lat,
                 'lon': pobj.lon,
                 'loc-square': (pobj.lat, pobj.lon),
                 'loc-circle': (pobj.lat, pobj.lon),
                 'tag': pobj.tags,
             }
             if by in ['ptype', 'pid']:
                 for key in keys:
                     if mode == 'fuzzy':
                         if key in target[by]:
                             pobjs.append(pobj)
                     elif mode == 'exact':
                         if key == target[by]:
                             pobjs.append(pobj)
-            elif by in ['lat', 'lon']:
+            elif by in ['dt', 'lat', 'lon']:
                 if target[by] >= keys[0] and target[by] <= keys[-1]:
                     pobjs.append(pobj)
             elif by == 'loc-square':
                 plat, plon = target[by]
                 if plat >= keys[0] and plat <= keys[1] and plon >= keys[2] and plon <= keys[3]:
                     pobjs.append(pobj)
             elif by == 'loc-circle':
```

### Comparing `cfr-0.5.3/cfr/psm.py` & `cfr-0.6.0/cfr/psm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.3/cfr/reconjob.py` & `cfr-0.6.0/cfr/reconjob.py`

 * *Files 8% similar despite different names*

```diff
@@ -153,14 +153,16 @@
 
         Args:
             inplace (bool): if True, the annualized proxy database will replace the current `self.proxydb`.
             verbose (bool, optional): print verbose information. Defaults to False.
         
         See :py:mod:`cfr.proxy.ProxyDatabase.filter()` for more information.
         '''
+        args = self.io_cfg('filter_proxydb_args', list(args), verbose=verbose)
+        kwargs = self.io_cfg('filter_proxydb_kwargs', kwargs, verbose=verbose)
         if inplace:
             self.proxydb = self.proxydb.filter(*args, **kwargs)
 
             if verbose:
                 p_success(f'>>> {self.proxydb.nrec} records remaining')
                 p_success(f'>>> job.proxydb updated')
 
@@ -287,15 +289,15 @@
             time_name (str): the name of the time dimension in the climate data files.
             load (bool): if True, the data will be loaded into the memory instead of lazy-loading.
             lon_name (str): the name of the longitude dimension in the climate data files.
             verbose (bool, optional): print verbose information. Defaults to False.
         '''
         path_dict = self.io_cfg(f'{tag}_path', path_dict, verbose=verbose)
         if rename_dict is not None: rename_dict = self.io_cfg(f'{tag}_rename_dict', rename_dict, verbose=verbose)
-        anom_period = self.io_cfg(f'{tag}_anom_period', anom_period, verbose=verbose)
+        anom_period = self.io_cfg(f'{tag}_anom_period', list(anom_period), verbose=verbose)
         lat_name = self.io_cfg(f'{tag}_lat_name', lat_name, default='lat', verbose=verbose)
         lon_name = self.io_cfg(f'{tag}_lon_name', lon_name, default='lon', verbose=verbose)
         time_name = self.io_cfg(f'{tag}_time_name', time_name, default='time', verbose=verbose)
 
         self.__dict__[tag] = {}
         for vn, path in path_dict.items():
             if rename_dict is None:
@@ -380,18 +382,18 @@
             tag (str): the tag to denote identity; either 'prior' or 'obs.
             lat_min (float): the minimum latitude of the cropped grid.
             lat_max (float): the maximum latitude of the cropped grid.
             lon_min (float): the minimum longitude of the cropped grid.
             lon_max (float): the maximum longitude of the cropped grid.
             verbose (bool, optional): print verbose information. Defaults to False.
         '''
-        lat_min = self.io_cfg(f'prior_lat_min', lat_min, default=-90, verbose=verbose)
-        lat_max = self.io_cfg(f'prior_lat_max', lat_max, default=90, verbose=verbose)
-        lon_min = self.io_cfg(f'prior_lon_min', lon_min, default=0, verbose=verbose)
-        lon_max = self.io_cfg(f'prior_lon_max', lon_max, default=360, verbose=verbose)
+        lat_min = self.io_cfg(f'{tag}_lat_min', lat_min, default=-90, verbose=verbose)
+        lat_max = self.io_cfg(f'{tag}_lat_max', lat_max, default=90, verbose=verbose)
+        lon_min = self.io_cfg(f'{tag}_lon_min', lon_min, default=0, verbose=verbose)
+        lon_max = self.io_cfg(f'{tag}_lon_max', lon_max, default=360, verbose=verbose)
 
         for vn, fd in self.__dict__[tag].items():
             if verbose: p_header(f'>>> Processing {vn} ...')
             self.__dict__[tag][vn] = fd.crop(lat_min=lat_min, lat_max=lat_max, lon_min=lon_min, lon_max=lon_max)
         
         
     def calib_psms(self, ptype_psm_dict=None, ptype_season_dict=None, calib_period=None,
@@ -529,15 +531,15 @@
         self.recon_fields = self.da_solver.recon_fields
         if verbose: p_success(f'>>> job.recon_fields created')
 
     def run_da_mc(self, recon_period=None, recon_loc_rad=None, recon_timescale=None, nens=None,
                output_full_ens=None, recon_sampling_mode=None, recon_sampling_dist=None, recon_vars=None,
                normal_sampling_sigma=None, normal_sampling_cutoff_factor=None, trim_prior=None,
                recon_seeds=None, assim_frac=None, save_dirpath=None, compress_params=None,
-               allownan=None, verbose=False):
+               allownan=None, output_indices=None, verbose=False):
         ''' Run the Monte-Carlo iterations of data assimilation workflows.
 
         Args:
             recon_period (tuple or list): the time period for reconstruction.
             recon_loc_rad (float): the localization radius; unit: km.
             recon_timescale (int or float): the timescale for reconstruction.
             recon_sampling_mode (str): 'fixed' or 'rolling' window for prior sampling.
@@ -563,14 +565,15 @@
         nens = self.io_cfg('nens', nens, default=100, verbose=verbose)
         recon_seeds = self.io_cfg('recon_seeds', recon_seeds, default=np.arange(0, 20), verbose=verbose)
         assim_frac = self.io_cfg('assim_frac', assim_frac, default=0.75, verbose=verbose)
         save_dirpath = self.io_cfg('save_dirpath', save_dirpath, verbose=verbose)
         os.makedirs(save_dirpath, exist_ok=True)
         compress_params = self.io_cfg('compress_params', compress_params, default={'zlib': True}, verbose=verbose)
         output_full_ens = self.io_cfg('output_full_ens', output_full_ens, default=False, verbose=verbose)
+        output_indices = self.io_cfg('output_indices', output_indices, default=['gm', 'nhm', 'shm', 'nino3.4'], verbose=False)
         recon_sampling_mode = self.io_cfg('recon_sampling_mode', recon_sampling_mode, default='fixed', verbose=verbose)
         trim_prior = self.io_cfg('trim_prior', trim_prior, default=True, verbose=verbose)
         allownan = self.io_cfg('allownan', allownan, default=False, verbose=verbose)
         if recon_sampling_mode == 'rolling':
             normal_sampling_sigma = self.io_cfg('normal_sampling_sigma', normal_sampling_sigma, verbose=verbose)
             normal_sampling_cutoff_factor = self.io_cfg('normal_sampling_cutoff_factor', normal_sampling_cutoff_factor, default=3, verbose=verbose)
             recon_sampling_dist = self.io_cfg('recon_sampling_dist', recon_sampling_dist, default='normal', verbose=verbose)
@@ -586,15 +589,15 @@
                         normal_sampling_sigma=normal_sampling_sigma,
                         normal_sampling_cutoff_factor=normal_sampling_cutoff_factor,
                         recon_timescale=recon_timescale, seed=seed,
                         allownan=allownan, verbose=False)
 
             recon_savepath = os.path.join(save_dirpath, f'job_r{seed:02d}_recon.nc')
             self.save_recon(recon_savepath, compress_params=compress_params, mark_assim_pids=True,
-                            verbose=verbose, output_full_ens=output_full_ens, grid='prior')
+                            verbose=verbose, output_full_ens=output_full_ens, grid='prior', output_indices=output_indices)
 
         t_e = time.time()
         t_used = t_e - t_s
         p_success(f'>>> DONE! Total time spent: {t_used/60:.2f} mins.')
 
 
     def save(self, save_dirpath=None, filename='job.pkl', verbose=False):
@@ -739,15 +742,15 @@
 
         # save to a netCDF file
         ds.to_netcdf(save_path, encoding=encoding_dict)
 
         if verbose: p_success(f'>>> Reconstructed fields saved to: {save_path}')
 
 
-    def prep_da_cfg(self, cfg_path, seeds=None, verbose=False):
+    def prep_da_cfg(self, cfg_path, seeds=None, save_job=False, verbose=False):
         ''' Prepare the configuration items.
 
         Args:
             cfg_path (str): the path of the configuration YAML file.
             seeds (list, optional): the list of random seeds.
             verbose (bool, optional): print verbose information. Defaults to False.
         '''
@@ -763,14 +766,21 @@
         if verbose:
             p_success(f'>>> job.configs loaded')
             pp.pprint(self.configs)
 
         self.load_proxydb(self.configs['proxydb_path'], verbose=verbose)
         if 'pids' in self.configs:
             self.filter_proxydb(by='pid', keys=self.configs['pids'], verbose=verbose)
+        if 'filter_proxydb_args' in self.configs and len(self.configs['filter_proxydb_args'])==2:
+            args = self.configs['filter_proxydb_args']
+            self.filter_proxydb(by=args[0], keys=args[1], verbose=verbose)
+        if 'filter_proxydb_kwargs' in self.configs and len(self.configs['filter_proxydb_kwargs'])==2:
+            kwargs = self.configs['filter_proxydb_kwargs']
+            self.filter_proxydb(by=kwargs['by'], keys=kwargs['keys'], verbose=verbose)
+
         self.annualize_proxydb(
             months=self.configs['annualize_proxydb_months'],
             ptypes=self.configs['annualize_proxydb_ptypes'])
 
         if 'prior_rename_dict' in self.configs:
             prior_rename_dict = self.configs['prior_rename_dict']
         else:
@@ -794,16 +804,24 @@
         if 'prior_annualize_months' in self.configs:
             self.annualize_clim(tag='prior', months=self.configs['prior_annualize_months'], verbose=verbose)
 
         if 'prior_regrid_nlat' in self.configs:
             self.regrid_clim(tag='prior', nlat=self.configs['prior_regrid_nlat'], 
                              nlon=self.configs['prior_regrid_nlon'], verbose=verbose)
 
+        if 'prior_lat_max' in self.configs:
+            self.crop_clim(tag='prior',
+                           lat_min=self.configs['prior_lat_min'], 
+                           lat_max=self.configs['prior_lat_max'], 
+                           lon_min=self.configs['prior_lon_min'], 
+                           lon_max=self.configs['prior_lon_max'], 
+                           verbose=verbose)
+
         self.save_cfg(save_dirpath=self.configs['save_dirpath'], verbose=verbose)
-        self.save(save_dirpath=self.configs['save_dirpath'], verbose=verbose)
+        if save_job: self.save(save_dirpath=self.configs['save_dirpath'], verbose=verbose)
 
         t_e = time.time()
         t_used = t_e - t_s
         p_success(f'>>> DONE! Total time used: {t_used/60:.2f} mins.')
 
     def prep_graphem(self, recon_time=None, calib_time=None,  recon_period=None, recon_timescale=None, calib_period=None, verbose=False):
         ''' A shortcut of the steps for GraphEM data preparation
@@ -815,17 +833,17 @@
                 Effective when `recon_time` or `calib_time` is None. Defaults to None.
             recon_timescale (float, optional): the reconstruction timescale. Defaults to None.
                 Effective when `recon_time` or `calib_time` is None. Defaults to None.
             calib_period (tuple, optional): the calibration timespan. Defaults to None.
             verbose (bool, optional): print verbose information. Defaults to False.
         '''
         if recon_time is None or calib_time is None:
-            recon_period = self.io_cfg('recon_period', recon_period, default=(1001, 2000), verbose=verbose)
+            recon_period = self.io_cfg('recon_period', list(recon_period), default=[1001, 2000], verbose=verbose)
             recon_timescale = self.io_cfg('recon_timescale', recon_timescale, default=1, verbose=verbose)  # unit: yr
-            calib_period = self.io_cfg('calib_period', calib_period, default=(1850, 2000), verbose=verbose)
+            calib_period = self.io_cfg('calib_period', list(calib_period), default=[1850, 2000], verbose=verbose)
 
             recon_time = np.arange(recon_period[0], recon_period[1]+1, recon_timescale)
             calib_time = np.arange(calib_period[0], calib_period[1]+1, recon_timescale)
         else:
             recon_time = self.io_cfg('recon_time', recon_time, verbose=verbose)
             calib_time = self.io_cfg('calib_time', calib_time, verbose=verbose)
 
@@ -956,15 +974,15 @@
         kcv_res = KCV(cv_stats, cutoff_radii=ctrl_params, adjs=adjs)
 
         return kcv_res
 
 
     def run_graphem(self, save_recon=True, save_dirpath=None, save_filename=None,
                     load_precalc_solver=False, solver_save_path=None,
-                    compress_params=None, verbose=False,
+                    compress_params=None, verbose=False, output_indices=None,
                     **fit_kws):
         ''' Run the GraphEM solver, essentially the :py:meth: `GraphEM.solver.GraphEM.fit` method
 
         Note that the arguments for :py:meth: `GraphEM.solver.GraphEM.fit` can be appended in the
         argument list of this function directly. For instance, to pass a pre-calculated graph, use
         `estimate_graph=False` and `graph=g.adj`, where `g` is the :py:`Graph` object.
 
@@ -979,16 +997,21 @@
 
         '''
         compress_params = self.io_cfg('compress_params', compress_params, default={'zlib': True}, verbose=verbose)
 
         if save_recon:
             save_dirpath = self.io_cfg('save_dirpath', save_dirpath, verbose=verbose)
             save_filename = self.io_cfg('save_filename', save_filename, default='job_r01_recon.nc', verbose=verbose)
+            output_indices = self.io_cfg('output_indices', output_indices, default=['gm', 'nhm', 'shm', 'nino3.4'], verbose=False)
             os.makedirs(save_dirpath, exist_ok=True)
 
+        if len(fit_kws) >= 1:
+            for k, v in fit_kws.items():
+                self.io_cfg(k, v, verbose=verbose)
+
         if load_precalc_solver:
             self.graphem_solver = pd.read_pickle(solver_save_path)
             if verbose: p_success(f'job.graphem_solver created with the existing result at: {solver_save_path}')
         else:
             self.graphem_solver = GraphEM()
             fit_kwargs = {
                 'lonlat': self.graphem_params['lonlat'],
@@ -1013,48 +1036,120 @@
         _, nlat, nlon = np.shape(self.obs[vn].da.values)
         self.recon_fields = {}  # to make it multivariable reconstruction ready
         self.recon_fields[vn] = self.graphem_solver.field_r.reshape((nt, nlat, nlon))
         if verbose: p_success(f'>>> job.recon_fields created')
 
         if save_recon:
             recon_savepath = os.path.join(save_dirpath, save_filename)
-            self.save_recon(recon_savepath, compress_params=compress_params, verbose=verbose, grid='obs')
+            self.save_recon(recon_savepath, output_indices=output_indices, compress_params=compress_params, verbose=verbose, grid='obs')
 
 
-def run_da_cfg(cfg_path, seeds=None, run_mc=True, verbose=False):
-    ''' Run the reconstruction job according to a configuration YAML file.
+    def run_da_cfg(self, cfg_path, load_precalculated=False, seeds=None, run_mc=True, verbose=False):
+        ''' Running DA according to a configuration YAML file.
+
+        Args:
+            cfg_path (str): the path of the configuration YAML file.
+            run_mc (bool): if False, the reconstruction part will not executed for the convenience of checking the preparation part.
+            seeds (list, optional): the list of random seeds.
+            verbose (bool, optional): print verbose information. Defaults to False.
+        '''
+        # get job_save_path
+        job = self
+        with open(cfg_path, 'r') as f:
+            job.configs = yaml.safe_load(f)
 
-    Args:
-        cfg_path (str): the path of the configuration YAML file.
-        run_mc (bool): if False, the reconstruction part will not executed for the convenience of checking the preparation part.
-        seeds (list, optional): the list of random seeds.
-        verbose (bool, optional): print verbose information. Defaults to False.
-    '''
-    # get job_save_path
-    job = ReconJob()
-    with open(cfg_path, 'r') as f:
-        job.configs = yaml.safe_load(f)
-
-    job_save_path = os.path.join(job.configs['save_dirpath'], 'job.pkl')
-
-    # load precalculated job.pkl if exists, or prepare the job
-    if os.path.exists(job_save_path):
-        job = pd.read_pickle(job_save_path)
-        p_success(f'>>> {job_save_path} loaded')
-    else:
-        job.prep_da_cfg(cfg_path, seeds=seeds, verbose=verbose)
+        job_save_path = os.path.join(job.configs['save_dirpath'], 'job.pkl')
 
-    if seeds is not None and np.size(seeds) == 1:
-        seeds = [seeds]
-    
-    # run the Monte-Carlo iterations
-    if run_mc:
-        job.run_da_mc(
-            recon_period=job.configs['recon_period'],
-            recon_loc_rad=job.configs['recon_loc_rad'],
-            recon_timescale=job.configs['recon_timescale'],
-            recon_seeds=seeds,
-            assim_frac=job.configs['assim_frac'],
-            compress_params=job.configs['compress_params'],
-            output_full_ens=job.configs['output_full_ens'],
+        # load precalculated job.pkl if exists, or prepare the job
+        if load_precalculated and os.path.exists(job_save_path):
+            job = pd.read_pickle(job_save_path)
+            p_success(f'>>> {job_save_path} loaded')
+        else:
+            job.prep_da_cfg(cfg_path, seeds=seeds, verbose=verbose)
+
+        if seeds is not None and np.size(seeds) == 1:
+            seeds = [seeds]
+
+        # run the Monte-Carlo iterations
+        if run_mc:
+            job.run_da_mc(
+                recon_period=job.configs['recon_period'],
+                recon_loc_rad=job.configs['recon_loc_rad'],
+                recon_timescale=job.configs['recon_timescale'],
+                recon_seeds=seeds,
+                assim_frac=job.configs['assim_frac'],
+                compress_params=job.configs['compress_params'],
+                output_full_ens=job.configs['output_full_ens'],
+                output_indices=job.configs['output_indices'],
+                verbose=verbose,
+            )
+
+    def run_graphem_cfg(self, cfg_path, verbose=False):
+        ''' Running GraphEM according to a configuration YAML file.
+
+        Args:
+            cfg_path (str): the path of the configuration YAML file.
+            verbose (bool, optional): print verbose information. Defaults to False.
+        '''
+        # get job_save_path
+        job = self
+        with open(cfg_path, 'r') as f:
+            job.configs = yaml.safe_load(f)
+
+        job_save_path = os.path.join(job.configs['save_dirpath'], 'job.pkl')
+
+        self.load_proxydb(self.configs['proxydb_path'], verbose=verbose)
+        if 'pids' in self.configs:
+            self.filter_proxydb(by='pid', keys=self.configs['pids'], verbose=verbose)
+        if 'filter_proxydb_args' in self.configs and len(self.configs['filter_proxydb_args'])==2:
+            args = self.configs['filter_proxydb_args']
+            self.filter_proxydb(by=args[0], keys=args[1], verbose=verbose)
+        if 'filter_proxydb_kwargs' in self.configs and len(self.configs['filter_proxydb_kwargs'])==2:
+            kwargs = self.configs['filter_proxydb_kwargs']
+            self.filter_proxydb(by=kwargs['by'], keys=kwargs['keys'], verbose=verbose)
+
+        self.annualize_proxydb(
+            months=self.configs['annualize_proxydb_months'],
+            ptypes=self.configs['annualize_proxydb_ptypes'])
+
+        self.center_proxydb(ref_period=self.configs['proxydb_center_ref_period'])
+
+        if 'obs_rename_dict' in self.configs:
+            obs_rename_dict = self.configs['obs_rename_dict']
+        else:
+            obs_rename_dict = None
+
+        self.load_clim(tag='obs', path_dict=self.configs['obs_path'],
+                       anom_period=self.configs[f'obs_anom_period'],
+                       rename_dict=obs_rename_dict, verbose=verbose)
+
+        if 'obs_annualize_months' in self.configs:
+            self.annualize_clim(tag='obs', months=self.configs['obs_annualize_months'], verbose=verbose)
+
+        if 'obs_regrid_nlat' in self.configs:
+            self.regrid_clim(tag='obs', nlat=self.configs['obs_regrid_nlat'], 
+                             nlon=self.configs['obs_regrid_nlon'], verbose=verbose)
+
+        if 'obs_lat_max' in self.configs:
+            self.crop_clim(tag='obs',
+                           lat_min=self.configs['obs_lat_min'], 
+                           lat_max=self.configs['obs_lat_max'], 
+                           lon_min=self.configs['obs_lon_min'], 
+                           lon_max=self.configs['obs_lon_max'], 
+                           verbose=verbose)
+
+
+        self.prep_graphem(
+            recon_period=self.configs['recon_period'],  # period to reconstruct
+            calib_period=self.configs['calib_period'],  # period for calibration
+            verbose=verbose,
+        )
+
+        self.save_cfg(save_dirpath=self.configs['save_dirpath'], verbose=verbose)
+
+        self.run_graphem(
+            save_dirpath=self.configs['save_dirpath'],
+            graph_method=self.configs['graph_method'],
+            cutoff_radius=self.configs['cutoff_radius'],
+            output_indices=job.configs['output_indices'],
             verbose=verbose,
         )
```

### Comparing `cfr-0.5.3/cfr/reconres.py` & `cfr-0.6.0/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.3/cfr/ts.py` & `cfr-0.6.0/cfr/ts.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.3/cfr/utils.py` & `cfr-0.6.0/cfr/utils.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.3/cfr/visual.py` & `cfr-0.6.0/cfr/visual.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.3/cfr.egg-info/PKG-INFO` & `cfr-0.6.0/cfr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.5.3
-Summary: cfr: the Python package for Climate Field Reconstruction
+Version: 0.6.0
+Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
-Keywords: paleocliamte reconstruction
+Keywords: climate field reconstruction
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: psm
 Provides-Extra: ml
 Provides-Extra: graphem
```

### Comparing `cfr-0.5.3/setup.py` & `cfr-0.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='0.5.3',
-    description='cfr: the Python package for Climate Field Reconstruction',
+    version='0.6.0',
+    description='cfr: a Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
     include_package_data=True,
     license='BSD 3-Clause',
     zip_safe=False,
-    keywords='paleocliamte reconstruction',
+    keywords='climate field reconstruction',
     scripts=['bin/cfr'],
     classifiers=[
         'Natural Language :: English',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     install_requires=[
```

