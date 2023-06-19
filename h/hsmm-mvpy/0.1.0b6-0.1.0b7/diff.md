# Comparing `tmp/hsmm_mvpy-0.1.0b6.tar.gz` & `tmp/hsmm_mvpy-0.1.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsmm_mvpy-0.1.0b6.tar", last modified: Mon Jun 19 16:17:59 2023, max compression
+gzip compressed data, was "hsmm_mvpy-0.1.0b7.tar", last modified: Mon Jun 19 17:13:47 2023, max compression
```

## Comparing `hsmm_mvpy-0.1.0b6.tar` & `hsmm_mvpy-0.1.0b7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 16:17:59.581714 hsmm_mvpy-0.1.0b6/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b6/LICENSE.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 16:17:59.577715 hsmm_mvpy-0.1.0b6/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22740 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b6/README.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      830 2023-06-19 16:17:20.000000 hsmm_mvpy-0.1.0b6/pyproject.toml
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-06-19 16:17:59.581714 hsmm_mvpy-0.1.0b6/setup.cfg
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 16:17:59.577715 hsmm_mvpy-0.1.0b6/src/
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 16:17:59.577715 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      194 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/__init__.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    57323 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/models.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     5735 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/resample.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    11044 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/simulations.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    41525 2023-06-19 16:15:32.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/utils.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22654 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/visu.py
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 16:17:59.577715 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy.egg-info/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 16:17:59.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy.egg-info/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      369 2023-06-19 16:17:59.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy.egg-info/SOURCES.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-06-19 16:17:59.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy.egg-info/dependency_links.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       71 2023-06-19 16:17:59.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy.egg-info/requires.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-06-19 16:17:59.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy.egg-info/top_level.txt
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 17:13:47.768928 hsmm_mvpy-0.1.0b7/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b7/LICENSE.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 17:13:47.768928 hsmm_mvpy-0.1.0b7/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22740 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b7/README.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      830 2023-06-19 17:09:10.000000 hsmm_mvpy-0.1.0b7/pyproject.toml
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-06-19 17:13:47.768928 hsmm_mvpy-0.1.0b7/setup.cfg
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 17:13:47.768928 hsmm_mvpy-0.1.0b7/src/
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 17:13:47.768928 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      194 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/__init__.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    57320 2023-06-19 17:06:18.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/models.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     5735 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/resample.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    11082 2023-06-19 17:02:09.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/simulations.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    41436 2023-06-19 16:49:13.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/utils.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22869 2023-06-19 16:59:30.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/visu.py
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 17:13:47.768928 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy.egg-info/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 17:13:47.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy.egg-info/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      369 2023-06-19 17:13:47.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-06-19 17:13:47.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       71 2023-06-19 17:13:47.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy.egg-info/requires.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-06-19 17:13:47.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy.egg-info/top_level.txt
```

### Comparing `hsmm_mvpy-0.1.0b6/LICENSE.md` & `hsmm_mvpy-0.1.0b7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b6/PKG-INFO` & `hsmm_mvpy-0.1.0b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm_mvpy
-Version: 0.1.0b6
+Version: 0.1.0b7
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
```

### Comparing `hsmm_mvpy-0.1.0b6/README.md` & `hsmm_mvpy-0.1.0b7/README.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b6/pyproject.toml` & `hsmm_mvpy-0.1.0b7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "hsmm_mvpy"
-version = "0.1.0-beta6"
+version = "0.1.0-beta7"
 authors = [
   { name="Gabriel Weindel", email="gabriel.weindel@gmail.com" },
   { name="Leendert van Maanen", email="e@mail.com" },
   { name="Jelmer Borst", email="e@mail.com" },
 ]
 description = "Package for fitting Hidden Semi-Markov Models to electro-encephalographic data"
 readme = "README.md"
```

### Comparing `hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/models.py` & `hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -884,15 +884,15 @@
                 estimates.append(self.EM(1, mags, pars, threshold, magnitudes_to_fix, parameters_to_fix))
         lkhs_sp = np.array([x[0] for x in estimates])
         mags_sp = np.array([x[1] for x in estimates])
         pars_sp = np.array([x[2] for x in estimates])
         eventprobs_sp = np.array([x[3] for x in estimates])
         return lkhs_sp, mags_sp, pars_sp, eventprobs_sp
     
-    def fit(self, step=1, verbose=True, figsize=(12,3), end=None, threshold=None, trace=False):
+    def fit(self, step=1, verbose=True, figsize=(12,3), end=None, threshold=1, trace=False):
         '''
         '''
         if end is None:
             end = self.mean_d
         n_points = int(end//step)
         if threshold is None:
             means = np.array([np.mean(self.events[np.random.choice(range(len(self.events)), self.n_trials),:], axis=0) for x in range(1000)])
```

### Comparing `hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/resample.py` & `hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/resample.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/simulations.py` & `hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/simulations.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,16 @@
     generating_events: ndarray
         Times of the simulated bumps used to test for accurate recovery compared to estimation
     files: list
         list of file names (file + number of subject)
     '''
     if seed is not None:
         random_state = np.random.RandomState(seed)
+    else:
+        random_state = None
     sources = np.array(sources, dtype=object)
     if len(np.shape(sources)) == 2:
         sources = [sources]#If only one subject
     if np.shape(sources)[0] != n_subj:
         raise ValueError('Number of subject is not coherent with the sources provided')
     #Infer max duration of a trial from the specified sources
     percentiles = np.empty(len(sources[0]))
```

### Comparing `hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/utils.py` & `hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,25 +128,25 @@
         if epoched == False:# performs epoching on raw data
             if '.fif' in participant:
                 data = mne.io.read_raw_fif(participant, preload=False, verbose=verbose)
             elif '.bdf' in participant:
                 data = mne.io.read_raw_bdf(participant, preload=False, verbose=verbose)
             else:
                 raise ValueError(f'Unknown EEG file format for participant {participant}')
-            data = _pick_channels(pick_channels,data, stim=True)
             if sfreq is None: 
                 sfreq = data.info['sfreq']
 
             if 'response' not in list(resp_id.keys())[0]:
                 resp_id = {f'response/{k}': v for k, v in resp_id.items()}
             if events_provided is None:
                 try:
                     events = mne.find_events(data, verbose=verbose, min_duration = 1 / data.info['sfreq'])
                 except:
                     events = mne.events_from_annotations(data, verbose=verbose)
+                data = _pick_channels(pick_channels,data, stim=True)
                 if events[0,1] > 0:#bug from some stim channel, should be 0 otherwise indicates offset in the trggers
                     print(f'Correcting event values as trigger channel has offset {np.unique(events[:,1])}')
                     events[:,2] = events[:,2]-events[:,1]#correction on event value                
                 events_values = np.concatenate([np.array([x for x in event_id.values()]), np.array([x for x in resp_id.values()])])
                 events = np.array([list(x) for x in events if x[2] in events_values])#only keeps events with stim or response
                 events_stim = np.array([list(x) for x in events if x[2] in event_id.values()])#only stim
             else:
@@ -206,17 +206,15 @@
                 raise ValueError('Metadata should be a pandas data-frame as generated by mne or be contained in the passed epoch data')
         offset_after_resp_samples = np.rint(offset_after_resp*sfreq).astype(int)
         valid_epoch_index = [x for x,y in enumerate(epochs.drop_log) if len(y) == 0]
         data_epoch = epochs.get_data()#preserves index
         rts = metadata_i[rt_col]
         if isinstance(metadata_i, pd.DataFrame):
             if len(metadata_i) > len(data_epoch):#assumes metadata contains rejected epochs
-                print(True)
-                metadata_i = metadata_i.iloc[valid_epoch_index]
-                metadata_i.reset_index(drop=True, inplace=True)
+                metadata_i = metadata_i.loc[valid_epoch_index]
                 rts = metadata_i[rt_col]
             try:
                 rts = rts/scale
             except:
                 raise ValueError(f'Expected column named {rt_col} in the provided metadata file, alternative names can be passed through the rt_col parameter')
         elif rts is None:
             raise ValueError(f'Expected either a metadata Dataframe or an array of Reaction Times')
```

### Comparing `hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/visu.py` & `hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/visu.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,17 @@
         Whether to plot individual lines
     ax : matplotlib.pyplot.ax
         Matplotlib object on which to draw the plot, can be useful if you want to control specific aspects of the plots
         outside of this function
 
     Returns
     -------
-    ax : matplotlib.pyplot.ax
+    ax : matplotlib.pyplot.aiptions: ['BAD_', 'BAD_breaks']
+(array([[     0,      0,      2],
+       [     0,      0,      2],x
         if ax was specified otherwise returns the plot
     '''
     if pvals:
         if test == 'sign':
             from statsmodels.stats.descriptivestats import sign_test 
         elif test == 't-test':
             from scipy.stats import ttest_1samp
@@ -499,16 +501,18 @@
     if model_to_compare is None: 
         plot_topo_timecourse(maxboot_model.channels_activity.values, maxboot_model.event_times.values, info, init,ax=axes['a'])
         times = maxboot_model.event_times#init.compute_times(init, maxboot_model, mean=True)#computing predicted event times
     else:
         plot_topo_timecourse(epoch_data, model_to_compare, info, init,ax=axes['a'])
         times = init.compute_times(init, model_to_compare, mean=True)
         maxboot_model = model_to_compare
+    counts_adjusted = np.zeros(int(maxboot_model.event.max()+1))
+    counts_adjusted[:len(counts)] = counts
     axes['a'].set_xlabel('Time (samples)')
-    axes['b'].bar(maxboot_model.event+1,counts)
+    axes['b'].bar(maxboot_model.event+1,counts_adjusted)
     axes['b'].set_xlabel('Event number')
     axes['b'].set_xticks(maxboot_model.event+1)
     axes['b'].set_ylabel('Frequency')
     axes['b'].set_ylim(0,1)
     
     axes['c'].bar(label_event_num,event_number)
     axes['c'].set_xlabel('Number of events')
```

### Comparing `hsmm_mvpy-0.1.0b6/src/hsmm_mvpy.egg-info/PKG-INFO` & `hsmm_mvpy-0.1.0b7/src/hsmm_mvpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm-mvpy
-Version: 0.1.0b6
+Version: 0.1.0b7
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
```

