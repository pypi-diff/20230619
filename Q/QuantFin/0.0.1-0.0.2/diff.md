# Comparing `tmp/QuantFin-0.0.1.tar.gz` & `tmp/QuantFin-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantFin-0.0.1.tar", last modified: Mon Jun 19 13:19:37 2023, max compression
+gzip compressed data, was "QuantFin-0.0.2.tar", last modified: Mon Jun 19 15:29:38 2023, max compression
```

## Comparing `QuantFin-0.0.1.tar` & `QuantFin-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-19 13:19:37.467801 QuantFin-0.0.1/
--rwx------   0 stephencheung   (501) staff       (20)     1085 2023-01-27 14:04:52.000000 QuantFin-0.0.1/LICENSE
--rw-r--r--   0 stephencheung   (501) staff       (20)     4268 2023-06-19 13:19:37.468155 QuantFin-0.0.1/PKG-INFO
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-19 13:19:37.460839 QuantFin-0.0.1/QuantFin/
--rwx------   0 stephencheung   (501) staff       (20)      258 2023-06-19 08:40:48.000000 QuantFin-0.0.1/QuantFin/HandleError.py
--rwx------   0 stephencheung   (501) staff       (20)      911 2022-04-18 08:21:26.000000 QuantFin-0.0.1/QuantFin/MarketRisk.py
--rwx------   0 stephencheung   (501) staff       (20)     8086 2023-06-19 11:09:38.000000 QuantFin-0.0.1/QuantFin/Portfolio.py
--rwx------   0 stephencheung   (501) staff       (20)     2835 2023-01-26 18:52:42.000000 QuantFin-0.0.1/QuantFin/Proxy.py
--rwx------   0 stephencheung   (501) staff       (20)    17098 2023-06-19 11:46:44.000000 QuantFin-0.0.1/QuantFin/Regression.py
--rwx------   0 stephencheung   (501) staff       (20)    12285 2023-06-19 12:36:02.000000 QuantFin-0.0.1/QuantFin/ReqData.py
--rwx------   0 stephencheung   (501) staff       (20)      257 2023-06-19 11:48:05.000000 QuantFin-0.0.1/QuantFin/__init__.py
--rwx------   0 stephencheung   (501) staff       (20)     4274 2023-06-19 10:59:09.000000 QuantFin-0.0.1/QuantFin/_deciles.py
--rwx------   0 stephencheung   (501) staff       (20)     4812 2023-06-19 10:56:38.000000 QuantFin-0.0.1/QuantFin/tool.py
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-19 13:19:37.467265 QuantFin-0.0.1/QuantFin.egg-info/
--rw-r--r--   0 stephencheung   (501) staff       (20)     4268 2023-06-19 13:19:37.000000 QuantFin-0.0.1/QuantFin.egg-info/PKG-INFO
--rw-r--r--   0 stephencheung   (501) staff       (20)      384 2023-06-19 13:19:37.000000 QuantFin-0.0.1/QuantFin.egg-info/SOURCES.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)        1 2023-06-19 13:19:37.000000 QuantFin-0.0.1/QuantFin.egg-info/dependency_links.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)       47 2023-06-19 13:19:37.000000 QuantFin-0.0.1/QuantFin.egg-info/requires.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)        9 2023-06-19 13:19:37.000000 QuantFin-0.0.1/QuantFin.egg-info/top_level.txt
--rwx------   0 stephencheung   (501) staff       (20)     3451 2023-06-19 13:17:02.000000 QuantFin-0.0.1/README.md
--rw-r--r--   0 stephencheung   (501) staff       (20)       79 2023-06-19 13:19:37.468806 QuantFin-0.0.1/setup.cfg
--rwx------   0 stephencheung   (501) staff       (20)     1506 2023-06-19 13:14:53.000000 QuantFin-0.0.1/setup.py
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-19 15:29:38.468305 QuantFin-0.0.2/
+-rwx------   0 stephencheung   (501) staff       (20)     1085 2023-01-27 14:04:52.000000 QuantFin-0.0.2/LICENSE
+-rw-r--r--   0 stephencheung   (501) staff       (20)     4235 2023-06-19 15:29:38.469020 QuantFin-0.0.2/PKG-INFO
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-19 15:29:38.402779 QuantFin-0.0.2/QuantFin/
+-rwx------   0 stephencheung   (501) staff       (20)      258 2023-06-19 08:40:48.000000 QuantFin-0.0.2/QuantFin/HandleError.py
+-rwx------   0 stephencheung   (501) staff       (20)      911 2022-04-18 08:21:26.000000 QuantFin-0.0.2/QuantFin/MarketRisk.py
+-rw-r--r--   0 stephencheung   (501) staff       (20)    13350 2023-06-19 15:09:08.000000 QuantFin-0.0.2/QuantFin/PanelRegs.py
+-rwx------   0 stephencheung   (501) staff       (20)     8087 2023-06-19 15:11:23.000000 QuantFin-0.0.2/QuantFin/Portfolio.py
+-rwx------   0 stephencheung   (501) staff       (20)     2835 2023-06-19 15:11:28.000000 QuantFin-0.0.2/QuantFin/Proxy.py
+-rwx------   0 stephencheung   (501) staff       (20)    12285 2023-06-19 12:36:02.000000 QuantFin-0.0.2/QuantFin/ReqData.py
+-rwx------   0 stephencheung   (501) staff       (20)      256 2023-06-19 15:09:41.000000 QuantFin-0.0.2/QuantFin/__init__.py
+-rwx------   0 stephencheung   (501) staff       (20)     4274 2023-06-19 10:59:09.000000 QuantFin-0.0.2/QuantFin/_deciles.py
+-rwx------   0 stephencheung   (501) staff       (20)     2303 2023-06-19 15:02:45.000000 QuantFin-0.0.2/QuantFin/_regression.py
+-rwx------   0 stephencheung   (501) staff       (20)     4812 2023-06-19 10:56:38.000000 QuantFin-0.0.2/QuantFin/tool.py
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-19 15:29:38.467443 QuantFin-0.0.2/QuantFin.egg-info/
+-rw-r--r--   0 stephencheung   (501) staff       (20)     4235 2023-06-19 15:29:37.000000 QuantFin-0.0.2/QuantFin.egg-info/PKG-INFO
+-rw-r--r--   0 stephencheung   (501) staff       (20)      407 2023-06-19 15:29:38.000000 QuantFin-0.0.2/QuantFin.egg-info/SOURCES.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)        1 2023-06-19 15:29:37.000000 QuantFin-0.0.2/QuantFin.egg-info/dependency_links.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)       47 2023-06-19 15:29:37.000000 QuantFin-0.0.2/QuantFin.egg-info/requires.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)        9 2023-06-19 15:29:37.000000 QuantFin-0.0.2/QuantFin.egg-info/top_level.txt
+-rwx------   0 stephencheung   (501) staff       (20)     3418 2023-06-19 15:28:49.000000 QuantFin-0.0.2/README.md
+-rw-r--r--   0 stephencheung   (501) staff       (20)       79 2023-06-19 15:29:38.472461 QuantFin-0.0.2/setup.cfg
+-rwx------   0 stephencheung   (501) staff       (20)     1506 2023-06-19 15:28:14.000000 QuantFin-0.0.2/setup.py
```

### Comparing `QuantFin-0.0.1/LICENSE` & `QuantFin-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.1/PKG-INFO` & `QuantFin-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantFin
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for Academic Research on Asset Pricing
 Home-page: https://github.com/yuz0101/QuantFin
 Download-URL: https://github.com/yuz0101/QuantFin/archive/refs/tags/Test.tar.gz
 Author: Stephen Zhang
 Author-email: stephen_se@outlook.com
 License: MIT
 Keywords: ACADEMIC,EMPIRICAL,FIANCE,RESEARCH,QUANT,PORTFOLIO
@@ -22,15 +22,15 @@
 # QuantFin
 A toolkit for asset pricing.
 Working... ...
 
 ### Install
 
 ```consol
-pip install -i https://test.pypi.org/simple/ QuantFin==0.0.1
+pip install QuantFin==0.0.2
 ```
 
 ### Get started
 
 #### Momentum Effects
 
 1) Calculat momentum value on stocks (MOM)
```

### Comparing `QuantFin-0.0.1/QuantFin/MarketRisk.py` & `QuantFin-0.0.2/QuantFin/MarketRisk.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.1/QuantFin/Portfolio.py` & `QuantFin-0.0.2/QuantFin/Portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from numpy import ones, nan
 from pandas import DataFrame, DatetimeIndex, concat, qcut
 
 from QuantFin._deciles import *
 from QuantFin.HandleError import InputError
-from QuantFin.Regression import OLS
+from QuantFin._regression import OLS
 from QuantFin.ReqData import KenFrenchLib
 
 
 class Performance:
 
     def __init__(self, data: DataFrame, freq: str = 'M', models: list = ['CAPM', 'FF3', 'FF4'],
                  datename: str = 'date'):
```

### Comparing `QuantFin-0.0.1/QuantFin/Proxy.py` & `QuantFin-0.0.2/QuantFin/Proxy.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.1/QuantFin/Regression.py` & `QuantFin-0.0.2/QuantFin/PanelRegs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,348 +1,290 @@
-# -*- coding: utf-8 -*-
-
-import statsmodels.api as sm
-from linearmodels import (FamaMacBeth, PanelOLS)
-from pandas import concat, DataFrame
-from numpy import log, nan
-from QuantFin.HandleError import QueryError
-
-
-class PanelRegs:
-    """
-    The class provides functions for performing regression analysis for panel data with various
-    options, including fixed effects, covariance estimators, and other specifications.
-
-    Special features:
-        1. Customize regression with stata-like string, e.g., 
-             "y ~ 1 + x1 + x2 if 2010<=year<=2020, fe(firmid, year, month), cluster(firmid)"
-             "y ~ 1 + x1 + x2 if 2010<=year<=2020, fe(firmid, year, month), robust"
-             "y ~ 1 + x1 + x2 if 2010<=year<=2020, famamacbeth, robust"
-        2. Return academic-like table summarising statistical results.
-    """
-
-    def _panel_reg(self, formula, data, weights=None, singletons=True, drop_absorbed=False, check_rank=True, use_lsdv=False, use_lsmr=False, low_memory=None, debiased=True, count_effects=True, bandwidth=None, kernel=None):
-        '''This is a Python function that handles panel regression using various fixed effects and
-        covariance estimators.
-        
-        Parameters
-        ----------
-        formula
-            The formula for the regression model in the form of a string, with the dependent variable on
-        the left side of the tilde (~) and the independent variables on the right side separated by plus
-        signs (+).
-        data
-            The data on which the regression is to be performed.
-        weights
-            Weights are used to adjust the contribution of each observation in the regression analysis.
-        They can be used to account for differences in sample sizes or to give more weight to certain
-        observations based on their importance or relevance to the analysis.
-        singletons, optional
-            A boolean indicating whether to include singleton columns in the regression. A singleton column
-        is a column with only one unique value, which does not provide any information for the
-        regression. If set to True, singleton columns will be included in the regression. If set to
-        False, singleton columns will be dropped.
-        drop_absorbed, optional
-            A boolean parameter that determines whether to drop absorbed variables from the regression.
-        Absorbed variables are those that are perfectly collinear with other independent variables in
-        the model. If set to True, the function will drop these variables from the model. If set to
-        False, the function will keep these variables in
-        check_rank, optional
-            A boolean parameter that indicates whether to check the rank of the design matrix before
-        fitting the model. If set to True, the function will raise an error if the rank is deficient.
-        use_lsdv, optional
-            A boolean indicating whether to use least-squares dummy variable (LSDV) estimation. Default is
-        False.
-        use_lsmr, optional
-            A boolean indicating whether to use the LSMR algorithm for solving the least squares problem.
-        Default is False.
-        low_memory
-            A boolean indicating whether to use a lower memory footprint algorithm for fitting the model.
-        If set to True, the algorithm will use less memory but may take longer to run. If set to False,
-        the algorithm will use more memory but may run faster. If set to None, the algorithm will
-        automatically choose
-        debiased, optional
-            A boolean parameter that indicates whether to use a debiased estimator for the covariance
-        matrix. If True, the estimator will be debiased. If False, the estimator will not be debiased.
-        count_effects, optional
-            A boolean parameter that indicates whether to count the number of entity and time effects
-        included in the model. If set to True, the number of entity and time effects will be returned as
-        attributes of the fitted model object.
-        bandwidth
-            The bandwidth parameter is used in kernel-based covariance estimators to determine the size of
-        the kernel window. It specifies the distance over which the kernel function is applied to
-        calculate the weights for each observation. A larger bandwidth will result in a smoother
-        estimate, while a smaller bandwidth will result in a more localized estimate
-        kernel
-            The type of kernel to use for kernel-based covariance estimation. Possible values are
-        'bartlett', 'parzen', and 'qs'.
-        
-        Returns
-        -------
-            either a FamaMacBeth or a PanelOLS object depending on the value of the fama_macbeth variable.
-        
-        '''
-        fama_macbeth = False
-        entity_effects, time_effects, other_effects = False, False, None
-        cov_type, cov_config = 'unadjusted', {}
-
-        # 1 handle formula
-        dep, right = formula.split('~')
-        dep = dep.replace(' ', '')
-        formulas = right.split(',')
-        if ' if ' in formulas[0]:
-            formulas[0], data_query = formulas[0].split(' if ')
-            data.query(data_query, inplace=True)
-            if data.empty:
-                raise QueryError("""Return a empty dataframe after Query""")
-        indeps = formulas[0].replace(' ', '').split('+')
-
-        # 2 handle right-hand variables
-        xvars = []
-        for indep in indeps:
-            if indep.lower() == '1' or 'const' in indep.lower() or 'intercept' in indep.lower():
-                data.loc[:, '_cons'] = 1
-                xvars.append('_cons')
-
-            elif '##' in indep or '*' in indep:
-                indep = indep.replace('##', ' X ')
-                indep = indep.replace('*', ' X ')
-                interxs = indep.split(' X ')
-                data.loc[:, indep] = 1
-                for interx in interxs:
-                    data.loc[:, indep] *= data.loc[:, interx]
-                xvars.append(indep)
-                xvars += interxs
-
-            elif (':' in indep or '#' in indep) and ('##' not in indep):
-                indep = indep.replace('#', ' X ')
-                indep = indep.replace(':', ' X ')
-                data[indep] = 1
-                for interx in indep.split(' X '):
-                    data[indep] *= data[interx]
-                xvars.append(indep)
-
-            elif 'log(' in indep:
-                logvar = indep[indep.find("(")+1:indep.find(")")]
-                data[f'log({logvar})'] = log(data[logvar])
-                xvars.append(indep)
-
-            else:
-                xvars.append(indep)
-
-        if len(formulas) > 1:
-            for _f in formulas:
-
-                # 3 handle fixed effects
-                if 'fe(' in _f:
-                    var_effects = _f[_f.find("(")+1:_f.find(")")].split(' ')
-                    other_effects = data[var_effects]
-
-                # 4 handle convariance estimators
-                elif 'cluster(' in _f:
-                    cov_type = 'clustered'
-                    var_effects = _f[_f.find("(")+1:_f.find(")")].split(' ')
-                    clusters = data[var_effects]
-                    cov_config.update({'clusters': clusters})
-
-                elif 'robust' in _f.lower() or 'heteroskedastic' in _f.lower():
-                    cov_type = 'robust'
-
-                elif 'kernel' in _f.lower():
-                    kernels = _f[_f.find("(")+1:_f.find(")")].split(' ')
-                    if len(kernels) > 1:
-                        kernel, bandwidth = kernels
-                        cov_config['bandwidth'] = bandwidth
-                    else:
-                        kernel = kernels[0]
-                    if kernel.lower() not in ['bartlett', 'parzen', 'qs']:
-                        pass  # raise error
-                    cov_type = 'kernel'
-                    cov_config['kernel'] = kernel
-
-                # 5 indicate if running in fama macbeth
-                elif 'famamacbeth' in _f.lower():
-                    fama_macbeth = True
-
-        if fama_macbeth:
-            return FamaMacBeth(
-                data[dep], data[xvars], weights=weights, check_rank=check_rank,
-            ).fit(cov_type=cov_type, debiased=debiased, bandwidth=bandwidth, kernel=kernel)
-        else:
-            return PanelOLS(
-                data[dep], data[xvars], 
-                entity_effects=entity_effects, time_effects=time_effects, other_effects=other_effects,
-                weights=weights, singletons=singletons, drop_absorbed=drop_absorbed, check_rank=check_rank,
-            ).fit(
-                use_lsdv=use_lsdv, use_lsmr=use_lsmr, low_memory=low_memory, cov_type=cov_type, 
-                debiased=debiased, auto_df=debiased, count_effects=count_effects, **cov_config
-                )
-
-    def _get_results(self, model, model_label, dep_label, decimal_coef: int = 2, decimal_tvalue: int = 2, decimal_rsquared: int = 2, coef_in_percentage: bool = True, varname_in_cap: bool = False):
-        '''This function returns a summary of regression results with various formatting options.
-        
-        Parameters
-        ----------
-        model
-            a statistical model object, such as a regression model
-        model_label
-            A label or name for the model being analyzed.
-        dep_label
-            The label for the dependent variable in the regression model.
-        decimal_coef : int, optional
-            The number of decimal places to display for the coefficient estimates.
-        decimal_tvalue : int, optional
-            The number of decimal places to display for the t-value in the output.
-        decimal_rsquared : int, optional
-            The number of decimal places to display for the R-squared values in the output.
-        coef_in_percentage : bool, optional
-            A boolean parameter that determines whether the coefficients should be displayed as percentages or
-        not. If set to True, the coefficients will be multiplied by 100 and displayed as percentages.
-        varname_in_cap : bool, optional
-            This parameter determines whether variable names should be displayed in uppercase or not. If set to
-        True, variable names will be displayed in uppercase.
-        
-        Returns
-        -------
-            a pandas DataFrame containing the results of a statistical model, including coefficients, t-values,
-        p-values, number of observations, and various measures of R-squared. The DataFrame also includes
-        information on whether fixed effects were included in the model and the dependent variable label.
-        
-        '''
-        percent = 100 if coef_in_percentage else 1
-        _pv = model.pvalues
-        _pv = _pv.mask(_pv <= .01, 3)
-        _pv = _pv.mask(_pv <= .05, 2)
-        _pv = _pv.mask(_pv <= .10, 1)
-        _pv = _pv.mask((_pv > .10) & (_pv < 1), 0)
-        _pv = _pv.apply(lambda x: int(x)*'*')
-        params = (model.params*percent).apply(lambda x: f'{x: .{decimal_coef}f}') + _pv
-        tstats = (model.tstats).apply(lambda x: f'{x: .{decimal_tvalue}f}')
-        tstats = '(' + tstats.astype(str) + ')'
-        tstats.index = tstats.index + " (T-value)"
-        _stats = concat([params, tstats]).sort_index()
-        _stats.index = _stats.index.str.replace('Intercept', '_cons', regex=True)
-        if varname_in_cap:
-            _stats.index = _stats.index.str.upper()
-        _stats['No. of Obs.'] = f'{model.nobs:,}'
-        _stats['Rsquared (Within) (%)'] = f'{model.rsquared_within*100: .{decimal_rsquared}f}'
-        _stats['Rsquared (Overall) (%)'] = f'{model.rsquared_overall*100: .{decimal_rsquared}f}'
-        _stats['Rsquared (%)'] = f'{model.rsquared*100: .{decimal_rsquared}f}'
-        try:
-            for effects in model.included_effects:
-                if 'Other Effect' in effects:
-                    effects = effects.split('(')[1].replace(')', '').capitalize()
-                _stats[f'{effects} Fixed Effects'] = 'YES'
-        except: # pylint: disable=bare-except
-            pass
-        _stats['Dep.'] = dep_label
-        _stats = _stats.rename(model_label).to_frame()
-        return _stats
-
-    def multiregressions(self, formulas, data, entity_label, time_label, **kwargs):
-        '''This function performs multiple regressions on a panel data set and returns the statistical results.
-        
-        Parameters
-        ----------
-        formulas
-            a dictionary where the keys are names of regression models and the values are formulas for the
-        models in the form of strings
-        data
-            The data parameter is a pandas DataFrame containing the data to be used in the regression analysis.
-        entity_label
-            The label for the entity variable in the dataset.
-        time_label
-            The label for the time variable in the dataset.
-        
-        Returns
-        -------
-            a pandas DataFrame containing the results of multiple regressions performed on the input data using
-        the input formulas. The DataFrame includes statistics such as coefficients, standard errors,
-        t-values, p-values, and R-squared values for each regression.
-        
-        '''
-        if not [entity_label, time_label] == data.index.names:
-            data = data.set_index([entity_label, time_label], drop=False)
-
-        stats = DataFrame()
-        for i in formulas:
-            print('Running Regression', i)
-            _data = data.copy()
-            model = self._panel_reg(formulas[i], _data,
-                            entity_label, time_label, **kwargs)
-            del _data
-            dep = formulas[i].replace(' ', '').split('~')[0]
-            _stats = self._get_results(model, i, dep)
-            stats = stats.merge(_stats, how='outer',
-                                right_index=True, left_index=True)
-        
-        stats['index'] = stats.index
-        lenth = len(stats)
-        stats.loc[stats.index.str.contains('Dep.'), ''] = 0
-        stats.loc[stats.index.str.contains(' X '), ''] = 1
-        stats.loc[stats.index.str.contains('_cons'), ''] = lenth - 4
-        stats.loc[stats.index.str.contains('Obs.'), ''] = lenth - 3
-        stats.loc[stats.index.str.contains('Rsquared'), ''] = lenth - 2
-        stats.loc[stats.index.str.contains('Fixed Effects'), ''] = lenth - 1
-        stats.loc[:, ''] = stats.loc[:, ''].fillna(lenth-5)
-
-        stats = stats.sort_values(by=['', 'index'])
-        stats.loc[stats.index.str.contains('T-value'), 'index'] = ''
-        stats = stats.set_index('index').drop(columns='')
-        stats.index.rename('', inplace=True)
-        return stats.replace(nan, '')
-
-class OLS:
-    """
-    developing
-    """
-
-    def __init__(self, y, x, constant=True, **args):
-        if constant:
-            x = sm.add_constant(x)
-        self.mod = sm.OLS(y, x).fit(**args)
-
-    def stats(self, param):
-        return self.mod.params[param], self.mod.tvalues[param], self.mod.pvalues[param]
-
-    def r2(self):
-        return self.mod.rsquared_adj
-
-def ols_regs(formulas, data, decimal: int = 2):
-    """
-    developing
-    """
-    stats = []
-    rsquared_adjs = []
-    nobss = []
-    for colname in formulas.keys():
-        formula = formulas[colname]
-        model = sm.OLS.from_formula(formula, data=data).fit(cov_type='HAC', cov_kwds={'maxlags':6})
-        stat = concat([model.params, model.tvalues, model.pvalues], axis=1)
-        stat.columns = ['coef', 'tvalue', 'pvalue']
-        stat = stat.unstack().rename(colname)
-        stats.append(stat)
-        rsquared_adjs.append(model.rsquared_adj)
-        nobss.append(model.nobs)
-    stats = concat(stats, axis=1)
-    stats = stats.sort_index()
-
-    stats[stats.loc[['pvalue'], :]<=0.01] = 3
-    stats[(stats.loc[['pvalue'], :]<=0.05)&(stats.loc[['pvalue'], :]>0.01)] = 2
-    stats[(stats.loc[['pvalue'], :]<=0.10)&(stats.loc[['pvalue'], :]>0.05)] = 1
-    stats[stats.loc[['pvalue'], :]<1] = nan
-    stats.loc[['pvalue'], :] = stats.loc[['pvalue'], :].fillna(0)
-    stats.loc[['pvalue'], :] = stats.loc[['pvalue'], :].applymap(lambda x:  int(x)*'*')
-    stats.loc[['coef'], :] *= 100
-
-    stats.loc[['coef', 'tvalue'], :] = stats.loc[['coef', 'tvalue'], :].applymap(lambda x: f'{x: .{decimal}f}')
-    stats = stats.replace("nan", "")
-    df = stats.loc['coef', :] + stats.loc['pvalue', :]
-    df.index = stats.loc[['coef'], :].index
-    stats.loc[['coef'], :] = df
-    stats = stats.drop(index='pvalue')
-    stats = stats.swaplevel().sort_index()
-    stats = concat([stats, DataFrame({('Adj R2 (%)',''): rsquared_adjs, ('Obs',''):nobss}, index=stats.columns).T])
-
-    stats.loc[['Adj R2 (%)'], :] = (stats.loc[['Adj R2 (%)'], :]*100).applymap(lambda x: f'{x: .{decimal}f}')
-    stats.loc[['Obs'], :] = stats.loc[['Obs'], :].astype(int)
-    return stats
+# -*- coding: utf-8 -*-
+
+from linearmodels import (FamaMacBeth, PanelOLS)
+from pandas import concat, DataFrame
+from numpy import log, nan
+from QuantFin.HandleError import QueryError
+
+def _panel_reg(
+        formula, data, weights=None, singletons=True, drop_absorbed=False, check_rank=True, 
+        use_lsdv=False, use_lsmr=False, low_memory=None, debiased=True, count_effects=True, 
+        bandwidth=None, kernel=None
+        ):
+    '''This is a Python function that handles panel regression using various fixed effects and
+    covariance estimators.
+    
+    Parameters
+    ----------
+    formula
+        The formula for the regression model in the form of a string, with the dependent variable on
+    the left side of the tilde (~) and the independent variables on the right side separated by plus
+    signs (+).
+    data
+        The data on which the regression is to be performed.
+    weights
+        Weights are used to adjust the contribution of each observation in the regression analysis.
+    They can be used to account for differences in sample sizes or to give more weight to certain
+    observations based on their importance or relevance to the analysis.
+    singletons, optional
+        A boolean indicating whether to include singleton columns in the regression. A singleton column
+    is a column with only one unique value, which does not provide any information for the
+    regression. If set to True, singleton columns will be included in the regression. If set to
+    False, singleton columns will be dropped.
+    drop_absorbed, optional
+        A boolean parameter that determines whether to drop absorbed variables from the regression.
+    Absorbed variables are those that are perfectly collinear with other independent variables in
+    the model. If set to True, the function will drop these variables from the model. If set to
+    False, the function will keep these variables in
+    check_rank, optional
+        A boolean parameter that indicates whether to check the rank of the design matrix before
+    fitting the model. If set to True, the function will raise an error if the rank is deficient.
+    use_lsdv, optional
+        A boolean indicating whether to use least-squares dummy variable (LSDV) estimation. Default is
+    False.
+    use_lsmr, optional
+        A boolean indicating whether to use the LSMR algorithm for solving the least squares problem.
+    Default is False.
+    low_memory
+        A boolean indicating whether to use a lower memory footprint algorithm for fitting the model.
+    If set to True, the algorithm will use less memory but may take longer to run. If set to False,
+    the algorithm will use more memory but may run faster. If set to None, the algorithm will
+    automatically choose
+    debiased, optional
+        A boolean parameter that indicates whether to use a debiased estimator for the covariance
+    matrix. If True, the estimator will be debiased. If False, the estimator will not be debiased.
+    count_effects, optional
+        A boolean parameter that indicates whether to count the number of entity and time effects
+    included in the model. If set to True, the number of entity and time effects will be returned as
+    attributes of the fitted model object.
+    bandwidth
+        The bandwidth parameter is used in kernel-based covariance estimators to determine the size of
+    the kernel window. It specifies the distance over which the kernel function is applied to
+    calculate the weights for each observation. A larger bandwidth will result in a smoother
+    estimate, while a smaller bandwidth will result in a more localized estimate
+    kernel
+        The type of kernel to use for kernel-based covariance estimation. Possible values are
+    'bartlett', 'parzen', and 'qs'.
+    
+    Returns
+    -------
+        either a FamaMacBeth or a PanelOLS object depending on the value of the fama_macbeth variable.
+    
+    '''
+    fama_macbeth = False
+    entity_effects, time_effects, other_effects = False, False, None
+    cov_type, cov_config = 'unadjusted', {}
+
+    # 1 handle formula
+    dep, right = formula.split('~')
+    dep = dep.replace(' ', '')
+    formulas = right.split(',')
+    if ' if ' in formulas[0]:
+        formulas[0], data_query = formulas[0].split(' if ')
+        data.query(data_query, inplace=True)
+        if data.empty:
+            raise QueryError("""Return a empty dataframe after Query""")
+    indeps = formulas[0].replace(' ', '').split('+')
+
+    # 2 handle right-hand variables
+    xvars = []
+    for indep in indeps:
+        if indep.lower() == '1' or 'const' in indep.lower() or 'intercept' in indep.lower():
+            data.loc[:, '_cons'] = 1
+            xvars.append('_cons')
+
+        elif '##' in indep or '*' in indep:
+            indep = indep.replace('##', ' X ')
+            indep = indep.replace('*', ' X ')
+            interxs = indep.split(' X ')
+            data.loc[:, indep] = 1
+            for interx in interxs:
+                data.loc[:, indep] *= data.loc[:, interx]
+            xvars.append(indep)
+            xvars += interxs
+
+        elif (':' in indep or '#' in indep) and ('##' not in indep):
+            indep = indep.replace('#', ' X ')
+            indep = indep.replace(':', ' X ')
+            data[indep] = 1
+            for interx in indep.split(' X '):
+                data[indep] *= data[interx]
+            xvars.append(indep)
+
+        elif 'log(' in indep:
+            logvar = indep[indep.find("(")+1:indep.find(")")]
+            data[f'log({logvar})'] = log(data[logvar])
+            xvars.append(indep)
+
+        else:
+            xvars.append(indep)
+
+    if len(formulas) > 1:
+        for _f in formulas:
+
+            # 3 handle fixed effects
+            if 'fe(' in _f:
+                var_effects = _f[_f.find("(")+1:_f.find(")")].split(' ')
+                other_effects = data[var_effects]
+
+            # 4 handle convariance estimators
+            elif 'cluster(' in _f:
+                cov_type = 'clustered'
+                var_effects = _f[_f.find("(")+1:_f.find(")")].split(' ')
+                clusters = data[var_effects]
+                cov_config.update({'clusters': clusters})
+
+            elif 'robust' in _f.lower() or 'heteroskedastic' in _f.lower():
+                cov_type = 'robust'
+
+            elif 'kernel' in _f.lower():
+                kernels = _f[_f.find("(")+1:_f.find(")")].split(' ')
+                if len(kernels) > 1:
+                    kernel, bandwidth = kernels
+                    cov_config['bandwidth'] = bandwidth
+                else:
+                    kernel = kernels[0]
+                if kernel.lower() not in ['bartlett', 'parzen', 'qs']:
+                    pass  # raise error
+                cov_type = 'kernel'
+                cov_config['kernel'] = kernel
+
+            # 5 indicate if running in fama macbeth
+            elif 'famamacbeth' in _f.lower():
+                fama_macbeth = True
+
+    if fama_macbeth:
+        return FamaMacBeth(
+            data[dep], data[xvars], weights=weights, check_rank=check_rank,
+        ).fit(cov_type=cov_type, debiased=debiased, bandwidth=bandwidth, kernel=kernel)
+    else:
+        return PanelOLS(
+            data[dep], data[xvars], 
+            entity_effects=entity_effects, time_effects=time_effects, other_effects=other_effects,
+            weights=weights, singletons=singletons, drop_absorbed=drop_absorbed, check_rank=check_rank,
+        ).fit(
+            use_lsdv=use_lsdv, use_lsmr=use_lsmr, low_memory=low_memory, cov_type=cov_type, 
+            debiased=debiased, auto_df=debiased, count_effects=count_effects, **cov_config
+            )
+
+def _get_results(
+        model, model_label, dep_label, decimal_coef: int = 2, decimal_tvalue: int = 2, 
+        decimal_rsquared: int = 2, coef_in_percentage: bool = True, varname_in_cap: bool = False
+        ):
+    '''This function returns a summary of regression results with various formatting options.
+    
+    Parameters
+    ----------
+    model
+        a statistical model object, such as a regression model
+    model_label
+        A label or name for the model being analyzed.
+    dep_label
+        The label for the dependent variable in the regression model.
+    decimal_coef : int, optional
+        The number of decimal places to display for the coefficient estimates.
+    decimal_tvalue : int, optional
+        The number of decimal places to display for the t-value in the output.
+    decimal_rsquared : int, optional
+        The number of decimal places to display for the R-squared values in the output.
+    coef_in_percentage : bool, optional
+        A boolean parameter that determines whether the coefficients should be displayed as percentages or
+    not. If set to True, the coefficients will be multiplied by 100 and displayed as percentages.
+    varname_in_cap : bool, optional
+        This parameter determines whether variable names should be displayed in uppercase or not. If set to
+    True, variable names will be displayed in uppercase.
+    
+    Returns
+    -------
+        a pandas DataFrame containing the results of a statistical model, including coefficients, t-values,
+    p-values, number of observations, and various measures of R-squared. The DataFrame also includes
+    information on whether fixed effects were included in the model and the dependent variable label.
+    
+    '''
+    percent = 100 if coef_in_percentage else 1
+    _pv = model.pvalues
+    _pv = _pv.mask(_pv <= .01, 3)
+    _pv = _pv.mask(_pv <= .05, 2)
+    _pv = _pv.mask(_pv <= .10, 1)
+    _pv = _pv.mask((_pv > .10) & (_pv < 1), 0)
+    _pv = _pv.apply(lambda x: int(x)*'*')
+    params = (model.params*percent).apply(lambda x: f'{x: .{decimal_coef}f}') + _pv
+    tstats = (model.tstats).apply(lambda x: f'{x: .{decimal_tvalue}f}')
+    tstats = '(' + tstats.astype(str) + ')'
+    tstats.index = tstats.index + " (T-value)"
+    _stats = concat([params, tstats]).sort_index()
+    _stats.index = _stats.index.str.replace('Intercept', '_cons', regex=True)
+    if varname_in_cap:
+        _stats.index = _stats.index.str.upper()
+    _stats['No. of Obs.'] = f'{model.nobs:,}'
+    _stats['Rsquared (Within) (%)'] = f'{model.rsquared_within*100: .{decimal_rsquared}f}'
+    _stats['Rsquared (Overall) (%)'] = f'{model.rsquared_overall*100: .{decimal_rsquared}f}'
+    _stats['Rsquared (%)'] = f'{model.rsquared*100: .{decimal_rsquared}f}'
+    try:
+        for effects in model.included_effects:
+            if 'Other Effect' in effects:
+                effects = effects.split('(')[1].replace(')', '').capitalize()
+            _stats[f'{effects} Fixed Effects'] = 'YES'
+    except: # pylint: disable=bare-except
+        pass
+    _stats['Dep.'] = dep_label
+    _stats = _stats.rename(model_label).to_frame()
+    return _stats
+
+def multiregs(formulas, data, entity_label, time_label, **kwargs):
+    '''
+    This function performs multiple regressions on a panel data set and returns the statistical results.
+    Special features:
+        1. Customize regression with stata-like string, e.g., 
+                "y ~ 1 + x1 + x2 if 2010<=year<=2020, fe(firmid, year, month), cluster(firmid)"
+                "y ~ 1 + x1 + x2 if 2010<=year<=2020, fe(firmid, year, month), robust"
+                "y ~ 1 + x1 + x2 if 2010<=year<=2020, famamacbeth, robust"
+        2. Return academic-like table summarising statistical results.
+    
+    Parameters
+    ----------
+    formulas
+        a dictionary where the keys are names of regression models and the values are formulas for the
+    models in the form of strings
+    data
+        The data parameter is a pandas DataFrame containing the data to be used in the regression analysis.
+    entity_label
+        The label for the entity variable in the dataset.
+    time_label
+        The label for the time variable in the dataset.
+    
+    Returns
+    -------
+        a pandas DataFrame containing the results of multiple regressions performed on the input data using
+    the input formulas. The DataFrame includes statistics such as coefficients, standard errors,
+    t-values, p-values, and R-squared values for each regression.
+    
+    '''
+    if not [entity_label, time_label] == data.index.names:
+        data = data.set_index([entity_label, time_label], drop=False)
+
+    stats = DataFrame()
+    for i in formulas:
+        print('Running Regression', i)
+        _data = data.copy()
+        model = _panel_reg(formulas[i], _data, **kwargs)
+        del _data
+        dep = formulas[i].replace(' ', '').split('~')[0]
+        _stats = _get_results(model, i, dep)
+        stats = stats.merge(_stats, how='outer',
+                            right_index=True, left_index=True)
+    
+    stats['index'] = stats.index
+    lenth = len(stats)
+    stats.loc[stats.index.str.contains('Dep.'), ''] = 0
+    stats.loc[stats.index.str.contains(' X '), ''] = 1
+    stats.loc[stats.index.str.contains('_cons'), ''] = lenth - 4
+    stats.loc[stats.index.str.contains('Obs.'), ''] = lenth - 3
+    stats.loc[stats.index.str.contains('Rsquared'), ''] = lenth - 2
+    stats.loc[stats.index.str.contains('Fixed Effects'), ''] = lenth - 1
+    stats.loc[:, ''] = stats.loc[:, ''].fillna(lenth-5)
+
+    stats = stats.sort_values(by=['', 'index'])
+    stats.loc[stats.index.str.contains('T-value'), 'index'] = ''
+    stats = stats.set_index('index').drop(columns='')
+    stats.index.rename('', inplace=True)
+    return stats.replace(nan, '')
```

### Comparing `QuantFin-0.0.1/QuantFin/ReqData.py` & `QuantFin-0.0.2/QuantFin/ReqData.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.1/QuantFin/_deciles.py` & `QuantFin-0.0.2/QuantFin/_deciles.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.1/QuantFin/tool.py` & `QuantFin-0.0.2/QuantFin/tool.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.1/QuantFin.egg-info/PKG-INFO` & `QuantFin-0.0.2/QuantFin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantFin
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for Academic Research on Asset Pricing
 Home-page: https://github.com/yuz0101/QuantFin
 Download-URL: https://github.com/yuz0101/QuantFin/archive/refs/tags/Test.tar.gz
 Author: Stephen Zhang
 Author-email: stephen_se@outlook.com
 License: MIT
 Keywords: ACADEMIC,EMPIRICAL,FIANCE,RESEARCH,QUANT,PORTFOLIO
@@ -22,15 +22,15 @@
 # QuantFin
 A toolkit for asset pricing.
 Working... ...
 
 ### Install
 
 ```consol
-pip install -i https://test.pypi.org/simple/ QuantFin==0.0.1
+pip install QuantFin==0.0.2
 ```
 
 ### Get started
 
 #### Momentum Effects
 
 1) Calculat momentum value on stocks (MOM)
```

### Comparing `QuantFin-0.0.1/README.md` & `QuantFin-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # QuantFin
 A toolkit for asset pricing.
 Working... ...
 
 ### Install
 
 ```consol
-pip install -i https://test.pypi.org/simple/ QuantFin==0.0.1
+pip install QuantFin==0.0.2
 ```
 
 ### Get started
 
 #### Momentum Effects
 
 1) Calculat momentum value on stocks (MOM)
```

### Comparing `QuantFin-0.0.1/setup.py` & `QuantFin-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="QuantFin",
     packages=["QuantFin"],
-    version="0.0.1",
+    version="0.0.2",
     license="MIT",
     description="Library for Academic Research on Asset Pricing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Stephen Zhang",
     author_email="stephen_se@outlook.com",
     url="https://github.com/yuz0101/QuantFin",
```

