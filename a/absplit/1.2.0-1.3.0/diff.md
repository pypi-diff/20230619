# Comparing `tmp/absplit-1.2.0.tar.gz` & `tmp/absplit-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absplit-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absplit-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absplit-1.2.0.tar` & `absplit-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     4958 2023-06-05 23:23:06.124000 absplit-1.2.0/.gitignore
--rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.2.0/.idea/.gitignore
--rw-r--r--   0        0        0      291 2023-06-12 08:40:13.087000 absplit-1.2.0/.idea/genetic_algorithm.iml
--rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.2.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      303 2023-06-12 08:40:13.168000 absplit-1.2.0/.idea/misc.xml
--rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.2.0/.idea/modules.xml
--rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.2.0/.idea/vcs.xml
--rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.2.0/LICENSE
--rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.2.0/MANIFEST.in
--rw-r--r--   0        0        0     7387 2023-06-14 16:57:57.554000 absplit-1.2.0/README.md
--rw-r--r--   0        0        0       62 2023-06-14 16:57:57.570000 absplit-1.2.0/absplit/__init__.py
--rw-r--r--   0        0        0     8654 2023-06-14 16:57:57.585000 absplit-1.2.0/absplit/data.py
--rw-r--r--   0        0        0    23681 2023-06-14 16:57:57.601000 absplit-1.2.0/absplit/ga.py
--rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.2.0/absplit/param.py
--rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.2.0/images/logo.jpeg
--rw-r--r--   0        0        0     1531 2023-06-14 16:57:57.617000 absplit-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.2.0/requirements.txt
--rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.2.0/tests/test_data.py
--rw-r--r--   0        0        0     2125 2023-06-12 08:32:24.989000 absplit-1.2.0/tests/test_ga.py
--rw-r--r--   0        0        0     8425 1970-01-01 00:00:00.000000 absplit-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4958 2023-06-05 23:23:06.124000 absplit-1.3.0/.gitignore
+-rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.3.0/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2023-06-12 08:40:13.087000 absplit-1.3.0/.idea/genetic_algorithm.iml
+-rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.3.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      303 2023-06-12 08:40:13.168000 absplit-1.3.0/.idea/misc.xml
+-rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.3.0/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.3.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.3.0/LICENSE
+-rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.3.0/MANIFEST.in
+-rw-r--r--   0        0        0     7816 2023-06-18 23:20:04.805000 absplit-1.3.0/README.md
+-rw-r--r--   0        0        0       93 2023-06-18 23:20:04.840000 absplit-1.3.0/absplit/__init__.py
+-rw-r--r--   0        0        0     8940 2023-06-14 19:51:59.610000 absplit-1.3.0/absplit/data.py
+-rw-r--r--   0        0        0    25425 2023-06-18 23:15:55.977000 absplit-1.3.0/absplit/ga.py
+-rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.3.0/absplit/param.py
+-rw-r--r--   0        0        0     3976 2023-06-18 21:48:19.019000 absplit-1.3.0/absplit/tutorials.py
+-rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.3.0/images/logo.jpeg
+-rw-r--r--   0        0        0     1531 2023-06-18 23:20:04.770000 absplit-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.3.0/requirements.txt
+-rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.3.0/tests/test_data.py
+-rw-r--r--   0        0        0     2125 2023-06-12 08:32:24.989000 absplit-1.3.0/tests/test_ga.py
+-rw-r--r--   0        0        0     8850 1970-01-01 00:00:00.000000 absplit-1.3.0/PKG-INFO
```

### Comparing `absplit-1.2.0/.gitignore` & `absplit-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `absplit-1.2.0/LICENSE` & `absplit-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `absplit-1.2.0/README.md` & `absplit-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.2.0-blue.svg)
+![version](https://img.shields.io/badge/version-1.3.0-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
@@ -132,31 +132,35 @@
 ```
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## API Reference
 ### Absplit 
 `ABSplit(df, metrics, splitting, date_col=None, ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)`
 
-Splits population into 2 groups. Mutually exclusive, completely exhaustive
+Splits population into n groups. Mutually exclusive, completely exhaustive
 
 Arguments:
-* `df` (pd.DataFrame): Dataframe to be split
-* `metrics` (str, list): Name of, or list of names of, metric columns in DataFrame
-* `splitting` (str): Name of column that represents individuals in the population that is getting split
+* `df` (pd.DataFrame): Dataframe of population to be split
+* `metrics` (str, list): Name of, or list of names of, metric columns in DataFrame to be considered in split
+* `splitting` (str): Name of column that represents individuals in the population that is getting split. For example, if 
+you wanted to split a dataframe of US counties, this would be the county name column
 * `date_col` (str, optional): Name of column that represents time periods, if applicable. If left empty, it will
 perform a static split, i.e. not across timeseries, (default `None`)
 * `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters, see 
 [here](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
 (default: `{}`)
 * `splits` (list, optional): How many groups to split into, and relative size of the groups (default: `[0.5, 0.5]`,
 2 groups of equal size)
 * `size_penalty` (float, optional): Penalty weighting for differences in the population count between groups 
 (default: `0`)
-* `cutoff_date` (str, optional): Cutoff date between fitting and validation data. If `None`, it will fit on all 
-available data. If cutoff date provided, RMSE scores will be for validation period
+* `cutoff_date` (str, optional): Cutoff date between fitting and validation data. For example, if you have data between 
+2023-01-01 and 2023-03-01, and the cutoff date is 2023-02-01, the algorithm will only perform the fit on data between 
+2023-01-01 and 2023-02-01. If `None`, it will fit on all available data. If cutoff date is provided, RMSE scores
+  (gotten by using the `ab.rmse` attribute) will only be for validation period (i.e., from 2023-02-01 to end of 
+timeseries)
 * `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on 
 one metrics more than the other, you can prioritise this here (default: `{}`)
 
 
 ### Match 
 `Match(population, sample, metrics, splitting, date_col=None, ga_params={}, metric_weights={})`
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.2.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.3.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
@@ -50,43 +50,49 @@
 generation fitness ab.fitness() # Visualise data ab.visualise() # Extract bin
 splits df = ab.results # Extract distributions summary df_dist =
 ab.distributions # Extract data aggregated by bins df_agg = ab.aggregations #
 Extract RMSE summary df_rmse = ab.rmse ```
                                                                   (back_to_top)
 ## API Reference ### Absplit `ABSplit(df, metrics, splitting, date_col=None,
 ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)` Splits
-population into 2 groups. Mutually exclusive, completely exhaustive Arguments:
-* `df` (pd.DataFrame): Dataframe to be split * `metrics` (str, list): Name of,
-or list of names of, metric columns in DataFrame * `splitting` (str): Name of
-column that represents individuals in the population that is getting split *
+population into n groups. Mutually exclusive, completely exhaustive Arguments:
+* `df` (pd.DataFrame): Dataframe of population to be split * `metrics` (str,
+list): Name of, or list of names of, metric columns in DataFrame to be
+considered in split * `splitting` (str): Name of column that represents
+individuals in the population that is getting split. For example, if you wanted
+to split a dataframe of US counties, this would be the county name column *
 `date_col` (str, optional): Name of column that represents time periods, if
 applicable. If left empty, it will perform a static split, i.e. not across
 timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
 genetic algorithm `pygad.GA` module parameters, see [here](https://
 pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
 for arguments you can pass (default: `{}`) * `splits` (list, optional): How
 many groups to split into, and relative size of the groups (default: `[0.5,
 0.5]`, 2 groups of equal size) * `size_penalty` (float, optional): Penalty
 weighting for differences in the population count between groups (default: `0`)
 * `cutoff_date` (str, optional): Cutoff date between fitting and validation
-data. If `None`, it will fit on all available data. If cutoff date provided,
-RMSE scores will be for validation period * `metric_weights` (dict, optional):
-Weights for each metric in the data. If you want the splitting to focus on one
-metrics more than the other, you can prioritise this here (default: `{}`) ###
-Match `Match(population, sample, metrics, splitting, date_col=None, ga_params=
-{}, metric_weights={})` Takes DataFrame `sample` and finds a comparable group
-in `population`. Arguments: * `population` (pd.DataFrame): Population to search
-for comparable group (**Must exclude sample data**) * `sample` (pd.DataFrame):
-Sample we are looking to find a match for. * `metrics` (str, list): Name of, or
-list of names of, metric columns in DataFrame * `splitting` (str): Name of
-column that represents individuals in the population that is getting split *
-`date_col` (str, optional): Name of column that represents time periods, if
-applicable. If left empty, it will perform a static split, i.e. not across
-timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
-genetic algorithm `pygad.GA` module parameters, see [here](https://
+data. For example, if you have data between 2023-01-01 and 2023-03-01, and the
+cutoff date is 2023-02-01, the algorithm will only perform the fit on data
+between 2023-01-01 and 2023-02-01. If `None`, it will fit on all available
+data. If cutoff date is provided, RMSE scores (gotten by using the `ab.rmse`
+attribute) will only be for validation period (i.e., from 2023-02-01 to end of
+timeseries) * `metric_weights` (dict, optional): Weights for each metric in the
+data. If you want the splitting to focus on one metrics more than the other,
+you can prioritise this here (default: `{}`) ### Match `Match(population,
+sample, metrics, splitting, date_col=None, ga_params={}, metric_weights={})`
+Takes DataFrame `sample` and finds a comparable group in `population`.
+Arguments: * `population` (pd.DataFrame): Population to search for comparable
+group (**Must exclude sample data**) * `sample` (pd.DataFrame): Sample we are
+looking to find a match for. * `metrics` (str, list): Name of, or list of names
+of, metric columns in DataFrame * `splitting` (str): Name of column that
+represents individuals in the population that is getting split * `date_col`
+(str, optional): Name of column that represents time periods, if applicable. If
+left empty, it will perform a static split, i.e. not across timeseries,
+(default `None`) * `ga_params` (dict, optional): Parameters for the genetic
+algorithm `pygad.GA` module parameters, see [here](https://
 pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
 for arguments you can pass (default: `{}`) * `splits` (list, optional): How
 many groups to split into, and relative size of the groups (default: `[0.5,
 0.5]`, 2 groups of equal size) * `metric_weights` (dict, optional): Weights for
 each metric in the data. If you want the splitting to focus on one metrics more
 than the other, you can prioritise this here (default: `{}`)
                                                                   (back_to_top)
```

### Comparing `absplit-1.2.0/absplit/data.py` & `absplit-1.3.0/absplit/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 
         Args:
             df (pd.DataFrame): Dataframe to process
             scaler (object, optional): Scaling function object. Default None
             scale (bool, optional): To apply scaling to data or not. Default True
             **kwargs: Additional keyword arguments
         """
-        # print(f'data: {cutoff_date}')
         super().__init__(**kwargs)
         self._df_stacked = df
         self._pre_fit_scaler = scaler
         self._scaler_flag = scale
         self._cutoff_date = cutoff_date
 
         self.remainder_cols = [x for x in self._df_stacked.columns if x not in self.all_spec_columns]
@@ -72,14 +71,19 @@
         self.reshape_tup = None
 
         logger.debug(f'Remainder: {self.remainder_cols}, dim_spec: {self.dim_spec_columns}, metric:{self.metrics}')
 
         self._check_columns_object()
 
         # Transformations
+        if self.date_col and self._cutoff_date:
+            self._df_stacked[self.date_col] = pd.to_datetime(self._df_stacked[self.date_col])
+            if self._df_stacked[self.date_col].max() < pd.to_datetime(self._cutoff_date):
+                raise ValueError('Arg `cutoff_date` is greater than maximum date value')
+
         self._df_stacked = self._set_indexes()
         self._df_unstacked = self._df_stacked.copy()
         self._scale()
         self._unstack()
 
         # Extract unstacked index
         self._df_index = pd.DataFrame(index=self._df_unstacked.index)
```

### Comparing `absplit-1.2.0/absplit/ga.py` & `absplit-1.3.0/absplit/ga.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,33 +102,39 @@
             'init_range_low',
             'init_range_high',
             'random_mutation_min_val',
             'random_mutation_max_val',
             'gene_type'
         ]
 
+        self._silence = [
+            'initial_population'
+        ]
+
         # Copy default, update
         self.params = dict(self._default_ga_params)
-        self._update_params(**kwargs)
+        self.update(**kwargs)
 
-    def _update_params(self, **kwargs):
+    def update(self, **kwargs):
         """Update GA params if any passed
 
         Returns:
             None
         """
 
         # Update if args passed
         if kwargs:
             for key, value in kwargs.items():
                 if key in self._dont_touch:
                     print(f'Parameter \'{key}\' is essential to running the genetic algorithm as a'\
                           f'discrete genetic algorith, and so you\'re not allowed to modify this')
                     continue
-                if not callable(value):
+                if callable(value) or key in self._silence:
+                    print(f'[Updating] {key}')
+                else:
                     print(f'[Updating] {key} to {value}')
                 self.params[key] = value
 
 
 class SplitBase(ParamMixin, ABC):
     """Base class for genetic algorithm orchestration.
 
@@ -165,16 +171,18 @@
             ga_params (dict, optional): Genetic algorithm parameters to add/modify
             metric_weights (dict, optional): Cost weightings to apply to metrics
             runs (int, optional): How many runs to try
             **kwargs: Additional keyword arguments
         """
         super().__init__(**kwargs)
         global size_penalty_global
+        global group_ids_global
         size_penalty_global = size_penalty
-        # print(cutoff_date)
+        group_ids_global = np.arange(0, len(splits))
+
         if ga_params:
             assert isinstance(ga_params, dict), 'ga_params must be a dictionary'
         self._runs = runs
         self._splits = splits
         self._splits_num = len(self._splits)
         self._ga_params = GAParams(splits=splits, **ga_params)
         self._best_score = -1
@@ -189,16 +197,14 @@
         self._df_vis = None  # Visualisation dataframe
         self._df_rmse = None  # RMSE between groups
         self._best_ga = None
         self._solution = None
 
         self._cost_weighting()
 
-        # print(self._cutoff_date)
-
     def _cost_weighting(self):
         """Set relative cost weights for each metric. Defaults to 1 unless specified.
 
         Used if you want the genetic algorithm to penalise the MSE cost of some metrics
         over others. Particularly useful if one metric is quite volatile, as the MSE cost can
         end up with it prioritising this over others.
 
@@ -249,54 +255,69 @@
                 self._best_score = self._ga.fitness
 
         if self._solution is None:
             raise ValueError('Solution is None')
 
         # Assign solution to index
         self._df_result = self._population.assign(self._solution)
+        self._post_run()
+        self._build_data()
+        logger.debug('Split complete')
+
+    def _build_data(self):
         self._build_distributions()
         self._build_df_vis()
         self._build_aggregation()
         self._build_rmse()
 
-        logger.debug('Split complete')
-
     @abstractmethod
     def _build_df_vis(self):
         pass
 
+    @abstractmethod
+    def _post_run(self):
+        pass
+
     def fitness(self, title=None):
         """Plots the fitness-generation graph
 
         Returns:
             None
         """
 
         if self._best_ga:
             self._best_ga.ga.plot_fitness(title=title)
         else:
             print('No solution available, please use .run() first')
 
     def _build_distributions(self):
-        """Build dataframe that contains data on the count distributions of each group
+        """Build dataframe that contains data on the population count distributions of each group
 
         Sets:
             _df_dist
         """
         self._df_dist = self._df_result['bin'].value_counts().to_frame('count')
         self._df_dist.index.name = 'bin'
         self._df_dist['pct'] = (self._df_dist['count'] / self._df_dist['count'].sum()).round(4)
         return self._df_dist.sort_index()
 
     def _build_rmse(self):
+        """Scores the RMSE for each group, for each metric.
+
+        If cutoff_date is passed in class init, rmse scores are only for the post-cutoff period.
+
+        Sets:
+            _df_rsme (pd.DataFrame): Datafame of RMSE scores for each group and metric
+        """
         df_agg = self._df_agg.copy()
 
         if self.date_col is None:
             df_agg.index = [0]*df_agg.shape[0]
 
+        # If cutoff, use post cut off period for rmse
         if self.date_col and self._cutoff_date:
             df_agg = df_agg[
                 df_agg[self.date_col] > pd.to_datetime(self._cutoff_date)
             ]
 
         df_ = df_agg.pivot(index=self.date_col, columns='bin', values=self.metrics)
         df_.columns = df_.columns.map('_'.join).str.lower()
@@ -346,15 +367,15 @@
         return self._df_rmse
 
     @property
     def aggregations(self):
         return self._df_agg
 
     def _build_aggregation(self):
-        """Aggregates data by bins
+        """Aggregates metric data by bins
 
         Sets:
             _df_agg
         """
 
         # Aggregate by bin
         group_cols = ['bin']
@@ -431,21 +452,31 @@
         """
         # print(cutoff_date)
         super().__init__(ga_params=ga_params, metric_weights=metric_weights, cutoff_date=cutoff_date, **kwargs)
         self.df = df
         self._population = Data(self.df.copy(), cutoff_date=cutoff_date, **kwargs)
 
     def _build_df_vis(self):
+        """Builds dataframe for use in visualisation of groups.
+
+        For ABSplit class, this is just joining the bins to the original data.
+
+        Sets:
+            _df_vis (pd.DataFrame):
+        """
         # Merge solution results (_df_results) onto input data (metrics) so that data can be visualised
         self._df_vis = self._population.stacked.merge(
             self._df_result,
             left_index=True,
             right_index=True
         )
 
+    def _post_run(self):
+        pass
+
     def __repr__(self):
         lst_str = [f"'{col}', " for col in self.all_spec_columns]
         return f'ABSplit([{lst_str}])'
 
 
 class MatchDataProc:
     """Ensures consistent number of dates between sample and population data
@@ -516,15 +547,14 @@
         _df_samp (pd.DataFrame): Dataframe of sample data
         _population (Data): Instance of the Data class for population data
         _sample (Data): Instance of the Data class for sample data
         _df_result (pd.DataFrame): Dataframe of population data that matches the sample group
         _df_vis (pd.DataFrame): Dataframe of population data, sample data and matched population data for visualization
 
     Methods:
-        _broadcast_match(): Makes the match matrix available globally
         run(): Runs the genetic algorithm
         fitness(): Plot generation fitness graph
         visualise(): Plots metrics using results from genetic algorithm output
     """
 
     def __init__(self, population, sample, ga_params={}, metric_weights={}, **kwargs):
         """Initializes the class and sets the attributes
@@ -536,15 +566,14 @@
             metric_weights (dict): Weights for the metrics being compared
             **kwargs: Additional keyword arguments
         """
 
         # Specify fitness function
         global fitness_func_match
         ga_params['fitness_func'] = fitness_func_match
-        ga_params['mutation_type'] = 'scramble'
         super().__init__(ga_params=ga_params, metric_weights=metric_weights, **kwargs)
         self._splits = [0.5, 0.5]
         self._splits_num = 2
         self._df_pop = population
         self._df_samp = sample
 
         # Ensure consistent dates between sample and population
@@ -555,44 +584,55 @@
 
         # Fit scaler on combined data
         scaler = preprocessing.MinMaxScaler()
         scaler.fit(pd.concat([self._df_pop, self._df_samp], axis=0)[self.metrics])
 
         self._population = Data(self._df_pop, scaler=scaler, **kwargs)
         self._sample = Data(self._df_samp, scaler=scaler, **kwargs)
-        self._broadcast_match()
-
-    def _broadcast_match(self):
-        """Makes the match matrix available globally
 
-        Returns:
-            None
-        """
+        # Makes the match matrix available globally, sum along population axis
         global match_metrics_global
-        match_metrics_global = self._sample.matrix
+        match_metrics_global = self._sample.matrix.sum(1)
 
-    def run(self):
-        """Runs the genetic algorithm, filters out all except sample and result
+        # Update initial population
+        pop_size = self._population.unstacked.shape[0]
+        sample_size = self._sample.unstacked.shape[0]
+        total = pop_size + sample_size
+        init_pop = np.random.choice(
+            [0, 1],
+            p=[pop_size/total, sample_size/total],
+            size=(self._ga_params.params['sol_per_pop'], self._population.unstacked.shape[0])
+        )
+        self._ga_params.update(initial_population=init_pop)
 
-        Returns:
-            None
-        """
-        # Run genetic algorithm
-        super().run()
+    def _post_run(self):
+        """Extract where solution == '1' from solution, concatenate with sample index and label sample bin '0'
 
+        Sets:
+            _df_result
+        """
         # Filter on only bin == 1
         self._df_result = self._df_result[self._df_result['bin'] == '1']
 
         # Get sample index, set as bin 0, concat to _df_results (which are all bin 1)
         index_cols = self._sample.index.index.names
         df_match = self._df_samp[index_cols].drop_duplicates().set_index(index_cols)
         df_match['bin'] = '0'
         self._df_result = pd.concat([self._df_result, df_match], axis=0).sort_index()
 
     def _build_df_vis(self):
+        """Build dataframe for visualisation
+
+        For Match class, this both population and sample data concatenated. All samples from the
+        popoulation that are not chosen from the matching process are filtered out by the inner
+        join on the results.
+
+        Sets:
+            _df_vis (pd.DataFrame): Dataframe of metrics and bin groups
+        """
         # Concat to form entire population
         self._df_vis = pd.concat([self._population.stacked, self._sample.stacked], axis=0)
 
         # Inner join to filter out all but sample and match
         self._df_vis = self._df_vis.merge(
             self._df_result,
             left_index=True,
@@ -604,23 +644,23 @@
         lst_str = [f"'{col}', " for col in self.all_spec_columns]
         return f'Match([{lst_str}])'
 
 
 def fitness_func_absplit(ga_instance, solution, solution_idx):
     """Fitness function for ABSplit
     """
-    global all_metrics_global
-    global metric_weights_global
-    global splits_global
-    global size_penalty_global
+    global all_metrics_global     # 3d matrix of (metrics, population, dates)
+    global metric_weights_global  # Relative weights for each metric
+    global splits_global          # Proportional splits for each group
+    global size_penalty_global    # Float weight for size penalty
+    global group_ids_global       # Array of group IDs
 
     # Generate binary array, 1 row of 0s and 1s for each group (where solution == 1/2/3 etc)
-    groups = np.array([(solution == i).astype(int) for i in range(len(splits_global))])
-
-    # print(groups.shape)
+    # groups = np.array([(solution == i).astype(int) for i in range(len(splits_global))])
+    groups = (solution == group_ids_global[:, None]).astype(int)
 
     # Size penalty
     # Calculate all_metrics mean * number of days * number of metrics
     mean = np.mean(all_metrics_global) * all_metrics_global.shape[0] * all_metrics_global.shape[2]
     # Get size cost for each group
     mean_group = (groups * mean).sum(1) * splits_global
     # Calculate group differences, sum
@@ -641,18 +681,18 @@
 def fitness_func_match(ga_instance, solution, solution_idx):
     """Fitness function for Match
     """
     global all_metrics_global
     global match_metrics_global
     global metric_weights_global
 
-    cost1 = match_metrics_global.sum(1)  # Sum along population axis
+    cost1 = match_metrics_global  # Sum along population axis
     cost2 = solution @ all_metrics_global
     # Average over time axis, sum over metric axis
     mse = (metric_weights_global @ ((cost1 - cost2)**2).mean(1)).sum()
 
     # Fitness
     fitness = 1.0 / np.abs(mse + 1e-10)  # Add small sum to prevent divide by zero
     return fitness
 
 
-fitness_func_match.__name__ = 'fitness_function_match'
+
```

### Comparing `absplit-1.2.0/absplit/param.py` & `absplit-1.3.0/absplit/param.py`

 * *Files identical despite different names*

### Comparing `absplit-1.2.0/images/logo.jpeg` & `absplit-1.3.0/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `absplit-1.2.0/pyproject.toml` & `absplit-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "absplit"
-version = "1.2.0"
+version = "1.3.0"
 description = "Generates A/B test groups"
 readme = "README.md"
 authors = [{name = "Cormac Rynne", email = "cormac.ry@gmail.com"}]
 license = {file = "LICENSE"}
 repository = "https://github.com/cormac-rynne/absplit"
 requires-python = "<=3.11"
 classifiers = [
```

### Comparing `absplit-1.2.0/tests/test_data.py` & `absplit-1.3.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `absplit-1.2.0/tests/test_ga.py` & `absplit-1.3.0/tests/test_ga.py`

 * *Files identical despite different names*

### Comparing `absplit-1.2.0/PKG-INFO` & `absplit-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absplit
-Version: 1.2.0
+Version: 1.3.0
 Summary: Generates A/B test groups
 Keywords: absplit,a/b test,ab test,ab split,split,set formation,group formation
 Author-email: Cormac Rynne <cormac.ry@gmail.com>
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -31,15 +31,15 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.2.0-blue.svg)
+![version](https://img.shields.io/badge/version-1.3.0-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
@@ -161,31 +161,35 @@
 ```
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## API Reference
 ### Absplit 
 `ABSplit(df, metrics, splitting, date_col=None, ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)`
 
-Splits population into 2 groups. Mutually exclusive, completely exhaustive
+Splits population into n groups. Mutually exclusive, completely exhaustive
 
 Arguments:
-* `df` (pd.DataFrame): Dataframe to be split
-* `metrics` (str, list): Name of, or list of names of, metric columns in DataFrame
-* `splitting` (str): Name of column that represents individuals in the population that is getting split
+* `df` (pd.DataFrame): Dataframe of population to be split
+* `metrics` (str, list): Name of, or list of names of, metric columns in DataFrame to be considered in split
+* `splitting` (str): Name of column that represents individuals in the population that is getting split. For example, if 
+you wanted to split a dataframe of US counties, this would be the county name column
 * `date_col` (str, optional): Name of column that represents time periods, if applicable. If left empty, it will
 perform a static split, i.e. not across timeseries, (default `None`)
 * `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters, see 
 [here](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
 (default: `{}`)
 * `splits` (list, optional): How many groups to split into, and relative size of the groups (default: `[0.5, 0.5]`,
 2 groups of equal size)
 * `size_penalty` (float, optional): Penalty weighting for differences in the population count between groups 
 (default: `0`)
-* `cutoff_date` (str, optional): Cutoff date between fitting and validation data. If `None`, it will fit on all 
-available data. If cutoff date provided, RMSE scores will be for validation period
+* `cutoff_date` (str, optional): Cutoff date between fitting and validation data. For example, if you have data between 
+2023-01-01 and 2023-03-01, and the cutoff date is 2023-02-01, the algorithm will only perform the fit on data between 
+2023-01-01 and 2023-02-01. If `None`, it will fit on all available data. If cutoff date is provided, RMSE scores
+  (gotten by using the `ab.rmse` attribute) will only be for validation period (i.e., from 2023-02-01 to end of 
+timeseries)
 * `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on 
 one metrics more than the other, you can prioritise this here (default: `{}`)
 
 
 ### Match 
 `Match(population, sample, metrics, splitting, date_col=None, ga_params={}, metric_weights={})`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: absplit Version: 1.2.0 Summary: Generates A/B test
+Metadata-Version: 2.1 Name: absplit Version: 1.3.0 Summary: Generates A/B test
 groups Keywords: absplit,a/b test,ab test,ab split,split,set formation,group
 formation Author-email: Cormac Rynne
 ry@gmail.com> Requires-Python: <=3.11 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -15,15 +15,15 @@
 Libraries :: Python Modules Requires-Dist: pygad==3.0.1 Requires-Dist: scikit-
 learn Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: seaborn
 Project-URL: Home, https://github.com/cormac-rynne/absplit
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.2.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.3.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
@@ -67,43 +67,49 @@
 generation fitness ab.fitness() # Visualise data ab.visualise() # Extract bin
 splits df = ab.results # Extract distributions summary df_dist =
 ab.distributions # Extract data aggregated by bins df_agg = ab.aggregations #
 Extract RMSE summary df_rmse = ab.rmse ```
                                                                   (back_to_top)
 ## API Reference ### Absplit `ABSplit(df, metrics, splitting, date_col=None,
 ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)` Splits
-population into 2 groups. Mutually exclusive, completely exhaustive Arguments:
-* `df` (pd.DataFrame): Dataframe to be split * `metrics` (str, list): Name of,
-or list of names of, metric columns in DataFrame * `splitting` (str): Name of
-column that represents individuals in the population that is getting split *
+population into n groups. Mutually exclusive, completely exhaustive Arguments:
+* `df` (pd.DataFrame): Dataframe of population to be split * `metrics` (str,
+list): Name of, or list of names of, metric columns in DataFrame to be
+considered in split * `splitting` (str): Name of column that represents
+individuals in the population that is getting split. For example, if you wanted
+to split a dataframe of US counties, this would be the county name column *
 `date_col` (str, optional): Name of column that represents time periods, if
 applicable. If left empty, it will perform a static split, i.e. not across
 timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
 genetic algorithm `pygad.GA` module parameters, see [here](https://
 pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
 for arguments you can pass (default: `{}`) * `splits` (list, optional): How
 many groups to split into, and relative size of the groups (default: `[0.5,
 0.5]`, 2 groups of equal size) * `size_penalty` (float, optional): Penalty
 weighting for differences in the population count between groups (default: `0`)
 * `cutoff_date` (str, optional): Cutoff date between fitting and validation
-data. If `None`, it will fit on all available data. If cutoff date provided,
-RMSE scores will be for validation period * `metric_weights` (dict, optional):
-Weights for each metric in the data. If you want the splitting to focus on one
-metrics more than the other, you can prioritise this here (default: `{}`) ###
-Match `Match(population, sample, metrics, splitting, date_col=None, ga_params=
-{}, metric_weights={})` Takes DataFrame `sample` and finds a comparable group
-in `population`. Arguments: * `population` (pd.DataFrame): Population to search
-for comparable group (**Must exclude sample data**) * `sample` (pd.DataFrame):
-Sample we are looking to find a match for. * `metrics` (str, list): Name of, or
-list of names of, metric columns in DataFrame * `splitting` (str): Name of
-column that represents individuals in the population that is getting split *
-`date_col` (str, optional): Name of column that represents time periods, if
-applicable. If left empty, it will perform a static split, i.e. not across
-timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
-genetic algorithm `pygad.GA` module parameters, see [here](https://
+data. For example, if you have data between 2023-01-01 and 2023-03-01, and the
+cutoff date is 2023-02-01, the algorithm will only perform the fit on data
+between 2023-01-01 and 2023-02-01. If `None`, it will fit on all available
+data. If cutoff date is provided, RMSE scores (gotten by using the `ab.rmse`
+attribute) will only be for validation period (i.e., from 2023-02-01 to end of
+timeseries) * `metric_weights` (dict, optional): Weights for each metric in the
+data. If you want the splitting to focus on one metrics more than the other,
+you can prioritise this here (default: `{}`) ### Match `Match(population,
+sample, metrics, splitting, date_col=None, ga_params={}, metric_weights={})`
+Takes DataFrame `sample` and finds a comparable group in `population`.
+Arguments: * `population` (pd.DataFrame): Population to search for comparable
+group (**Must exclude sample data**) * `sample` (pd.DataFrame): Sample we are
+looking to find a match for. * `metrics` (str, list): Name of, or list of names
+of, metric columns in DataFrame * `splitting` (str): Name of column that
+represents individuals in the population that is getting split * `date_col`
+(str, optional): Name of column that represents time periods, if applicable. If
+left empty, it will perform a static split, i.e. not across timeseries,
+(default `None`) * `ga_params` (dict, optional): Parameters for the genetic
+algorithm `pygad.GA` module parameters, see [here](https://
 pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
 for arguments you can pass (default: `{}`) * `splits` (list, optional): How
 many groups to split into, and relative size of the groups (default: `[0.5,
 0.5]`, 2 groups of equal size) * `metric_weights` (dict, optional): Weights for
 each metric in the data. If you want the splitting to focus on one metrics more
 than the other, you can prioritise this here (default: `{}`)
                                                                   (back_to_top)
```

