# Comparing `tmp/domino-composite-0.262.tar.gz` & `tmp/domino-composite-0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-composite-0.262.tar", last modified: Wed Apr 12 15:41:44 2023, max compression
+gzip compressed data, was "domino-composite-0.27.tar", last modified: Mon Jun 19 15:39:14 2023, max compression
```

## Comparing `domino-composite-0.262.tar` & `domino-composite-0.27.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-04-12 15:41:44.497071 domino-composite-0.262/
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1213 2023-04-12 15:41:44.497071 domino-composite-0.262/PKG-INFO
-drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-04-12 15:41:44.497071 domino-composite-0.262/domino/
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2022-11-23 14:01:08.000000 domino-composite-0.262/domino/__init__.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      444 2022-11-23 14:10:19.000000 domino-composite-0.262/domino/agg.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     2702 2022-11-23 14:10:17.000000 domino-composite-0.262/domino/categorical_analysis.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    50813 2023-03-31 15:44:13.000000 domino-composite-0.262/domino/core.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4248 2023-01-30 10:05:05.000000 domino-composite-0.262/domino/deseasonaliser.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     3667 2023-03-31 11:02:48.000000 domino-composite-0.262/domino/filtering.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4784 2023-04-03 16:12:11.000000 domino-composite-0.262/domino/plsr.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    13677 2023-04-04 09:10:15.000000 domino-composite-0.262/domino/prediction.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     5671 2023-04-12 15:41:15.000000 domino-composite-0.262/domino/util.py
-drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-04-12 15:41:44.497071 domino-composite-0.262/domino_composite.egg-info/
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1213 2023-04-12 15:41:44.000000 domino-composite-0.262/domino_composite.egg-info/PKG-INFO
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      382 2023-04-12 15:41:44.000000 domino-composite-0.262/domino_composite.egg-info/SOURCES.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        1 2023-04-12 15:41:44.000000 domino-composite-0.262/domino_composite.egg-info/dependency_links.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2023-04-12 15:41:44.000000 domino-composite-0.262/domino_composite.egg-info/requires.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        7 2023-04-12 15:41:44.000000 domino-composite-0.262/domino_composite.egg-info/top_level.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       38 2023-04-12 15:41:44.497071 domino-composite-0.262/setup.cfg
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      728 2023-04-12 15:41:24.000000 domino-composite-0.262/setup.py
+drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:39:14.273861 domino-composite-0.27/
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1212 2023-06-19 15:39:14.273861 domino-composite-0.27/PKG-INFO
+drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:39:14.273861 domino-composite-0.27/domino/
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2022-11-23 14:01:08.000000 domino-composite-0.27/domino/__init__.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1034 2023-06-19 15:18:52.000000 domino-composite-0.27/domino/agg.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     2702 2022-11-23 14:10:17.000000 domino-composite-0.27/domino/categorical_analysis.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    50731 2023-06-19 15:18:52.000000 domino-composite-0.27/domino/core.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4248 2023-01-30 10:05:05.000000 domino-composite-0.27/domino/deseasonaliser.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     3810 2023-06-19 15:18:52.000000 domino-composite-0.27/domino/filtering.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4784 2023-04-03 16:12:11.000000 domino-composite-0.27/domino/plsr.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    14070 2023-04-12 16:04:19.000000 domino-composite-0.27/domino/prediction.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     5814 2023-06-19 15:18:52.000000 domino-composite-0.27/domino/util.py
+drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:39:14.273861 domino-composite-0.27/domino_composite.egg-info/
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1212 2023-06-19 15:39:14.000000 domino-composite-0.27/domino_composite.egg-info/PKG-INFO
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      382 2023-06-19 15:39:14.000000 domino-composite-0.27/domino_composite.egg-info/SOURCES.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        1 2023-06-19 15:39:14.000000 domino-composite-0.27/domino_composite.egg-info/dependency_links.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2023-06-19 15:39:14.000000 domino-composite-0.27/domino_composite.egg-info/requires.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        7 2023-06-19 15:39:14.000000 domino-composite-0.27/domino_composite.egg-info/top_level.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       38 2023-06-19 15:39:14.273861 domino-composite-0.27/setup.cfg
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      727 2023-06-19 15:39:03.000000 domino-composite-0.27/setup.py
```

### Comparing `domino-composite-0.262/PKG-INFO` & `domino-composite-0.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-composite
-Version: 0.262
+Version: 0.27
 Summary: A package for compositing atmospheric datasets
 Home-page: https://github.com/joshdorrington/domino
 Author: Josh Dorrington
 Author-email: joshua.dorrington@kit.edu
 License: bsd-3-clause
 Description-Content-Type: text/markdown
```

### Comparing `domino-composite-0.262/domino/categorical_analysis.py` & `domino-composite-0.27/domino/categorical_analysis.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.262/domino/core.py` & `domino-composite-0.27/domino/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from domino import agg
 from domino.categorical_analysis import get_transmat, synthetic_states_from_transmat
 from domino.util import holm_bonferroni_correction, split_to_contiguous, is_time_type, make_all_dims_coords, drop_scalar_coords, squeeze_da,offset_time_dim
 from domino.filtering import ds_large_regions, convolve_pad_ds
 from domino.deseasonaliser import Agg_Deseasonaliser
 
-
 class LaggedAnalyser(object):
     """Computes lagged composites of variables with respect to a categorical categorical event series, with support for bootstrap resampling to provide a non-parametric assessment of composite significance, and for deseasonalisation of variables.
     
         **Arguments:**
         
         *event*
             An xarray.DataArray with one dimension taking on categorical values, each defining a class of event (or non-event).
@@ -150,19 +149,17 @@
             return
         if (offset in self._lagged_variables)&(not overwrite):
             raise(KeyError(f'Key "{offset}" is already in lagged_variables.'))
             
         #We are really paranoid about mixing up our lags. So we implement this safety check
         self._check_offset_is_valid(offset,mode)
         
-        #The meat of the function:  BREAKING CHANGE WITH RESPECT TO PREVIOUS VERSION
-        time_offset=durel.relativedelta(**{offset_unit:offset})
-        new_dim=pd.to_datetime(self.variables[offset_dim]).map(lambda t: t- time_offset) #THIS USED TO BE +time_offset
-        self._lagged_variables[offset]=self.variables.copy(deep=False)
-        self._lagged_variables[offset][offset_dim]=new_dim
+        #REPLACED PREVIOUS IMPLEMENTATION WITH EQUIVALENT UTIL IMPORT.
+        self._lagged_variables[offset]=offset_time_dim(self.variables,-offset,offset_unit=offset_unit,offset_dim=offset_dim)
+
         return
     
     #For coords not in a time format
     def _ilag_variables(self,offset,*args,overwrite=False):
         raise(NotImplementedError('Only lagging along timelike dimensions is currently supported.'))
         
     def lag_variables(self,offsets,offset_unit='days',offset_dim='time',mode='any',overwrite=False):
@@ -648,37 +645,41 @@
         lags=np.unique([0,*list(self._lagged_variables)])
         
         mean_states={}
         for var in variable_list:
             dsnlsr=self.deseasonalisers_[var]
             agg=dsnlsr.agg
             mean_states[var]=xr.concat([\
-                             xr.concat([\
-                                    self.deseasonalisers_[var].cycle_coeffs.sel(\
-                                    {agg:getattr(pd.to_datetime(t).map(\
-                                        lambda ti: ti+durel.relativedelta(**{self.offset_unit:int(l)})),agg)}\
-                                    ).mean(agg).assign_coords({'lag':l,'index_val':i})\
-                            for l in lags],'lag')\
+                                 xr.concat([\
+                                    self._lag_average_cycle(dsnlsr,agg,l,t,i)\
+                                for l in lags],'lag')\
                             for i,t in ts.items()],'index_val')
             
         return xr.Dataset(mean_states)
         
-
+    def _lag_average_cycle(self,dsnlsr,agg,l,t,i):
+        
+        dt=durel.relativedelta(**{self.offset_unit:int(l)})
+        tvals=pd.to_datetime([pd.to_datetime(tt)+dt for tt in t.values])
+        cycle_eval=dsnlsr.cycle_coeffs.sel({agg:getattr(tvals,agg)})
+        cycle_mean=cycle_eval.mean(agg).assign_coords({'lag':l,'index_val':i})
+        return cycle_mean
+    
 class PatternFilter(object):
     """Provides filtering methods to refine n-dimensional boolean masks, and apply them to an underlying dataset.
     
         **Optional arguments:**
         *mask_ds*
             An xarray boolean Dataset of arbitrary dimensions which provides the initial mask dataset. If *mask_ds*=None  and *analyser*=None, then *mask_ds* will be initialised as a Dataset of the same dimensions and data_vars as *val_ds*, with all values = 1 (i.e. initially unmasked). 
         
         *val_ds*
             An xarray Dataset with the same dimensions as *mask_ds* if provided, otherwise arbitrary, consisting of an underlying dataset to which the mask is applied. If *val_ds*=None and *analyser*=None, then *PatternFilter.apply_value_mask* will raise an Error
             
         *analyser*
-            An instance of a domino.core.LaggedAnalyser class for which both composites and significance masks have been computed, used to infer the *val_ds* and *mask_ds* arguments respectively. This overrides any values passed explicitly to  *mask_ds* and *val_ds*.
+            An instance of a  core.LaggedAnalyser class for which both composites and significance masks have been computed, used to infer the *val_ds* and *mask_ds* arguments respectively. This overrides any values passed explicitly to  *mask_ds* and *val_ds*.
             
     """
     def __init__(self,mask_ds=None,val_ds=None,analyser=None):
         
         self.mask_ds=mask_ds
         self.val_ds=val_ds
         if analyser is not None:
@@ -791,15 +792,15 @@
         """        
         if area_type=='gridpoint':
             area_based=False
         elif area_type=='spherical':
             area_based=True
         else:
             raise(ValueError(f"Unknown area_type {area_type}. Valid options are 'gridpoint' and 'spherical'"))
-        area_mask=ds_large_regions(self.mask_ds,n,dims=dims,area_based=area_type)
+        area_mask=ds_large_regions(self.mask_ds,n,dims=dims,area_based=area_based)
         self.update_mask(area_mask,mode)
         return
     
     
     def apply_convolution(self,n,dims,mode='replace'):
         """ Apply a square n-point convolution filter to *PatternFilter.mask_ds* in one or two dimensions specified by *dims*, iterated over remaining dimensions. This has the effect of extending the unmasked regions and smoothing the mask overall.
         
@@ -1008,16 +1009,16 @@
         
         self.generated_index=index
         return index
     
     def _add_index_attrs(self,index,sl,mean,std):
         for v in index:
             ix=index[v]
-            ix.attrs['mean']=mean[v]
-            ix.attrs['std']=std[v]
+            ix.attrs['mean']=np.array(mean[v])
+            ix.attrs['std']=np.array(std[v])
             for k,i in sl.items():
                 ix.attrs[k]=i
             index[v]=ix
         return index
     
     def _rename_index_vars(self,index,sl):
         func=self._rename_function
@@ -1027,8 +1028,8 @@
         
         """ Retrieve index means and stds for computed indices, for use as future inputs into index_means or index_stds in *IndexGenerator.Generate*
         """
         if as_dict:
             return self.means,self.stds
         else:
             params=[xr.Dataset(self.means),xr.Dataset(self.stds)]
-            return xr.concat(params,'param').assign_coords({'param':['mean','std']})
+            return xr.concat(params,'param').assign_coords({'param':['mean','std']})
```

### Comparing `domino-composite-0.262/domino/deseasonaliser.py` & `domino-composite-0.27/domino/deseasonaliser.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.262/domino/filtering.py` & `domino-composite-0.27/domino/filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,28 @@
     dtheta=lat1-lat0
     A=r2*np.abs(np.cos(theta))*dtheta*dphi #in km**2
     return A
 
 def grid_area(da,lat_coord='lat',lon_coord='lon',r=6371):
     lat=da[lat_coord].values
     lon=da[lon_coord].values
-    dlon=(lon[1:]-lon[:-1])/2
+    
+    #If coords are descending, we sort that out by
+    #just taking absolute value of the final area
+    dlon=(lon[1:]-lon[:-1])/2 
     dlat=(lat[1:]-lat[:-1])/2
     dlon=[np.median(dlon),*dlon]
     dlat=[np.median(dlat),*dlat]
     areas=np.array([[\
         latlonarea(la-dla,la+dla,lo-dlo,lo+dlo,r=r)\
         for la,dla in zip(lat,dlat)]\
         for lo,dlo in zip(lon,dlon)])
     area=xr.DataArray(data=areas.T,\
-        coords={lat_coord:lat,lon_coord:lon})
-    return area
+        coords={lat_coord:lat,lon_coord:lon},dims=[lat_coord,lon_coord])
+    return np.abs(area)
 
 
 def apply_2d_func_to_da(da,func,*args,dims=None):
     da=da.copy(deep=True)
     da_dim=None    
     if dims is not None:
         #if dims is specified, ignore da's without all dims
@@ -111,8 +114,8 @@
 def convolve_pad_ds(ds,n,dims):
     ds=ds.copy()
     for var in list(ds.data_vars):
         ds[var]=convolve_pad_da(ds[var],n,dims=dims)
     return ds
 
 def std_filter(val_ds,std,frac):
-    return np.abs(val_ds)>=frac*std
+    return np.abs(val_ds)>=frac*std
```

### Comparing `domino-composite-0.262/domino/plsr.py` & `domino-composite-0.27/domino/plsr.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.262/domino/prediction.py` & `domino-composite-0.27/domino/prediction.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     
     *predictors*
     An xarray Dataset of scalar predictors
     
     *predictand*
     An xarray DataArray with a shared coord to *predictors*.
     """
-    def __init__(self,predictors,predictand):
+    def __init__(self,predictors,predictand,tolerate_empty_variables=False):
         
         self.predictand=self._predictand_to_dataarray(predictand)
         self.predictors=self._predictors_to_dataset(predictors)
         
         
         self.predefined_models=dict(
             logregression=log_regression_model
@@ -105,27 +105,37 @@
         )
         
         self.predefined_scores=dict(
             sklearn_roc_auc=ROC_AUC,
             test=blank_score
         )
         self.computed_scores=None
+        
+        self.tol_empty=tolerate_empty_variables
         return
     
     def __repr__(self):
         return 'A PredictionTest object'
     def __str__(self):
         return self.__repr__
     
     def _predictand_to_dataarray(self,predictand):
         return predictand
     
     def _predictors_to_dataset(self,predictors):
         return predictors
     
+    def _handle_potentially_empty_variable_list(self,vlist):
+        if len(vlist)>0:
+            return 0
+        else:
+            if self.tol_empty:
+                return 1
+            raise(ValueError('Empty variable list passed, but tolerate_empty_variables=False was set in PredictionTest.init'))
+
     def categorical_prediction(self,model,score='sklearn_roc_auc',cv_method=None,predictor_variables='univariate',keep_models=False,model_kwargs={},cv_kwargs={},score_kwargs={}):
         
         """
         
         **Arguments**
         
         *model*
```

### Comparing `domino-composite-0.262/domino/util.py` & `domino-composite-0.27/domino/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,20 @@
 
 def offset_time_dim(da,offset,offset_unit='days',offset_dim='time',deep=False):#
     """Shifts the time-like *offset_dim* coord of *da* by *offset* *offset_units*.
     
     e.g. offset_time_dim(da,3,'days'), adds three days to the time axis of da."""
     
     time_offset=dt.timedelta(**{offset_unit:offset})
-    new_dim=pd.to_datetime(da[offset_dim])+time_offset
+    
+    #rewritten to handle older pandas versions that don't play nicely with dataarrays
+    offset_dim_vals=pd.to_datetime(da[offset_dim].values)+time_offset
     new_da=da.copy(deep=deep)
-    new_da[offset_dim]=new_dim
+    new_da=new_da.assign_coords({offset_dim:offset_dim_vals})
+    
     return new_da
 
 
 #Takes a time axis t_arr, and splits it into
 #contiguous subarrays. Alternatively it splits an 
 #axis x_arr into subarrays. If no dt is provided
 #to define contiguous segments, the minimum difference
@@ -146,8 +149,8 @@
     for v in indices.data_vars:
         da=indices[v]
         l=offsets[v]
         if type(l)==np.int_:
             l=int(l) #datetime can't handle np.ints, no idea why not.
         da_arr.append(offset_time_dim(da,-l,offset_unit,offset_dim=dim))
     ds=xr.merge(da_arr)
-    return ds
+    return ds
```

### Comparing `domino-composite-0.262/domino_composite.egg-info/PKG-INFO` & `domino-composite-0.27/domino_composite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-composite
-Version: 0.262
+Version: 0.27
 Summary: A package for compositing atmospheric datasets
 Home-page: https://github.com/joshdorrington/domino
 Author: Josh Dorrington
 Author-email: joshua.dorrington@kit.edu
 License: bsd-3-clause
 Description-Content-Type: text/markdown
```

### Comparing `domino-composite-0.262/setup.py` & `domino-composite-0.27/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("/data/ox5324/Domino/readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='domino-composite',
-    version='0.262',
+    version='0.27',
     author='Josh Dorrington',
     author_email='joshua.dorrington@kit.edu',
     description='A package for compositing atmospheric datasets',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/joshdorrington/domino',
     license='bsd-3-clause',
```

