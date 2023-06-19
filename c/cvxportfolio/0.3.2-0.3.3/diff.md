# Comparing `tmp/cvxportfolio-0.3.2.tar.gz` & `tmp/cvxportfolio-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxportfolio-0.3.2.tar", last modified: Thu Jun 15 03:37:08 2023, max compression
+gzip compressed data, was "cvxportfolio-0.3.3.tar", last modified: Mon Jun 19 17:48:13 2023, max compression
```

## Comparing `cvxportfolio-0.3.2.tar` & `cvxportfolio-0.3.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-15 03:37:08.857925 cvxportfolio-0.3.2/
--rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.3.2/AUTHORS
--rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.3.2/LICENSE
--rw-r--r--   0 enzo       (501) staff       (20)      329 2023-06-15 03:37:08.857583 cvxportfolio-0.3.2/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)     5665 2023-05-30 16:04:26.000000 cvxportfolio-0.3.2/README.md
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-15 03:37:08.841769 cvxportfolio-0.3.2/cvxportfolio/
--rw-r--r--   0 enzo       (501) staff       (20)      912 2023-06-15 03:37:01.000000 cvxportfolio-0.3.2/cvxportfolio/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     2053 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/benchmark.py
--rw-r--r--   0 enzo       (501) staff       (20)    10850 2023-05-28 07:36:34.000000 cvxportfolio-0.3.2/cvxportfolio/constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)    14017 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    20123 2023-06-10 04:38:54.000000 cvxportfolio-0.3.2/cvxportfolio/data.py
--rw-r--r--   0 enzo       (501) staff       (20)     1004 2023-05-11 16:35:10.000000 cvxportfolio-0.3.2/cvxportfolio/errors.py
--rw-r--r--   0 enzo       (501) staff       (20)    13721 2023-05-28 07:37:04.000000 cvxportfolio-0.3.2/cvxportfolio/estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)     9446 2023-06-10 04:38:54.000000 cvxportfolio-0.3.2/cvxportfolio/forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)    21131 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     6483 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/result.py
--rw-r--r--   0 enzo       (501) staff       (20)     8731 2023-06-15 03:34:41.000000 cvxportfolio-0.3.2/cvxportfolio/returns.py
--rw-r--r--   0 enzo       (501) staff       (20)    17814 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    35304 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/simulator.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-15 03:37:08.855323 cvxportfolio-0.3.2/cvxportfolio/tests/
--rw-r--r--   0 enzo       (501) staff       (20)        0 2023-06-15 03:37:01.000000 cvxportfolio-0.3.2/cvxportfolio/tests/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     1623 2023-05-27 05:39:35.000000 cvxportfolio-0.3.2/cvxportfolio/tests/base.py
--rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.3.2/cvxportfolio/tests/returns.csv
--rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.3.2/cvxportfolio/tests/sigmas.csv
--rw-r--r--   0 enzo       (501) staff       (20)     9929 2023-05-27 05:39:35.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)     8359 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    10308 2023-05-27 05:39:35.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_data.py
--rw-r--r--   0 enzo       (501) staff       (20)     6698 2023-05-27 05:39:35.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)     8877 2023-06-10 04:38:54.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)    21842 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     5754 2023-06-10 04:38:54.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_returns.py
--rw-r--r--   0 enzo       (501) staff       (20)     9065 2023-05-27 05:39:35.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    25275 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_simulator.py
--rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.3.2/cvxportfolio/tests/volumes.csv
--rw-r--r--   0 enzo       (501) staff       (20)     1074 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/utils.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-15 03:37:08.843520 cvxportfolio-0.3.2/cvxportfolio.egg-info/
--rw-r--r--   0 enzo       (501) staff       (20)      329 2023-06-15 03:37:08.000000 cvxportfolio-0.3.2/cvxportfolio.egg-info/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)     1019 2023-06-15 03:37:08.000000 cvxportfolio-0.3.2/cvxportfolio.egg-info/SOURCES.txt
--rw-r--r--   0 enzo       (501) staff       (20)        1 2023-06-15 03:37:08.000000 cvxportfolio-0.3.2/cvxportfolio.egg-info/dependency_links.txt
--rw-r--r--   0 enzo       (501) staff       (20)       59 2023-06-15 03:37:08.000000 cvxportfolio-0.3.2/cvxportfolio.egg-info/requires.txt
--rw-r--r--   0 enzo       (501) staff       (20)       13 2023-06-15 03:37:08.000000 cvxportfolio-0.3.2/cvxportfolio.egg-info/top_level.txt
--rw-r--r--   0 enzo       (501) staff       (20)       38 2023-06-15 03:37:08.858009 cvxportfolio-0.3.2/setup.cfg
--rw-r--r--   0 enzo       (501) staff       (20)      783 2023-06-15 03:37:01.000000 cvxportfolio-0.3.2/setup.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-19 17:48:13.788514 cvxportfolio-0.3.3/
+-rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.3.3/AUTHORS
+-rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.3.3/LICENSE
+-rw-r--r--   0 enzo       (501) staff       (20)      329 2023-06-19 17:48:13.788174 cvxportfolio-0.3.3/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     5710 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/README.md
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-19 17:48:13.775309 cvxportfolio-0.3.3/cvxportfolio/
+-rw-r--r--   0 enzo       (501) staff       (20)      912 2023-06-19 17:48:06.000000 cvxportfolio-0.3.3/cvxportfolio/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     2053 2023-06-14 04:09:34.000000 cvxportfolio-0.3.3/cvxportfolio/benchmark.py
+-rw-r--r--   0 enzo       (501) staff       (20)    11940 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)    14023 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    20123 2023-06-10 04:38:54.000000 cvxportfolio-0.3.3/cvxportfolio/data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1004 2023-05-11 16:35:10.000000 cvxportfolio-0.3.3/cvxportfolio/errors.py
+-rw-r--r--   0 enzo       (501) staff       (20)    14756 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9724 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)    21189 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     6483 2023-06-14 04:09:34.000000 cvxportfolio-0.3.3/cvxportfolio/result.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9003 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)    17823 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    39747 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/simulator.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-19 17:48:13.787300 cvxportfolio-0.3.3/cvxportfolio/tests/
+-rw-r--r--   0 enzo       (501) staff       (20)        0 2023-06-19 17:48:06.000000 cvxportfolio-0.3.3/cvxportfolio/tests/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1623 2023-05-27 05:39:35.000000 cvxportfolio-0.3.3/cvxportfolio/tests/base.py
+-rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.3.3/cvxportfolio/tests/returns.csv
+-rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.3.3/cvxportfolio/tests/sigmas.csv
+-rw-r--r--   0 enzo       (501) staff       (20)     9929 2023-05-27 05:39:35.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8359 2023-06-14 04:09:34.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10308 2023-05-27 05:39:35.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     6737 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8877 2023-06-10 04:38:54.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)    21842 2023-06-14 04:09:34.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     5754 2023-06-10 04:38:54.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9065 2023-05-27 05:39:35.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    26143 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_simulator.py
+-rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.3.3/cvxportfolio/tests/volumes.csv
+-rw-r--r--   0 enzo       (501) staff       (20)     1269 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/utils.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-19 17:48:13.777056 cvxportfolio-0.3.3/cvxportfolio.egg-info/
+-rw-r--r--   0 enzo       (501) staff       (20)      329 2023-06-19 17:48:13.000000 cvxportfolio-0.3.3/cvxportfolio.egg-info/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     1019 2023-06-19 17:48:13.000000 cvxportfolio-0.3.3/cvxportfolio.egg-info/SOURCES.txt
+-rw-r--r--   0 enzo       (501) staff       (20)        1 2023-06-19 17:48:13.000000 cvxportfolio-0.3.3/cvxportfolio.egg-info/dependency_links.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       59 2023-06-19 17:48:13.000000 cvxportfolio-0.3.3/cvxportfolio.egg-info/requires.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       13 2023-06-19 17:48:13.000000 cvxportfolio-0.3.3/cvxportfolio.egg-info/top_level.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       38 2023-06-19 17:48:13.788594 cvxportfolio-0.3.3/setup.cfg
+-rw-r--r--   0 enzo       (501) staff       (20)      783 2023-06-19 17:48:06.000000 cvxportfolio-0.3.3/setup.py
```

### Comparing `cvxportfolio-0.3.2/LICENSE` & `cvxportfolio-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/README.md` & `cvxportfolio-0.3.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Cvxportfolio
 
 [![CVXportfolio on PyPI](https://img.shields.io/pypi/v/cvxportfolio.svg)](https://pypi.org/project/cvxportfolio/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cvxportfolio?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cvxportfolio)
-[![Documentation Status](https://readthedocs.org/projects/cvxportfolio/badge/?version=latest)](https://cvxportfolio.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/cvxgrp/cvxportfolio/badge.svg?branch=master)](https://coveralls.io/github/cvxgrp/cvxportfolio?branch=master)
 
 
 **WORK IN PROGRESS. Cvxportfolio is currently under development. We will freeze the user interface by end of 2023Q2 and release the first stable version by end of 2023Q3.**
 
 
 `cvxportfolio` is a python library for portfolio optimization and simulation
@@ -33,15 +32,18 @@
 
 
 Example
 ------------
 To get a sneak preview of `cvxportfolio` you may try the following code. This is available in `examples/hello_world.py` and runs 
 with `cvxportfolio >= 0.3.0`. All objects in `cvxportfolio` can either be provided data (in a variety of forms, but preferably pandas
 series or dataframes) or infer/download it. For example in the following example, market data is downloaded by a public source
-(Yahoo finance) and the forecasts are computed iteratively, at each point in the backtest, from past data. The logic used
+(Yahoo finance) and the forecasts are computed iteratively, at each point in the backtest, from past data. That is, at each point in the backtest,
+the policy object only operates on **past data**, and thus the result you get is a realistic simulation of what the strategy would have performed in the market.
+The simulator by default includes holding and transaction costs, using the models described in the book, and default parameters that are typical for the US stock market.
+The logic used
 matches what is described in Chapter 7 of the book. For example, returns are forecasted as the historical mean returns 
 and covariances as historical covariances (both ignoring `np.nan`'s). The logic used is detailed in the `forecast` module. Many optimizations
 are applied to make sure the system works well with real data. 
 
 
 ```python
 import cvxportfolio as cvx
@@ -68,19 +70,14 @@
 plt.title('Total value of the portfolio in time')
 plt.show()
 
 # plot weights of the (non-cash) assets for the SPO policy
 result.w.iloc[:, :-1].plot()
 plt.title('Weights of the portfolio in time')
 plt.show()
-
-print('\ntotal tcost ($)', result.tcost.sum())
-print('total borrow cost ($)', result.hcost_stocks.sum())
-print('total cash return + cost ($)', result.hcost_cash.sum())
-
 ```
 
 Development
 -----------
 Cvxportfolio is under development and things might change (quite fast), however you are (most) welcome to 
 read the code, play with it, and contribute. To set up a development environment locally you should
```

### Comparing `cvxportfolio-0.3.2/cvxportfolio/__init__.py` & `cvxportfolio-0.3.3/cvxportfolio/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 from .data import *
 from .simulator import *
 from .result import *
 from .policies import *
 from .constraints import *
 from .costs import *
 from .returns import *
```

### Comparing `cvxportfolio-0.3.2/cvxportfolio/benchmark.py` & `cvxportfolio-0.3.3/cvxportfolio/benchmark.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/cvxportfolio/constraints.py` & `cvxportfolio-0.3.3/cvxportfolio/constraints.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 and MultiPeriodOptimization policies, or other Cvxpy-based policies.
 """
 
 
 import cvxpy as cp
 import numpy as np
 
-from .estimator import CvxpyExpressionEstimator, ParameterEstimator, DataEstimator
+from .estimator import CvxpyExpressionEstimator, DataEstimator
 from .forecast import HistoricalFactorizedCovariance
 
 __all__ = [
     "LongOnly",
     "LeverageLimit",
     "LongCash",
     "DollarNeutral",
@@ -96,44 +96,44 @@
     See page 37 of the book.
     
     :param delta: constant or changing in time turnover limit 
     :type delta: float or pd.Series 
     """
     
     def __init__(self, delta):
-        self.delta = ParameterEstimator(delta)
+        self.delta = DataEstimator(delta, compile_parameter=True)
         
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
-        return .5 * cp.norm1(z[:-1]) <= self.delta
+        return .5 * cp.norm1(z[:-1]) <= self.delta.parameter
         
 
 class ParticipationRateLimit(BaseTradeConstraint):
     """A limit on maximum trades size as a fraction of market volumes.
     
 
     :param volumes: per-stock and per-day market volume estimates, or constant in time
     :type volumes: pd.Series or pd.DataFrame
     :param max_fraction_of_volumes: max fraction of market volumes that we're allowed to trade
     :type max_fraction_of_volumes: float, pd.Series, pd.DataFrame
     """
 
     def __init__(self, volumes, max_fraction_of_volumes=0.05):
-        self.volumes = ParameterEstimator(volumes)
-        self.max_participation_rate = ParameterEstimator(
-            max_fraction_of_volumes)
+        self.volumes = DataEstimator(volumes, compile_parameter=True)
+        self.max_participation_rate = DataEstimator(
+            max_fraction_of_volumes, compile_parameter=True)
         self.portfolio_value = cp.Parameter(nonneg=True)
 
     def values_in_time(self, current_portfolio_value, **kwargs):
         self.portfolio_value.value = current_portfolio_value
         super().values_in_time(current_portfolio_value=current_portfolio_value, **kwargs)
         
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return cp.multiply(cp.abs(z[:-1]), self.portfolio_value) <= cp.multiply(
-            self.volumes, self.max_participation_rate
+            self.volumes.parameter, self.max_participation_rate.parameter
         )
 
 
 class LongOnly(BaseWeightConstraint):
     """A long only constraint.
     
     Imposes that at each point in time the post-trade
@@ -141,31 +141,57 @@
     """
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[:-1] >= 0
 
 
+class NoTrade(BaseTradeConstraint):
+    """No-trade condition on name on periods(s)."""
+    
+    def __init__(self, asset, periods):
+        self.asset = asset
+        self.periods = periods
+    
+    def pre_evaluation(self, universe, backtest_times):
+        self.index = universe.get_loc(self.asset)
+        self.low = cp.Parameter()
+        self.high = cp.Parameter()
+    
+    def values_in_time(self, t, **kwargs):
+        if t in self.periods:
+            self.low.value = 0.
+            self.high.value = 0.
+        else:
+            self.low.value = -100.
+            self.high.value = +100.
+    
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+        return [z[self.index] >= self.low, 
+            z[self.index] <= self.high] 
+        
+
+
 class LeverageLimit(BaseWeightConstraint):
     """A limit on leverage.
     
     Leverage is defined as the :math:`\ell_1` norm of non-cash
     post-trade weights. Here we require that it is smaller than
     a given value
 
     :param limit: constant or varying in time leverage limit
     :type limit: float or pd.Series
     """
 
     def __init__(self, limit):
-        self.limit = ParameterEstimator(limit)
+        self.limit = DataEstimator(limit, compile_parameter=True)
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return cp.norm(w_plus[:-1], 1) <= self.limit
+        return cp.norm(w_plus[:-1], 1) <= self.limit.parameter
 
 
 class MinCashBalance(BaseWeightConstraint):
     """Requires that the cash account is larger than c_min dollars.
     
     This uses logic to subtract cash used as margin for the short 
     positions that is not documented in the book but is
@@ -206,34 +232,34 @@
     """A max limit on weights.
 
     Attributes:
       limit: A series or number giving the weights limit.
     """
 
     def __init__(self, limit):
-        self.limit = ParameterEstimator(limit)
+        self.limit = DataEstimator(limit, compile_parameter=True)
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return w_plus[:-1] <= self.limit
+        return w_plus[:-1] <= self.limit.parameter
 
 
 class MinWeights(BaseWeightConstraint):
     """A min limit on weights.
 
     Attributes:
       limit: A series or number giving the weights limit.
     """
 
     def __init__(self, limit):
-        self.limit = ParameterEstimator(limit)
+        self.limit = DataEstimator(limit, compile_parameter=True)
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return w_plus[:-1] >= self.limit
+        return w_plus[:-1] >= self.limit.parameter
 
 class MinMaxWeightsAtTimes(BaseWeightConstraint):
 
     def __init__(self, limit, times):
         self.base_limit = limit
         self.times = times
     
@@ -275,51 +301,51 @@
     Args:
         factor_exposure: An (n * r) matrix giving the factor exposure per asset
         per factor, where n represents # of assets and r represents # of factors
         limit: A series of list or a single list giving the factor limits
     """
 
     def __init__(self, factor_exposure, limit):
-        self.factor_exposure = ParameterEstimator(factor_exposure)
-        self.limit = ParameterEstimator(limit)
+        self.factor_exposure = DataEstimator(factor_exposure, compile_parameter=True)
+        self.limit = DataEstimator(limit, compile_parameter=True)
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return self.factor_exposure.T @ w_plus[:-1] <= self.limit
+        return self.factor_exposure.parameter.T @ w_plus[:-1] <= self.limit.parameter
 
 
 class FactorMinLimit(BaseWeightConstraint):
     """A min limit on portfolio-wide factor (e.g. beta) exposure.
 
     Args:
         factor_exposure: An (n * r) matrix giving the factor exposure per asset
         per factor, where n represents # of assets and r represents # of factors
         limit: A series of list or a single list giving the factor limits
     """
 
     def __init__(self, factor_exposure, limit):
-        self.factor_exposure = ParameterEstimator(factor_exposure)
-        self.limit = ParameterEstimator(limit)
+        self.factor_exposure = DataEstimator(factor_exposure, compile_parameter=True)
+        self.limit = DataEstimator(limit, compile_parameter=True)
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return self.factor_exposure.T @ w_plus[:-1] >= self.limit
+        return self.factor_exposure.parameter.T @ w_plus[:-1] >= self.limit.parameter
 
 
 class FixedFactorLoading(BaseWeightConstraint):
     """A constraint to fix portfolio loadings to a set of factors.
 
     This can be used to impose market neutrality, a certain portfolio-wide alpha, ....
 
     Attributes:
         factor_exposure: An (n * r) matrix giving the factor exposure on each
         factor
         target: A series or number giving the targeted factor loading
     """
 
     def __init__(self, factor_exposure, target):
-        self.factor_exposure = ParameterEstimator(factor_exposure)
-        self.target = ParameterEstimator(target)
+        self.factor_exposure = DataEstimator(factor_exposure, compile_parameter=True)
+        self.target = DataEstimator(target, compile_parameter=True)
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return self.factor_exposure.T @ w_plus[:-1] == self.target
+        return self.factor_exposure.parameter.T @ w_plus[:-1] == self.target.parameter
```

### Comparing `cvxportfolio-0.3.2/cvxportfolio/costs.py` & `cvxportfolio-0.3.3/cvxportfolio/costs.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 import cvxpy as cp
 import numpy as np
 import pandas as pd
 import copy
 import inspect
 
-from .estimator import CvxpyExpressionEstimator, ParameterEstimator, DataEstimator
+from .estimator import CvxpyExpressionEstimator,  DataEstimator
 from .utils import periods_per_year
 __all__ = ["HoldingCost", "TransactionCost"]
 
 
 class BaseCost(CvxpyExpressionEstimator):
     """Base class for cost objects (and also risks).
 
@@ -153,16 +153,16 @@
         dividends=0.):
         
         self.spread_on_borrowing_stocks_percent = None if spread_on_borrowing_stocks_percent is None else \
             DataEstimator(spread_on_borrowing_stocks_percent)
         if dividends is None:
             self.dividends = None
         else:
-            self.dividends = DataEstimator(dividends)
-            self.dividends_parameter = ParameterEstimator(dividends)
+            self.dividends = DataEstimator(dividends, compile_parameter=True)
+            #self.dividends_parameter = ParameterEstimator(dividends)
         
         self.spread_on_lending_cash_percent = None if spread_on_lending_cash_percent is None else \
             DataEstimator(spread_on_lending_cash_percent)        
         self.spread_on_borrowing_cash_percent = None if spread_on_borrowing_cash_percent is None else \
             DataEstimator(spread_on_borrowing_cash_percent)
             
         self.periods_per_year = periods_per_year
@@ -224,15 +224,15 @@
         
         expression = 0. 
         
         if not (self.spread_on_borrowing_stocks_percent is None):
            expression += cp.multiply(self.borrow_cost_stocks, cp.neg(w_plus)[:-1])
         
         if not (self.dividends is None):
-            expression -= cp.multiply(self.dividends_parameter, w_plus[:-1])
+            expression -= cp.multiply(self.dividends.parameter, w_plus[:-1])
         assert cp.sum(expression).is_convex()
         return cp.sum(expression)
 
 
 class TransactionCost(BaseCost):
     """A model for transaction costs.
```

### Comparing `cvxportfolio-0.3.2/cvxportfolio/data.py` & `cvxportfolio-0.3.3/cvxportfolio/data.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/cvxportfolio/errors.py` & `cvxportfolio-0.3.3/cvxportfolio/errors.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/cvxportfolio/estimator.py` & `cvxportfolio-0.3.3/cvxportfolio/estimator.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 This module implements Estimator base classes. Policies, costs, and constraints inherit
 from this.
 """
 
 import numpy as np
 import pandas as pd
 from .errors import MissingValuesError, DataError
-import cvxpy
+import cvxpy as cp
 
 
 class Estimator:
     """Estimator base class.
 
     Policies, costs, and constraints inherit from this. When overloading
     methods defined here one should be careful on deciding whether to call
@@ -93,15 +93,15 @@
         :type z: cvxpy.Variable
         :param w_plus_minus_w_bm: post-trade weights minus benchmark weights 
         :type w_plus_minus_w_bm: cvxpy.Variable
         """
         raise NotImplementedError
 
 
-class DataEstimator(Estimator):
+class DataEstimator(PolicyEstimator):
     """Estimator of point-in-time values from internal `self.data`.
 
     It also implements logic to check that no `np.nan` are returned
     by its `values_in_time` method, which is the way `cvxportfolio`
     objects use this class to get data.
 
     Args:
@@ -116,18 +116,30 @@
         use_last_available_time (bool): if the pandas index exists
             and is a pandas.DateTimeIndex you can instruct self.values_in_time
             to retrieve the last available value at time t by setting
             this to True. Default is False.
 
     """
 
-    def __init__(self, data, use_last_available_time=False, allow_nans=False):
+    def __init__(self, data, use_last_available_time=False, allow_nans=False, 
+        compile_parameter=False, non_negative=False, positive_semi_definite=False):
         self.data = data
         self.use_last_available_time = use_last_available_time
         self.allow_nans = allow_nans
+        self.compile_parameter = compile_parameter
+        self.non_negative = non_negative
+        self.positive_semi_definite =positive_semi_definite
+    
+    def pre_evaluation(self, universe, backtest_times):
+        # super().pre_evaluation(universe, backtest_times)
+        if self.compile_parameter:
+            value = self.internal_values_in_time(t=backtest_times[0])
+            self.parameter = cp.Parameter(value.shape if hasattr(value, "shape") else (), 
+                PSD=self.positive_semi_definite, nonneg=self.non_negative)
+            
 
     def value_checker(self, result):
         """Ensure that only scalars or arrays without np.nan are returned.
 
         Args:
             result (int, float, or np.array): data produced by self.values_in_time
 
@@ -214,14 +226,17 @@
         Returns:
             result (float, numpy.array): if you use a callable object make
                 sure that it returns a float or numpy array (and not,
                 for example, a pandas object)
 
         """
         self.current_value = self.internal_values_in_time(t, *args, **kwargs)
+        # we do this because in some cases they never get compiled
+        if hasattr(self, 'parameter'): 
+            self.parameter.value = self.current_value
         return self.current_value
 
 
 # class ConstantEstimator(cvxpy.Constant, DataEstimator):
 #     """Cvxpy constant that uses the pre_evalution method to be initialized."""
 #
 #     def pre_evaluation(self, returns, volumes, start_time, end_time, **kwargs):
@@ -293,37 +308,41 @@
 #             value if hasattr(value, "shape") else (),
 #             PSD=self.positive_semi_definite, nonneg=self.non_negative)
 #
 #     def values_in_time(self, t, **kwargs):
 #         self.parameter.value = self.internal_values_in_time(t, **kwargs)
         
         
-
-class ParameterEstimator(cvxpy.Parameter, DataEstimator, PolicyEstimator):
-    """Data estimator of point-in-time values that contains a Cvxpy Parameter.
-
-    Attributes:
-        parameter (cvxpy.Parameter): the parameter object to use with cvxpy
-            expressions
-    Args:
-        same as cvxportfolio.DataEstimator
-
-    """
-
-    def __init__(self, data, positive_semi_definite=False, non_negative=False, use_last_available_time=False, allow_nans=False):
-        self.positive_semi_definite = positive_semi_definite
-        self.non_negative = non_negative
-        self.use_last_available_time = use_last_available_time
-        self.data = data
-        self.allow_nans = allow_nans
-        # super(DataEstimator).__init__(data, use_last_available_time)
-
-    def pre_evaluation(self, universe, backtest_times):
-        """Use the start time of the simulation to initialize the Parameter."""
-        super().pre_evaluation(universe, backtest_times)
-        value = super().values_in_time(t=backtest_times[0])
-        super().__init__(value.shape if hasattr(value, "shape") else (), 
-            PSD=self.positive_semi_definite, nonneg=self.non_negative)
-
-    def values_in_time(self, t, **kwargs):
-        """Update Cvxpy Parameter value."""
-        self.value = super().values_in_time(t=t, **kwargs)
+#
+# class ParameterEstimator(DataEstimator):
+#     def __init__(self, *args, **kwargs):
+#         super().__init__(self, *args, compile_parameter=True, **kwargs)
+        
+# class ParameterEstimator(cvxpy.Parameter, DataEstimator, PolicyEstimator):
+#     """Data estimator of point-in-time values that contains a Cvxpy Parameter.
+#
+#     Attributes:
+#         parameter (cvxpy.Parameter): the parameter object to use with cvxpy
+#             expressions
+#     Args:
+#         same as cvxportfolio.DataEstimator
+#
+#     """
+#
+#     def __init__(self, data, positive_semi_definite=False, non_negative=False, use_last_available_time=False, allow_nans=False):
+#         self.positive_semi_definite = positive_semi_definite
+#         self.non_negative = non_negative
+#         self.use_last_available_time = use_last_available_time
+#         self.data = data
+#         self.allow_nans = allow_nans
+#         # super(DataEstimator).__init__(data, use_last_available_time)
+#
+#     def pre_evaluation(self, universe, backtest_times):
+#         """Use the start time of the simulation to initialize the Parameter."""
+#         super().pre_evaluation(universe, backtest_times)
+#         value = super().values_in_time(t=backtest_times[0])
+#         super().__init__(value.shape if hasattr(value, "shape") else (),
+#             PSD=self.positive_semi_definite, nonneg=self.non_negative)
+#
+#     def values_in_time(self, t, **kwargs):
+#         """Update Cvxpy Parameter value."""
+#         self.value = super().values_in_time(t=t, **kwargs)
```

### Comparing `cvxportfolio-0.3.2/cvxportfolio/forecast.py` & `cvxportfolio-0.3.3/cvxportfolio/forecast.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,17 @@
     This ignores both the cash returns column and all missing values.
     """
          
     def __post_init__(self):
         self.last_time = None
         self.last_counts = None
         self.last_sum = None
+        
+    def pre_evaluation(self, universe, backtest_times):
+        self.__post_init__()
     
     def values_in_time(self, t, past_returns, cache=None, **kwargs):
         super().values_in_time(t=t, past_returns=past_returns, cache=cache, **kwargs)
         self.update_chooser(t=t, past_returns=past_returns)
         self.current_value = (self.last_sum / self.last_counts).values        
         return self.current_value
         
@@ -141,14 +144,17 @@
 
     def __post_init__(self):
         if not self.kelly:
             self.meanforecaster = HistoricalMeanReturn()
         self.last_time = None
         self.last_counts = None
         self.last_sum = None
+        
+    def pre_evaluation(self, universe, backtest_times):
+        self.__post_init__()
     
     def values_in_time(self, t, past_returns, **kwargs):
         super().values_in_time(t=t, past_returns=past_returns, **kwargs)
         self.update_chooser(t=t, past_returns=past_returns)
         self.current_value = (self.last_sum / self.last_counts).values
         if not self.kelly:
             self.current_value -= self.meanforecaster.current_value**2
@@ -178,14 +184,17 @@
     """
     
     kelly: bool = True
     
     def __post_init__(self):
         self.last_time = None
     
+    def pre_evaluation(self, universe, backtest_times):
+        self.__post_init__()
+    
     @staticmethod
     def get_count_matrix(past_returns):
         r"""We obtain the matrix of non-null joint counts:
         
         .. math::
         
             \text{Count}\left(r^{i}r^{j} \neq \texttt{nan}\right).
```

### Comparing `cvxportfolio-0.3.2/cvxportfolio/policies.py` & `cvxportfolio-0.3.3/cvxportfolio/policies.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from .costs import BaseCost
 from .returns import BaseReturnsModel
 from .constraints import BaseConstraint
 from .estimator import PolicyEstimator, DataEstimator
 from .errors import MissingValuesError, PortfolioOptimizationError
 from .returns import ReturnsForecast, CashReturn
 from .benchmark import *
+from .utils import *
 
 __all__ = [
     "Hold",
     "SellAll",
     "FixedTrades",
     "PeriodicRebalance",
     "ProportionalRebalance",
@@ -358,16 +359,16 @@
         self.cvxpy_objective = [
             el.compile_to_cvxpy(self.w_plus_at_lags[i], self.z_at_lags[i], self.w_plus_minus_w_bm_at_lags[i]) 
             for i, el in enumerate(self.objective)]
         self.cvxpy_objective = sum(self.cvxpy_objective)
         assert self.cvxpy_objective.is_dcp()  # dpp=True)
         assert self.cvxpy_objective.is_concave()
         self.cvxpy_constraints = [
-            [constr.compile_to_cvxpy(self.w_plus_at_lags[i], self.z_at_lags[i], self.w_plus_minus_w_bm_at_lags[i]) 
-                for constr in el]
+            flatten_heterogeneous_list([constr.compile_to_cvxpy(self.w_plus_at_lags[i], self.z_at_lags[i], self.w_plus_minus_w_bm_at_lags[i]) 
+                for constr in el])
             for i, el in enumerate(self.constraints)]
         self.cvxpy_constraints = sum(self.cvxpy_constraints, [])
         self.cvxpy_constraints += [cp.sum(z) == 0 for z in self.z_at_lags]
         w = self.w_current
         for i in range(self.planning_horizon):
             self.cvxpy_constraints.append(self.w_plus_at_lags[i] == self.z_at_lags[i] + w)
             self.cvxpy_constraints.append(self.w_plus_at_lags[i] - self.w_bm == self.w_plus_minus_w_bm_at_lags[i])
@@ -375,14 +376,15 @@
         if not self.terminal_constraint is None:
             self.cvxpy_constraints.append(w == self.terminal_constraint)
         self.problem = cp.Problem(cp.Maximize(self.cvxpy_objective), self.cvxpy_constraints)
         assert self.problem.is_dcp()  # dpp=True)
 
     def pre_evaluation(self, universe, backtest_times):
         """Pass a full view of the data to initialize objects that need it."""
+        
         for obj in self.objective:
             obj.pre_evaluation(universe=universe, backtest_times=backtest_times)
         for constr_at_lag in self.constraints:
             for constr in constr_at_lag:
                 constr.pre_evaluation(universe=universe, backtest_times=backtest_times)
         
         self.benchmark.pre_evaluation(universe=universe, backtest_times=backtest_times)
```

### Comparing `cvxportfolio-0.3.2/cvxportfolio/result.py` & `cvxportfolio-0.3.3/cvxportfolio/result.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/cvxportfolio/returns.py` & `cvxportfolio-0.3.3/cvxportfolio/returns.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import cvxpy as cp
 import numpy as np
 import pandas as pd
 
 
 from .costs import BaseCost, CombinedCosts
 from .risks import BaseRiskModel
-from .estimator import DataEstimator, ParameterEstimator
+from .estimator import DataEstimator #, ParameterEstimator
 from .forecast import HistoricalMeanReturn, HistoricalMeanError
 
 __all__ = [
     "ReturnsForecast",
     "ReturnsForecastError",
     "CashReturn",
 ]
@@ -51,21 +51,25 @@
     
     :param short_margin_requirement: fraction of value of a short positions
         that is margined by portfolio cash
     :type short_margin_requirement: float
     """
     
     def __init__(self, cash_returns=None, short_margin_requirement=1.):
-        self.cash_returns = cash_returns
+        self.cash_returns = None if cash_returns is None else DataEstimator(cash_returns, 
+            compile_parameter=True, non_negative=True)
         self.short_margin_requirement = short_margin_requirement
         
     def pre_evaluation(self, universe, backtest_times):
-        self.cash_return_parameter = cp.Parameter(nonneg=True) if self.cash_returns is None \
-            else ParameterEstimator(self.cash_returns, non_negative=True)
         super().pre_evaluation(universe, backtest_times)
+        self.cash_return_parameter = cp.Parameter(nonneg=True) if self.cash_returns is None \
+            else self.cash_returns.parameter
+            
+        # else DataEstimator(self.cash_returns, non_negative=True, compile_parameter=True)
+        
         
     def values_in_time(self, t, past_returns, **kwargs):
         """Update cash return parameter as last cash return."""
         super().values_in_time(t=t, past_returns=past_returns, **kwargs)
         if self.cash_returns is None:
             self.cash_return_parameter.value = past_returns.iloc[-1,-1]
         
@@ -142,14 +146,15 @@
         if not r_hat is None:
             self.r_hat = DataEstimator(r_hat)
         else:
             self.r_hat = HistoricalMeanReturn()
         self.decay = decay
         
     def pre_evaluation(self, universe, backtest_times):
+        super().pre_evaluation(universe=universe, backtest_times=backtest_times)
         self.r_hat_parameter = cp.Parameter(len(universe)-1)
         
     def values_in_time(self, t, past_returns, mpo_step=0, **kwargs):
         super().values_in_time(t=t, past_returns=past_returns, mpo_step=mpo_step, **kwargs)
         self.r_hat_parameter.value = self.r_hat.current_value * self.decay**(mpo_step)
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
```

### Comparing `cvxportfolio-0.3.2/cvxportfolio/risks.py` & `cvxportfolio-0.3.3/cvxportfolio/risks.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .estimator import ParameterEstimator, DataEstimator 
+from .estimator import DataEstimator 
 import logging
 import warnings
 
 import scipy.linalg
 
 import cvxpy as cp
 import numpy as np
@@ -269,15 +269,15 @@
     #         assets' correlations. See the paper, pages 32-33.
 
     # """
 
     factor_Sigma = None
 
     def __init__(self, F=None, d=None, num_factors=1, kelly=True):#, normalize=False):
-        self.F = F if F is None else ParameterEstimator(F) 
+        self.F = F if F is None else DataEstimator(F, compile_parameter=True) 
         self.d = d if d is None else DataEstimator(d) 
         if (self.F is None) or (self.d is None):
             self.fit = True
             self.Sigma = HistoricalFactorizedCovariance(kelly=kelly) #Sigma
         else:
             self.fit = False
         self.num_factors = num_factors
@@ -322,15 +322,15 @@
     #         raise ForeCastError("Low rank risk estimation with iterative SVD did not work.")
     #     return F, idyosyncratic
 
     def pre_evaluation(self, universe, backtest_times):
         super().pre_evaluation(universe, backtest_times)
         # super().pre_evaluation(returns, volumes, start_time, end_time, **kwargs)
         self.idyosync_sqrt_parameter = cp.Parameter(len(universe)-1)
-        self.F_parameter = cp.Parameter((self.num_factors, len(universe)-1)) if self.F is None else self.F
+        self.F_parameter = cp.Parameter((self.num_factors, len(universe)-1)) if self.F is None else self.F.parameter
         # if not (self.factor_Sigma is None):
         #     self.factor_Sigma_sqrt = cp.Parameter(self.factor_Sigma.shape, PSD=True)
         # self.forecast_error_penalizer = cp.Parameter(returns.shape[1], nonneg=True)
 
     def values_in_time(self, t, past_returns, **kwargs):
         super().values_in_time(t=t, past_returns=past_returns, **kwargs)
```

### Comparing `cvxportfolio-0.3.2/cvxportfolio/simulator.py` & `cvxportfolio-0.3.3/cvxportfolio/simulator.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import time
 from pathlib import Path
 from multiprocess import Pool
 import pickle
 import hashlib
 from functools import cached_property
 from collections import defaultdict, OrderedDict
+from itertools import starmap
 
 import numpy as np
 import pandas as pd
 
 from .costs import BaseCost, TransactionCost, HoldingCost
 from .data import FredTimeSeries, YfinanceTimeSeries, BASE_LOCATION
 from .estimator import Estimator, DataEstimator
@@ -37,17 +38,14 @@
 from .utils import *
 from .errors import DataError
 
 PPY = 252
 __all__ = ['MarketSimulator', #'simulate_cash_holding_cost', 'simulate_stocks_holding_cost', 'simulate_transaction_cost', 
     'MarketData']
 
-
-def parallel_worker(policy, simulator, start_time, end_time, h):
-    return simulator._single_backtest(policy, start_time, end_time, h)
     
 def hash_universe(universe):
     return hashlib.sha256(bytes(str(tuple(universe)), 'utf-8')).hexdigest()
         
 def load_cache(universe, trading_interval, base_location):
     folder = base_location/f'hash(universe)={hash_universe(universe)},trading_interval={trading_interval}'
     try:
@@ -200,28 +198,28 @@
     def __init__(self, 
         universe = [], 
         returns=None,
         volumes=None,
         prices=None, 
         cash_key='USDOLLAR',
         base_location=BASE_LOCATION, 
-        min_history=PPY,
+        min_history=pd.Timedelta('365.24d'),
         max_contiguous_missing='10d',
         trading_interval=None,  # disabled for now because cache is not robust against this
         **kwargs,
     ):
         
         # TODO unblock once cache fixed
         # trading_interval = None
         
         # drop duplicates and ensure ordering
         universe = sorted(set(universe))
         
         self.base_location = Path(base_location)
-        self.min_history = min_history
+        self.min_history_timedelta = min_history
         self.max_contiguous_missing = max_contiguous_missing
         self.cash_key = cash_key
         
         if len(universe):
             self.get_market_data(universe)
             self.add_cash_column(self.cash_key)
         else:
@@ -231,21 +229,35 @@
             #     raise SyntaxError(
             #         "In `returns` you must include the cash returns as the last column (and not in `volumes`).")
             self.returns = returns
             self.volumes = volumes
             self.prices = prices
             if cash_key != returns.columns[-1]:
                 self.add_cash_column(cash_key)
-            
+                            
         if trading_interval:
             self.downsample(trading_interval)
         
         self.set_read_only()
         self.check_sizes()
-            
+    
+    
+    def _reduce_universe(self, reduced_universe):
+        assert reduced_universe[-1] == self.cash_key
+        return MarketData(
+            returns=self.returns[reduced_universe],
+            volumes=self.volumes[reduced_universe[:-1]] if not (self.volumes is None) else None,
+            prices=self.prices[reduced_universe[:-1]] if not (self.prices is None) else None,
+            cash_key = self.cash_key)
+    
+    @property
+    def min_history(self):
+        """Min. history expressed in periods."""
+        return int(np.round(self.PPY * (self.min_history_timedelta / pd.Timedelta('365.24d'))))
+        
     @property
     def universe(self):
         return self.returns.columns
         
     sampling_intervals = {'weekly': 'W-MON', 'monthly':'MS', 'quarterly':'QS', 'annual':'AS'}
         
     def downsample(self, interval):
@@ -367,17 +379,18 @@
             self.volumes = self.volumes.loc[self.volumes.index<drop_at]
         
         # for consistency we must also nan-out the last row of returns and volumes
         self.returns.iloc[-1] = np.nan
         self.volumes.iloc[-1] = np.nan
         
         
-    def backtest_times(self, start_time=None, end_time=None, include_end=False):
+    def backtest_times(self, start_time=None, end_time=None, include_end=True):
         """Get trading calendar from market data."""
         result = self.returns.index
+        result = result[result >= self.earliest_backtest_start]
         if start_time:
             result = result[result >= start_time]
         if end_time:
             result = result[(result <= end_time)]
         if not include_end:
             result = result[:-1]
         return result
@@ -415,15 +428,15 @@
         uni = []
         for ts in self.break_timestamps:
             uni += self.entry_dates[ts]
             uni = [el for el in uni if not el in self.exit_dates[ts]]
             result[ts] = tuple(sorted(uni))
         return result
     
-    @cached_property
+    @property
     def earliest_backtest_start(self):
         """Earliest date at which we can start a backtest."""
         return self.returns.iloc[:,:-1].dropna(how='all').index[self.min_history]
         
         
     def get_limited_backtests(self, start_time, end_time):
         """Get start/end times and universes of constituent backtests.
@@ -518,14 +531,15 @@
         self.base_location = Path(base_location)
         
         self.market_data = MarketData(
             universe=universe, returns=returns,
             volumes=volumes, prices=prices,
             cash_key=cash_key, base_location=base_location,
             trading_interval=trading_interval,
+            min_history=min_history_for_inclusion,
             **kwargs)
             
         self.trading_interval = trading_interval
                 
         if not len(universe) and prices is None:
             if round_trades:
                 raise SyntaxError(
@@ -616,54 +630,129 @@
             
         return h_next, z, u, realized_costs, policy_time
         
     def initialize_policy(self, policy, start_time, end_time):
         """Initialize the policy object.
         """
         policy.pre_evaluation(universe = self.market_data.universe,
-                             backtest_times = self.market_data.backtest_times(start_time, end_time))
-        
+                             backtest_times = self.market_data.backtest_times(start_time, end_time, include_end=False))
+
         # if policy initialized a cache, rewrite it with loaded one
-        if hasattr(policy, 'cache'):
-            policy.cache = load_cache(universe=self.market_data.universe, trading_interval = self.trading_interval, 
-                base_location=self.base_location)
-            
-                                 
-    def _single_backtest(self, policy, start_time, end_time, h):
-        
+        #if hasattr(policy, 'cache'):
+        #    policy.cache = load_cache(universe=self.market_data.universe, trading_interval = self.trading_interval,
+        #        base_location=self.base_location)
+
+
+    def _single_backtest(self, policy, start_time, end_time, h, universe=None#, backtest_times=None
+    ):
+        if universe is None:
+            universe = self.market_data.universe
+        #if backtest_times is None:
+        backtest_times = self.market_data.backtest_times(start_time, end_time, include_end=False)
+
         # self.initialize_policy(policy, start_time, end_time)
-        
+
         if hasattr(policy, 'compile_to_cvxpy'):
             policy.compile_to_cvxpy()
-        
-        result = BacktestResult(self.market_data.universe, self.market_data.backtest_times(start_time, end_time), self.costs)
-        
+
+        result = BacktestResult(universe, backtest_times, self.costs)
+
         # this is the main loop of a backtest
-        for t in self.market_data.backtest_times(start_time, end_time):
+        for t in backtest_times:
             result.h.loc[t] = h
+            # print(t, h)
             s = time.time()
             h, result.z.loc[t], result.u.loc[t], realized_costs, \
                     result.policy_times.loc[t] = self.simulate(t=t, h=h, policy=policy)
             for cost in realized_costs:
                 result.costs[cost].loc[t] = realized_costs[cost]
             result.simulator_times.loc[t] = time.time() - s - result.policy_times.loc[t]
 
-        result.h.loc[pd.Timestamp(end_time)] = h  
-        
+        result.h.loc[pd.Timestamp(end_time)] = h
+
         # TODO fix this
         result.cash_returns = self.market_data.returns.iloc[:,-1].loc[result.u.index]
-        
-        if hasattr(policy, 'cache'):
-            store_cache(cache=policy.cache, universe=self.market_data.universe, 
-            trading_interval = self.trading_interval, base_location=self.base_location)
-        
+
+        #if hasattr(policy, 'cache'):
+        #    store_cache(cache=policy.cache, universe=universe,
+        #    trading_interval = self.trading_interval, base_location=self.base_location)
+
         return result
+
+    def _concatenated_backtests(self, policy, start_time, end_time, h):
+        constituent_backtests_params = self.market_data.get_limited_backtests(start_time, end_time)
+        # print(constituent_backtests_params)
+        results = []
+        orig_md = self.market_data
+        orig_policy = policy
+        for el in constituent_backtests_params:
+            self.market_data = orig_md._reduce_universe(el['universe'])
+            # TODO improve
+            if len(el['universe']) > len(h):
+                tmp = pd.Series(0, el['universe'])
+                tmp[h.index] = h
+                h = tmp
+            else:
+                h = h[el['universe']]
+           #  # print('h')
+            # print(h)
+            
+            policy = copy.deepcopy(orig_policy)
+            # print(el['start_time'], el['end_time'])
+            policy.pre_evaluation(universe = el['universe'],
+                backtest_times = self.market_data.backtest_times(el['start_time'], el['end_time'], include_end=True))
+            if not (hasattr(self, 'PARALLEL') and self.PARALLEL):
+                if hasattr(policy, 'cache'):
+                    policy.cache = load_cache(universe=el['universe'], trading_interval = self.trading_interval, 
+                        base_location=self.base_location)
+                    
+            results.append(self._single_backtest(policy, el['start_time'], el['end_time'], h, el['universe']))
+            # print(results[0].w)
+            #print(results[0].h)
+            # print(results[0].returns)
+            # print(dir(results[0]))
+            h = results[-1].h.iloc[-1]
+            if not (hasattr(self, 'PARALLEL') and self.PARALLEL):
+                if hasattr(policy, 'cache'):
+                    store_cache(cache=policy.cache, universe=el['universe'], 
+                    trading_interval = self.trading_interval, base_location=self.base_location)
+        # print(results)
+        
+        res = BacktestResult.__new__(BacktestResult)
+        res.costs = {}
+        
+        res.h = pd.concat([el.h.iloc[:-1] if i < len(results) -1 else el.h for i, el in enumerate(results)])
+        for attr in ['cash_returns', 'u', 'z', 'simulator_times', 'policy_times']:
+            res.__setattr__(attr, pd.concat([el.__getattribute__(attr) for el in results]) )
+        # pandas concat can misalign the columns ordering
+        ck = self.market_data.cash_key
+        sortcol = sorted([el for el in res.u.columns if not el == ck]) + [ck]
+        res.u = res.u[sortcol]
+        res.z = res.z[sortcol]
+        # sortcol += [self.market_data.cash_key]
+        res.h = res.h[sortcol]
+        for k in results[0].costs:
+            res.costs[k] = pd.concat([el.costs[k] for el in results])
+        # raise Exception
+        # res.returns = pd.concat([el.returns el in results])
+        # res.cash_returns = pd.concat([el.cash_returns el in results])
+        # res.u = pd.concat([el.u el in results])
+        # res.z = pd.concat([el.z el in results])
+                
+        self.market_data = orig_md
+        # raise Exception
+        return res
         
+            
+    @staticmethod
+    def worker(policy, simulator, start_time, end_time, h):
+        #return simulator._single_backtest(policy, start_time, end_time, h)
+        return simulator._concatenated_backtests(policy, start_time, end_time, h)
                                     
-    def backtest(self, policy, start_time, end_time=None, initial_value = 1E6, h=None, parallel=True):
+    def backtest(self, policy, start_time=None, end_time=None, initial_value = 1E6, h=None, parallel=True):
         """Backtest one or more trading policy.
         
         If runnning in parallel you must be careful at how you use this method. If 
         you use this in a script, you should define the MarketSimulator
         *in* the `if __name__ == '__main__:'` clause, and call this method there as well.
         
         The default initial portfolio is all cash, or you can pass any portfolio with
@@ -710,47 +799,54 @@
         #     end_time  = self.returns.data.index[-1]
         # else:
         #    end_time = self.returns.data.index[self.returns.data.index <= end_time][-1]
             
         backtest_times_inclusive = self.market_data.backtest_times(start_time, end_time, include_end=True)
         start_time = backtest_times_inclusive[0]
         end_time = backtest_times_inclusive[-1]
+        
+        #constituent_backtests = self.market_data.get_limited_backtests(start_time, end_time)
+        #raise Exception
             
-        # TODO fix this - discard names that don't meet the min_history_for_inclusion
-        min_history = self.market_data.PPY * int(round(self.min_history_for_inclusion.days/365))
-        # print('min_history', min_history)
-        history = (~self.market_data.returns.loc[self.market_data.returns.index < start_time].isnull()).sum()
-        reduced_universe = self.market_data.returns.columns[history >= min_history]
-        # print('reduced_universe', reduced_universe)
-        self.market_data.returns = self.market_data.returns[reduced_universe]
-        if not (self.market_data.volumes is None):
-            self.market_data.volumes = self.market_data.volumes[reduced_universe[:-1]]
-        if not (self.market_data.prices is None):
-            self.market_data.prices = self.market_data.prices[reduced_universe[:-1]]
-        # self.sigma_estimate.data = self.sigma_estimate.data[reduced_universe[:-1]]
+        if False:
+            # TODO fix this - discard names that don't meet the min_history_for_inclusion
+            min_history = self.market_data.PPY * int(round(self.min_history_for_inclusion.days/365))
+            # print('min_history', min_history)
+            history = (~self.market_data.returns.loc[self.market_data.returns.index < start_time].isnull()).sum()
+            reduced_universe = self.market_data.returns.columns[history >= min_history]
+            # print('reduced_universe', reduced_universe)
+            self.market_data.returns = self.market_data.returns[reduced_universe]
+            if not (self.market_data.volumes is None):
+                self.market_data.volumes = self.market_data.volumes[reduced_universe[:-1]]
+            if not (self.market_data.prices is None):
+                self.market_data.prices = self.market_data.prices[reduced_universe[:-1]]
+            # self.sigma_estimate.data = self.sigma_estimate.data[reduced_universe[:-1]]
         
         # initialize policies and get initial portfolios
         for i in range(len(policy)):
-            self.initialize_policy(policy[i], start_time, end_time)
+            # self.initialize_policy(policy[i], start_time, end_time)
         
             if h[i] is None:
                 h[i] = pd.Series(0., self.market_data.universe)
                 h[i][-1] = initial_value
                 
-        def nonparallel_runner(zipped):
-            return self._single_backtest(zipped[0], start_time, end_time, zipped[1])
-                    
+        # def nonparallel_runner(zipped):
+        #     return self._single_backtest(zipped[0], start_time, end_time, zipped[1])
+        
+        zip_args = zip(policy, [self] * len(policy), [start_time] * len(policy), [end_time] * len(policy), h)
+        
         # decide if run in parallel or not
         if (not parallel) or len(policy)==1: 
-            result = list(map(nonparallel_runner, zip(policy, h)))
+            #result = list(map(nonparallel_runner, zip(policy, h)))
+            result = list(starmap(self.worker, zip_args))
         else:
+            self.PARALLEL = True # TODO temporary, to disable some features when running in parallel
             with Pool() as p:
-                result = p.starmap(parallel_worker, zip(policy, [self] * len(policy), [start_time] * len(policy), [end_time] * len(policy), h))
-           
-                
+                result = p.starmap(self.worker, zip_args)   
+            del self.PARALLEL
         if len(result) == 1:
             return result[0]
         return result
 
 # def _do_single_backtest(policy, start_time, end_time, simulator, cache):
 #     """This function can run on remote process/machine."""
 #
```

### Comparing `cvxportfolio-0.3.2/cvxportfolio/tests/base.py` & `cvxportfolio-0.3.3/cvxportfolio/tests/base.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/cvxportfolio/tests/returns.csv` & `cvxportfolio-0.3.3/cvxportfolio/tests/returns.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/cvxportfolio/tests/sigmas.csv` & `cvxportfolio-0.3.3/cvxportfolio/tests/sigmas.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/cvxportfolio/tests/test_constraints.py` & `cvxportfolio-0.3.3/cvxportfolio/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/cvxportfolio/tests/test_costs.py` & `cvxportfolio-0.3.3/cvxportfolio/tests/test_costs.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/cvxportfolio/tests/test_data.py` & `cvxportfolio-0.3.3/cvxportfolio/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/cvxportfolio/tests/test_estimator.py` & `cvxportfolio-0.3.3/cvxportfolio/tests/test_estimator.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 """Unit tests for the data and parameter estimator objects."""
 
 import numpy as np
 import pandas as pd
 import unittest
 
-from cvxportfolio.estimator import DataEstimator, ParameterEstimator
+from cvxportfolio.estimator import DataEstimator #, ParameterEstimator
 from cvxportfolio.errors import MissingValuesError, DataError
 
 
 class PlaceholderCallable:
     def __init__(self, value):
         self.value = value
 
@@ -158,18 +158,18 @@
 
 
     def test_parameter_estimator(self):
         timeindex = pd.date_range("2022-01-01", "2022-01-30")
         second_level = ["hello", "ciao", "hola"]
         index = pd.MultiIndex.from_product([timeindex, second_level])
         data = pd.DataFrame(np.random.randn(len(index), 10), index=index)
-        estimator = ParameterEstimator(data)
-        self.assertTrue( not hasattr(estimator, "value"))
+        estimator = DataEstimator(data, compile_parameter=True)
+        self.assertTrue( not hasattr(estimator, "parameter"))
         estimator.pre_evaluation(universe=None, backtest_times=timeindex)
         # assert hasattr(estimator, 'parameter')
-        self.assertTrue( hasattr(estimator, "value"))
+        self.assertTrue( hasattr(estimator, "parameter"))
         estimator.values_in_time("2022-01-05")
-        self.assertTrue( np.all(estimator.value == data.loc["2022-01-05"]))
+        self.assertTrue( np.all(estimator.parameter.value == data.loc["2022-01-05"]))
         
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cvxportfolio-0.3.2/cvxportfolio/tests/test_forecast.py` & `cvxportfolio-0.3.3/cvxportfolio/tests/test_forecast.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/cvxportfolio/tests/test_policies.py` & `cvxportfolio-0.3.3/cvxportfolio/tests/test_policies.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/cvxportfolio/tests/test_returns.py` & `cvxportfolio-0.3.3/cvxportfolio/tests/test_returns.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/cvxportfolio/tests/test_risks.py` & `cvxportfolio-0.3.3/cvxportfolio/tests/test_risks.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/cvxportfolio/tests/test_simulator.py` & `cvxportfolio-0.3.3/cvxportfolio/tests/test_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         self.assertTrue(current_and_past_returns.index[-1] == t)
         self.assertTrue(current_and_past_volumes.index[-1] == t)
         print(current_prices.name)
         print(t)
         self.assertTrue(current_prices.name == t)
         
     def test_break_timestamp(self):
-        md = MarketData(['AAPL', 'ZM', 'TSLA'], min_history=252, base_location=self.datadir)
+        md = MarketData(['AAPL', 'ZM', 'TSLA'], min_history=pd.Timedelta('365d'), base_location=self.datadir)
         self.assertTrue(pd.Timestamp('2020-04-20') in md.break_timestamps)
         # self.assertTrue(len(md.break_up_backtest('2000-01-01')) == 3)
         self.assertTrue(md.limited_universes[pd.Timestamp('2011-06-28')] == ('AAPL', 'TSLA'))
         
         
     def test_market_data_object_safety(self):
         t = self.returns.index[10]
@@ -458,14 +458,31 @@
             [#cvx.LongOnly(),
             cvx.LeverageLimit(1)], verbose=True)
         sim = cvx.MarketSimulator(['AAPL', 'MSFT'],#', 'GE', 'CVX', 'XOM', 'AMZN', 'ORCL', 'WMT', 'HD', 'DIS', 'MCD', 'NKE']
          base_location=self.datadir)
         result = sim.backtest(pol, pd.Timestamp('2023-01-01'), pd.Timestamp('2023-04-20'))
         
         print(result)
+        
+    def test_backtest_concatenation(self):
+        sim = cvx.MarketSimulator(['AAPL', 'ZM'])
+        pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast() -
+            cvx.ReturnsForecastError() -
+            .5 * cvx.FullCovariance(),
+            [#cvx.LongOnly(),
+            cvx.LeverageLimit(1)], verbose=True)
+        
+        result = sim.backtest(pol, pd.Timestamp('2020-04-01'), pd.Timestamp('2020-05-01')) # zoom enters in mid-april
+        ridx = result.w.index
+        self.assertTrue(result.w['ZM'].isnull().sum() > 5)
+        self.assertTrue(result.w['AAPL'].isnull().sum() < 2)
+        self.assertTrue(len(ridx) == len(set(ridx)))
+        self.assertTrue(len(ridx) == len(sim.market_data.returns.loc[
+            (sim.market_data.returns.index>=ridx[0]) & (sim.market_data.returns.index<=ridx[-1]) ]))
+        print(result)
             
     def test_multiple_backtest(self):
         
         pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast() -
             cvx.ReturnsForecastError() -
             .5 * cvx.FullCovariance(),
             [#cvx.LongOnly(),
```

### Comparing `cvxportfolio-0.3.2/cvxportfolio/tests/volumes.csv` & `cvxportfolio-0.3.3/cvxportfolio/tests/volumes.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/cvxportfolio/utils.py` & `cvxportfolio-0.3.3/cvxportfolio/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,17 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pandas as pd
 import numpy as np
 
-__all__ = ['periods_per_year', 'resample_returns']
+__all__ = ['periods_per_year', 'resample_returns', 'flatten_heterogeneous_list']
 
 def periods_per_year(idx):
     """Given a datetime pandas index return the periods per year."""
     return int(np.round(len(idx) / ((idx[-1] - idx[0]) / pd.Timedelta('365.24d'))))
     
 def resample_returns(returns, periods):
     """Resample returns expressed over number of periods to single period."""
     return np.exp(np.log(1 + returns) / periods) - 1
-    
+
+def flatten_heterogeneous_list(l):
+    """[1, 2, 3, [4, 5]] -> [1, 2, 3, 4, 5]"""
+    return sum(([el] if not hasattr(el, '__iter__') 
+        else el for el in l), [])
```

### Comparing `cvxportfolio-0.3.2/cvxportfolio.egg-info/SOURCES.txt` & `cvxportfolio-0.3.3/cvxportfolio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.2/setup.py` & `cvxportfolio-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='cvxportfolio',
-    version='0.3.2',
+    version='0.3.3',
     author='Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.',
     maintainer='Enzo Busseti',
     author_email='enzo.busseti@gmail.com',
     packages=['cvxportfolio',
               'cvxportfolio.tests'],
     package_dir={'cvxportfolio': 'cvxportfolio'},
     package_data={'cvxportfolio': [
```

