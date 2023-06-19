# Comparing `tmp/seaborn-analyzer-0.2.9.tar.gz` & `tmp/seaborn-analyzer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaborn-analyzer-0.2.9.tar", last modified: Sat Apr 23 11:08:13 2022, max compression
+gzip compressed data, was "seaborn-analyzer-0.3.0.tar", last modified: Mon Jun 19 08:11:46 2023, max compression
```

## Comparing `seaborn-analyzer-0.2.9.tar` & `seaborn-analyzer-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-04-23 11:08:13.875429 seaborn-analyzer-0.2.9/
--rw-rw-rw-   0        0        0     1551 2021-07-23 13:15:04.000000 seaborn-analyzer-0.2.9/LICENSE
--rw-rw-rw-   0        0        0    18266 2022-04-23 11:08:13.868431 seaborn-analyzer-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0    14360 2022-04-23 11:06:32.000000 seaborn-analyzer-0.2.9/README.rst
-drwxrwxrwx   0        0        0        0 2022-04-23 11:08:13.764451 seaborn-analyzer-0.2.9/seaborn_analyzer/
--rw-rw-rw-   0        0        0      184 2022-04-23 10:24:19.000000 seaborn-analyzer-0.2.9/seaborn_analyzer/__init__.py
--rw-rw-rw-   0        0        0    54159 2021-11-05 08:42:07.000000 seaborn-analyzer-0.2.9/seaborn_analyzer/_cv_eval_set.py
--rw-rw-rw-   0        0        0    83867 2021-11-03 16:57:13.000000 seaborn-analyzer-0.2.9/seaborn_analyzer/custom_class_plot.py
--rw-rw-rw-   0        0        0    22617 2021-08-30 13:54:02.000000 seaborn-analyzer-0.2.9/seaborn_analyzer/custom_hist_plot.py
--rw-rw-rw-   0        0        0    12386 2021-11-01 16:53:33.000000 seaborn-analyzer-0.2.9/seaborn_analyzer/custom_pair_plot.py
--rw-rw-rw-   0        0        0    99561 2022-04-23 10:24:19.000000 seaborn-analyzer-0.2.9/seaborn_analyzer/custom_reg_plot.py
--rw-rw-rw-   0        0        0     1675 2021-09-06 14:55:33.000000 seaborn-analyzer-0.2.9/seaborn_analyzer/multiclass_fitparams.py
-drwxrwxrwx   0        0        0        0 2022-04-23 11:08:13.837414 seaborn-analyzer-0.2.9/seaborn_analyzer.egg-info/
--rw-rw-rw-   0        0        0    18266 2022-04-23 11:08:11.000000 seaborn-analyzer-0.2.9/seaborn_analyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2022-04-23 11:08:12.000000 seaborn-analyzer-0.2.9/seaborn_analyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-23 11:08:11.000000 seaborn-analyzer-0.2.9/seaborn_analyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2022-04-23 11:08:11.000000 seaborn-analyzer-0.2.9/seaborn_analyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-04-23 11:08:11.000000 seaborn-analyzer-0.2.9/seaborn_analyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-04-23 11:08:13.878436 seaborn-analyzer-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     2241 2021-08-05 17:37:47.000000 seaborn-analyzer-0.2.9/setup.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-19 08:11:46.069201 seaborn-analyzer-0.3.0/
+-rw-r--r--   0 knakamura   (501) staff       (20)     1522 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.0/LICENSE
+-rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-19 08:11:46.068953 seaborn-analyzer-0.3.0/PKG-INFO
+-rw-r--r--   0 knakamura   (501) staff       (20)    14461 2023-06-19 08:03:26.000000 seaborn-analyzer-0.3.0/README.rst
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-19 08:11:46.067335 seaborn-analyzer-0.3.0/seaborn_analyzer/
+-rw-r--r--   0 knakamura   (501) staff       (20)      178 2023-06-19 08:03:43.000000 seaborn-analyzer-0.3.0/seaborn_analyzer/__init__.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    54281 2023-06-19 07:33:33.000000 seaborn-analyzer-0.3.0/seaborn_analyzer/_cv_eval_set.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    82441 2023-06-19 07:44:36.000000 seaborn-analyzer-0.3.0/seaborn_analyzer/custom_class_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    22202 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.0/seaborn_analyzer/custom_hist_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    12128 2021-11-01 17:19:31.000000 seaborn-analyzer-0.3.0/seaborn_analyzer/custom_pair_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    97795 2022-04-23 10:03:42.000000 seaborn-analyzer-0.3.0/seaborn_analyzer/custom_reg_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)     1635 2023-06-19 07:33:38.000000 seaborn-analyzer-0.3.0/seaborn_analyzer/multiclass_fitparams.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-19 08:11:46.068508 seaborn-analyzer-0.3.0/seaborn_analyzer.egg-info/
+-rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-19 08:11:46.000000 seaborn-analyzer-0.3.0/seaborn_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 knakamura   (501) staff       (20)      477 2023-06-19 08:11:46.000000 seaborn-analyzer-0.3.0/seaborn_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)        1 2023-06-19 08:11:46.000000 seaborn-analyzer-0.3.0/seaborn_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)      155 2023-06-19 08:11:46.000000 seaborn-analyzer-0.3.0/seaborn_analyzer.egg-info/requires.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)       17 2023-06-19 08:11:46.000000 seaborn-analyzer-0.3.0/seaborn_analyzer.egg-info/top_level.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)       38 2023-06-19 08:11:46.069255 seaborn-analyzer-0.3.0/setup.cfg
+-rw-r--r--   0 knakamura   (501) staff       (20)     2163 2023-06-19 08:02:59.000000 seaborn-analyzer-0.3.0/setup.py
```

### Comparing `seaborn-analyzer-0.2.9/LICENSE` & `seaborn-analyzer-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2021, Kenta Nakamura
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2021, Kenta Nakamura
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `seaborn-analyzer-0.2.9/README.rst` & `seaborn-analyzer-0.3.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,296 +1,313 @@
-================
-seaborn-analyzer
-================
-
-|python| |pypi| |license|
-
-.. |python| image:: https://img.shields.io/pypi/pyversions/seaborn-analyzer
-   :target: https://www.python.org/
-
-.. |pypi| image:: https://img.shields.io/pypi/v/seaborn-analyzer?color=blue
-   :target: https://pypi.org/project/seaborn-analyzer/
-
-.. |license| image:: https://img.shields.io/pypi/l/seaborn-analyzer?color=blue
-   :target: https://github.com/c60evaporator/seaborn-analyzer/blob/master/LICENSE
-   
-**A data analysis and visualization tool using Seaborn library.**
-
-.. image:: https://user-images.githubusercontent.com/59557625/126887193-ceba9bdd-3653-4d58-a916-21dcfe9c38a0.png
-
-=====
-Usage
-=====
-An example of using CustomPairPlot class
-
-.. code-block:: python
-
-    from seaborn_analyzer import CustomPairPlot
-    import seaborn as sns
- 
-    titanic = sns.load_dataset("titanic")
-    cp = CustomPairPlot()
-    cp.pairanalyzer(titanic, hue='survived')
-   
-If you want to know usage of the other classes, see `API Reference
-<https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#api-reference>`__ and `Examples
-<https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#examples>`__
-
-============
-Requirements
-============
-seaborn-analyzer 0.2.9 requires
-
-* Python >=3.6
-* Numpy >=1.20.3
-* Pandas >=1.2.4
-* Matplotlib >=3.3.4
-* Seaborn >=0.11.1
-* Scipy >=1.6.3
-* Scikit-learn >=0.24.2
-
-===========================
-Installing seaborn-analyzer
-===========================
-Use pip to install the binary wheels on `PyPI <https://pypi.org/project/seaborn-analyzer/>`__
-
-.. code-block:: console
-
-    $ pip install seaborn-analyzer
-
-=======
-Support
-=======
-Bugs may be reported at https://github.com/c60evaporator/seaborn-analyzer/issues
-
-=============
-API Reference
-=============
-The following classes and methods are included in seaborn-analyzer
-
-CustomPairPlot class
-====================
-
-.. csv-table::
-    :header: "Method name", "Summary", "API Documentation", "Example"
-    :widths: 30, 50, 15, 15
-
-    "**pairanalyzer**", Plot pair plot including scatter plot and correlation coefficient matrix simultaneously., `CustomPairPlot.pairanalyzer <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_pair_plot.CustomPairPlot.pairanalyzer>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#custompairplotpairanalyzer>`__
-
-
-hist class
-==========
-
-.. csv-table::
-    :header: "Method name", "Summary", "API Documentation", "Example"
-    :widths: 30, 50, 15, 15
-
-    "**plot_normality**", Plot normality test result and QQ plot., `hist.plot_normality <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_hist_plot.hist.plot_normality>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#histplot_normality>`__
-    "**fit_dist**", Fit distributions by maximum likelihood estimation and calculate fitting scores., `hist.fit_dist <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_hist_plot.hist.fit_dist>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#histfit_dist>`__
-
-
-classplot class
-===============
-
-.. csv-table::
-    :header: "Method name", "Summary", "API Documentation", "Example"
-    :widths: 30, 50, 15, 15
-
-    "**class_separator_plot**", Plot class separation lines of any scikit-learn classifier., `hist.class_separator_plot <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_class_plot.classplot.class_separator_plot>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#classplotclass_separator_plot>`__
-    "**class_proba_plot**", Plot class prediction probability of any scikit-learn classifier., `hist.class_proba_plot <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_class_plot.classplot.class_proba_plot>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#classplotclass_proba_plot>`__
-    "**plot_roc_curve_multiclass**", Plot ROC curve in multiclass classifier., `hist.class_separator_plot <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_class_plot.classplot.class_separator_plot>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#classplotplot_roc_curve_multiclass>`__
-    "**roc_plot**", Plot ROC curve with cross validation., `hist.class_proba_plot <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_class_plot.classplot.roc_plot>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#classplotroc_plot>`__
-
-regplot class
-=============
-
-.. csv-table::
-    :header: "Method name", "Summary", "API Documentation", "Example"
-    :widths: 30, 50, 15, 15
-
-    "**linear_plot**", Plot linear regression line and calculate Pearson correlation coefficient., `regplot.linear_plot <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_reg_plot.regplot.linear_plot>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#regplotlinear_plot>`__
-    "**regression_pred_true**", Plot prediction vs. true scatter plots of any scikit-learn regressor., `regplot.regression_pred_true <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_reg_plot.regplot.regression_pred_true>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#regplotregression_pred_true>`__
-    "**regression_plot_1d**", Plot regression lines of any scikit-learn regressor with 1D explanatory variable., `regplot.regression_plot_1d <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_reg_plot.regplot.regression_plot_1d>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#regplotregression_plot_1d>`__
-    "**regression_heat_plot**", Plot regression heatmaps of any scikit-learn regressor with 2 to 4D explanatory variables., `regplot.regression_heat_plot <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_reg_plot.regplot.regression_heat_plot>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#regplotregression_heat_plot>`__
-    "**average_plot**", Plot relationship between one explanatory variable and predicted value by line graph., `regplot.average_plot <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_reg_plot.regplot.average_plot>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#average_plot>`__
-
-
-========
-Examples
-========
-
-CustomPairPlot.pairanalyzer
-===========================
-.. code-block:: python
-
-    from seaborn_analyzer import CustomPairPlot
-    import seaborn as sns
-    titanic = sns.load_dataset("titanic")
-    cp = CustomPairPlot()
-    cp.pairanalyzer(titanic, hue='survived')
-.. image:: https://user-images.githubusercontent.com/59557625/115889860-4e8bde80-a48f-11eb-826a-cd3c79556a42.png
-
-hist.plot_normality
-===================
-.. code-block:: python
-
-    from seaborn_analyzer import hist
-    from sklearn.datasets import load_boston
-    import pandas as pd
-    df = pd.DataFrame(load_boston().data, columns= load_boston().feature_names)
-    hist.plot_normality(df, x='LSTAT', norm_hist=False, rounddigit=5)
-.. image:: https://user-images.githubusercontent.com/59557625/117275256-cfd46f80-ae98-11eb-9da7-6f6e133846fa.png
-
-hist.fit_dist
-=============
-.. code-block:: python
-
-    from seaborn_analyzer import hist
-    from sklearn.datasets import load_boston
-    import pandas as pd
-    import matplotlib.pyplot as plt
-    from scipy import stats
-    df = pd.DataFrame(load_boston().data, columns= load_boston().feature_names)
-    all_params, all_scores = hist.fit_dist(df, x='LSTAT', dist=['norm', 'gamma', 'lognorm', 'uniform'])
-    df_scores = pd.DataFrame(all_scores).T
-    df_scores
-.. image:: https://user-images.githubusercontent.com/59557625/115890066-81ce6d80-a48f-11eb-8390-f985d9e2b8b1.png
-.. image:: https://user-images.githubusercontent.com/59557625/115890108-8d219900-a48f-11eb-9896-38f7dedbb6e4.png
-
-classplot.class_separator_plot
-==============================
-.. code-block:: python
-
-    import seaborn as sns
-    from sklearn.svm import SVC
-    from seaborn_analyzer import classplot
-    iris = sns.load_dataset("iris")
-    clf = SVC()
-    classplot.class_separator_plot(clf, ['petal_width', 'petal_length'], 'species', iris)
-.. image:: https://user-images.githubusercontent.com/59557625/117274234-d7474900-ae97-11eb-9de2-c8a74dc179a5.png
-
-classplot.class_proba_plot
-==========================
-.. code-block:: python
-
-    import seaborn as sns
-    from sklearn.svm import SVC
-    from seaborn_analyzer import classplot
-    iris = sns.load_dataset("iris")
-    clf = SVC()
-    classplot.class_proba_plot(clf, ['petal_width', 'petal_length'], 'species', iris,
-                               proba_type='imshow')
-.. image:: https://user-images.githubusercontent.com/59557625/117276085-a1a35f80-ae99-11eb-8368-cdd1cfa78346.png
-
-classplot.plot_roc_curve_multiclass
-===================================
-.. code-block:: python
-
-    import seaborn as sns
-    from sklearn.svm import SVC
-    from sklearn.model_selection import train_test_split
-    import numpy as np
-    import matplotlib.pyplot as plt
-    from seaborn_analyzer import classplot
-    # Load dataset
-    iris = sns.load_dataset("iris")
-    OBJECTIVE_VARIALBLE = 'species'  # Objective variable
-    USE_EXPLANATORY = ['petal_width', 'petal_length', 'sepal_width', 'sepal_length']  # Explantory variables
-    y = iris[OBJECTIVE_VARIALBLE].values
-    X = iris[USE_EXPLANATORY].values
-    # Add random noise features
-    random_state = np.random.RandomState(0)
-    n_samples, n_features = X.shape
-    X = np.c_[X, random_state.randn(n_samples, 10 * n_features)]
-    # Plot ROC curve in multiclass classification
-    X_train, X_test, y_train, y_test = train_test_split(X, y, shuffle=True, random_state=42)
-    estimator = SVC(probability=True, random_state=42)
-    classplot.plot_roc_curve_multiclass(estimator, X_train, y_train, 
-                                        X_test=X_test, y_test=y_test)
-    plt.plot([0, 1], [0, 1], label='Chance', alpha=0.8,
-            lw=2, color='red', linestyle='--')
-    plt.legend(loc='lower right')
-.. image:: https://user-images.githubusercontent.com/59557625/132558369-c6bfee32-156b-4043-bedb-5b1854b00660.png
-
-classplot.roc_plot
-==================
-.. code-block:: python
-
-    from lightgbm import LGBMClassifier
-    import seaborn as sns
-    import matplotlib.pyplot as plt
-    from seaborn_analyzer import classplot
-    # Load dataset
-    iris = sns.load_dataset("iris")
-    OBJECTIVE_VARIALBLE = 'species'  # Objective variable
-    USE_EXPLANATORY = ['petal_width', 'petal_length', 'sepal_width', 'sepal_length']  # Explantory variables
-    y = iris[OBJECTIVE_VARIALBLE].values
-    X = iris[USE_EXPLANATORY].values
-    fit_params = {'verbose': 0,
-                'early_stopping_rounds': 10,
-                'eval_metric': 'rmse',
-                'eval_set': [(X, y)]
-                }
-    # Plot ROC curve with cross validation in multiclass classification
-    estimator = LGBMClassifier(random_state=42, n_estimators=10000)
-    fig, axes = plt.subplots(4, 1, figsize=(6, 24))
-    classplot.roc_plot(estimator, X, y, ax=axes, cv=3, fit_params=fit_params)
-.. image:: https://user-images.githubusercontent.com/59557625/132708291-99f7bda0-eb24-4fc0-8994-a976d097908e.png
-
-regplot.linear_plot
-===================
-.. code-block:: python
-
-    from seaborn_analyzer import regplot
-    import seaborn as sns
-    iris = sns.load_dataset("iris")
-    regplot.linear_plot(x='petal_length', y='sepal_length', data=iris)
-.. image:: https://user-images.githubusercontent.com/59557625/117276994-65243380-ae9a-11eb-8ec8-fa1fb5d60a55.png
-
-regplot.regression_pred_true
-============================
-.. code-block:: python
-
-    import pandas as pd
-    from seaborn_analyzer import regplot
-    import seaborn as sns
-    from sklearn.linear_model import LinearRegression
-    df_temp = pd.read_csv(f'./sample_data/temp_pressure.csv')
-    regplot.regression_pred_true(LinearRegression(), x=['altitude', 'latitude'], y='temperature', data=df_temp)
-.. image:: https://user-images.githubusercontent.com/59557625/117277036-6fdec880-ae9a-11eb-887a-5f8b2a93b0f9.png
-
-regplot.regression_plot_1d
-==========================
-.. code-block:: python
-
-    from seaborn_analyzer import regplot
-    import seaborn as sns
-    from sklearn.svm import SVR
-    iris = sns.load_dataset("iris")
-    regplot.regression_plot_1d(SVR(), x='petal_length', y='sepal_length', data=iris)
-.. image:: https://user-images.githubusercontent.com/59557625/117277075-78cf9a00-ae9a-11eb-835c-01f635754f7b.png
-
-regplot.regression_heat_plot
-============================
-.. code-block:: python
-
-    import pandas as pd
-    from sklearn.linear_model import LinearRegression
-    from seaborn_analyzer import regplot
-    df_temp = pd.read_csv(f'./sample_data/temp_pressure.csv')
-    regplot.regression_heat_plot(LinearRegression(), x=['altitude', 'latitude'], y='temperature', data=df_temp)
-.. image:: https://user-images.githubusercontent.com/59557625/115955837-1b4f5b00-a534-11eb-91b0-b913019d26ff.png
-
-regplot.average_plot
-============================
-.. code-block:: python
-
-    import seaborn as sns
-    from sklearn.svm import SVR
-    from seaborn_analyzer import regplot
-    iris = sns.load_dataset("iris")
-    svr = SVR()
-    features = ['petal_width', 'petal_length', 'sepal_width']
-    X = iris[features].values
-    y = iris['sepal_length'].values
-    regplot.average_plot(svr, X, y, x_colnames=features, cv=3)
-.. image:: https://user-images.githubusercontent.com/59557625/137940484-31f1fec7-012e-4c36-83a8-a1803755caa6.png
+================
+seaborn-analyzer
+================
+
+|python| |pypi| |license|
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/seaborn-analyzer
+   :target: https://www.python.org/
+
+.. |pypi| image:: https://img.shields.io/pypi/v/seaborn-analyzer?color=blue
+   :target: https://pypi.org/project/seaborn-analyzer/
+
+.. |license| image:: https://img.shields.io/pypi/l/seaborn-analyzer?color=blue
+   :target: https://github.com/c60evaporator/seaborn-analyzer/blob/master/LICENSE
+   
+**A data analysis and visualization tool using Seaborn library.**
+
+.. image:: https://user-images.githubusercontent.com/59557625/126887193-ceba9bdd-3653-4d58-a916-21dcfe9c38a0.png
+   :width: 720px
+   
+=====
+Usage
+=====
+An example of using CustomPairPlot class
+
+.. code-block:: python
+
+    from seaborn_analyzer import CustomPairPlot
+    import seaborn as sns
+ 
+    titanic = sns.load_dataset("titanic")
+    cp = CustomPairPlot()
+    cp.pairanalyzer(titanic, hue='survived')
+.. image:: https://user-images.githubusercontent.com/59557625/115889860-4e8bde80-a48f-11eb-826a-cd3c79556a42.png
+   :width: 480px
+   
+If you want to know the usage of the other classes, see `API Reference
+<https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#api-reference>`__ and `Examples
+<https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#examples>`__
+
+============
+Requirements
+============
+seaborn-analyzer 0.3.0 requires
+
+* Python >=3.6
+* Numpy >=1.20.3
+* Pandas >=1.2.4
+* Matplotlib >=3.1.3
+* Seaborn >=0.11.1
+* Scipy >=1.6.3
+* Scikit-learn >=0.24.2
+* LightGBM >=3.3.2
+
+===========================
+Installing seaborn-analyzer
+===========================
+Use pip to install the binary wheels on `PyPI <https://pypi.org/project/seaborn-analyzer/>`__
+
+.. code-block:: console
+
+    $ pip install seaborn-analyzer
+
+=======
+Support
+=======
+Bugs may be reported at https://github.com/c60evaporator/seaborn-analyzer/issues
+
+=============
+API Reference
+=============
+The following classes and methods are included in seaborn-analyzer
+
+CustomPairPlot class
+====================
+
+.. csv-table::
+    :header: "Method name", "Summary", "API Documentation", "Example"
+    :widths: 30, 50, 15, 15
+
+    "**pairanalyzer**", Plot pair plot including scatter plot and correlation coefficient matrix simultaneously., `CustomPairPlot.pairanalyzer <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_pair_plot.CustomPairPlot.pairanalyzer>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#custompairplotpairanalyzer>`__
+
+
+hist class
+==========
+
+.. csv-table::
+    :header: "Method name", "Summary", "API Documentation", "Example"
+    :widths: 30, 50, 15, 15
+
+    "**plot_normality**", Plot normality test result and QQ plot., `hist.plot_normality <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_hist_plot.hist.plot_normality>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#histplot_normality>`__
+    "**fit_dist**", Fit distributions by maximum likelihood estimation and calculate fitting scores., `hist.fit_dist <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_hist_plot.hist.fit_dist>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#histfit_dist>`__
+
+
+classplot class
+===============
+
+.. csv-table::
+    :header: "Method name", "Summary", "API Documentation", "Example"
+    :widths: 30, 50, 15, 15
+
+    "**class_separator_plot**", Plot class separation lines of any scikit-learn classifier., `hist.class_separator_plot <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_class_plot.classplot.class_separator_plot>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#classplotclass_separator_plot>`__
+    "**class_proba_plot**", Plot class prediction probability of any scikit-learn classifier., `hist.class_proba_plot <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_class_plot.classplot.class_proba_plot>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#classplotclass_proba_plot>`__
+    "**plot_roc_curve_multiclass**", Plot ROC curve in multiclass classifier., `hist.class_separator_plot <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_class_plot.classplot.class_separator_plot>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#classplotplot_roc_curve_multiclass>`__
+    "**roc_plot**", Plot ROC curve with cross validation., `hist.class_proba_plot <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_class_plot.classplot.roc_plot>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#classplotroc_plot>`__
+
+regplot class
+=============
+
+.. csv-table::
+    :header: "Method name", "Summary", "API Documentation", "Example"
+    :widths: 30, 50, 15, 15
+
+    "**linear_plot**", Plot linear regression line and calculate Pearson correlation coefficient., `regplot.linear_plot <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_reg_plot.regplot.linear_plot>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#regplotlinear_plot>`__
+    "**regression_pred_true**", Plot prediction vs. true scatter plots of any scikit-learn regressor., `regplot.regression_pred_true <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_reg_plot.regplot.regression_pred_true>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#regplotregression_pred_true>`__
+    "**regression_plot_1d**", Plot regression lines of any scikit-learn regressor with 1D explanatory variable., `regplot.regression_plot_1d <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_reg_plot.regplot.regression_plot_1d>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#regplotregression_plot_1d>`__
+    "**regression_heat_plot**", Plot regression heatmaps of any scikit-learn regressor with 2 to 4D explanatory variables., `regplot.regression_heat_plot <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_reg_plot.regplot.regression_heat_plot>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#regplotregression_heat_plot>`__
+    "**average_plot**", Plot relationship between one explanatory variable and predicted value by line graph., `regplot.average_plot <https://c60evaporator.github.io/seaborn-analyzer/seaborn_analyzer.html#seaborn_analyzer.custom_reg_plot.regplot.average_plot>`__, `example <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#average_plot>`__
+
+
+========
+Examples
+========
+
+CustomPairPlot.pairanalyzer
+===========================
+.. code-block:: python
+
+    from seaborn_analyzer import CustomPairPlot
+    import seaborn as sns
+    titanic = sns.load_dataset("titanic")
+    cp = CustomPairPlot()
+    cp.pairanalyzer(titanic, hue='survived')
+.. image:: https://user-images.githubusercontent.com/59557625/115889860-4e8bde80-a48f-11eb-826a-cd3c79556a42.png
+   :width: 640px
+   
+hist.plot_normality
+===================
+.. code-block:: python
+
+    from seaborn_analyzer import hist
+    from sklearn.datasets import load_boston
+    import pandas as pd
+    df = pd.DataFrame(load_boston().data, columns= load_boston().feature_names)
+    hist.plot_normality(df, x='LSTAT', norm_hist=False, rounddigit=5)
+.. image:: https://user-images.githubusercontent.com/59557625/117275256-cfd46f80-ae98-11eb-9da7-6f6e133846fa.png
+   :width: 240px
+
+hist.fit_dist
+=============
+.. code-block:: python
+
+    from seaborn_analyzer import hist
+    from sklearn.datasets import load_boston
+    import pandas as pd
+    import matplotlib.pyplot as plt
+    from scipy import stats
+    df = pd.DataFrame(load_boston().data, columns= load_boston().feature_names)
+    all_params, all_scores = hist.fit_dist(df, x='LSTAT', dist=['norm', 'gamma', 'lognorm', 'uniform'])
+    df_scores = pd.DataFrame(all_scores).T
+    df_scores
+.. image:: https://user-images.githubusercontent.com/59557625/115890066-81ce6d80-a48f-11eb-8390-f985d9e2b8b1.png
+   :width: 280px
+.. image:: https://user-images.githubusercontent.com/59557625/115890108-8d219900-a48f-11eb-9896-38f7dedbb6e4.png
+   :width: 280px
+
+classplot.class_separator_plot
+==============================
+.. code-block:: python
+
+    import seaborn as sns
+    from sklearn.svm import SVC
+    from seaborn_analyzer import classplot
+    iris = sns.load_dataset("iris")
+    clf = SVC()
+    classplot.class_separator_plot(clf, ['petal_width', 'petal_length'], 'species', iris)
+.. image:: https://user-images.githubusercontent.com/59557625/117274234-d7474900-ae97-11eb-9de2-c8a74dc179a5.png
+   :width: 320px
+
+classplot.class_proba_plot
+==========================
+.. code-block:: python
+
+    import seaborn as sns
+    from sklearn.svm import SVC
+    from seaborn_analyzer import classplot
+    iris = sns.load_dataset("iris")
+    clf = SVC()
+    classplot.class_proba_plot(clf, ['petal_width', 'petal_length'], 'species', iris,
+                               proba_type='imshow')
+.. image:: https://user-images.githubusercontent.com/59557625/117276085-a1a35f80-ae99-11eb-8368-cdd1cfa78346.png
+   :width: 320px
+
+classplot.plot_roc_curve_multiclass
+===================================
+.. code-block:: python
+
+    import seaborn as sns
+    from sklearn.svm import SVC
+    from sklearn.model_selection import train_test_split
+    import numpy as np
+    import matplotlib.pyplot as plt
+    from seaborn_analyzer import classplot
+    # Load dataset
+    iris = sns.load_dataset("iris")
+    OBJECTIVE_VARIALBLE = 'species'  # Objective variable
+    USE_EXPLANATORY = ['petal_width', 'petal_length', 'sepal_width', 'sepal_length']  # Explantory variables
+    y = iris[OBJECTIVE_VARIALBLE].values
+    X = iris[USE_EXPLANATORY].values
+    # Add random noise features
+    random_state = np.random.RandomState(0)
+    n_samples, n_features = X.shape
+    X = np.c_[X, random_state.randn(n_samples, 10 * n_features)]
+    # Plot ROC curve in multiclass classification
+    X_train, X_test, y_train, y_test = train_test_split(X, y, shuffle=True, random_state=42)
+    estimator = SVC(probability=True, random_state=42)
+    classplot.plot_roc_curve_multiclass(estimator, X_train, y_train, 
+                                        X_test=X_test, y_test=y_test)
+    plt.plot([0, 1], [0, 1], label='Chance', alpha=0.8,
+            lw=2, color='red', linestyle='--')
+    plt.legend(loc='lower right')
+.. image:: https://user-images.githubusercontent.com/59557625/132558369-c6bfee32-156b-4043-bedb-5b1854b00660.png
+   :width: 320px
+
+classplot.roc_plot
+==================
+.. code-block:: python
+
+    from lightgbm import LGBMClassifier
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    from seaborn_analyzer import classplot
+    # Load dataset
+    iris = sns.load_dataset("iris")
+    OBJECTIVE_VARIALBLE = 'species'  # Objective variable
+    USE_EXPLANATORY = ['petal_width', 'petal_length', 'sepal_width', 'sepal_length']  # Explantory variables
+    y = iris[OBJECTIVE_VARIALBLE].values
+    X = iris[USE_EXPLANATORY].values
+    fit_params = {'verbose': 0,
+                'early_stopping_rounds': 10,
+                'eval_metric': 'rmse',
+                'eval_set': [(X, y)]
+                }
+    # Plot ROC curve with cross validation in multiclass classification
+    estimator = LGBMClassifier(random_state=42, n_estimators=10000)
+    fig, axes = plt.subplots(4, 1, figsize=(6, 24))
+    classplot.roc_plot(estimator, X, y, ax=axes, cv=3, fit_params=fit_params)
+.. image:: https://user-images.githubusercontent.com/59557625/132708291-99f7bda0-eb24-4fc0-8994-a976d097908e.png
+   :width: 320px
+
+regplot.linear_plot
+===================
+.. code-block:: python
+
+    from seaborn_analyzer import regplot
+    import seaborn as sns
+    iris = sns.load_dataset("iris")
+    regplot.linear_plot(x='petal_length', y='sepal_length', data=iris)
+.. image:: https://user-images.githubusercontent.com/59557625/117276994-65243380-ae9a-11eb-8ec8-fa1fb5d60a55.png
+   :width: 320px
+
+regplot.regression_pred_true
+============================
+.. code-block:: python
+
+    import pandas as pd
+    from seaborn_analyzer import regplot
+    import seaborn as sns
+    from sklearn.linear_model import LinearRegression
+    df_temp = pd.read_csv(f'./sample_data/temp_pressure.csv')
+    regplot.regression_pred_true(LinearRegression(), x=['altitude', 'latitude'], y='temperature', data=df_temp)
+.. image:: https://user-images.githubusercontent.com/59557625/117277036-6fdec880-ae9a-11eb-887a-5f8b2a93b0f9.png
+   :width: 320px
+
+regplot.regression_plot_1d
+==========================
+.. code-block:: python
+
+    from seaborn_analyzer import regplot
+    import seaborn as sns
+    from sklearn.svm import SVR
+    iris = sns.load_dataset("iris")
+    regplot.regression_plot_1d(SVR(), x='petal_length', y='sepal_length', data=iris)
+.. image:: https://user-images.githubusercontent.com/59557625/117277075-78cf9a00-ae9a-11eb-835c-01f635754f7b.png
+   :width: 320px
+
+regplot.regression_heat_plot
+============================
+.. code-block:: python
+
+    import pandas as pd
+    from sklearn.linear_model import LinearRegression
+    from seaborn_analyzer import regplot
+    df_temp = pd.read_csv(f'./sample_data/temp_pressure.csv')
+    regplot.regression_heat_plot(LinearRegression(), x=['altitude', 'latitude'], y='temperature', data=df_temp)
+.. image:: https://user-images.githubusercontent.com/59557625/115955837-1b4f5b00-a534-11eb-91b0-b913019d26ff.png
+   :width: 320px
+
+regplot.average_plot
+============================
+.. code-block:: python
+
+    import seaborn as sns
+    from sklearn.svm import SVR
+    from seaborn_analyzer import regplot
+    iris = sns.load_dataset("iris")
+    svr = SVR()
+    features = ['petal_width', 'petal_length', 'sepal_width']
+    X = iris[features].values
+    y = iris['sepal_length'].values
+    regplot.average_plot(svr, X, y, x_colnames=features, cv=3)
+.. image:: https://user-images.githubusercontent.com/59557625/137940484-31f1fec7-012e-4c36-83a8-a1803755caa6.png
+   :width: 320px
```

### Comparing `seaborn-analyzer-0.2.9/seaborn_analyzer/_cv_eval_set.py` & `seaborn-analyzer-0.3.0/seaborn_analyzer/_cv_eval_set.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,1166 +1,1184 @@
-import copy
-from joblib import Parallel
-import numpy as np
-import time
-import numbers
-from itertools import product
-from collections import defaultdict
-from sklearn import clone
-from sklearn.pipeline import Pipeline
-from sklearn.model_selection import check_cv, GridSearchCV, RandomizedSearchCV
-from sklearn.model_selection._validation import _fit_and_score, _insert_error_scores, _aggregate_score_dicts, _normalize_score_results, _translate_train_sizes, _incremental_fit_estimator
-from sklearn.utils.validation import indexable, check_random_state, _check_fit_params
-from sklearn.metrics import check_scoring
-from sklearn.metrics._scorer import _check_multimetric_scoring
-from sklearn.base import is_classifier
-from sklearn.utils.fixes import delayed
-
-def init_eval_set(src_eval_set_selection, src_fit_params, X, y):
-        """
-        fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理
-        
-        Parameters
-        ----------
-        src_eval_set_selection : {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            eval_setに渡すデータの決め方 ('all': X, 'test': X[test], 'train': X[train], 'original': 入力そのまま, 'original_transformed': 入力そのまま＆パイプラインの時は最終学習器以外の変換実行)
-
-        src_fit_params : Dict
-            処理前の学習時パラメータ
-        """
-
-        fit_params = copy.deepcopy(src_fit_params)
-        eval_set_selection = src_eval_set_selection
-        # fit_paramsにeval_metricが設定されているときのみ以下の処理を実施
-        if 'eval_metric' in src_fit_params and src_fit_params['eval_metric'] is not None:
-            # fit_paramsにeval_setが存在しないとき、入力データをそのまま追加
-            if 'eval_set' not in src_fit_params:
-                print('There is no "eval_set" in fit_params, so "eval_set" is set to (self.X, self.y)')
-                fit_params['eval_set'] = [(X, y)]
-                if src_eval_set_selection is None:  # eval_set_selection未指定時、eval_setが入力されていなければeval_set_selection='test'とする
-                    eval_set_selection = 'test'
-                if eval_set_selection not in ['all', 'train', 'test']:  # eval_set_selectionの指定が間違っていたらエラーを出す
-                    raise ValueError('The `eval_set_selection` argument should be "all", "train", or "test" when `eval_set` is not in `fit_params`')
-            # src_fit_paramsにeval_setが存在するとき、eval_set_selection未指定ならばeval_set_selection='original_transformed'とする
-            else:
-                if src_eval_set_selection is None:
-                    eval_set_selection = 'original_transformed'
-
-        return fit_params, eval_set_selection
-
-def _transform_except_last_estimator(transformer, X_src, X_train):
-    """パイプラインのとき、最終学習器以外のtransformを適用"""
-    if transformer is not None:
-        transformer.fit(X_train)
-        X_dst = transformer.transform(X_src)
-        return X_dst
-    else:
-        return X_src
-
-def _eval_set_selection(eval_set_selection, transformer,
-                        fit_params, train, test):
-    """eval_setの中から学習データ or テストデータのみを抽出"""
-    fit_params_modified = copy.deepcopy(fit_params)
-    # eval_setが存在しない or Noneなら、そのままfit_paramsを返す
-    eval_sets = [v for v in fit_params.keys() if 'eval_set' in v]
-    if len(eval_sets) == 0 or fit_params[eval_sets[0]] is None:
-        return fit_params_modified
-    eval_set_name = eval_sets[0]  # eval_setの列名(pipelineでは列名が変わるため)
-    # 元のeval_setからX, yを取得
-    X_fit = fit_params[eval_set_name][0][0]
-    y_fit = fit_params[eval_set_name][0][1]
-    # eval_setに該当データを入力し直す
-    if eval_set_selection == 'train':
-        fit_params_modified[eval_set_name] = [(_transform_except_last_estimator(transformer, X_fit[train], X_fit[train])\
-                                              , y_fit[train])]
-    elif eval_set_selection == 'test':
-        fit_params_modified[eval_set_name] = [(_transform_except_last_estimator(transformer, X_fit[test], X_fit[train])\
-                                              , y_fit[test])]
-    elif eval_set_selection == 'all':
-        fit_params_modified[eval_set_name] = [(_transform_except_last_estimator(transformer, X_fit, X_fit[train])\
-                                              , y_fit)]
-    else:
-        fit_params_modified[eval_set_name] = [(_transform_except_last_estimator(transformer, X_fit, X_fit)\
-                                              , y_fit)]
-    return fit_params_modified
-
-def _fit_and_score_eval_set(eval_set_selection, transformer,
-                            estimator, X, y, scorer, train, test, verbose,
-                            parameters, fit_params, return_train_score=False,
-                            return_parameters=False, return_n_test_samples=False,
-                            return_times=False, return_estimator=False,
-                            split_progress=None, candidate_progress=None,
-                            error_score=np.nan,
-                            print_message=None):
-
-    """Fit estimator and compute scores for a given dataset split."""
-    # eval_setの中から学習データ or テストデータのみを抽出
-    fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
-                                              fit_params, train, test)
-    if print_message is not None:
-        print(print_message)
-    # 学習してスコア計算
-    result = _fit_and_score(estimator, X, y, scorer, train, test, verbose, parameters,
-                            fit_params_modified,
-                            return_train_score=return_train_score,
-                            return_parameters=return_parameters, return_n_test_samples=return_n_test_samples,
-                            return_times=return_times, return_estimator=return_estimator,
-                            split_progress=split_progress, candidate_progress=candidate_progress,
-                            error_score=error_score)
-    return result
-
-def _make_transformer(eval_set_selection, estimator):
-    """estimatorがパイプラインのとき、最終学習器以外の変換器(前処理クラスのリスト)を作成"""
-    if isinstance(estimator, Pipeline) and eval_set_selection != 'original':
-        transformer = Pipeline([step for i, step in enumerate(estimator.steps) if i < len(estimator) - 1])
-        return transformer
-    else:
-        return None
-
-def cross_validate_eval_set(eval_set_selection,
-                            estimator, X, y=None, groups=None, scoring=None, cv=None,
-                            n_jobs=None, verbose=0, fit_params=None,
-                            pre_dispatch='2*n_jobs', return_train_score=False,
-                            return_estimator=False, error_score=np.nan):
-    """
-    Evaluate a scores by cross-validation with `eval_set` argument in `fit_params`
-
-    This method is suitable for calculating cross validation scores with `early_stopping_round` in XGBoost or LightGBM.
-
-    Parameters
-    ----------
-    eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
-        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-        If "all", use all data in `X` and `y`.
-
-        If "train", select train data from `X` and `y` using cv.split().
-
-        If "test", select test data from `X` and `y` using cv.split().
-
-        If "original", use raw `eval_set`.
-
-        If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
-
-    estimator : estimator object implementing 'fit'
-        The object to use to fit the data.
-
-    X : array-like of shape (n_samples, n_features)
-        The data to fit. Can be for example a list, or an array.
-
-    y : array-like of shape (n_samples,) or (n_samples, n_outputs), \
-            default=None
-        The target variable to try to predict in the case of
-        supervised learning.
-
-    groups : array-like of shape (n_samples,), default=None
-        Group labels for the samples used while splitting the dataset into
-        train/test set. Only used in conjunction with a "Group" :term:`cv`
-        instance (e.g., :class:`GroupKFold`).
-
-    scoring : str, callable, list, tuple, or dict, default=None
-        Strategy to evaluate the performance of the cross-validated model on
-        the test set.
-
-        If `scoring` represents a single score, one can use:
-
-        - a single string (see :ref:`scoring_parameter`);
-        - a callable (see :ref:`scoring`) that returns a single value.
-
-        If `scoring` represents multiple scores, one can use:
-
-        - a list or tuple of unique strings;
-        - a callable returning a dictionary where the keys are the metric
-          names and the values are the metric scores;
-        - a dictionary with metric names as keys and callables a values.
-
-        See :ref:`multimetric_grid_search` for an example.
-
-    cv : int, cross-validation generator or an iterable, default=None
-        Determines the cross-validation splitting strategy.
-        Possible inputs for cv are:
-
-        - None, to use the default 5-fold cross validation,
-        - int, to specify the number of folds in a `(Stratified)KFold`,
-        - :term:`CV splitter`,
-        - An iterable yielding (train, test) splits as arrays of indices.
-
-        For int/None inputs, if the estimator is a classifier and ``y`` is
-        either binary or multiclass, :class:`StratifiedKFold` is used. In all
-        other cases, :class:`.Fold` is used. These splitters are instantiated
-        with `shuffle=False` so the splits will be the same across calls.
-
-        Refer :ref:`User Guide <cross_validation>` for the various
-        cross-validation strategies that can be used here.
-
-        .. versionchanged:: 0.22
-            ``cv`` default value if None changed from 3-fold to 5-fold.
-
-    n_jobs : int, default=None
-        Number of jobs to run in parallel. Training the estimator and computing
-        the score are parallelized over the cross-validation splits.
-        ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
-        ``-1`` means using all processors. See :term:`Glossary <n_jobs>`
-        for more details.
-
-    verbose : int, default=0
-        The verbosity level.
-
-    fit_params : dict, default=None
-        Parameters to pass to the fit method of the estimator.
-
-    pre_dispatch : int or str, default='2*n_jobs'
-        Controls the number of jobs that get dispatched during parallel
-        execution. Reducing this number can be useful to avoid an
-        explosion of memory consumption when more jobs get dispatched
-        than CPUs can process. This parameter can be:
-
-            - None, in which case all the jobs are immediately
-              created and spawned. Use this for lightweight and
-              fast-running jobs, to avoid delays due to on-demand
-              spawning of the jobs
-
-            - An int, giving the exact number of total jobs that are
-              spawned
-
-            - A str, giving an expression as a function of n_jobs,
-              as in '2*n_jobs'
-
-    return_train_score : bool, default=False
-        Whether to include train scores.
-        Computing training scores is used to get insights on how different
-        parameter settings impact the overfitting/underfitting trade-off.
-        However computing the scores on the training set can be computationally
-        expensive and is not strictly required to select the parameters that
-        yield the best generalization performance.
-
-        .. versionadded:: 0.19
-
-        .. versionchanged:: 0.21
-            Default value was changed from ``True`` to ``False``
-
-    return_estimator : bool, default=False
-        Whether to return the estimators fitted on each split.
-
-        .. versionadded:: 0.20
-
-    error_score : 'raise' or numeric, default=np.nan
-        Value to assign to the score if an error occurs in estimator fitting.
-        If set to 'raise', the error is raised.
-        If a numeric value is given, FitFailedWarning is raised.
-
-        .. versionadded:: 0.20
-
-    Returns
-    -------
-    scores : dict of float arrays of shape (n_splits,)
-        Array of scores of the estimator for each run of the cross validation.
-    """
-
-    X, y, groups = indexable(X, y, groups)
-
-    cv = check_cv(cv, y, classifier=is_classifier(estimator))
-
-    if callable(scoring):
-        scorers = scoring
-    elif scoring is None or isinstance(scoring, str):
-        scorers = check_scoring(estimator, scoring)
-    else:
-        scorers = _check_multimetric_scoring(estimator, scoring)
-
-    # 最終学習器以外の前処理変換器作成
-    transformer = _make_transformer(eval_set_selection, estimator)
-
-    # We clone the estimator to make sure that all the folds are
-    # independent, and that it is pickle-able.
-    parallel = Parallel(n_jobs=n_jobs, verbose=verbose,
-                        pre_dispatch=pre_dispatch)
-    results = parallel(
-        delayed(_fit_and_score_eval_set)(
-            eval_set_selection, transformer,
-            clone(estimator), X, y, scorers, train, test, verbose, None,
-            fit_params, return_train_score=return_train_score,
-            return_times=True, return_estimator=return_estimator,
-            error_score=error_score)
-        for train, test in cv.split(X, y, groups))
-
-    # For callabe scoring, the return type is only know after calling. If the
-    # return type is a dictionary, the error scores can now be inserted with
-    # the correct key.
-    if callable(scoring):
-        _insert_error_scores(results, error_score)
-
-    results = _aggregate_score_dicts(results)
-
-    ret = {}
-    ret['fit_time'] = results["fit_time"]
-    ret['score_time'] = results["score_time"]
-
-    if return_estimator:
-        ret['estimator'] = results["estimator"]
-
-    test_scores_dict = _normalize_score_results(results["test_scores"])
-    if return_train_score:
-        train_scores_dict = _normalize_score_results(results["train_scores"])
-
-    for name in test_scores_dict:
-        ret['test_%s' % name] = test_scores_dict[name]
-        if return_train_score:
-            key = 'train_%s' % name
-            ret[key] = train_scores_dict[name]
-
-    return ret
-
-def cross_val_score_eval_set(eval_set_selection,
-                             estimator, X, y=None, groups=None, scoring=None,
-                             cv=None, n_jobs=None, verbose=0, fit_params=None,
-                             pre_dispatch='2*n_jobs', error_score=np.nan):
-    """
-    Evaluate a score by cross-validation with `eval_set` argument in `fit_params`
-
-    This method is suitable for calculating cross validation score with `early_stopping_round` in XGBoost or LightGBM.
-
-    Parameters
-    ----------
-    eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
-        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-        If "all", use all data in `X` and `y`.
-
-        If "train", select train data from `X` and `y` using cv.split().
-
-        If "test", select test data from `X` and `y` using cv.split().
-
-        If "original", use raw `eval_set`.
-
-        If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
-    
-    estimator : estimator object implementing 'fit'
-        The object to use to fit the data.
-
-    X : array-like of shape (n_samples, n_features)
-        The data to fit. Can be for example a list, or an array.
-
-    y : array-like of shape (n_samples,) or (n_samples, n_outputs), \
-            default=None
-        The target variable to try to predict in the case of
-        supervised learning.
-
-    groups : array-like of shape (n_samples,), default=None
-        Group labels for the samples used while splitting the dataset into
-        train/test set. Only used in conjunction with a "Group" :term:`cv`
-        instance (e.g., :class:`GroupKFold`).
-
-    scoring : str or callable, default=None
-        A str (see model evaluation documentation) or
-        a scorer callable object / function with signature
-        ``scorer(estimator, X, y)`` which should return only
-        a single value.
-
-        Similar to :func:`cross_validate`
-        but only a single metric is permitted.
-
-        If None, the estimator's default scorer (if available) is used.
-
-    cv : int, cross-validation generator or an iterable, default=None
-        Determines the cross-validation splitting strategy.
-        Possible inputs for cv are:
-
-        - None, to use the default 5-fold cross validation,
-        - int, to specify the number of folds in a `(Stratified)KFold`,
-        - :term:`CV splitter`,
-        - An iterable yielding (train, test) splits as arrays of indices.
-
-        For int/None inputs, if the estimator is a classifier and ``y`` is
-        either binary or multiclass, :class:`StratifiedKFold` is used. In all
-        other cases, :class:`KFold` is used. These splitters are instantiated
-        with `shuffle=False` so the splits will be the same across calls.
-
-        Refer :ref:`User Guide <cross_validation>` for the various
-        cross-validation strategies that can be used here.
-
-        .. versionchanged:: 0.22
-            ``cv`` default value if None changed from 3-fold to 5-fold.
-
-    n_jobs : int, default=None
-        Number of jobs to run in parallel. Training the estimator and computing
-        the score are parallelized over the cross-validation splits.
-        ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
-        ``-1`` means using all processors. See :term:`Glossary <n_jobs>`
-        for more details.
-
-    verbose : int, default=0
-        The verbosity level.
-
-    fit_params : dict, default=None
-        Parameters to pass to the fit method of the estimator.
-
-    pre_dispatch : int or str, default='2*n_jobs'
-        Controls the number of jobs that get dispatched during parallel
-        execution. Reducing this number can be useful to avoid an
-        explosion of memory consumption when more jobs get dispatched
-        than CPUs can process. This parameter can be:
-
-            - None, in which case all the jobs are immediately
-              created and spawned. Use this for lightweight and
-              fast-running jobs, to avoid delays due to on-demand
-              spawning of the jobs
-
-            - An int, giving the exact number of total jobs that are
-              spawned
-
-            - A str, giving an expression as a function of n_jobs,
-              as in '2*n_jobs'
-
-    error_score : 'raise' or numeric, default=np.nan
-        Value to assign to the score if an error occurs in estimator fitting.
-        If set to 'raise', the error is raised.
-        If a numeric value is given, FitFailedWarning is raised.
-
-        .. versionadded:: 0.20
-
-    Returns
-    -------
-    scores : ndarray of float of shape=(len(list(cv)),)
-        Array of scores of the estimator for each run of the cross validation.
-    """
-    # To ensure multimetric format is not supported
-    scorer = check_scoring(estimator, scoring=scoring)
-
-    cv_results = cross_validate_eval_set(eval_set_selection=eval_set_selection,
-                                         estimator=estimator, X=X, y=y, groups=groups,
-                                         scoring={'score': scorer}, cv=cv,
-                                         n_jobs=n_jobs, verbose=verbose,
-                                         fit_params=fit_params,
-                                         pre_dispatch=pre_dispatch,
-                                         error_score=error_score)
-    return cv_results['test_score']
-
-def validation_curve_eval_set(eval_set_selection,
-                              estimator, X, y, param_name, param_range, groups=None,
-                              cv=None, scoring=None, n_jobs=None, pre_dispatch="all",
-                              verbose=0, error_score=np.nan, fit_params=None):
-    """Validation curve.
-
-    Determine training and test scores for varying parameter values with `eval_set` argument in `fit_params`
-
-    Parameters
-    ----------
-    eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
-        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-        If "all", use all data in `X` and `y`.
-
-        If "train", select train data from `X` and `y` using cv.split().
-
-        If "test", select test data from `X` and `y` using cv.split().
-
-        If "original", use raw `eval_set`.
-
-        If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
-    
-    estimator : object type that implements the "fit" and "predict" methods
-        An object of that type which is cloned for each validation.
-
-    X : array-like of shape (n_samples, n_features)
-        Training vector, where n_samples is the number of samples and
-        n_features is the number of features.
-
-    y : array-like of shape (n_samples,) or (n_samples, n_outputs) or None
-        Target relative to X for classification or regression;
-        None for unsupervised learning.
-
-    param_name : str
-        Name of the parameter that will be varied.
-
-    param_range : array-like of shape (n_values,)
-        The values of the parameter that will be evaluated.
-
-    groups : array-like of shape (n_samples,), default=None
-        Group labels for the samples used while splitting the dataset into
-        train/test set. Only used in conjunction with a "Group" :term:`cv`
-        instance (e.g., :class:`GroupKFold`).
-
-    cv : int, cross-validation generator or an iterable, default=None
-        Determines the cross-validation splitting strategy.
-        Possible inputs for cv are:
-
-        - None, to use the default 5-fold cross validation,
-        - int, to specify the number of folds in a `(Stratified)KFold`,
-        - :term:`CV splitter`,
-        - An iterable yielding (train, test) splits as arrays of indices.
-
-        For int/None inputs, if the estimator is a classifier and ``y`` is
-        either binary or multiclass, :class:`StratifiedKFold` is used. In all
-        other cases, :class:`KFold` is used. These splitters are instantiated
-        with `shuffle=False` so the splits will be the same across calls.
-
-        Refer :ref:`User Guide <cross_validation>` for the various
-        cross-validation strategies that can be used here.
-
-        .. versionchanged:: 0.22
-            ``cv`` default value if None changed from 3-fold to 5-fold.
-
-    scoring : str or callable, default=None
-        A str (see model evaluation documentation) or
-        a scorer callable object / function with signature
-        ``scorer(estimator, X, y)``.
-
-    n_jobs : int, default=None
-        Number of jobs to run in parallel. Training the estimator and computing
-        the score are parallelized over the combinations of each parameter
-        value and each cross-validation split.
-        ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
-        ``-1`` means using all processors. See :term:`Glossary <n_jobs>`
-        for more details.
-
-    pre_dispatch : int or str, default='all'
-        Number of predispatched jobs for parallel execution (default is
-        all). The option can reduce the allocated memory. The str can
-        be an expression like '2*n_jobs'.
-
-    verbose : int, default=0
-        Controls the verbosity: the higher, the more messages.
-
-    fit_params : dict, default=None
-        Parameters to pass to the fit method of the estimator.
-
-        .. versionadded:: 0.24
-
-    error_score : 'raise' or numeric, default=np.nan
-        Value to assign to the score if an error occurs in estimator fitting.
-        If set to 'raise', the error is raised.
-        If a numeric value is given, FitFailedWarning is raised.
-
-        .. versionadded:: 0.20
-
-    Returns
-    -------
-    train_scores : array of shape (n_ticks, n_cv_folds)
-        Scores on training sets.
-
-    test_scores : array of shape (n_ticks, n_cv_folds)
-        Scores on test set.
-    """
-    X, y, groups = indexable(X, y, groups)
-
-    cv = check_cv(cv, y, classifier=is_classifier(estimator))
-    scorer = check_scoring(estimator, scoring=scoring)
-
-    # 最終学習器以外の前処理変換器作成
-    transformer = _make_transformer(eval_set_selection, estimator)
-
-    parallel = Parallel(n_jobs=n_jobs, pre_dispatch=pre_dispatch,
-                        verbose=verbose)
-    results = parallel(delayed(_fit_and_score_eval_set)(
-        eval_set_selection, transformer,
-        clone(estimator), X, y, scorer, train, test, verbose,
-        parameters={param_name: v}, fit_params=fit_params,
-        return_train_score=True, error_score=error_score,
-        print_message=f'Caluculating score. {param_name}={v}')
-
-        # NOTE do not change order of iteration to allow one time cv splitters
-        for train, test in cv.split(X, y, groups) for v in param_range)
-    n_params = len(param_range)
-
-    results = _aggregate_score_dicts(results)
-    train_scores = results["train_scores"].reshape(-1, n_params).T
-    test_scores = results["test_scores"].reshape(-1, n_params).T
-
-    return train_scores, test_scores
-
-def learning_curve_eval_set(eval_set_selection,
-                            estimator, X, y, groups=None,
-                            train_sizes=np.linspace(0.1, 1.0, 5), cv=None,
-                            scoring=None, exploit_incremental_learning=False,
-                            n_jobs=None, pre_dispatch="all", verbose=0, shuffle=False,
-                            random_state=None, error_score=np.nan, return_times=False,
-                            fit_params=None):
-    """Learning curve.
-
-    Determines cross-validated training and test scores for different training set sizes with `eval_set` argument in `fit_params`
-
-    Parameters
-    ----------
-    eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
-        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-        If "all", use all data in `X` and `y`.
-
-        If "train", select train data from `X` and `y` using cv.split().
-
-        If "test", select test data from `X` and `y` using cv.split().
-
-        If "original", use raw `eval_set`.
-
-        If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
-    
-    estimator : object type that implements the "fit" and "predict" methods
-        An object of that type which is cloned for each validation.
-
-    X : array-like of shape (n_samples, n_features)
-        Training vector, where n_samples is the number of samples and
-        n_features is the number of features.
-
-    y : array-like of shape (n_samples,) or (n_samples, n_outputs)
-        Target relative to X for classification or regression;
-        None for unsupervised learning.
-
-    groups : array-like of  shape (n_samples,), default=None
-        Group labels for the samples used while splitting the dataset into
-        train/test set. Only used in conjunction with a "Group" :term:`cv`
-        instance (e.g., :class:`GroupKFold`).
-
-    train_sizes : array-like of shape (n_ticks,), \
-            default=np.linspace(0.1, 1.0, 5)
-        Relative or absolute numbers of training examples that will be used to
-        generate the learning curve. If the dtype is float, it is regarded as a
-        fraction of the maximum size of the training set (that is determined
-        by the selected validation method), i.e. it has to be within (0, 1].
-        Otherwise it is interpreted as absolute sizes of the training sets.
-        Note that for classification the number of samples usually have to
-        be big enough to contain at least one sample from each class.
-
-    cv : int, cross-validation generator or an iterable, default=None
-        Determines the cross-validation splitting strategy.
-        Possible inputs for cv are:
-
-        - None, to use the default 5-fold cross validation,
-        - int, to specify the number of folds in a `(Stratified)KFold`,
-        - :term:`CV splitter`,
-        - An iterable yielding (train, test) splits as arrays of indices.
-
-        For int/None inputs, if the estimator is a classifier and ``y`` is
-        either binary or multiclass, :class:`StratifiedKFold` is used. In all
-        other cases, :class:`KFold` is used. These splitters are instantiated
-        with `shuffle=False` so the splits will be the same across calls.
-
-        Refer :ref:`User Guide <cross_validation>` for the various
-        cross-validation strategies that can be used here.
-
-        .. versionchanged:: 0.22
-            ``cv`` default value if None changed from 3-fold to 5-fold.
-
-    scoring : str or callable, default=None
-        A str (see model evaluation documentation) or
-        a scorer callable object / function with signature
-        ``scorer(estimator, X, y)``.
-
-    exploit_incremental_learning : bool, default=False
-        If the estimator supports incremental learning, this will be
-        used to speed up fitting for different training set sizes.
-
-    n_jobs : int, default=None
-        Number of jobs to run in parallel. Training the estimator and computing
-        the score are parallelized over the different training and test sets.
-        ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
-        ``-1`` means using all processors. See :term:`Glossary <n_jobs>`
-        for more details.
-
-    pre_dispatch : int or str, default='all'
-        Number of predispatched jobs for parallel execution (default is
-        all). The option can reduce the allocated memory. The str can
-        be an expression like '2*n_jobs'.
-
-    verbose : int, default=0
-        Controls the verbosity: the higher, the more messages.
-
-    shuffle : bool, default=False
-        Whether to shuffle training data before taking prefixes of it
-        based on``train_sizes``.
-
-    random_state : int, RandomState instance or None, default=None
-        Used when ``shuffle`` is True. Pass an int for reproducible
-        output across multiple function calls.
-        See :term:`Glossary <random_state>`.
-
-    error_score : 'raise' or numeric, default=np.nan
-        Value to assign to the score if an error occurs in estimator fitting.
-        If set to 'raise', the error is raised.
-        If a numeric value is given, FitFailedWarning is raised.
-
-        .. versionadded:: 0.20
-
-    return_times : bool, default=False
-        Whether to return the fit and score times.
-
-    fit_params : dict, default=None
-        Parameters to pass to the fit method of the estimator.
-
-        .. versionadded:: 0.24
-
-    Returns
-    -------
-    train_sizes_abs : array of shape (n_unique_ticks,)
-        Numbers of training examples that has been used to generate the
-        learning curve. Note that the number of ticks might be less
-        than n_ticks because duplicate entries will be removed.
-
-    train_scores : array of shape (n_ticks, n_cv_folds)
-        Scores on training sets.
-
-    test_scores : array of shape (n_ticks, n_cv_folds)
-        Scores on test set.
-
-    fit_times : array of shape (n_ticks, n_cv_folds)
-        Times spent for fitting in seconds. Only present if ``return_times``
-        is True.
-
-    score_times : array of shape (n_ticks, n_cv_folds)
-        Times spent for scoring in seconds. Only present if ``return_times``
-        is True.
-    """
-    if exploit_incremental_learning and not hasattr(estimator, "partial_fit"):
-        raise ValueError("An estimator must support the partial_fit interface "
-                         "to exploit incremental learning")
-    X, y, groups = indexable(X, y, groups)
-
-    cv = check_cv(cv, y, classifier=is_classifier(estimator))
-    # Store it as list as we will be iterating over the list multiple times
-    cv_iter = list(cv.split(X, y, groups))
-
-    scorer = check_scoring(estimator, scoring=scoring)
-
-    n_max_training_samples = len(cv_iter[0][0])
-    # Because the lengths of folds can be significantly different, it is
-    # not guaranteed that we use all of the available training data when we
-    # use the first 'n_max_training_samples' samples.
-    train_sizes_abs = _translate_train_sizes(train_sizes,
-                                             n_max_training_samples)
-    n_unique_ticks = train_sizes_abs.shape[0]
-    if verbose > 0:
-        print("[learning_curve] Training set sizes: " + str(train_sizes_abs))
-
-    # 最終学習器以外の前処理変換器作成
-    transformer = _make_transformer(eval_set_selection, estimator)
-
-    parallel = Parallel(n_jobs=n_jobs, pre_dispatch=pre_dispatch,
-                        verbose=verbose)
-
-    if shuffle:
-        rng = check_random_state(random_state)
-        cv_iter = ((rng.permutation(train), test) for train, test in cv_iter)
-
-    if exploit_incremental_learning:
-        classes = np.unique(y) if is_classifier(estimator) else None
-        out = parallel(delayed(_incremental_fit_estimator)(
-            clone(estimator), X, y, classes, train, test, train_sizes_abs,
-            scorer, verbose, return_times, error_score=error_score,
-            fit_params=fit_params)
-            for train, test in cv_iter
-        )
-        out = np.asarray(out).transpose((2, 1, 0))
-    else:
-        train_test_proportions = []
-        for train, test in cv_iter:
-            for n_train_samples in train_sizes_abs:
-                train_test_proportions.append((train[:n_train_samples], test))
-
-        results = parallel(delayed(_fit_and_score_eval_set)(
-            eval_set_selection, transformer,
-            clone(estimator), X, y, scorer, train, test, verbose,
-            parameters=None, fit_params=fit_params, return_train_score=True,
-            error_score=error_score, return_times=return_times)
-            for train, test in train_test_proportions
-        )
-        results = _aggregate_score_dicts(results)
-        train_scores = results["train_scores"].reshape(-1, n_unique_ticks).T
-        test_scores = results["test_scores"].reshape(-1, n_unique_ticks).T
-        out = [train_scores, test_scores]
-
-        if return_times:
-            fit_times = results["fit_time"].reshape(-1, n_unique_ticks).T
-            score_times = results["score_time"].reshape(-1, n_unique_ticks).T
-            out.extend([fit_times, score_times])
-
-    ret = train_sizes_abs, out[0], out[1]
-
-    if return_times:
-        ret = ret + (out[2], out[3])
-
-    return ret
-
-class GridSearchCVEvalSet(GridSearchCV):
-    """
-    Exhaustive search over specified parameter values for an estimator with `eval_set` argument in `fit_params`.
-    """
-    def fit(self, eval_set_selection,
-            X, y=None, groups=None, **fit_params):
-        """Run fit with all sets of parameters.
-
-        Parameters
-        ----------
-        eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
-            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-                
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
-
-            If "test", select test data from `X` and `y` using cv.split().
-
-            If "original", use raw `eval_set`.
-
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
-
-        X : array-like of shape (n_samples, n_features)
-            Training vector, where n_samples is the number of samples and
-            n_features is the number of features.
-
-        y : array-like of shape (n_samples, n_output) \
-            or (n_samples,), default=None
-            Target relative to X for classification or regression;
-            None for unsupervised learning.
-
-        groups : array-like of shape (n_samples,), default=None
-            Group labels for the samples used while splitting the dataset into
-            train/test set. Only used in conjunction with a "Group" :term:`cv`
-            instance (e.g., :class:`~sklearn.model_selection.GroupKFold`).
-
-        **fit_params : dict of str -> object
-            Parameters passed to the ``fit`` method of the estimator
-        """
-        estimator = self.estimator
-        refit_metric = "score"
-
-        if callable(self.scoring):
-            scorers = self.scoring
-        elif self.scoring is None or isinstance(self.scoring, str):
-            scorers = check_scoring(self.estimator, self.scoring)
-        else:
-            scorers = _check_multimetric_scoring(self.estimator, self.scoring)
-            self._check_refit_for_multimetric(scorers)
-            refit_metric = self.refit
-
-        X, y, groups = indexable(X, y, groups)
-        fit_params = _check_fit_params(X, fit_params)
-
-        cv_orig = check_cv(self.cv, y, classifier=is_classifier(estimator))
-        n_splits = cv_orig.get_n_splits(X, y, groups)
-
-        base_estimator = clone(self.estimator)
-
-        # 最終学習器以外の前処理変換器作成
-        transformer = _make_transformer(eval_set_selection, estimator)
-
-        parallel = Parallel(n_jobs=self.n_jobs,
-                            pre_dispatch=self.pre_dispatch)
-
-        fit_and_score_kwargs = dict(scorer=scorers,
-                                    fit_params=fit_params,
-                                    return_train_score=self.return_train_score,
-                                    return_n_test_samples=True,
-                                    return_times=True,
-                                    return_parameters=False,
-                                    error_score=self.error_score,
-                                    verbose=self.verbose)
-        results = {}
-        with parallel:
-            all_candidate_params = []
-            all_out = []
-            all_more_results = defaultdict(list)
-
-            def evaluate_candidates(candidate_params, cv=None,
-                                    more_results=None):
-                cv = cv or cv_orig
-                candidate_params = list(candidate_params)
-                n_candidates = len(candidate_params)
-
-                if self.verbose > 0:
-                    print("Fitting {0} folds for each of {1} candidates,"
-                          " totalling {2} fits".format(
-                              n_splits, n_candidates, n_candidates * n_splits))
-
-                out = parallel(delayed(_fit_and_score_eval_set)(
-                                        eval_set_selection, transformer,
-                                        clone(base_estimator),
-                                        X, y,
-                                        train=train, test=test,
-                                        parameters=parameters,
-                                        split_progress=(
-                                            split_idx,
-                                            n_splits),
-                                        candidate_progress=(
-                                            cand_idx,
-                                            n_candidates),
-                                        print_message=f'cand={cand_idx}/{n_candidates}, cv={split_idx}: {parameters}',
-                                        **fit_and_score_kwargs)
-                               for (cand_idx, parameters),
-                                   (split_idx, (train, test)) in product(
-                                   enumerate(candidate_params),
-                                   enumerate(cv.split(X, y, groups))))
-
-                if len(out) < 1:
-                    raise ValueError('No fits were performed. '
-                                     'Was the CV iterator empty? '
-                                     'Were there no candidates?')
-                elif len(out) != n_candidates * n_splits:
-                    raise ValueError('cv.split and cv.get_n_splits returned '
-                                     'inconsistent results. Expected {} '
-                                     'splits, got {}'
-                                     .format(n_splits,
-                                             len(out) // n_candidates))
-
-                # For callable self.scoring, the return type is only know after
-                # calling. If the return type is a dictionary, the error scores
-                # can now be inserted with the correct key. The type checking
-                # of out will be done in `_insert_error_scores`.
-                if callable(self.scoring):
-                    _insert_error_scores(out, self.error_score)
-                all_candidate_params.extend(candidate_params)
-                all_out.extend(out)
-                if more_results is not None:
-                    for key, value in more_results.items():
-                        all_more_results[key].extend(value)
-
-                nonlocal results
-                results = self._format_results(
-                    all_candidate_params, n_splits, all_out,
-                    all_more_results)
-
-                return results
-
-            self._run_search(evaluate_candidates)
-
-            # multimetric is determined here because in the case of a callable
-            # self.scoring the return type is only known after calling
-            first_test_score = all_out[0]['test_scores']
-            self.multimetric_ = isinstance(first_test_score, dict)
-
-            # check refit_metric now for a callabe scorer that is multimetric
-            if callable(self.scoring) and self.multimetric_:
-                self._check_refit_for_multimetric(first_test_score)
-                refit_metric = self.refit
-
-        # For multi-metric evaluation, store the best_index_, best_params_ and
-        # best_score_ iff refit is one of the scorer names
-        # In single metric evaluation, refit_metric is "score"
-        if self.refit or not self.multimetric_:
-            # If callable, refit is expected to return the index of the best
-            # parameter set.
-            if callable(self.refit):
-                self.best_index_ = self.refit(results)
-                if not isinstance(self.best_index_, numbers.Integral):
-                    raise TypeError('best_index_ returned is not an integer')
-                if (self.best_index_ < 0 or
-                   self.best_index_ >= len(results["params"])):
-                    raise IndexError('best_index_ index out of range')
-            else:
-                self.best_index_ = results["rank_test_%s"
-                                           % refit_metric].argmin()
-                self.best_score_ = results["mean_test_%s" % refit_metric][
-                                           self.best_index_]
-            self.best_params_ = results["params"][self.best_index_]
-
-        if self.refit:
-            # we clone again after setting params in case some
-            # of the params are estimators as well.
-            self.best_estimator_ = clone(clone(base_estimator).set_params(
-                **self.best_params_))
-            refit_start_time = time.time()
-            if y is not None:
-                self.best_estimator_.fit(X, y, **fit_params)
-            else:
-                self.best_estimator_.fit(X, **fit_params)
-            refit_end_time = time.time()
-            self.refit_time_ = refit_end_time - refit_start_time
-
-        # Store the only scorer not as a dict for single metric evaluation
-        self.scorer_ = scorers
-
-        self.cv_results_ = results
-        self.n_splits_ = n_splits
-
-        return self
-
-class RandomizedSearchCVEvalSet(RandomizedSearchCV):
-    """
-    Randomized search on hyper parameters with `eval_set` argument in `fit_params`.
-    """
-    def fit(self, eval_set_selection,
-            X, y=None, groups=None, **fit_params):
-        """Run fit with all sets of parameters.
-
-        Parameters
-        ----------
-        eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
-            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
-
-            If "test", select test data from `X` and `y` using cv.split().
-
-            If "original", use raw `eval_set`.
-
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
-
-        X : array-like of shape (n_samples, n_features)
-            Training vector, where n_samples is the number of samples and
-            n_features is the number of features.
-
-        y : array-like of shape (n_samples, n_output) \
-            or (n_samples,), default=None
-            Target relative to X for classification or regression;
-            None for unsupervised learning.
-
-        groups : array-like of shape (n_samples,), default=None
-            Group labels for the samples used while splitting the dataset into
-            train/test set. Only used in conjunction with a "Group" :term:`cv`
-            instance (e.g., :class:`~sklearn.model_selection.GroupKFold`).
-
-        **fit_params : dict of str -> object
-            Parameters passed to the ``fit`` method of the estimator
-        """
-        estimator = self.estimator
-        refit_metric = "score"
-
-        if callable(self.scoring):
-            scorers = self.scoring
-        elif self.scoring is None or isinstance(self.scoring, str):
-            scorers = check_scoring(self.estimator, self.scoring)
-        else:
-            scorers = _check_multimetric_scoring(self.estimator, self.scoring)
-            self._check_refit_for_multimetric(scorers)
-            refit_metric = self.refit
-
-        X, y, groups = indexable(X, y, groups)
-        fit_params = _check_fit_params(X, fit_params)
-
-        cv_orig = check_cv(self.cv, y, classifier=is_classifier(estimator))
-        n_splits = cv_orig.get_n_splits(X, y, groups)
-
-        base_estimator = clone(self.estimator)
-
-        # 最終学習器以外の前処理変換器作成
-        transformer = _make_transformer(eval_set_selection, estimator)
-
-        parallel = Parallel(n_jobs=self.n_jobs,
-                            pre_dispatch=self.pre_dispatch)
-
-        fit_and_score_kwargs = dict(scorer=scorers,
-                                    fit_params=fit_params,
-                                    return_train_score=self.return_train_score,
-                                    return_n_test_samples=True,
-                                    return_times=True,
-                                    return_parameters=False,
-                                    error_score=self.error_score,
-                                    verbose=self.verbose)
-        results = {}
-        with parallel:
-            all_candidate_params = []
-            all_out = []
-            all_more_results = defaultdict(list)
-
-            def evaluate_candidates(candidate_params, cv=None,
-                                    more_results=None):
-                cv = cv or cv_orig
-                candidate_params = list(candidate_params)
-                n_candidates = len(candidate_params)
-
-                if self.verbose > 0:
-                    print("Fitting {0} folds for each of {1} candidates,"
-                          " totalling {2} fits".format(
-                              n_splits, n_candidates, n_candidates * n_splits))
-
-                out = parallel(delayed(_fit_and_score_eval_set)(
-                                        eval_set_selection, transformer,
-                                        clone(base_estimator),
-                                        X, y,
-                                        train=train, test=test,
-                                        parameters=parameters,
-                                        split_progress=(
-                                            split_idx,
-                                            n_splits),
-                                        candidate_progress=(
-                                            cand_idx,
-                                            n_candidates),
-                                        print_message=f'cand={cand_idx}/{n_candidates}, cv={split_idx}: {parameters}',
-                                        **fit_and_score_kwargs)
-                               for (cand_idx, parameters),
-                                   (split_idx, (train, test)) in product(
-                                   enumerate(candidate_params),
-                                   enumerate(cv.split(X, y, groups))))
-
-                if len(out) < 1:
-                    raise ValueError('No fits were performed. '
-                                     'Was the CV iterator empty? '
-                                     'Were there no candidates?')
-                elif len(out) != n_candidates * n_splits:
-                    raise ValueError('cv.split and cv.get_n_splits returned '
-                                     'inconsistent results. Expected {} '
-                                     'splits, got {}'
-                                     .format(n_splits,
-                                             len(out) // n_candidates))
-
-                # For callable self.scoring, the return type is only know after
-                # calling. If the return type is a dictionary, the error scores
-                # can now be inserted with the correct key. The type checking
-                # of out will be done in `_insert_error_scores`.
-                if callable(self.scoring):
-                    _insert_error_scores(out, self.error_score)
-                all_candidate_params.extend(candidate_params)
-                all_out.extend(out)
-                if more_results is not None:
-                    for key, value in more_results.items():
-                        all_more_results[key].extend(value)
-
-                nonlocal results
-                results = self._format_results(
-                    all_candidate_params, n_splits, all_out,
-                    all_more_results)
-
-                return results
-
-            self._run_search(evaluate_candidates)
-
-            # multimetric is determined here because in the case of a callable
-            # self.scoring the return type is only known after calling
-            first_test_score = all_out[0]['test_scores']
-            self.multimetric_ = isinstance(first_test_score, dict)
-
-            # check refit_metric now for a callabe scorer that is multimetric
-            if callable(self.scoring) and self.multimetric_:
-                self._check_refit_for_multimetric(first_test_score)
-                refit_metric = self.refit
-
-        # For multi-metric evaluation, store the best_index_, best_params_ and
-        # best_score_ iff refit is one of the scorer names
-        # In single metric evaluation, refit_metric is "score"
-        if self.refit or not self.multimetric_:
-            # If callable, refit is expected to return the index of the best
-            # parameter set.
-            if callable(self.refit):
-                self.best_index_ = self.refit(results)
-                if not isinstance(self.best_index_, numbers.Integral):
-                    raise TypeError('best_index_ returned is not an integer')
-                if (self.best_index_ < 0 or
-                   self.best_index_ >= len(results["params"])):
-                    raise IndexError('best_index_ index out of range')
-            else:
-                self.best_index_ = results["rank_test_%s"
-                                           % refit_metric].argmin()
-                self.best_score_ = results["mean_test_%s" % refit_metric][
-                                           self.best_index_]
-            self.best_params_ = results["params"][self.best_index_]
-
-        if self.refit:
-            # we clone again after setting params in case some
-            # of the params are estimators as well.
-            self.best_estimator_ = clone(clone(base_estimator).set_params(
-                **self.best_params_))
-            refit_start_time = time.time()
-            if y is not None:
-                self.best_estimator_.fit(X, y, **fit_params)
-            else:
-                self.best_estimator_.fit(X, **fit_params)
-            refit_end_time = time.time()
-            self.refit_time_ = refit_end_time - refit_start_time
-
-        # Store the only scorer not as a dict for single metric evaluation
-        self.scorer_ = scorers
-
-        self.cv_results_ = results
-        self.n_splits_ = n_splits
-
+import copy
+from joblib import Parallel
+import numpy as np
+import time
+import numbers
+from itertools import product
+from collections import defaultdict
+from sklearn import clone
+from sklearn.pipeline import Pipeline
+from sklearn.model_selection import check_cv, GridSearchCV, RandomizedSearchCV
+from sklearn.model_selection._validation import _fit_and_score, _insert_error_scores, _aggregate_score_dicts, _normalize_score_results, _translate_train_sizes, _incremental_fit_estimator
+from sklearn.utils.validation import indexable, check_random_state, _check_fit_params
+from sklearn.metrics import check_scoring
+from sklearn.metrics._scorer import _check_multimetric_scoring
+from sklearn.base import is_classifier
+from sklearn.utils.fixes import delayed
+from lightgbm import LGBMModel
+from lightgbm import early_stopping, log_evaluation
+
+def init_eval_set(src_eval_set_selection, src_fit_params, X, y):
+        """
+        fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理
+        
+        Parameters
+        ----------
+        src_eval_set_selection : {'all', 'test', 'train', 'original', 'original_transformed'}, optional
+            eval_setに渡すデータの決め方 ('all': X, 'test': X[test], 'train': X[train], 'original': 入力そのまま, 'original_transformed': 入力そのまま＆パイプラインの時は最終学習器以外の変換実行)
+
+        src_fit_params : Dict
+            処理前の学習時パラメータ
+        """
+
+        fit_params = copy.deepcopy(src_fit_params)
+        eval_set_selection = src_eval_set_selection
+        # fit_paramsにeval_metricが設定されているときのみ以下の処理を実施
+        if 'eval_metric' in src_fit_params and src_fit_params['eval_metric'] is not None:
+            # fit_paramsにeval_setが存在しないとき、入力データをそのまま追加
+            if 'eval_set' not in src_fit_params:
+                print('There is no "eval_set" in fit_params, so "eval_set" is set to (self.X, self.y)')
+                fit_params['eval_set'] = [(X, y)]
+                if src_eval_set_selection is None:  # eval_set_selection未指定時、eval_setが入力されていなければeval_set_selection='test'とする
+                    eval_set_selection = 'test'
+                if eval_set_selection not in ['all', 'train', 'test']:  # eval_set_selectionの指定が間違っていたらエラーを出す
+                    raise ValueError('The `eval_set_selection` argument should be "all", "train", or "test" when `eval_set` is not in `fit_params`')
+            # src_fit_paramsにeval_setが存在するとき、eval_set_selection未指定ならばeval_set_selection='original_transformed'とする
+            else:
+                if src_eval_set_selection is None:
+                    eval_set_selection = 'original_transformed'
+
+        return fit_params, eval_set_selection
+
+def _transform_except_last_estimator(transformer, X_src, X_train):
+    """パイプラインのとき、最終学習器以外のtransformを適用"""
+    if transformer is not None:
+        transformer.fit(X_train)
+        X_dst = transformer.transform(X_src)
+        return X_dst
+    else:
+        return X_src
+
+def _eval_set_selection(eval_set_selection, transformer,
+                        fit_params, train, test):
+    """eval_setの中から学習データ or テストデータのみを抽出"""
+    fit_params_modified = copy.deepcopy(fit_params)
+    # eval_setが存在しない or Noneなら、そのままfit_paramsを返す
+    eval_sets = [v for v in fit_params.keys() if 'eval_set' in v]
+    if len(eval_sets) == 0 or fit_params[eval_sets[0]] is None:
+        return fit_params_modified
+    eval_set_name = eval_sets[0]  # eval_setの列名(pipelineでは列名が変わるため)
+    # 元のeval_setからX, yを取得
+    X_fit = fit_params[eval_set_name][0][0]
+    y_fit = fit_params[eval_set_name][0][1]
+    # eval_setに該当データを入力し直す
+    if eval_set_selection == 'train':
+        fit_params_modified[eval_set_name] = [(_transform_except_last_estimator(transformer, X_fit[train], X_fit[train])\
+                                              , y_fit[train])]
+    elif eval_set_selection == 'test':
+        fit_params_modified[eval_set_name] = [(_transform_except_last_estimator(transformer, X_fit[test], X_fit[train])\
+                                              , y_fit[test])]
+    elif eval_set_selection == 'all':
+        fit_params_modified[eval_set_name] = [(_transform_except_last_estimator(transformer, X_fit, X_fit[train])\
+                                              , y_fit)]
+    else:
+        fit_params_modified[eval_set_name] = [(_transform_except_last_estimator(transformer, X_fit, X_fit)\
+                                              , y_fit)]
+    return fit_params_modified
+
+def _lgbm_early_stop_transform(estimator, fit_params_modified):
+    """LightGBMのearly_stoppingおよびverbose引数をコールバック関数に変更 (FutureWarning対策)"""
+    if isinstance(estimator, LGBMModel):
+        if 'early_stopping_rounds' in fit_params_modified.keys() or 'verbose' in fit_params_modified.keys():
+            if 'callbacks' in fit_params_modified.keys():
+                raise ValueError('The `callbacks` argument and the `early_stopping_rounds` or the `verbose` argument cannot be compatible in `fit_params`')
+            fit_params_modified['callbacks'] = []
+            if 'verbose' in fit_params_modified.keys():
+                fit_params_modified['callbacks'].append(log_evaluation(fit_params_modified['verbose']))
+                fit_params_modified.pop('verbose')
+            if 'early_stopping_rounds' in fit_params_modified.keys():
+                fit_params_modified['callbacks'].append(early_stopping(fit_params_modified['early_stopping_rounds'], False, False))
+                fit_params_modified.pop('early_stopping_rounds')
+
+def _fit_and_score_eval_set(eval_set_selection, transformer,
+                            estimator, X, y, scorer, train, test, verbose,
+                            parameters, fit_params, return_train_score=False,
+                            return_parameters=False, return_n_test_samples=False,
+                            return_times=False, return_estimator=False,
+                            split_progress=None, candidate_progress=None,
+                            error_score=np.nan,
+                            print_message=None):
+
+    """Fit estimator and compute scores for a given dataset split."""
+    # eval_setの中から学習データ or テストデータのみを抽出
+    fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
+                                              fit_params, train, test)
+    # LightGBMのearly_stoppingをコールバック関数に変更
+    _lgbm_early_stop_transform(estimator, fit_params_modified)
+    if print_message is not None:
+        print(print_message)
+    # 学習してスコア計算
+    result = _fit_and_score(estimator, X, y, scorer, train, test, verbose, parameters,
+                            fit_params_modified,
+                            return_train_score=return_train_score,
+                            return_parameters=return_parameters, return_n_test_samples=return_n_test_samples,
+                            return_times=return_times, return_estimator=return_estimator,
+                            split_progress=split_progress, candidate_progress=candidate_progress,
+                            error_score=error_score)
+    return result
+
+def _make_transformer(eval_set_selection, estimator):
+    """estimatorがパイプラインのとき、最終学習器以外の変換器(前処理クラスのリスト)を作成"""
+    if isinstance(estimator, Pipeline) and eval_set_selection != 'original':
+        transformer = Pipeline([step for i, step in enumerate(estimator.steps) if i < len(estimator) - 1])
+        return transformer
+    else:
+        return None
+
+def cross_validate_eval_set(eval_set_selection,
+                            estimator, X, y=None, groups=None, scoring=None, cv=None,
+                            n_jobs=None, verbose=0, fit_params=None,
+                            pre_dispatch='2*n_jobs', return_train_score=False,
+                            return_estimator=False, error_score=np.nan):
+    """
+    Evaluate a scores by cross-validation with `eval_set` argument in `fit_params`
+
+    This method is suitable for calculating cross validation scores with `early_stopping_round` in XGBoost or LightGBM.
+
+    Parameters
+    ----------
+    eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
+        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
+            
+        If "all", use all data in `X` and `y`.
+
+        If "train", select train data from `X` and `y` using cv.split().
+
+        If "test", select test data from `X` and `y` using cv.split().
+
+        If "original", use raw `eval_set`.
+
+        If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+
+    estimator : estimator object implementing 'fit'
+        The object to use to fit the data.
+
+    X : array-like of shape (n_samples, n_features)
+        The data to fit. Can be for example a list, or an array.
+
+    y : array-like of shape (n_samples,) or (n_samples, n_outputs), \
+            default=None
+        The target variable to try to predict in the case of
+        supervised learning.
+
+    groups : array-like of shape (n_samples,), default=None
+        Group labels for the samples used while splitting the dataset into
+        train/test set. Only used in conjunction with a "Group" :term:`cv`
+        instance (e.g., :class:`GroupKFold`).
+
+    scoring : str, callable, list, tuple, or dict, default=None
+        Strategy to evaluate the performance of the cross-validated model on
+        the test set.
+
+        If `scoring` represents a single score, one can use:
+
+        - a single string (see :ref:`scoring_parameter`);
+        - a callable (see :ref:`scoring`) that returns a single value.
+
+        If `scoring` represents multiple scores, one can use:
+
+        - a list or tuple of unique strings;
+        - a callable returning a dictionary where the keys are the metric
+          names and the values are the metric scores;
+        - a dictionary with metric names as keys and callables a values.
+
+        See :ref:`multimetric_grid_search` for an example.
+
+    cv : int, cross-validation generator or an iterable, default=None
+        Determines the cross-validation splitting strategy.
+        Possible inputs for cv are:
+
+        - None, to use the default 5-fold cross validation,
+        - int, to specify the number of folds in a `(Stratified)KFold`,
+        - :term:`CV splitter`,
+        - An iterable yielding (train, test) splits as arrays of indices.
+
+        For int/None inputs, if the estimator is a classifier and ``y`` is
+        either binary or multiclass, :class:`StratifiedKFold` is used. In all
+        other cases, :class:`.Fold` is used. These splitters are instantiated
+        with `shuffle=False` so the splits will be the same across calls.
+
+        Refer :ref:`User Guide <cross_validation>` for the various
+        cross-validation strategies that can be used here.
+
+        .. versionchanged:: 0.22
+            ``cv`` default value if None changed from 3-fold to 5-fold.
+
+    n_jobs : int, default=None
+        Number of jobs to run in parallel. Training the estimator and computing
+        the score are parallelized over the cross-validation splits.
+        ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
+        ``-1`` means using all processors. See :term:`Glossary <n_jobs>`
+        for more details.
+
+    verbose : int, default=0
+        The verbosity level.
+
+    fit_params : dict, default=None
+        Parameters to pass to the fit method of the estimator.
+
+    pre_dispatch : int or str, default='2*n_jobs'
+        Controls the number of jobs that get dispatched during parallel
+        execution. Reducing this number can be useful to avoid an
+        explosion of memory consumption when more jobs get dispatched
+        than CPUs can process. This parameter can be:
+
+            - None, in which case all the jobs are immediately
+              created and spawned. Use this for lightweight and
+              fast-running jobs, to avoid delays due to on-demand
+              spawning of the jobs
+
+            - An int, giving the exact number of total jobs that are
+              spawned
+
+            - A str, giving an expression as a function of n_jobs,
+              as in '2*n_jobs'
+
+    return_train_score : bool, default=False
+        Whether to include train scores.
+        Computing training scores is used to get insights on how different
+        parameter settings impact the overfitting/underfitting trade-off.
+        However computing the scores on the training set can be computationally
+        expensive and is not strictly required to select the parameters that
+        yield the best generalization performance.
+
+        .. versionadded:: 0.19
+
+        .. versionchanged:: 0.21
+            Default value was changed from ``True`` to ``False``
+
+    return_estimator : bool, default=False
+        Whether to return the estimators fitted on each split.
+
+        .. versionadded:: 0.20
+
+    error_score : 'raise' or numeric, default=np.nan
+        Value to assign to the score if an error occurs in estimator fitting.
+        If set to 'raise', the error is raised.
+        If a numeric value is given, FitFailedWarning is raised.
+
+        .. versionadded:: 0.20
+
+    Returns
+    -------
+    scores : dict of float arrays of shape (n_splits,)
+        Array of scores of the estimator for each run of the cross validation.
+    """
+
+    X, y, groups = indexable(X, y, groups)
+
+    cv = check_cv(cv, y, classifier=is_classifier(estimator))
+
+    if callable(scoring):
+        scorers = scoring
+    elif scoring is None or isinstance(scoring, str):
+        scorers = check_scoring(estimator, scoring)
+    else:
+        scorers = _check_multimetric_scoring(estimator, scoring)
+
+    # 最終学習器以外の前処理変換器作成
+    transformer = _make_transformer(eval_set_selection, estimator)
+
+    # We clone the estimator to make sure that all the folds are
+    # independent, and that it is pickle-able.
+    parallel = Parallel(n_jobs=n_jobs, verbose=verbose,
+                        pre_dispatch=pre_dispatch)
+    results = parallel(
+        delayed(_fit_and_score_eval_set)(
+            eval_set_selection, transformer,
+            clone(estimator), X, y, scorers, train, test, verbose, None,
+            fit_params, return_train_score=return_train_score,
+            return_times=True, return_estimator=return_estimator,
+            error_score=error_score)
+        for train, test in cv.split(X, y, groups))
+
+    # For callabe scoring, the return type is only know after calling. If the
+    # return type is a dictionary, the error scores can now be inserted with
+    # the correct key.
+    if callable(scoring):
+        _insert_error_scores(results, error_score)
+
+    results = _aggregate_score_dicts(results)
+
+    ret = {}
+    ret['fit_time'] = results["fit_time"]
+    ret['score_time'] = results["score_time"]
+
+    if return_estimator:
+        ret['estimator'] = results["estimator"]
+
+    test_scores_dict = _normalize_score_results(results["test_scores"])
+    if return_train_score:
+        train_scores_dict = _normalize_score_results(results["train_scores"])
+
+    for name in test_scores_dict:
+        ret['test_%s' % name] = test_scores_dict[name]
+        if return_train_score:
+            key = 'train_%s' % name
+            ret[key] = train_scores_dict[name]
+
+    return ret
+
+def cross_val_score_eval_set(eval_set_selection,
+                             estimator, X, y=None, groups=None, scoring=None,
+                             cv=None, n_jobs=None, verbose=0, fit_params=None,
+                             pre_dispatch='2*n_jobs', error_score=np.nan):
+    """
+    Evaluate a score by cross-validation with `eval_set` argument in `fit_params`
+
+    This method is suitable for calculating cross validation score with `early_stopping_round` in XGBoost or LightGBM.
+
+    Parameters
+    ----------
+    eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
+        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
+            
+        If "all", use all data in `X` and `y`.
+
+        If "train", select train data from `X` and `y` using cv.split().
+
+        If "test", select test data from `X` and `y` using cv.split().
+
+        If "original", use raw `eval_set`.
+
+        If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+    
+    estimator : estimator object implementing 'fit'
+        The object to use to fit the data.
+
+    X : array-like of shape (n_samples, n_features)
+        The data to fit. Can be for example a list, or an array.
+
+    y : array-like of shape (n_samples,) or (n_samples, n_outputs), \
+            default=None
+        The target variable to try to predict in the case of
+        supervised learning.
+
+    groups : array-like of shape (n_samples,), default=None
+        Group labels for the samples used while splitting the dataset into
+        train/test set. Only used in conjunction with a "Group" :term:`cv`
+        instance (e.g., :class:`GroupKFold`).
+
+    scoring : str or callable, default=None
+        A str (see model evaluation documentation) or
+        a scorer callable object / function with signature
+        ``scorer(estimator, X, y)`` which should return only
+        a single value.
+
+        Similar to :func:`cross_validate`
+        but only a single metric is permitted.
+
+        If None, the estimator's default scorer (if available) is used.
+
+    cv : int, cross-validation generator or an iterable, default=None
+        Determines the cross-validation splitting strategy.
+        Possible inputs for cv are:
+
+        - None, to use the default 5-fold cross validation,
+        - int, to specify the number of folds in a `(Stratified)KFold`,
+        - :term:`CV splitter`,
+        - An iterable yielding (train, test) splits as arrays of indices.
+
+        For int/None inputs, if the estimator is a classifier and ``y`` is
+        either binary or multiclass, :class:`StratifiedKFold` is used. In all
+        other cases, :class:`KFold` is used. These splitters are instantiated
+        with `shuffle=False` so the splits will be the same across calls.
+
+        Refer :ref:`User Guide <cross_validation>` for the various
+        cross-validation strategies that can be used here.
+
+        .. versionchanged:: 0.22
+            ``cv`` default value if None changed from 3-fold to 5-fold.
+
+    n_jobs : int, default=None
+        Number of jobs to run in parallel. Training the estimator and computing
+        the score are parallelized over the cross-validation splits.
+        ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
+        ``-1`` means using all processors. See :term:`Glossary <n_jobs>`
+        for more details.
+
+    verbose : int, default=0
+        The verbosity level.
+
+    fit_params : dict, default=None
+        Parameters to pass to the fit method of the estimator.
+
+    pre_dispatch : int or str, default='2*n_jobs'
+        Controls the number of jobs that get dispatched during parallel
+        execution. Reducing this number can be useful to avoid an
+        explosion of memory consumption when more jobs get dispatched
+        than CPUs can process. This parameter can be:
+
+            - None, in which case all the jobs are immediately
+              created and spawned. Use this for lightweight and
+              fast-running jobs, to avoid delays due to on-demand
+              spawning of the jobs
+
+            - An int, giving the exact number of total jobs that are
+              spawned
+
+            - A str, giving an expression as a function of n_jobs,
+              as in '2*n_jobs'
+
+    error_score : 'raise' or numeric, default=np.nan
+        Value to assign to the score if an error occurs in estimator fitting.
+        If set to 'raise', the error is raised.
+        If a numeric value is given, FitFailedWarning is raised.
+
+        .. versionadded:: 0.20
+
+    Returns
+    -------
+    scores : ndarray of float of shape=(len(list(cv)),)
+        Array of scores of the estimator for each run of the cross validation.
+    """
+    # To ensure multimetric format is not supported
+    scorer = check_scoring(estimator, scoring=scoring)
+
+    cv_results = cross_validate_eval_set(eval_set_selection=eval_set_selection,
+                                         estimator=estimator, X=X, y=y, groups=groups,
+                                         scoring={'score': scorer}, cv=cv,
+                                         n_jobs=n_jobs, verbose=verbose,
+                                         fit_params=fit_params,
+                                         pre_dispatch=pre_dispatch,
+                                         error_score=error_score)
+    return cv_results['test_score']
+
+def validation_curve_eval_set(eval_set_selection,
+                              estimator, X, y, param_name, param_range, groups=None,
+                              cv=None, scoring=None, n_jobs=None, pre_dispatch="all",
+                              verbose=0, error_score=np.nan, fit_params=None):
+    """Validation curve.
+
+    Determine training and test scores for varying parameter values with `eval_set` argument in `fit_params`
+
+    Parameters
+    ----------
+    eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
+        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
+            
+        If "all", use all data in `X` and `y`.
+
+        If "train", select train data from `X` and `y` using cv.split().
+
+        If "test", select test data from `X` and `y` using cv.split().
+
+        If "original", use raw `eval_set`.
+
+        If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+    
+    estimator : object type that implements the "fit" and "predict" methods
+        An object of that type which is cloned for each validation.
+
+    X : array-like of shape (n_samples, n_features)
+        Training vector, where n_samples is the number of samples and
+        n_features is the number of features.
+
+    y : array-like of shape (n_samples,) or (n_samples, n_outputs) or None
+        Target relative to X for classification or regression;
+        None for unsupervised learning.
+
+    param_name : str
+        Name of the parameter that will be varied.
+
+    param_range : array-like of shape (n_values,)
+        The values of the parameter that will be evaluated.
+
+    groups : array-like of shape (n_samples,), default=None
+        Group labels for the samples used while splitting the dataset into
+        train/test set. Only used in conjunction with a "Group" :term:`cv`
+        instance (e.g., :class:`GroupKFold`).
+
+    cv : int, cross-validation generator or an iterable, default=None
+        Determines the cross-validation splitting strategy.
+        Possible inputs for cv are:
+
+        - None, to use the default 5-fold cross validation,
+        - int, to specify the number of folds in a `(Stratified)KFold`,
+        - :term:`CV splitter`,
+        - An iterable yielding (train, test) splits as arrays of indices.
+
+        For int/None inputs, if the estimator is a classifier and ``y`` is
+        either binary or multiclass, :class:`StratifiedKFold` is used. In all
+        other cases, :class:`KFold` is used. These splitters are instantiated
+        with `shuffle=False` so the splits will be the same across calls.
+
+        Refer :ref:`User Guide <cross_validation>` for the various
+        cross-validation strategies that can be used here.
+
+        .. versionchanged:: 0.22
+            ``cv`` default value if None changed from 3-fold to 5-fold.
+
+    scoring : str or callable, default=None
+        A str (see model evaluation documentation) or
+        a scorer callable object / function with signature
+        ``scorer(estimator, X, y)``.
+
+    n_jobs : int, default=None
+        Number of jobs to run in parallel. Training the estimator and computing
+        the score are parallelized over the combinations of each parameter
+        value and each cross-validation split.
+        ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
+        ``-1`` means using all processors. See :term:`Glossary <n_jobs>`
+        for more details.
+
+    pre_dispatch : int or str, default='all'
+        Number of predispatched jobs for parallel execution (default is
+        all). The option can reduce the allocated memory. The str can
+        be an expression like '2*n_jobs'.
+
+    verbose : int, default=0
+        Controls the verbosity: the higher, the more messages.
+
+    fit_params : dict, default=None
+        Parameters to pass to the fit method of the estimator.
+
+        .. versionadded:: 0.24
+
+    error_score : 'raise' or numeric, default=np.nan
+        Value to assign to the score if an error occurs in estimator fitting.
+        If set to 'raise', the error is raised.
+        If a numeric value is given, FitFailedWarning is raised.
+
+        .. versionadded:: 0.20
+
+    Returns
+    -------
+    train_scores : array of shape (n_ticks, n_cv_folds)
+        Scores on training sets.
+
+    test_scores : array of shape (n_ticks, n_cv_folds)
+        Scores on test set.
+    """
+    X, y, groups = indexable(X, y, groups)
+
+    cv = check_cv(cv, y, classifier=is_classifier(estimator))
+    scorer = check_scoring(estimator, scoring=scoring)
+
+    # 最終学習器以外の前処理変換器作成
+    transformer = _make_transformer(eval_set_selection, estimator)
+
+    parallel = Parallel(n_jobs=n_jobs, pre_dispatch=pre_dispatch,
+                        verbose=verbose)
+    results = parallel(delayed(_fit_and_score_eval_set)(
+        eval_set_selection, transformer,
+        clone(estimator), X, y, scorer, train, test, verbose,
+        parameters={param_name: v}, fit_params=fit_params,
+        return_train_score=True, error_score=error_score,
+        print_message=f'Caluculating score. {param_name}={v}')
+
+        # NOTE do not change order of iteration to allow one time cv splitters
+        for train, test in cv.split(X, y, groups) for v in param_range)
+    n_params = len(param_range)
+
+    results = _aggregate_score_dicts(results)
+    train_scores = results["train_scores"].reshape(-1, n_params).T
+    test_scores = results["test_scores"].reshape(-1, n_params).T
+
+    return train_scores, test_scores
+
+def learning_curve_eval_set(eval_set_selection,
+                            estimator, X, y, groups=None,
+                            train_sizes=np.linspace(0.1, 1.0, 5), cv=None,
+                            scoring=None, exploit_incremental_learning=False,
+                            n_jobs=None, pre_dispatch="all", verbose=0, shuffle=False,
+                            random_state=None, error_score=np.nan, return_times=False,
+                            fit_params=None):
+    """Learning curve.
+
+    Determines cross-validated training and test scores for different training set sizes with `eval_set` argument in `fit_params`
+
+    Parameters
+    ----------
+    eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
+        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
+            
+        If "all", use all data in `X` and `y`.
+
+        If "train", select train data from `X` and `y` using cv.split().
+
+        If "test", select test data from `X` and `y` using cv.split().
+
+        If "original", use raw `eval_set`.
+
+        If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+    
+    estimator : object type that implements the "fit" and "predict" methods
+        An object of that type which is cloned for each validation.
+
+    X : array-like of shape (n_samples, n_features)
+        Training vector, where n_samples is the number of samples and
+        n_features is the number of features.
+
+    y : array-like of shape (n_samples,) or (n_samples, n_outputs)
+        Target relative to X for classification or regression;
+        None for unsupervised learning.
+
+    groups : array-like of  shape (n_samples,), default=None
+        Group labels for the samples used while splitting the dataset into
+        train/test set. Only used in conjunction with a "Group" :term:`cv`
+        instance (e.g., :class:`GroupKFold`).
+
+    train_sizes : array-like of shape (n_ticks,), \
+            default=np.linspace(0.1, 1.0, 5)
+        Relative or absolute numbers of training examples that will be used to
+        generate the learning curve. If the dtype is float, it is regarded as a
+        fraction of the maximum size of the training set (that is determined
+        by the selected validation method), i.e. it has to be within (0, 1].
+        Otherwise it is interpreted as absolute sizes of the training sets.
+        Note that for classification the number of samples usually have to
+        be big enough to contain at least one sample from each class.
+
+    cv : int, cross-validation generator or an iterable, default=None
+        Determines the cross-validation splitting strategy.
+        Possible inputs for cv are:
+
+        - None, to use the default 5-fold cross validation,
+        - int, to specify the number of folds in a `(Stratified)KFold`,
+        - :term:`CV splitter`,
+        - An iterable yielding (train, test) splits as arrays of indices.
+
+        For int/None inputs, if the estimator is a classifier and ``y`` is
+        either binary or multiclass, :class:`StratifiedKFold` is used. In all
+        other cases, :class:`KFold` is used. These splitters are instantiated
+        with `shuffle=False` so the splits will be the same across calls.
+
+        Refer :ref:`User Guide <cross_validation>` for the various
+        cross-validation strategies that can be used here.
+
+        .. versionchanged:: 0.22
+            ``cv`` default value if None changed from 3-fold to 5-fold.
+
+    scoring : str or callable, default=None
+        A str (see model evaluation documentation) or
+        a scorer callable object / function with signature
+        ``scorer(estimator, X, y)``.
+
+    exploit_incremental_learning : bool, default=False
+        If the estimator supports incremental learning, this will be
+        used to speed up fitting for different training set sizes.
+
+    n_jobs : int, default=None
+        Number of jobs to run in parallel. Training the estimator and computing
+        the score are parallelized over the different training and test sets.
+        ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
+        ``-1`` means using all processors. See :term:`Glossary <n_jobs>`
+        for more details.
+
+    pre_dispatch : int or str, default='all'
+        Number of predispatched jobs for parallel execution (default is
+        all). The option can reduce the allocated memory. The str can
+        be an expression like '2*n_jobs'.
+
+    verbose : int, default=0
+        Controls the verbosity: the higher, the more messages.
+
+    shuffle : bool, default=False
+        Whether to shuffle training data before taking prefixes of it
+        based on``train_sizes``.
+
+    random_state : int, RandomState instance or None, default=None
+        Used when ``shuffle`` is True. Pass an int for reproducible
+        output across multiple function calls.
+        See :term:`Glossary <random_state>`.
+
+    error_score : 'raise' or numeric, default=np.nan
+        Value to assign to the score if an error occurs in estimator fitting.
+        If set to 'raise', the error is raised.
+        If a numeric value is given, FitFailedWarning is raised.
+
+        .. versionadded:: 0.20
+
+    return_times : bool, default=False
+        Whether to return the fit and score times.
+
+    fit_params : dict, default=None
+        Parameters to pass to the fit method of the estimator.
+
+        .. versionadded:: 0.24
+
+    Returns
+    -------
+    train_sizes_abs : array of shape (n_unique_ticks,)
+        Numbers of training examples that has been used to generate the
+        learning curve. Note that the number of ticks might be less
+        than n_ticks because duplicate entries will be removed.
+
+    train_scores : array of shape (n_ticks, n_cv_folds)
+        Scores on training sets.
+
+    test_scores : array of shape (n_ticks, n_cv_folds)
+        Scores on test set.
+
+    fit_times : array of shape (n_ticks, n_cv_folds)
+        Times spent for fitting in seconds. Only present if ``return_times``
+        is True.
+
+    score_times : array of shape (n_ticks, n_cv_folds)
+        Times spent for scoring in seconds. Only present if ``return_times``
+        is True.
+    """
+    if exploit_incremental_learning and not hasattr(estimator, "partial_fit"):
+        raise ValueError("An estimator must support the partial_fit interface "
+                         "to exploit incremental learning")
+    X, y, groups = indexable(X, y, groups)
+
+    cv = check_cv(cv, y, classifier=is_classifier(estimator))
+    # Store it as list as we will be iterating over the list multiple times
+    cv_iter = list(cv.split(X, y, groups))
+
+    scorer = check_scoring(estimator, scoring=scoring)
+
+    n_max_training_samples = len(cv_iter[0][0])
+    # Because the lengths of folds can be significantly different, it is
+    # not guaranteed that we use all of the available training data when we
+    # use the first 'n_max_training_samples' samples.
+    train_sizes_abs = _translate_train_sizes(train_sizes,
+                                             n_max_training_samples)
+    n_unique_ticks = train_sizes_abs.shape[0]
+    if verbose > 0:
+        print("[learning_curve] Training set sizes: " + str(train_sizes_abs))
+
+    # 最終学習器以外の前処理変換器作成
+    transformer = _make_transformer(eval_set_selection, estimator)
+
+    parallel = Parallel(n_jobs=n_jobs, pre_dispatch=pre_dispatch,
+                        verbose=verbose)
+
+    if shuffle:
+        rng = check_random_state(random_state)
+        cv_iter = ((rng.permutation(train), test) for train, test in cv_iter)
+
+    if exploit_incremental_learning:
+        classes = np.unique(y) if is_classifier(estimator) else None
+        out = parallel(delayed(_incremental_fit_estimator)(
+            clone(estimator), X, y, classes, train, test, train_sizes_abs,
+            scorer, verbose, return_times, error_score=error_score,
+            fit_params=fit_params)
+            for train, test in cv_iter
+        )
+        out = np.asarray(out).transpose((2, 1, 0))
+    else:
+        train_test_proportions = []
+        for train, test in cv_iter:
+            for n_train_samples in train_sizes_abs:
+                train_test_proportions.append((train[:n_train_samples], test))
+
+        results = parallel(delayed(_fit_and_score_eval_set)(
+            eval_set_selection, transformer,
+            clone(estimator), X, y, scorer, train, test, verbose,
+            parameters=None, fit_params=fit_params, return_train_score=True,
+            error_score=error_score, return_times=return_times)
+            for train, test in train_test_proportions
+        )
+        results = _aggregate_score_dicts(results)
+        train_scores = results["train_scores"].reshape(-1, n_unique_ticks).T
+        test_scores = results["test_scores"].reshape(-1, n_unique_ticks).T
+        out = [train_scores, test_scores]
+
+        if return_times:
+            fit_times = results["fit_time"].reshape(-1, n_unique_ticks).T
+            score_times = results["score_time"].reshape(-1, n_unique_ticks).T
+            out.extend([fit_times, score_times])
+
+    ret = train_sizes_abs, out[0], out[1]
+
+    if return_times:
+        ret = ret + (out[2], out[3])
+
+    return ret
+
+class GridSearchCVEvalSet(GridSearchCV):
+    """
+    Exhaustive search over specified parameter values for an estimator with `eval_set` argument in `fit_params`.
+    """
+    def fit(self, eval_set_selection,
+            X, y=None, groups=None, **fit_params):
+        """Run fit with all sets of parameters.
+
+        Parameters
+        ----------
+        eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
+                
+            If "all", use all data in `X` and `y`.
+
+            If "train", select train data from `X` and `y` using cv.split().
+
+            If "test", select test data from `X` and `y` using cv.split().
+
+            If "original", use raw `eval_set`.
+
+            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+
+        X : array-like of shape (n_samples, n_features)
+            Training vector, where n_samples is the number of samples and
+            n_features is the number of features.
+
+        y : array-like of shape (n_samples, n_output) \
+            or (n_samples,), default=None
+            Target relative to X for classification or regression;
+            None for unsupervised learning.
+
+        groups : array-like of shape (n_samples,), default=None
+            Group labels for the samples used while splitting the dataset into
+            train/test set. Only used in conjunction with a "Group" :term:`cv`
+            instance (e.g., :class:`~sklearn.model_selection.GroupKFold`).
+
+        **fit_params : dict of str -> object
+            Parameters passed to the ``fit`` method of the estimator
+        """
+        estimator = self.estimator
+        refit_metric = "score"
+
+        if callable(self.scoring):
+            scorers = self.scoring
+        elif self.scoring is None or isinstance(self.scoring, str):
+            scorers = check_scoring(self.estimator, self.scoring)
+        else:
+            scorers = _check_multimetric_scoring(self.estimator, self.scoring)
+            self._check_refit_for_multimetric(scorers)
+            refit_metric = self.refit
+
+        X, y, groups = indexable(X, y, groups)
+        fit_params = _check_fit_params(X, fit_params)
+
+        cv_orig = check_cv(self.cv, y, classifier=is_classifier(estimator))
+        n_splits = cv_orig.get_n_splits(X, y, groups)
+
+        base_estimator = clone(self.estimator)
+
+        # 最終学習器以外の前処理変換器作成
+        transformer = _make_transformer(eval_set_selection, estimator)
+
+        parallel = Parallel(n_jobs=self.n_jobs,
+                            pre_dispatch=self.pre_dispatch)
+
+        fit_and_score_kwargs = dict(scorer=scorers,
+                                    fit_params=fit_params,
+                                    return_train_score=self.return_train_score,
+                                    return_n_test_samples=True,
+                                    return_times=True,
+                                    return_parameters=False,
+                                    error_score=self.error_score,
+                                    verbose=self.verbose)
+        results = {}
+        with parallel:
+            all_candidate_params = []
+            all_out = []
+            all_more_results = defaultdict(list)
+
+            def evaluate_candidates(candidate_params, cv=None,
+                                    more_results=None):
+                cv = cv or cv_orig
+                candidate_params = list(candidate_params)
+                n_candidates = len(candidate_params)
+
+                if self.verbose > 0:
+                    print("Fitting {0} folds for each of {1} candidates,"
+                          " totalling {2} fits".format(
+                              n_splits, n_candidates, n_candidates * n_splits))
+
+                out = parallel(delayed(_fit_and_score_eval_set)(
+                                        eval_set_selection, transformer,
+                                        clone(base_estimator),
+                                        X, y,
+                                        train=train, test=test,
+                                        parameters=parameters,
+                                        split_progress=(
+                                            split_idx,
+                                            n_splits),
+                                        candidate_progress=(
+                                            cand_idx,
+                                            n_candidates),
+                                        print_message=f'cand={cand_idx}/{n_candidates}, cv={split_idx}: {parameters}',
+                                        **fit_and_score_kwargs)
+                               for (cand_idx, parameters),
+                                   (split_idx, (train, test)) in product(
+                                   enumerate(candidate_params),
+                                   enumerate(cv.split(X, y, groups))))
+
+                if len(out) < 1:
+                    raise ValueError('No fits were performed. '
+                                     'Was the CV iterator empty? '
+                                     'Were there no candidates?')
+                elif len(out) != n_candidates * n_splits:
+                    raise ValueError('cv.split and cv.get_n_splits returned '
+                                     'inconsistent results. Expected {} '
+                                     'splits, got {}'
+                                     .format(n_splits,
+                                             len(out) // n_candidates))
+
+                # For callable self.scoring, the return type is only know after
+                # calling. If the return type is a dictionary, the error scores
+                # can now be inserted with the correct key. The type checking
+                # of out will be done in `_insert_error_scores`.
+                if callable(self.scoring):
+                    _insert_error_scores(out, self.error_score)
+                all_candidate_params.extend(candidate_params)
+                all_out.extend(out)
+                if more_results is not None:
+                    for key, value in more_results.items():
+                        all_more_results[key].extend(value)
+
+                nonlocal results
+                results = self._format_results(
+                    all_candidate_params, n_splits, all_out,
+                    all_more_results)
+
+                return results
+
+            self._run_search(evaluate_candidates)
+
+            # multimetric is determined here because in the case of a callable
+            # self.scoring the return type is only known after calling
+            first_test_score = all_out[0]['test_scores']
+            self.multimetric_ = isinstance(first_test_score, dict)
+
+            # check refit_metric now for a callabe scorer that is multimetric
+            if callable(self.scoring) and self.multimetric_:
+                self._check_refit_for_multimetric(first_test_score)
+                refit_metric = self.refit
+
+        # For multi-metric evaluation, store the best_index_, best_params_ and
+        # best_score_ iff refit is one of the scorer names
+        # In single metric evaluation, refit_metric is "score"
+        if self.refit or not self.multimetric_:
+            # If callable, refit is expected to return the index of the best
+            # parameter set.
+            if callable(self.refit):
+                self.best_index_ = self.refit(results)
+                if not isinstance(self.best_index_, numbers.Integral):
+                    raise TypeError('best_index_ returned is not an integer')
+                if (self.best_index_ < 0 or
+                   self.best_index_ >= len(results["params"])):
+                    raise IndexError('best_index_ index out of range')
+            else:
+                self.best_index_ = results["rank_test_%s"
+                                           % refit_metric].argmin()
+                self.best_score_ = results["mean_test_%s" % refit_metric][
+                                           self.best_index_]
+            self.best_params_ = results["params"][self.best_index_]
+
+        if self.refit:
+            # we clone again after setting params in case some
+            # of the params are estimators as well.
+            self.best_estimator_ = clone(clone(base_estimator).set_params(
+                **self.best_params_))
+            refit_start_time = time.time()
+            if y is not None:
+                self.best_estimator_.fit(X, y, **fit_params)
+            else:
+                self.best_estimator_.fit(X, **fit_params)
+            refit_end_time = time.time()
+            self.refit_time_ = refit_end_time - refit_start_time
+
+        # Store the only scorer not as a dict for single metric evaluation
+        self.scorer_ = scorers
+
+        self.cv_results_ = results
+        self.n_splits_ = n_splits
+
+        return self
+
+class RandomizedSearchCVEvalSet(RandomizedSearchCV):
+    """
+    Randomized search on hyper parameters with `eval_set` argument in `fit_params`.
+    """
+    def fit(self, eval_set_selection,
+            X, y=None, groups=None, **fit_params):
+        """Run fit with all sets of parameters.
+
+        Parameters
+        ----------
+        eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
+            
+            If "all", use all data in `X` and `y`.
+
+            If "train", select train data from `X` and `y` using cv.split().
+
+            If "test", select test data from `X` and `y` using cv.split().
+
+            If "original", use raw `eval_set`.
+
+            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+
+        X : array-like of shape (n_samples, n_features)
+            Training vector, where n_samples is the number of samples and
+            n_features is the number of features.
+
+        y : array-like of shape (n_samples, n_output) \
+            or (n_samples,), default=None
+            Target relative to X for classification or regression;
+            None for unsupervised learning.
+
+        groups : array-like of shape (n_samples,), default=None
+            Group labels for the samples used while splitting the dataset into
+            train/test set. Only used in conjunction with a "Group" :term:`cv`
+            instance (e.g., :class:`~sklearn.model_selection.GroupKFold`).
+
+        **fit_params : dict of str -> object
+            Parameters passed to the ``fit`` method of the estimator
+        """
+        estimator = self.estimator
+        refit_metric = "score"
+
+        if callable(self.scoring):
+            scorers = self.scoring
+        elif self.scoring is None or isinstance(self.scoring, str):
+            scorers = check_scoring(self.estimator, self.scoring)
+        else:
+            scorers = _check_multimetric_scoring(self.estimator, self.scoring)
+            self._check_refit_for_multimetric(scorers)
+            refit_metric = self.refit
+
+        X, y, groups = indexable(X, y, groups)
+        fit_params = _check_fit_params(X, fit_params)
+
+        cv_orig = check_cv(self.cv, y, classifier=is_classifier(estimator))
+        n_splits = cv_orig.get_n_splits(X, y, groups)
+
+        base_estimator = clone(self.estimator)
+
+        # 最終学習器以外の前処理変換器作成
+        transformer = _make_transformer(eval_set_selection, estimator)
+
+        parallel = Parallel(n_jobs=self.n_jobs,
+                            pre_dispatch=self.pre_dispatch)
+
+        fit_and_score_kwargs = dict(scorer=scorers,
+                                    fit_params=fit_params,
+                                    return_train_score=self.return_train_score,
+                                    return_n_test_samples=True,
+                                    return_times=True,
+                                    return_parameters=False,
+                                    error_score=self.error_score,
+                                    verbose=self.verbose)
+        results = {}
+        with parallel:
+            all_candidate_params = []
+            all_out = []
+            all_more_results = defaultdict(list)
+
+            def evaluate_candidates(candidate_params, cv=None,
+                                    more_results=None):
+                cv = cv or cv_orig
+                candidate_params = list(candidate_params)
+                n_candidates = len(candidate_params)
+
+                if self.verbose > 0:
+                    print("Fitting {0} folds for each of {1} candidates,"
+                          " totalling {2} fits".format(
+                              n_splits, n_candidates, n_candidates * n_splits))
+
+                out = parallel(delayed(_fit_and_score_eval_set)(
+                                        eval_set_selection, transformer,
+                                        clone(base_estimator),
+                                        X, y,
+                                        train=train, test=test,
+                                        parameters=parameters,
+                                        split_progress=(
+                                            split_idx,
+                                            n_splits),
+                                        candidate_progress=(
+                                            cand_idx,
+                                            n_candidates),
+                                        print_message=f'cand={cand_idx}/{n_candidates}, cv={split_idx}: {parameters}',
+                                        **fit_and_score_kwargs)
+                               for (cand_idx, parameters),
+                                   (split_idx, (train, test)) in product(
+                                   enumerate(candidate_params),
+                                   enumerate(cv.split(X, y, groups))))
+
+                if len(out) < 1:
+                    raise ValueError('No fits were performed. '
+                                     'Was the CV iterator empty? '
+                                     'Were there no candidates?')
+                elif len(out) != n_candidates * n_splits:
+                    raise ValueError('cv.split and cv.get_n_splits returned '
+                                     'inconsistent results. Expected {} '
+                                     'splits, got {}'
+                                     .format(n_splits,
+                                             len(out) // n_candidates))
+
+                # For callable self.scoring, the return type is only know after
+                # calling. If the return type is a dictionary, the error scores
+                # can now be inserted with the correct key. The type checking
+                # of out will be done in `_insert_error_scores`.
+                if callable(self.scoring):
+                    _insert_error_scores(out, self.error_score)
+                all_candidate_params.extend(candidate_params)
+                all_out.extend(out)
+                if more_results is not None:
+                    for key, value in more_results.items():
+                        all_more_results[key].extend(value)
+
+                nonlocal results
+                results = self._format_results(
+                    all_candidate_params, n_splits, all_out,
+                    all_more_results)
+
+                return results
+
+            self._run_search(evaluate_candidates)
+
+            # multimetric is determined here because in the case of a callable
+            # self.scoring the return type is only known after calling
+            first_test_score = all_out[0]['test_scores']
+            self.multimetric_ = isinstance(first_test_score, dict)
+
+            # check refit_metric now for a callabe scorer that is multimetric
+            if callable(self.scoring) and self.multimetric_:
+                self._check_refit_for_multimetric(first_test_score)
+                refit_metric = self.refit
+
+        # For multi-metric evaluation, store the best_index_, best_params_ and
+        # best_score_ iff refit is one of the scorer names
+        # In single metric evaluation, refit_metric is "score"
+        if self.refit or not self.multimetric_:
+            # If callable, refit is expected to return the index of the best
+            # parameter set.
+            if callable(self.refit):
+                self.best_index_ = self.refit(results)
+                if not isinstance(self.best_index_, numbers.Integral):
+                    raise TypeError('best_index_ returned is not an integer')
+                if (self.best_index_ < 0 or
+                   self.best_index_ >= len(results["params"])):
+                    raise IndexError('best_index_ index out of range')
+            else:
+                self.best_index_ = results["rank_test_%s"
+                                           % refit_metric].argmin()
+                self.best_score_ = results["mean_test_%s" % refit_metric][
+                                           self.best_index_]
+            self.best_params_ = results["params"][self.best_index_]
+
+        if self.refit:
+            # we clone again after setting params in case some
+            # of the params are estimators as well.
+            self.best_estimator_ = clone(clone(base_estimator).set_params(
+                **self.best_params_))
+            refit_start_time = time.time()
+            if y is not None:
+                self.best_estimator_.fit(X, y, **fit_params)
+            else:
+                self.best_estimator_.fit(X, **fit_params)
+            refit_end_time = time.time()
+            self.refit_time_ = refit_end_time - refit_start_time
+
+        # Store the only scorer not as a dict for single metric evaluation
+        self.scorer_ = scorers
+
+        self.cv_results_ = results
+        self.n_splits_ = n_splits
+
         return self
```

### Comparing `seaborn-analyzer-0.2.9/seaborn_analyzer/custom_class_plot.py` & `seaborn-analyzer-0.3.0/seaborn_analyzer/custom_class_plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1452 +1,1452 @@
-from typing import List
-import matplotlib.pyplot as plt
-import numbers
-import numpy as np
-import pandas as pd
-from scipy import stats
-from sklearn.metrics import auc, plot_roc_curve, roc_curve, RocCurveDisplay
-from sklearn.model_selection import KFold, LeaveOneOut, GroupKFold, LeaveOneGroupOut
-from sklearn.preprocessing import label_binarize
-from matplotlib import colors
-import copy
-import decimal
-
-from .multiclass_fitparams import OneVsRestClassifierPatched
-from ._cv_eval_set import init_eval_set, _make_transformer, _eval_set_selection
-
-class classplot():
-    # 散布図カラーリスト
-    _SCATTER_COLORS = ['green', 'red', 'mediumblue', 'brown', 'darkmagenta', 'darkorange', 'gold', 'grey']
-    # クラス確率図カラーマップ
-    _PROB_CMAP = ['Greens', 'Reds', 'Blues', 'YlOrBr', 'Purples', 'OrRd', 'Wistia', 'Greys']
-    # デフォルトでの決定境界図の透明度(alpha)
-    _DEFAULT_SEPARATOR_ALPHA = 0.3
-    # デフォルトでのクラス確率図等高線モードの透明度(alpha)
-    _DEFAULT_PROBA_CONTOURF_ALPHA = 0.5
-    # デフォルトでのクラス確率図透明度補正シグモイド関数のゲイン
-    _DEFAULT_PROBA_CONTOURF_SIG_GAIN = 0.5
-    # デフォルトでのクラス確率図の等高線段階数
-    _DEFAULT_PROBA_CONTOURF_LEVELS = 10
-    # デフォルトでのクラス確率図RGB画像モードの透明度(alpha)
-    _DEFAULT_PROBA_RGB_ALPHA = 0.45
-
-    def _round_digits(src: float, rounddigit: int = None, method='decimal'):
-        """
-        指定桁数で小数を丸める
-
-        Parameters
-        ----------
-        src : float
-            丸め対象の数値
-        rounddigit : int
-            フィッティング線の表示範囲（標準偏差の何倍まで表示するか指定）
-        method : int
-            桁数決定手法（'decimal':小数点以下, 'sig':有効数字(Decimal指定), 'format':formatで有効桁数指定）
-        """
-        if method == 'decimal':
-            return round(src, rounddigit)
-        elif method == 'sig':
-            with decimal.localcontext() as ctx:
-                ctx.prec = rounddigit
-                return ctx.create_decimal(src)
-        elif method == 'format':
-            return '{:.{width}g}'.format(src, width=rounddigit)
-    
-    def _reshape_input_data(x, y, data, x_colnames, cv_group):
-        """
-        入力データの形式統一(pd.DataFrame or np.ndarray)
-        """
-        # dataがpd.DataFrameのとき
-        if isinstance(data, pd.DataFrame):
-            if not isinstance(x, list):
-                raise Exception('`x` argument should be list[str] if `data` is pd.DataFrame')
-            if not isinstance(y, str):
-                raise Exception('`y` argument should be str if `data` is pd.DataFrame')
-            if x_colnames is not None:
-                raise Exception('`x_colnames` argument should be None if `data` is pd.DataFrame')
-            X = data[x].values
-            y_true = data[y].values
-            x_colnames = x
-            y_colname = y
-            cv_group_colname = cv_group
-            
-        # dataがNoneのとき(x, y, cv_groupがnp.ndarray)
-        elif data is None:
-            if not isinstance(x, np.ndarray):
-                raise Exception('`x` argument should be np.ndarray if `data` is None')
-            if not isinstance(y, np.ndarray):
-                raise Exception('`y` argument should be np.ndarray if `data` is None')
-            X = x if len(x.shape) == 2 else x.reshape([x.shape[0], 1])
-            y_true = y.ravel()
-            # x_colnameとXの整合性確認
-            if x_colnames is None:
-                x_colnames = list(range(X.shape[1]))
-            elif X.shape[1] != len(x_colnames):
-                raise Exception('width of X must be equal to length of x_colnames')
-            else:
-                x_colnames = x_colnames
-            y_colname = 'objective_variable'
-            if cv_group is not None:  # cv_group指定時
-                cv_group_colname = 'group'
-                data = pd.DataFrame(np.column_stack((X, y_true, cv_group)),
-                                    columns=x_colnames + [y_colname] + [cv_group_colname])
-            else:
-                cv_group_colname = None
-                data = pd.DataFrame(np.column_stack((X, y)),
-                                    columns=x_colnames + [y_colname])
-        else:
-            raise Exception('`data` argument should be pd.DataFrame or None')
-
-        return X, y_true, data, x_colnames, y_colname, cv_group_colname
-
-    @classmethod
-    def _chart_plot_2d(cls, trained_clf, x_chart, y_true_col, y_pred_col, data, x_chart_indices,
-                       x1_start, x1_end, x2_start, x2_end, other_x, chart_scale,
-                       proba_pred_col, proba_class_indices, ax, plot_border, plot_scatter,
-                       scatter_color_dict, scatter_marker_dict, proba_cmap_dict, proba_type,
-                       contourf_kws=None, imshow_kws=None, scatter_kws=None, legend_kws=None):
-        """
-        分類チャート（決定境界図 or クラス確率図）と各種散布図の表示
-        (class_separator_plotあるいはclass_prob_plotメソッドの描画処理部分)
-        """
-        # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
-        if ax is None:
-            ax=plt.gca()
-
-        # 図のサイズからグリッド数を取得
-        xnum, ynum = plt.gcf().dpi * plt.gcf().get_size_inches()
-        # チャート用グリッドデータを作成
-        xx = np.linspace(x1_start, x1_end, num=int(xnum/chart_scale))
-        yy = np.linspace(x2_start, x2_end, num=int(ynum/chart_scale))
-        X1, X2 = np.meshgrid(xx, yy)
-        X_grid = np.c_[X1.ravel(), X2.ravel()]
-        # 推論用に全説明変数を保持したndarrayを作成 (チャート非使用変数は固定値other_xとして追加)
-        n_rows = X_grid.shape[0]
-        X_all = []
-        other_add_flg = False
-        for i in range(2 + len(other_x)):
-            if i == x_chart_indices[0]: # チャート使用変数(1個目)を追加
-                X_all.append(X_grid[:, 0].reshape(n_rows, 1))
-            elif i == x_chart_indices[1]: # チャート使用変数(2個目)を追加
-                X_all.append(X_grid[:, 1].reshape(n_rows, 1))
-            elif len(other_x) >= 1 and not other_add_flg:  # チャート非使用変数(1個目)を固定値として追加
-                X_all.append(np.full((n_rows, 1), other_x[0]))
-                other_add_flg = True
-            elif len(other_x) == 2:  # チャート非使用変数(2個目)を固定値として追加
-                X_all.append(np.full((n_rows, 1), other_x[1]))
-        X_all = np.hstack(X_all)
-
-        # グリッドデータに対して推論し、推定値を作成
-        y_pred_grid = trained_clf.predict(X_all)
-        # 推定値をint型に変換
-        class_int_dict = dict(zip(scatter_color_dict.keys(), range(len(scatter_color_dict))))
-        y_pred_grid_int = np.vectorize(lambda x: class_int_dict[x])(y_pred_grid)
-        # グリッドデータをピボット化
-        y_pred_pivot = y_pred_grid_int.reshape(X1.shape)
-
-        # 決定境界図をプロット
-        if proba_pred_col is None:
-            # 決定境界色分けプロット
-            ax.contourf(X1, X2, y_pred_pivot,
-                        levels=np.arange(y_pred_pivot.max() + 2) - 0.5,
-                        **contourf_kws)
-
-        # クラス確率図をプロット
-        else:
-            # クラス数
-            nclass = len(proba_class_indices)
-            # グリッドデータに対してクラス確率算出
-            y_proba_grid = trained_clf.predict_proba(X_all)[:, proba_class_indices]
-
-            # contourfで等高線プロット（塗りつぶしあり）するとき
-            if proba_type == 'contourf':
-                # alpha値を保持(描画終了後に更新前に戻すため)
-                src_alpha = contourf_kws['alpha']
-                # シグモイド関数(クラス数1のときalphaで、クラス数∞のとき1に漸近)でalphaを補正
-                contourf_kws['alpha'] = 2*(1-src_alpha)/(1+np.exp(-cls._DEFAULT_PROBA_CONTOURF_SIG_GAIN*(nclass-1)))+2*src_alpha-1
-                # クラスごとに処理
-                for i in range(nclass):
-                    # グリッドデータから該当クラスのみ抜き出してピボット化
-                    y_proba_pivot = y_proba_grid[:, i].reshape(X1.shape)
-                    # カラーマップをproba_cmap_dictの値から取得
-                    cmap = list(proba_cmap_dict.values())[i]
-                    # クラス確率図プロット
-                    ax.contourf(X1, X2, y_proba_pivot,
-                                cmap=cmap,
-                                **contourf_kws)
-                    # alpha値を更新(alpha/(1+alpha))
-                    old_alpha = contourf_kws['alpha']
-                    contourf_kws['alpha'] = old_alpha / (1 + old_alpha)
-                # alpha値を更新前に戻す
-                contourf_kws['alpha'] = src_alpha
-            
-            # contourで等高線プロット（塗りつぶしなし）するとき
-            elif proba_type == 'contour':
-                # クラスごとに処理
-                for i in range(nclass):
-                    # グリッドデータから該当クラスのみ抜き出してピボット化
-                    y_proba_pivot = y_proba_grid[:, i].reshape(X1.shape)
-                    # 線の色をscatter_color_dictの値から取得
-                    cmap = list(proba_cmap_dict.values())[i]
-                    #c=list(scatter_color_dict.values())[proba_class_indices[i]]
-                    ax.contour(X1, X2, y_proba_pivot,
-                               cmap=cmap,
-                               **contourf_kws)
-            
-            # imshowでRGB画像プロットするとき
-            elif proba_type == 'imshow':
-                # いったんRGB各色ゼロで埋める
-                proba_g = np.zeros(X1.shape)  # 緑
-                proba_r = np.zeros(X1.shape)  # 赤
-                proba_b = np.zeros(X1.shape)  # 青
-                # RGBいずれかのカラーマップを持つクラスが存在すれば、そのクラスの確率を格納
-                for i, cmap in enumerate(proba_cmap_dict.values()):
-                    if cmap == 'Greens':
-                        proba_g = y_proba_grid[:, i].reshape(X1.shape)
-                    elif cmap == 'Reds':
-                        proba_r = y_proba_grid[:, i].reshape(X1.shape)
-                    elif cmap == 'Blues':
-                        proba_b = y_proba_grid[:, i].reshape(X1.shape)
-                    else:
-                        # imshowのとき、Greens, Reds, Blues以外のカラーマップを指定したらエラーを出す(4クラス以上は描画不可)
-                        raise Exception('only "Greens, Reds, Blues" cmap are allowd if the "proba_type" argument is "imshow"')
-                # RGBのデータを合体して上下反転
-                im_grid = np.flip(np.stack([proba_r, proba_g, proba_b], 2), axis=0)
-                # RGB画像をプロット
-                ax.imshow(im_grid,
-                          aspect="auto", extent=(x1_start, x1_end, x2_start, x2_end),
-                          **imshow_kws)
-            else:
-                raise Exception('the "proba_type" argument must be "contourf", "contour" or "imshow"')
-
-        # 境界線をプロット
-        if plot_border:
-            ax.contour(X1, X2, y_pred_pivot,
-                       levels=np.arange(y_pred_pivot.max() + 2) - 0.5,
-                       colors='k',
-                       linewidths=0.5,
-                       antialiased=True)
-
-        # 散布図をプロット
-        if plot_scatter is not None:
-            # マーカの縁の色未指定のとき、dimgreyを指定
-            if 'edgecolors' not in scatter_kws.keys():
-                scatter_kws['edgecolors'] = 'dimgrey'
-            # 正誤を判定
-            data['error'] = (data[y_true_col] == data[y_pred_col])
-            # 色分け
-            if plot_scatter == 'error':  # 正誤で色分け
-                cdict = {True:'blue', False:'red'}
-                for name, group in data.groupby('error'):
-                    ax.scatter(group[x_chart[0]].values, group[x_chart[1]].values,
-                               label=name, c=cdict[name],
-                               marker=scatter_marker_dict[name],
-                               **scatter_kws)
-            elif plot_scatter == 'class':  # クラスで色分け
-                for name, group in data.groupby(y_true_col):
-                    ax.scatter(group[x_chart[0]].values, group[x_chart[1]].values,
-                               label=name, c=scatter_color_dict[name],
-                               **scatter_kws)
-            elif plot_scatter == 'class_error':  # クラスと正誤で色分け
-                for name, group in data.groupby([y_true_col, 'error']):
-                    ax.scatter(group[x_chart[0]].values, group[x_chart[1]].values,
-                               label=f'{name[0]}   {name[1]}', c=scatter_color_dict[name[0]],
-                               marker=scatter_marker_dict[name[1]],
-                               **scatter_kws)
-            # 凡例表示
-            ax.legend(**legend_kws)
-
-        # 軸ラベルを追加
-        ax.set_xlabel(x_chart[0])
-        ax.set_ylabel(x_chart[1])
-
-    @classmethod
-    def _class_chart_plot(cls, trained_clf, X, y_pred, y_true, x_chart, x_not_chart, x_chart_indices,
-                       pair_sigmarange=2.0, pair_sigmainterval=0.5, chart_extendsigma=0.5, chart_scale=1,
-                       proba_pred = None, proba_class_indices = None, plot_border=True, plot_scatter='class', 
-                       scatter_color_dict=None, scatter_marker_dict=None, proba_cmap_dict=None, proba_type=None,
-                       rounddigit_x3=None, cv_index=None,
-                       subplot_kws=None, contourf_kws=None, imshow_kws=None, scatter_kws=None, legend_kws=None):
-        """
-        分類チャート（決定境界図 or クラス確率図）表示の、説明変数の数に応じた分岐処理
-        (class_separator_plotあるいはclass_prob_plotメソッド処理のうち、説明変数の数に応じたデータ分割等を行う)
-        """
-        # 説明変数の数
-        x_num = X.shape[1]
-        # チャート（決定境界図 or クラス確率図）使用DataFrame
-        df_chart = pd.DataFrame(X[:, x_chart_indices], columns=x_chart)
-        # チャート非使用DataFrame
-        X_not_chart = X[:, [i for i in range(X.shape[1]) if i not in x_chart_indices]]
-        df_not_chart = pd.DataFrame(X_not_chart, columns=x_not_chart)
-        # 結合＆目的変数実測値と予測値追加
-        df_all = df_chart.join(df_not_chart)
-        df_all = df_all.join(pd.DataFrame(y_true, columns=['y_true']))
-        df_all = df_all.join(pd.DataFrame(y_pred, columns=['y_pred']))
-        # クラス確率追加（クラス確率図プロット時のみ）
-        if proba_pred is not None:
-            proba_pred_col = list(proba_cmap_dict.keys())
-            df_all = df_all.join(pd.DataFrame(proba_pred, columns=[proba_pred_col]))
-        else:
-            proba_pred_col = None
-        # チャート非使用変数を標準化してDataFrameに追加
-        if x_num >= 3:
-            X_not_chart_norm = stats.zscore(df_not_chart)
-            if isinstance(X_not_chart_norm, pd.DataFrame):  # X_not_chart_normがDataFrameの時
-                not_chart_rename_dir = {c: f'normalize_{c}' for c in df_not_chart}
-                df_all = df_all.join(X_not_chart_norm.rename(columns=not_chart_rename_dir))
-            else:  # X_not_chart_normがndarrayの時（古いscipyのバージョン時）
-                df_all = df_all.join(pd.DataFrame(X_not_chart_norm, columns=[f'normalize_{c}' for c in df_not_chart]))
-
-        # チャートのX1軸およびX2軸の表示範囲(最大最小値 + extendsigma)
-        x1_min = np.min(X[:, x_chart_indices[0]])
-        x1_max = np.max(X[:, x_chart_indices[0]])
-        x1_std = np.std(X[:, x_chart_indices[0]])
-        x1_start = x1_min - x1_std * chart_extendsigma
-        x1_end = x1_max + x1_std * chart_extendsigma
-        x2_min = np.min(X[:, x_chart_indices[1]])
-        x2_max = np.max(X[:, x_chart_indices[1]])
-        x2_std = np.std(X[:, x_chart_indices[1]])
-        x2_start = x2_min - x2_std * chart_extendsigma
-        x2_end = x2_max + x2_std * chart_extendsigma
-
-        # プロットする図の数(sigmarange外「2枚」 + sigmarange内「int(pair_sigmarange / pair_sigmainterval) * 2枚」)
-        pair_n = int(pair_sigmarange / pair_sigmainterval) * 2 + 2
-        # チャート非使用変数をプロットする範囲の下限(標準化後)
-        pair_min = -(pair_n - 2) / 2 * pair_sigmainterval
-
-        # 説明変数が2次元のとき (図は1枚のみ)
-        if x_num == 2:
-            pair_w = 1
-            pair_h = 1
-        # 説明変数が3次元のとき (図はpair_n × 1枚)
-        elif x_num == 3:
-            pair_w = 1
-            pair_h = pair_n
-        # 説明変数が4次元のとき (図はpair_n × pair_n枚)
-        elif x_num == 4:
-            pair_w = pair_n
-            pair_h = pair_n
-
-        # figsize (全ての図全体のサイズ)指定
-        if 'figsize' not in subplot_kws.keys():
-            subplot_kws['figsize'] = (pair_w * 6, pair_h * 5)
-        # プロット用のaxes作成
-        fig, axes = plt.subplots(pair_h, pair_w, **subplot_kws)
-        if cv_index is not None:
-            fig.suptitle(f'CV {cv_index}')
-
-        # 図ごとにプロット
-        for i in range(pair_h):
-            for j in range(pair_w):
-                # pair縦軸変数(標準化後)の最小値
-                if i == 0:
-                    h_min = -float('inf')
-                    h_mean = pair_min - pair_sigmainterval / 2  # チャート非使用変数指定用の平均値
-                else:
-                    h_min = pair_min + (i - 1) * pair_sigmainterval
-                    h_mean = pair_min + (i - 0.5) * pair_sigmainterval  # チャート非使用変数指定用の平均値
-                # pair縦軸変数(標準化後)の最大値
-                if i == pair_h - 1:
-                    h_max = float('inf')
-                else:
-                    h_max = pair_min + i * pair_sigmainterval
-                # pair横軸変数(標準化後)の最小値
-                if j == 0:
-                    w_min = -float('inf')
-                    w_mean = pair_min - pair_sigmainterval / 2  # チャート非使用変数指定用の平均値
-                else:
-                    w_min = pair_min + (j - 1) * pair_sigmainterval
-                    w_mean = pair_min + (j - 0.5) * pair_sigmainterval  # チャート非使用変数指定用の平均値
-                # pair横軸変数(標準化後)の最大値
-                if j == pair_w - 1:
-                    w_max = float('inf')
-                else:
-                    w_max = pair_min + j * pair_sigmainterval
-
-                # 説明変数が2次元のとき (図は1枚のみ)
-                if x_num == 2:
-                    ax = axes
-                    df_pair = df_all.copy()
-                    other_x = []
-                # 説明変数が3次元のとき (図はpair_n × 1枚)
-                elif x_num == 3:
-                    ax = axes[i]
-                    # 縦軸変数範囲内のみのデータを抽出
-                    df_pair = df_all[(df_all[f'normalize_{x_not_chart[0]}'] >= h_min) & (df_all[f'normalize_{x_not_chart[0]}'] < h_max)].copy()
-                    # 決定境界図非使用変数の標準化逆変換
-                    x3_mean = np.mean(X_not_chart[:, 0])
-                    x3_std = np.std(X_not_chart[:, 0])
-                    other_x = [h_mean * x3_std + x3_mean]
-                # 説明変数が4次元のとき (図はpair_n × pair_n枚)
-                elif x_num == 4:
-                    ax = axes[j, i]
-                    # 縦軸変数範囲内のみのデータを抽出
-                    df_pair = df_all[(df_all[f'normalize_{x_not_chart[0]}'] >= h_min) & (df_all[f'normalize_{x_not_chart[0]}'] < h_max)].copy()
-                    # 横軸変数範囲内のみのデータを抽出
-                    df_pair = df_pair[(df_pair[f'normalize_{x_not_chart[1]}'] >= w_min) & (df_pair[f'normalize_{x_not_chart[1]}'] < w_max)]
-                    # チャート非使用変数の標準化逆変換
-                    x3_mean = np.mean(X_not_chart[:, 0])
-                    x3_std = np.std(X_not_chart[:, 0])
-                    x4_mean = np.mean(X_not_chart[:, 1])
-                    x4_std = np.std(X_not_chart[:, 1])
-                    other_x = [h_mean * x3_std + x3_mean, w_mean * x4_std + x4_mean]
-                
-                cls._chart_plot_2d(trained_clf, x_chart, 'y_true', 'y_pred', df_pair, x_chart_indices,
-                                      x1_start, x1_end, x2_start, x2_end, other_x, chart_scale,
-                                      proba_pred_col, proba_class_indices, ax, plot_border, plot_scatter,
-                                      scatter_color_dict, scatter_marker_dict, proba_cmap_dict,  proba_type,
-                                      contourf_kws=contourf_kws, imshow_kws=imshow_kws, scatter_kws=scatter_kws,
-                                      legend_kws=legend_kws)
-
-                # グラフタイトルとして、チャート非使用変数の範囲を記載（説明変数が3次元以上のとき）
-                if x_num == 3:
-                    if i == 0:
-                        ax.set_title(f'{x_not_chart[0]}=- {cls._round_digits(h_max * x3_std + x3_mean, rounddigit=rounddigit_x3)} (- {h_max}σ)')
-                    elif i == pair_h - 1:
-                        ax.set_title(f'{x_not_chart[0]}={cls._round_digits(h_min * x3_std + x3_mean, rounddigit=rounddigit_x3)} - ({h_min}σ -)')
-                    else:
-                        ax.set_title(f'{x_not_chart[0]}={cls._round_digits(h_min * x3_std + x3_mean, rounddigit=rounddigit_x3)} - {cls._round_digits(h_max * x3_std + x3_mean, rounddigit=rounddigit_x3)} ({h_min}σ - {h_max}σ)')
-                if x_num == 4:
-                    ax.set_title(f'{x_not_chart[0]}= {h_min}σ - {h_max}σ  {x_not_chart[1]}= {w_min}σ - {w_max}σ')
-
-        # 字が重なるのでtight_layoutにする
-        plt.tight_layout()
-
-    @classmethod
-    def class_separator_plot(cls, clf, x: List[str], y: str, data: pd.DataFrame = None,
-                             x_colnames: List[str] = None, x_chart: List[str] = None,
-                             pair_sigmarange = 1.0, pair_sigmainterval = 0.5, chart_extendsigma = 0.5, chart_scale = 1,
-                             plot_scatter = 'class_error', rounddigit_x3 = 2,
-                             scatter_colors = None, true_marker = 'o', false_marker = 'x',
-                             cv=None, cv_seed=42, cv_group=None, display_cv_indices = 0,
-                             clf_params=None, fit_params=None, eval_set_selection=None,
-                             subplot_kws=None, contourf_kws=None, scatter_kws=None, legend_kws=None):
-        """
-        Plot class separation lines of any scikit-learn classifier with 2 to 4D explanatory variables.
-
-        Parameters
-        ----------
-        clf: classifier object implementing ``fit``
-            Classifier. This is assumed to implement the scikit-learn estimator interface.
-
-        x : list[str], or np.ndarray
-            Explanatory variables. Should be list[str] if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
-
-        y : str or np.ndarray
-            Objective variable. Should be str if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
-
-        data: pd.DataFrame
-            Input data structure.
-
-        x_colnames: list[str], optional
-            Names of explanatory variables. Available only if ``data`` is NOT pd.DataFrame
-
-        x_chart: list[str], optional
-            X-axis . If None, use two variables in ``x`` from the front.
-
-        pair_sigmarange: float, optional
-            Set the range of subplots. The lower limit is mean({x3, x4}) - ``pair_sigmarange`` * std({x3, x4}). The higher limit is mean({x3, x4}) + ``pair_sigmarange`` * std({x3, x4}). Available only if len(x) is bigger than 2.
-
-        pair_sigmainterval: float, optional
-            Set the interval of subplots. For example, if ``pair_sigmainterval`` is set to 0.5 and ``pair_sigmarange`` is set to 1.0, The ranges of subplots are lower than μ-1σ, μ-1σ to μ-0.5σ, μ-0.5σ to μ, μ to μ+0.5σ, μ+0.5σ to μ+1σ, and higher than μ+1σ. Available only if len(x) is bigger than 2.
-
-        chart_extendsigma: float, optional
-            Set the axis view limits of the separation map. The lower limit is min({x1, x2}) - std({x1, x2}) * chart_extendsigma. The higher limit is max({x1, x2}) + std({x1, x2}) * chart_extendsigma
-
-        chart_scale: int, optional
-            Set the resolution of the separation lines. If plotting speed is slow, we reccomend setting chart_scale to 2. We DON'T reccomend setting it to larger than 3 because of jaggies.
-
-        plot_scatter: {'error', 'class', 'class_error', None}, optional
-            Color decision of scatter plot. If 'error', to be mapped to colors using true-false. If 'class', to be mapped to colors using class labels. If 'class_error', to be mapped to colors using class labels and marker styles using true-false. If None, no scatter.
-
-        rounddigit_x3: int, optional
-            Round a number of y-axis valiable of subplots to a given precision in decimal digits.
-
-        scatter_colors: list[str], optional
-            Set of colors for mapping the class labels. Available only if ``plot_scatter`` is set to 'class' or 'class_error'.
-
-        true_marker: str, optional
-            Marker style of True label. Available only if ``plot_scatter`` is set to 'error' or 'class_error'. See https://matplotlib.org/stable/api/markers_api.html#module-matplotlib.markers
-
-        false_marker: str, optional
-            Marker style of False label. Available only if ``plot_scatter`` is set to 'error' or 'class_error'. See https://matplotlib.org/stable/api/markers_api.html#module-matplotlib.markers
-
-        cv : int, cross-validation generator, or an iterable, optional
-            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
-
-        cv_seed: int, optional
-            Seed for random number generator of cross validation.
-
-        cv_group: str, optional
-            Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
-
-        display_cv_indices: int, optional
-            Cross validation index or indices to display.
-
-        clf_params: dict, optional
-            Parameters passed to the classifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
-
-        fit_params: dict, optional
-            Parameters passed to the fit() method of the classifier, e.g. ``early_stopping_round`` and ``eval_set`` of XGBClassifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
-        
-        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
-
-            If "test", select test data from `X` and `y` using cv.split().
-
-            If "original", use raw `eval_set`.
-
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
-
-        subplot_kws: dict, optional
-            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize.`` See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
-
-        contourf_kws: dict, optional
-            Additional parameters passed to matplotlib.pyplot.contourf(), e.g. ``alpha``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.contourf.html
-
-        scatter_kws: dict, optional
-            Additional parameters passed to matplotlib.pyplot.scatter(), e.g. ``alpha``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.scatter.html
-
-        legend_kws : dict
-            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
-        """
-
-        # 入力データの形式統一
-        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data(x, y, data,
-                                                                                           x_colnames,
-                                                                                           cv_group)
-        # 説明変数xの次元が2～4以外ならエラーを出す
-        if len(x_colnames) < 2 or len(x_colnames) > 4:
-            raise Exception('Dimension of x must be 2 to 4')
-        
-        # display_cv_indicesをList化
-        if isinstance(display_cv_indices, int):
-            display_cv_indices = [display_cv_indices]
-        elif not isinstance(x_colnames, list):
-            raise Exception('the "cv_display_num" argument must be int or List[int]')
-        # 学習器パラメータがあれば適用
-        if clf_params is not None:
-            clf.set_params(**clf_params)
-        # 学習時パラメータがNoneなら空のdictを入力
-        if fit_params is None:
-            fit_params = {}
-        # subplot_kwsがNoneなら空のdictを入力
-        if subplot_kws is None:
-            subplot_kws = {}
-        # contourf_kwsがNoneなら空のdictを入力
-        if contourf_kws is None:
-            contourf_kws = {}
-        # scatter_kwsがNoneなら空のdictを入力
-        if scatter_kws is None:
-            scatter_kws = {}
-        # legend_kwsがNoneなら空のdictを入力
-        if legend_kws is None:
-            legend_kws = {}
-        
-        # 決定境界図表示用の列を抽出
-        if x_chart is None:  # 列名指定していないとき、前から2列を抽出
-            x_chart = x_colnames[:2]
-            x_chart_indices = [0, 1]
-        else:  # 列名指定しているとき、該当列のXにおけるインデックス(0～3)を保持
-            if len(x_chart) != 2:
-                raise Exception('length of x_chart must be 2')
-            x_chart_indices = []
-            for colname in x_chart:
-                x_chart_indices.append(x_colnames.index(colname))
-        # 決定境界図表示以外の列
-        x_not_chart = [colname for colname in x_colnames if colname not in x_chart]
-
-        # クラス名と散布図色を紐づけ(色分けを全ての図で統一用)
-        if scatter_colors is None:
-            scatter_colors = cls._SCATTER_COLORS
-        class_list = data[y_colname].values.tolist()
-        class_list = sorted(set(class_list), key=class_list.index)
-        scatter_color_dict = dict(zip(class_list, scatter_colors[0:len(class_list)]))
-        # 散布図マーカー形状をdict化
-        scatter_marker_dict = {True: true_marker, False: false_marker}
-        # contourf_kwsにcolors指定ないとき、scatter_color_dictの値を使用
-        if 'colors' not in contourf_kws.keys():
-            contourf_kws['colors'] = list(scatter_color_dict.values())
-        # contourf_kwsにalphat指定ないとき、DEFAULT_SEPARATOR_ALPHAを使用
-        if 'alpha' not in contourf_kws.keys():
-            contourf_kws['alpha'] = cls._DEFAULT_SEPARATOR_ALPHA
-        
-        # クロスバリデーション有無で場合分け
-        # クロスバリデーション未実施時(学習データから学習してプロット)
-        if cv is None:
-            # 学習と推論
-            clf.fit(X, y_true, **fit_params)
-            y_pred = clf.predict(X)
-            # 決定境界図をプロット
-            cls._class_chart_plot(clf, X, y_pred, y_true, x_chart, x_not_chart, x_chart_indices,
-                               pair_sigmarange = pair_sigmarange, pair_sigmainterval=pair_sigmainterval, chart_extendsigma=chart_extendsigma, chart_scale=chart_scale,
-                               proba_pred = None, proba_class_indices = None, plot_border = True, plot_scatter = plot_scatter,
-                               scatter_color_dict=scatter_color_dict, scatter_marker_dict=scatter_marker_dict, proba_cmap_dict=None, proba_type=None,
-                               rounddigit_x3=rounddigit_x3, cv_index=None,
-                               subplot_kws=subplot_kws, contourf_kws=contourf_kws, imshow_kws=None, scatter_kws=scatter_kws, legend_kws=legend_kws)
-            
-        # クロスバリデーション実施時(分割ごとに別々にプロット＆指標算出)
-        if cv is not None:
-            # 分割法未指定時、cv_numとseedに基づきKFoldでランダムに分割
-            if isinstance(cv, numbers.Integral):
-                cv = KFold(n_splits=cv, shuffle=True, random_state=cv_seed)
-            # LeaveOneOutのときエラーを出す
-            if isinstance(cv, LeaveOneOut):
-                raise Exception('"regression_heat_plot" method does not support ``LeaveOneOut`` cross validation')
-            # cv_groupをグルーピング対象に指定(GroupKFold、LeaveOneGroupOut等)
-            split_kws={}
-            if cv_group_colname is not None:
-                split_kws['groups'] = data[cv_group_colname].values
-            elif isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
-                raise Exception('"GroupKFold" and "LeaveOneGroupOut" cross validations need ``cv_group`` argument')
-            # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
-            if isinstance(cv, LeaveOneGroupOut):
-                cv_num = len(set(data[cv_group_colname].values))
-            else:
-                cv_num = cv.n_splits
-
-            # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
-            if eval_set_selection is None:
-                eval_set_selection = 'test'
-            fit_params, eval_set_selection = init_eval_set(
-                    eval_set_selection, fit_params, X, y)
-            # 最終学習器以外の前処理変換器作成
-            transformer = _make_transformer(eval_set_selection, clf)
-
-            # クロスバリデーション
-            for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
-                # 表示対象以外のCVなら飛ばす
-                if i not in display_cv_indices:
-                    continue
-                print(f'cv_number={i}/{cv_num}')
-                # グラフタイトル(CV番号を指定。グルーピング系CVのときはグループ名を指定)
-                if isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
-                    cv_index = f'No.{i}  {cv_group_colname}={data[cv_group_colname].values[test][0]}'
-                else:
-                    cv_index = f'No.{i}'
-                # 表示用にテストデータと学習データ分割
-                X_train = X[train]
-                y_train = y_true[train]
-                X_test = X[test]
-                y_test = y_true[test]
-
-                # eval_setの中から学習データ or テストデータのみを抽出
-                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
-                                                        fit_params, train, test)
-
-                # 学習と推論
-                clf.fit(X_train, y_train, **fit_params_modified)
-                y_pred = clf.predict(X_test)
-                # 決定境界図をプロット
-                cls._class_chart_plot(clf, X_test, y_pred, y_test, x_chart, x_not_chart, x_chart_indices,
-                                   pair_sigmarange = pair_sigmarange, pair_sigmainterval = pair_sigmainterval, chart_extendsigma=chart_extendsigma, chart_scale=chart_scale,
-                                   proba_pred = None, proba_class_indices = None, plot_border = True, plot_scatter = plot_scatter,
-                                   scatter_color_dict=scatter_color_dict, scatter_marker_dict=scatter_marker_dict, proba_cmap_dict=None, proba_type=None,
-                                   rounddigit_x3=rounddigit_x3, cv_index=cv_index,
-                                   subplot_kws=subplot_kws, contourf_kws=contourf_kws, imshow_kws=None, scatter_kws=scatter_kws, legend_kws=legend_kws)
-
-    @classmethod
-    def class_proba_plot(cls, clf, x: List[str], y: str, data: pd.DataFrame = None,
-                         x_colnames: List[str] = None, x_chart: List[str] = None,
-                         pair_sigmarange = 1.0, pair_sigmainterval = 0.5, chart_extendsigma = 0.5, chart_scale = 1,
-                         plot_border = True, plot_scatter = 'class', rounddigit_x3 = 2,
-                         proba_class = None, proba_cmap_dict = None, proba_type = 'contourf',
-                         scatter_colors = None, true_marker = 'o', false_marker = 'x',
-                         cv=None, cv_seed=42, cv_group=None, display_cv_indices = 0,
-                         clf_params=None, fit_params=None, eval_set_selection=None,
-                         subplot_kws=None, contourf_kws=None, imshow_kws=None, scatter_kws=None, legend_kws=None):
-        """
-        Plot class prediction probability of any scikit-learn classifier with 2 to 4D explanatory variables.
-
-        Parameters
-        ----------
-        clf: classifier object implementing ``fit``
-            Classifier. This is assumed to implement the scikit-learn estimator interface.
-
-        x : list[str], or np.ndarray
-            Explanatory variables. Should be list[str] if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
-
-        y : str or np.ndarray
-            Objective variable. Should be str if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
-
-        data: pd.DataFrame, optional
-            Input data structure.
-
-        x_colnames: list[str], optional
-            Names of explanatory variables. Available only if ``data`` is NOT pd.DataFrame
-
-        x_chart: list[str], optional
-            X-axis and y-axis variables of separation map. If None, use two variables in ``x`` from the front.
-
-        pair_sigmarange: float, optional
-            Set the range of subplots. The lower limit is mean({x3, x4}) - ``pair_sigmarange`` * std({x3, x4}). The higher limit is mean({x3, x4}) + ``pair_sigmarange`` * std({x3, x4}). Available only if len(x) is bigger than 2.
-
-        pair_sigmainterval: float, optional
-            Set the interval of subplots. For example, if ``pair_sigmainterval`` is set to 0.5 and ``pair_sigmarange`` is set to 1.0, The ranges of subplots are lower than μ-1σ, μ-1σ to μ-0.5σ, μ-0.5σ to μ, μ to μ+0.5σ, μ+0.5σ to μ+1σ, and higher than μ+1σ. Available only if len(x) is bigger than 2.
-
-        chart_extendsigma: float, optional
-            Set the axis view limits of the separation map. The lower limit is min({x1, x2}) - std({x1, x2}) * ``chart_extendsigma``. The higher limit is max({x1, x2}) + std({x1, x2}) * ``chart_extendsigma``
-
-        chart_scale: int, optional
-            Set the resolution of the separation lines. If plotting speed is slow, we reccomend setting chart_scale to 2. We DON'T reccomend setting it to larger than 3 because of jaggies.
-
-        plot_border: bool, optional
-            If True, display class separation lines
-
-        plot_scatter: {'error', 'class', 'class_error', None}, optional
-            Color decision of scatter plot. If 'error', to be mapped to colors using true-false. If 'class', to be mapped to colors using class labels. If 'class_error', to be mapped to colors using class labels and marker styles using true-false. If None, no scatter.
-
-        rounddigit_x3: int, optional
-            Round a number of y-axis valiable of subplots to a given precision in decimal digits.
-
-        proba_class: str or list[str], optional
-            Class label name, in which probability map is displayed.
-
-        proba_cmap_dict: dict[str, str], optional
-            Colormap of probability map. The keys must be class label name and the values must be colormap names in Matplotlib. See https://matplotlib.org/stable/tutorials/colors/colormaps.html
-
-        proba_type: {'contourf', 'contour', 'imshow'}, optional
-            Plotting type of probabiliity map. If 'contourf', mapped by matplotlib.pyplot.contourf(). If 'contour', mapped by matplotlib.pyplot.contour(). If 'imshow', mapped by matplotlib.pyplot.imshow(). 'imshow' is available only if the number of class labels is less than 4.
-
-        scatter_colors: list[str], optional
-            Set of colors for mapping the class labels. Available only if ``plot_scatter`` is set to 'class' or 'class_error'.
-
-        true_marker: str, optional
-            Marker style of True label. Available only if ``plot_scatter`` is set to 'error' or 'class_error'. See https://matplotlib.org/stable/api/markers_api.html#module-matplotlib.markers
-
-        false_marker: str, optional
-            Marker style of False label. Available only if ``plot_scatter`` is set to 'error' or 'class_error'. See https://matplotlib.org/stable/api/markers_api.html#module-matplotlib.markers
-
-        cv: int or sklearn.model_selection.*, optional
-            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
-
-        cv_seed: int, optional
-            Seed for random number generator of cross validation.
-
-        cv_group: str, optional
-            Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
-
-        display_cv_indices: int, optional
-            Cross validation index or indices to display.
-
-        clf_params: dict, optional
-            Parameters passed to the classifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
-
-        fit_params: dict, optional
-            Parameters passed to the fit() method of the classifier, e.g. ``early_stopping_round`` and ``eval_set`` of XGBClassifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
-
-        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
-
-            If "test", select test data from `X` and `y` using cv.split().
-
-            If "original", use raw `eval_set`.
-
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
-
-        subplot_kws: dict, optional
-            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
-
-        contourf_kws: dict, optional
-            Additional parameters passed to matplotlib.pyplot.contourf() if proba_type is set to 'contourf', or additional parameters passed to matplotlib.pyplot.contour() if proba_type is set to 'contour'. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.contourf.html or https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.contour.html
-
-        imshow_kws: dict, optional
-            Additional parameters passed to matplotlib.pyplot.imshow(), e.g. ``alpha``. Available only if proba_type is set to 'imshow'. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.imshow.html
-
-        scatter_kws: dict, optional
-            Additional parameters passed to matplotlib.pyplot.scatter(), e.g. ``alpha``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.scatter.html
-
-        legend_kws : dict
-            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
-        """
-
-        # 入力データの形式統一
-        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data(x, y, data,
-                                                                                           x_colnames,
-                                                                                           cv_group)
-        # 説明変数xの次元が2～4以外ならエラーを出す
-        if len(x_colnames) < 2 or len(x_colnames) > 4:
-            raise Exception('Dimension of x must be 2 to 4')
-        
-        # display_cv_indicesをList化
-        if isinstance(display_cv_indices, int):
-            display_cv_indices = [display_cv_indices]
-        elif not isinstance(x_colnames, list):
-            raise Exception('the "cv_display_num" argument must be int or List[int]')
-        # 学習器パラメータがあれば適用
-        if clf_params is not None:
-            clf.set_params(**clf_params)
-        # 学習時パラメータがNoneなら空のdictを入力
-        if fit_params is None:
-            fit_params = {}
-        # subplot_kwsがNoneなら空のdictを入力
-        if subplot_kws is None:
-            subplot_kws = {}
-        # contourf_kwsがNoneなら空のdictを入力
-        if contourf_kws is None:
-            contourf_kws = {}
-        # imshow_kwsがNoneなら空のdictを入力
-        if imshow_kws is None:
-            imshow_kws = {}
-        # scatter_kwsがNoneなら空のdictを入力
-        if scatter_kws is None:
-            scatter_kws = {}
-        # legend_kwsがNoneなら空のdictを入力
-        if legend_kws is None:
-            legend_kws = {}
-
-        # クラス確率図表示用の列を抽出
-        if x_chart is None:  # 列名指定していないとき、前から2列を抽出
-            x_chart = x_colnames[:2]
-            x_chart_indices = [0, 1]
-        else:  # 列名指定しているとき、該当列のXにおけるインデックス(0～3)を保持
-            if len(x_chart) != 2:
-                raise Exception('length of x_chart must be 2')
-            x_chart_indices = []
-            for colname in x_chart:
-                x_chart_indices.append(x_colnames.index(colname))
-        # クラス確率図表示以外の列
-        x_not_chart = [colname for colname in x_colnames if colname not in x_chart]
-
-        # scatter_colors未指定のとき、デフォルト値を使用
-        if scatter_colors is None:
-            scatter_colors = cls._SCATTER_COLORS
-        # クラス名と散布図色を紐づけ(色分けを全ての図で統一用)
-        class_list = data[y_colname].values.tolist()
-        class_list = sorted(set(class_list), key=class_list.index)
-        scatter_color_dict = dict(zip(class_list, scatter_colors[0:len(class_list)]))
-        # 散布図マーカー形状をdict化
-        scatter_marker_dict = {True: true_marker, False: false_marker}
-
-        # proba_class未指定のとき、全てのクラスを使用
-        if proba_class is None:
-            proba_class = [c for c in class_list]
-        # proba_classをList化
-        if isinstance(proba_class, int) or isinstance(proba_class, str) or isinstance(proba_class, bool):
-            proba_class = [proba_class]
-        elif not isinstance(x_colnames, list):
-            raise Exception('the "proba_class" argument must be int, str, bool or List')
-        # List化したproba_classを走査してデータ上でのインデックスを取得
-        proba_class_indices = []
-        for pc in proba_class:
-            if pc not in class_list:  # 指定したproba_classがデータ上に存在しないとき、エラーを出す
-                raise Exception(f'"{proba_class}"" is not in the "{y_colname}" column')
-            proba_class_indices.append(class_list.index(pc))
-        # proba_cmap_dict未指定のとき、デフォルト値を使用
-        if proba_cmap_dict is None:
-            proba_cmap_dict = dict(zip(proba_class,
-                                       [cls._PROB_CMAP[pci] for pci in proba_class_indices]))
-        # proba_cmap_dictがproba_classと一致していないとき、エラーを出す
-        if list(proba_cmap_dict.keys()) != proba_class:
-            raise Exception(f'the keys of the "proba_cmap_dict" argument must be equal to the argument "proba_class"')
-
-        # contourf_kwsにalpha指定ないとき、DEFAULT_PROBA_CONTOURF_ALPHAを使用
-        if 'alpha' not in contourf_kws.keys():
-            contourf_kws['alpha'] = cls._DEFAULT_PROBA_CONTOURF_ALPHA
-        # contourf_kwsにlevels指定ないとき、DDEFAULT_PROBA_CONTOURF_LEVELSを使用
-        if 'levels' not in contourf_kws.keys():
-            contourf_kws['levels'] = cls._DEFAULT_PROBA_CONTOURF_LEVELS
-        # imshow_kwsにalpha指定ないとき、DEFAULT_PROBA_RGB_ALPHAを使用
-        if 'alpha' not in imshow_kws.keys():
-            imshow_kws['alpha'] = cls._DEFAULT_PROBA_RGB_ALPHA
-        
-        # クロスバリデーション有無で場合分け
-        # クロスバリデーション未実施時(学習データから学習してプロット)
-        if cv is None:
-            # 学習と推論
-            clf.fit(X, y_true, **fit_params)
-            y_pred = clf.predict(X)
-            # クラス確率を推定
-            proba_pred = clf.predict_proba(X)[:, proba_class_indices]
-            # TODO:クラス確率の順番が逆転した時の対策をメソッドとして実装する必要あり
-            # https://qiita.com/rawHam/items/3bcb6a68a533f2b82a85
-            # クラス確率図をプロット
-            cls._class_chart_plot(clf, X, y_pred, y_true, x_chart, x_not_chart, x_chart_indices,
-                                pair_sigmarange = pair_sigmarange, pair_sigmainterval=pair_sigmainterval, chart_extendsigma=chart_extendsigma, chart_scale=chart_scale,
-                                proba_pred = proba_pred, proba_class_indices = proba_class_indices, plot_border = plot_border, plot_scatter = plot_scatter,
-                                scatter_color_dict=scatter_color_dict, scatter_marker_dict=scatter_marker_dict, proba_cmap_dict=proba_cmap_dict, proba_type = proba_type,
-                                rounddigit_x3=rounddigit_x3, cv_index=None,
-                                subplot_kws=subplot_kws, contourf_kws=contourf_kws, imshow_kws=imshow_kws, scatter_kws=scatter_kws, legend_kws=legend_kws)
-            
-        # クロスバリデーション実施時(分割ごとに別々にプロット＆指標算出)
-        if cv is not None:
-            # 分割法未指定時、cv_numとseedに基づきKFoldでランダムに分割
-            if isinstance(cv, numbers.Integral):
-                cv = KFold(n_splits=cv, shuffle=True, random_state=cv_seed)
-            # LeaveOneOutのときエラーを出す
-            if isinstance(cv, LeaveOneOut):
-                raise Exception('"regression_heat_plot" method does not support "LeaveOneOut" cross validation')
-            # cv_groupをグルーピング対象に指定(GroupKFold、LeaveOneGroupOut等)
-            split_kws={}
-            if cv_group_colname is not None:
-                split_kws['groups'] = data[cv_group_colname].values
-            elif isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
-                raise Exception('"GroupKFold" and "LeaveOneGroupOut" cross validations need ``cv_group`` argument')
-            # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
-            if isinstance(cv, LeaveOneGroupOut):
-                cv_num = len(set(data[cv_group_colname].values))
-            else:
-                cv_num = cv.n_splits
-
-            # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
-            if eval_set_selection is None:
-                eval_set_selection = 'test'
-            fit_params, eval_set_selection = init_eval_set(
-                    eval_set_selection, fit_params, X, y)
-            # 最終学習器以外の前処理変換器作成
-            transformer = _make_transformer(eval_set_selection, clf)
-
-            # クロスバリデーション
-            for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
-                # 表示対象以外のCVなら飛ばす
-                if i not in display_cv_indices:
-                    continue
-                print(f'cv_number={i}/{cv_num}')
-                # グラフタイトル(CV番号を指定。グルーピング系CVのときはグループ名を指定)
-                if isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
-                    cv_index = f'No.{i}  {cv_group_colname}={data[cv_group_colname].values[test][0]}'
-                else:
-                    cv_index = f'No.{i}'
-                # 表示用にテストデータと学習データ分割
-                X_train = X[train]
-                y_train = y_true[train]
-                X_test = X[test]
-                y_test = y_true[test]
-                # proba_class_indicesを学習データから再取得（存在しなければ飛ばす）
-                class_list_train = y_train.tolist()
-                class_list_train = sorted(set(class_list_train), key=class_list_train.index)
-                proba_class_indices = [class_list_train.index(pc) for pc in proba_class if pc in class_list_train]
-                if len(proba_class_indices) == 0:
-                    print(f'there is no assigned "proba_class" in the train data')
-                    continue
-                # proba_cmap_dictも学習データから再取得
-                proba_cmap_dict = {k: v for k, v in proba_cmap_dict.items() if k in class_list_train}
-
-                # eval_setの中から学習データ or テストデータのみを抽出
-                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
-                                                        fit_params, train, test)
-
-                # 学習と推論
-                clf.fit(X_train, y_train, **fit_params_modified)
-                y_pred = clf.predict(X_test)
-                # クラス確率を推定
-                proba_pred = clf.predict_proba(X_test)[:, proba_class_indices]
-                # クラス確率図をプロット
-                cls._class_chart_plot(clf, X_test, y_pred, y_test, x_chart, x_not_chart, x_chart_indices,
-                                    pair_sigmarange = pair_sigmarange, pair_sigmainterval = pair_sigmainterval, chart_extendsigma=chart_extendsigma, chart_scale=chart_scale,
-                                    proba_pred = proba_pred, proba_class_indices = proba_class_indices, plot_border = plot_border, plot_scatter = plot_scatter,
-                                    scatter_color_dict=scatter_color_dict, scatter_marker_dict=scatter_marker_dict, proba_cmap_dict=proba_cmap_dict, proba_type = proba_type,
-                                    rounddigit_x3=rounddigit_x3, cv_index=cv_index,
-                                    subplot_kws=subplot_kws, contourf_kws=contourf_kws, imshow_kws=imshow_kws, scatter_kws=scatter_kws, legend_kws=legend_kws)
-    
-    @classmethod
-    def plot_roc_curve_multiclass(cls, estimator, X_train, y_train, *,
-                                  X_test=None, y_test=None,
-                                  sample_weight=None, drop_intermediate=True,
-                                  response_method="predict_proba", name=None, ax=None, pos_label=None,
-                                  average='macro', fit_params=None,
-                                  plot_roc_kws=None, class_average_kws=None,
-                                  ):
-        """Plot Receiver operating characteristic (ROC) curve.
-
-        Available both multiclass and binary classification
-
-        Extra keyword arguments will be passed to matplotlib's `plot`.
-
-        Parameters
-        ----------
-        estimator : estimator instance
-            Fitted classifier or a fitted :class:`~sklearn.pipeline.Pipeline`
-            in which the last estimator is a classifier.
-
-        X_train : {array-like, sparse matrix} of shape (n_samples, n_features)
-            Input values of train data.
-
-        y_train : array-like of shape (n_samples,)
-            Target values of train data.
-
-        X_test : {array-like, sparse matrix} of shape (n_samples, n_features)
-            Input values of test data.
-
-        y_test : array-like of shape (n_samples,)
-            Target values of test data.
-
-        sample_weight : array-like of shape (n_samples,), default=None
-            Sample weights.
-
-        drop_intermediate : boolean, default=True
-            Whether to drop some suboptimal thresholds which would not appear
-            on a plotted ROC curve. This is useful in order to create lighter
-            ROC curves.
-
-        response_method : {'predict_proba', 'decision_function'}, default='predict_proba'
-            Specifies whether to use for calcurating class probability.
-
-        name : str, default=None
-            Name of ROC Curve for labeling. If `None`, use the name of the
-            estimator.
-
-        ax : matplotlib axes, default=None
-            Axes object to plot on. If `None`, a new figure and axes is created.
-
-        pos_label : str or int, default=None
-            The class considered as the positive class when computing the roc auc
-            metrics. By default, `estimators.classes_[1]` is considered
-            as the positive class.
-
-        average : {'macro', 'micro'}, default='micro'
-            Specifies whether to use for calcurating average of tpr and fpr.
-
-        fit_params : dict, default=None
-            Parameters passed to the fit() method of the classifier, e.g. ``early_stopping_round`` and ``eval_set`` of XGBClassifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
-
-        plot_roc_kws : dict, optional
-            Additional parameters passed to matplotlib.pyplot.plot() that draws ROC curve of each classes, e.g. ``lw``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
-        
-        class_average_kws : dict, optional
-            Additional parameters passed to matplotlib.pyplot.plot() or sklearn.metrics.plot_roc_curve() that draws ROC curve of average, e.g. ``alpha``. See https://scikit-learn.org/stable/modules/generated/sklearn.metrics.plot_roc_curve.html
-
-        Returns
-        -------
-        display : :class:`~sklearn.metrics.RocCurveDisplay`
-            Object that stores computed values.
-        """
-
-        # X_testがNoneのとき、X_trainを使用
-        if X_test is None:
-            X_test = X_train
-        # y_testがNoneのとき、y_trainを使用
-        if y_test is None:
-            y_test = y_train
-        # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
-        if ax is None:
-            ax = plt.gca()
-        # 学習時パラメータがNoneなら空のdictを入力
-        if fit_params is None:
-            fit_params = {}
-        # plot_roc_kwsがNoneなら空のdictを入力
-        if plot_roc_kws is None:
-            plot_roc_kws = {}
-        # class_average_kwsがNoneなら空のdictを入力
-        if class_average_kws is None:
-            class_average_kws = {}
-        # 目的変数のクラス一覧
-        y_labels = sorted(np.unique(np.concatenate([y_train, y_test], 0)).tolist())
-        n_classes = len(y_labels)
-        
-        # 2クラス分類のとき
-        if n_classes == 2:
-            estimator.fit(X_train, y_train, **fit_params)
-            viz = plot_roc_curve(estimator, X_test, y_test,
-                                sample_weight=sample_weight, drop_intermediate=drop_intermediate,
-                                response_method=response_method, name=name, ax=ax, pos_label=pos_label,
-                                **class_average_kws
-                                )
-        # 多クラス分類のとき
-        elif n_classes >= 3:
-            # label_binarize()で目的変数を二値化
-            y_train_binarize = label_binarize(y_train, classes=y_labels)
-            y_test_binarize = label_binarize(y_test, classes=y_labels)
-            # fit_paramsにeval_setがあるとき、二値化
-            eval_sets = [v for v in fit_params.keys() if 'eval_set' in v]
-            if len(eval_sets) > 0 and fit_params[eval_sets[0]] is not None:
-                eval_set_y_binarized = label_binarize(fit_params[eval_sets[0]][0][1], classes=y_labels)
-            # fit_paramsをクラス数で分割
-            fit_params_list = []
-            for i in range(n_classes):
-                fit_params_cls = copy.deepcopy(fit_params)
-                # fit_paramsにeval_setがあるとき、二値化したものに置き換える
-                if len(eval_sets) > 0 and fit_params[eval_sets[0]] is not None:
-                    fit_params_cls[eval_sets[0]] = [(fit_params[eval_sets[0]][0][0], eval_set_y_binarized[:, i])]
-                fit_params_list.append(fit_params_cls)
-                
-            # One vs Restの分類器を作成
-            clf_ovr = OneVsRestClassifierPatched(estimator)
-            clf_ovr.fit(X_train, y_train_binarize,
-                        fit_params_list)
-            # predict_probaまたはdecision_functionでクラス確率を取得
-            if response_method == 'predict_proba':
-                y_score = clf_ovr.predict_proba(X_test)
-            elif response_method == 'decision_function':
-                y_score = clf_ovr.decision_function(X_test)
-            else:
-                raise Exception('The `response_method` argument should be `predict_proba` or `decision_function`')
-            # クラスごとのROC曲線を算出
-            fpr = {}
-            tpr = {}
-            roc_auc = {}
-            for i in range(n_classes):
-                fpr[i], tpr[i], _ = roc_curve(y_test_binarize[:, i], y_score[:, i],
-                                              pos_label=pos_label,
-                                              sample_weight=sample_weight,
-                                              drop_intermediate=drop_intermediate)
-                roc_auc[i] = auc(fpr[i], tpr[i])
-            # micro-averageしたROC曲線を算出
-            fpr["micro"], tpr["micro"], _ = roc_curve(y_test_binarize.ravel(), y_score.ravel(),
-                                                      pos_label=pos_label,
-                                                      sample_weight=sample_weight,
-                                                      drop_intermediate=drop_intermediate)
-            roc_auc["micro"] = auc(fpr["micro"], tpr["micro"])
-            # macro-averageしたROC曲線を算出
-            all_fpr = np.unique(np.concatenate([fpr[i] for i in range(n_classes)]))  # FPRのユニーク値を抽出
-            mean_tpr = np.zeros_like(all_fpr)  # Then interpolate all ROC curves at this points
-            for i in range(n_classes):
-                mean_tpr += np.interp(all_fpr, fpr[i], tpr[i])
-            mean_tpr /= n_classes
-            fpr["macro"] = all_fpr
-            tpr["macro"] = mean_tpr
-            roc_auc["macro"] = auc(fpr["macro"], tpr["macro"])
-
-            # Micro、Macroを選択
-            fpr_avg = fpr[average]
-            tpr_avg = tpr[average]
-            roc_auc_avg = roc_auc[average]
-            fpr_avg_graph = np.concatenate([np.array([0]), fpr_avg])  # グラフ表示用に端点を追加
-            tpr_avg_graph = np.concatenate([np.array([0]), tpr_avg])  # グラフ表示用に端点を追加
-            
-            # class_average_kwsに渡す引数
-            if 'alpha' not in class_average_kws.keys():
-                class_average_kws['alpha'] = 0.8
-            if 'lw' not in class_average_kws.keys():
-                class_average_kws['lw'] = 2
-            if 'linestyle' not in class_average_kws.keys():
-                class_average_kws['linestyle'] = ':'
-            # 平均ROC曲線をプロット
-            ax.plot(fpr_avg_graph, tpr_avg_graph,
-                    label=f'{average}' + '-average ROC (area = {0:0.2f})'
-                        ''.format(roc_auc_avg),
-                    **class_average_kws)
-
-            # plot_roc_curveに渡す引数            
-            if 'alpha' not in plot_roc_kws.keys():
-                plot_roc_kws['alpha'] = 0.4
-            if 'lw' not in plot_roc_kws.keys():
-                plot_roc_kws['lw'] = 1
-            # クラスごとのROC曲線をプロット
-            color_list = list(colors.TABLEAU_COLORS.values())
-            for i, color in zip(range(n_classes), color_list):
-                ax.plot(fpr[i], tpr[i], color=color,
-                        label='ROC class {0} (area = {1:0.2f})'
-                        ''.format(y_labels[i], roc_auc[i]),
-                        **plot_roc_kws)
-            # 軸ラベルと凡例を追加
-            ax.set_xlabel('False Positive rate')
-            ax.set_ylabel('True Positive Rate')
-            ax.legend()
-
-            # FPR、TPR、ROC曲線を保持
-            name = estimator.__class__.__name__ if name is None else name
-            viz = RocCurveDisplay(
-                fpr=fpr_avg,
-                tpr=tpr_avg,
-                roc_auc=roc_auc_avg,
-                estimator_name=name,
-                pos_label=pos_label
-            )
-        
-        return viz
-
-    @classmethod
-    def roc_plot(cls, clf, x: List[str], y: str, data: pd.DataFrame = None,
-                 x_colnames: List[str] = None, 
-                 cv=None, cv_seed=42, cv_group=None,
-                 ax=None,
-                 sample_weight=None, drop_intermediate=True,
-                 response_method="predict_proba", pos_label=None, average='macro',
-                 clf_params=None, fit_params=None, eval_set_selection=None,
-                 draw_grid=True, grid_kws=None, subplot_kws=None, legend_kws=None,
-                 plot_roc_kws=None, class_average_kws=None, cv_mean_kws=None, chance_plot_kws=None):
-        """Plot Receiver operating characteristic (ROC) curve with cross validation.
-
-        Available both binary and multiclass classifiction.
-
-        Extra keyword arguments will be passed to matplotlib's ``plot``.
-
-        Parameters
-        ----------
-        clf: classifier object implementing ``fit``
-            Fitted classifier or a fitted :class:`~sklearn.pipeline.Pipeline`
-            in which the last estimator is a classifier.
-
-        x : list[str], or np.ndarray
-            Explanatory variables. Should be list[str] if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
-
-        y : str or np.ndarray
-            Objective variable. Should be str if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
-
-        data: pd.DataFrame, default=None
-            Input data structure.
-
-        x_colnames: list[str], default=None
-            Names of explanatory variables. Available only if ``data`` is NOT pd.DataFrame
-
-        cv: int or sklearn.model_selection.*, default=5
-            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
-
-        cv_seed: int, default=42
-            Seed for random number generator of cross validation.
-
-        cv_group: str, optional
-            Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
-
-        ax : {matplotlib.axes.Axes, list[matplotlib.axes.Axes]}, default=None
-            Pre-existing axes for the plot or list of it. Otherwise, call matplotlib.pyplot.subplot() internally.
-
-        sample_weight : array-like of shape (n_samples,), default=None
-            Sample weights.
-
-        drop_intermediate : boolean, default=True
-            Whether to drop some suboptimal thresholds which would not appear
-            on a plotted ROC curve. This is useful in order to create lighter
-            ROC curves.
-
-        response_method : {'predict_proba', 'decision_function'}, default='predict_proba'
-            Specifies whether to use for calcurating class probability.
-
-        pos_label : str or int, default=None
-            The class considered as the positive class when computing the roc auc
-            metrics. By default, `estimators.classes_[1]` is considered
-            as the positive class.
-
-        average : {'macro', 'micro'}, default='micro'
-            Specifies whether to use for calcurating average of tpr and fpr.
-
-        clf_params: dict, default=None
-            Parameters passed to the classifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
-
-        fit_params : dict, default=None
-            Parameters passed to the fit() method of the classifier, e.g. ``early_stopping_round`` and ``eval_set`` of XGBClassifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
-        
-        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
-
-            If "test", select test data from `X` and `y` using cv.split().
-
-            If "original", use raw `eval_set`.
-
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
-
-        draw_grid: bool, default=True
-            If True, grid lines are drawn.
-
-        grid_kws: dict, default=None
-            Additional parameters passed to matplotlib.pyplot.grid() that draws grid lines, e.g. ``color``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.grid.html
-
-        subplot_kws: dict, default=None
-            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize``. Avealable only if ``ax`` is None. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
-
-        legend_kws : dict
-            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
-
-        plot_roc_kws : dict, default=None
-            Additional parameters passed to matplotlib.pyplot.plot() that draws ROC curve of each classes, e.g. ``lw``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
-        
-        class_average_kws : dict, default=None
-            Additional parameters passed to matplotlib.pyplot.plot() or sklearn.metrics.plot_roc_curve() that draws average ROC curve of all classes, e.g. ``lw``. See https://scikit-learn.org/stable/modules/generated/sklearn.metrics.plot_roc_curve.html
-        
-        cv_mean_kws : dict, default=None
-            Additional parameters passed to matplotlib.pyplot.plot() that draws mean ROC curve of all folds of cross validation, e.g. ``lw``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
-        
-        chance_plot_kws : dict, default=None
-            Additional parameters passed to matplotlib.pyplot.plot() that draws chance line, e.g. ``lw``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
-        """
-        # 入力データの形式統一
-        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data(x, y, data,
-                                                                                        x_colnames,
-                                                                                        cv_group)
-
-        # 学習器パラメータがあれば適用
-        if clf_params is not None:
-            clf.set_params(**clf_params)
-        # 学習時パラメータがNoneなら空のdictを入力
-        if fit_params is None:
-            fit_params = {}
-        # grid_kwsがNoneなら空のdictを入力
-        if grid_kws is None:
-            grid_kws = {}
-        # subplot_kwsがNoneなら空のdictを入力
-        if subplot_kws is None:
-            subplot_kws = {}
-        # legend_kwsがNoneなら空のdictを入力
-        if legend_kws is None:
-            legend_kws = {}
-        # plot_roc_kwsがNoneなら空のdictを入力
-        if plot_roc_kws is None:
-            plot_roc_kws = {}
-        # class_average_kwsがNoneなら空のdictを入力
-        if class_average_kws is None:
-            class_average_kws = {}
-        # cv_mean_kwsがNoneなら空のdictを入力
-        if cv_mean_kws is None:
-            cv_mean_kws = {}
-        # chance_plot_kwsがNoneなら空のdictを入力
-        if chance_plot_kws is None:
-            chance_plot_kws = {}
-
-        # クロスバリデーション有無で場合分け
-        # クロスバリデーション未実施時(学習データから学習してプロット)
-        if cv is None:
-            # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
-            if ax is None:
-                ax=plt.gca()
-            # plot_roc_curveに渡す引数
-            name = 'ROC'
-            if 'alpha' not in plot_roc_kws.keys():
-                plot_roc_kws['alpha'] = 0.5
-            if 'lw' not in plot_roc_kws.keys():
-                plot_roc_kws['lw'] = 1
-            # ROC曲線をプロット
-            viz = cls.plot_roc_curve_multiclass(clf, X, y_true,
-                                                sample_weight=sample_weight, drop_intermediate=drop_intermediate,
-                                                response_method=response_method, name=name, ax=ax,
-                                                pos_label=pos_label, average=average,
-                                                fit_params = fit_params,
-                                                plot_roc_kws=plot_roc_kws,
-                                                class_average_kws=class_average_kws
-                                                )
-                                  
-        # クロスバリデーション実施時(分割ごとに別々にプロット＆指標算出)
-        if cv is not None:
-            # 分割法未指定時、cv_numとseedに基づきKFoldでランダムに分割
-            if isinstance(cv, numbers.Integral):
-                cv = KFold(n_splits=cv, shuffle=True, random_state=cv_seed)
-            # LeaveOneOutのときエラーを出す
-            if isinstance(cv, LeaveOneOut):
-                raise Exception('"regression_heat_plot" method does not support "LeaveOneOut" cross validation')
-            # cv_groupをグルーピング対象に指定(GroupKFold、LeaveOneGroupOut等)
-            split_kws={}
-            if cv_group_colname is not None:
-                split_kws['groups'] = data[cv_group_colname].values
-            elif isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
-                raise Exception('"GroupKFold" and "LeaveOneGroupOut" cross validations need ``cv_group`` argument')
-            # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
-            if isinstance(cv, LeaveOneGroupOut):
-                cv_num = len(set(data[cv_group_colname].values))
-            else:
-                cv_num = cv.n_splits
-
-            # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
-            if eval_set_selection is None:
-                eval_set_selection = 'test'
-            fit_params, eval_set_selection = init_eval_set(
-                    eval_set_selection, fit_params, X, y)
-            # 最終学習器以外の前処理変換器作成
-            transformer = _make_transformer(eval_set_selection, clf)
-
-            # 表示用のax作成
-            if ax is None:
-                if 'figsize' not in subplot_kws.keys():
-                    subplot_kws['figsize'] = (6, (cv_num + 1) * 6)
-                fig, ax = plt.subplots(cv_num + 1, 1, **subplot_kws)
-
-            # 平均ROC曲線算出用のリスト
-            tprs = []
-            aucs = []
-            mean_fpr = np.linspace(0, 1, 100)
-            color_list = list(colors.TABLEAU_COLORS.values())
-            # クロスバリデーション
-            for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
-                name = 'ROC fold {}'.format(i)
-                # plot_roc_curveに渡す引数            
-                if 'alpha' not in plot_roc_kws.keys():
-                    plot_roc_kws['alpha'] = 0.3
-                if 'lw' not in plot_roc_kws.keys():
-                    plot_roc_kws['lw'] = 1
-                # class_average_kwsに渡す引数
-                if 'alpha' not in class_average_kws.keys():
-                    class_average_kws['alpha'] = 0.6
-                if 'lw' not in class_average_kws.keys():
-                    class_average_kws['lw'] = 2
-                if 'linestyle' not in class_average_kws.keys():
-                    class_average_kws['linestyle'] = ':'
-                class_average_kws['color'] = color_list[i]
-
-                # eval_setの中から学習データ or テストデータのみを抽出
-                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
-                                                        fit_params, train, test)
-                
-                # CVごとのROC曲線をプロット
-                viz = cls.plot_roc_curve_multiclass(clf, X[train], y_true[train], 
-                                                    X_test=X[test], y_test=y_true[test],
-                                                    sample_weight=sample_weight, drop_intermediate=drop_intermediate,
-                                                    response_method=response_method,
-                                                    name=name, ax=ax[i],
-                                                    pos_label=pos_label, average=average, fit_params=fit_params_modified,
-                                                    plot_roc_kws=plot_roc_kws,
-                                                    class_average_kws=class_average_kws
-                                                    )
-                ax[i].set_title(f'Cross Validation Fold{i}')
-                # TPRとAUCを保持
-                interp_tpr = np.interp(mean_fpr, viz.fpr, viz.tpr)  # データが存在しない部分を補完
-                interp_tpr[0] = 0.0
-                tprs.append(interp_tpr)
-                aucs.append(viz.roc_auc)
-                # CVごとのROC曲線を全体図にプロット
-                ax[cv_num].plot(mean_fpr, interp_tpr,
-                                label=f'{name} (AUC = {aucs[i]:.2f})',
-                                color=color_list[i],
-                                **plot_roc_kws)
-            
-            # CV平均ROC曲線を計算
-            mean_tpr = np.mean(tprs, axis=0)
-            mean_tpr[-1] = 1.0
-            mean_auc = auc(mean_fpr, mean_tpr)
-            std_auc = np.std(aucs)
-            # CV平均ROC曲線plotに渡す引数
-            if 'label' not in cv_mean_kws.keys():
-                    cv_mean_kws['label'] = r'Mean ROC (AUC = %0.2f $\pm$ %0.2f)' % (mean_auc, std_auc)
-            if 'alpha' not in cv_mean_kws.keys():
-                cv_mean_kws['alpha'] = 0.8
-            if 'lw' not in cv_mean_kws.keys():
-                cv_mean_kws['lw'] = 2
-            if 'color' not in cv_mean_kws.keys():
-                cv_mean_kws['color'] = 'blue'
-            # 平均ROC曲線プロット
-            ax[cv_num].plot(mean_fpr, mean_tpr, **cv_mean_kws)
-            ax[cv_num].set_title('All Cross Validations')
-            # 軸ラベルを追加
-            ax[cv_num].set_xlabel('False Positive rate')
-            ax[cv_num].set_ylabel('True Positive Rate')
-
-        # ランダム時の直線描画に渡す引数
-        if 'label' not in chance_plot_kws.keys():
-                chance_plot_kws['label'] = 'Chance'
-        if 'alpha' not in chance_plot_kws.keys():
-            chance_plot_kws['alpha'] = 0.8
-        if 'lw' not in chance_plot_kws.keys():
-            chance_plot_kws['lw'] = 2
-        if 'color' not in chance_plot_kws.keys():
-            chance_plot_kws['color'] = 'red'
-        if 'linestyle' not in chance_plot_kws.keys():
-            chance_plot_kws['linestyle'] = '--'
-        # ランダム時の直線描画
-        for ax_cv in ax if cv is not None else [ax]:
-            ax_cv.plot([0, 1], [0, 1], **chance_plot_kws)
-            # 凡例追加
-            if 'loc' not in legend_kws.keys():
-                legend_kws['loc'] = 'lower right'
-            ax_cv.legend(**legend_kws)
-            ax_cv.set(xlim=[-0.05, 1.05], ylim=[-0.05, 1.05])
-
-        # グリッド線描画
-        if draw_grid:
-            if 'which' not in grid_kws.keys():
-                grid_kws['which'] = 'major'
-            if 'color' not in grid_kws.keys():
-                grid_kws['color'] = 'lightgrey'
-            if 'linestyle' not in grid_kws.keys():
-                grid_kws['linestyle'] = '-'
-            for ax_cv in ax if cv is not None else [ax]:
+from typing import List
+import matplotlib.pyplot as plt
+import numbers
+import numpy as np
+import pandas as pd
+from scipy import stats
+from sklearn.metrics import auc, roc_curve, RocCurveDisplay
+from sklearn.model_selection import KFold, LeaveOneOut, GroupKFold, LeaveOneGroupOut
+from sklearn.preprocessing import label_binarize
+from matplotlib import colors
+import copy
+import decimal
+
+from .multiclass_fitparams import OneVsRestClassifierPatched
+from ._cv_eval_set import init_eval_set, _make_transformer, _eval_set_selection
+
+class classplot():
+    # 散布図カラーリスト
+    _SCATTER_COLORS = ['green', 'red', 'mediumblue', 'brown', 'darkmagenta', 'darkorange', 'gold', 'grey']
+    # クラス確率図カラーマップ
+    _PROB_CMAP = ['Greens', 'Reds', 'Blues', 'YlOrBr', 'Purples', 'OrRd', 'Wistia', 'Greys']
+    # デフォルトでの決定境界図の透明度(alpha)
+    _DEFAULT_SEPARATOR_ALPHA = 0.3
+    # デフォルトでのクラス確率図等高線モードの透明度(alpha)
+    _DEFAULT_PROBA_CONTOURF_ALPHA = 0.5
+    # デフォルトでのクラス確率図透明度補正シグモイド関数のゲイン
+    _DEFAULT_PROBA_CONTOURF_SIG_GAIN = 0.5
+    # デフォルトでのクラス確率図の等高線段階数
+    _DEFAULT_PROBA_CONTOURF_LEVELS = 10
+    # デフォルトでのクラス確率図RGB画像モードの透明度(alpha)
+    _DEFAULT_PROBA_RGB_ALPHA = 0.45
+
+    def _round_digits(src: float, rounddigit: int = None, method='decimal'):
+        """
+        指定桁数で小数を丸める
+
+        Parameters
+        ----------
+        src : float
+            丸め対象の数値
+        rounddigit : int
+            フィッティング線の表示範囲（標準偏差の何倍まで表示するか指定）
+        method : int
+            桁数決定手法（'decimal':小数点以下, 'sig':有効数字(Decimal指定), 'format':formatで有効桁数指定）
+        """
+        if method == 'decimal':
+            return round(src, rounddigit)
+        elif method == 'sig':
+            with decimal.localcontext() as ctx:
+                ctx.prec = rounddigit
+                return ctx.create_decimal(src)
+        elif method == 'format':
+            return '{:.{width}g}'.format(src, width=rounddigit)
+    
+    def _reshape_input_data(x, y, data, x_colnames, cv_group):
+        """
+        入力データの形式統一(pd.DataFrame or np.ndarray)
+        """
+        # dataがpd.DataFrameのとき
+        if isinstance(data, pd.DataFrame):
+            if not isinstance(x, list):
+                raise Exception('`x` argument should be list[str] if `data` is pd.DataFrame')
+            if not isinstance(y, str):
+                raise Exception('`y` argument should be str if `data` is pd.DataFrame')
+            if x_colnames is not None:
+                raise Exception('`x_colnames` argument should be None if `data` is pd.DataFrame')
+            X = data[x].values
+            y_true = data[y].values
+            x_colnames = x
+            y_colname = y
+            cv_group_colname = cv_group
+            
+        # dataがNoneのとき(x, y, cv_groupがnp.ndarray)
+        elif data is None:
+            if not isinstance(x, np.ndarray):
+                raise Exception('`x` argument should be np.ndarray if `data` is None')
+            if not isinstance(y, np.ndarray):
+                raise Exception('`y` argument should be np.ndarray if `data` is None')
+            X = x if len(x.shape) == 2 else x.reshape([x.shape[0], 1])
+            y_true = y.ravel()
+            # x_colnameとXの整合性確認
+            if x_colnames is None:
+                x_colnames = list(range(X.shape[1]))
+            elif X.shape[1] != len(x_colnames):
+                raise Exception('width of X must be equal to length of x_colnames')
+            else:
+                x_colnames = x_colnames
+            y_colname = 'objective_variable'
+            if cv_group is not None:  # cv_group指定時
+                cv_group_colname = 'group'
+                data = pd.DataFrame(np.column_stack((X, y_true, cv_group)),
+                                    columns=x_colnames + [y_colname] + [cv_group_colname])
+            else:
+                cv_group_colname = None
+                data = pd.DataFrame(np.column_stack((X, y)),
+                                    columns=x_colnames + [y_colname])
+        else:
+            raise Exception('`data` argument should be pd.DataFrame or None')
+
+        return X, y_true, data, x_colnames, y_colname, cv_group_colname
+
+    @classmethod
+    def _chart_plot_2d(cls, trained_clf, x_chart, y_true_col, y_pred_col, data, x_chart_indices,
+                       x1_start, x1_end, x2_start, x2_end, other_x, chart_scale,
+                       proba_pred_col, proba_class_indices, ax, plot_border, plot_scatter,
+                       scatter_color_dict, scatter_marker_dict, proba_cmap_dict, proba_type,
+                       contourf_kws=None, imshow_kws=None, scatter_kws=None, legend_kws=None):
+        """
+        分類チャート（決定境界図 or クラス確率図）と各種散布図の表示
+        (class_separator_plotあるいはclass_prob_plotメソッドの描画処理部分)
+        """
+        # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
+        if ax is None:
+            ax=plt.gca()
+
+        # 図のサイズからグリッド数を取得
+        xnum, ynum = plt.gcf().dpi * plt.gcf().get_size_inches()
+        # チャート用グリッドデータを作成
+        xx = np.linspace(x1_start, x1_end, num=int(xnum/chart_scale))
+        yy = np.linspace(x2_start, x2_end, num=int(ynum/chart_scale))
+        X1, X2 = np.meshgrid(xx, yy)
+        X_grid = np.c_[X1.ravel(), X2.ravel()]
+        # 推論用に全説明変数を保持したndarrayを作成 (チャート非使用変数は固定値other_xとして追加)
+        n_rows = X_grid.shape[0]
+        X_all = []
+        other_add_flg = False
+        for i in range(2 + len(other_x)):
+            if i == x_chart_indices[0]: # チャート使用変数(1個目)を追加
+                X_all.append(X_grid[:, 0].reshape(n_rows, 1))
+            elif i == x_chart_indices[1]: # チャート使用変数(2個目)を追加
+                X_all.append(X_grid[:, 1].reshape(n_rows, 1))
+            elif len(other_x) >= 1 and not other_add_flg:  # チャート非使用変数(1個目)を固定値として追加
+                X_all.append(np.full((n_rows, 1), other_x[0]))
+                other_add_flg = True
+            elif len(other_x) == 2:  # チャート非使用変数(2個目)を固定値として追加
+                X_all.append(np.full((n_rows, 1), other_x[1]))
+        X_all = np.hstack(X_all)
+
+        # グリッドデータに対して推論し、推定値を作成
+        y_pred_grid = trained_clf.predict(X_all)
+        # 推定値をint型に変換
+        class_int_dict = dict(zip(scatter_color_dict.keys(), range(len(scatter_color_dict))))
+        y_pred_grid_int = np.vectorize(lambda x: class_int_dict[x])(y_pred_grid)
+        # グリッドデータをピボット化
+        y_pred_pivot = y_pred_grid_int.reshape(X1.shape)
+
+        # 決定境界図をプロット
+        if proba_pred_col is None:
+            # 決定境界色分けプロット
+            ax.contourf(X1, X2, y_pred_pivot,
+                        levels=np.arange(y_pred_pivot.max() + 2) - 0.5,
+                        **contourf_kws)
+
+        # クラス確率図をプロット
+        else:
+            # クラス数
+            nclass = len(proba_class_indices)
+            # グリッドデータに対してクラス確率算出
+            y_proba_grid = trained_clf.predict_proba(X_all)[:, proba_class_indices]
+
+            # contourfで等高線プロット（塗りつぶしあり）するとき
+            if proba_type == 'contourf':
+                # alpha値を保持(描画終了後に更新前に戻すため)
+                src_alpha = contourf_kws['alpha']
+                # シグモイド関数(クラス数1のときalphaで、クラス数∞のとき1に漸近)でalphaを補正
+                contourf_kws['alpha'] = 2*(1-src_alpha)/(1+np.exp(-cls._DEFAULT_PROBA_CONTOURF_SIG_GAIN*(nclass-1)))+2*src_alpha-1
+                # クラスごとに処理
+                for i in range(nclass):
+                    # グリッドデータから該当クラスのみ抜き出してピボット化
+                    y_proba_pivot = y_proba_grid[:, i].reshape(X1.shape)
+                    # カラーマップをproba_cmap_dictの値から取得
+                    cmap = list(proba_cmap_dict.values())[i]
+                    # クラス確率図プロット
+                    ax.contourf(X1, X2, y_proba_pivot,
+                                cmap=cmap,
+                                **contourf_kws)
+                    # alpha値を更新(alpha/(1+alpha))
+                    old_alpha = contourf_kws['alpha']
+                    contourf_kws['alpha'] = old_alpha / (1 + old_alpha)
+                # alpha値を更新前に戻す
+                contourf_kws['alpha'] = src_alpha
+            
+            # contourで等高線プロット（塗りつぶしなし）するとき
+            elif proba_type == 'contour':
+                # クラスごとに処理
+                for i in range(nclass):
+                    # グリッドデータから該当クラスのみ抜き出してピボット化
+                    y_proba_pivot = y_proba_grid[:, i].reshape(X1.shape)
+                    # 線の色をscatter_color_dictの値から取得
+                    cmap = list(proba_cmap_dict.values())[i]
+                    #c=list(scatter_color_dict.values())[proba_class_indices[i]]
+                    ax.contour(X1, X2, y_proba_pivot,
+                               cmap=cmap,
+                               **contourf_kws)
+            
+            # imshowでRGB画像プロットするとき
+            elif proba_type == 'imshow':
+                # いったんRGB各色ゼロで埋める
+                proba_g = np.zeros(X1.shape)  # 緑
+                proba_r = np.zeros(X1.shape)  # 赤
+                proba_b = np.zeros(X1.shape)  # 青
+                # RGBいずれかのカラーマップを持つクラスが存在すれば、そのクラスの確率を格納
+                for i, cmap in enumerate(proba_cmap_dict.values()):
+                    if cmap == 'Greens':
+                        proba_g = y_proba_grid[:, i].reshape(X1.shape)
+                    elif cmap == 'Reds':
+                        proba_r = y_proba_grid[:, i].reshape(X1.shape)
+                    elif cmap == 'Blues':
+                        proba_b = y_proba_grid[:, i].reshape(X1.shape)
+                    else:
+                        # imshowのとき、Greens, Reds, Blues以外のカラーマップを指定したらエラーを出す(4クラス以上は描画不可)
+                        raise Exception('only "Greens, Reds, Blues" cmap are allowd if the "proba_type" argument is "imshow"')
+                # RGBのデータを合体して上下反転
+                im_grid = np.flip(np.stack([proba_r, proba_g, proba_b], 2), axis=0)
+                # RGB画像をプロット
+                ax.imshow(im_grid,
+                          aspect="auto", extent=(x1_start, x1_end, x2_start, x2_end),
+                          **imshow_kws)
+            else:
+                raise Exception('the "proba_type" argument must be "contourf", "contour" or "imshow"')
+
+        # 境界線をプロット
+        if plot_border:
+            ax.contour(X1, X2, y_pred_pivot,
+                       levels=np.arange(y_pred_pivot.max() + 2) - 0.5,
+                       colors='k',
+                       linewidths=0.5,
+                       antialiased=True)
+
+        # 散布図をプロット
+        if plot_scatter is not None:
+            # マーカの縁の色未指定のとき、dimgreyを指定
+            if 'edgecolors' not in scatter_kws.keys():
+                scatter_kws['edgecolors'] = 'dimgrey'
+            # 正誤を判定
+            data['error'] = (data[y_true_col] == data[y_pred_col])
+            # 色分け
+            if plot_scatter == 'error':  # 正誤で色分け
+                cdict = {True:'blue', False:'red'}
+                for name, group in data.groupby('error'):
+                    ax.scatter(group[x_chart[0]].values, group[x_chart[1]].values,
+                               label=name, c=cdict[name],
+                               marker=scatter_marker_dict[name],
+                               **scatter_kws)
+            elif plot_scatter == 'class':  # クラスで色分け
+                for name, group in data.groupby(y_true_col):
+                    ax.scatter(group[x_chart[0]].values, group[x_chart[1]].values,
+                               label=name, c=scatter_color_dict[name],
+                               **scatter_kws)
+            elif plot_scatter == 'class_error':  # クラスと正誤で色分け
+                for name, group in data.groupby([y_true_col, 'error']):
+                    ax.scatter(group[x_chart[0]].values, group[x_chart[1]].values,
+                               label=f'{name[0]}   {name[1]}', c=scatter_color_dict[name[0]],
+                               marker=scatter_marker_dict[name[1]],
+                               **scatter_kws)
+            # 凡例表示
+            ax.legend(**legend_kws)
+
+        # 軸ラベルを追加
+        ax.set_xlabel(x_chart[0])
+        ax.set_ylabel(x_chart[1])
+
+    @classmethod
+    def _class_chart_plot(cls, trained_clf, X, y_pred, y_true, x_chart, x_not_chart, x_chart_indices,
+                       pair_sigmarange=2.0, pair_sigmainterval=0.5, chart_extendsigma=0.5, chart_scale=1,
+                       proba_pred = None, proba_class_indices = None, plot_border=True, plot_scatter='class', 
+                       scatter_color_dict=None, scatter_marker_dict=None, proba_cmap_dict=None, proba_type=None,
+                       rounddigit_x3=None, cv_index=None,
+                       subplot_kws=None, contourf_kws=None, imshow_kws=None, scatter_kws=None, legend_kws=None):
+        """
+        分類チャート（決定境界図 or クラス確率図）表示の、説明変数の数に応じた分岐処理
+        (class_separator_plotあるいはclass_prob_plotメソッド処理のうち、説明変数の数に応じたデータ分割等を行う)
+        """
+        # 説明変数の数
+        x_num = X.shape[1]
+        # チャート（決定境界図 or クラス確率図）使用DataFrame
+        df_chart = pd.DataFrame(X[:, x_chart_indices], columns=x_chart)
+        # チャート非使用DataFrame
+        X_not_chart = X[:, [i for i in range(X.shape[1]) if i not in x_chart_indices]]
+        df_not_chart = pd.DataFrame(X_not_chart, columns=x_not_chart)
+        # 結合＆目的変数実測値と予測値追加
+        df_all = df_chart.join(df_not_chart)
+        df_all = df_all.join(pd.DataFrame(y_true, columns=['y_true']))
+        df_all = df_all.join(pd.DataFrame(y_pred, columns=['y_pred']))
+        # クラス確率追加（クラス確率図プロット時のみ）
+        if proba_pred is not None:
+            proba_pred_col = list(proba_cmap_dict.keys())
+            df_all = df_all.join(pd.DataFrame(proba_pred, columns=[proba_pred_col]))
+        else:
+            proba_pred_col = None
+        # チャート非使用変数を標準化してDataFrameに追加
+        if x_num >= 3:
+            X_not_chart_norm = stats.zscore(df_not_chart)
+            if isinstance(X_not_chart_norm, pd.DataFrame):  # X_not_chart_normがDataFrameの時
+                not_chart_rename_dir = {c: f'normalize_{c}' for c in df_not_chart}
+                df_all = df_all.join(X_not_chart_norm.rename(columns=not_chart_rename_dir))
+            else:  # X_not_chart_normがndarrayの時（古いscipyのバージョン時）
+                df_all = df_all.join(pd.DataFrame(X_not_chart_norm, columns=[f'normalize_{c}' for c in df_not_chart]))
+
+        # チャートのX1軸およびX2軸の表示範囲(最大最小値 + extendsigma)
+        x1_min = np.min(X[:, x_chart_indices[0]])
+        x1_max = np.max(X[:, x_chart_indices[0]])
+        x1_std = np.std(X[:, x_chart_indices[0]])
+        x1_start = x1_min - x1_std * chart_extendsigma
+        x1_end = x1_max + x1_std * chart_extendsigma
+        x2_min = np.min(X[:, x_chart_indices[1]])
+        x2_max = np.max(X[:, x_chart_indices[1]])
+        x2_std = np.std(X[:, x_chart_indices[1]])
+        x2_start = x2_min - x2_std * chart_extendsigma
+        x2_end = x2_max + x2_std * chart_extendsigma
+
+        # プロットする図の数(sigmarange外「2枚」 + sigmarange内「int(pair_sigmarange / pair_sigmainterval) * 2枚」)
+        pair_n = int(pair_sigmarange / pair_sigmainterval) * 2 + 2
+        # チャート非使用変数をプロットする範囲の下限(標準化後)
+        pair_min = -(pair_n - 2) / 2 * pair_sigmainterval
+
+        # 説明変数が2次元のとき (図は1枚のみ)
+        if x_num == 2:
+            pair_w = 1
+            pair_h = 1
+        # 説明変数が3次元のとき (図はpair_n × 1枚)
+        elif x_num == 3:
+            pair_w = 1
+            pair_h = pair_n
+        # 説明変数が4次元のとき (図はpair_n × pair_n枚)
+        elif x_num == 4:
+            pair_w = pair_n
+            pair_h = pair_n
+
+        # figsize (全ての図全体のサイズ)指定
+        if 'figsize' not in subplot_kws.keys():
+            subplot_kws['figsize'] = (pair_w * 6, pair_h * 5)
+        # プロット用のaxes作成
+        fig, axes = plt.subplots(pair_h, pair_w, **subplot_kws)
+        if cv_index is not None:
+            fig.suptitle(f'CV {cv_index}')
+
+        # 図ごとにプロット
+        for i in range(pair_h):
+            for j in range(pair_w):
+                # pair縦軸変数(標準化後)の最小値
+                if i == 0:
+                    h_min = -float('inf')
+                    h_mean = pair_min - pair_sigmainterval / 2  # チャート非使用変数指定用の平均値
+                else:
+                    h_min = pair_min + (i - 1) * pair_sigmainterval
+                    h_mean = pair_min + (i - 0.5) * pair_sigmainterval  # チャート非使用変数指定用の平均値
+                # pair縦軸変数(標準化後)の最大値
+                if i == pair_h - 1:
+                    h_max = float('inf')
+                else:
+                    h_max = pair_min + i * pair_sigmainterval
+                # pair横軸変数(標準化後)の最小値
+                if j == 0:
+                    w_min = -float('inf')
+                    w_mean = pair_min - pair_sigmainterval / 2  # チャート非使用変数指定用の平均値
+                else:
+                    w_min = pair_min + (j - 1) * pair_sigmainterval
+                    w_mean = pair_min + (j - 0.5) * pair_sigmainterval  # チャート非使用変数指定用の平均値
+                # pair横軸変数(標準化後)の最大値
+                if j == pair_w - 1:
+                    w_max = float('inf')
+                else:
+                    w_max = pair_min + j * pair_sigmainterval
+
+                # 説明変数が2次元のとき (図は1枚のみ)
+                if x_num == 2:
+                    ax = axes
+                    df_pair = df_all.copy()
+                    other_x = []
+                # 説明変数が3次元のとき (図はpair_n × 1枚)
+                elif x_num == 3:
+                    ax = axes[i]
+                    # 縦軸変数範囲内のみのデータを抽出
+                    df_pair = df_all[(df_all[f'normalize_{x_not_chart[0]}'] >= h_min) & (df_all[f'normalize_{x_not_chart[0]}'] < h_max)].copy()
+                    # 決定境界図非使用変数の標準化逆変換
+                    x3_mean = np.mean(X_not_chart[:, 0])
+                    x3_std = np.std(X_not_chart[:, 0])
+                    other_x = [h_mean * x3_std + x3_mean]
+                # 説明変数が4次元のとき (図はpair_n × pair_n枚)
+                elif x_num == 4:
+                    ax = axes[j, i]
+                    # 縦軸変数範囲内のみのデータを抽出
+                    df_pair = df_all[(df_all[f'normalize_{x_not_chart[0]}'] >= h_min) & (df_all[f'normalize_{x_not_chart[0]}'] < h_max)].copy()
+                    # 横軸変数範囲内のみのデータを抽出
+                    df_pair = df_pair[(df_pair[f'normalize_{x_not_chart[1]}'] >= w_min) & (df_pair[f'normalize_{x_not_chart[1]}'] < w_max)]
+                    # チャート非使用変数の標準化逆変換
+                    x3_mean = np.mean(X_not_chart[:, 0])
+                    x3_std = np.std(X_not_chart[:, 0])
+                    x4_mean = np.mean(X_not_chart[:, 1])
+                    x4_std = np.std(X_not_chart[:, 1])
+                    other_x = [h_mean * x3_std + x3_mean, w_mean * x4_std + x4_mean]
+                
+                cls._chart_plot_2d(trained_clf, x_chart, 'y_true', 'y_pred', df_pair, x_chart_indices,
+                                      x1_start, x1_end, x2_start, x2_end, other_x, chart_scale,
+                                      proba_pred_col, proba_class_indices, ax, plot_border, plot_scatter,
+                                      scatter_color_dict, scatter_marker_dict, proba_cmap_dict,  proba_type,
+                                      contourf_kws=contourf_kws, imshow_kws=imshow_kws, scatter_kws=scatter_kws,
+                                      legend_kws=legend_kws)
+
+                # グラフタイトルとして、チャート非使用変数の範囲を記載（説明変数が3次元以上のとき）
+                if x_num == 3:
+                    if i == 0:
+                        ax.set_title(f'{x_not_chart[0]}=- {cls._round_digits(h_max * x3_std + x3_mean, rounddigit=rounddigit_x3)} (- {h_max}σ)')
+                    elif i == pair_h - 1:
+                        ax.set_title(f'{x_not_chart[0]}={cls._round_digits(h_min * x3_std + x3_mean, rounddigit=rounddigit_x3)} - ({h_min}σ -)')
+                    else:
+                        ax.set_title(f'{x_not_chart[0]}={cls._round_digits(h_min * x3_std + x3_mean, rounddigit=rounddigit_x3)} - {cls._round_digits(h_max * x3_std + x3_mean, rounddigit=rounddigit_x3)} ({h_min}σ - {h_max}σ)')
+                if x_num == 4:
+                    ax.set_title(f'{x_not_chart[0]}= {h_min}σ - {h_max}σ  {x_not_chart[1]}= {w_min}σ - {w_max}σ')
+
+        # 字が重なるのでtight_layoutにする
+        plt.tight_layout()
+
+    @classmethod
+    def class_separator_plot(cls, clf, x: List[str], y: str, data: pd.DataFrame = None,
+                             x_colnames: List[str] = None, x_chart: List[str] = None,
+                             pair_sigmarange = 1.0, pair_sigmainterval = 0.5, chart_extendsigma = 0.5, chart_scale = 1,
+                             plot_scatter = 'class_error', rounddigit_x3 = 2,
+                             scatter_colors = None, true_marker = 'o', false_marker = 'x',
+                             cv=None, cv_seed=42, cv_group=None, display_cv_indices = 0,
+                             clf_params=None, fit_params=None, eval_set_selection=None,
+                             subplot_kws=None, contourf_kws=None, scatter_kws=None, legend_kws=None):
+        """
+        Plot class separation lines of any scikit-learn classifier with 2 to 4D explanatory variables.
+
+        Parameters
+        ----------
+        clf: classifier object implementing ``fit``
+            Classifier. This is assumed to implement the scikit-learn estimator interface.
+
+        x : list[str], or np.ndarray
+            Explanatory variables. Should be list[str] if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
+
+        y : str or np.ndarray
+            Objective variable. Should be str if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
+
+        data: pd.DataFrame
+            Input data structure.
+
+        x_colnames: list[str], optional
+            Names of explanatory variables. Available only if ``data`` is NOT pd.DataFrame
+
+        x_chart: list[str], optional
+            X-axis . If None, use two variables in ``x`` from the front.
+
+        pair_sigmarange: float, optional
+            Set the range of subplots. The lower limit is mean({x3, x4}) - ``pair_sigmarange`` * std({x3, x4}). The higher limit is mean({x3, x4}) + ``pair_sigmarange`` * std({x3, x4}). Available only if len(x) is bigger than 2.
+
+        pair_sigmainterval: float, optional
+            Set the interval of subplots. For example, if ``pair_sigmainterval`` is set to 0.5 and ``pair_sigmarange`` is set to 1.0, The ranges of subplots are lower than μ-1σ, μ-1σ to μ-0.5σ, μ-0.5σ to μ, μ to μ+0.5σ, μ+0.5σ to μ+1σ, and higher than μ+1σ. Available only if len(x) is bigger than 2.
+
+        chart_extendsigma: float, optional
+            Set the axis view limits of the separation map. The lower limit is min({x1, x2}) - std({x1, x2}) * chart_extendsigma. The higher limit is max({x1, x2}) + std({x1, x2}) * chart_extendsigma
+
+        chart_scale: int, optional
+            Set the resolution of the separation lines. If plotting speed is slow, we reccomend setting chart_scale to 2. We DON'T reccomend setting it to larger than 3 because of jaggies.
+
+        plot_scatter: {'error', 'class', 'class_error', None}, optional
+            Color decision of scatter plot. If 'error', to be mapped to colors using true-false. If 'class', to be mapped to colors using class labels. If 'class_error', to be mapped to colors using class labels and marker styles using true-false. If None, no scatter.
+
+        rounddigit_x3: int, optional
+            Round a number of y-axis valiable of subplots to a given precision in decimal digits.
+
+        scatter_colors: list[str], optional
+            Set of colors for mapping the class labels. Available only if ``plot_scatter`` is set to 'class' or 'class_error'.
+
+        true_marker: str, optional
+            Marker style of True label. Available only if ``plot_scatter`` is set to 'error' or 'class_error'. See https://matplotlib.org/stable/api/markers_api.html#module-matplotlib.markers
+
+        false_marker: str, optional
+            Marker style of False label. Available only if ``plot_scatter`` is set to 'error' or 'class_error'. See https://matplotlib.org/stable/api/markers_api.html#module-matplotlib.markers
+
+        cv : int, cross-validation generator, or an iterable, optional
+            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
+
+        cv_seed: int, optional
+            Seed for random number generator of cross validation.
+
+        cv_group: str, optional
+            Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
+
+        display_cv_indices: int, optional
+            Cross validation index or indices to display.
+
+        clf_params: dict, optional
+            Parameters passed to the classifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
+
+        fit_params: dict, optional
+            Parameters passed to the fit() method of the classifier, e.g. ``early_stopping_round`` and ``eval_set`` of XGBClassifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
+        
+        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
+            
+            If "all", use all data in `X` and `y`.
+
+            If "train", select train data from `X` and `y` using cv.split().
+
+            If "test", select test data from `X` and `y` using cv.split().
+
+            If "original", use raw `eval_set`.
+
+            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+
+        subplot_kws: dict, optional
+            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize.`` See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
+
+        contourf_kws: dict, optional
+            Additional parameters passed to matplotlib.pyplot.contourf(), e.g. ``alpha``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.contourf.html
+
+        scatter_kws: dict, optional
+            Additional parameters passed to matplotlib.pyplot.scatter(), e.g. ``alpha``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.scatter.html
+
+        legend_kws : dict
+            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
+        """
+
+        # 入力データの形式統一
+        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data(x, y, data,
+                                                                                           x_colnames,
+                                                                                           cv_group)
+        # 説明変数xの次元が2～4以外ならエラーを出す
+        if len(x_colnames) < 2 or len(x_colnames) > 4:
+            raise Exception('Dimension of x must be 2 to 4')
+        
+        # display_cv_indicesをList化
+        if isinstance(display_cv_indices, int):
+            display_cv_indices = [display_cv_indices]
+        elif not isinstance(x_colnames, list):
+            raise Exception('the "cv_display_num" argument must be int or List[int]')
+        # 学習器パラメータがあれば適用
+        if clf_params is not None:
+            clf.set_params(**clf_params)
+        # 学習時パラメータがNoneなら空のdictを入力
+        if fit_params is None:
+            fit_params = {}
+        # subplot_kwsがNoneなら空のdictを入力
+        if subplot_kws is None:
+            subplot_kws = {}
+        # contourf_kwsがNoneなら空のdictを入力
+        if contourf_kws is None:
+            contourf_kws = {}
+        # scatter_kwsがNoneなら空のdictを入力
+        if scatter_kws is None:
+            scatter_kws = {}
+        # legend_kwsがNoneなら空のdictを入力
+        if legend_kws is None:
+            legend_kws = {}
+        
+        # 決定境界図表示用の列を抽出
+        if x_chart is None:  # 列名指定していないとき、前から2列を抽出
+            x_chart = x_colnames[:2]
+            x_chart_indices = [0, 1]
+        else:  # 列名指定しているとき、該当列のXにおけるインデックス(0～3)を保持
+            if len(x_chart) != 2:
+                raise Exception('length of x_chart must be 2')
+            x_chart_indices = []
+            for colname in x_chart:
+                x_chart_indices.append(x_colnames.index(colname))
+        # 決定境界図表示以外の列
+        x_not_chart = [colname for colname in x_colnames if colname not in x_chart]
+
+        # クラス名と散布図色を紐づけ(色分けを全ての図で統一用)
+        if scatter_colors is None:
+            scatter_colors = cls._SCATTER_COLORS
+        class_list = data[y_colname].values.tolist()
+        class_list = sorted(set(class_list), key=class_list.index)
+        scatter_color_dict = dict(zip(class_list, scatter_colors[0:len(class_list)]))
+        # 散布図マーカー形状をdict化
+        scatter_marker_dict = {True: true_marker, False: false_marker}
+        # contourf_kwsにcolors指定ないとき、scatter_color_dictの値を使用
+        if 'colors' not in contourf_kws.keys():
+            contourf_kws['colors'] = list(scatter_color_dict.values())
+        # contourf_kwsにalphat指定ないとき、DEFAULT_SEPARATOR_ALPHAを使用
+        if 'alpha' not in contourf_kws.keys():
+            contourf_kws['alpha'] = cls._DEFAULT_SEPARATOR_ALPHA
+        
+        # クロスバリデーション有無で場合分け
+        # クロスバリデーション未実施時(学習データから学習してプロット)
+        if cv is None:
+            # 学習と推論
+            clf.fit(X, y_true, **fit_params)
+            y_pred = clf.predict(X)
+            # 決定境界図をプロット
+            cls._class_chart_plot(clf, X, y_pred, y_true, x_chart, x_not_chart, x_chart_indices,
+                               pair_sigmarange = pair_sigmarange, pair_sigmainterval=pair_sigmainterval, chart_extendsigma=chart_extendsigma, chart_scale=chart_scale,
+                               proba_pred = None, proba_class_indices = None, plot_border = True, plot_scatter = plot_scatter,
+                               scatter_color_dict=scatter_color_dict, scatter_marker_dict=scatter_marker_dict, proba_cmap_dict=None, proba_type=None,
+                               rounddigit_x3=rounddigit_x3, cv_index=None,
+                               subplot_kws=subplot_kws, contourf_kws=contourf_kws, imshow_kws=None, scatter_kws=scatter_kws, legend_kws=legend_kws)
+            
+        # クロスバリデーション実施時(分割ごとに別々にプロット＆指標算出)
+        if cv is not None:
+            # 分割法未指定時、cv_numとseedに基づきKFoldでランダムに分割
+            if isinstance(cv, numbers.Integral):
+                cv = KFold(n_splits=cv, shuffle=True, random_state=cv_seed)
+            # LeaveOneOutのときエラーを出す
+            if isinstance(cv, LeaveOneOut):
+                raise Exception('"regression_heat_plot" method does not support ``LeaveOneOut`` cross validation')
+            # cv_groupをグルーピング対象に指定(GroupKFold、LeaveOneGroupOut等)
+            split_kws={}
+            if cv_group_colname is not None:
+                split_kws['groups'] = data[cv_group_colname].values
+            elif isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
+                raise Exception('"GroupKFold" and "LeaveOneGroupOut" cross validations need ``cv_group`` argument')
+            # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
+            if isinstance(cv, LeaveOneGroupOut):
+                cv_num = len(set(data[cv_group_colname].values))
+            else:
+                cv_num = cv.n_splits
+
+            # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
+            if eval_set_selection is None:
+                eval_set_selection = 'test'
+            fit_params, eval_set_selection = init_eval_set(
+                    eval_set_selection, fit_params, X, y)
+            # 最終学習器以外の前処理変換器作成
+            transformer = _make_transformer(eval_set_selection, clf)
+
+            # クロスバリデーション
+            for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
+                # 表示対象以外のCVなら飛ばす
+                if i not in display_cv_indices:
+                    continue
+                print(f'cv_number={i}/{cv_num}')
+                # グラフタイトル(CV番号を指定。グルーピング系CVのときはグループ名を指定)
+                if isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
+                    cv_index = f'No.{i}  {cv_group_colname}={data[cv_group_colname].values[test][0]}'
+                else:
+                    cv_index = f'No.{i}'
+                # 表示用にテストデータと学習データ分割
+                X_train = X[train]
+                y_train = y_true[train]
+                X_test = X[test]
+                y_test = y_true[test]
+
+                # eval_setの中から学習データ or テストデータのみを抽出
+                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
+                                                        fit_params, train, test)
+
+                # 学習と推論
+                clf.fit(X_train, y_train, **fit_params_modified)
+                y_pred = clf.predict(X_test)
+                # 決定境界図をプロット
+                cls._class_chart_plot(clf, X_test, y_pred, y_test, x_chart, x_not_chart, x_chart_indices,
+                                   pair_sigmarange = pair_sigmarange, pair_sigmainterval = pair_sigmainterval, chart_extendsigma=chart_extendsigma, chart_scale=chart_scale,
+                                   proba_pred = None, proba_class_indices = None, plot_border = True, plot_scatter = plot_scatter,
+                                   scatter_color_dict=scatter_color_dict, scatter_marker_dict=scatter_marker_dict, proba_cmap_dict=None, proba_type=None,
+                                   rounddigit_x3=rounddigit_x3, cv_index=cv_index,
+                                   subplot_kws=subplot_kws, contourf_kws=contourf_kws, imshow_kws=None, scatter_kws=scatter_kws, legend_kws=legend_kws)
+
+    @classmethod
+    def class_proba_plot(cls, clf, x: List[str], y: str, data: pd.DataFrame = None,
+                         x_colnames: List[str] = None, x_chart: List[str] = None,
+                         pair_sigmarange = 1.0, pair_sigmainterval = 0.5, chart_extendsigma = 0.5, chart_scale = 1,
+                         plot_border = True, plot_scatter = 'class', rounddigit_x3 = 2,
+                         proba_class = None, proba_cmap_dict = None, proba_type = 'contourf',
+                         scatter_colors = None, true_marker = 'o', false_marker = 'x',
+                         cv=None, cv_seed=42, cv_group=None, display_cv_indices = 0,
+                         clf_params=None, fit_params=None, eval_set_selection=None,
+                         subplot_kws=None, contourf_kws=None, imshow_kws=None, scatter_kws=None, legend_kws=None):
+        """
+        Plot class prediction probability of any scikit-learn classifier with 2 to 4D explanatory variables.
+
+        Parameters
+        ----------
+        clf: classifier object implementing ``fit``
+            Classifier. This is assumed to implement the scikit-learn estimator interface.
+
+        x : list[str], or np.ndarray
+            Explanatory variables. Should be list[str] if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
+
+        y : str or np.ndarray
+            Objective variable. Should be str if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
+
+        data: pd.DataFrame, optional
+            Input data structure.
+
+        x_colnames: list[str], optional
+            Names of explanatory variables. Available only if ``data`` is NOT pd.DataFrame
+
+        x_chart: list[str], optional
+            X-axis and y-axis variables of separation map. If None, use two variables in ``x`` from the front.
+
+        pair_sigmarange: float, optional
+            Set the range of subplots. The lower limit is mean({x3, x4}) - ``pair_sigmarange`` * std({x3, x4}). The higher limit is mean({x3, x4}) + ``pair_sigmarange`` * std({x3, x4}). Available only if len(x) is bigger than 2.
+
+        pair_sigmainterval: float, optional
+            Set the interval of subplots. For example, if ``pair_sigmainterval`` is set to 0.5 and ``pair_sigmarange`` is set to 1.0, The ranges of subplots are lower than μ-1σ, μ-1σ to μ-0.5σ, μ-0.5σ to μ, μ to μ+0.5σ, μ+0.5σ to μ+1σ, and higher than μ+1σ. Available only if len(x) is bigger than 2.
+
+        chart_extendsigma: float, optional
+            Set the axis view limits of the separation map. The lower limit is min({x1, x2}) - std({x1, x2}) * ``chart_extendsigma``. The higher limit is max({x1, x2}) + std({x1, x2}) * ``chart_extendsigma``
+
+        chart_scale: int, optional
+            Set the resolution of the separation lines. If plotting speed is slow, we reccomend setting chart_scale to 2. We DON'T reccomend setting it to larger than 3 because of jaggies.
+
+        plot_border: bool, optional
+            If True, display class separation lines
+
+        plot_scatter: {'error', 'class', 'class_error', None}, optional
+            Color decision of scatter plot. If 'error', to be mapped to colors using true-false. If 'class', to be mapped to colors using class labels. If 'class_error', to be mapped to colors using class labels and marker styles using true-false. If None, no scatter.
+
+        rounddigit_x3: int, optional
+            Round a number of y-axis valiable of subplots to a given precision in decimal digits.
+
+        proba_class: str or list[str], optional
+            Class label name, in which probability map is displayed.
+
+        proba_cmap_dict: dict[str, str], optional
+            Colormap of probability map. The keys must be class label name and the values must be colormap names in Matplotlib. See https://matplotlib.org/stable/tutorials/colors/colormaps.html
+
+        proba_type: {'contourf', 'contour', 'imshow'}, optional
+            Plotting type of probabiliity map. If 'contourf', mapped by matplotlib.pyplot.contourf(). If 'contour', mapped by matplotlib.pyplot.contour(). If 'imshow', mapped by matplotlib.pyplot.imshow(). 'imshow' is available only if the number of class labels is less than 4.
+
+        scatter_colors: list[str], optional
+            Set of colors for mapping the class labels. Available only if ``plot_scatter`` is set to 'class' or 'class_error'.
+
+        true_marker: str, optional
+            Marker style of True label. Available only if ``plot_scatter`` is set to 'error' or 'class_error'. See https://matplotlib.org/stable/api/markers_api.html#module-matplotlib.markers
+
+        false_marker: str, optional
+            Marker style of False label. Available only if ``plot_scatter`` is set to 'error' or 'class_error'. See https://matplotlib.org/stable/api/markers_api.html#module-matplotlib.markers
+
+        cv: int or sklearn.model_selection.*, optional
+            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
+
+        cv_seed: int, optional
+            Seed for random number generator of cross validation.
+
+        cv_group: str, optional
+            Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
+
+        display_cv_indices: int, optional
+            Cross validation index or indices to display.
+
+        clf_params: dict, optional
+            Parameters passed to the classifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
+
+        fit_params: dict, optional
+            Parameters passed to the fit() method of the classifier, e.g. ``early_stopping_round`` and ``eval_set`` of XGBClassifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
+
+        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
+            
+            If "all", use all data in `X` and `y`.
+
+            If "train", select train data from `X` and `y` using cv.split().
+
+            If "test", select test data from `X` and `y` using cv.split().
+
+            If "original", use raw `eval_set`.
+
+            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+
+        subplot_kws: dict, optional
+            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
+
+        contourf_kws: dict, optional
+            Additional parameters passed to matplotlib.pyplot.contourf() if proba_type is set to 'contourf', or additional parameters passed to matplotlib.pyplot.contour() if proba_type is set to 'contour'. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.contourf.html or https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.contour.html
+
+        imshow_kws: dict, optional
+            Additional parameters passed to matplotlib.pyplot.imshow(), e.g. ``alpha``. Available only if proba_type is set to 'imshow'. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.imshow.html
+
+        scatter_kws: dict, optional
+            Additional parameters passed to matplotlib.pyplot.scatter(), e.g. ``alpha``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.scatter.html
+
+        legend_kws : dict
+            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
+        """
+
+        # 入力データの形式統一
+        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data(x, y, data,
+                                                                                           x_colnames,
+                                                                                           cv_group)
+        # 説明変数xの次元が2～4以外ならエラーを出す
+        if len(x_colnames) < 2 or len(x_colnames) > 4:
+            raise Exception('Dimension of x must be 2 to 4')
+        
+        # display_cv_indicesをList化
+        if isinstance(display_cv_indices, int):
+            display_cv_indices = [display_cv_indices]
+        elif not isinstance(x_colnames, list):
+            raise Exception('the "cv_display_num" argument must be int or List[int]')
+        # 学習器パラメータがあれば適用
+        if clf_params is not None:
+            clf.set_params(**clf_params)
+        # 学習時パラメータがNoneなら空のdictを入力
+        if fit_params is None:
+            fit_params = {}
+        # subplot_kwsがNoneなら空のdictを入力
+        if subplot_kws is None:
+            subplot_kws = {}
+        # contourf_kwsがNoneなら空のdictを入力
+        if contourf_kws is None:
+            contourf_kws = {}
+        # imshow_kwsがNoneなら空のdictを入力
+        if imshow_kws is None:
+            imshow_kws = {}
+        # scatter_kwsがNoneなら空のdictを入力
+        if scatter_kws is None:
+            scatter_kws = {}
+        # legend_kwsがNoneなら空のdictを入力
+        if legend_kws is None:
+            legend_kws = {}
+
+        # クラス確率図表示用の列を抽出
+        if x_chart is None:  # 列名指定していないとき、前から2列を抽出
+            x_chart = x_colnames[:2]
+            x_chart_indices = [0, 1]
+        else:  # 列名指定しているとき、該当列のXにおけるインデックス(0～3)を保持
+            if len(x_chart) != 2:
+                raise Exception('length of x_chart must be 2')
+            x_chart_indices = []
+            for colname in x_chart:
+                x_chart_indices.append(x_colnames.index(colname))
+        # クラス確率図表示以外の列
+        x_not_chart = [colname for colname in x_colnames if colname not in x_chart]
+
+        # scatter_colors未指定のとき、デフォルト値を使用
+        if scatter_colors is None:
+            scatter_colors = cls._SCATTER_COLORS
+        # クラス名と散布図色を紐づけ(色分けを全ての図で統一用)
+        class_list = data[y_colname].values.tolist()
+        class_list = sorted(set(class_list), key=class_list.index)
+        scatter_color_dict = dict(zip(class_list, scatter_colors[0:len(class_list)]))
+        # 散布図マーカー形状をdict化
+        scatter_marker_dict = {True: true_marker, False: false_marker}
+
+        # proba_class未指定のとき、全てのクラスを使用
+        if proba_class is None:
+            proba_class = [c for c in class_list]
+        # proba_classをList化
+        if isinstance(proba_class, int) or isinstance(proba_class, str) or isinstance(proba_class, bool):
+            proba_class = [proba_class]
+        elif not isinstance(x_colnames, list):
+            raise Exception('the "proba_class" argument must be int, str, bool or List')
+        # List化したproba_classを走査してデータ上でのインデックスを取得
+        proba_class_indices = []
+        for pc in proba_class:
+            if pc not in class_list:  # 指定したproba_classがデータ上に存在しないとき、エラーを出す
+                raise Exception(f'"{proba_class}"" is not in the "{y_colname}" column')
+            proba_class_indices.append(class_list.index(pc))
+        # proba_cmap_dict未指定のとき、デフォルト値を使用
+        if proba_cmap_dict is None:
+            proba_cmap_dict = dict(zip(proba_class,
+                                       [cls._PROB_CMAP[pci] for pci in proba_class_indices]))
+        # proba_cmap_dictがproba_classと一致していないとき、エラーを出す
+        if list(proba_cmap_dict.keys()) != proba_class:
+            raise Exception(f'the keys of the "proba_cmap_dict" argument must be equal to the argument "proba_class"')
+
+        # contourf_kwsにalpha指定ないとき、DEFAULT_PROBA_CONTOURF_ALPHAを使用
+        if 'alpha' not in contourf_kws.keys():
+            contourf_kws['alpha'] = cls._DEFAULT_PROBA_CONTOURF_ALPHA
+        # contourf_kwsにlevels指定ないとき、DDEFAULT_PROBA_CONTOURF_LEVELSを使用
+        if 'levels' not in contourf_kws.keys():
+            contourf_kws['levels'] = cls._DEFAULT_PROBA_CONTOURF_LEVELS
+        # imshow_kwsにalpha指定ないとき、DEFAULT_PROBA_RGB_ALPHAを使用
+        if 'alpha' not in imshow_kws.keys():
+            imshow_kws['alpha'] = cls._DEFAULT_PROBA_RGB_ALPHA
+        
+        # クロスバリデーション有無で場合分け
+        # クロスバリデーション未実施時(学習データから学習してプロット)
+        if cv is None:
+            # 学習と推論
+            clf.fit(X, y_true, **fit_params)
+            y_pred = clf.predict(X)
+            # クラス確率を推定
+            proba_pred = clf.predict_proba(X)[:, proba_class_indices]
+            # TODO:クラス確率の順番が逆転した時の対策をメソッドとして実装する必要あり
+            # https://qiita.com/rawHam/items/3bcb6a68a533f2b82a85
+            # クラス確率図をプロット
+            cls._class_chart_plot(clf, X, y_pred, y_true, x_chart, x_not_chart, x_chart_indices,
+                                pair_sigmarange = pair_sigmarange, pair_sigmainterval=pair_sigmainterval, chart_extendsigma=chart_extendsigma, chart_scale=chart_scale,
+                                proba_pred = proba_pred, proba_class_indices = proba_class_indices, plot_border = plot_border, plot_scatter = plot_scatter,
+                                scatter_color_dict=scatter_color_dict, scatter_marker_dict=scatter_marker_dict, proba_cmap_dict=proba_cmap_dict, proba_type = proba_type,
+                                rounddigit_x3=rounddigit_x3, cv_index=None,
+                                subplot_kws=subplot_kws, contourf_kws=contourf_kws, imshow_kws=imshow_kws, scatter_kws=scatter_kws, legend_kws=legend_kws)
+            
+        # クロスバリデーション実施時(分割ごとに別々にプロット＆指標算出)
+        if cv is not None:
+            # 分割法未指定時、cv_numとseedに基づきKFoldでランダムに分割
+            if isinstance(cv, numbers.Integral):
+                cv = KFold(n_splits=cv, shuffle=True, random_state=cv_seed)
+            # LeaveOneOutのときエラーを出す
+            if isinstance(cv, LeaveOneOut):
+                raise Exception('"regression_heat_plot" method does not support "LeaveOneOut" cross validation')
+            # cv_groupをグルーピング対象に指定(GroupKFold、LeaveOneGroupOut等)
+            split_kws={}
+            if cv_group_colname is not None:
+                split_kws['groups'] = data[cv_group_colname].values
+            elif isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
+                raise Exception('"GroupKFold" and "LeaveOneGroupOut" cross validations need ``cv_group`` argument')
+            # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
+            if isinstance(cv, LeaveOneGroupOut):
+                cv_num = len(set(data[cv_group_colname].values))
+            else:
+                cv_num = cv.n_splits
+
+            # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
+            if eval_set_selection is None:
+                eval_set_selection = 'test'
+            fit_params, eval_set_selection = init_eval_set(
+                    eval_set_selection, fit_params, X, y)
+            # 最終学習器以外の前処理変換器作成
+            transformer = _make_transformer(eval_set_selection, clf)
+
+            # クロスバリデーション
+            for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
+                # 表示対象以外のCVなら飛ばす
+                if i not in display_cv_indices:
+                    continue
+                print(f'cv_number={i}/{cv_num}')
+                # グラフタイトル(CV番号を指定。グルーピング系CVのときはグループ名を指定)
+                if isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
+                    cv_index = f'No.{i}  {cv_group_colname}={data[cv_group_colname].values[test][0]}'
+                else:
+                    cv_index = f'No.{i}'
+                # 表示用にテストデータと学習データ分割
+                X_train = X[train]
+                y_train = y_true[train]
+                X_test = X[test]
+                y_test = y_true[test]
+                # proba_class_indicesを学習データから再取得（存在しなければ飛ばす）
+                class_list_train = y_train.tolist()
+                class_list_train = sorted(set(class_list_train), key=class_list_train.index)
+                proba_class_indices = [class_list_train.index(pc) for pc in proba_class if pc in class_list_train]
+                if len(proba_class_indices) == 0:
+                    print(f'there is no assigned "proba_class" in the train data')
+                    continue
+                # proba_cmap_dictも学習データから再取得
+                proba_cmap_dict = {k: v for k, v in proba_cmap_dict.items() if k in class_list_train}
+
+                # eval_setの中から学習データ or テストデータのみを抽出
+                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
+                                                        fit_params, train, test)
+
+                # 学習と推論
+                clf.fit(X_train, y_train, **fit_params_modified)
+                y_pred = clf.predict(X_test)
+                # クラス確率を推定
+                proba_pred = clf.predict_proba(X_test)[:, proba_class_indices]
+                # クラス確率図をプロット
+                cls._class_chart_plot(clf, X_test, y_pred, y_test, x_chart, x_not_chart, x_chart_indices,
+                                    pair_sigmarange = pair_sigmarange, pair_sigmainterval = pair_sigmainterval, chart_extendsigma=chart_extendsigma, chart_scale=chart_scale,
+                                    proba_pred = proba_pred, proba_class_indices = proba_class_indices, plot_border = plot_border, plot_scatter = plot_scatter,
+                                    scatter_color_dict=scatter_color_dict, scatter_marker_dict=scatter_marker_dict, proba_cmap_dict=proba_cmap_dict, proba_type = proba_type,
+                                    rounddigit_x3=rounddigit_x3, cv_index=cv_index,
+                                    subplot_kws=subplot_kws, contourf_kws=contourf_kws, imshow_kws=imshow_kws, scatter_kws=scatter_kws, legend_kws=legend_kws)
+    
+    @classmethod
+    def plot_roc_curve_multiclass(cls, estimator, X_train, y_train, *,
+                                  X_test=None, y_test=None,
+                                  sample_weight=None, drop_intermediate=True,
+                                  response_method="predict_proba", name=None, ax=None, pos_label=None,
+                                  average='macro', fit_params=None,
+                                  plot_roc_kws=None, class_average_kws=None,
+                                  ):
+        """Plot Receiver operating characteristic (ROC) curve.
+
+        Available both multiclass and binary classification
+
+        Extra keyword arguments will be passed to matplotlib's `plot`.
+
+        Parameters
+        ----------
+        estimator : estimator instance
+            Fitted classifier or a fitted :class:`~sklearn.pipeline.Pipeline`
+            in which the last estimator is a classifier.
+
+        X_train : {array-like, sparse matrix} of shape (n_samples, n_features)
+            Input values of train data.
+
+        y_train : array-like of shape (n_samples,)
+            Target values of train data.
+
+        X_test : {array-like, sparse matrix} of shape (n_samples, n_features)
+            Input values of test data.
+
+        y_test : array-like of shape (n_samples,)
+            Target values of test data.
+
+        sample_weight : array-like of shape (n_samples,), default=None
+            Sample weights.
+
+        drop_intermediate : boolean, default=True
+            Whether to drop some suboptimal thresholds which would not appear
+            on a plotted ROC curve. This is useful in order to create lighter
+            ROC curves.
+
+        response_method : {'predict_proba', 'decision_function'}, default='predict_proba'
+            Specifies whether to use for calcurating class probability.
+
+        name : str, default=None
+            Name of ROC Curve for labeling. If `None`, use the name of the
+            estimator.
+
+        ax : matplotlib axes, default=None
+            Axes object to plot on. If `None`, a new figure and axes is created.
+
+        pos_label : str or int, default=None
+            The class considered as the positive class when computing the roc auc
+            metrics. By default, `estimators.classes_[1]` is considered
+            as the positive class.
+
+        average : {'macro', 'micro'}, default='micro'
+            Specifies whether to use for calcurating average of tpr and fpr.
+
+        fit_params : dict, default=None
+            Parameters passed to the fit() method of the classifier, e.g. ``early_stopping_round`` and ``eval_set`` of XGBClassifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
+
+        plot_roc_kws : dict, optional
+            Additional parameters passed to matplotlib.pyplot.plot() that draws ROC curve of each classes, e.g. ``lw``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+        
+        class_average_kws : dict, optional
+            Additional parameters passed to matplotlib.pyplot.plot() or sklearn.metrics.plot_roc_curve() that draws ROC curve of average, e.g. ``alpha``. See https://scikit-learn.org/stable/modules/generated/sklearn.metrics.plot_roc_curve.html
+
+        Returns
+        -------
+        display : :class:`~sklearn.metrics.RocCurveDisplay`
+            Object that stores computed values.
+        """
+
+        # X_testがNoneのとき、X_trainを使用
+        if X_test is None:
+            X_test = X_train
+        # y_testがNoneのとき、y_trainを使用
+        if y_test is None:
+            y_test = y_train
+        # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
+        if ax is None:
+            ax = plt.gca()
+        # 学習時パラメータがNoneなら空のdictを入力
+        if fit_params is None:
+            fit_params = {}
+        # plot_roc_kwsがNoneなら空のdictを入力
+        if plot_roc_kws is None:
+            plot_roc_kws = {}
+        # class_average_kwsがNoneなら空のdictを入力
+        if class_average_kws is None:
+            class_average_kws = {}
+        # 目的変数のクラス一覧
+        y_labels = sorted(np.unique(np.concatenate([y_train, y_test], 0)).tolist())
+        n_classes = len(y_labels)
+        
+        # 2クラス分類のとき
+        if n_classes == 2:
+            estimator.fit(X_train, y_train, **fit_params)
+            viz = RocCurveDisplay.from_estimator(estimator, X_test, y_test,
+                                sample_weight=sample_weight, drop_intermediate=drop_intermediate,
+                                response_method=response_method, name=name, ax=ax, pos_label=pos_label,
+                                **class_average_kws
+                                )
+        # 多クラス分類のとき
+        elif n_classes >= 3:
+            # label_binarize()で目的変数を二値化
+            y_train_binarize = label_binarize(y_train, classes=y_labels)
+            y_test_binarize = label_binarize(y_test, classes=y_labels)
+            # fit_paramsにeval_setがあるとき、二値化
+            eval_sets = [v for v in fit_params.keys() if 'eval_set' in v]
+            if len(eval_sets) > 0 and fit_params[eval_sets[0]] is not None:
+                eval_set_y_binarized = label_binarize(fit_params[eval_sets[0]][0][1], classes=y_labels)
+            # fit_paramsをクラス数で分割
+            fit_params_list = []
+            for i in range(n_classes):
+                fit_params_cls = copy.deepcopy(fit_params)
+                # fit_paramsにeval_setがあるとき、二値化したものに置き換える
+                if len(eval_sets) > 0 and fit_params[eval_sets[0]] is not None:
+                    fit_params_cls[eval_sets[0]] = [(fit_params[eval_sets[0]][0][0], eval_set_y_binarized[:, i])]
+                fit_params_list.append(fit_params_cls)
+                
+            # One vs Restの分類器を作成
+            clf_ovr = OneVsRestClassifierPatched(estimator)
+            clf_ovr.fit(X_train, y_train_binarize,
+                        fit_params_list)
+            # predict_probaまたはdecision_functionでクラス確率を取得
+            if response_method == 'predict_proba':
+                y_score = clf_ovr.predict_proba(X_test)
+            elif response_method == 'decision_function':
+                y_score = clf_ovr.decision_function(X_test)
+            else:
+                raise Exception('The `response_method` argument should be `predict_proba` or `decision_function`')
+            # クラスごとのROC曲線を算出
+            fpr = {}
+            tpr = {}
+            roc_auc = {}
+            for i in range(n_classes):
+                fpr[i], tpr[i], _ = roc_curve(y_test_binarize[:, i], y_score[:, i],
+                                              pos_label=pos_label,
+                                              sample_weight=sample_weight,
+                                              drop_intermediate=drop_intermediate)
+                roc_auc[i] = auc(fpr[i], tpr[i])
+            # micro-averageしたROC曲線を算出
+            fpr["micro"], tpr["micro"], _ = roc_curve(y_test_binarize.ravel(), y_score.ravel(),
+                                                      pos_label=pos_label,
+                                                      sample_weight=sample_weight,
+                                                      drop_intermediate=drop_intermediate)
+            roc_auc["micro"] = auc(fpr["micro"], tpr["micro"])
+            # macro-averageしたROC曲線を算出
+            all_fpr = np.unique(np.concatenate([fpr[i] for i in range(n_classes)]))  # FPRのユニーク値を抽出
+            mean_tpr = np.zeros_like(all_fpr)  # Then interpolate all ROC curves at this points
+            for i in range(n_classes):
+                mean_tpr += np.interp(all_fpr, fpr[i], tpr[i])
+            mean_tpr /= n_classes
+            fpr["macro"] = all_fpr
+            tpr["macro"] = mean_tpr
+            roc_auc["macro"] = auc(fpr["macro"], tpr["macro"])
+
+            # Micro、Macroを選択
+            fpr_avg = fpr[average]
+            tpr_avg = tpr[average]
+            roc_auc_avg = roc_auc[average]
+            fpr_avg_graph = np.concatenate([np.array([0]), fpr_avg])  # グラフ表示用に端点を追加
+            tpr_avg_graph = np.concatenate([np.array([0]), tpr_avg])  # グラフ表示用に端点を追加
+            
+            # class_average_kwsに渡す引数
+            if 'alpha' not in class_average_kws.keys():
+                class_average_kws['alpha'] = 0.8
+            if 'lw' not in class_average_kws.keys():
+                class_average_kws['lw'] = 2
+            if 'linestyle' not in class_average_kws.keys():
+                class_average_kws['linestyle'] = ':'
+            # 平均ROC曲線をプロット
+            ax.plot(fpr_avg_graph, tpr_avg_graph,
+                    label=f'{average}' + '-average ROC (area = {0:0.2f})'
+                        ''.format(roc_auc_avg),
+                    **class_average_kws)
+
+            # ax.plotに渡す引数            
+            if 'alpha' not in plot_roc_kws.keys():
+                plot_roc_kws['alpha'] = 0.4
+            if 'lw' not in plot_roc_kws.keys():
+                plot_roc_kws['lw'] = 1
+            # クラスごとのROC曲線をプロット
+            color_list = list(colors.TABLEAU_COLORS.values())
+            for i, color in zip(range(n_classes), color_list):
+                ax.plot(fpr[i], tpr[i], color=color,
+                        label='ROC class {0} (area = {1:0.2f})'
+                        ''.format(y_labels[i], roc_auc[i]),
+                        **plot_roc_kws)
+            # 軸ラベルと凡例を追加
+            ax.set_xlabel('False Positive rate')
+            ax.set_ylabel('True Positive Rate')
+            ax.legend()
+
+            # FPR、TPR、ROC曲線を保持
+            name = estimator.__class__.__name__ if name is None else name
+            viz = RocCurveDisplay(
+                fpr=fpr_avg,
+                tpr=tpr_avg,
+                roc_auc=roc_auc_avg,
+                estimator_name=name,
+                pos_label=pos_label
+            )
+        
+        return viz
+
+    @classmethod
+    def roc_plot(cls, clf, x: List[str], y: str, data: pd.DataFrame = None,
+                 x_colnames: List[str] = None, 
+                 cv=None, cv_seed=42, cv_group=None,
+                 ax=None,
+                 sample_weight=None, drop_intermediate=True,
+                 response_method="predict_proba", pos_label=None, average='macro',
+                 clf_params=None, fit_params=None, eval_set_selection=None,
+                 draw_grid=True, grid_kws=None, subplot_kws=None, legend_kws=None,
+                 plot_roc_kws=None, class_average_kws=None, cv_mean_kws=None, chance_plot_kws=None):
+        """Plot Receiver operating characteristic (ROC) curve with cross validation.
+
+        Available both binary and multiclass classifiction.
+
+        Extra keyword arguments will be passed to matplotlib's ``plot``.
+
+        Parameters
+        ----------
+        clf: classifier object implementing ``fit``
+            Fitted classifier or a fitted :class:`~sklearn.pipeline.Pipeline`
+            in which the last estimator is a classifier.
+
+        x : list[str], or np.ndarray
+            Explanatory variables. Should be list[str] if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
+
+        y : str or np.ndarray
+            Objective variable. Should be str if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
+
+        data: pd.DataFrame, default=None
+            Input data structure.
+
+        x_colnames: list[str], default=None
+            Names of explanatory variables. Available only if ``data`` is NOT pd.DataFrame
+
+        cv: int or sklearn.model_selection.*, default=5
+            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
+
+        cv_seed: int, default=42
+            Seed for random number generator of cross validation.
+
+        cv_group: str, optional
+            Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
+
+        ax : {matplotlib.axes.Axes, list[matplotlib.axes.Axes]}, default=None
+            Pre-existing axes for the plot or list of it. Otherwise, call matplotlib.pyplot.subplot() internally.
+
+        sample_weight : array-like of shape (n_samples,), default=None
+            Sample weights.
+
+        drop_intermediate : boolean, default=True
+            Whether to drop some suboptimal thresholds which would not appear
+            on a plotted ROC curve. This is useful in order to create lighter
+            ROC curves.
+
+        response_method : {'predict_proba', 'decision_function'}, default='predict_proba'
+            Specifies whether to use for calcurating class probability.
+
+        pos_label : str or int, default=None
+            The class considered as the positive class when computing the roc auc
+            metrics. By default, `estimators.classes_[1]` is considered
+            as the positive class.
+
+        average : {'macro', 'micro'}, default='micro'
+            Specifies whether to use for calcurating average of tpr and fpr.
+
+        clf_params: dict, default=None
+            Parameters passed to the classifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
+
+        fit_params : dict, default=None
+            Parameters passed to the fit() method of the classifier, e.g. ``early_stopping_round`` and ``eval_set`` of XGBClassifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
+        
+        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
+            
+            If "all", use all data in `X` and `y`.
+
+            If "train", select train data from `X` and `y` using cv.split().
+
+            If "test", select test data from `X` and `y` using cv.split().
+
+            If "original", use raw `eval_set`.
+
+            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+
+        draw_grid: bool, default=True
+            If True, grid lines are drawn.
+
+        grid_kws: dict, default=None
+            Additional parameters passed to matplotlib.pyplot.grid() that draws grid lines, e.g. ``color``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.grid.html
+
+        subplot_kws: dict, default=None
+            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize``. Avealable only if ``ax`` is None. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
+
+        legend_kws : dict
+            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
+
+        plot_roc_kws : dict, default=None
+            Additional parameters passed to matplotlib.pyplot.plot() that draws ROC curve of each classes, e.g. ``lw``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+        
+        class_average_kws : dict, default=None
+            Additional parameters passed to matplotlib.pyplot.plot() or sklearn.metrics.plot_roc_curve() that draws average ROC curve of all classes, e.g. ``lw``. See https://scikit-learn.org/stable/modules/generated/sklearn.metrics.plot_roc_curve.html
+        
+        cv_mean_kws : dict, default=None
+            Additional parameters passed to matplotlib.pyplot.plot() that draws mean ROC curve of all folds of cross validation, e.g. ``lw``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+        
+        chance_plot_kws : dict, default=None
+            Additional parameters passed to matplotlib.pyplot.plot() that draws chance line, e.g. ``lw``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+        """
+        # 入力データの形式統一
+        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data(x, y, data,
+                                                                                        x_colnames,
+                                                                                        cv_group)
+
+        # 学習器パラメータがあれば適用
+        if clf_params is not None:
+            clf.set_params(**clf_params)
+        # 学習時パラメータがNoneなら空のdictを入力
+        if fit_params is None:
+            fit_params = {}
+        # grid_kwsがNoneなら空のdictを入力
+        if grid_kws is None:
+            grid_kws = {}
+        # subplot_kwsがNoneなら空のdictを入力
+        if subplot_kws is None:
+            subplot_kws = {}
+        # legend_kwsがNoneなら空のdictを入力
+        if legend_kws is None:
+            legend_kws = {}
+        # plot_roc_kwsがNoneなら空のdictを入力
+        if plot_roc_kws is None:
+            plot_roc_kws = {}
+        # class_average_kwsがNoneなら空のdictを入力
+        if class_average_kws is None:
+            class_average_kws = {}
+        # cv_mean_kwsがNoneなら空のdictを入力
+        if cv_mean_kws is None:
+            cv_mean_kws = {}
+        # chance_plot_kwsがNoneなら空のdictを入力
+        if chance_plot_kws is None:
+            chance_plot_kws = {}
+
+        # クロスバリデーション有無で場合分け
+        # クロスバリデーション未実施時(学習データから学習してプロット)
+        if cv is None:
+            # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
+            if ax is None:
+                ax=plt.gca()
+            # RocCurveDisplay.from_estimatorに渡す引数
+            name = 'ROC'
+            if 'alpha' not in plot_roc_kws.keys():
+                plot_roc_kws['alpha'] = 0.5
+            if 'lw' not in plot_roc_kws.keys():
+                plot_roc_kws['lw'] = 1
+            # ROC曲線をプロット
+            viz = cls.plot_roc_curve_multiclass(clf, X, y_true,
+                                                sample_weight=sample_weight, drop_intermediate=drop_intermediate,
+                                                response_method=response_method, name=name, ax=ax,
+                                                pos_label=pos_label, average=average,
+                                                fit_params = fit_params,
+                                                plot_roc_kws=plot_roc_kws,
+                                                class_average_kws=class_average_kws
+                                                )
+                                  
+        # クロスバリデーション実施時(分割ごとに別々にプロット＆指標算出)
+        if cv is not None:
+            # 分割法未指定時、cv_numとseedに基づきKFoldでランダムに分割
+            if isinstance(cv, numbers.Integral):
+                cv = KFold(n_splits=cv, shuffle=True, random_state=cv_seed)
+            # LeaveOneOutのときエラーを出す
+            if isinstance(cv, LeaveOneOut):
+                raise Exception('"regression_heat_plot" method does not support "LeaveOneOut" cross validation')
+            # cv_groupをグルーピング対象に指定(GroupKFold、LeaveOneGroupOut等)
+            split_kws={}
+            if cv_group_colname is not None:
+                split_kws['groups'] = data[cv_group_colname].values
+            elif isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
+                raise Exception('"GroupKFold" and "LeaveOneGroupOut" cross validations need ``cv_group`` argument')
+            # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
+            if isinstance(cv, LeaveOneGroupOut):
+                cv_num = len(set(data[cv_group_colname].values))
+            else:
+                cv_num = cv.n_splits
+
+            # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
+            if eval_set_selection is None:
+                eval_set_selection = 'test'
+            fit_params, eval_set_selection = init_eval_set(
+                    eval_set_selection, fit_params, X, y)
+            # 最終学習器以外の前処理変換器作成
+            transformer = _make_transformer(eval_set_selection, clf)
+
+            # 表示用のax作成
+            if ax is None:
+                if 'figsize' not in subplot_kws.keys():
+                    subplot_kws['figsize'] = (6, (cv_num + 1) * 6)
+                fig, ax = plt.subplots(cv_num + 1, 1, **subplot_kws)
+
+            # 平均ROC曲線算出用のリスト
+            tprs = []
+            aucs = []
+            mean_fpr = np.linspace(0, 1, 100)
+            color_list = list(colors.TABLEAU_COLORS.values())
+            # クロスバリデーション
+            for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
+                name = 'ROC fold {}'.format(i)
+                # RocCurveDisplay.from_estimatorに渡す引数            
+                if 'alpha' not in plot_roc_kws.keys():
+                    plot_roc_kws['alpha'] = 0.3
+                if 'lw' not in plot_roc_kws.keys():
+                    plot_roc_kws['lw'] = 1
+                # class_average_kwsに渡す引数
+                if 'alpha' not in class_average_kws.keys():
+                    class_average_kws['alpha'] = 0.6
+                if 'lw' not in class_average_kws.keys():
+                    class_average_kws['lw'] = 2
+                if 'linestyle' not in class_average_kws.keys():
+                    class_average_kws['linestyle'] = ':'
+                class_average_kws['color'] = color_list[i]
+
+                # eval_setの中から学習データ or テストデータのみを抽出
+                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
+                                                        fit_params, train, test)
+                
+                # CVごとのROC曲線をプロット
+                viz = cls.plot_roc_curve_multiclass(clf, X[train], y_true[train], 
+                                                    X_test=X[test], y_test=y_true[test],
+                                                    sample_weight=sample_weight, drop_intermediate=drop_intermediate,
+                                                    response_method=response_method,
+                                                    name=name, ax=ax[i],
+                                                    pos_label=pos_label, average=average, fit_params=fit_params_modified,
+                                                    plot_roc_kws=plot_roc_kws,
+                                                    class_average_kws=class_average_kws
+                                                    )
+                ax[i].set_title(f'Cross Validation Fold{i}')
+                # TPRとAUCを保持
+                interp_tpr = np.interp(mean_fpr, viz.fpr, viz.tpr)  # データが存在しない部分を補完
+                interp_tpr[0] = 0.0
+                tprs.append(interp_tpr)
+                aucs.append(viz.roc_auc)
+                # CVごとのROC曲線を全体図にプロット
+                ax[cv_num].plot(mean_fpr, interp_tpr,
+                                label=f'{name} (AUC = {aucs[i]:.2f})',
+                                color=color_list[i],
+                                **plot_roc_kws)
+            
+            # CV平均ROC曲線を計算
+            mean_tpr = np.mean(tprs, axis=0)
+            mean_tpr[-1] = 1.0
+            mean_auc = auc(mean_fpr, mean_tpr)
+            std_auc = np.std(aucs)
+            # CV平均ROC曲線plotに渡す引数
+            if 'label' not in cv_mean_kws.keys():
+                    cv_mean_kws['label'] = r'Mean ROC (AUC = %0.2f $\pm$ %0.2f)' % (mean_auc, std_auc)
+            if 'alpha' not in cv_mean_kws.keys():
+                cv_mean_kws['alpha'] = 0.8
+            if 'lw' not in cv_mean_kws.keys():
+                cv_mean_kws['lw'] = 2
+            if 'color' not in cv_mean_kws.keys():
+                cv_mean_kws['color'] = 'blue'
+            # 平均ROC曲線プロット
+            ax[cv_num].plot(mean_fpr, mean_tpr, **cv_mean_kws)
+            ax[cv_num].set_title('All Cross Validations')
+            # 軸ラベルを追加
+            ax[cv_num].set_xlabel('False Positive rate')
+            ax[cv_num].set_ylabel('True Positive Rate')
+
+        # ランダム時の直線描画に渡す引数
+        if 'label' not in chance_plot_kws.keys():
+                chance_plot_kws['label'] = 'Chance'
+        if 'alpha' not in chance_plot_kws.keys():
+            chance_plot_kws['alpha'] = 0.8
+        if 'lw' not in chance_plot_kws.keys():
+            chance_plot_kws['lw'] = 2
+        if 'color' not in chance_plot_kws.keys():
+            chance_plot_kws['color'] = 'red'
+        if 'linestyle' not in chance_plot_kws.keys():
+            chance_plot_kws['linestyle'] = '--'
+        # ランダム時の直線描画
+        for ax_cv in ax if cv is not None else [ax]:
+            ax_cv.plot([0, 1], [0, 1], **chance_plot_kws)
+            # 凡例追加
+            if 'loc' not in legend_kws.keys():
+                legend_kws['loc'] = 'lower right'
+            ax_cv.legend(**legend_kws)
+            ax_cv.set(xlim=[-0.05, 1.05], ylim=[-0.05, 1.05])
+
+        # グリッド線描画
+        if draw_grid:
+            if 'which' not in grid_kws.keys():
+                grid_kws['which'] = 'major'
+            if 'color' not in grid_kws.keys():
+                grid_kws['color'] = 'lightgrey'
+            if 'linestyle' not in grid_kws.keys():
+                grid_kws['linestyle'] = '-'
+            for ax_cv in ax if cv is not None else [ax]:
                 ax_cv.grid(**grid_kws)
```

### Comparing `seaborn-analyzer-0.2.9/seaborn_analyzer/custom_hist_plot.py` & `seaborn-analyzer-0.3.0/seaborn_analyzer/custom_hist_plot.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,416 +1,416 @@
-from typing import Dict
-import seaborn as sns
-import numpy as np
-import pandas as pd
-import matplotlib.pyplot as plt
-from scipy import stats
-from scipy.stats import distributions
-import decimal
-
-class hist():
-    # 分布フィッティング線のデフォルトカラーマップ
-    _DEFAULT_LINECOLORS = ['red', 'darkmagenta', 'mediumblue', 'darkorange',  'pink', 'brown', 'green', 'cyan', 'gold']
-    
-    def _fit_distribution(x: np.ndarray, distribution: distributions, sigmarange: float, linesplit: int, fit_params: Dict):
-        """
-        分布のフィッティング
-
-        Parameters
-        ----------
-        x : ndarray
-            フィッティング対象のデータ
-        distribution : scipy.stats.distributions
-            分布の種類
-        sigmarange : float
-            フィッティング線の表示範囲（標準偏差の何倍まで表示するか指定）
-        linesplit : int
-            フィッティング線の分割数（カクカクしたら増やす）
-        fit_params : dict
-            フィッティング時に固定するパラメータ
-        """
-        # 表示範囲指定用に平均と不偏標準偏差計算(正規分布のときを基準に)
-        mean = np.mean(x)
-        std = np.std(x, ddof=1)
-
-        # フィッティング実行
-        params = distribution.fit(x, **fit_params)
-        # フィッティング結果のパラメータを分割
-        best_params = {'arg': params[:-2],
-                      'loc': params[-2],
-                      'scale': params[-1]
-                      }
-        # フィッティング曲線の生成
-        Xline = np.linspace(min(mean - std * sigmarange, np.amin(x)), max(mean + std * sigmarange, np.amax(x)), linesplit)
-        Yline = distribution.pdf(Xline, loc=best_params['loc'], scale=best_params['scale'], *best_params['arg'])
-
-        # フィッティングの残差平方和を計算 (参考https://rmizutaa.hatenablog.com/entry/2020/02/24/191312)
-        hist_y, hist_x = np.histogram(x, bins=20, density=True)  # ヒストグラム化して標準化
-        hist_x = (hist_x + np.roll(hist_x, -1))[:-1] / 2.0  # ヒストグラムのxの値をビンの左端→中央に移動
-        pred = distribution.pdf(hist_x, loc=best_params['loc'], scale=best_params['scale'], *best_params['arg'])
-        rss = np.sum(np.power(pred - hist_y, 2.0))
-        # AIC、BICを計算
-        k = len(params) - len(fit_params)  # パラメータ数
-        n = len(x)  # サンプル数
-        logL = np.sum(distribution.logpdf(x, loc=best_params['loc'], scale=best_params['scale'], *best_params['arg']))  # 対数尤度
-        aic = -2 * logL + 2 * k  # AIC
-        bic = -2 * logL + k * np.log(n)  # BIC
-        # 評価指標()
-        fit_scores = {'RSS': rss,
-                      'AIC': aic,
-                      'BIC': bic
-                      }
-
-        return Xline, Yline, best_params, fit_scores
-
-    def _round_digits(src: float, rounddigit: int = None, method='decimal'):
-        """
-        指定桁数で小数を丸める
-
-        Parameters
-        ----------
-        src : float
-            丸め対象の数値
-        rounddigit : int
-            フィッティング線の表示範囲（標準偏差の何倍まで表示するか指定）
-        method : int
-            桁数決定手法（'decimal':小数点以下, 'sig':有効数字(Decimal指定), 'format':formatで有効桁数指定）
-        """
-        if method == 'decimal':
-            return round(src, rounddigit)
-        elif method == 'sig':
-            with decimal.localcontext() as ctx:
-                ctx.prec = rounddigit
-                return ctx.create_decimal(src)
-        elif method == 'format':
-            return '{:.{width}g}'.format(src, width=rounddigit)
-
-    @classmethod
-    def _round_dict_digits(cls, srcdict: Dict[str, float], rounddigit: int = None, method='decimal'):
-        """
-        指定桁数でDictの値を丸める
-
-        Parameters
-        ----------
-        srcdict : dict[str, float]
-            丸め対象のDict
-        rounddigit : int
-            フィッティング線の表示範囲（標準偏差の何倍まで表示するか指定）
-        method : int
-            桁数決定手法（'decimal':小数点以下, 'sig':有効数字(Decimal指定), 'format':formatで有効桁数指定）
-        """
-        dstdict = {}
-        for k, v in srcdict.items():
-            if rounddigit is not None and isinstance(v, float):
-                dstdict[k] = cls._round_digits(v, rounddigit=rounddigit, method=method)
-            else:
-                dstdict[k] = v
-        return dstdict
-
-    @classmethod
-    def fit_dist(cls, data: pd.DataFrame, x: str=None, hue=None, dist='norm', ax=None, binwidth=None, bins='auto', norm_hist=True,
-                  floc=None, sigmarange=4, linecolor='red', linesplit=200, hist_kws={}):
-        """
-        Fit distributions by maximum likelihood estimation, and calculate fitting scores.
-
-        Parameters
-        ----------
-        data : pd.DataFrame, pd.Series, or pd.ndarray
-            Input data structure. Either a long-form collection of vectors that can be assigned to named variables or a wide-form dataset that will be internally reshaped.
-        x : str, optional
-            Variables that specify positions on the x. Available only if data is pd.DataFrame.
-        hue : str, pd.Series, or pd.ndarray, optional
-            Semantic variable that is mapped to determine the color of plot elements. If ``data`` is pd.DataFrame, the argument must be key in data.
-        dist : {'norm', 'lognorm', 'gamma', 't', 'expon', 'uniform', 'chi2', 'weibull'} or list, optional
-            Type of fitting distribution or list of distrbutions.
-        ax : matplotlib.axes.Axes, optional
-            Pre-existing axes for the plot. Otherwise, call matplotlib.pyplot.gca() internally.
-        binwidth : float, optional
-            Width of each bin, overrides ``bins``.
-        bins : int, optional
-            Generic bin parameter that can be the name of a reference rule, the number of bins, or the breaks of the bins. Passed to numpy.histogram_bin_edges().
-        norm_hist : bool, optional
-            If True, the histogram height shows a density rather than a count.
-        floc : float, optional
-            Hold location parameter fixed to specified value. If None, location parameter is fitted by maximum likelihood estimation except when ``dist`` is 'weibull' or expon'. See https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.rv_continuous.fit.html#scipy.stats.rv_continuous.fit
-        sigmarange : float, optional
-            Set the x-axis view limits. The lower limit is -sigmarange * std(data) + mean(data). The higher limit is sigmarange * std(data) + mean(data).
-        linecolor : str or List[str], optional
-            Color of fitting line or colors of fitting lines. See https://matplotlib.org/stable/gallery/color/named_colors.html
-        linesplit : int, optional
-            Number of fitting line divisions.
-        hist_kws : dict, optional
-            Additional parameters passed to seaborn.histplot() other than the above arguments.
-        
-        Returns
-        ----------
-        all_params : dict
-            Parameters estimated by maximum likelihood estimation.
-        all_scores : dict
-            Fitting scores, which consist of RSS, AIC, and BIC.
-        """
-
-        # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
-        if ax == None:
-            ax=plt.gca()
-        
-        # スタイルを変更 (デフォルト設定は見づらいため)
-        if 'alpha' not in hist_kws.keys():
-            hist_kws['alpha'] = 0.7
-        if 'edgecolor' not in hist_kws.keys():
-            hist_kws['edgecolor'] = 'white'
-
-        # フィッティング対象データをndarrayで抽出
-        if isinstance(data, pd.DataFrame):
-            X = data[x].values
-        elif isinstance(data, pd.Series):
-            X = data.values
-        elif isinstance(data, np.ndarray):
-            X = data
-        # フィッティング対象データの最小値よりflocが大きい場合、エラーを出す
-        if floc is not None and floc >= np.amin(X):
-            raise Exception('the "floc" argument must be larger than minimum of data')
-
-        # ビンサイズを設定
-        if binwidth is not None:
-            if bins == 'auto':
-                bins = np.arange(np.floor(X.min()), np.ceil(X.max()), binwidth)
-            else: # binsとbin_widthは同時指定できない
-                raise Exception('the arguments "bins" and "binwidth" cannot coexist')
-
-        # norm_hist=Trueのとき、statをdensityに指定 (histplotの引数)
-        stat = 'density' if norm_hist else 'count'
-        # 色分けあるとき、ヒストグラム種類を積み上げに指定 (histplotの引数)
-        multiple = 'layer' if hue is None else 'stack'
-
-        # ヒストグラム描画
-        ax = sns.histplot(data, x=x, hue=hue, ax=ax, bins=bins, stat=stat, multiple=multiple, **hist_kws)
-
-        # 色分けあるとき、凡例を左上に表示
-        if hue is not None:
-            lg = ax.legend_
-            handles = lg.legendHandles
-            labels = [t.get_text() for t in lg.texts]
-            leg_hist = ax.legend(handles, labels, loc='upper left')
-            ax.add_artist(leg_hist)
-
-        # distをList化
-        dists = [dist] if not isinstance(dist, list) else dist
-        # フィッティング線の色指定をリスト化
-        linecolor = [linecolor] if isinstance(linecolor, str) else linecolor
-        # 2種類以上をプロットしており、かつ色指定がListでないとき、他の色を追加
-        if len(dists) >= 2:
-            if len(linecolor) == 1:
-                linecolor = cls._DEFAULT_LINECOLORS
-            elif len(dists) != len(linecolor):
-                raise Exception('the length of the "linecolor" argument must be equal to the length of the "dist" argument')
-
-        # 分布をフィッティング
-        all_params = {}
-        all_scores = {}
-        line_legends = []
-        for i, distribution in enumerate(dists):
-            fit_params = {}
-            # 分布が文字列型のとき、scipy.stats.distributionsに変更
-            if isinstance(distribution, str):
-                if distribution == 'norm':
-                    distribution = stats.norm
-                elif distribution == 'lognorm':
-                    distribution = stats.lognorm
-                elif distribution == 'gamma':
-                    distribution = stats.gamma
-                elif distribution == 'cauchy':
-                    distribution = stats.cauchy
-                elif distribution == 't':
-                    distribution = stats.t
-                elif distribution == 'pareto':
-                    distribution = stats.pareto
-                elif distribution == 'uniform':
-                    distribution = stats.uniform
-                elif distribution == 'expon':
-                    distribution = stats.expon
-                    fit_params = {'floc': 0} # 指数分布のとき、locパラメータを0で固定
-                elif distribution == 'weibull':
-                    distribution = stats.weibull_min
-                    fit_params = {'floc': 0} # ワイブル分布のとき、locパラメータを0で固定
-                elif distribution == 'chi2':
-                    distribution = stats.chi2
-                    fit_params = {'floc': 0,  # カイ二乗分布のとき、locパラメータを0で固定
-                                  'fscale': 1,  # カイ二乗分布のとき、scaleパラメータを1で固定
-                                  }
-
-            # flocしているとき、X方向オフセットを指定値で固定
-            if floc is not None:
-                fit_params['floc'] = floc
-            # 分布フィット
-            xline, yline, best_params, fit_scores = cls._fit_distribution(X, distribution, sigmarange, linesplit, fit_params)
-
-            # 標準化していないとき、ヒストグラムと最大値の8割を合わせるようフィッティング線の倍率調整
-            if norm_hist is False:
-                line_max = np.amax(yline)
-                hist_max = ax.get_ylim()[1]
-                yline = yline * hist_max / line_max * 0.8
-            # フィッティング線の描画
-            leg, = ax.plot(xline, yline, color=linecolor[i])
-            line_legends.append(leg)
-
-            # フィッティング結果パラメータをdict化
-            params = {}
-            # 正規分布
-            if distribution == stats.norm:
-                params['mean'] = best_params['loc']
-                params['std'] = best_params['scale']
-                all_params['norm'] = params
-                all_scores['norm'] = fit_scores  # フィッティングの評価指標
-            # 対数正規分布 (通常の対数正規分布＋オフセット、参考https://analytics-note.xyz/statistics/scipy-lognorm/)
-            elif distribution == stats.lognorm:
-                params['mu'] = np.log(best_params['scale'])
-                params['sigma'] = best_params['arg'][0]
-                params['loc'] = best_params['loc']
-                all_params['lognorm'] = params
-                all_scores['lognorm'] = fit_scores  # フィッティングの評価指標
-            # ガンマ分布 (通常のガンマ分布＋オフセット、参考https://qiita.com/kidaufo/items/2a5ba5a4bf100dc0f106)
-            elif distribution == stats.gamma:
-                params['theta'] = best_params['scale']
-                params['k'] = best_params['arg'][0]
-                params['loc'] = best_params['loc']
-                all_params['gamma'] = params
-                all_scores['gamma'] = fit_scores  # フィッティングの評価指標
-            # コーシー分布 (通常のコーシー分布＋オフセット＋スケール、参考https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.cauchy.html)
-            elif distribution == stats.cauchy:
-                params['scale'] = best_params['scale']
-                params['loc'] = best_params['loc']
-                all_params['cauchy'] = params
-                all_scores['cauchy'] = fit_scores  # フィッティングの評価指標
-            # t分布 (通常のt分布＋オフセット＋スケール、参考https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.t.html)
-            elif distribution == stats.t:
-                params['scale'] = best_params['scale']
-                params['df'] = best_params['arg'][0]
-                params['loc'] = best_params['loc']
-                all_params['t'] = params
-                all_scores['t'] = fit_scores  # フィッティングの評価指標
-            # パレート分布 (通常のパレート分布＋オフセット、参考https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.pareto.html)
-            elif distribution == stats.pareto:
-                params['scale'] = best_params['scale']
-                params['b'] = best_params['arg'][0]
-                params['loc'] = best_params['loc']
-                all_params['pareto'] = params
-                all_scores['pareto'] = fit_scores  # フィッティングの評価指標
-            # 一様分布 (オフセット＋スケール、参考https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.uniform.html)
-            elif distribution == stats.uniform:
-                params['scale'] = best_params['scale']
-                params['loc'] = best_params['loc']
-                all_params['uniform'] = params
-                all_scores['uniform'] = fit_scores  # フィッティングの評価指標
-            # 指数分布 (オフセットなし、参考https://stackoverflow.com/questions/25085200/scipy-stats-expon-fit-with-no-location-parameter)
-            elif distribution == stats.expon:
-                params['lambda'] = 1 / best_params['scale']
-                params['loc'] = best_params['loc']
-                all_params['expon'] = params
-                all_scores['expon'] = fit_scores  # フィッティングの評価指標
-            # ワイブル分布 (オフセットなし、参考https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.weibull_min.html)
-            elif distribution == stats.weibull_min:
-                params['c'] = best_params['scale']
-                params['k'] = best_params['arg'][0]
-                params['loc'] = best_params['loc']
-                all_params['weibull'] = params
-                all_scores['weibull'] = fit_scores  # フィッティングの評価指標
-            # カイ二乗分布 (オフセット・スケールなし、参考https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.chi2.html)
-            elif distribution == stats.chi2:
-                params['df'] = best_params['arg'][0]
-                all_params['chi2'] = params
-                all_scores['chi2'] = fit_scores  # フィッティングの評価指標
-            # その他の分布
-            else:
-                all_params[distribution.name] = params
-                all_scores[distribution.name] = fit_scores
-            
-        # フィッティング線の凡例をプロット (2色以上のときのみ)
-        if len(dists) >= 2:
-            line_labels = [d if isinstance(d, str) else d.name for d in dists]
-            ax.legend(line_legends, line_labels, loc='upper right')
-
-        return all_params, all_scores
-
-
-
-    @classmethod
-    def plot_normality(cls, data: pd.DataFrame, x: str=None, hue=None, binwidth=None, bins='auto', norm_hist=False,
-                        sigmarange=4, linesplit=200, rounddigit=5,
-                        hist_kws={}, subplot_kws={}):
-        """
-        Plot normality test result and QQ plot.
-
-        Parameters
-        ----------
-        data : pd.DataFrame, pd.Series, or pd.ndarray
-            Input data structure. Either a long-form collection of vectors that can be assigned to named variables or a wide-form dataset that will be internally reshaped.
-        x : str, optional
-            Variables that specify positions on the x. Available only if data is pd.DataFrame.
-        hue : str, optional
-            Semantic variable that is mapped to determine the color of plot elements. Available only if ``data`` is pd.DataFrame
-        binwidth : float, optional
-            Width of each bin, overrides ``bins``.
-        bins : int, optional
-            Generic bin parameter that can be the name of a reference rule, the number of bins, or the breaks of the bins. Passed to numpy.histogram_bin_edges().
-        norm_hist : bool, optional
-            If True, the histogram height shows a density rather than a count.
-        sigmarange : float, optional
-            Set the x-axis view limits. The lower limit is -sigmarange * std(data) + mean(data). The higher limit is sigmarange * std(data) + mean(data).
-        linesplit : int, optional
-            Number of fitting line divisions.
-        rounddigit: int, optional
-            Round a number of score to a given precision in decimal digits.
-        hist_kws : dict, optional
-            Additional parameters passed to seaborn.histplot() other than the above arguments.
-        subplot_kws : dict, optional
-            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. figsize. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
-        """
-
-        # 描画用のsubplots作成
-        if 'figsize' not in subplot_kws.keys():
-            subplot_kws['figsize'] = (6, 12)
-        fig, axes = plt.subplots(2, 1, **subplot_kws)
-
-        # QQプロット描画
-        if isinstance(data, pd.DataFrame):
-            X = data[x].values
-        elif isinstance(data, pd.Series):
-            X = data.values
-        elif isinstance(data, np.ndarray):
-            X = data
-        stats.probplot(X, dist='norm', plot=axes[0])
-
-        # ヒストグラムとフィッティング線を描画
-        cls.fit_dist(data, x=x, hue=hue, dist='norm', ax=axes[1], binwidth=binwidth, bins=bins, norm_hist=norm_hist,
-                      sigmarange=sigmarange, linecolor='red', linesplit=linesplit, hist_kws=hist_kws)
-        # 平均と不偏標準偏差を計算し、ヒストグラム図中に記載
-        mean = np.mean(X)
-        std = np.std(X, ddof=1)
-        if rounddigit > 0:  # rounddigitが0のときは文字表示しない
-            params = {'mean':mean,
-                    'std':std
-                    }
-            param_list = [f'{k}={v}' for k, v in cls._round_dict_digits(params, rounddigit, 'sig').items()]
-            param_text = "\n".join(param_list)
-            axes[1].text(axes[1].get_xlim()[0] + (axes[1].get_xlim()[1] - axes[1].get_xlim()[0]) * 0.95,
-                        axes[1].get_ylim()[1] * 0.9,
-                        param_text, verticalalignment='top', horizontalalignment='right')
-
-        # 正規性検定
-        if len(X) <= 2000: # シャピロウィルク検定 (N<=2000のとき)
-            method = 'shapiro-wilk'
-            normality=stats.shapiro(X)
-        else: # コルモゴロフ-スミルノフ検定 (N>2000のとき)
-            method = 'kolmogorov-smirnov'
-            normality = stats.kstest(X, stats.norm(loc=mean, scale=std).cdf)
-        # 検定結果を図中に記載
-        if rounddigit > 0:  # rounddigitが0のときは文字表示しない
-            params = {'statistic':normality.statistic,
-                    'pvalue':normality.pvalue,
-                    }
-            param_list = [f'{k}={v}' for k, v in cls._round_dict_digits(params, rounddigit, 'sig').items()]
-            param_list.insert(0, f'method={method}')
-            param_text = "\n".join(param_list)
-            axes[0].text(axes[0].get_xlim()[0] + (axes[0].get_xlim()[1] - axes[0].get_xlim()[0]) * 0.95,
-                        axes[0].get_ylim()[0] + (axes[0].get_ylim()[1] - axes[0].get_ylim()[0]) * 0.1,
+from typing import Dict
+import seaborn as sns
+import numpy as np
+import pandas as pd
+import matplotlib.pyplot as plt
+from scipy import stats
+from scipy.stats import distributions
+import decimal
+
+class hist():
+    # 分布フィッティング線のデフォルトカラーマップ
+    _DEFAULT_LINECOLORS = ['red', 'darkmagenta', 'mediumblue', 'darkorange',  'pink', 'brown', 'green', 'cyan', 'gold']
+    
+    def _fit_distribution(x: np.ndarray, distribution: distributions, sigmarange: float, linesplit: int, fit_params: Dict):
+        """
+        分布のフィッティング
+
+        Parameters
+        ----------
+        x : ndarray
+            フィッティング対象のデータ
+        distribution : scipy.stats.distributions
+            分布の種類
+        sigmarange : float
+            フィッティング線の表示範囲（標準偏差の何倍まで表示するか指定）
+        linesplit : int
+            フィッティング線の分割数（カクカクしたら増やす）
+        fit_params : dict
+            フィッティング時に固定するパラメータ
+        """
+        # 表示範囲指定用に平均と不偏標準偏差計算(正規分布のときを基準に)
+        mean = np.mean(x)
+        std = np.std(x, ddof=1)
+
+        # フィッティング実行
+        params = distribution.fit(x, **fit_params)
+        # フィッティング結果のパラメータを分割
+        best_params = {'arg': params[:-2],
+                      'loc': params[-2],
+                      'scale': params[-1]
+                      }
+        # フィッティング曲線の生成
+        Xline = np.linspace(min(mean - std * sigmarange, np.amin(x)), max(mean + std * sigmarange, np.amax(x)), linesplit)
+        Yline = distribution.pdf(Xline, loc=best_params['loc'], scale=best_params['scale'], *best_params['arg'])
+
+        # フィッティングの残差平方和を計算 (参考https://rmizutaa.hatenablog.com/entry/2020/02/24/191312)
+        hist_y, hist_x = np.histogram(x, bins=20, density=True)  # ヒストグラム化して標準化
+        hist_x = (hist_x + np.roll(hist_x, -1))[:-1] / 2.0  # ヒストグラムのxの値をビンの左端→中央に移動
+        pred = distribution.pdf(hist_x, loc=best_params['loc'], scale=best_params['scale'], *best_params['arg'])
+        rss = np.sum(np.power(pred - hist_y, 2.0))
+        # AIC、BICを計算
+        k = len(params) - len(fit_params)  # パラメータ数
+        n = len(x)  # サンプル数
+        logL = np.sum(distribution.logpdf(x, loc=best_params['loc'], scale=best_params['scale'], *best_params['arg']))  # 対数尤度
+        aic = -2 * logL + 2 * k  # AIC
+        bic = -2 * logL + k * np.log(n)  # BIC
+        # 評価指標()
+        fit_scores = {'RSS': rss,
+                      'AIC': aic,
+                      'BIC': bic
+                      }
+
+        return Xline, Yline, best_params, fit_scores
+
+    def _round_digits(src: float, rounddigit: int = None, method='decimal'):
+        """
+        指定桁数で小数を丸める
+
+        Parameters
+        ----------
+        src : float
+            丸め対象の数値
+        rounddigit : int
+            フィッティング線の表示範囲（標準偏差の何倍まで表示するか指定）
+        method : int
+            桁数決定手法（'decimal':小数点以下, 'sig':有効数字(Decimal指定), 'format':formatで有効桁数指定）
+        """
+        if method == 'decimal':
+            return round(src, rounddigit)
+        elif method == 'sig':
+            with decimal.localcontext() as ctx:
+                ctx.prec = rounddigit
+                return ctx.create_decimal(src)
+        elif method == 'format':
+            return '{:.{width}g}'.format(src, width=rounddigit)
+
+    @classmethod
+    def _round_dict_digits(cls, srcdict: Dict[str, float], rounddigit: int = None, method='decimal'):
+        """
+        指定桁数でDictの値を丸める
+
+        Parameters
+        ----------
+        srcdict : dict[str, float]
+            丸め対象のDict
+        rounddigit : int
+            フィッティング線の表示範囲（標準偏差の何倍まで表示するか指定）
+        method : int
+            桁数決定手法（'decimal':小数点以下, 'sig':有効数字(Decimal指定), 'format':formatで有効桁数指定）
+        """
+        dstdict = {}
+        for k, v in srcdict.items():
+            if rounddigit is not None and isinstance(v, float):
+                dstdict[k] = cls._round_digits(v, rounddigit=rounddigit, method=method)
+            else:
+                dstdict[k] = v
+        return dstdict
+
+    @classmethod
+    def fit_dist(cls, data: pd.DataFrame, x: str=None, hue=None, dist='norm', ax=None, binwidth=None, bins='auto', norm_hist=True,
+                  floc=None, sigmarange=4, linecolor='red', linesplit=200, hist_kws={}):
+        """
+        Fit distributions by maximum likelihood estimation, and calculate fitting scores.
+
+        Parameters
+        ----------
+        data : pd.DataFrame, pd.Series, or pd.ndarray
+            Input data structure. Either a long-form collection of vectors that can be assigned to named variables or a wide-form dataset that will be internally reshaped.
+        x : str, optional
+            Variables that specify positions on the x. Available only if data is pd.DataFrame.
+        hue : str, pd.Series, or pd.ndarray, optional
+            Semantic variable that is mapped to determine the color of plot elements. If ``data`` is pd.DataFrame, the argument must be key in data.
+        dist : {'norm', 'lognorm', 'gamma', 't', 'expon', 'uniform', 'chi2', 'weibull'} or list, optional
+            Type of fitting distribution or list of distrbutions.
+        ax : matplotlib.axes.Axes, optional
+            Pre-existing axes for the plot. Otherwise, call matplotlib.pyplot.gca() internally.
+        binwidth : float, optional
+            Width of each bin, overrides ``bins``.
+        bins : int, optional
+            Generic bin parameter that can be the name of a reference rule, the number of bins, or the breaks of the bins. Passed to numpy.histogram_bin_edges().
+        norm_hist : bool, optional
+            If True, the histogram height shows a density rather than a count.
+        floc : float, optional
+            Hold location parameter fixed to specified value. If None, location parameter is fitted by maximum likelihood estimation except when ``dist`` is 'weibull' or expon'. See https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.rv_continuous.fit.html#scipy.stats.rv_continuous.fit
+        sigmarange : float, optional
+            Set the x-axis view limits. The lower limit is -sigmarange * std(data) + mean(data). The higher limit is sigmarange * std(data) + mean(data).
+        linecolor : str or List[str], optional
+            Color of fitting line or colors of fitting lines. See https://matplotlib.org/stable/gallery/color/named_colors.html
+        linesplit : int, optional
+            Number of fitting line divisions.
+        hist_kws : dict, optional
+            Additional parameters passed to seaborn.histplot() other than the above arguments.
+        
+        Returns
+        ----------
+        all_params : dict
+            Parameters estimated by maximum likelihood estimation.
+        all_scores : dict
+            Fitting scores, which consist of RSS, AIC, and BIC.
+        """
+
+        # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
+        if ax == None:
+            ax=plt.gca()
+        
+        # スタイルを変更 (デフォルト設定は見づらいため)
+        if 'alpha' not in hist_kws.keys():
+            hist_kws['alpha'] = 0.7
+        if 'edgecolor' not in hist_kws.keys():
+            hist_kws['edgecolor'] = 'white'
+
+        # フィッティング対象データをndarrayで抽出
+        if isinstance(data, pd.DataFrame):
+            X = data[x].values
+        elif isinstance(data, pd.Series):
+            X = data.values
+        elif isinstance(data, np.ndarray):
+            X = data
+        # フィッティング対象データの最小値よりflocが大きい場合、エラーを出す
+        if floc is not None and floc >= np.amin(X):
+            raise Exception('the "floc" argument must be larger than minimum of data')
+
+        # ビンサイズを設定
+        if binwidth is not None:
+            if bins == 'auto':
+                bins = np.arange(np.floor(X.min()), np.ceil(X.max()), binwidth)
+            else: # binsとbin_widthは同時指定できない
+                raise Exception('the arguments "bins" and "binwidth" cannot coexist')
+
+        # norm_hist=Trueのとき、statをdensityに指定 (histplotの引数)
+        stat = 'density' if norm_hist else 'count'
+        # 色分けあるとき、ヒストグラム種類を積み上げに指定 (histplotの引数)
+        multiple = 'layer' if hue is None else 'stack'
+
+        # ヒストグラム描画
+        ax = sns.histplot(data, x=x, hue=hue, ax=ax, bins=bins, stat=stat, multiple=multiple, **hist_kws)
+
+        # 色分けあるとき、凡例を左上に表示
+        if hue is not None:
+            lg = ax.legend_
+            handles = lg.legendHandles
+            labels = [t.get_text() for t in lg.texts]
+            leg_hist = ax.legend(handles, labels, loc='upper left')
+            ax.add_artist(leg_hist)
+
+        # distをList化
+        dists = [dist] if not isinstance(dist, list) else dist
+        # フィッティング線の色指定をリスト化
+        linecolor = [linecolor] if isinstance(linecolor, str) else linecolor
+        # 2種類以上をプロットしており、かつ色指定がListでないとき、他の色を追加
+        if len(dists) >= 2:
+            if len(linecolor) == 1:
+                linecolor = cls._DEFAULT_LINECOLORS
+            elif len(dists) != len(linecolor):
+                raise Exception('the length of the "linecolor" argument must be equal to the length of the "dist" argument')
+
+        # 分布をフィッティング
+        all_params = {}
+        all_scores = {}
+        line_legends = []
+        for i, distribution in enumerate(dists):
+            fit_params = {}
+            # 分布が文字列型のとき、scipy.stats.distributionsに変更
+            if isinstance(distribution, str):
+                if distribution == 'norm':
+                    distribution = stats.norm
+                elif distribution == 'lognorm':
+                    distribution = stats.lognorm
+                elif distribution == 'gamma':
+                    distribution = stats.gamma
+                elif distribution == 'cauchy':
+                    distribution = stats.cauchy
+                elif distribution == 't':
+                    distribution = stats.t
+                elif distribution == 'pareto':
+                    distribution = stats.pareto
+                elif distribution == 'uniform':
+                    distribution = stats.uniform
+                elif distribution == 'expon':
+                    distribution = stats.expon
+                    fit_params = {'floc': 0} # 指数分布のとき、locパラメータを0で固定
+                elif distribution == 'weibull':
+                    distribution = stats.weibull_min
+                    fit_params = {'floc': 0} # ワイブル分布のとき、locパラメータを0で固定
+                elif distribution == 'chi2':
+                    distribution = stats.chi2
+                    fit_params = {'floc': 0,  # カイ二乗分布のとき、locパラメータを0で固定
+                                  'fscale': 1,  # カイ二乗分布のとき、scaleパラメータを1で固定
+                                  }
+
+            # flocしているとき、X方向オフセットを指定値で固定
+            if floc is not None:
+                fit_params['floc'] = floc
+            # 分布フィット
+            xline, yline, best_params, fit_scores = cls._fit_distribution(X, distribution, sigmarange, linesplit, fit_params)
+
+            # 標準化していないとき、ヒストグラムと最大値の8割を合わせるようフィッティング線の倍率調整
+            if norm_hist is False:
+                line_max = np.amax(yline)
+                hist_max = ax.get_ylim()[1]
+                yline = yline * hist_max / line_max * 0.8
+            # フィッティング線の描画
+            leg, = ax.plot(xline, yline, color=linecolor[i])
+            line_legends.append(leg)
+
+            # フィッティング結果パラメータをdict化
+            params = {}
+            # 正規分布
+            if distribution == stats.norm:
+                params['mean'] = best_params['loc']
+                params['std'] = best_params['scale']
+                all_params['norm'] = params
+                all_scores['norm'] = fit_scores  # フィッティングの評価指標
+            # 対数正規分布 (通常の対数正規分布＋オフセット、参考https://analytics-note.xyz/statistics/scipy-lognorm/)
+            elif distribution == stats.lognorm:
+                params['mu'] = np.log(best_params['scale'])
+                params['sigma'] = best_params['arg'][0]
+                params['loc'] = best_params['loc']
+                all_params['lognorm'] = params
+                all_scores['lognorm'] = fit_scores  # フィッティングの評価指標
+            # ガンマ分布 (通常のガンマ分布＋オフセット、参考https://qiita.com/kidaufo/items/2a5ba5a4bf100dc0f106)
+            elif distribution == stats.gamma:
+                params['theta'] = best_params['scale']
+                params['k'] = best_params['arg'][0]
+                params['loc'] = best_params['loc']
+                all_params['gamma'] = params
+                all_scores['gamma'] = fit_scores  # フィッティングの評価指標
+            # コーシー分布 (通常のコーシー分布＋オフセット＋スケール、参考https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.cauchy.html)
+            elif distribution == stats.cauchy:
+                params['scale'] = best_params['scale']
+                params['loc'] = best_params['loc']
+                all_params['cauchy'] = params
+                all_scores['cauchy'] = fit_scores  # フィッティングの評価指標
+            # t分布 (通常のt分布＋オフセット＋スケール、参考https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.t.html)
+            elif distribution == stats.t:
+                params['scale'] = best_params['scale']
+                params['df'] = best_params['arg'][0]
+                params['loc'] = best_params['loc']
+                all_params['t'] = params
+                all_scores['t'] = fit_scores  # フィッティングの評価指標
+            # パレート分布 (通常のパレート分布＋オフセット、参考https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.pareto.html)
+            elif distribution == stats.pareto:
+                params['scale'] = best_params['scale']
+                params['b'] = best_params['arg'][0]
+                params['loc'] = best_params['loc']
+                all_params['pareto'] = params
+                all_scores['pareto'] = fit_scores  # フィッティングの評価指標
+            # 一様分布 (オフセット＋スケール、参考https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.uniform.html)
+            elif distribution == stats.uniform:
+                params['scale'] = best_params['scale']
+                params['loc'] = best_params['loc']
+                all_params['uniform'] = params
+                all_scores['uniform'] = fit_scores  # フィッティングの評価指標
+            # 指数分布 (オフセットなし、参考https://stackoverflow.com/questions/25085200/scipy-stats-expon-fit-with-no-location-parameter)
+            elif distribution == stats.expon:
+                params['lambda'] = 1 / best_params['scale']
+                params['loc'] = best_params['loc']
+                all_params['expon'] = params
+                all_scores['expon'] = fit_scores  # フィッティングの評価指標
+            # ワイブル分布 (オフセットなし、参考https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.weibull_min.html)
+            elif distribution == stats.weibull_min:
+                params['c'] = best_params['scale']
+                params['k'] = best_params['arg'][0]
+                params['loc'] = best_params['loc']
+                all_params['weibull'] = params
+                all_scores['weibull'] = fit_scores  # フィッティングの評価指標
+            # カイ二乗分布 (オフセット・スケールなし、参考https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.chi2.html)
+            elif distribution == stats.chi2:
+                params['df'] = best_params['arg'][0]
+                all_params['chi2'] = params
+                all_scores['chi2'] = fit_scores  # フィッティングの評価指標
+            # その他の分布
+            else:
+                all_params[distribution.name] = params
+                all_scores[distribution.name] = fit_scores
+            
+        # フィッティング線の凡例をプロット (2色以上のときのみ)
+        if len(dists) >= 2:
+            line_labels = [d if isinstance(d, str) else d.name for d in dists]
+            ax.legend(line_legends, line_labels, loc='upper right')
+
+        return all_params, all_scores
+
+
+
+    @classmethod
+    def plot_normality(cls, data: pd.DataFrame, x: str=None, hue=None, binwidth=None, bins='auto', norm_hist=False,
+                        sigmarange=4, linesplit=200, rounddigit=5,
+                        hist_kws={}, subplot_kws={}):
+        """
+        Plot normality test result and QQ plot.
+
+        Parameters
+        ----------
+        data : pd.DataFrame, pd.Series, or pd.ndarray
+            Input data structure. Either a long-form collection of vectors that can be assigned to named variables or a wide-form dataset that will be internally reshaped.
+        x : str, optional
+            Variables that specify positions on the x. Available only if data is pd.DataFrame.
+        hue : str, optional
+            Semantic variable that is mapped to determine the color of plot elements. Available only if ``data`` is pd.DataFrame
+        binwidth : float, optional
+            Width of each bin, overrides ``bins``.
+        bins : int, optional
+            Generic bin parameter that can be the name of a reference rule, the number of bins, or the breaks of the bins. Passed to numpy.histogram_bin_edges().
+        norm_hist : bool, optional
+            If True, the histogram height shows a density rather than a count.
+        sigmarange : float, optional
+            Set the x-axis view limits. The lower limit is -sigmarange * std(data) + mean(data). The higher limit is sigmarange * std(data) + mean(data).
+        linesplit : int, optional
+            Number of fitting line divisions.
+        rounddigit: int, optional
+            Round a number of score to a given precision in decimal digits.
+        hist_kws : dict, optional
+            Additional parameters passed to seaborn.histplot() other than the above arguments.
+        subplot_kws : dict, optional
+            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. figsize. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
+        """
+
+        # 描画用のsubplots作成
+        if 'figsize' not in subplot_kws.keys():
+            subplot_kws['figsize'] = (6, 12)
+        fig, axes = plt.subplots(2, 1, **subplot_kws)
+
+        # QQプロット描画
+        if isinstance(data, pd.DataFrame):
+            X = data[x].values
+        elif isinstance(data, pd.Series):
+            X = data.values
+        elif isinstance(data, np.ndarray):
+            X = data
+        stats.probplot(X, dist='norm', plot=axes[0])
+
+        # ヒストグラムとフィッティング線を描画
+        cls.fit_dist(data, x=x, hue=hue, dist='norm', ax=axes[1], binwidth=binwidth, bins=bins, norm_hist=norm_hist,
+                      sigmarange=sigmarange, linecolor='red', linesplit=linesplit, hist_kws=hist_kws)
+        # 平均と不偏標準偏差を計算し、ヒストグラム図中に記載
+        mean = np.mean(X)
+        std = np.std(X, ddof=1)
+        if rounddigit > 0:  # rounddigitが0のときは文字表示しない
+            params = {'mean':mean,
+                    'std':std
+                    }
+            param_list = [f'{k}={v}' for k, v in cls._round_dict_digits(params, rounddigit, 'sig').items()]
+            param_text = "\n".join(param_list)
+            axes[1].text(axes[1].get_xlim()[0] + (axes[1].get_xlim()[1] - axes[1].get_xlim()[0]) * 0.95,
+                        axes[1].get_ylim()[1] * 0.9,
+                        param_text, verticalalignment='top', horizontalalignment='right')
+
+        # 正規性検定
+        if len(X) <= 2000: # シャピロウィルク検定 (N<=2000のとき)
+            method = 'shapiro-wilk'
+            normality=stats.shapiro(X)
+        else: # コルモゴロフ-スミルノフ検定 (N>2000のとき)
+            method = 'kolmogorov-smirnov'
+            normality = stats.kstest(X, stats.norm(loc=mean, scale=std).cdf)
+        # 検定結果を図中に記載
+        if rounddigit > 0:  # rounddigitが0のときは文字表示しない
+            params = {'statistic':normality.statistic,
+                    'pvalue':normality.pvalue,
+                    }
+            param_list = [f'{k}={v}' for k, v in cls._round_dict_digits(params, rounddigit, 'sig').items()]
+            param_list.insert(0, f'method={method}')
+            param_text = "\n".join(param_list)
+            axes[0].text(axes[0].get_xlim()[0] + (axes[0].get_xlim()[1] - axes[0].get_xlim()[0]) * 0.95,
+                        axes[0].get_ylim()[0] + (axes[0].get_ylim()[1] - axes[0].get_ylim()[0]) * 0.1,
                         param_text, verticalalignment='bottom', horizontalalignment='right')
```

### Comparing `seaborn-analyzer-0.2.9/seaborn_analyzer/custom_pair_plot.py` & `seaborn-analyzer-0.3.0/seaborn_analyzer/custom_pair_plot.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,259 +1,259 @@
-import seaborn as sns
-import numpy as np
-import pandas as pd
-import matplotlib.pyplot as plt
-from scipy import stats
-
-class CustomPairPlot():
-    #初期化
-    def __init__(self):
-        self.df = None
-        self.hue = None
-        self.hue_names = None
-        self.corr_mat = None
-    
-    #hueごとに相関係数計算
-    def _corrfunc(self, x, y, **kws):
-        if self.hue_names is None:
-            labelnum=0
-            hue_num = 0
-        else:
-            labelnum=self.hue_names.index(kws["label"])
-            hue_num = len(self.hue_names)
-        #xまたはyがNaNの行を除外
-        mask = ~np.logical_or(np.isnan(x), np.isnan(y))
-        x, y = x[mask], y[mask]
-        #相関係数算出＆0.4ごとにフォントサイズ拡大
-        r, _ = stats.pearsonr(x, y)
-        fsize = min(9, 45/hue_num) + min(4.5, 22.5/hue_num) * np.ceil(abs(r)/0.4)
-        fsize = min(9, 45/hue_num) if np.isnan(fsize) else fsize
-        #該当マスのaxを取得
-        if 'ax' in kws.keys():  # seaborn 0.11.1以降
-            ax = kws['ax']
-        else:  # seaborn 0.11.0以前
-            ax = plt.gca()
-        #既に表示したhueの分だけ下にさげて相関係数表示
-        ax.annotate("r={:.2f}".format(r), xy=(.1, .65-min(.15,.75/hue_num)*labelnum), xycoords=ax.transAxes, size=fsize, color=kws["color"])
-    
-    #hueを分けない相関係数計算して上半分に表示
-    def _corrall_upper(self, g):
-        #右上を1マスずつ走査
-        for i, j in zip(*np.triu_indices_from(g.axes, 1)):
-            #該当マスのaxesを取得
-            ax = g.axes[i, j]
-            plt.sca(ax)
-            #フィールド名を取得
-            x_var = g.x_vars[j]
-            y_var = g.y_vars[i]
-            #相関係数
-            r = self.corr_mat[x_var][y_var]
-            #相関係数0.2ごとにフォントサイズ拡大
-            fsize = 10 + 5 * np.ceil(abs(r)/0.2)
-            fsize = 10 if np.isnan(fsize) else fsize
-            #一番上に表示
-            ax.annotate("r={:.2f}".format(r), xy=(.1, .85), xycoords=ax.transAxes, size=fsize, color="black")
-
-    #重複数に応じたバブルチャート
-    def _duplicate_bubblescatter(self, data, x, y, hue=None, hue_names=None, hue_slide="horizontal", palette=None):
-        #hueの要素数および値を取得
-        if hue is not None:
-            #hue_nameを入力していないとき、hueの要素から自動生成
-            if hue_names is None:
-                hue_names = data[hue].dropna().unique()
-            hue_num = len(hue_names)
-            hue_vals = data[hue]
-        #hueを入力していないときも、groupby用にhue関係変数生成
-        else:
-            hue_names = ["_nolegend_"]
-            hue_num = 0
-            hue_vals = pd.Series(["_nolegend_"] * len(data),
-                                      index=data.index)
-        #hueで区切らない全データ数（NaNは除外）をカウント
-        ndata = len(data[[x,y]].dropna(how="any"))
-
-        ######hueごとにGroupByして表示処理######
-        hue_grouped = data.groupby(hue_vals)
-        for k, label_k in enumerate(hue_names):
-            try:
-                data_k = hue_grouped.get_group(label_k)
-            except KeyError:
-                data_k = pd.DataFrame(columns=data.columns,
-                                      dtype=np.float)
-            #X,Yごとに要素数をカウント
-            df_xy = data_k[[x,y]].copy()
-            df_xy["xyrec"] = 1
-            df_xycount = df_xy.dropna(how="any").groupby([x,y], as_index=False).count()
-            #hueが2個以上存在するとき、表示位置ずらし量（対象軸のユニーク値差分最小値÷4に収まるよう設定）を計算
-            if hue_num >=2:
-                if hue_slide == "horizontal":
-                    x_distinct_sort = sorted(data[x].dropna().unique())
-                    x_diff_min = min(np.diff(x_distinct_sort))
-                    x_offset = k * (x_diff_min/4)/(hue_num - 1) - x_diff_min/8
-                    y_offset = 0
-                else:
-                    y_distinct_sort = sorted(data[y].dropna().unique())
-                    y_diff_min = min(np.diff(y_distinct_sort))
-                    x_offset = 0
-                    y_offset = k * (y_diff_min/4)/(hue_num - 1) - y_diff_min/8
-            else:
-                x_offset = 0
-                y_offset = 0
-            #散布図表示（要素数をプロットサイズで表現）
-            ax = plt.gca()
-            ax.scatter(df_xycount[x] + x_offset, df_xycount[y] + y_offset, s=df_xycount["xyrec"]*1000/ndata, color=palette[k])
-
-    #plotter=scatterかつ要素数が2以下なら箱ひげ図、それ以外ならscatterplotを使用
-    def _boxscatter_lower(self, g, **kwargs):
-        #kw_color = kwargs.pop("color", None)
-        kw_color = g.palette
-        #左下を走査
-        for i, j in zip(*np.tril_indices_from(g.axes, -1)):
-            ax = g.axes[i, j]
-            plt.sca(ax)
-            #軸表示対象のフィールド名を取得
-            x_var = g.x_vars[j]
-            y_var = g.y_vars[i]
-            #XY軸データ抽出
-            x_data = self.df[x_var]
-            y_data = self.df[y_var]
-            #XY軸のユニーク値
-            x_distinct = x_data.dropna().unique()
-            y_distinct = y_data.dropna().unique()
-            
-            #箱ひげ図(x方向)
-            if len(x_distinct) ==2 and len(y_distinct) >= 5:
-                sns.boxplot(data=self.df, x=x_var, y=y_var, orient="v",
-                     hue=self.hue, palette=g.palette, **kwargs)
-            #重複数に応じたバブルチャート(x方向)
-            elif len(x_distinct) ==2 and len(y_distinct) < 5:
-                self._duplicate_bubblescatter(data=self.df, x=x_var, y=y_var, hue=self.hue, hue_names=g.hue_names, hue_slide="horizontal", palette=g.palette)
-            #箱ひげ図(y方向)
-            elif len(y_distinct) ==2 and len(x_distinct) >= 5:
-                sns.boxplot(data=self.df, x=x_var, y=y_var, orient="h",
-                     hue=self.hue, palette=g.palette, **kwargs)
-            #重複数に応じたバブルチャート(y方向)
-            elif len(y_distinct) ==2 and len(x_distinct) < 5:
-                self._duplicate_bubblescatter(data=self.df, x=x_var, y=y_var, hue=self.hue, hue_names=g.hue_names, hue_slide="vertical", palette=g.palette)
-            #散布図
-            else:
-                if len(g.hue_kws) > 0 and "marker" in g.hue_kws.keys():#マーカー指定あるとき
-                    markers = dict(zip(g.hue_names, g.hue_kws["marker"]))
-                else:#マーカー指定ないとき
-                    markers = True
-                sns.scatterplot(data=self.df, x=x_var, y=y_var, hue=self.hue,
-                     palette=g.palette, style=self.hue, markers=markers)
-            #凡例を追加
-            g._update_legend_data(ax)
-            ax.legend_ = None
-
-        if kw_color is not None:
-            kwargs["color"] = kw_color
-        #軸ラベルを追加
-        g._add_axis_labels()
-
-    #メイン関数
-    def pairanalyzer(self, df, hue=None, palette=None, vars=None,
-             lowerkind="boxscatter", diag_kind="kde", markers=None,
-             height=2.5, aspect=1, dropna=True,
-             lower_kws={}, diag_kws={}, grid_kws={}):
-        """
-        Plotting pair plot including scatter plot and correlation coefficient matrix simultaneously.
-        This method mainly uses seaborn.PairGrid class.
-
-        Parameters
-        ----------
-        df : pd.DataFrame
-            Input data structure. Int, float, and bool columns are displayed in the output graph.
-        hue : str
-            Variable in data to map plot aspects to different colors.
-        palette : str or dict[str]
-            Set of colors for mapping the hue variable. If a dict, keys should be values in the hue variable.
-        vars : list[str]
-            Variables within data to use, otherwise use every column with a numeric datatype.
-        lowerkind : {'boxscatter', 'scatter', or 'reg'}
-            Kind of plot for the lower triangular subplots.
-        diag_kind : {'kde' or 'hist'}
-            Kind of plot for the diagonal subplots.
-        markers : str or list[str]
-            Marker to use for all scatterplot points or a list of markers. See https://matplotlib.org/stable/api/markers_api.html
-        height : float
-            Height (in inches) of each facet.
-        aspect : float
-            Aspect * height gives the width (in inches) of each facet.
-        dropna : bool
-            Drop missing values from the data before plotting.
-        lower_kws : dict
-            Additional parameters passed to seaborn.PairGrid.map_lower(). If ``lowerkind`` is 'scatter', the arguments are applied to seaborn.scatterplot method of the lower subplots.
-        diag_kws : dict
-            Additional parameters passed to seaborn.PairGrid.map_diag(). If ``lowerkind`` is 'kde', the arguments are applied to seaborn.kdeplot method of the diagonal subplots.
-        grid_kws : dict
-            Additional parameters passed to seaborn.PairGrid.__init__() other than the above arguments. See https://seaborn.pydata.org/generated/seaborn.PairGrid.html
-        """
-        # bool型の列をintに変換
-        self.df = df.copy()
-        bool_cols = self.df.select_dtypes(include=bool).columns
-        for col in bool_cols:
-            self.df[col] = self.df[col] * 1
-        #メンバ変数入力
-        self.hue = hue
-        self.corr_mat = df.corr(method="pearson")
-        #文字サイズ調整
-        sns.set_context("notebook")
-
-        #PairGridインスタンス作成
-        plt.figure()
-        diag_sharey = diag_kind == "hist"
-        g = sns.PairGrid(self.df, hue=self.hue,
-                 palette=palette, vars=vars, diag_sharey=diag_sharey,
-                 height=height, aspect=aspect, dropna=dropna, size=None, **grid_kws)
-        self.hue_names = g.hue_names
-
-        #マーカーを設定
-        if markers is not None:
-            if g.hue_names is None:
-                n_markers = 1
-            else:
-                n_markers = len(g.hue_names)
-            if not isinstance(markers, list):
-                markers = [markers] * n_markers
-            if len(markers) != n_markers:
-                raise ValueError(("markers must be a singleton or a list of "
-                                "markers for each level of the hue variable"))
-            g.hue_kws = {"marker": markers}
-
-        #対角にヒストグラム or KDEをプロット
-        if diag_kind == "hist":
-            g.map_diag(plt.hist, **diag_kws)
-        elif diag_kind == "kde":
-            diag_kws.setdefault("shade", True)
-            diag_kws["legend"] = False
-            g.map_diag(sns.kdeplot, **diag_kws)
-
-        #各変数のユニーク数を計算
-        nuniques = []
-        for col_name in g.x_vars:
-            col_data = self.df[col_name]
-            nuniques.append(len(col_data.dropna().unique()))
-
-        #左下に散布図etc.をプロット
-        if lowerkind == "boxscatter":
-            if min(nuniques) <= 2: #ユニーク数が2の変数が存在するときのみ、箱ひげ表示
-                self._boxscatter_lower(g, **lower_kws)
-            else: #ユニーク数が2の変数が存在しないとき、散布図(_boxscatter_lowerを実行すると凡例マーカーが消えてしまう)
-                g.map_lower(sns.scatterplot, **lower_kws)
-        elif lowerkind == "scatter":
-            g.map_lower(sns.scatterplot, **lower_kws)
-        else:
-            g.map_lower(sns.regplot, **lower_kws)
-
-        #色分け（hue）有無で場合分けしてプロット＆相関係数表示実行
-        #hueなし
-        if self.hue is None:
-            #右上に相関係数表示
-            self._corrall_upper(g)
-        #hueあり
-        else:
-            #右上に相関係数表示(hueごとに色分け＆全体の相関係数を黒表示)
-            g.map_upper(self._corrfunc)
-            self._corrall_upper(g)
+import seaborn as sns
+import numpy as np
+import pandas as pd
+import matplotlib.pyplot as plt
+from scipy import stats
+
+class CustomPairPlot():
+    #初期化
+    def __init__(self):
+        self.df = None
+        self.hue = None
+        self.hue_names = None
+        self.corr_mat = None
+    
+    #hueごとに相関係数計算
+    def _corrfunc(self, x, y, **kws):
+        if self.hue_names is None:
+            labelnum=0
+            hue_num = 0
+        else:
+            labelnum=self.hue_names.index(kws["label"])
+            hue_num = len(self.hue_names)
+        #xまたはyがNaNの行を除外
+        mask = ~np.logical_or(np.isnan(x), np.isnan(y))
+        x, y = x[mask], y[mask]
+        #相関係数算出＆0.4ごとにフォントサイズ拡大
+        r, _ = stats.pearsonr(x, y)
+        fsize = min(9, 45/hue_num) + min(4.5, 22.5/hue_num) * np.ceil(abs(r)/0.4)
+        fsize = min(9, 45/hue_num) if np.isnan(fsize) else fsize
+        #該当マスのaxを取得
+        if 'ax' in kws.keys():  # seaborn 0.11.1以降
+            ax = kws['ax']
+        else:  # seaborn 0.11.0以前
+            ax = plt.gca()
+        #既に表示したhueの分だけ下にさげて相関係数表示
+        ax.annotate("r={:.2f}".format(r), xy=(.1, .65-min(.15,.75/hue_num)*labelnum), xycoords=ax.transAxes, size=fsize, color=kws["color"])
+    
+    #hueを分けない相関係数計算して上半分に表示
+    def _corrall_upper(self, g):
+        #右上を1マスずつ走査
+        for i, j in zip(*np.triu_indices_from(g.axes, 1)):
+            #該当マスのaxesを取得
+            ax = g.axes[i, j]
+            plt.sca(ax)
+            #フィールド名を取得
+            x_var = g.x_vars[j]
+            y_var = g.y_vars[i]
+            #相関係数
+            r = self.corr_mat[x_var][y_var]
+            #相関係数0.2ごとにフォントサイズ拡大
+            fsize = 10 + 5 * np.ceil(abs(r)/0.2)
+            fsize = 10 if np.isnan(fsize) else fsize
+            #一番上に表示
+            ax.annotate("r={:.2f}".format(r), xy=(.1, .85), xycoords=ax.transAxes, size=fsize, color="black")
+
+    #重複数に応じたバブルチャート
+    def _duplicate_bubblescatter(self, data, x, y, hue=None, hue_names=None, hue_slide="horizontal", palette=None):
+        #hueの要素数および値を取得
+        if hue is not None:
+            #hue_nameを入力していないとき、hueの要素から自動生成
+            if hue_names is None:
+                hue_names = data[hue].dropna().unique()
+            hue_num = len(hue_names)
+            hue_vals = data[hue]
+        #hueを入力していないときも、groupby用にhue関係変数生成
+        else:
+            hue_names = ["_nolegend_"]
+            hue_num = 0
+            hue_vals = pd.Series(["_nolegend_"] * len(data),
+                                      index=data.index)
+        #hueで区切らない全データ数（NaNは除外）をカウント
+        ndata = len(data[[x,y]].dropna(how="any"))
+
+        ######hueごとにGroupByして表示処理######
+        hue_grouped = data.groupby(hue_vals)
+        for k, label_k in enumerate(hue_names):
+            try:
+                data_k = hue_grouped.get_group(label_k)
+            except KeyError:
+                data_k = pd.DataFrame(columns=data.columns,
+                                      dtype=np.float)
+            #X,Yごとに要素数をカウント
+            df_xy = data_k[[x,y]].copy()
+            df_xy["xyrec"] = 1
+            df_xycount = df_xy.dropna(how="any").groupby([x,y], as_index=False).count()
+            #hueが2個以上存在するとき、表示位置ずらし量（対象軸のユニーク値差分最小値÷4に収まるよう設定）を計算
+            if hue_num >=2:
+                if hue_slide == "horizontal":
+                    x_distinct_sort = sorted(data[x].dropna().unique())
+                    x_diff_min = min(np.diff(x_distinct_sort))
+                    x_offset = k * (x_diff_min/4)/(hue_num - 1) - x_diff_min/8
+                    y_offset = 0
+                else:
+                    y_distinct_sort = sorted(data[y].dropna().unique())
+                    y_diff_min = min(np.diff(y_distinct_sort))
+                    x_offset = 0
+                    y_offset = k * (y_diff_min/4)/(hue_num - 1) - y_diff_min/8
+            else:
+                x_offset = 0
+                y_offset = 0
+            #散布図表示（要素数をプロットサイズで表現）
+            ax = plt.gca()
+            ax.scatter(df_xycount[x] + x_offset, df_xycount[y] + y_offset, s=df_xycount["xyrec"]*1000/ndata, color=palette[k])
+
+    #plotter=scatterかつ要素数が2以下なら箱ひげ図、それ以外ならscatterplotを使用
+    def _boxscatter_lower(self, g, **kwargs):
+        #kw_color = kwargs.pop("color", None)
+        kw_color = g.palette
+        #左下を走査
+        for i, j in zip(*np.tril_indices_from(g.axes, -1)):
+            ax = g.axes[i, j]
+            plt.sca(ax)
+            #軸表示対象のフィールド名を取得
+            x_var = g.x_vars[j]
+            y_var = g.y_vars[i]
+            #XY軸データ抽出
+            x_data = self.df[x_var]
+            y_data = self.df[y_var]
+            #XY軸のユニーク値
+            x_distinct = x_data.dropna().unique()
+            y_distinct = y_data.dropna().unique()
+            
+            #箱ひげ図(x方向)
+            if len(x_distinct) ==2 and len(y_distinct) >= 5:
+                sns.boxplot(data=self.df, x=x_var, y=y_var, orient="v",
+                     hue=self.hue, palette=g.palette, **kwargs)
+            #重複数に応じたバブルチャート(x方向)
+            elif len(x_distinct) ==2 and len(y_distinct) < 5:
+                self._duplicate_bubblescatter(data=self.df, x=x_var, y=y_var, hue=self.hue, hue_names=g.hue_names, hue_slide="horizontal", palette=g.palette)
+            #箱ひげ図(y方向)
+            elif len(y_distinct) ==2 and len(x_distinct) >= 5:
+                sns.boxplot(data=self.df, x=x_var, y=y_var, orient="h",
+                     hue=self.hue, palette=g.palette, **kwargs)
+            #重複数に応じたバブルチャート(y方向)
+            elif len(y_distinct) ==2 and len(x_distinct) < 5:
+                self._duplicate_bubblescatter(data=self.df, x=x_var, y=y_var, hue=self.hue, hue_names=g.hue_names, hue_slide="vertical", palette=g.palette)
+            #散布図
+            else:
+                if len(g.hue_kws) > 0 and "marker" in g.hue_kws.keys():#マーカー指定あるとき
+                    markers = dict(zip(g.hue_names, g.hue_kws["marker"]))
+                else:#マーカー指定ないとき
+                    markers = True
+                sns.scatterplot(data=self.df, x=x_var, y=y_var, hue=self.hue,
+                     palette=g.palette, style=self.hue, markers=markers)
+            #凡例を追加
+            g._update_legend_data(ax)
+            ax.legend_ = None
+
+        if kw_color is not None:
+            kwargs["color"] = kw_color
+        #軸ラベルを追加
+        g._add_axis_labels()
+
+    #メイン関数
+    def pairanalyzer(self, df, hue=None, palette=None, vars=None,
+             lowerkind="boxscatter", diag_kind="kde", markers=None,
+             height=2.5, aspect=1, dropna=True,
+             lower_kws={}, diag_kws={}, grid_kws={}):
+        """
+        Plotting pair plot including scatter plot and correlation coefficient matrix simultaneously.
+        This method mainly uses seaborn.PairGrid class.
+
+        Parameters
+        ----------
+        df : pd.DataFrame
+            Input data structure. Int, float, and bool columns are displayed in the output graph.
+        hue : str
+            Variable in data to map plot aspects to different colors.
+        palette : str or dict[str]
+            Set of colors for mapping the hue variable. If a dict, keys should be values in the hue variable.
+        vars : list[str]
+            Variables within data to use, otherwise use every column with a numeric datatype.
+        lowerkind : {'boxscatter', 'scatter', or 'reg'}
+            Kind of plot for the lower triangular subplots.
+        diag_kind : {'kde' or 'hist'}
+            Kind of plot for the diagonal subplots.
+        markers : str or list[str]
+            Marker to use for all scatterplot points or a list of markers. See https://matplotlib.org/stable/api/markers_api.html
+        height : float
+            Height (in inches) of each facet.
+        aspect : float
+            Aspect * height gives the width (in inches) of each facet.
+        dropna : bool
+            Drop missing values from the data before plotting.
+        lower_kws : dict
+            Additional parameters passed to seaborn.PairGrid.map_lower(). If ``lowerkind`` is 'scatter', the arguments are applied to seaborn.scatterplot method of the lower subplots.
+        diag_kws : dict
+            Additional parameters passed to seaborn.PairGrid.map_diag(). If ``lowerkind`` is 'kde', the arguments are applied to seaborn.kdeplot method of the diagonal subplots.
+        grid_kws : dict
+            Additional parameters passed to seaborn.PairGrid.__init__() other than the above arguments. See https://seaborn.pydata.org/generated/seaborn.PairGrid.html
+        """
+        # bool型の列をintに変換
+        self.df = df.copy()
+        bool_cols = self.df.select_dtypes(include=bool).columns
+        for col in bool_cols:
+            self.df[col] = self.df[col] * 1
+        #メンバ変数入力
+        self.hue = hue
+        self.corr_mat = df.corr(method="pearson")
+        #文字サイズ調整
+        sns.set_context("notebook")
+
+        #PairGridインスタンス作成
+        plt.figure()
+        diag_sharey = diag_kind == "hist"
+        g = sns.PairGrid(self.df, hue=self.hue,
+                 palette=palette, vars=vars, diag_sharey=diag_sharey,
+                 height=height, aspect=aspect, dropna=dropna, size=None, **grid_kws)
+        self.hue_names = g.hue_names
+
+        #マーカーを設定
+        if markers is not None:
+            if g.hue_names is None:
+                n_markers = 1
+            else:
+                n_markers = len(g.hue_names)
+            if not isinstance(markers, list):
+                markers = [markers] * n_markers
+            if len(markers) != n_markers:
+                raise ValueError(("markers must be a singleton or a list of "
+                                "markers for each level of the hue variable"))
+            g.hue_kws = {"marker": markers}
+
+        #対角にヒストグラム or KDEをプロット
+        if diag_kind == "hist":
+            g.map_diag(plt.hist, **diag_kws)
+        elif diag_kind == "kde":
+            diag_kws.setdefault("shade", True)
+            diag_kws["legend"] = False
+            g.map_diag(sns.kdeplot, **diag_kws)
+
+        #各変数のユニーク数を計算
+        nuniques = []
+        for col_name in g.x_vars:
+            col_data = self.df[col_name]
+            nuniques.append(len(col_data.dropna().unique()))
+
+        #左下に散布図etc.をプロット
+        if lowerkind == "boxscatter":
+            if min(nuniques) <= 2: #ユニーク数が2の変数が存在するときのみ、箱ひげ表示
+                self._boxscatter_lower(g, **lower_kws)
+            else: #ユニーク数が2の変数が存在しないとき、散布図(_boxscatter_lowerを実行すると凡例マーカーが消えてしまう)
+                g.map_lower(sns.scatterplot, **lower_kws)
+        elif lowerkind == "scatter":
+            g.map_lower(sns.scatterplot, **lower_kws)
+        else:
+            g.map_lower(sns.regplot, **lower_kws)
+
+        #色分け（hue）有無で場合分けしてプロット＆相関係数表示実行
+        #hueなし
+        if self.hue is None:
+            #右上に相関係数表示
+            self._corrall_upper(g)
+        #hueあり
+        else:
+            #右上に相関係数表示(hueごとに色分け＆全体の相関係数を黒表示)
+            g.map_upper(self._corrfunc)
+            self._corrall_upper(g)
             g.add_legend()
```

### Comparing `seaborn-analyzer-0.2.9/seaborn_analyzer/custom_reg_plot.py` & `seaborn-analyzer-0.3.0/seaborn_analyzer/custom_reg_plot.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,1766 +1,1766 @@
-from typing import List, Dict
-import seaborn as sns
-import matplotlib.pyplot as plt
-import numbers
-import numpy as np
-import pandas as pd
-from scipy import stats
-from sklearn.linear_model import LinearRegression
-from sklearn.metrics import r2_score, mean_absolute_error, mean_squared_error, mean_squared_log_error, mean_absolute_percentage_error
-from sklearn.model_selection import KFold, LeaveOneOut, GroupKFold, LeaveOneGroupOut
-import decimal
-
-from ._cv_eval_set import init_eval_set, _make_transformer, _eval_set_selection, cross_val_score_eval_set
-
-class regplot():
-    # regression_heat_plotメソッド (回帰モデルヒートマップ表示)における、散布図カラーマップ
-    _HEAT_SCATTER_HUECOLORS = ['red', 'mediumblue', 'darkorange', 'darkmagenta', 'cyan',  'pink', 'brown', 'gold', 'grey']
-
-    def _round_digits(src: float, rounddigit: int = None, method='decimal'):
-        """
-        指定桁数で小数を丸める
-
-        Parameters
-        ----------
-        src : float
-            丸め対象の数値
-        rounddigit : int
-            フィッティング線の表示範囲（標準偏差の何倍まで表示するか指定）
-        method : int
-            桁数決定手法（'decimal':小数点以下, 'sig':有効数字(Decimal指定), 'format':formatで有効桁数指定）
-        """
-        if method == 'decimal':
-            return round(src, rounddigit)
-        elif method == 'sig':
-            with decimal.localcontext() as ctx:
-                ctx.prec = rounddigit
-                return ctx.create_decimal(src)
-        elif method == 'format':
-            return '{:.{width}g}'.format(src, width=rounddigit)
-    
-    @classmethod
-    def _round_dict_digits(cls, srcdict: Dict[str, float], rounddigit: int = None, method='decimal'):
-        """
-        指定桁数でdictの値を丸める
-
-        Parameters
-        ----------
-        srcdict : dict[str, float]
-            丸め対象のdict
-        rounddigit : int
-            フィッティング線の表示範囲（標準偏差の何倍まで表示するか指定）
-        method : int
-            桁数決定手法（'decimal':小数点以下, 'sig':有効数字(Decimal指定), 'format':formatで有効桁数指定）
-        """
-        dstdict = {}
-        for k, v in srcdict.items():
-            if rounddigit is not None and isinstance(v, float):
-                dstdict[k] = cls._round_digits(v, rounddigit=rounddigit, method=method)
-            else:
-                dstdict[k] = v
-        return dstdict
-
-    def _make_score_dict(y_true, y_pred, scores):
-        """
-        回帰評価指標を算出してdict化
-        """
-        score_dict = {}
-        for scoring in scores:
-            if scoring == 'r2':
-                score_dict['r2'] = r2_score(y_true, y_pred)
-            elif scoring == 'mae':
-                score_dict['mae'] = mean_absolute_error(y_true, y_pred)
-            elif scoring == 'mse':
-                score_dict['mse'] = mean_squared_error(y_true, y_pred, squared=True)
-            elif scoring == 'rmse':
-                score_dict['rmse'] = mean_squared_error(y_true, y_pred, squared=False)
-            elif scoring == 'rmsle':
-                score_dict['rmsle'] = mean_squared_log_error(y_true, y_pred)
-            elif scoring == 'mape':
-                score_dict['mape'] = mean_absolute_percentage_error(y_true, y_pred)
-            elif scoring == 'max_error':
-                score_dict['max_error'] = max([abs(p - r) for r, p in zip(y_true, y_pred)])
-        return score_dict
-
-    def _reshape_input_data(x, y, data, x_colnames, cv_group):
-        """
-        入力データの形式統一(pd.DataFrame or np.ndarray)
-        """
-        # dataがpd.DataFrameのとき
-        if isinstance(data, pd.DataFrame):
-            if not isinstance(x, list):
-                raise Exception('`x` argument should be list[str] if `data` is pd.DataFrame')
-            if not isinstance(y, str):
-                raise Exception('`y` argument should be str if `data` is pd.DataFrame')
-            if x_colnames is not None:
-                raise Exception('`x_colnames` argument should be None if `data` is pd.DataFrame')
-            X = data[x].values
-            y_true = data[y].values
-            x_colnames = x
-            y_colname = y
-            cv_group_colname = cv_group
-            
-        # dataがNoneのとき(x, y, cv_groupがnp.ndarray)
-        elif data is None:
-            if not isinstance(x, np.ndarray):
-                raise Exception('`x` argument should be np.ndarray if `data` is None')
-            if not isinstance(y, np.ndarray):
-                raise Exception('`y` argument should be np.ndarray if `data` is None')
-            X = x if len(x.shape) == 2 else x.reshape([x.shape[0], 1])
-            y_true = y.ravel()
-            # x_colnameとXの整合性確認
-            if x_colnames is None:
-                x_colnames = list(range(X.shape[1]))
-            elif X.shape[1] != len(x_colnames):
-                raise Exception('width of X must be equal to length of x_colnames')
-            else:
-                x_colnames = x_colnames
-            y_colname = 'objective_variable'
-            if cv_group is not None:  # cv_group指定時
-                cv_group_colname = 'group'
-                data = pd.DataFrame(np.column_stack((X, y_true, cv_group)),
-                                    columns=x_colnames + [y_colname] + [cv_group_colname])
-            else:
-                cv_group_colname = None
-                data = pd.DataFrame(np.column_stack((X, y)),
-                                    columns=x_colnames + [y_colname])
-        else:
-            raise Exception('`data` argument should be pd.DataFrame or None')
-
-        return X, y_true, data, x_colnames, y_colname, cv_group_colname
-
-    @classmethod
-    def _rank_display(cls, y_true, y_pred, rank_number, rank_col, rank_col_data, x=None, ax=None, rounddigit=None):
-        """
-        誤差上位を文字プロット
-
-        Parameters
-        ----------
-        y_true : np.ndarray
-            目的変数実測値
-        y_pred : np.ndarray
-            目的変数予測値
-        rank_number : int
-            誤差上位何番目までを文字表示するか
-        rank_col : List[str]
-            誤差上位と一緒に表示するフィールド名 (NoneならIndexを使用)
-        x : np.ndarray
-            説明変数の値 (Noneなら横軸y_true縦軸y_pred、Noneでなければ横軸x縦軸y_true)
-        ax : matplotlib.axes.Axes
-            表示対象のax（Noneならmatplotlib.pyplot.plotで1枚ごとにプロット）
-        rounddigit: int
-            表示指標の小数丸め桁数
-        """
-        # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
-        if ax is None:
-            ax=plt.gca()
-
-        if rank_col is None:
-            rank_col = 'index'
-        y_error = y_pred - y_true
-        y_error_abs = np.abs(y_error)
-        rank_index  = np.argsort(-y_error_abs)[:rank_number]
-        for rank, i in enumerate(rank_index):
-            error = cls._round_digits(y_error[i], rounddigit=rounddigit, method='decimal')
-            rank_text = f'      no{rank+1}\n-<-error={error}\n      {rank_col}={rank_col_data[i]}'
-            if x is None:  # 横軸y_true縦軸y_pred (regression_pred_trueメソッド用)
-                ax.text(y_true[i], y_pred[i], rank_text, verticalalignment='center', horizontalalignment='left')
-            else:  # 横軸x縦軸y_true (regression_plot_1dメソッド用)
-                ax.text(x[i], y_true[i], rank_text, verticalalignment='center', horizontalalignment='left')
-    
-    @classmethod
-    def _scatterplot_ndarray(cls, x, x_name, y, y_name, hue_data, hue_name, ax, scatter_kws, legend_kws):
-        """
-        np.ndarrayを入力として散布図表示(scatterplot)
-        """
-        # X値とY値を合体してDataFrame化
-        data = np.stack([x, y], axis=1)
-        data = pd.DataFrame(data, columns=[x_name, y_name])
-        # 色分け指定しているとき、色分け用のフィールドを追加
-        if hue_data is not None:
-            if hue_name is None:
-                hue_name = 'hue'
-            data[hue_name] = pd.Series(hue_data)
-        # 散布図プロット
-        sns.scatterplot(x=x_name, y=y_name, data=data, ax=ax, hue=hue_name, **scatter_kws)
-        # 凡例追加
-        if 'title' not in legend_kws.keys():
-            legend_kws['title'] = hue_name 
-        ax.legend(**legend_kws)
-
-    @classmethod
-    def _plot_pred_true(cls, y_true, y_pred, hue_data=None, hue_name=None, ax=None,
-                        linecolor='red', linesplit=200, rounddigit=None,
-                        score_dict=None, scatter_kws=None, legend_kws=None):
-        """
-        予測値と実測値を、回帰評価指標とともにプロット
-
-        Parameters
-        ----------
-        y_true : ndarray
-            目的変数実測値
-        y_pred : ndarray
-            目的変数予測値
-        hue_data : ndarray
-            色分け用ラベルデータ
-        hue_name : str
-            色分け用の列名
-        ax : matplotlib.axes.Axes
-            表示対象のax (Noneならmatplotlib.pyplot.plotで1枚ごとにプロット)
-        linecolor : str
-            予測値=実測値の線の色
-        linesplit : int
-            フィッティング線の分割数 (カクカクしたら増やす)
-        rounddigit: int
-            表示指標の小数丸め桁数
-        score_dict : dict[str, float]
-            算出した評価指標一覧
-        scatter_kws : dict
-            Additional parameters passed to sns.scatterplot(), e.g. ``alpha``. See https://seaborn.pydata.org/generated/seaborn.scatterplot.html
-        legend_kws : dict
-            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
-        """
-        # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
-        if ax is None:
-            ax=plt.gca()
-        # score_dictがNoneのとき、空のDictを加瀬宇
-        if score_dict is None:
-            score_dict = {}
-        # scatter_kwsがNoneなら空のdictを入力
-        if scatter_kws is None:
-            scatter_kws = {}
-        
-        # 散布図プロット
-        cls._scatterplot_ndarray(y_true, 'y_true', y_pred, 'y_pred', hue_data, hue_name, ax, scatter_kws, legend_kws)
-
-        # 予測値=実測値の線を作成
-        true_min = np.amin(y_true)
-        true_max = np.amax(y_true)
-        true_line = np.linspace(true_min, true_max, linesplit)
-        # 評価指標文字列作成
-        score_list = [f'{k}={v}' for k, v in cls._round_dict_digits(score_dict, rounddigit, 'sig').items()]
-        score_text = "\n".join(score_list)
-        # 線と文字をプロット
-        ax.plot(true_line, true_line, color=linecolor)
-        ax.text(true_max, np.amin(y_pred), score_text, verticalalignment='bottom', horizontalalignment='right')
-    
-    @classmethod
-    def regression_pred_true(cls, estimator, x: List[str], y: str, data: pd.DataFrame = None,
-                             x_colnames: List[str] = None, hue=None, linecolor='red', rounddigit=3,
-                             rank_number=None, rank_col=None, scores='mae', 
-                             cv_stats='mean', cv=None, cv_seed=42, cv_group=None, ax=None,
-                             estimator_params=None, fit_params=None, eval_set_selection=None,
-                             subplot_kws=None, scatter_kws=None, legend_kws=None):
-
-        """
-        Plot prediction vs. true scatter plots of any scikit-learn regression estimator
-
-        Parameters
-        ----------
-        estimator : estimator object implementing ``fit``
-            Regression estimator. This is assumed to implement the scikit-learn estimator interface.
-
-        x : str or list[str]
-            Explanatory variables.
-
-        y : str
-            Objective variable.
-
-        data : pd.DataFrame
-            Input data structure.
-
-        x_colnames: list[str], optional
-            Names of explanatory variables. Available only if ``data`` is NOT pd.DataFrame
-
-        hue : str, optional
-            Grouping variable that will produce points with different colors.
-
-        linecolor : str, optional
-            Color of prediction = true line. See https://matplotlib.org/stable/gallery/color/named_colors.html
-
-        rounddigit: int, optional
-            Round a number of score to a given precision in decimal digits.
-
-        rank_number : int, optional
-            Number of emphasized data that are in the top posiotions for regression error.
-
-        rank_col : list[str], optional
-            Variables that are displayed with emphasized data that are in the top posiotions for regression error.
-
-        scores : {'r2', 'mae', 'mse', 'rmse', 'rmsle', 'mape', 'max_error'} or list, optional
-            Regression score that are displayed at the lower right of the graph.
-
-        cv_stats : {'mean', 'median', 'max', 'min'}, optional
-            Statistical method of cross validation score that are displayed at the lower right of the graph.
-
-        cv : int, cross-validation generator, or an iterable, optional
-            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
-
-        cv_seed : int, optional
-            Seed for random number generator of cross validation.
-
-        cv_group: str, optional
-            Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
-
-        ax : {matplotlib.axes.Axes, list[matplotlib.axes.Axes]}, optional
-            Pre-existing axes for the plot or list of it. Otherwise, call matplotlib.pyplot.subplot() internally.
-
-        estimator_params : dict, optional
-            Parameters passed to the regression estimator. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
-
-        fit_params : dict, optional
-            Parameters passed to the fit() method of the regression estimator, e.g. ``early_stopping_round`` and ``eval_set`` of XGBRegressor. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
-
-        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            Select data passed to `eval_set` in `fit_params`. Available only if `estimator` is LightGBM or XGBoost and `cv` is not None.
-            
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
-
-            If "test", select test data from `X` and `y` using cv.split().
-
-            If "original", use raw `eval_set`.
-
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
-
-        subplot_kws : dict, optional
-            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. figsize. Available only if ``axes`` is None. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
-
-        scatter_kws: dict, optional
-            Additional parameters passed to sns.scatterplot(), e.g. ``alpha``. See https://seaborn.pydata.org/generated/seaborn.scatterplot.html
-
-        legend_kws : dict
-            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
-
-        Returns
-        ----------
-        score_dict : dict
-            Validation scores, e.g. r2, mae and rmse
-        """
-
-        # 入力データの形式統一
-        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data([x] if isinstance(x, str) else x, 
-                                                                                           y, data,
-                                                                                           x_colnames,
-                                                                                           cv_group)
-        # scoresの型をListに統一
-        if scores is None:
-            scores = []
-        elif isinstance(scores, str):
-            scores = [scores]
-        elif not isinstance(scores, list):
-            raise Exception('the "scores" argument must be str or list[str]')
-        # 学習器パラメータがあれば適用
-        if estimator_params is not None:
-            estimator.set_params(**estimator_params)
-        # 学習時パラメータがNoneなら空のdictを入力
-        if fit_params is None:
-            fit_params = {}
-        # subplot_kwsがNoneなら空のdictを入力
-        if subplot_kws is None:
-            subplot_kws = {}
-        # scatter_kwsがNoneなら空のdictを入力
-        if scatter_kws is None:
-            scatter_kws = {}
-        # legend_kwsがNoneなら空のdictを入力
-        if legend_kws is None:
-            legend_kws = {}
-        
-        # クロスバリデーション有無で場合分け
-        # クロスバリデーション未実施時(学習データからプロット＆指標算出)
-        if cv is None:
-            # 学習と推論
-            estimator.fit(X, y_true, **fit_params)
-            y_pred = estimator.predict(X)
-            # 評価指標算出
-            score_dict = cls._make_score_dict(y_true, y_pred, scores)
-            # 色分け用データ取得
-            hue_data = None if hue is None else data[hue]
-            hue_name = None if hue is None else hue
-            # 誤差上位表示用データ取得
-            if rank_number is not None:
-                if rank_col is None:  # 表示フィールド指定ないとき、Index使用
-                    rank_col_data = data.index.values
-                else:  # 表示フィールド指定あるとき
-                    rank_col_data = data[rank_col].values
-            # 予測値と実測値プロット
-            cls._plot_pred_true(y_true, y_pred, hue_data=hue_data, hue_name=hue_name, ax=ax,
-                                linecolor=linecolor, rounddigit=rounddigit, score_dict=score_dict,
-                                scatter_kws=scatter_kws, legend_kws=legend_kws)
-            # 誤差上位を文字表示
-            if rank_number is not None:
-                cls._rank_display(y_true, y_pred, rank_number, rank_col, rank_col_data, rounddigit=rounddigit)
-            return score_dict
-            
-        # クロスバリデーション実施時(分割ごとに別々にプロット＆指標算出)
-        if cv is not None:
-            # 分割法未指定時、cv_numとseedに基づきKFoldでランダムに分割
-            if isinstance(cv, numbers.Integral):
-                cv = KFold(n_splits=cv, shuffle=True, random_state=cv_seed)
-            #LeaveOneOutかどうかを判定
-            isLeaveOneOut = isinstance(cv, LeaveOneOut)
-            # cv_groupをグルーピング対象に指定(GroupKFold、LeaveOneGroupOut等)
-            split_kws={}
-            if cv_group_colname is not None:
-                split_kws['groups'] = data[cv_group_colname].values
-            elif isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
-                raise Exception('"GroupKFold" and "LeaveOneGroupOut" cross validations need ``cv_group`` argument')
-            # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
-            if isinstance(cv, LeaveOneGroupOut):
-                cv_num = len(set(data[cv_group_colname].values))
-            elif isLeaveOneOut:
-                cv_num = 1
-            else:
-                cv_num = cv.n_splits
-
-            # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
-            if eval_set_selection is None:
-                eval_set_selection = 'test'
-            fit_params, eval_set_selection = init_eval_set(
-                    eval_set_selection, fit_params, X, y)
-            # 最終学習器以外の前処理変換器作成
-            transformer = _make_transformer(eval_set_selection, estimator)
-
-            # スコア種類ごとにクロスバリデーションスコアの算出
-            score_all_dict = {}
-            for scoring in scores:
-                # cross_val_scoreでクロスバリデーション
-                if scoring == 'r2':
-                    score_all_dict['r2'] = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
-                                                    cv=cv, scoring='r2',
-                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
-                elif scoring == 'mae':
-                    neg_mae = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
-                                                    cv=cv, scoring='neg_mean_absolute_error',
-                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
-                    score_all_dict['mae'] = -neg_mae  # scikit-learnの仕様に合わせ正負を逆に
-                elif scoring == 'mse':
-                    neg_mse = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
-                                                    cv=cv, scoring='neg_mean_squared_error',
-                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
-                    score_all_dict['mse'] = -neg_mse  # scikit-learnの仕様に合わせ正負を逆に
-                elif scoring == 'rmse':
-                    neg_rmse = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
-                                                    cv=cv, scoring='neg_root_mean_squared_error',
-                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
-                    score_all_dict['rmse'] = -neg_rmse  # scikit-learnの仕様に合わせ正負を逆に
-                elif scoring == 'rmsle':
-                    neg_msle = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true, 
-                                                    cv=cv, scoring='neg_mean_squared_log_error',
-                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
-                    score_all_dict['rmsle'] = np.sqrt(-neg_msle)  # 正負を逆にしてルートをとる
-                elif scoring == 'mape':
-                    neg_mape = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
-                                                    cv=cv, scoring='neg_mean_absolute_percentage_error',
-                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
-                    score_all_dict['mape'] = -neg_mape  # scikit-learnの仕様に合わせ正負を逆に
-                elif scoring == 'max_error':
-                    neg_max_error = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
-                                                    cv=cv, scoring='max_error',
-                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
-                    score_all_dict['max_error'] = - neg_max_error  # scikit-learnの仕様に合わせ正負を逆に
-            
-            # 表示用のax作成
-            if ax is None:
-                # LeaveOneOutのとき、クロスバリデーションごとの図は作成せず
-                if isLeaveOneOut:
-                    if 'figsize' not in subplot_kws.keys():
-                        subplot_kws['figsize'] = (6, 6)
-                    fig, ax = plt.subplots(1, 1, **subplot_kws)
-                # LeaveOneOut以外のとき、クロスバリデーションごとに図作成
-                else:
-                    if 'figsize' not in subplot_kws.keys():
-                        subplot_kws['figsize'] = (6, (cv_num + 1) * 6)
-                    fig, ax = plt.subplots(cv_num + 1, 1, **subplot_kws)
-
-            # クロスバリデーション
-            y_true_all = []
-            y_pred_all = []
-            hue_all = []
-            rank_col_all = []
-            score_train_dict = {}
-            for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
-                # 表示用にテストデータと学習データ分割
-                X_train = X[train]
-                y_train = y_true[train]
-                X_test = X[test]
-                y_test = y_true[test]
-                # 色分け用データ取得(していないときは、クロスバリデーション番号を使用、LeaveOuneOutのときは番号分けない)
-                if hue is None:
-                    hue_test = np.full(1 ,'leave_one_out') if isLeaveOneOut else np.full(len(test) ,f'cv_{i}')
-                    hue_name = 'cv_number'  # 色分け名を'cv_number'に指定
-                else:
-                    hue_test = data[hue].values[test]
-                    hue_name = hue
-                # 誤差上位表示用データ取得
-                if rank_number is not None:
-                    if rank_col is None:  # 表示フィールド指定ないとき、Index使用
-                        rank_col_test = data.index.values[test]
-                    else:  # 表示フィールド指定あるとき
-                        rank_col_test = data[rank_col].values[test]
-                else:
-                    rank_col_test = np.array([])
-
-                # eval_setの中から学習データ or テストデータのみを抽出
-                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
-                                                        fit_params, train, test)
-
-                # 学習と推論
-                estimator.fit(X_train, y_train, **fit_params_modified)
-                y_pred = estimator.predict(X_test)
-                # 学習データスコア算出
-                y_pred_train = estimator.predict(X_train)
-                score_dict = cls._make_score_dict(y_train, y_pred_train, scores)
-                for score in scores:
-                    if f'{score}_train' not in score_train_dict:
-                        score_train_dict[f'{score}_train'] = []
-                    score_train_dict[f'{score}_train'].append(score_dict[score])
-                # CV内結果をプロット(LeaveOneOutのときはプロットしない)
-                if not isLeaveOneOut:
-                    score_cv_dict = {k: v[i] for k, v in score_all_dict.items()}
-                    score_cv_dict.update({f'{k}_train': v for k, v in score_dict.items()})
-                    cls._plot_pred_true(y_test, y_pred, hue_data=hue_test, hue_name=hue_name, ax=ax[i],
-                                        linecolor=linecolor, rounddigit=rounddigit, score_dict=score_cv_dict,
-                                        scatter_kws=scatter_kws, legend_kws=legend_kws)
-                    ax[i].set_title(f'Cross Validation Fold{i}')
-                # 全体プロット用データに追加
-                y_true_all.append(y_test)
-                y_pred_all.append(y_pred)
-                hue_all.append(hue_test)
-                rank_col_all.append(rank_col_test)
-
-            # 全体プロット用データを合体
-            y_true_all = np.hstack(y_true_all)
-            y_pred_all = np.hstack(y_pred_all)
-            hue_all = np.hstack(hue_all)
-            rank_col_all = np.hstack(rank_col_all)
-            # スコアの統計値を計算
-            if cv_stats == 'mean':
-                score_stats_dict = {f'{k}_mean': np.mean(v) for k, v in score_all_dict.items()}
-                train_stats_dict = {k: np.mean(v) for k, v in score_train_dict.items()}
-            elif cv_stats == 'median':
-                score_stats_dict = {f'{k}_median': np.median(v) for k, v in score_all_dict.items()}
-                train_stats_dict = {k: np.median(v) for k, v in score_train_dict.items()}
-            elif cv_stats == 'min':
-                score_stats_dict = {f'{k}_min': np.amin(v) for k, v in score_all_dict.items()}
-                train_stats_dict = {k: np.amin(v) for k, v in score_train_dict.items()}
-            elif cv_stats == 'max':
-                score_stats_dict = {f'{k}_max': np.amax(v) for k, v in score_all_dict.items()}
-                train_stats_dict = {k: np.amax(v) for k, v in score_train_dict.items()}
-            # 学習データスコアをdictに追加
-            score_stats_dict.update(train_stats_dict)
-            # 全体プロット
-            ax_all = ax if isLeaveOneOut else ax[cv_num]
-            cls._plot_pred_true(y_true_all, y_pred_all, hue_data=hue_all, hue_name=hue_name, ax=ax_all,
-                               linecolor=linecolor, rounddigit=rounddigit, score_dict=score_stats_dict,
-                               scatter_kws=scatter_kws, legend_kws=legend_kws)
-            ax_all.set_title('All Cross Validations')
-            # 誤差上位を文字表示
-            if rank_number is not None:
-                cls._rank_display(y_true_all, y_pred_all, rank_number, rank_col, rank_col_all,
-                                  ax=ax_all, rounddigit=rounddigit)
-            return score_stats_dict
-    
-    def _average_plot(estimator, data, x_colnames, y_colname, hue,
-                      aggregate, subplot_kws, plot_kws, scatter_kws, legend_kws,
-                      cv_index, x_range=200):
-        # figsize (全ての図全体のサイズ)指定
-        if 'figsize' not in subplot_kws.keys():
-            subplot_kws['figsize'] = (6, len(x_colnames) * 5)
-        if 'color' not in plot_kws:
-            plot_kws['color'] = 'red'
-        # プロット用のaxes作成
-        fig, axes = plt.subplots(len(x_colnames), 1, **subplot_kws)
-        if cv_index is not None:
-            fig.suptitle(f'CV No.{cv_index}')
-        # 全列を走査
-        for i, colname in enumerate(x_colnames):
-            # 該当列（グラフのX軸）の値を作成
-            x_max = data[colname].max()
-            x_min = data[colname].min()
-            x_array = np.linspace(x_min, x_max, x_range)
-            # 該当列以外を抽出して平均値算出
-            if aggregate == 'mean':
-                other_x_agg = data[[col for col in x_colnames if col != colname]].mean()
-            elif aggregate == 'median':
-                other_x_agg = data[[col for col in x_colnames if col != colname]].median()
-            else:
-                raise ValueError('the `aggregate` argument should be "mean" or "median"')
-            X_mean = np.tile(other_x_agg, (x_range, 1))
-            # 該当列を挿入して説明変数とし、モデルで推論
-            X_mean = np.insert(X_mean, i, x_array, axis=1)
-            y_pred = estimator.predict(X_mean)
-            # 実測値を散布図プロット
-            ax = axes if len(x_colnames) == 1 else axes[i]
-            sns.scatterplot(x=colname, y=y_colname, hue=hue, data=data, ax=ax, **scatter_kws)
-            # 推測値曲線をプロット
-            ax.plot(x_array, y_pred, **plot_kws)
-            # 色分け時は凡例表示
-            if hue is not None:
-                ax.legend(**legend_kws)
-
-        fig.tight_layout(rect=[0, 0, 1, 0.98])          
-
-
-    @classmethod
-    def average_plot(cls, estimator, x: List[str], y: str, data: pd.DataFrame = None,
-                     x_colnames: List[str] = None, hue=None,
-                     aggregate='mean',
-                     cv=None, cv_seed=42, cv_group=None, display_cv_indices = 0,
-                     estimator_params=None, fit_params=None, eval_set_selection=None,
-                     subplot_kws=None, plot_kws=None, scatter_kws=None, legend_kws=None):
-        """
-        Plot relationship between one explanatory variable and predicted value by line graph.
-
-        Other explanatory variables are fixed to aggregated values such as mean values or median values.
-
-        Parameters
-        ----------
-        estimator : estimator object implementing ``fit``
-            Regression estimator. This is assumed to implement the scikit-learn estimator interface.
-        x : list[str] or np.ndarray
-            Explanatory variables. Should be list[str] if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
-
-        y : str or np.ndarray
-            Objective variable. Should be str if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
-
-        data: pd.DataFrame
-            Input data structure.
-
-        x_colnames: list[str], optional
-            Names of explanatory variables. Available only if ``data`` is NOT pd.DataFrame
-
-        hue : str, optional
-            Grouping variable that will produce points with different colors.
-
-        aggregate : {'mean', 'median'}, optional
-            Statistic method of aggregating explanatory variables except x_axis variable.
-
-        cv : int, cross-validation generator, or an iterable, optional
-            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
-
-        cv_seed : int, optional
-            Seed for random number generator of cross validation.
-
-        cv_group: str, optional
-            Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
-
-        display_cv_indices : int or list, optional
-            Cross validation index or indices to display.
-
-        estimator_params : dict, optional
-            Parameters passed to the regression estimator. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
-
-        fit_params : dict, optional
-            Parameters passed to the fit() method of the regression estimator, e.g. ``early_stopping_round`` and ``eval_set`` of XGBRegressor. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
-        
-        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            Select data passed to `eval_set` in `fit_params`. Available only if `estimator` is LightGBM or XGBoost and `cv` is not None.
-            
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
-
-            If "test", select test data from `X` and `y` using cv.split().
-
-            If "original", use raw `eval_set`.
-
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
-
-        subplot_kws: dict, optional
-            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
-
-        plot_kws: dict, optional
-            Additional parameters passed to matplotlib.axes.Axes.plot(), e.g. ``alpha``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.plot.html
-
-        scatter_kws: dict, optional
-            Additional parameters passed to seaborn.scatterplot(), e.g. ``alpha``. See https://seaborn.pydata.org/generated/seaborn.scatterplot.html
-
-        legend_kws : dict
-            Additional parameters passed to matplotlib.axes.Axes.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
-        """
-
-        # 入力データの形式統一
-        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data(x, y, data,
-                                                                                           x_colnames,
-                                                                                           cv_group)
-        
-        # display_cv_indicesをList化
-        if isinstance(display_cv_indices, int):
-            display_cv_indices = [display_cv_indices]
-        elif not isinstance(x_colnames, list):
-            raise Exception('the "cv_display_indices" argument should be int or List[int]')
-        # 学習器パラメータがあれば適用
-        if estimator_params is not None:
-            estimator.set_params(**estimator_params)
-        # 学習時パラメータがNoneなら空のdictを入力
-        if fit_params is None:
-            fit_params = {}
-        # subplot_kwsがNoneなら空のdictを入力
-        if subplot_kws is None:
-            subplot_kws = {}
-        # plot_kwsがNoneなら空のdictを入力
-        if plot_kws is None:
-            plot_kws = {}
-        # scatter_kwsがNoneなら空のdictを入力
-        if scatter_kws is None:
-            scatter_kws = {}
-        # legend_kwsがNoneなら空のdictを入力
-        if legend_kws is None:
-            legend_kws = {}
-        
-        # クロスバリデーション有無で場合分け
-        # クロスバリデーション未実施時(学習データからプロット＆指標算出)
-        if cv is None:
-            # 学習と推論
-            estimator.fit(X, y_true, **fit_params)
-            # 平均値
-            cls._average_plot(estimator, data, x_colnames, y_colname, hue,
-                              aggregate=aggregate,
-                              subplot_kws=subplot_kws, plot_kws=plot_kws,
-                              scatter_kws=scatter_kws, legend_kws=legend_kws,
-                              cv_index=None)
-            
-        # クロスバリデーション実施時(分割ごとに別々にプロット＆指標算出)
-        if cv is not None:
-            # 分割法未指定時、cv_numとseedに基づきKFoldでランダムに分割
-            if isinstance(cv, numbers.Integral):
-                cv = KFold(n_splits=cv, shuffle=True, random_state=cv_seed)
-            # LeaveOneOutのときエラーを出す
-            if isinstance(cv, LeaveOneOut):
-                raise Exception('"regression_heat_plot" method does not support "LeaveOneOut" cross validation')
-            # cv_groupをグルーピング対象に指定(GroupKFold、LeaveOneGroupOut等)
-            split_kws={}
-            if cv_group_colname is not None:
-                split_kws['groups'] = data[cv_group_colname].values
-            elif isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
-                raise Exception('"GroupKFold" and "LeaveOneGroupOut" cross validations need ``cv_group`` argument')
-            # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
-            if isinstance(cv, LeaveOneGroupOut):
-                cv_num = len(set(data[cv_group_colname].values))
-            else:
-                cv_num = cv.n_splits
-
-            # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
-            if eval_set_selection is None:
-                eval_set_selection = 'test'
-            fit_params, eval_set_selection = init_eval_set(
-                    eval_set_selection, fit_params, X, y)
-            # 最終学習器以外の前処理変換器作成
-            transformer = _make_transformer(eval_set_selection, estimator)
-
-            # クロスバリデーション
-            for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
-                # 表示対象以外のCVなら飛ばす
-                if i not in display_cv_indices:
-                    continue
-                print(f'cv_number={i}/{cv_num}')
-                # 表示用にテストデータと学習データ分割
-                X_train = X[train]
-                y_train = y_true[train]
-                data_test = data.iloc[test]
-                
-                # eval_setの中から学習データ or テストデータのみを抽出
-                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
-                                                        fit_params, train, test)
-
-                # 学習と推論
-                estimator.fit(X_train, y_train, **fit_params_modified)
-                # ヒートマップをプロット
-                cls._average_plot(estimator, data_test, x_colnames, y_colname, hue,
-                                  aggregate=aggregate,
-                                  subplot_kws=subplot_kws, plot_kws=plot_kws,
-                                  scatter_kws=scatter_kws, legend_kws=legend_kws,
-                                  cv_index=i)
-
-        
-    @classmethod
-    def linear_plot(cls, x: str, y: str, data: pd.DataFrame = None,
-                    x_colname: str = None,
-                    ax=None, hue=None, linecolor='red',
-                    rounddigit=5, plot_scores=True, scatter_kws=None, legend_kws=None):
-        """
-        Plot linear regression line and calculate Pearson correlation coefficient.
-
-        Parameters
-        ----------
-        x : str
-            Variable that specify positions on the x.
-
-        y : str
-            Variable that specify positions on the y.
-
-        data : pd.DataFrame
-            Input data structure.
-
-        x_colname: str, optional
-            Names of explanatory variable. Available only if ``data`` is NOT pd.DataFrame
-
-        ax : matplotlib.axes.Axes, optional
-            Pre-existing axes for the plot. Otherwise, call matplotlib.pyplot.gca() internally.
-
-        hue : str, optional
-            Grouping variable that will produce points with different colors.
-
-        linecolor : str, optional
-            Color of regression line. See https://matplotlib.org/stable/gallery/color/named_colors.html
-
-        rounddigit: int, optional
-            Round a number of score to a given precision in decimal digits.
-
-        plot_scores: bool, optional
-            If True, display Pearson correlation coefficient and the p-value.
-
-        scatter_kws: dict, optional
-            Additional parameters passed to sns.scatterplot(), e.g. ``alpha``. See https://seaborn.pydata.org/generated/seaborn.scatterplot.html
-
-        legend_kws : dict
-            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
-
-        Returns
-        ----------
-        ax : matplotlib.axes.Axes
-            Returns the Axes object with the plot drawn onto it.
-        """
-
-        # 入力データの形式統一
-        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data([x] if isinstance(x, str) else x, 
-                                                                                           y, data,
-                                                                                           [x_colname] if x_colname is not None else x_colname,
-                                                                                           cv_group=None)
-        if x_colname is None:
-            x_colname = x_colnames[0]
-        # scatter_kwsがNoneなら空のdictを入力
-        if scatter_kws is None:
-            scatter_kws = {}
-        # legend_kwsがNoneなら空のdictを入力
-        if legend_kws is None:
-            legend_kws = {}
-
-        # まずは散布図プロット
-        ax = sns.scatterplot(x=x_colname, y=y_colname, data=data, ax=ax, hue=hue, **scatter_kws)
-        # 凡例追加
-        if hue is not None and 'title' not in legend_kws.keys():
-            legend_kws['title'] = hue
-        if len(legend_kws.keys()) > 0:
-            ax.legend(**legend_kws)
-
-        # 線形回帰モデル作成
-        lr = LinearRegression()
-        lr.fit(X, y_true)
-        xmin = np.amin(X)
-        xmax = np.amax(X)
-        linesplit=200
-        Xline = np.linspace(xmin, xmax, linesplit)
-        Xline = Xline.reshape(len(Xline), 1)
-        # 回帰線を描画
-        ax.plot(Xline, lr.predict(Xline), color=linecolor)
-
-        # 回帰式、ピアソンの相関係数およびp値を表示
-        if plot_scores == True:
-            # 回帰式
-            coef = cls._round_digits(lr.coef_[0], rounddigit=rounddigit, method="decimal")
-            intercept = cls._round_digits(lr.intercept_, rounddigit=rounddigit, method="decimal")
-            equation = f'y={coef}x+{intercept}' if intercept >= 0 else f'y={coef}x-{-intercept}'
-            # ピアソン相関係数
-            pearsonr = stats.pearsonr(data[x_colname], data[y_colname])
-            r = cls._round_digits(pearsonr[0], rounddigit=rounddigit, method="decimal")
-            pvalue = cls._round_digits(pearsonr[1], rounddigit=rounddigit, method="decimal")            
-            # プロット
-            rtext = f'{equation}\nr={r}\np={pvalue}'
-            ax.text(xmax, np.amin(y_true), rtext, verticalalignment='bottom', horizontalalignment='right')
-
-        return ax
-
-    @classmethod
-    def _estimator_plot_1d(cls, trained_estimator, X, y_true, hue_data=None, hue_name=None, ax=None, linecolor='red', linesplit=1000, rounddigit=None,
-                       score_dict=None, scatter_kws=None, legend_kws=None):
-        """
-        1次説明変数回帰曲線を、回帰評価指標とともにプロット
-
-        Parameters
-        ----------
-        trained_estimator : 
-            学習済の回帰モデル(scikit-learn API)
-
-        X : ndarray
-            説明変数
-
-        y_true : ndarray
-            目的変数実測値
-
-        hue_data : ndarray
-            色分け用ラベルデータ
-
-        hue_name : str
-            色分け用の列名
-
-        ax : matplotlib.axes.Axes
-            表示対象のax (Noneならplt.plotで1枚ごとにプロット)
-
-        linecolor : str
-            予測値=実測値の線の色
-
-        linesplit : int
-            フィッティング線の分割数 (カクカクしたら増やす)
-
-        rounddigit: int
-            表示指標の小数丸め桁数
-
-        score_dict : dict[str, float]
-            算出した評価指標一覧
-
-        scatter_kws: dict, optional
-            Additional parameters passed to sns.scatterplot(), e.g. ``alpha``. See https://seaborn.pydata.org/generated/seaborn.scatterplot.html
-
-        legend_kws : dict
-            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
-        """
-        # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
-        if ax is None:
-            ax=plt.gca()
-        # score_dictがNoneのとき、空のDictを入力
-        if score_dict is None:
-            score_dict = {}
-        # scatter_kwsがNoneなら空のdictを入力
-        if scatter_kws is None:
-            scatter_kws = {}
-        # legend_kwsがNoneなら空のdictを入力
-        if legend_kws is None:
-            legend_kws = {}
-        
-        # 散布図プロット
-        cls._scatterplot_ndarray(np.ravel(X), 'X', y_true, 'Y', hue_data, hue_name, ax, scatter_kws, legend_kws)
-
-        # 回帰モデルの線を作成
-        xmin = np.amin(X)
-        xmax = np.amax(X)
-        Xline = np.linspace(xmin, xmax, linesplit)
-        Xline = Xline.reshape(len(Xline), 1)
-        # 回帰線を描画
-        ax.plot(Xline, trained_estimator.predict(Xline), color=linecolor)
-        
-        # 評価指標文字列作成
-        score_list = [f'{k}={v}' for k, v in cls._round_dict_digits(score_dict, rounddigit, 'sig').items()]
-        score_text = "\n".join(score_list)
-        ax.text(xmax, np.amin(y_true), score_text, verticalalignment='bottom', horizontalalignment='right')
-
-    @classmethod
-    def regression_plot_1d(cls, estimator, x: str, y: str, data: pd.DataFrame = None, x_colname: str = None,
-                           hue=None, linecolor='red', rounddigit=3,
-                           rank_number=None, rank_col=None, scores='mae',
-                           cv_stats='mean', cv=None, cv_seed=42, cv_group=None,
-                           estimator_params=None, fit_params=None, eval_set_selection=None,
-                           subplot_kws=None, scatter_kws=None, legend_kws=None):
-        """
-        Plot regression lines of any scikit-learn regressor with 1D explanatory variable.
-
-        Parameters
-        ----------
-        estimator : estimator object implementing ``fit``
-            Regression estimator. This is assumed to implement the scikit-learn estimator interface.
-
-        x : str, or np.ndarray
-            Explanatory variables. Should be str if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
-
-        y : str or np.ndarray
-            Objective variable. Should be str if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
-
-        data: pd.DataFrame
-            Input data structure.
-
-        x_colname: str, optional
-            Names of explanatory variable. Available only if ``data`` is NOT pd.DataFrame
-
-        hue : str, optional
-            Grouping variable that will produce points with different colors.
-
-        linecolor : str, optional
-            Color of prediction = true line. See https://matplotlib.org/stable/gallery/color/named_colors.html
-
-        rounddigit: int, optional
-            Round a number of score to a given precision in decimal digits.
-
-        rank_number : int, optional
-            Number of emphasized data that are in the top positions for regression error.
-
-        rank_col : list[str], optional
-            Variables that are displayed with emphasized data that are in the top posiotions for regression error.
-
-        scores : {'r2', 'mae', 'mse', 'rmse', 'rmsle', 'mape', 'max_error'} or list,, optional
-            Regression score that are displayed at the lower right of the graph.
-
-        cv_stats : {'mean', 'median', 'max', 'min'}, optional
-            Statistical method of cross validation score that are displayed at the lower right of the graph.
-
-        cv : int, cross-validation generator, or an iterable, optional
-            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
-
-        cv_seed : int, optional
-            Seed for random number generator of cross validation.
-
-        cv_group: str, optional
-            Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
-
-        estimator_params : dict, optional
-            Parameters passed to the regression estimator. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
-
-        fit_params : dict, optional
-            Parameters passed to the fit() method of the regression estimator, e.g. ``early_stopping_round`` and ``eval_set`` of XGBRegressor. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
-
-        subplot_kws : dict, optional
-            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
-
-        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
-
-            If "test", select test data from `X` and `y` using cv.split().
-
-            If "original", use raw `eval_set`.
-
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
-
-        scatter_kws: dict, optional
-            Additional parameters passed to sns.scatterplot(), e.g. ``alpha``. See https://seaborn.pydata.org/generated/seaborn.scatterplot.html
-
-        legend_kws : dict
-            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
-
-        Returns
-        ----------
-        score_dict : dict
-            Validation scores, e.g. r2, mae and rmse
-        """
-
-        # 入力データの形式統一
-        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data([x] if isinstance(x, str) else x,
-                                                                                           y, data,
-                                                                                           [x_colname] if x_colname is not None else x_colname,
-                                                                                           cv_group)
-        # scoresの型をListに統一
-        if scores is None:
-            scores = []
-        elif isinstance(scores, str):
-            scores = [scores]
-        elif not isinstance(scores, list):
-            raise Exception('the "scores" argument must be str or list[str]')
-        # 学習器パラメータがあれば適用
-        if estimator_params is not None:
-            estimator.set_params(**estimator_params)
-        # 学習時パラメータがNoneなら空のdictを入力
-        if fit_params is None:
-            fit_params = {}
-        # subplot_kwsがNoneなら空のdictを入力
-        if subplot_kws is None:
-            subplot_kws = {}
-        # scatter_kwsがNoneなら空のdictを入力
-        if scatter_kws is None:
-            scatter_kws = {}
-        # legend_kwsがNoneなら空のdictを入力
-        if legend_kws is None:
-            legend_kws = {}
-        
-        # クロスバリデーション有無で場合分け
-        # クロスバリデーション未実施時(学習データからプロット＆指標算出)
-        if cv is None:
-            # 学習と推論
-            estimator.fit(X, y_true, **fit_params)
-            y_pred = estimator.predict(X)
-            # 評価指標算出
-            score_dict = cls._make_score_dict(y_true, y_pred, scores)
-            # 色分け用データ取得
-            hue_data = None if hue is None else data[hue]
-            hue_name = None if hue is None else hue
-            # 誤差上位表示用データ取得
-            if rank_number is not None:
-                if rank_col is None:  # 表示フィールド指定ないとき、Index使用
-                    rank_col_data = data.index.values
-                else:  # 表示フィールド指定あるとき
-                    rank_col_data = data[rank_col].values
-            # 回帰線プロット
-            cls._estimator_plot_1d(estimator, X, y_true, hue_data=hue_data, hue_name=hue_name,
-                               linecolor=linecolor, rounddigit=rounddigit, score_dict=score_dict,
-                               scatter_kws=scatter_kws, legend_kws=legend_kws)
-            # 誤差上位を文字表示
-            if rank_number is not None:
-                cls._rank_display(y_true, y_pred, rank_number, rank_col, rank_col_data, x=X, rounddigit=rounddigit)
-            return score_dict
-            
-        # クロスバリデーション実施時(分割ごとに別々にプロット＆指標算出)
-        if cv is not None:
-            # 分割法未指定時、cv_numとseedに基づきKFoldでランダムに分割
-            if isinstance(cv, numbers.Integral):
-                cv = KFold(n_splits=cv, shuffle=True, random_state=cv_seed)
-            #LeaveOneOutのときエラーを出す
-            if isinstance(cv, LeaveOneOut):
-                raise Exception('"regression_plot_1d" method does not support "LeaveOneOut" cross validation')
-            # cv_groupをグルーピング対象に指定(GroupKFold、LeaveOneGroupOut等)
-            split_kws={}
-            if cv_group_colname is not None:
-                split_kws['groups'] = data[cv_group_colname].values
-            elif isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
-                raise Exception('"GroupKFold" and "LeaveOneGroupOut" cross validations need ``cv_group`` argument')
-            # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
-            if isinstance(cv, LeaveOneGroupOut):
-                cv_num = len(set(data[cv_group_colname].values))
-            else:
-                cv_num = cv.n_splits
-
-            # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
-            if eval_set_selection is None:
-                eval_set_selection = 'test'
-            fit_params, eval_set_selection = init_eval_set(
-                    eval_set_selection, fit_params, X, y)
-            # 最終学習器以外の前処理変換器作成
-            transformer = _make_transformer(eval_set_selection, estimator)
-
-            # スコア種類ごとにクロスバリデーションスコアの算出
-            score_all_dict = {}
-            for scoring in scores:
-                # cross_val_scoreでクロスバリデーション
-                if scoring == 'r2':
-                    score_all_dict['r2'] = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true, 
-                                                    cv=cv, scoring='r2',
-                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
-                elif scoring == 'mae':
-                    neg_mae = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true, 
-                                                    cv=cv, scoring='neg_mean_absolute_error',
-                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
-                    score_all_dict['mae'] = -neg_mae  # scikit-learnの仕様に合わせ正負を逆に
-                elif scoring == 'mse':
-                    neg_mse = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
-                                                    cv=cv, scoring='neg_mean_squared_error',
-                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
-                    score_all_dict['mse'] = -neg_mse  # scikit-learnの仕様に合わせ正負を逆に
-                elif scoring == 'rmse':
-                    neg_rmse = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
-                                                    cv=cv, scoring='neg_root_mean_squared_error',
-                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
-                    score_all_dict['rmse'] = -neg_rmse  # scikit-learnの仕様に合わせ正負を逆に
-                elif scoring == 'rmsle':
-                    neg_msle = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
-                                                    cv=cv, scoring='neg_mean_squared_log_error',
-                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
-                    score_all_dict['rmsle'] = np.sqrt(-neg_msle)  # 正負を逆にしてルートをとる
-                elif scoring == 'mape':
-                    neg_mape = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
-                                                    cv=cv, scoring='neg_mean_absolute_percentage_error',
-                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
-                    score_all_dict['mape'] = -neg_mape  # scikit-learnの仕様に合わせ正負を逆に
-                elif scoring == 'max_error':
-                    neg_max_error = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
-                                                    cv=cv, scoring='max_error',
-                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
-                    score_all_dict['max_error'] = - neg_max_error  # scikit-learnの仕様に合わせ正負を逆に
-            
-            # 表示用のaxes作成
-            # クロスバリデーションごとに図作成
-            if 'figsize' not in subplot_kws.keys():
-                subplot_kws['figsize'] = (6, (cv_num + 1) * 6)
-            fig, axes = plt.subplots(cv_num + 1, 1, **subplot_kws)
-
-            # クロスバリデーション
-            score_train_dict = {}
-            for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
-                # 表示用にテストデータと学習データ分割
-                X_train = X[train]
-                y_train = y_true[train]
-                X_test = X[test]
-                y_test = y_true[test]
-                # 色分け用データ取得(していないときは、クロスバリデーション番号を使用、LeaveOuneOutのときは番号分けない)
-                if hue is None:
-                    hue_test = np.full(len(test) ,f'cv_{i}')
-                    hue_name = 'cv_number'  # 色分け名を'cv_number'に指定
-                else:
-                    hue_test = data[hue].values[test]
-                    hue_name = hue
-                # 誤差上位表示用データ取得
-                if rank_number is not None:
-                    if rank_col is None:  # 表示フィールド指定ないとき、Index使用
-                        rank_col_test = data.index.values[test]
-                    else:  # 表示フィールド指定あるとき
-                        rank_col_test = data[rank_col].values[test]
-                
-                # eval_setの中から学習データ or テストデータのみを抽出
-                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
-                                                        fit_params, train, test)
-
-                # 学習と推論
-                estimator.fit(X_train, y_train, **fit_params_modified)
-                # 学習データスコア算出
-                y_pred_train = estimator.predict(X_train)
-                score_dict = cls._make_score_dict(y_train, y_pred_train, scores)
-                for score in scores:
-                    if f'{score}_train' not in score_train_dict:
-                        score_train_dict[f'{score}_train'] = []
-                    score_train_dict[f'{score}_train'].append(score_dict[score])
-                # CV内結果をプロット
-                score_cv_dict = {k: v[i] for k, v in score_all_dict.items()}
-                score_cv_dict.update({f'{k}_train': v for k, v in score_dict.items()})
-                cls._estimator_plot_1d(estimator, X_test, y_test, hue_data=hue_test, hue_name=hue_name, ax=axes[i],
-                                   linecolor=linecolor, rounddigit=rounddigit, score_dict=score_cv_dict,
-                                   scatter_kws=scatter_kws, legend_kws=legend_kws)
-                # 誤差上位を文字表示
-                if rank_number is not None:
-                    cls._rank_display(y_test, estimator.predict(X_test), rank_number, rank_col, rank_col_test, x=X_test, ax=axes[i], rounddigit=rounddigit)
-                axes[i].set_title(f'Cross Validation Fold{i}')
-
-            # スコアの統計値を計算
-            if cv_stats == 'mean':
-                score_stats_dict = {f'{k}_mean': np.mean(v) for k, v in score_all_dict.items()}
-                train_stats_dict = {k: np.mean(v) for k, v in score_train_dict.items()}
-            elif cv_stats == 'median':
-                score_stats_dict = {f'{k}_median': np.median(v) for k, v in score_all_dict.items()}
-                train_stats_dict = {k: np.median(v) for k, v in score_train_dict.items()}
-            elif cv_stats == 'min':
-                score_stats_dict = {f'{k}_min': np.amin(v) for k, v in score_all_dict.items()}
-                train_stats_dict = {k: np.amin(v) for k, v in score_train_dict.items()}
-            elif cv_stats == 'max':
-                score_stats_dict = {f'{k}_max': np.amax(v) for k, v in score_all_dict.items()}
-                train_stats_dict = {k: np.amax(v) for k, v in score_train_dict.items()}
-            # 学習データスコアをdictに追加
-            score_stats_dict.update(train_stats_dict)
-            # 全体色分け用データ取得
-            hue_data = None if hue is None else data[hue]
-            hue_name = None if hue is None else hue
-            # 全体プロット
-            ax_all = axes[cv_num]
-            cls._estimator_plot_1d(estimator, X, y_true, hue_data=hue_data, hue_name=hue_name, ax=ax_all,
-                               linecolor=linecolor, rounddigit=rounddigit, score_dict=score_stats_dict,
-                               scatter_kws=scatter_kws, legend_kws=legend_kws)
-            ax_all.set_title('All Cross Validations')
-            return score_stats_dict
-
-    @classmethod
-    def _reg_heat_plot_2d(cls, trained_estimator, x_heat, y_true_col, y_pred_col, rank_col, data, x_heat_indices, hue_name,
-                          x1_start, x1_end, x2_start, x2_end, heat_division, other_x,
-                          vmin, vmax, ax, plot_scatter, maxerror, rank_dict, scatter_hue_dict,
-                          rounddigit_rank, rounddigit_x1, rounddigit_x2,
-                          heat_kws=None, scatter_kws=None, legend_kws=None):
-        """
-        回帰予測値ヒートマップと各種散布図の表示
-        (regression_heat_plotメソッドの描画処理部分)
-        """
-        # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
-        if ax is None:
-            ax=plt.gca()
-
-        # ヒートマップ用グリッドデータを作成
-        xx = np.linspace(x1_start, x1_end, heat_division)
-        yy = np.linspace(x2_start, x2_end, heat_division)
-        X1, X2 = np.meshgrid(xx, yy)
-        X_grid = np.c_[X1.ravel(), X2.ravel()]
-        df_heat = pd.DataFrame(X_grid, columns=x_heat)
-        # 推論用に全説明変数を保持したndarrayを作成 (ヒートマップ非使用変数は固定値other_xとして追加)
-        n_rows = X_grid.shape[0]
-        X_all = []
-        other_add_flg = False
-        for i in range(2 + len(other_x)):
-            if i == x_heat_indices[0]: # ヒートマップ使用変数(1個目)を追加
-                X_all.append(X_grid[:, 0].reshape(n_rows, 1))
-            elif i == x_heat_indices[1]: # ヒートマップ使用変数(2個目)を追加
-                X_all.append(X_grid[:, 1].reshape(n_rows, 1))
-            elif len(other_x) >= 1 and not other_add_flg:  # ヒートマップ非使用変数(1個目)を固定値として追加
-                X_all.append(np.full((n_rows, 1), other_x[0]))
-                other_add_flg = True
-            elif len(other_x) == 2:  # ヒートマップ非使用変数(2個目)を固定値として追加
-                X_all.append(np.full((n_rows, 1), other_x[1]))
-        X_all = np.hstack(X_all)
-        # グリッドデータに対して学習し、推定値を作成
-        y_pred_grid = trained_estimator.predict(X_all)
-        df_heat['y_pred'] = pd.Series(y_pred_grid)
-        # グリッドデータ縦軸横軸の表示桁数を調整
-        df_heat[x_heat[0]] = df_heat[x_heat[0]].map(lambda x: cls._round_digits(x, rounddigit=rounddigit_x1))
-        df_heat[x_heat[1]] = df_heat[x_heat[1]].map(lambda x: cls._round_digits(x, rounddigit=rounddigit_x2))
-        # グリッドデータをピボット化
-        df_heat_pivot = pd.pivot_table(data=df_heat, values='y_pred', 
-                                  columns=x_heat[0], index=x_heat[1], aggfunc=np.mean)
-        # 横軸の列数がheat_divisionに満たない時、分解能不足のためrounddigit_x1桁数を増やすようエラー表示
-        if len(df_heat_pivot.columns) < heat_division:
-            raise Exception(f'the "rounddigit_x1" argument must be bigger than {rounddigit_x1} because of the shortage of the "{x_heat[0]}" resolution')
-        # 縦軸の列数がheat_divisionに満たない時、分解能不足のためrounddigit_x2桁数を増やすようエラー表示
-        if len(df_heat_pivot) < heat_division:
-            raise Exception(f'the "rounddigit_x2" argument must be bigger than {rounddigit_x2} because of the shortage of the "{x_heat[1]}" resolution')
-
-        # ヒートマップのカラーマップ指定ないとき、YlGnを指定
-        if 'cmap' not in heat_kws.keys():
-            heat_kws['cmap'] = 'YlGn'
-        # ヒートマップをプロット
-        sns.heatmap(df_heat_pivot, ax=ax, vmax=vmax, vmin=vmin, center=(vmax+vmin)/2, **heat_kws)
-
-        # 誤差散布図をプロット
-        if plot_scatter is not None:
-            # 軸範囲が0～heat_divisionになっているので、スケール変換
-            x1_scatter = 0.5 + (data[x_heat[0]].values - x1_start) * (heat_division - 1) / (x1_end - x1_start)
-            x2_scatter = 0.5 + (data[x_heat[1]].values - x2_start) * (heat_division - 1) / (x2_end - x2_start)
-            # 色分け
-            if plot_scatter == 'error':  # 誤差で色分け
-                scatter_c = data[y_pred_col].values - data[y_true_col].values
-                scatter_vmin = -maxerror
-                scatter_vmax = maxerror
-                if 'cmap' not in scatter_kws.keys():  # 散布図のカラーマップ指定ないとき、seismicを指定
-                    scatter_kws['cmap'] = 'seismic'
-            elif plot_scatter == 'true':  # 真値で色分け
-                scatter_c = data[y_true_col].values
-                scatter_vmin = vmin
-                scatter_vmax = vmax
-                if 'cmap' not in scatter_kws.keys():  # 散布図のカラーマップ指定ないとき、ヒートマップと同cmap使用
-                    scatter_kws['cmap'] = heat_kws['cmap']
-                if 'edgecolors' not in scatter_kws.keys():  # 線の色指定ないとき、ブラウンを指定
-                    scatter_kws['edgecolors'] = 'brown'
-            # 散布図プロット (誤差or真値で色分けしたとき)
-            if plot_scatter == 'error' or plot_scatter == 'true':
-                ax.scatter(x1_scatter, x2_scatter, vmin=scatter_vmin, vmax=scatter_vmax, c=scatter_c, **scatter_kws)
-            # 散布図プロット (hue列名で色分けしたとき)
-            if plot_scatter == 'hue':
-                scatter_data = pd.DataFrame(np.stack([x1_scatter, x2_scatter, data[hue_name]], 1), columns=['x1', 'x2', hue_name])
-                for name, group in scatter_data.groupby(hue_name):
-                    ax.scatter(group['x1'].values, group['x2'].values, label=name, c=scatter_hue_dict[name], **scatter_kws)
-                ax.legend(**legend_kws)
-        
-        # 誤差上位を文字表示
-        df_rank = data[data.index.isin(rank_dict.keys())]
-        for index, row in df_rank.iterrows():
-            # rank_col指定ないとき、indexがfloat型に変換されてしまうので、int型に戻す
-            rank_col_value = int(row[rank_col]) if rank_col == 'index' else row[rank_col]
-            # 誤差を計算してテキスト化
-            error = cls._round_digits(row['y_pred'] - row['y_true'], rounddigit=rounddigit_rank)
-            rank_text = f'     no{rank_dict[index]+1}\n-<-error={error}\n     {rank_col}={rank_col_value}'
-            # 軸範囲が0～heat_divisionになっているので、スケール変換してプロット
-            x1_text = 0.5 + (row[x_heat[0]] - x1_start) * (heat_division - 1) / (x1_end - x1_start)
-            x2_text = 0.5 + (row[x_heat[1]] - x2_start) * (heat_division - 1) / (x2_end - x2_start)
-            ax.text(x1_text, x2_text, rank_text, verticalalignment='center', horizontalalignment='left')
-    
-    @classmethod
-    def _reg_heat_plot(cls, trained_estimator, X, y_pred, y_true, x_heat, x_not_heat, x_heat_indices, hue_data, hue_name,
-                       pair_sigmarange=1.0, pair_sigmainterval=0.5, heat_extendsigma=0.5, heat_division=30, 
-                       vmin=None, vmax=None, plot_scatter='true', maxerror=None,
-                       rank_number=None, rank_col=None, rank_col_data=None, scatter_hue_dict=None,
-                       rounddigit_rank=None, rounddigit_x1=None, rounddigit_x2=None, rounddigit_x3=None,
-                       cv_index=None, subplot_kws=None, heat_kws=None, scatter_kws=None, legend_kws=None):
-        """
-        回帰予測値ヒートマップ表示の、説明変数の数に応じた分岐処理
-        (regression_heat_plotメソッド処理のうち、説明変数の数に応じたデータ分割等を行う)
-        """
-        # 説明変数の数
-        x_num = X.shape[1]
-        # ヒートマップ使用DataFrame
-        df_heat = pd.DataFrame(X[:, x_heat_indices], columns=x_heat)
-        # ヒートマップ非使用DataFrame
-        X_not_heat = X[:, [i for i in range(X.shape[1]) if i not in x_heat_indices]]
-        df_not_heat = pd.DataFrame(X_not_heat, columns=x_not_heat)
-        # 結合＆目的変数実測値と予測値追加
-        df_all = df_heat.join(df_not_heat)
-        df_all = df_all.join(pd.DataFrame(y_true, columns=['y_true']))
-        df_all = df_all.join(pd.DataFrame(y_pred, columns=['y_pred']))
-        # ヒートップ非使用変数を標準化してDataFrameに追加
-        if x_num >= 3:
-            X_not_heat_norm = stats.zscore(X_not_heat)
-            df_all = df_all.join(pd.DataFrame(X_not_heat_norm, columns=[f'normalize_{c}' for c in x_not_heat]))
-        # 誤差上位表示用IDデータをDataFrameに追加
-        rank_col = 'index' if rank_col is None else rank_col
-        df_all = df_all.join(pd.DataFrame(rank_col_data, columns=[rank_col]))
-        # 散布図色分け用列をDataFrameに追加(hue_nameがNoneでないときのみ))
-        if hue_name is not None:
-            df_all = df_all.join(pd.DataFrame(hue_data, columns=[hue_name]))
-
-        # 誤差の順位を計算
-        if rank_number is not None:
-            y_error_abs = np.abs(y_pred - y_true)
-            rank_index  = np.argsort(-y_error_abs)[:rank_number]
-            rank_dict = dict(zip(rank_index.tolist(), range(rank_number)))
-        else:
-            rank_dict = {}
-
-        # ヒートマップのX1軸およびX2軸の表示範囲(最大最小値 + extendsigma)
-        x1_min = np.min(X[:, x_heat_indices[0]])
-        x1_max = np.max(X[:, x_heat_indices[0]])
-        x1_std = np.std(X[:, x_heat_indices[0]])
-        x1_start = x1_min - x1_std * heat_extendsigma
-        x1_end = x1_max + x1_std * heat_extendsigma
-        x2_min = np.min(X[:, x_heat_indices[1]])
-        x2_max = np.max(X[:, x_heat_indices[1]])
-        x2_std = np.std(X[:, x_heat_indices[1]])
-        x2_start = x2_min - x2_std * heat_extendsigma
-        x2_end = x2_max + x2_std * heat_extendsigma
-
-        # プロットする図の数(sigmarange外「2枚」 + sigmarange内「int(pair_sigmarange / pair_sigmainterval) * 2枚」)
-        pair_n = int(pair_sigmarange / pair_sigmainterval) * 2 + 2
-        # ヒートップ非使用変数をプロットする範囲の下限(標準化後)
-        pair_min = -(pair_n - 2) / 2 * pair_sigmainterval
-
-        # 説明変数が2次元のとき (図は1枚のみ)
-        if x_num == 2:
-            pair_w = 1
-            pair_h = 1
-        # 説明変数が3次元のとき (図はpair_n × 1枚)
-        elif x_num == 3:
-            pair_w = 1
-            pair_h = pair_n
-        # 説明変数が4次元のとき (図はpair_n × pair_n枚)
-        elif x_num == 4:
-            pair_w = pair_n
-            pair_h = pair_n
-
-        # figsize (全ての図全体のサイズ)指定
-        if 'figsize' not in subplot_kws.keys():
-            subplot_kws['figsize'] = (pair_w * 6, pair_h * 5)
-        # プロット用のaxes作成
-        fig, axes = plt.subplots(pair_h, pair_w, **subplot_kws)
-        if cv_index is not None:
-            fig.suptitle(f'CV No.{cv_index}')
-
-        # 図ごとにプロット
-        for i in range(pair_h):
-            for j in range(pair_w):
-                # pair縦軸変数(標準化後)の最小値
-                if i == 0:
-                    h_min = -float('inf')
-                    h_mean = pair_min - pair_sigmainterval / 2  # ヒートマップ非使用変数指定用の平均値
-                else:
-                    h_min = pair_min + (i - 1) * pair_sigmainterval
-                    h_mean = pair_min + (i - 0.5) * pair_sigmainterval  # ヒートマップ非使用変数指定用の平均値
-                # pair縦軸変数(標準化後)の最大値
-                if i == pair_h - 1:
-                    h_max = float('inf')
-                else:
-                    h_max = pair_min + i * pair_sigmainterval
-                # pair横軸変数(標準化後)の最小値
-                if j == 0:
-                    w_min = -float('inf')
-                    w_mean = pair_min - pair_sigmainterval / 2  # ヒートマップ非使用変数指定用の平均値
-                else:
-                    w_min = pair_min + (j - 1) * pair_sigmainterval
-                    w_mean = pair_min + (j - 0.5) * pair_sigmainterval  # ヒートマップ非使用変数指定用の平均値
-                # pair横軸変数(標準化後)の最大値
-                if j == pair_w - 1:
-                    w_max = float('inf')
-                else:
-                    w_max = pair_min + j * pair_sigmainterval
-
-                # 説明変数が2次元のとき (図は1枚のみ)
-                if x_num == 2:
-                    ax = axes
-                    df_pair = df_all.copy()
-                    other_x = []
-                # 説明変数が3次元のとき (図はpair_n × 1枚)
-                elif x_num == 3:
-                    ax = axes[i]
-                    # 縦軸変数範囲内のみのデータを抽出
-                    df_pair = df_all[(df_all[f'normalize_{x_not_heat[0]}'] >= h_min) & (df_all[f'normalize_{x_not_heat[0]}'] < h_max)].copy()
-                    # ヒートマップ非使用変数の標準化逆変換
-                    x3_mean = np.mean(X_not_heat[:, 0])
-                    x3_std = np.std(X_not_heat[:, 0])
-                    other_x = [h_mean * x3_std + x3_mean]
-                # 説明変数が4次元のとき (図はpair_n × pair_n枚)
-                elif x_num == 4:
-                    ax = axes[j, i]
-                    # 縦軸変数範囲内のみのデータを抽出
-                    df_pair = df_all[(df_all[f'normalize_{x_not_heat[0]}'] >= h_min) & (df_all[f'normalize_{x_not_heat[0]}'] < h_max)].copy()
-                    # 横軸変数範囲内のみのデータを抽出
-                    df_pair = df_pair[(df_pair[f'normalize_{x_not_heat[1]}'] >= w_min) & (df_pair[f'normalize_{x_not_heat[1]}'] < w_max)]
-                    # ヒートマップ非使用変数の標準化逆変換
-                    x3_mean = np.mean(X_not_heat[:, 0])
-                    x3_std = np.std(X_not_heat[:, 0])
-                    x4_mean = np.mean(X_not_heat[:, 1])
-                    x4_std = np.std(X_not_heat[:, 1])
-                    other_x = [h_mean * x3_std + x3_mean, w_mean * x4_std + x4_mean]
-                
-                cls._reg_heat_plot_2d(trained_estimator, x_heat, 'y_true', 'y_pred', rank_col, df_pair, x_heat_indices, hue_name,
-                                      x1_start, x1_end, x2_start, x2_end, heat_division, other_x,
-                                      vmin, vmax, ax, plot_scatter, maxerror, rank_dict, scatter_hue_dict,
-                                      rounddigit_rank, rounddigit_x1, rounddigit_x2,
-                                      heat_kws=heat_kws, scatter_kws=scatter_kws, legend_kws=legend_kws)
-
-                # グラフタイトルとして、ヒートマップ非使用変数の範囲を記載（説明変数が3次元以上のとき）
-                if x_num == 3:
-                    if i == 0:
-                        ax.set_title(f'{x_not_heat[0]}=- {cls._round_digits(h_max * x3_std + x3_mean, rounddigit=rounddigit_x3)} (- {h_max}σ)')
-                    elif i == pair_h - 1:
-                        ax.set_title(f'{x_not_heat[0]}={cls._round_digits(h_min * x3_std + x3_mean, rounddigit=rounddigit_x3)} - ({h_min}σ -)')
-                    else:
-                        ax.set_title(f'{x_not_heat[0]}={cls._round_digits(h_min * x3_std + x3_mean, rounddigit=rounddigit_x3)} - {cls._round_digits(h_max * x3_std + x3_mean, rounddigit=rounddigit_x3)} ({h_min}σ - {h_max}σ)')
-                if x_num == 4:
-                    ax.set_title(f'{x_not_heat[0]}= {h_min}σ - {h_max}σ  {x_not_heat[1]}= {w_min}σ - {w_max}σ')
-
-        # 字が重なるのでtight_layoutにする
-        plt.tight_layout(rect=[0, 0, 1, 0.98])
-
-    @classmethod
-    def regression_heat_plot(cls, estimator, x: List[str], y: str, data: pd.DataFrame = None,
-                             x_colnames: List[str] = None, x_heat: List[str] = None, scatter_hue=None,
-                             pair_sigmarange = 1.0, pair_sigmainterval = 0.5, heat_extendsigma = 0.5, 
-                             heat_division = 30, color_extendsigma = 0.5,
-                             plot_scatter = 'true', rounddigit_rank=3, rounddigit_x1=2, rounddigit_x2=2, rounddigit_x3=2,
-                             rank_number=None, rank_col=None,
-                             cv=None, cv_seed=42, cv_group=None, display_cv_indices = 0,
-                             estimator_params=None, fit_params=None, eval_set_selection=None,
-                             subplot_kws=None, heat_kws=None, scatter_kws=None, legend_kws=None):
-        """
-        Plot regression heatmaps of any scikit-learn regressor with 2 to 4D explanatory variables.
-
-        Parameters
-        ----------
-        estimator : estimator object implementing ``fit``
-            Regression estimator. This is assumed to implement the scikit-learn estimator interface.
-
-        x : list[str] or np.ndarray
-            Explanatory variables. Should be list[str] if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
-
-        y : str or np.ndarray
-            Objective variable. Should be str if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
-
-        data: pd.DataFrame
-            Input data structure.
-
-        x_colnames: list[str], optional
-            Names of explanatory variables. Available only if ``data`` is NOT pd.DataFrame
-
-        x_heat: list[str], optional
-            X-axis and y-axis variables of heatmap. If None, use two variables in ``x`` from the front.
-
-        scatter_hue : str, optional
-            Grouping variable that will produce points with different colors. Available only if plot_scatter is set to ``hue``.
-
-        pair_sigmarange: float, optional
-            Set the range of subplots. The lower limit is mean({x3, x4}) - ``pair_sigmarange`` * std({x3, x4}). The higher limit is mean({x3, x4}) + ``pair_sigmarange`` * std({x3, x4}). Available only if len(x) is bigger than 2.
-
-        pair_sigmainterval: float, optional
-            Set the interval of subplots. For example, if ``pair_sigmainterval`` is set to 0.5 and ``pair_sigmarange`` is set to 1.0, The ranges of subplots are lower than μ-1σ, μ-1σ to μ-0.5σ, μ-0.5σ to μ, μ to μ+0.5σ, μ+0.5σ to μ+1σ, and higher than μ+1σ. Available only if len(x) is bigger than 2.
-
-        heat_extendsigma: float, optional
-            Set the axis view limits of the heatmap. The lower limit is min({x1, x2}) - std({x1, x2}) * ``heat_extendsigma``. The higher limit is max({x1, x2}) + std({x1, x2}) * ``heat_extendsigma``
-
-        heat_division: int, optional
-            Resolution of the heatmap.
-
-        color_extendsigma: float, optional
-            Set the colormap limits of the heatmap. The lower limit is min(y_ture) - std(y_ture) * ``color_extendsigma``. The higher limit is max(y_ture) - std(y_ture) * ``color_extendsigma``.
-
-        plot_scatter: {'error', 'true', 'hue'}, optional
-            Color decision of scatter plot. If 'error', to be mapped to colors using error value. If 'true', to be mapped to colors using y_ture value. If 'hue', to be mapped to colors using scatter_hue variable. If None, no scatter.
-
-        rounddigit_rank: int, optional
-            Round a number of error that are in the top posiotions for regression error to a given precision in decimal digits.
-
-        rounddigit_x1: int, optional
-            Round a number of x-axis valiable of the heatmap to a given precision in decimal digits.
-
-        rounddigit_x2: int, optional
-            Round a number of y-axis valiable of the heatmap to a given precision in decimal digits.
-
-        rounddigit_x3: int, optional
-            Round a number of y-axis valiable of subplots to a given precision in decimal digits.
-
-        rank_number: int, optional
-            Number of emphasized data that are in the top posiotions for regression error.
-
-        rank_col: str, optional
-            Variables that are displayed with emphasized data that are in the top posiotions for regression error.
-
-        cv : int, cross-validation generator, or an iterable, optional
-            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
-
-        cv_seed : int, optional
-            Seed for random number generator of cross validation.
-
-        cv_group: str, optional
-            Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
-
-        display_cv_indices : int or list, optional
-            Cross validation index or indices to display.
-
-        estimator_params : dict, optional
-            Parameters passed to the regression estimator. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
-
-        fit_params : dict, optional
-            Parameters passed to the fit() method of the regression estimator, e.g. ``early_stopping_round`` and ``eval_set`` of XGBRegressor. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
-
-        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
-
-            If "test", select test data from `X` and `y` using cv.split().
-
-            If "original", use raw `eval_set`.
-
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
-
-        subplot_kws: dict, optional
-            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
-
-        heat_kws: dict, optional
-            Additional parameters passed to sns.heatmap(), e.g. ``cmap``. See https://seaborn.pydata.org/generated/seaborn.heatmap.html
-
-        scatter_kws: dict, optional
-            Additional parameters passed to matplotlib.pyplot.scatter(), e.g. ``alpha``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.scatter.html
-
-        legend_kws : dict
-            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
-        """
-
-        # 入力データの形式統一
-        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data(x, y, data,
-                                                                                           x_colnames,
-                                                                                           cv_group)
-        # 説明変数xの次元が2～4以外ならエラーを出す
-        if len(x_colnames) < 2 or len(x_colnames) > 4:
-            raise Exception('Dimension of x must be 2 to 4')
-        
-        # display_cv_indicesをList化
-        if isinstance(display_cv_indices, int):
-            display_cv_indices = [display_cv_indices]
-        elif not isinstance(x_colnames, list):
-            raise Exception('the "cv_display_indices" argument must be int or List[int]')
-        # 学習器パラメータがあれば適用
-        if estimator_params is not None:
-            estimator.set_params(**estimator_params)
-        # 学習時パラメータがNoneなら空のdictを入力
-        if fit_params is None:
-            fit_params = {}
-        # subplot_kwsがNoneなら空のdictを入力
-        if subplot_kws is None:
-            subplot_kws = {}
-        # heat_kwsがNoneなら空のdictを入力
-        if heat_kws is None:
-            heat_kws = {}
-        # scatter_kwsがNoneなら空のdictを入力
-        if scatter_kws is None:
-            scatter_kws = {}
-        # legend_kwsがNoneなら空のdictを入力
-        if legend_kws is None:
-            legend_kws = {}
-        
-        # ヒートマップ表示用の列を抽出
-        if x_heat is None:  # 列名指定していないとき、前から2列を抽出
-            x_heat = x_colnames[:2]
-            x_heat_indices = [0, 1]
-        else:  # 列名指定しているとき、該当列のXにおけるインデックス(0～3)を保持
-            if len(x_heat) != 2:
-                raise Exception('length of x_heat must be 2')
-            x_heat_indices = []
-            for colname in x_heat:
-                x_heat_indices.append(x_colnames.index(colname))
-        # ヒートマップ表示以外の列
-        x_not_heat = [colname for colname in x_colnames if colname not in x_heat]        
-        # ヒートマップの色分け最大最小値(y_trueの最大最小値 ± y_trueの標準偏差 × color_extendsigma)
-        y_true_std = np.std(y_true)
-        vmin = np.min(y_true) - y_true_std * color_extendsigma
-        vmax = np.max(y_true) + y_true_std * color_extendsigma
-
-        # 引数plot_scatter='hue'とscatter_hueが同時指定されていないとき、エラーを出す
-        if scatter_hue is not None:
-            if plot_scatter != 'hue' and not isinstance(cv, GroupKFold) and not isinstance(cv, LeaveOneGroupOut):
-                raise Exception('the "plot_scatter" argument must be "hue" when the argument "scatter_hue" is not None')
-        elif plot_scatter == 'hue':
-            raise Exception('the "scatter_hue" argument is required when the argument "plot_scatter" is "hue"')
-        # 引数plot_scatter='hue'のとき、色分け対象列とカラーマップを紐づけ(色分けを全ての図で統一用)
-        if plot_scatter == 'hue':
-            hue_list = data[scatter_hue].values.tolist()
-            hue_list = sorted(set(hue_list), key=hue_list.index)
-            scatter_hue_dict = dict(zip(hue_list, cls._HEAT_SCATTER_HUECOLORS[0:len(hue_list)]))
-        else:
-            scatter_hue_dict = None
-        
-        # クロスバリデーション有無で場合分け
-        # クロスバリデーション未実施時(学習データからプロット＆指標算出)
-        if cv is None:
-            # 学習と推論
-            estimator.fit(X, y_true, **fit_params)
-            y_pred = estimator.predict(X)
-            # 誤差上位表示用データ取得
-            if rank_number is not None:
-                if rank_col is None:  # 表示フィールド指定ないとき、Index使用
-                    rank_col_data = data.index.values
-                else:  # 表示フィールド指定あるとき
-                    rank_col_data = data[rank_col].values
-            else:
-                rank_col_data = None
-            # 誤差最大値
-            maxerror = np.max(np.abs(y_pred - y_true))
-            # 散布図色分け用データ取得(plot_scatter='hue'のときのみ有効)
-            hue_data = data[scatter_hue] if scatter_hue is not None and plot_scatter=='hue' else None
-            hue_name = scatter_hue if scatter_hue is not None and plot_scatter=='hue' else None
-            # ヒートマップをプロット
-            cls._reg_heat_plot(estimator, X, y_pred, y_true, x_heat, x_not_heat, x_heat_indices, hue_data, hue_name,
-                               pair_sigmarange = pair_sigmarange, pair_sigmainterval=pair_sigmainterval, heat_extendsigma=heat_extendsigma, heat_division=heat_division,
-                               vmin=vmin, vmax=vmax, plot_scatter=plot_scatter, maxerror=maxerror,
-                               rank_number=rank_number, rank_col=rank_col, rank_col_data=rank_col_data, scatter_hue_dict=scatter_hue_dict,
-                               rounddigit_rank=rounddigit_rank, rounddigit_x1=rounddigit_x1, rounddigit_x2=rounddigit_x2, rounddigit_x3=rounddigit_x3,
-                               cv_index=None, subplot_kws=subplot_kws, heat_kws=heat_kws, scatter_kws=scatter_kws, legend_kws=legend_kws)
-            
-        # クロスバリデーション実施時(分割ごとに別々にプロット＆指標算出)
-        if cv is not None:
-            # 分割法未指定時、cv_numとseedに基づきKFoldでランダムに分割
-            if isinstance(cv, numbers.Integral):
-                cv = KFold(n_splits=cv, shuffle=True, random_state=cv_seed)
-            # LeaveOneOutのときエラーを出す
-            if isinstance(cv, LeaveOneOut):
-                raise Exception('"regression_heat_plot" method does not support "LeaveOneOut" cross validation')
-            # cv_groupをグルーピング対象に指定(GroupKFold、LeaveOneGroupOut等)
-            split_kws={}
-            if cv_group_colname is not None:
-                split_kws['groups'] = data[cv_group_colname].values
-            elif isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
-                raise Exception('"GroupKFold" and "LeaveOneGroupOut" cross validations need ``cv_group`` argument')
-            # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
-            if isinstance(cv, LeaveOneGroupOut):
-                cv_num = len(set(data[cv_group_colname].values))
-            else:
-                cv_num = cv.n_splits
-
-            # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
-            if eval_set_selection is None:
-                eval_set_selection = 'test'
-            fit_params, eval_set_selection = init_eval_set(
-                    eval_set_selection, fit_params, X, y)
-            # 最終学習器以外の前処理変換器作成
-            transformer = _make_transformer(eval_set_selection, estimator)
-
-            # クロスバリデーション
-            for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
-                # 表示対象以外のCVなら飛ばす
-                if i not in display_cv_indices:
-                    continue
-                print(f'cv_number={i}/{cv_num}')
-                # 表示用にテストデータと学習データ分割
-                X_train = X[train]
-                y_train = y_true[train]
-                X_test = X[test]
-                y_test = y_true[test]
-
-                # eval_setの中から学習データ or テストデータのみを抽出
-                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
-                                                        fit_params, train, test)
-
-                # 学習と推論
-                estimator.fit(X_train, y_train, **fit_params_modified)
-                y_pred = estimator.predict(X_test)
-                # 誤差上位表示用データ取得
-                if rank_number is not None:
-                    if rank_col is None:  # 表示フィールド指定ないとき、Index使用
-                        rank_col_test = data.index.values[test]
-                    else:  # 表示フィールド指定あるとき
-                        rank_col_test = data[rank_col].values[test]
-                else:
-                    rank_col_test = None
-                # 誤差最大値
-                maxerror = np.max(np.abs(y_pred - y_test))
-                # 散布図色分け用データ取得(plot_scatter='hue'のときのみ有効))
-                hue_data = data[scatter_hue].values[test] if scatter_hue is not None and plot_scatter=='hue' else None
-                hue_name = scatter_hue if scatter_hue is not None and plot_scatter=='hue' else None
-                # ヒートマップをプロット
-                cls._reg_heat_plot(estimator, X_test, y_pred, y_test, x_heat, x_not_heat, x_heat_indices, hue_data, hue_name,
-                                   pair_sigmarange = pair_sigmarange, pair_sigmainterval = pair_sigmainterval, heat_extendsigma=heat_extendsigma, heat_division=heat_division,
-                                   vmin=vmin, vmax=vmax, plot_scatter = plot_scatter, maxerror=maxerror,
-                                   rank_number=rank_number, rank_col=rank_col, rank_col_data=rank_col_test, scatter_hue_dict=scatter_hue_dict,
-                                   rounddigit_rank=rounddigit_rank, rounddigit_x1=rounddigit_x1, rounddigit_x2=rounddigit_x2, rounddigit_x3=rounddigit_x3,
-                                   cv_index=i, subplot_kws=subplot_kws, heat_kws=heat_kws, scatter_kws=scatter_kws, legend_kws=legend_kws)
+from typing import List, Dict
+import seaborn as sns
+import matplotlib.pyplot as plt
+import numbers
+import numpy as np
+import pandas as pd
+from scipy import stats
+from sklearn.linear_model import LinearRegression
+from sklearn.metrics import r2_score, mean_absolute_error, mean_squared_error, mean_squared_log_error, mean_absolute_percentage_error
+from sklearn.model_selection import KFold, LeaveOneOut, GroupKFold, LeaveOneGroupOut
+import decimal
+
+from ._cv_eval_set import init_eval_set, _make_transformer, _eval_set_selection, cross_val_score_eval_set
+
+class regplot():
+    # regression_heat_plotメソッド (回帰モデルヒートマップ表示)における、散布図カラーマップ
+    _HEAT_SCATTER_HUECOLORS = ['red', 'mediumblue', 'darkorange', 'darkmagenta', 'cyan',  'pink', 'brown', 'gold', 'grey']
+
+    def _round_digits(src: float, rounddigit: int = None, method='decimal'):
+        """
+        指定桁数で小数を丸める
+
+        Parameters
+        ----------
+        src : float
+            丸め対象の数値
+        rounddigit : int
+            フィッティング線の表示範囲（標準偏差の何倍まで表示するか指定）
+        method : int
+            桁数決定手法（'decimal':小数点以下, 'sig':有効数字(Decimal指定), 'format':formatで有効桁数指定）
+        """
+        if method == 'decimal':
+            return round(src, rounddigit)
+        elif method == 'sig':
+            with decimal.localcontext() as ctx:
+                ctx.prec = rounddigit
+                return ctx.create_decimal(src)
+        elif method == 'format':
+            return '{:.{width}g}'.format(src, width=rounddigit)
+    
+    @classmethod
+    def _round_dict_digits(cls, srcdict: Dict[str, float], rounddigit: int = None, method='decimal'):
+        """
+        指定桁数でdictの値を丸める
+
+        Parameters
+        ----------
+        srcdict : dict[str, float]
+            丸め対象のdict
+        rounddigit : int
+            フィッティング線の表示範囲（標準偏差の何倍まで表示するか指定）
+        method : int
+            桁数決定手法（'decimal':小数点以下, 'sig':有効数字(Decimal指定), 'format':formatで有効桁数指定）
+        """
+        dstdict = {}
+        for k, v in srcdict.items():
+            if rounddigit is not None and isinstance(v, float):
+                dstdict[k] = cls._round_digits(v, rounddigit=rounddigit, method=method)
+            else:
+                dstdict[k] = v
+        return dstdict
+
+    def _make_score_dict(y_true, y_pred, scores):
+        """
+        回帰評価指標を算出してdict化
+        """
+        score_dict = {}
+        for scoring in scores:
+            if scoring == 'r2':
+                score_dict['r2'] = r2_score(y_true, y_pred)
+            elif scoring == 'mae':
+                score_dict['mae'] = mean_absolute_error(y_true, y_pred)
+            elif scoring == 'mse':
+                score_dict['mse'] = mean_squared_error(y_true, y_pred, squared=True)
+            elif scoring == 'rmse':
+                score_dict['rmse'] = mean_squared_error(y_true, y_pred, squared=False)
+            elif scoring == 'rmsle':
+                score_dict['rmsle'] = mean_squared_log_error(y_true, y_pred)
+            elif scoring == 'mape':
+                score_dict['mape'] = mean_absolute_percentage_error(y_true, y_pred)
+            elif scoring == 'max_error':
+                score_dict['max_error'] = max([abs(p - r) for r, p in zip(y_true, y_pred)])
+        return score_dict
+
+    def _reshape_input_data(x, y, data, x_colnames, cv_group):
+        """
+        入力データの形式統一(pd.DataFrame or np.ndarray)
+        """
+        # dataがpd.DataFrameのとき
+        if isinstance(data, pd.DataFrame):
+            if not isinstance(x, list):
+                raise Exception('`x` argument should be list[str] if `data` is pd.DataFrame')
+            if not isinstance(y, str):
+                raise Exception('`y` argument should be str if `data` is pd.DataFrame')
+            if x_colnames is not None:
+                raise Exception('`x_colnames` argument should be None if `data` is pd.DataFrame')
+            X = data[x].values
+            y_true = data[y].values
+            x_colnames = x
+            y_colname = y
+            cv_group_colname = cv_group
+            
+        # dataがNoneのとき(x, y, cv_groupがnp.ndarray)
+        elif data is None:
+            if not isinstance(x, np.ndarray):
+                raise Exception('`x` argument should be np.ndarray if `data` is None')
+            if not isinstance(y, np.ndarray):
+                raise Exception('`y` argument should be np.ndarray if `data` is None')
+            X = x if len(x.shape) == 2 else x.reshape([x.shape[0], 1])
+            y_true = y.ravel()
+            # x_colnameとXの整合性確認
+            if x_colnames is None:
+                x_colnames = list(range(X.shape[1]))
+            elif X.shape[1] != len(x_colnames):
+                raise Exception('width of X must be equal to length of x_colnames')
+            else:
+                x_colnames = x_colnames
+            y_colname = 'objective_variable'
+            if cv_group is not None:  # cv_group指定時
+                cv_group_colname = 'group'
+                data = pd.DataFrame(np.column_stack((X, y_true, cv_group)),
+                                    columns=x_colnames + [y_colname] + [cv_group_colname])
+            else:
+                cv_group_colname = None
+                data = pd.DataFrame(np.column_stack((X, y)),
+                                    columns=x_colnames + [y_colname])
+        else:
+            raise Exception('`data` argument should be pd.DataFrame or None')
+
+        return X, y_true, data, x_colnames, y_colname, cv_group_colname
+
+    @classmethod
+    def _rank_display(cls, y_true, y_pred, rank_number, rank_col, rank_col_data, x=None, ax=None, rounddigit=None):
+        """
+        誤差上位を文字プロット
+
+        Parameters
+        ----------
+        y_true : np.ndarray
+            目的変数実測値
+        y_pred : np.ndarray
+            目的変数予測値
+        rank_number : int
+            誤差上位何番目までを文字表示するか
+        rank_col : List[str]
+            誤差上位と一緒に表示するフィールド名 (NoneならIndexを使用)
+        x : np.ndarray
+            説明変数の値 (Noneなら横軸y_true縦軸y_pred、Noneでなければ横軸x縦軸y_true)
+        ax : matplotlib.axes.Axes
+            表示対象のax（Noneならmatplotlib.pyplot.plotで1枚ごとにプロット）
+        rounddigit: int
+            表示指標の小数丸め桁数
+        """
+        # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
+        if ax is None:
+            ax=plt.gca()
+
+        if rank_col is None:
+            rank_col = 'index'
+        y_error = y_pred - y_true
+        y_error_abs = np.abs(y_error)
+        rank_index  = np.argsort(-y_error_abs)[:rank_number]
+        for rank, i in enumerate(rank_index):
+            error = cls._round_digits(y_error[i], rounddigit=rounddigit, method='decimal')
+            rank_text = f'      no{rank+1}\n-<-error={error}\n      {rank_col}={rank_col_data[i]}'
+            if x is None:  # 横軸y_true縦軸y_pred (regression_pred_trueメソッド用)
+                ax.text(y_true[i], y_pred[i], rank_text, verticalalignment='center', horizontalalignment='left')
+            else:  # 横軸x縦軸y_true (regression_plot_1dメソッド用)
+                ax.text(x[i], y_true[i], rank_text, verticalalignment='center', horizontalalignment='left')
+    
+    @classmethod
+    def _scatterplot_ndarray(cls, x, x_name, y, y_name, hue_data, hue_name, ax, scatter_kws, legend_kws):
+        """
+        np.ndarrayを入力として散布図表示(scatterplot)
+        """
+        # X値とY値を合体してDataFrame化
+        data = np.stack([x, y], axis=1)
+        data = pd.DataFrame(data, columns=[x_name, y_name])
+        # 色分け指定しているとき、色分け用のフィールドを追加
+        if hue_data is not None:
+            if hue_name is None:
+                hue_name = 'hue'
+            data[hue_name] = pd.Series(hue_data)
+        # 散布図プロット
+        sns.scatterplot(x=x_name, y=y_name, data=data, ax=ax, hue=hue_name, **scatter_kws)
+        # 凡例追加
+        if 'title' not in legend_kws.keys():
+            legend_kws['title'] = hue_name 
+        ax.legend(**legend_kws)
+
+    @classmethod
+    def _plot_pred_true(cls, y_true, y_pred, hue_data=None, hue_name=None, ax=None,
+                        linecolor='red', linesplit=200, rounddigit=None,
+                        score_dict=None, scatter_kws=None, legend_kws=None):
+        """
+        予測値と実測値を、回帰評価指標とともにプロット
+
+        Parameters
+        ----------
+        y_true : ndarray
+            目的変数実測値
+        y_pred : ndarray
+            目的変数予測値
+        hue_data : ndarray
+            色分け用ラベルデータ
+        hue_name : str
+            色分け用の列名
+        ax : matplotlib.axes.Axes
+            表示対象のax (Noneならmatplotlib.pyplot.plotで1枚ごとにプロット)
+        linecolor : str
+            予測値=実測値の線の色
+        linesplit : int
+            フィッティング線の分割数 (カクカクしたら増やす)
+        rounddigit: int
+            表示指標の小数丸め桁数
+        score_dict : dict[str, float]
+            算出した評価指標一覧
+        scatter_kws : dict
+            Additional parameters passed to sns.scatterplot(), e.g. ``alpha``. See https://seaborn.pydata.org/generated/seaborn.scatterplot.html
+        legend_kws : dict
+            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
+        """
+        # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
+        if ax is None:
+            ax=plt.gca()
+        # score_dictがNoneのとき、空のDictを加瀬宇
+        if score_dict is None:
+            score_dict = {}
+        # scatter_kwsがNoneなら空のdictを入力
+        if scatter_kws is None:
+            scatter_kws = {}
+        
+        # 散布図プロット
+        cls._scatterplot_ndarray(y_true, 'y_true', y_pred, 'y_pred', hue_data, hue_name, ax, scatter_kws, legend_kws)
+
+        # 予測値=実測値の線を作成
+        true_min = np.amin(y_true)
+        true_max = np.amax(y_true)
+        true_line = np.linspace(true_min, true_max, linesplit)
+        # 評価指標文字列作成
+        score_list = [f'{k}={v}' for k, v in cls._round_dict_digits(score_dict, rounddigit, 'sig').items()]
+        score_text = "\n".join(score_list)
+        # 線と文字をプロット
+        ax.plot(true_line, true_line, color=linecolor)
+        ax.text(true_max, np.amin(y_pred), score_text, verticalalignment='bottom', horizontalalignment='right')
+    
+    @classmethod
+    def regression_pred_true(cls, estimator, x: List[str], y: str, data: pd.DataFrame = None,
+                             x_colnames: List[str] = None, hue=None, linecolor='red', rounddigit=3,
+                             rank_number=None, rank_col=None, scores='mae', 
+                             cv_stats='mean', cv=None, cv_seed=42, cv_group=None, ax=None,
+                             estimator_params=None, fit_params=None, eval_set_selection=None,
+                             subplot_kws=None, scatter_kws=None, legend_kws=None):
+
+        """
+        Plot prediction vs. true scatter plots of any scikit-learn regression estimator
+
+        Parameters
+        ----------
+        estimator : estimator object implementing ``fit``
+            Regression estimator. This is assumed to implement the scikit-learn estimator interface.
+
+        x : str or list[str]
+            Explanatory variables.
+
+        y : str
+            Objective variable.
+
+        data : pd.DataFrame
+            Input data structure.
+
+        x_colnames: list[str], optional
+            Names of explanatory variables. Available only if ``data`` is NOT pd.DataFrame
+
+        hue : str, optional
+            Grouping variable that will produce points with different colors.
+
+        linecolor : str, optional
+            Color of prediction = true line. See https://matplotlib.org/stable/gallery/color/named_colors.html
+
+        rounddigit: int, optional
+            Round a number of score to a given precision in decimal digits.
+
+        rank_number : int, optional
+            Number of emphasized data that are in the top posiotions for regression error.
+
+        rank_col : list[str], optional
+            Variables that are displayed with emphasized data that are in the top posiotions for regression error.
+
+        scores : {'r2', 'mae', 'mse', 'rmse', 'rmsle', 'mape', 'max_error'} or list, optional
+            Regression score that are displayed at the lower right of the graph.
+
+        cv_stats : {'mean', 'median', 'max', 'min'}, optional
+            Statistical method of cross validation score that are displayed at the lower right of the graph.
+
+        cv : int, cross-validation generator, or an iterable, optional
+            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
+
+        cv_seed : int, optional
+            Seed for random number generator of cross validation.
+
+        cv_group: str, optional
+            Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
+
+        ax : {matplotlib.axes.Axes, list[matplotlib.axes.Axes]}, optional
+            Pre-existing axes for the plot or list of it. Otherwise, call matplotlib.pyplot.subplot() internally.
+
+        estimator_params : dict, optional
+            Parameters passed to the regression estimator. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
+
+        fit_params : dict, optional
+            Parameters passed to the fit() method of the regression estimator, e.g. ``early_stopping_round`` and ``eval_set`` of XGBRegressor. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
+
+        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
+            Select data passed to `eval_set` in `fit_params`. Available only if `estimator` is LightGBM or XGBoost and `cv` is not None.
+            
+            If "all", use all data in `X` and `y`.
+
+            If "train", select train data from `X` and `y` using cv.split().
+
+            If "test", select test data from `X` and `y` using cv.split().
+
+            If "original", use raw `eval_set`.
+
+            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+
+        subplot_kws : dict, optional
+            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. figsize. Available only if ``axes`` is None. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
+
+        scatter_kws: dict, optional
+            Additional parameters passed to sns.scatterplot(), e.g. ``alpha``. See https://seaborn.pydata.org/generated/seaborn.scatterplot.html
+
+        legend_kws : dict
+            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
+
+        Returns
+        ----------
+        score_dict : dict
+            Validation scores, e.g. r2, mae and rmse
+        """
+
+        # 入力データの形式統一
+        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data([x] if isinstance(x, str) else x, 
+                                                                                           y, data,
+                                                                                           x_colnames,
+                                                                                           cv_group)
+        # scoresの型をListに統一
+        if scores is None:
+            scores = []
+        elif isinstance(scores, str):
+            scores = [scores]
+        elif not isinstance(scores, list):
+            raise Exception('the "scores" argument must be str or list[str]')
+        # 学習器パラメータがあれば適用
+        if estimator_params is not None:
+            estimator.set_params(**estimator_params)
+        # 学習時パラメータがNoneなら空のdictを入力
+        if fit_params is None:
+            fit_params = {}
+        # subplot_kwsがNoneなら空のdictを入力
+        if subplot_kws is None:
+            subplot_kws = {}
+        # scatter_kwsがNoneなら空のdictを入力
+        if scatter_kws is None:
+            scatter_kws = {}
+        # legend_kwsがNoneなら空のdictを入力
+        if legend_kws is None:
+            legend_kws = {}
+        
+        # クロスバリデーション有無で場合分け
+        # クロスバリデーション未実施時(学習データからプロット＆指標算出)
+        if cv is None:
+            # 学習と推論
+            estimator.fit(X, y_true, **fit_params)
+            y_pred = estimator.predict(X)
+            # 評価指標算出
+            score_dict = cls._make_score_dict(y_true, y_pred, scores)
+            # 色分け用データ取得
+            hue_data = None if hue is None else data[hue]
+            hue_name = None if hue is None else hue
+            # 誤差上位表示用データ取得
+            if rank_number is not None:
+                if rank_col is None:  # 表示フィールド指定ないとき、Index使用
+                    rank_col_data = data.index.values
+                else:  # 表示フィールド指定あるとき
+                    rank_col_data = data[rank_col].values
+            # 予測値と実測値プロット
+            cls._plot_pred_true(y_true, y_pred, hue_data=hue_data, hue_name=hue_name, ax=ax,
+                                linecolor=linecolor, rounddigit=rounddigit, score_dict=score_dict,
+                                scatter_kws=scatter_kws, legend_kws=legend_kws)
+            # 誤差上位を文字表示
+            if rank_number is not None:
+                cls._rank_display(y_true, y_pred, rank_number, rank_col, rank_col_data, rounddigit=rounddigit)
+            return score_dict
+            
+        # クロスバリデーション実施時(分割ごとに別々にプロット＆指標算出)
+        if cv is not None:
+            # 分割法未指定時、cv_numとseedに基づきKFoldでランダムに分割
+            if isinstance(cv, numbers.Integral):
+                cv = KFold(n_splits=cv, shuffle=True, random_state=cv_seed)
+            #LeaveOneOutかどうかを判定
+            isLeaveOneOut = isinstance(cv, LeaveOneOut)
+            # cv_groupをグルーピング対象に指定(GroupKFold、LeaveOneGroupOut等)
+            split_kws={}
+            if cv_group_colname is not None:
+                split_kws['groups'] = data[cv_group_colname].values
+            elif isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
+                raise Exception('"GroupKFold" and "LeaveOneGroupOut" cross validations need ``cv_group`` argument')
+            # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
+            if isinstance(cv, LeaveOneGroupOut):
+                cv_num = len(set(data[cv_group_colname].values))
+            elif isLeaveOneOut:
+                cv_num = 1
+            else:
+                cv_num = cv.n_splits
+
+            # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
+            if eval_set_selection is None:
+                eval_set_selection = 'test'
+            fit_params, eval_set_selection = init_eval_set(
+                    eval_set_selection, fit_params, X, y)
+            # 最終学習器以外の前処理変換器作成
+            transformer = _make_transformer(eval_set_selection, estimator)
+
+            # スコア種類ごとにクロスバリデーションスコアの算出
+            score_all_dict = {}
+            for scoring in scores:
+                # cross_val_scoreでクロスバリデーション
+                if scoring == 'r2':
+                    score_all_dict['r2'] = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                                                    cv=cv, scoring='r2',
+                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
+                elif scoring == 'mae':
+                    neg_mae = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                                                    cv=cv, scoring='neg_mean_absolute_error',
+                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
+                    score_all_dict['mae'] = -neg_mae  # scikit-learnの仕様に合わせ正負を逆に
+                elif scoring == 'mse':
+                    neg_mse = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                                                    cv=cv, scoring='neg_mean_squared_error',
+                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
+                    score_all_dict['mse'] = -neg_mse  # scikit-learnの仕様に合わせ正負を逆に
+                elif scoring == 'rmse':
+                    neg_rmse = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                                                    cv=cv, scoring='neg_root_mean_squared_error',
+                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
+                    score_all_dict['rmse'] = -neg_rmse  # scikit-learnの仕様に合わせ正負を逆に
+                elif scoring == 'rmsle':
+                    neg_msle = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true, 
+                                                    cv=cv, scoring='neg_mean_squared_log_error',
+                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
+                    score_all_dict['rmsle'] = np.sqrt(-neg_msle)  # 正負を逆にしてルートをとる
+                elif scoring == 'mape':
+                    neg_mape = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                                                    cv=cv, scoring='neg_mean_absolute_percentage_error',
+                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
+                    score_all_dict['mape'] = -neg_mape  # scikit-learnの仕様に合わせ正負を逆に
+                elif scoring == 'max_error':
+                    neg_max_error = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                                                    cv=cv, scoring='max_error',
+                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
+                    score_all_dict['max_error'] = - neg_max_error  # scikit-learnの仕様に合わせ正負を逆に
+            
+            # 表示用のax作成
+            if ax is None:
+                # LeaveOneOutのとき、クロスバリデーションごとの図は作成せず
+                if isLeaveOneOut:
+                    if 'figsize' not in subplot_kws.keys():
+                        subplot_kws['figsize'] = (6, 6)
+                    fig, ax = plt.subplots(1, 1, **subplot_kws)
+                # LeaveOneOut以外のとき、クロスバリデーションごとに図作成
+                else:
+                    if 'figsize' not in subplot_kws.keys():
+                        subplot_kws['figsize'] = (6, (cv_num + 1) * 6)
+                    fig, ax = plt.subplots(cv_num + 1, 1, **subplot_kws)
+
+            # クロスバリデーション
+            y_true_all = []
+            y_pred_all = []
+            hue_all = []
+            rank_col_all = []
+            score_train_dict = {}
+            for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
+                # 表示用にテストデータと学習データ分割
+                X_train = X[train]
+                y_train = y_true[train]
+                X_test = X[test]
+                y_test = y_true[test]
+                # 色分け用データ取得(していないときは、クロスバリデーション番号を使用、LeaveOuneOutのときは番号分けない)
+                if hue is None:
+                    hue_test = np.full(1 ,'leave_one_out') if isLeaveOneOut else np.full(len(test) ,f'cv_{i}')
+                    hue_name = 'cv_number'  # 色分け名を'cv_number'に指定
+                else:
+                    hue_test = data[hue].values[test]
+                    hue_name = hue
+                # 誤差上位表示用データ取得
+                if rank_number is not None:
+                    if rank_col is None:  # 表示フィールド指定ないとき、Index使用
+                        rank_col_test = data.index.values[test]
+                    else:  # 表示フィールド指定あるとき
+                        rank_col_test = data[rank_col].values[test]
+                else:
+                    rank_col_test = np.array([])
+
+                # eval_setの中から学習データ or テストデータのみを抽出
+                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
+                                                        fit_params, train, test)
+
+                # 学習と推論
+                estimator.fit(X_train, y_train, **fit_params_modified)
+                y_pred = estimator.predict(X_test)
+                # 学習データスコア算出
+                y_pred_train = estimator.predict(X_train)
+                score_dict = cls._make_score_dict(y_train, y_pred_train, scores)
+                for score in scores:
+                    if f'{score}_train' not in score_train_dict:
+                        score_train_dict[f'{score}_train'] = []
+                    score_train_dict[f'{score}_train'].append(score_dict[score])
+                # CV内結果をプロット(LeaveOneOutのときはプロットしない)
+                if not isLeaveOneOut:
+                    score_cv_dict = {k: v[i] for k, v in score_all_dict.items()}
+                    score_cv_dict.update({f'{k}_train': v for k, v in score_dict.items()})
+                    cls._plot_pred_true(y_test, y_pred, hue_data=hue_test, hue_name=hue_name, ax=ax[i],
+                                        linecolor=linecolor, rounddigit=rounddigit, score_dict=score_cv_dict,
+                                        scatter_kws=scatter_kws, legend_kws=legend_kws)
+                    ax[i].set_title(f'Cross Validation Fold{i}')
+                # 全体プロット用データに追加
+                y_true_all.append(y_test)
+                y_pred_all.append(y_pred)
+                hue_all.append(hue_test)
+                rank_col_all.append(rank_col_test)
+
+            # 全体プロット用データを合体
+            y_true_all = np.hstack(y_true_all)
+            y_pred_all = np.hstack(y_pred_all)
+            hue_all = np.hstack(hue_all)
+            rank_col_all = np.hstack(rank_col_all)
+            # スコアの統計値を計算
+            if cv_stats == 'mean':
+                score_stats_dict = {f'{k}_mean': np.mean(v) for k, v in score_all_dict.items()}
+                train_stats_dict = {k: np.mean(v) for k, v in score_train_dict.items()}
+            elif cv_stats == 'median':
+                score_stats_dict = {f'{k}_median': np.median(v) for k, v in score_all_dict.items()}
+                train_stats_dict = {k: np.median(v) for k, v in score_train_dict.items()}
+            elif cv_stats == 'min':
+                score_stats_dict = {f'{k}_min': np.amin(v) for k, v in score_all_dict.items()}
+                train_stats_dict = {k: np.amin(v) for k, v in score_train_dict.items()}
+            elif cv_stats == 'max':
+                score_stats_dict = {f'{k}_max': np.amax(v) for k, v in score_all_dict.items()}
+                train_stats_dict = {k: np.amax(v) for k, v in score_train_dict.items()}
+            # 学習データスコアをdictに追加
+            score_stats_dict.update(train_stats_dict)
+            # 全体プロット
+            ax_all = ax if isLeaveOneOut else ax[cv_num]
+            cls._plot_pred_true(y_true_all, y_pred_all, hue_data=hue_all, hue_name=hue_name, ax=ax_all,
+                               linecolor=linecolor, rounddigit=rounddigit, score_dict=score_stats_dict,
+                               scatter_kws=scatter_kws, legend_kws=legend_kws)
+            ax_all.set_title('All Cross Validations')
+            # 誤差上位を文字表示
+            if rank_number is not None:
+                cls._rank_display(y_true_all, y_pred_all, rank_number, rank_col, rank_col_all,
+                                  ax=ax_all, rounddigit=rounddigit)
+            return score_stats_dict
+    
+    def _average_plot(estimator, data, x_colnames, y_colname, hue,
+                      aggregate, subplot_kws, plot_kws, scatter_kws, legend_kws,
+                      cv_index, x_range=200):
+        # figsize (全ての図全体のサイズ)指定
+        if 'figsize' not in subplot_kws.keys():
+            subplot_kws['figsize'] = (6, len(x_colnames) * 5)
+        if 'color' not in plot_kws:
+            plot_kws['color'] = 'red'
+        # プロット用のaxes作成
+        fig, axes = plt.subplots(len(x_colnames), 1, **subplot_kws)
+        if cv_index is not None:
+            fig.suptitle(f'CV No.{cv_index}')
+        # 全列を走査
+        for i, colname in enumerate(x_colnames):
+            # 該当列（グラフのX軸）の値を作成
+            x_max = data[colname].max()
+            x_min = data[colname].min()
+            x_array = np.linspace(x_min, x_max, x_range)
+            # 該当列以外を抽出して平均値算出
+            if aggregate == 'mean':
+                other_x_agg = data[[col for col in x_colnames if col != colname]].mean()
+            elif aggregate == 'median':
+                other_x_agg = data[[col for col in x_colnames if col != colname]].median()
+            else:
+                raise ValueError('the `aggregate` argument should be "mean" or "median"')
+            X_mean = np.tile(other_x_agg, (x_range, 1))
+            # 該当列を挿入して説明変数とし、モデルで推論
+            X_mean = np.insert(X_mean, i, x_array, axis=1)
+            y_pred = estimator.predict(X_mean)
+            # 実測値を散布図プロット
+            ax = axes if len(x_colnames) == 1 else axes[i]
+            sns.scatterplot(x=colname, y=y_colname, hue=hue, data=data, ax=ax, **scatter_kws)
+            # 推測値曲線をプロット
+            ax.plot(x_array, y_pred, **plot_kws)
+            # 色分け時は凡例表示
+            if hue is not None:
+                ax.legend(**legend_kws)
+
+        fig.tight_layout(rect=[0, 0, 1, 0.98])          
+
+
+    @classmethod
+    def average_plot(cls, estimator, x: List[str], y: str, data: pd.DataFrame = None,
+                     x_colnames: List[str] = None, hue=None,
+                     aggregate='mean',
+                     cv=None, cv_seed=42, cv_group=None, display_cv_indices = 0,
+                     estimator_params=None, fit_params=None, eval_set_selection=None,
+                     subplot_kws=None, plot_kws=None, scatter_kws=None, legend_kws=None):
+        """
+        Plot relationship between one explanatory variable and predicted value by line graph.
+
+        Other explanatory variables are fixed to aggregated values such as mean values or median values.
+
+        Parameters
+        ----------
+        estimator : estimator object implementing ``fit``
+            Regression estimator. This is assumed to implement the scikit-learn estimator interface.
+        x : list[str] or np.ndarray
+            Explanatory variables. Should be list[str] if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
+
+        y : str or np.ndarray
+            Objective variable. Should be str if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
+
+        data: pd.DataFrame
+            Input data structure.
+
+        x_colnames: list[str], optional
+            Names of explanatory variables. Available only if ``data`` is NOT pd.DataFrame
+
+        hue : str, optional
+            Grouping variable that will produce points with different colors.
+
+        aggregate : {'mean', 'median'}, optional
+            Statistic method of aggregating explanatory variables except x_axis variable.
+
+        cv : int, cross-validation generator, or an iterable, optional
+            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
+
+        cv_seed : int, optional
+            Seed for random number generator of cross validation.
+
+        cv_group: str, optional
+            Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
+
+        display_cv_indices : int or list, optional
+            Cross validation index or indices to display.
+
+        estimator_params : dict, optional
+            Parameters passed to the regression estimator. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
+
+        fit_params : dict, optional
+            Parameters passed to the fit() method of the regression estimator, e.g. ``early_stopping_round`` and ``eval_set`` of XGBRegressor. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
+        
+        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
+            Select data passed to `eval_set` in `fit_params`. Available only if `estimator` is LightGBM or XGBoost and `cv` is not None.
+            
+            If "all", use all data in `X` and `y`.
+
+            If "train", select train data from `X` and `y` using cv.split().
+
+            If "test", select test data from `X` and `y` using cv.split().
+
+            If "original", use raw `eval_set`.
+
+            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+
+        subplot_kws: dict, optional
+            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
+
+        plot_kws: dict, optional
+            Additional parameters passed to matplotlib.axes.Axes.plot(), e.g. ``alpha``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.plot.html
+
+        scatter_kws: dict, optional
+            Additional parameters passed to seaborn.scatterplot(), e.g. ``alpha``. See https://seaborn.pydata.org/generated/seaborn.scatterplot.html
+
+        legend_kws : dict
+            Additional parameters passed to matplotlib.axes.Axes.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
+        """
+
+        # 入力データの形式統一
+        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data(x, y, data,
+                                                                                           x_colnames,
+                                                                                           cv_group)
+        
+        # display_cv_indicesをList化
+        if isinstance(display_cv_indices, int):
+            display_cv_indices = [display_cv_indices]
+        elif not isinstance(x_colnames, list):
+            raise Exception('the "cv_display_indices" argument should be int or List[int]')
+        # 学習器パラメータがあれば適用
+        if estimator_params is not None:
+            estimator.set_params(**estimator_params)
+        # 学習時パラメータがNoneなら空のdictを入力
+        if fit_params is None:
+            fit_params = {}
+        # subplot_kwsがNoneなら空のdictを入力
+        if subplot_kws is None:
+            subplot_kws = {}
+        # plot_kwsがNoneなら空のdictを入力
+        if plot_kws is None:
+            plot_kws = {}
+        # scatter_kwsがNoneなら空のdictを入力
+        if scatter_kws is None:
+            scatter_kws = {}
+        # legend_kwsがNoneなら空のdictを入力
+        if legend_kws is None:
+            legend_kws = {}
+        
+        # クロスバリデーション有無で場合分け
+        # クロスバリデーション未実施時(学習データからプロット＆指標算出)
+        if cv is None:
+            # 学習と推論
+            estimator.fit(X, y_true, **fit_params)
+            # 平均値
+            cls._average_plot(estimator, data, x_colnames, y_colname, hue,
+                              aggregate=aggregate,
+                              subplot_kws=subplot_kws, plot_kws=plot_kws,
+                              scatter_kws=scatter_kws, legend_kws=legend_kws,
+                              cv_index=None)
+            
+        # クロスバリデーション実施時(分割ごとに別々にプロット＆指標算出)
+        if cv is not None:
+            # 分割法未指定時、cv_numとseedに基づきKFoldでランダムに分割
+            if isinstance(cv, numbers.Integral):
+                cv = KFold(n_splits=cv, shuffle=True, random_state=cv_seed)
+            # LeaveOneOutのときエラーを出す
+            if isinstance(cv, LeaveOneOut):
+                raise Exception('"regression_heat_plot" method does not support "LeaveOneOut" cross validation')
+            # cv_groupをグルーピング対象に指定(GroupKFold、LeaveOneGroupOut等)
+            split_kws={}
+            if cv_group_colname is not None:
+                split_kws['groups'] = data[cv_group_colname].values
+            elif isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
+                raise Exception('"GroupKFold" and "LeaveOneGroupOut" cross validations need ``cv_group`` argument')
+            # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
+            if isinstance(cv, LeaveOneGroupOut):
+                cv_num = len(set(data[cv_group_colname].values))
+            else:
+                cv_num = cv.n_splits
+
+            # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
+            if eval_set_selection is None:
+                eval_set_selection = 'test'
+            fit_params, eval_set_selection = init_eval_set(
+                    eval_set_selection, fit_params, X, y)
+            # 最終学習器以外の前処理変換器作成
+            transformer = _make_transformer(eval_set_selection, estimator)
+
+            # クロスバリデーション
+            for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
+                # 表示対象以外のCVなら飛ばす
+                if i not in display_cv_indices:
+                    continue
+                print(f'cv_number={i}/{cv_num}')
+                # 表示用にテストデータと学習データ分割
+                X_train = X[train]
+                y_train = y_true[train]
+                data_test = data.iloc[test]
+                
+                # eval_setの中から学習データ or テストデータのみを抽出
+                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
+                                                        fit_params, train, test)
+
+                # 学習と推論
+                estimator.fit(X_train, y_train, **fit_params_modified)
+                # ヒートマップをプロット
+                cls._average_plot(estimator, data_test, x_colnames, y_colname, hue,
+                                  aggregate=aggregate,
+                                  subplot_kws=subplot_kws, plot_kws=plot_kws,
+                                  scatter_kws=scatter_kws, legend_kws=legend_kws,
+                                  cv_index=i)
+
+        
+    @classmethod
+    def linear_plot(cls, x: str, y: str, data: pd.DataFrame = None,
+                    x_colname: str = None,
+                    ax=None, hue=None, linecolor='red',
+                    rounddigit=5, plot_scores=True, scatter_kws=None, legend_kws=None):
+        """
+        Plot linear regression line and calculate Pearson correlation coefficient.
+
+        Parameters
+        ----------
+        x : str
+            Variable that specify positions on the x.
+
+        y : str
+            Variable that specify positions on the y.
+
+        data : pd.DataFrame
+            Input data structure.
+
+        x_colname: str, optional
+            Names of explanatory variable. Available only if ``data`` is NOT pd.DataFrame
+
+        ax : matplotlib.axes.Axes, optional
+            Pre-existing axes for the plot. Otherwise, call matplotlib.pyplot.gca() internally.
+
+        hue : str, optional
+            Grouping variable that will produce points with different colors.
+
+        linecolor : str, optional
+            Color of regression line. See https://matplotlib.org/stable/gallery/color/named_colors.html
+
+        rounddigit: int, optional
+            Round a number of score to a given precision in decimal digits.
+
+        plot_scores: bool, optional
+            If True, display Pearson correlation coefficient and the p-value.
+
+        scatter_kws: dict, optional
+            Additional parameters passed to sns.scatterplot(), e.g. ``alpha``. See https://seaborn.pydata.org/generated/seaborn.scatterplot.html
+
+        legend_kws : dict
+            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
+
+        Returns
+        ----------
+        ax : matplotlib.axes.Axes
+            Returns the Axes object with the plot drawn onto it.
+        """
+
+        # 入力データの形式統一
+        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data([x] if isinstance(x, str) else x, 
+                                                                                           y, data,
+                                                                                           [x_colname] if x_colname is not None else x_colname,
+                                                                                           cv_group=None)
+        if x_colname is None:
+            x_colname = x_colnames[0]
+        # scatter_kwsがNoneなら空のdictを入力
+        if scatter_kws is None:
+            scatter_kws = {}
+        # legend_kwsがNoneなら空のdictを入力
+        if legend_kws is None:
+            legend_kws = {}
+
+        # まずは散布図プロット
+        ax = sns.scatterplot(x=x_colname, y=y_colname, data=data, ax=ax, hue=hue, **scatter_kws)
+        # 凡例追加
+        if hue is not None and 'title' not in legend_kws.keys():
+            legend_kws['title'] = hue
+        if len(legend_kws.keys()) > 0:
+            ax.legend(**legend_kws)
+
+        # 線形回帰モデル作成
+        lr = LinearRegression()
+        lr.fit(X, y_true)
+        xmin = np.amin(X)
+        xmax = np.amax(X)
+        linesplit=200
+        Xline = np.linspace(xmin, xmax, linesplit)
+        Xline = Xline.reshape(len(Xline), 1)
+        # 回帰線を描画
+        ax.plot(Xline, lr.predict(Xline), color=linecolor)
+
+        # 回帰式、ピアソンの相関係数およびp値を表示
+        if plot_scores == True:
+            # 回帰式
+            coef = cls._round_digits(lr.coef_[0], rounddigit=rounddigit, method="decimal")
+            intercept = cls._round_digits(lr.intercept_, rounddigit=rounddigit, method="decimal")
+            equation = f'y={coef}x+{intercept}' if intercept >= 0 else f'y={coef}x-{-intercept}'
+            # ピアソン相関係数
+            pearsonr = stats.pearsonr(data[x_colname], data[y_colname])
+            r = cls._round_digits(pearsonr[0], rounddigit=rounddigit, method="decimal")
+            pvalue = cls._round_digits(pearsonr[1], rounddigit=rounddigit, method="decimal")            
+            # プロット
+            rtext = f'{equation}\nr={r}\np={pvalue}'
+            ax.text(xmax, np.amin(y_true), rtext, verticalalignment='bottom', horizontalalignment='right')
+
+        return ax
+
+    @classmethod
+    def _estimator_plot_1d(cls, trained_estimator, X, y_true, hue_data=None, hue_name=None, ax=None, linecolor='red', linesplit=1000, rounddigit=None,
+                       score_dict=None, scatter_kws=None, legend_kws=None):
+        """
+        1次説明変数回帰曲線を、回帰評価指標とともにプロット
+
+        Parameters
+        ----------
+        trained_estimator : 
+            学習済の回帰モデル(scikit-learn API)
+
+        X : ndarray
+            説明変数
+
+        y_true : ndarray
+            目的変数実測値
+
+        hue_data : ndarray
+            色分け用ラベルデータ
+
+        hue_name : str
+            色分け用の列名
+
+        ax : matplotlib.axes.Axes
+            表示対象のax (Noneならplt.plotで1枚ごとにプロット)
+
+        linecolor : str
+            予測値=実測値の線の色
+
+        linesplit : int
+            フィッティング線の分割数 (カクカクしたら増やす)
+
+        rounddigit: int
+            表示指標の小数丸め桁数
+
+        score_dict : dict[str, float]
+            算出した評価指標一覧
+
+        scatter_kws: dict, optional
+            Additional parameters passed to sns.scatterplot(), e.g. ``alpha``. See https://seaborn.pydata.org/generated/seaborn.scatterplot.html
+
+        legend_kws : dict
+            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
+        """
+        # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
+        if ax is None:
+            ax=plt.gca()
+        # score_dictがNoneのとき、空のDictを入力
+        if score_dict is None:
+            score_dict = {}
+        # scatter_kwsがNoneなら空のdictを入力
+        if scatter_kws is None:
+            scatter_kws = {}
+        # legend_kwsがNoneなら空のdictを入力
+        if legend_kws is None:
+            legend_kws = {}
+        
+        # 散布図プロット
+        cls._scatterplot_ndarray(np.ravel(X), 'X', y_true, 'Y', hue_data, hue_name, ax, scatter_kws, legend_kws)
+
+        # 回帰モデルの線を作成
+        xmin = np.amin(X)
+        xmax = np.amax(X)
+        Xline = np.linspace(xmin, xmax, linesplit)
+        Xline = Xline.reshape(len(Xline), 1)
+        # 回帰線を描画
+        ax.plot(Xline, trained_estimator.predict(Xline), color=linecolor)
+        
+        # 評価指標文字列作成
+        score_list = [f'{k}={v}' for k, v in cls._round_dict_digits(score_dict, rounddigit, 'sig').items()]
+        score_text = "\n".join(score_list)
+        ax.text(xmax, np.amin(y_true), score_text, verticalalignment='bottom', horizontalalignment='right')
+
+    @classmethod
+    def regression_plot_1d(cls, estimator, x: str, y: str, data: pd.DataFrame = None, x_colname: str = None,
+                           hue=None, linecolor='red', rounddigit=3,
+                           rank_number=None, rank_col=None, scores='mae',
+                           cv_stats='mean', cv=None, cv_seed=42, cv_group=None,
+                           estimator_params=None, fit_params=None, eval_set_selection=None,
+                           subplot_kws=None, scatter_kws=None, legend_kws=None):
+        """
+        Plot regression lines of any scikit-learn regressor with 1D explanatory variable.
+
+        Parameters
+        ----------
+        estimator : estimator object implementing ``fit``
+            Regression estimator. This is assumed to implement the scikit-learn estimator interface.
+
+        x : str, or np.ndarray
+            Explanatory variables. Should be str if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
+
+        y : str or np.ndarray
+            Objective variable. Should be str if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
+
+        data: pd.DataFrame
+            Input data structure.
+
+        x_colname: str, optional
+            Names of explanatory variable. Available only if ``data`` is NOT pd.DataFrame
+
+        hue : str, optional
+            Grouping variable that will produce points with different colors.
+
+        linecolor : str, optional
+            Color of prediction = true line. See https://matplotlib.org/stable/gallery/color/named_colors.html
+
+        rounddigit: int, optional
+            Round a number of score to a given precision in decimal digits.
+
+        rank_number : int, optional
+            Number of emphasized data that are in the top positions for regression error.
+
+        rank_col : list[str], optional
+            Variables that are displayed with emphasized data that are in the top posiotions for regression error.
+
+        scores : {'r2', 'mae', 'mse', 'rmse', 'rmsle', 'mape', 'max_error'} or list,, optional
+            Regression score that are displayed at the lower right of the graph.
+
+        cv_stats : {'mean', 'median', 'max', 'min'}, optional
+            Statistical method of cross validation score that are displayed at the lower right of the graph.
+
+        cv : int, cross-validation generator, or an iterable, optional
+            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
+
+        cv_seed : int, optional
+            Seed for random number generator of cross validation.
+
+        cv_group: str, optional
+            Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
+
+        estimator_params : dict, optional
+            Parameters passed to the regression estimator. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
+
+        fit_params : dict, optional
+            Parameters passed to the fit() method of the regression estimator, e.g. ``early_stopping_round`` and ``eval_set`` of XGBRegressor. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
+
+        subplot_kws : dict, optional
+            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
+
+        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
+            
+            If "all", use all data in `X` and `y`.
+
+            If "train", select train data from `X` and `y` using cv.split().
+
+            If "test", select test data from `X` and `y` using cv.split().
+
+            If "original", use raw `eval_set`.
+
+            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+
+        scatter_kws: dict, optional
+            Additional parameters passed to sns.scatterplot(), e.g. ``alpha``. See https://seaborn.pydata.org/generated/seaborn.scatterplot.html
+
+        legend_kws : dict
+            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
+
+        Returns
+        ----------
+        score_dict : dict
+            Validation scores, e.g. r2, mae and rmse
+        """
+
+        # 入力データの形式統一
+        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data([x] if isinstance(x, str) else x,
+                                                                                           y, data,
+                                                                                           [x_colname] if x_colname is not None else x_colname,
+                                                                                           cv_group)
+        # scoresの型をListに統一
+        if scores is None:
+            scores = []
+        elif isinstance(scores, str):
+            scores = [scores]
+        elif not isinstance(scores, list):
+            raise Exception('the "scores" argument must be str or list[str]')
+        # 学習器パラメータがあれば適用
+        if estimator_params is not None:
+            estimator.set_params(**estimator_params)
+        # 学習時パラメータがNoneなら空のdictを入力
+        if fit_params is None:
+            fit_params = {}
+        # subplot_kwsがNoneなら空のdictを入力
+        if subplot_kws is None:
+            subplot_kws = {}
+        # scatter_kwsがNoneなら空のdictを入力
+        if scatter_kws is None:
+            scatter_kws = {}
+        # legend_kwsがNoneなら空のdictを入力
+        if legend_kws is None:
+            legend_kws = {}
+        
+        # クロスバリデーション有無で場合分け
+        # クロスバリデーション未実施時(学習データからプロット＆指標算出)
+        if cv is None:
+            # 学習と推論
+            estimator.fit(X, y_true, **fit_params)
+            y_pred = estimator.predict(X)
+            # 評価指標算出
+            score_dict = cls._make_score_dict(y_true, y_pred, scores)
+            # 色分け用データ取得
+            hue_data = None if hue is None else data[hue]
+            hue_name = None if hue is None else hue
+            # 誤差上位表示用データ取得
+            if rank_number is not None:
+                if rank_col is None:  # 表示フィールド指定ないとき、Index使用
+                    rank_col_data = data.index.values
+                else:  # 表示フィールド指定あるとき
+                    rank_col_data = data[rank_col].values
+            # 回帰線プロット
+            cls._estimator_plot_1d(estimator, X, y_true, hue_data=hue_data, hue_name=hue_name,
+                               linecolor=linecolor, rounddigit=rounddigit, score_dict=score_dict,
+                               scatter_kws=scatter_kws, legend_kws=legend_kws)
+            # 誤差上位を文字表示
+            if rank_number is not None:
+                cls._rank_display(y_true, y_pred, rank_number, rank_col, rank_col_data, x=X, rounddigit=rounddigit)
+            return score_dict
+            
+        # クロスバリデーション実施時(分割ごとに別々にプロット＆指標算出)
+        if cv is not None:
+            # 分割法未指定時、cv_numとseedに基づきKFoldでランダムに分割
+            if isinstance(cv, numbers.Integral):
+                cv = KFold(n_splits=cv, shuffle=True, random_state=cv_seed)
+            #LeaveOneOutのときエラーを出す
+            if isinstance(cv, LeaveOneOut):
+                raise Exception('"regression_plot_1d" method does not support "LeaveOneOut" cross validation')
+            # cv_groupをグルーピング対象に指定(GroupKFold、LeaveOneGroupOut等)
+            split_kws={}
+            if cv_group_colname is not None:
+                split_kws['groups'] = data[cv_group_colname].values
+            elif isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
+                raise Exception('"GroupKFold" and "LeaveOneGroupOut" cross validations need ``cv_group`` argument')
+            # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
+            if isinstance(cv, LeaveOneGroupOut):
+                cv_num = len(set(data[cv_group_colname].values))
+            else:
+                cv_num = cv.n_splits
+
+            # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
+            if eval_set_selection is None:
+                eval_set_selection = 'test'
+            fit_params, eval_set_selection = init_eval_set(
+                    eval_set_selection, fit_params, X, y)
+            # 最終学習器以外の前処理変換器作成
+            transformer = _make_transformer(eval_set_selection, estimator)
+
+            # スコア種類ごとにクロスバリデーションスコアの算出
+            score_all_dict = {}
+            for scoring in scores:
+                # cross_val_scoreでクロスバリデーション
+                if scoring == 'r2':
+                    score_all_dict['r2'] = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true, 
+                                                    cv=cv, scoring='r2',
+                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
+                elif scoring == 'mae':
+                    neg_mae = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true, 
+                                                    cv=cv, scoring='neg_mean_absolute_error',
+                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
+                    score_all_dict['mae'] = -neg_mae  # scikit-learnの仕様に合わせ正負を逆に
+                elif scoring == 'mse':
+                    neg_mse = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                                                    cv=cv, scoring='neg_mean_squared_error',
+                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
+                    score_all_dict['mse'] = -neg_mse  # scikit-learnの仕様に合わせ正負を逆に
+                elif scoring == 'rmse':
+                    neg_rmse = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                                                    cv=cv, scoring='neg_root_mean_squared_error',
+                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
+                    score_all_dict['rmse'] = -neg_rmse  # scikit-learnの仕様に合わせ正負を逆に
+                elif scoring == 'rmsle':
+                    neg_msle = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                                                    cv=cv, scoring='neg_mean_squared_log_error',
+                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
+                    score_all_dict['rmsle'] = np.sqrt(-neg_msle)  # 正負を逆にしてルートをとる
+                elif scoring == 'mape':
+                    neg_mape = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                                                    cv=cv, scoring='neg_mean_absolute_percentage_error',
+                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
+                    score_all_dict['mape'] = -neg_mape  # scikit-learnの仕様に合わせ正負を逆に
+                elif scoring == 'max_error':
+                    neg_max_error = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                                                    cv=cv, scoring='max_error',
+                                                    fit_params=fit_params, n_jobs=-1, **split_kws)
+                    score_all_dict['max_error'] = - neg_max_error  # scikit-learnの仕様に合わせ正負を逆に
+            
+            # 表示用のaxes作成
+            # クロスバリデーションごとに図作成
+            if 'figsize' not in subplot_kws.keys():
+                subplot_kws['figsize'] = (6, (cv_num + 1) * 6)
+            fig, axes = plt.subplots(cv_num + 1, 1, **subplot_kws)
+
+            # クロスバリデーション
+            score_train_dict = {}
+            for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
+                # 表示用にテストデータと学習データ分割
+                X_train = X[train]
+                y_train = y_true[train]
+                X_test = X[test]
+                y_test = y_true[test]
+                # 色分け用データ取得(していないときは、クロスバリデーション番号を使用、LeaveOuneOutのときは番号分けない)
+                if hue is None:
+                    hue_test = np.full(len(test) ,f'cv_{i}')
+                    hue_name = 'cv_number'  # 色分け名を'cv_number'に指定
+                else:
+                    hue_test = data[hue].values[test]
+                    hue_name = hue
+                # 誤差上位表示用データ取得
+                if rank_number is not None:
+                    if rank_col is None:  # 表示フィールド指定ないとき、Index使用
+                        rank_col_test = data.index.values[test]
+                    else:  # 表示フィールド指定あるとき
+                        rank_col_test = data[rank_col].values[test]
+                
+                # eval_setの中から学習データ or テストデータのみを抽出
+                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
+                                                        fit_params, train, test)
+
+                # 学習と推論
+                estimator.fit(X_train, y_train, **fit_params_modified)
+                # 学習データスコア算出
+                y_pred_train = estimator.predict(X_train)
+                score_dict = cls._make_score_dict(y_train, y_pred_train, scores)
+                for score in scores:
+                    if f'{score}_train' not in score_train_dict:
+                        score_train_dict[f'{score}_train'] = []
+                    score_train_dict[f'{score}_train'].append(score_dict[score])
+                # CV内結果をプロット
+                score_cv_dict = {k: v[i] for k, v in score_all_dict.items()}
+                score_cv_dict.update({f'{k}_train': v for k, v in score_dict.items()})
+                cls._estimator_plot_1d(estimator, X_test, y_test, hue_data=hue_test, hue_name=hue_name, ax=axes[i],
+                                   linecolor=linecolor, rounddigit=rounddigit, score_dict=score_cv_dict,
+                                   scatter_kws=scatter_kws, legend_kws=legend_kws)
+                # 誤差上位を文字表示
+                if rank_number is not None:
+                    cls._rank_display(y_test, estimator.predict(X_test), rank_number, rank_col, rank_col_test, x=X_test, ax=axes[i], rounddigit=rounddigit)
+                axes[i].set_title(f'Cross Validation Fold{i}')
+
+            # スコアの統計値を計算
+            if cv_stats == 'mean':
+                score_stats_dict = {f'{k}_mean': np.mean(v) for k, v in score_all_dict.items()}
+                train_stats_dict = {k: np.mean(v) for k, v in score_train_dict.items()}
+            elif cv_stats == 'median':
+                score_stats_dict = {f'{k}_median': np.median(v) for k, v in score_all_dict.items()}
+                train_stats_dict = {k: np.median(v) for k, v in score_train_dict.items()}
+            elif cv_stats == 'min':
+                score_stats_dict = {f'{k}_min': np.amin(v) for k, v in score_all_dict.items()}
+                train_stats_dict = {k: np.amin(v) for k, v in score_train_dict.items()}
+            elif cv_stats == 'max':
+                score_stats_dict = {f'{k}_max': np.amax(v) for k, v in score_all_dict.items()}
+                train_stats_dict = {k: np.amax(v) for k, v in score_train_dict.items()}
+            # 学習データスコアをdictに追加
+            score_stats_dict.update(train_stats_dict)
+            # 全体色分け用データ取得
+            hue_data = None if hue is None else data[hue]
+            hue_name = None if hue is None else hue
+            # 全体プロット
+            ax_all = axes[cv_num]
+            cls._estimator_plot_1d(estimator, X, y_true, hue_data=hue_data, hue_name=hue_name, ax=ax_all,
+                               linecolor=linecolor, rounddigit=rounddigit, score_dict=score_stats_dict,
+                               scatter_kws=scatter_kws, legend_kws=legend_kws)
+            ax_all.set_title('All Cross Validations')
+            return score_stats_dict
+
+    @classmethod
+    def _reg_heat_plot_2d(cls, trained_estimator, x_heat, y_true_col, y_pred_col, rank_col, data, x_heat_indices, hue_name,
+                          x1_start, x1_end, x2_start, x2_end, heat_division, other_x,
+                          vmin, vmax, ax, plot_scatter, maxerror, rank_dict, scatter_hue_dict,
+                          rounddigit_rank, rounddigit_x1, rounddigit_x2,
+                          heat_kws=None, scatter_kws=None, legend_kws=None):
+        """
+        回帰予測値ヒートマップと各種散布図の表示
+        (regression_heat_plotメソッドの描画処理部分)
+        """
+        # 描画用axがNoneのとき、matplotlib.pyplot.gca()を使用
+        if ax is None:
+            ax=plt.gca()
+
+        # ヒートマップ用グリッドデータを作成
+        xx = np.linspace(x1_start, x1_end, heat_division)
+        yy = np.linspace(x2_start, x2_end, heat_division)
+        X1, X2 = np.meshgrid(xx, yy)
+        X_grid = np.c_[X1.ravel(), X2.ravel()]
+        df_heat = pd.DataFrame(X_grid, columns=x_heat)
+        # 推論用に全説明変数を保持したndarrayを作成 (ヒートマップ非使用変数は固定値other_xとして追加)
+        n_rows = X_grid.shape[0]
+        X_all = []
+        other_add_flg = False
+        for i in range(2 + len(other_x)):
+            if i == x_heat_indices[0]: # ヒートマップ使用変数(1個目)を追加
+                X_all.append(X_grid[:, 0].reshape(n_rows, 1))
+            elif i == x_heat_indices[1]: # ヒートマップ使用変数(2個目)を追加
+                X_all.append(X_grid[:, 1].reshape(n_rows, 1))
+            elif len(other_x) >= 1 and not other_add_flg:  # ヒートマップ非使用変数(1個目)を固定値として追加
+                X_all.append(np.full((n_rows, 1), other_x[0]))
+                other_add_flg = True
+            elif len(other_x) == 2:  # ヒートマップ非使用変数(2個目)を固定値として追加
+                X_all.append(np.full((n_rows, 1), other_x[1]))
+        X_all = np.hstack(X_all)
+        # グリッドデータに対して学習し、推定値を作成
+        y_pred_grid = trained_estimator.predict(X_all)
+        df_heat['y_pred'] = pd.Series(y_pred_grid)
+        # グリッドデータ縦軸横軸の表示桁数を調整
+        df_heat[x_heat[0]] = df_heat[x_heat[0]].map(lambda x: cls._round_digits(x, rounddigit=rounddigit_x1))
+        df_heat[x_heat[1]] = df_heat[x_heat[1]].map(lambda x: cls._round_digits(x, rounddigit=rounddigit_x2))
+        # グリッドデータをピボット化
+        df_heat_pivot = pd.pivot_table(data=df_heat, values='y_pred', 
+                                  columns=x_heat[0], index=x_heat[1], aggfunc=np.mean)
+        # 横軸の列数がheat_divisionに満たない時、分解能不足のためrounddigit_x1桁数を増やすようエラー表示
+        if len(df_heat_pivot.columns) < heat_division:
+            raise Exception(f'the "rounddigit_x1" argument must be bigger than {rounddigit_x1} because of the shortage of the "{x_heat[0]}" resolution')
+        # 縦軸の列数がheat_divisionに満たない時、分解能不足のためrounddigit_x2桁数を増やすようエラー表示
+        if len(df_heat_pivot) < heat_division:
+            raise Exception(f'the "rounddigit_x2" argument must be bigger than {rounddigit_x2} because of the shortage of the "{x_heat[1]}" resolution')
+
+        # ヒートマップのカラーマップ指定ないとき、YlGnを指定
+        if 'cmap' not in heat_kws.keys():
+            heat_kws['cmap'] = 'YlGn'
+        # ヒートマップをプロット
+        sns.heatmap(df_heat_pivot, ax=ax, vmax=vmax, vmin=vmin, center=(vmax+vmin)/2, **heat_kws)
+
+        # 誤差散布図をプロット
+        if plot_scatter is not None:
+            # 軸範囲が0～heat_divisionになっているので、スケール変換
+            x1_scatter = 0.5 + (data[x_heat[0]].values - x1_start) * (heat_division - 1) / (x1_end - x1_start)
+            x2_scatter = 0.5 + (data[x_heat[1]].values - x2_start) * (heat_division - 1) / (x2_end - x2_start)
+            # 色分け
+            if plot_scatter == 'error':  # 誤差で色分け
+                scatter_c = data[y_pred_col].values - data[y_true_col].values
+                scatter_vmin = -maxerror
+                scatter_vmax = maxerror
+                if 'cmap' not in scatter_kws.keys():  # 散布図のカラーマップ指定ないとき、seismicを指定
+                    scatter_kws['cmap'] = 'seismic'
+            elif plot_scatter == 'true':  # 真値で色分け
+                scatter_c = data[y_true_col].values
+                scatter_vmin = vmin
+                scatter_vmax = vmax
+                if 'cmap' not in scatter_kws.keys():  # 散布図のカラーマップ指定ないとき、ヒートマップと同cmap使用
+                    scatter_kws['cmap'] = heat_kws['cmap']
+                if 'edgecolors' not in scatter_kws.keys():  # 線の色指定ないとき、ブラウンを指定
+                    scatter_kws['edgecolors'] = 'brown'
+            # 散布図プロット (誤差or真値で色分けしたとき)
+            if plot_scatter == 'error' or plot_scatter == 'true':
+                ax.scatter(x1_scatter, x2_scatter, vmin=scatter_vmin, vmax=scatter_vmax, c=scatter_c, **scatter_kws)
+            # 散布図プロット (hue列名で色分けしたとき)
+            if plot_scatter == 'hue':
+                scatter_data = pd.DataFrame(np.stack([x1_scatter, x2_scatter, data[hue_name]], 1), columns=['x1', 'x2', hue_name])
+                for name, group in scatter_data.groupby(hue_name):
+                    ax.scatter(group['x1'].values, group['x2'].values, label=name, c=scatter_hue_dict[name], **scatter_kws)
+                ax.legend(**legend_kws)
+        
+        # 誤差上位を文字表示
+        df_rank = data[data.index.isin(rank_dict.keys())]
+        for index, row in df_rank.iterrows():
+            # rank_col指定ないとき、indexがfloat型に変換されてしまうので、int型に戻す
+            rank_col_value = int(row[rank_col]) if rank_col == 'index' else row[rank_col]
+            # 誤差を計算してテキスト化
+            error = cls._round_digits(row['y_pred'] - row['y_true'], rounddigit=rounddigit_rank)
+            rank_text = f'     no{rank_dict[index]+1}\n-<-error={error}\n     {rank_col}={rank_col_value}'
+            # 軸範囲が0～heat_divisionになっているので、スケール変換してプロット
+            x1_text = 0.5 + (row[x_heat[0]] - x1_start) * (heat_division - 1) / (x1_end - x1_start)
+            x2_text = 0.5 + (row[x_heat[1]] - x2_start) * (heat_division - 1) / (x2_end - x2_start)
+            ax.text(x1_text, x2_text, rank_text, verticalalignment='center', horizontalalignment='left')
+    
+    @classmethod
+    def _reg_heat_plot(cls, trained_estimator, X, y_pred, y_true, x_heat, x_not_heat, x_heat_indices, hue_data, hue_name,
+                       pair_sigmarange=1.0, pair_sigmainterval=0.5, heat_extendsigma=0.5, heat_division=30, 
+                       vmin=None, vmax=None, plot_scatter='true', maxerror=None,
+                       rank_number=None, rank_col=None, rank_col_data=None, scatter_hue_dict=None,
+                       rounddigit_rank=None, rounddigit_x1=None, rounddigit_x2=None, rounddigit_x3=None,
+                       cv_index=None, subplot_kws=None, heat_kws=None, scatter_kws=None, legend_kws=None):
+        """
+        回帰予測値ヒートマップ表示の、説明変数の数に応じた分岐処理
+        (regression_heat_plotメソッド処理のうち、説明変数の数に応じたデータ分割等を行う)
+        """
+        # 説明変数の数
+        x_num = X.shape[1]
+        # ヒートマップ使用DataFrame
+        df_heat = pd.DataFrame(X[:, x_heat_indices], columns=x_heat)
+        # ヒートマップ非使用DataFrame
+        X_not_heat = X[:, [i for i in range(X.shape[1]) if i not in x_heat_indices]]
+        df_not_heat = pd.DataFrame(X_not_heat, columns=x_not_heat)
+        # 結合＆目的変数実測値と予測値追加
+        df_all = df_heat.join(df_not_heat)
+        df_all = df_all.join(pd.DataFrame(y_true, columns=['y_true']))
+        df_all = df_all.join(pd.DataFrame(y_pred, columns=['y_pred']))
+        # ヒートップ非使用変数を標準化してDataFrameに追加
+        if x_num >= 3:
+            X_not_heat_norm = stats.zscore(X_not_heat)
+            df_all = df_all.join(pd.DataFrame(X_not_heat_norm, columns=[f'normalize_{c}' for c in x_not_heat]))
+        # 誤差上位表示用IDデータをDataFrameに追加
+        rank_col = 'index' if rank_col is None else rank_col
+        df_all = df_all.join(pd.DataFrame(rank_col_data, columns=[rank_col]))
+        # 散布図色分け用列をDataFrameに追加(hue_nameがNoneでないときのみ))
+        if hue_name is not None:
+            df_all = df_all.join(pd.DataFrame(hue_data, columns=[hue_name]))
+
+        # 誤差の順位を計算
+        if rank_number is not None:
+            y_error_abs = np.abs(y_pred - y_true)
+            rank_index  = np.argsort(-y_error_abs)[:rank_number]
+            rank_dict = dict(zip(rank_index.tolist(), range(rank_number)))
+        else:
+            rank_dict = {}
+
+        # ヒートマップのX1軸およびX2軸の表示範囲(最大最小値 + extendsigma)
+        x1_min = np.min(X[:, x_heat_indices[0]])
+        x1_max = np.max(X[:, x_heat_indices[0]])
+        x1_std = np.std(X[:, x_heat_indices[0]])
+        x1_start = x1_min - x1_std * heat_extendsigma
+        x1_end = x1_max + x1_std * heat_extendsigma
+        x2_min = np.min(X[:, x_heat_indices[1]])
+        x2_max = np.max(X[:, x_heat_indices[1]])
+        x2_std = np.std(X[:, x_heat_indices[1]])
+        x2_start = x2_min - x2_std * heat_extendsigma
+        x2_end = x2_max + x2_std * heat_extendsigma
+
+        # プロットする図の数(sigmarange外「2枚」 + sigmarange内「int(pair_sigmarange / pair_sigmainterval) * 2枚」)
+        pair_n = int(pair_sigmarange / pair_sigmainterval) * 2 + 2
+        # ヒートップ非使用変数をプロットする範囲の下限(標準化後)
+        pair_min = -(pair_n - 2) / 2 * pair_sigmainterval
+
+        # 説明変数が2次元のとき (図は1枚のみ)
+        if x_num == 2:
+            pair_w = 1
+            pair_h = 1
+        # 説明変数が3次元のとき (図はpair_n × 1枚)
+        elif x_num == 3:
+            pair_w = 1
+            pair_h = pair_n
+        # 説明変数が4次元のとき (図はpair_n × pair_n枚)
+        elif x_num == 4:
+            pair_w = pair_n
+            pair_h = pair_n
+
+        # figsize (全ての図全体のサイズ)指定
+        if 'figsize' not in subplot_kws.keys():
+            subplot_kws['figsize'] = (pair_w * 6, pair_h * 5)
+        # プロット用のaxes作成
+        fig, axes = plt.subplots(pair_h, pair_w, **subplot_kws)
+        if cv_index is not None:
+            fig.suptitle(f'CV No.{cv_index}')
+
+        # 図ごとにプロット
+        for i in range(pair_h):
+            for j in range(pair_w):
+                # pair縦軸変数(標準化後)の最小値
+                if i == 0:
+                    h_min = -float('inf')
+                    h_mean = pair_min - pair_sigmainterval / 2  # ヒートマップ非使用変数指定用の平均値
+                else:
+                    h_min = pair_min + (i - 1) * pair_sigmainterval
+                    h_mean = pair_min + (i - 0.5) * pair_sigmainterval  # ヒートマップ非使用変数指定用の平均値
+                # pair縦軸変数(標準化後)の最大値
+                if i == pair_h - 1:
+                    h_max = float('inf')
+                else:
+                    h_max = pair_min + i * pair_sigmainterval
+                # pair横軸変数(標準化後)の最小値
+                if j == 0:
+                    w_min = -float('inf')
+                    w_mean = pair_min - pair_sigmainterval / 2  # ヒートマップ非使用変数指定用の平均値
+                else:
+                    w_min = pair_min + (j - 1) * pair_sigmainterval
+                    w_mean = pair_min + (j - 0.5) * pair_sigmainterval  # ヒートマップ非使用変数指定用の平均値
+                # pair横軸変数(標準化後)の最大値
+                if j == pair_w - 1:
+                    w_max = float('inf')
+                else:
+                    w_max = pair_min + j * pair_sigmainterval
+
+                # 説明変数が2次元のとき (図は1枚のみ)
+                if x_num == 2:
+                    ax = axes
+                    df_pair = df_all.copy()
+                    other_x = []
+                # 説明変数が3次元のとき (図はpair_n × 1枚)
+                elif x_num == 3:
+                    ax = axes[i]
+                    # 縦軸変数範囲内のみのデータを抽出
+                    df_pair = df_all[(df_all[f'normalize_{x_not_heat[0]}'] >= h_min) & (df_all[f'normalize_{x_not_heat[0]}'] < h_max)].copy()
+                    # ヒートマップ非使用変数の標準化逆変換
+                    x3_mean = np.mean(X_not_heat[:, 0])
+                    x3_std = np.std(X_not_heat[:, 0])
+                    other_x = [h_mean * x3_std + x3_mean]
+                # 説明変数が4次元のとき (図はpair_n × pair_n枚)
+                elif x_num == 4:
+                    ax = axes[j, i]
+                    # 縦軸変数範囲内のみのデータを抽出
+                    df_pair = df_all[(df_all[f'normalize_{x_not_heat[0]}'] >= h_min) & (df_all[f'normalize_{x_not_heat[0]}'] < h_max)].copy()
+                    # 横軸変数範囲内のみのデータを抽出
+                    df_pair = df_pair[(df_pair[f'normalize_{x_not_heat[1]}'] >= w_min) & (df_pair[f'normalize_{x_not_heat[1]}'] < w_max)]
+                    # ヒートマップ非使用変数の標準化逆変換
+                    x3_mean = np.mean(X_not_heat[:, 0])
+                    x3_std = np.std(X_not_heat[:, 0])
+                    x4_mean = np.mean(X_not_heat[:, 1])
+                    x4_std = np.std(X_not_heat[:, 1])
+                    other_x = [h_mean * x3_std + x3_mean, w_mean * x4_std + x4_mean]
+                
+                cls._reg_heat_plot_2d(trained_estimator, x_heat, 'y_true', 'y_pred', rank_col, df_pair, x_heat_indices, hue_name,
+                                      x1_start, x1_end, x2_start, x2_end, heat_division, other_x,
+                                      vmin, vmax, ax, plot_scatter, maxerror, rank_dict, scatter_hue_dict,
+                                      rounddigit_rank, rounddigit_x1, rounddigit_x2,
+                                      heat_kws=heat_kws, scatter_kws=scatter_kws, legend_kws=legend_kws)
+
+                # グラフタイトルとして、ヒートマップ非使用変数の範囲を記載（説明変数が3次元以上のとき）
+                if x_num == 3:
+                    if i == 0:
+                        ax.set_title(f'{x_not_heat[0]}=- {cls._round_digits(h_max * x3_std + x3_mean, rounddigit=rounddigit_x3)} (- {h_max}σ)')
+                    elif i == pair_h - 1:
+                        ax.set_title(f'{x_not_heat[0]}={cls._round_digits(h_min * x3_std + x3_mean, rounddigit=rounddigit_x3)} - ({h_min}σ -)')
+                    else:
+                        ax.set_title(f'{x_not_heat[0]}={cls._round_digits(h_min * x3_std + x3_mean, rounddigit=rounddigit_x3)} - {cls._round_digits(h_max * x3_std + x3_mean, rounddigit=rounddigit_x3)} ({h_min}σ - {h_max}σ)')
+                if x_num == 4:
+                    ax.set_title(f'{x_not_heat[0]}= {h_min}σ - {h_max}σ  {x_not_heat[1]}= {w_min}σ - {w_max}σ')
+
+        # 字が重なるのでtight_layoutにする
+        plt.tight_layout(rect=[0, 0, 1, 0.98])
+
+    @classmethod
+    def regression_heat_plot(cls, estimator, x: List[str], y: str, data: pd.DataFrame = None,
+                             x_colnames: List[str] = None, x_heat: List[str] = None, scatter_hue=None,
+                             pair_sigmarange = 1.0, pair_sigmainterval = 0.5, heat_extendsigma = 0.5, 
+                             heat_division = 30, color_extendsigma = 0.5,
+                             plot_scatter = 'true', rounddigit_rank=3, rounddigit_x1=2, rounddigit_x2=2, rounddigit_x3=2,
+                             rank_number=None, rank_col=None,
+                             cv=None, cv_seed=42, cv_group=None, display_cv_indices = 0,
+                             estimator_params=None, fit_params=None, eval_set_selection=None,
+                             subplot_kws=None, heat_kws=None, scatter_kws=None, legend_kws=None):
+        """
+        Plot regression heatmaps of any scikit-learn regressor with 2 to 4D explanatory variables.
+
+        Parameters
+        ----------
+        estimator : estimator object implementing ``fit``
+            Regression estimator. This is assumed to implement the scikit-learn estimator interface.
+
+        x : list[str] or np.ndarray
+            Explanatory variables. Should be list[str] if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
+
+        y : str or np.ndarray
+            Objective variable. Should be str if ``data`` is pd.DataFrame. Should be np.ndarray if ``data`` is None
+
+        data: pd.DataFrame
+            Input data structure.
+
+        x_colnames: list[str], optional
+            Names of explanatory variables. Available only if ``data`` is NOT pd.DataFrame
+
+        x_heat: list[str], optional
+            X-axis and y-axis variables of heatmap. If None, use two variables in ``x`` from the front.
+
+        scatter_hue : str, optional
+            Grouping variable that will produce points with different colors. Available only if plot_scatter is set to ``hue``.
+
+        pair_sigmarange: float, optional
+            Set the range of subplots. The lower limit is mean({x3, x4}) - ``pair_sigmarange`` * std({x3, x4}). The higher limit is mean({x3, x4}) + ``pair_sigmarange`` * std({x3, x4}). Available only if len(x) is bigger than 2.
+
+        pair_sigmainterval: float, optional
+            Set the interval of subplots. For example, if ``pair_sigmainterval`` is set to 0.5 and ``pair_sigmarange`` is set to 1.0, The ranges of subplots are lower than μ-1σ, μ-1σ to μ-0.5σ, μ-0.5σ to μ, μ to μ+0.5σ, μ+0.5σ to μ+1σ, and higher than μ+1σ. Available only if len(x) is bigger than 2.
+
+        heat_extendsigma: float, optional
+            Set the axis view limits of the heatmap. The lower limit is min({x1, x2}) - std({x1, x2}) * ``heat_extendsigma``. The higher limit is max({x1, x2}) + std({x1, x2}) * ``heat_extendsigma``
+
+        heat_division: int, optional
+            Resolution of the heatmap.
+
+        color_extendsigma: float, optional
+            Set the colormap limits of the heatmap. The lower limit is min(y_ture) - std(y_ture) * ``color_extendsigma``. The higher limit is max(y_ture) - std(y_ture) * ``color_extendsigma``.
+
+        plot_scatter: {'error', 'true', 'hue'}, optional
+            Color decision of scatter plot. If 'error', to be mapped to colors using error value. If 'true', to be mapped to colors using y_ture value. If 'hue', to be mapped to colors using scatter_hue variable. If None, no scatter.
+
+        rounddigit_rank: int, optional
+            Round a number of error that are in the top posiotions for regression error to a given precision in decimal digits.
+
+        rounddigit_x1: int, optional
+            Round a number of x-axis valiable of the heatmap to a given precision in decimal digits.
+
+        rounddigit_x2: int, optional
+            Round a number of y-axis valiable of the heatmap to a given precision in decimal digits.
+
+        rounddigit_x3: int, optional
+            Round a number of y-axis valiable of subplots to a given precision in decimal digits.
+
+        rank_number: int, optional
+            Number of emphasized data that are in the top posiotions for regression error.
+
+        rank_col: str, optional
+            Variables that are displayed with emphasized data that are in the top posiotions for regression error.
+
+        cv : int, cross-validation generator, or an iterable, optional
+            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
+
+        cv_seed : int, optional
+            Seed for random number generator of cross validation.
+
+        cv_group: str, optional
+            Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
+
+        display_cv_indices : int or list, optional
+            Cross validation index or indices to display.
+
+        estimator_params : dict, optional
+            Parameters passed to the regression estimator. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
+
+        fit_params : dict, optional
+            Parameters passed to the fit() method of the regression estimator, e.g. ``early_stopping_round`` and ``eval_set`` of XGBRegressor. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
+
+        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
+            
+            If "all", use all data in `X` and `y`.
+
+            If "train", select train data from `X` and `y` using cv.split().
+
+            If "test", select test data from `X` and `y` using cv.split().
+
+            If "original", use raw `eval_set`.
+
+            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+
+        subplot_kws: dict, optional
+            Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
+
+        heat_kws: dict, optional
+            Additional parameters passed to sns.heatmap(), e.g. ``cmap``. See https://seaborn.pydata.org/generated/seaborn.heatmap.html
+
+        scatter_kws: dict, optional
+            Additional parameters passed to matplotlib.pyplot.scatter(), e.g. ``alpha``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.scatter.html
+
+        legend_kws : dict
+            Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
+        """
+
+        # 入力データの形式統一
+        X, y_true, data, x_colnames, y_colname, cv_group_colname = cls._reshape_input_data(x, y, data,
+                                                                                           x_colnames,
+                                                                                           cv_group)
+        # 説明変数xの次元が2～4以外ならエラーを出す
+        if len(x_colnames) < 2 or len(x_colnames) > 4:
+            raise Exception('Dimension of x must be 2 to 4')
+        
+        # display_cv_indicesをList化
+        if isinstance(display_cv_indices, int):
+            display_cv_indices = [display_cv_indices]
+        elif not isinstance(x_colnames, list):
+            raise Exception('the "cv_display_indices" argument must be int or List[int]')
+        # 学習器パラメータがあれば適用
+        if estimator_params is not None:
+            estimator.set_params(**estimator_params)
+        # 学習時パラメータがNoneなら空のdictを入力
+        if fit_params is None:
+            fit_params = {}
+        # subplot_kwsがNoneなら空のdictを入力
+        if subplot_kws is None:
+            subplot_kws = {}
+        # heat_kwsがNoneなら空のdictを入力
+        if heat_kws is None:
+            heat_kws = {}
+        # scatter_kwsがNoneなら空のdictを入力
+        if scatter_kws is None:
+            scatter_kws = {}
+        # legend_kwsがNoneなら空のdictを入力
+        if legend_kws is None:
+            legend_kws = {}
+        
+        # ヒートマップ表示用の列を抽出
+        if x_heat is None:  # 列名指定していないとき、前から2列を抽出
+            x_heat = x_colnames[:2]
+            x_heat_indices = [0, 1]
+        else:  # 列名指定しているとき、該当列のXにおけるインデックス(0～3)を保持
+            if len(x_heat) != 2:
+                raise Exception('length of x_heat must be 2')
+            x_heat_indices = []
+            for colname in x_heat:
+                x_heat_indices.append(x_colnames.index(colname))
+        # ヒートマップ表示以外の列
+        x_not_heat = [colname for colname in x_colnames if colname not in x_heat]        
+        # ヒートマップの色分け最大最小値(y_trueの最大最小値 ± y_trueの標準偏差 × color_extendsigma)
+        y_true_std = np.std(y_true)
+        vmin = np.min(y_true) - y_true_std * color_extendsigma
+        vmax = np.max(y_true) + y_true_std * color_extendsigma
+
+        # 引数plot_scatter='hue'とscatter_hueが同時指定されていないとき、エラーを出す
+        if scatter_hue is not None:
+            if plot_scatter != 'hue' and not isinstance(cv, GroupKFold) and not isinstance(cv, LeaveOneGroupOut):
+                raise Exception('the "plot_scatter" argument must be "hue" when the argument "scatter_hue" is not None')
+        elif plot_scatter == 'hue':
+            raise Exception('the "scatter_hue" argument is required when the argument "plot_scatter" is "hue"')
+        # 引数plot_scatter='hue'のとき、色分け対象列とカラーマップを紐づけ(色分けを全ての図で統一用)
+        if plot_scatter == 'hue':
+            hue_list = data[scatter_hue].values.tolist()
+            hue_list = sorted(set(hue_list), key=hue_list.index)
+            scatter_hue_dict = dict(zip(hue_list, cls._HEAT_SCATTER_HUECOLORS[0:len(hue_list)]))
+        else:
+            scatter_hue_dict = None
+        
+        # クロスバリデーション有無で場合分け
+        # クロスバリデーション未実施時(学習データからプロット＆指標算出)
+        if cv is None:
+            # 学習と推論
+            estimator.fit(X, y_true, **fit_params)
+            y_pred = estimator.predict(X)
+            # 誤差上位表示用データ取得
+            if rank_number is not None:
+                if rank_col is None:  # 表示フィールド指定ないとき、Index使用
+                    rank_col_data = data.index.values
+                else:  # 表示フィールド指定あるとき
+                    rank_col_data = data[rank_col].values
+            else:
+                rank_col_data = None
+            # 誤差最大値
+            maxerror = np.max(np.abs(y_pred - y_true))
+            # 散布図色分け用データ取得(plot_scatter='hue'のときのみ有効)
+            hue_data = data[scatter_hue] if scatter_hue is not None and plot_scatter=='hue' else None
+            hue_name = scatter_hue if scatter_hue is not None and plot_scatter=='hue' else None
+            # ヒートマップをプロット
+            cls._reg_heat_plot(estimator, X, y_pred, y_true, x_heat, x_not_heat, x_heat_indices, hue_data, hue_name,
+                               pair_sigmarange = pair_sigmarange, pair_sigmainterval=pair_sigmainterval, heat_extendsigma=heat_extendsigma, heat_division=heat_division,
+                               vmin=vmin, vmax=vmax, plot_scatter=plot_scatter, maxerror=maxerror,
+                               rank_number=rank_number, rank_col=rank_col, rank_col_data=rank_col_data, scatter_hue_dict=scatter_hue_dict,
+                               rounddigit_rank=rounddigit_rank, rounddigit_x1=rounddigit_x1, rounddigit_x2=rounddigit_x2, rounddigit_x3=rounddigit_x3,
+                               cv_index=None, subplot_kws=subplot_kws, heat_kws=heat_kws, scatter_kws=scatter_kws, legend_kws=legend_kws)
+            
+        # クロスバリデーション実施時(分割ごとに別々にプロット＆指標算出)
+        if cv is not None:
+            # 分割法未指定時、cv_numとseedに基づきKFoldでランダムに分割
+            if isinstance(cv, numbers.Integral):
+                cv = KFold(n_splits=cv, shuffle=True, random_state=cv_seed)
+            # LeaveOneOutのときエラーを出す
+            if isinstance(cv, LeaveOneOut):
+                raise Exception('"regression_heat_plot" method does not support "LeaveOneOut" cross validation')
+            # cv_groupをグルーピング対象に指定(GroupKFold、LeaveOneGroupOut等)
+            split_kws={}
+            if cv_group_colname is not None:
+                split_kws['groups'] = data[cv_group_colname].values
+            elif isinstance(cv, GroupKFold) or isinstance(cv, LeaveOneGroupOut):
+                raise Exception('"GroupKFold" and "LeaveOneGroupOut" cross validations need ``cv_group`` argument')
+            # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
+            if isinstance(cv, LeaveOneGroupOut):
+                cv_num = len(set(data[cv_group_colname].values))
+            else:
+                cv_num = cv.n_splits
+
+            # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
+            if eval_set_selection is None:
+                eval_set_selection = 'test'
+            fit_params, eval_set_selection = init_eval_set(
+                    eval_set_selection, fit_params, X, y)
+            # 最終学習器以外の前処理変換器作成
+            transformer = _make_transformer(eval_set_selection, estimator)
+
+            # クロスバリデーション
+            for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
+                # 表示対象以外のCVなら飛ばす
+                if i not in display_cv_indices:
+                    continue
+                print(f'cv_number={i}/{cv_num}')
+                # 表示用にテストデータと学習データ分割
+                X_train = X[train]
+                y_train = y_true[train]
+                X_test = X[test]
+                y_test = y_true[test]
+
+                # eval_setの中から学習データ or テストデータのみを抽出
+                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
+                                                        fit_params, train, test)
+
+                # 学習と推論
+                estimator.fit(X_train, y_train, **fit_params_modified)
+                y_pred = estimator.predict(X_test)
+                # 誤差上位表示用データ取得
+                if rank_number is not None:
+                    if rank_col is None:  # 表示フィールド指定ないとき、Index使用
+                        rank_col_test = data.index.values[test]
+                    else:  # 表示フィールド指定あるとき
+                        rank_col_test = data[rank_col].values[test]
+                else:
+                    rank_col_test = None
+                # 誤差最大値
+                maxerror = np.max(np.abs(y_pred - y_test))
+                # 散布図色分け用データ取得(plot_scatter='hue'のときのみ有効))
+                hue_data = data[scatter_hue].values[test] if scatter_hue is not None and plot_scatter=='hue' else None
+                hue_name = scatter_hue if scatter_hue is not None and plot_scatter=='hue' else None
+                # ヒートマップをプロット
+                cls._reg_heat_plot(estimator, X_test, y_pred, y_test, x_heat, x_not_heat, x_heat_indices, hue_data, hue_name,
+                                   pair_sigmarange = pair_sigmarange, pair_sigmainterval = pair_sigmainterval, heat_extendsigma=heat_extendsigma, heat_division=heat_division,
+                                   vmin=vmin, vmax=vmax, plot_scatter = plot_scatter, maxerror=maxerror,
+                                   rank_number=rank_number, rank_col=rank_col, rank_col_data=rank_col_test, scatter_hue_dict=scatter_hue_dict,
+                                   rounddigit_rank=rounddigit_rank, rounddigit_x1=rounddigit_x1, rounddigit_x2=rounddigit_x2, rounddigit_x3=rounddigit_x3,
+                                   cv_index=i, subplot_kws=subplot_kws, heat_kws=heat_kws, scatter_kws=scatter_kws, legend_kws=legend_kws)
```

### Comparing `seaborn-analyzer-0.2.9/seaborn_analyzer/multiclass_fitparams.py` & `seaborn-analyzer-0.3.0/seaborn_analyzer/multiclass_fitparams.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import warnings
-import numpy as np
-from sklearn import clone
-from sklearn.multiclass import OneVsRestClassifier, _ConstantPredictor
-from sklearn.preprocessing import LabelBinarizer
-from sklearn.utils.fixes import delayed
-from joblib import Parallel
-
-def _fit_binary(estimator, X, y, classes=None, **kwargs):
-    """Fit a single binary estimator with kwargs."""
-    unique_y = np.unique(y)
-    if len(unique_y) == 1:
-        if classes is not None:
-            if y[0] == -1:
-                c = 0
-            else:
-                c = y[0]
-            warnings.warn("Label %s is present in all training examples." % str(classes[c]))
-        estimator = _ConstantPredictor().fit(X, unique_y)
-    else:
-        estimator = clone(estimator)
-        estimator.fit(X, y, **kwargs)
-    return estimator
-
-class OneVsRestClassifierPatched(OneVsRestClassifier):
-    """One-vs-the-rest (OvR) multiclass strategy with ``fit_params``."""
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def fit(self, X, y, fit_params_list):
-        self.label_binarizer_ = LabelBinarizer(sparse_output=True)
-        Y = self.label_binarizer_.fit_transform(y)
-        Y = Y.tocsc()
-        self.classes_ = self.label_binarizer_.classes_
-        columns = (col.toarray().ravel() for col in Y.T)
-        self.estimators_ = Parallel(n_jobs=self.n_jobs)(delayed(_fit_binary)(
-            self.estimator, X, column, classes=[
-                "not %s" % self.label_binarizer_.classes_[i],
-                self.label_binarizer_.classes_[i]], **fit_params_list[i])
-            for i, column in enumerate(columns))
+import warnings
+import numpy as np
+from sklearn import clone
+from sklearn.multiclass import OneVsRestClassifier, _ConstantPredictor
+from sklearn.preprocessing import LabelBinarizer
+from sklearn.utils.fixes import delayed
+from joblib import Parallel
+
+def _fit_binary(estimator, X, y, classes=None, **kwargs):
+    """Fit a single binary estimator with kwargs."""
+    unique_y = np.unique(y)
+    if len(unique_y) == 1:
+        if classes is not None:
+            if y[0] == -1:
+                c = 0
+            else:
+                c = y[0]
+            warnings.warn("Label %s is present in all training examples." % str(classes[c]))
+        estimator = _ConstantPredictor().fit(X, unique_y)
+    else:
+        estimator = clone(estimator)
+        estimator.fit(X, y, **kwargs)
+    return estimator
+
+class OneVsRestClassifierPatched(OneVsRestClassifier):
+    """One-vs-the-rest (OvR) multiclass strategy with ``fit_params``."""
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def fit(self, X, y, fit_params_list):
+        self.label_binarizer_ = LabelBinarizer(sparse_output=True)
+        Y = self.label_binarizer_.fit_transform(y)
+        Y = Y.tocsc()
+        self.classes_ = self.label_binarizer_.classes_
+        columns = (col.toarray().ravel() for col in Y.T)
+        self.estimators_ = Parallel(n_jobs=self.n_jobs)(delayed(_fit_binary)(
+            self.estimator, X, column, classes=[
+                "not %s" % self.label_binarizer_.classes_[i],
+                self.label_binarizer_.classes_[i]], **fit_params_list[i])
+            for i, column in enumerate(columns))
         return self
```

### Comparing `seaborn-analyzer-0.2.9/setup.py` & `seaborn-analyzer-0.3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-# Author: Kenta Nakamura <c60evaporator@gmail.com>
-# Copyright (c) 2020-2021 Kenta Nakamura
-# License: BSD 3 clause
-
-from setuptools import setup
-import seaborn_analyzer
-
-DESCRIPTION = "seaborn-analyzer: data visualization of regression, classification and distribution"
-NAME = 'seaborn-analyzer'
-AUTHOR = 'Kenta Nakamura'
-AUTHOR_EMAIL = 'c60evaporator@gmail.com'
-URL = 'https://github.com/c60evaporator/seaborn-analyzer'
-LICENSE = 'BSD 3-Clause'
-DOWNLOAD_URL = 'https://github.com/c60evaporator/seaborn-analyzer'
-VERSION = seaborn_analyzer.__version__
-PYTHON_REQUIRES = ">=3.6"
-
-INSTALL_REQUIRES = [
-    'matplotlib>=3.3.4',
-    'seaborn>=0.11.0',
-    'numpy >=1.20.3',
-    'pandas>=1.2.4',
-    'matplotlib>=3.3.4',
-    'scipy>=1.6.3',
-    'scikit-learn>=0.24.2',
-]
-
-EXTRAS_REQUIRE = {
-    'tutorial': [
-        'mlxtend>=0.18.0',
-        'xgboost>=1.4.2',
-    ]
-}
-
-PACKAGES = [
-    'seaborn_analyzer'
-]
-
-CLASSIFIERS = [
-    'Intended Audience :: Science/Research',
-    'License :: OSI Approved :: BSD License',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3 :: Only',
-    'Topic :: Scientific/Engineering',
-    'Topic :: Scientific/Engineering :: Visualization',
-    'Topic :: Scientific/Engineering :: Artificial Intelligence',
-    'Topic :: Multimedia :: Graphics',
-    'Framework :: Matplotlib',
-]
-
-with open('README.rst', 'r') as fp:
-    readme = fp.read()
-with open('CONTACT.txt', 'r') as fp:
-    contacts = fp.read()
-long_description = readme + '\n\n' + contacts
-
-setup(name=NAME,
-      author=AUTHOR,
-      author_email=AUTHOR_EMAIL,
-      maintainer=AUTHOR,
-      maintainer_email=AUTHOR_EMAIL,
-      description=DESCRIPTION,
-      long_description=long_description,
-      license=LICENSE,
-      url=URL,
-      version=VERSION,
-      download_url=DOWNLOAD_URL,
-      python_requires=PYTHON_REQUIRES,
-      install_requires=INSTALL_REQUIRES,
-      extras_require=EXTRAS_REQUIRE,
-      packages=PACKAGES,
-      classifiers=CLASSIFIERS
+# Author: Kenta Nakamura <c60evaporator@gmail.com>
+# Copyright (c) 2020-2021 Kenta Nakamura
+# License: BSD 3 clause
+
+from setuptools import setup
+import seaborn_analyzer
+
+DESCRIPTION = "seaborn-analyzer: data visualization of regression, classification and distribution"
+NAME = 'seaborn-analyzer'
+AUTHOR = 'Kenta Nakamura'
+AUTHOR_EMAIL = 'c60evaporator@gmail.com'
+URL = 'https://github.com/c60evaporator/seaborn-analyzer'
+LICENSE = 'BSD 3-Clause'
+DOWNLOAD_URL = 'https://github.com/c60evaporator/seaborn-analyzer'
+VERSION = seaborn_analyzer.__version__
+PYTHON_REQUIRES = ">=3.6"
+
+INSTALL_REQUIRES = [
+    'matplotlib>=3.7.1',
+    'seaborn>=0.12.2',
+    'numpy >=1.22.1',
+    'pandas>=2.0.2',
+    'scipy>=1.10.1',
+    'scikit-learn>=1.2.2',
+    'lightgbm>=3.3.5',
+]
+
+EXTRAS_REQUIRE = {
+    'tutorial': [
+        'mlxtend>=0.18.0',
+        'xgboost>=1.7.4',
+    ]
+}
+
+PACKAGES = [
+    'seaborn_analyzer'
+]
+
+CLASSIFIERS = [
+    'Intended Audience :: Science/Research',
+    'License :: OSI Approved :: BSD License',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3 :: Only',
+    'Topic :: Scientific/Engineering',
+    'Topic :: Scientific/Engineering :: Visualization',
+    'Topic :: Scientific/Engineering :: Artificial Intelligence',
+    'Topic :: Multimedia :: Graphics',
+    'Framework :: Matplotlib',
+]
+
+with open('README.rst', 'r') as fp:
+    readme = fp.read()
+with open('CONTACT.txt', 'r') as fp:
+    contacts = fp.read()
+long_description = readme + '\n\n' + contacts
+
+setup(name=NAME,
+      author=AUTHOR,
+      author_email=AUTHOR_EMAIL,
+      maintainer=AUTHOR,
+      maintainer_email=AUTHOR_EMAIL,
+      description=DESCRIPTION,
+      long_description=long_description,
+      license=LICENSE,
+      url=URL,
+      version=VERSION,
+      download_url=DOWNLOAD_URL,
+      python_requires=PYTHON_REQUIRES,
+      install_requires=INSTALL_REQUIRES,
+      extras_require=EXTRAS_REQUIRE,
+      packages=PACKAGES,
+      classifiers=CLASSIFIERS
     )
```

