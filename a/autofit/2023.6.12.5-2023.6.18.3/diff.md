# Comparing `tmp/autofit-2023.6.12.5.tar.gz` & `tmp/autofit-2023.6.18.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofit-2023.6.12.5.tar", last modified: Mon Jun 12 14:10:20 2023, max compression
+gzip compressed data, was "autofit-2023.6.18.3.tar", last modified: Sun Jun 18 22:19:01 2023, max compression
```

## Comparing `autofit-2023.6.12.5.tar` & `autofit-2023.6.18.3.tar`

### file list

```diff
@@ -1,289 +1,289 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.161580 autofit-2023.6.12.5/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/CITATIONS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-12 14:10:20.161580 autofit-2023.6.12.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.137586 autofit-2023.6.12.5/autofit/
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-06-12 14:10:09.000000 autofit-2023.6.12.5/autofit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.137586 autofit-2023.6.12.5/autofit/aggregator/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/aggregator/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8944 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/aggregator/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/aggregator/predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/aggregator/search_output.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.137586 autofit-2023.6.12.5/autofit/config/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/general.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/logging.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.137586 autofit-2023.6.12.5/autofit/config/non_linear/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/non_linear/GridSearch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/non_linear/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/non_linear/mcmc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/non_linear/nest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/non_linear/optimize.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/notation.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.141585 autofit-2023.6.12.5/autofit/config/priors/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/priors/Exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/priors/Gaussian.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/priors/GaussianKurtosis.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/priors/MultiLevelGaussians.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/priors/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/priors/model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/priors/prior.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/priors/profiles.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/priors/template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.141585 autofit-2023.6.12.5/autofit/config/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/visualize/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/visualize/general.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/config/visualize/plots_search.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.141585 autofit-2023.6.12.5/autofit/database/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.141585 autofit-2023.6.12.5/autofit/database/aggregator/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/aggregator/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/aggregator/scrape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.141585 autofit-2023.6.12.5/autofit/database/migration/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/migration/migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/migration/session_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/migration/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.141585 autofit-2023.6.12.5/autofit/database/model/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/model/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/model/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/model/prior.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.141585 autofit-2023.6.12.5/autofit/database/query/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/query/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/query/junction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.141585 autofit-2023.6.12.5/autofit/database/query/query/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/query/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/query/query/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/query/query/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/query/query/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/query/query/named.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/database/sqlalchemy_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.141585 autofit-2023.6.12.5/autofit/example/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/example/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/example/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/example/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.141585 autofit-2023.6.12.5/autofit/graphical/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.141585 autofit-2023.6.12.5/autofit/graphical/declarative/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/declarative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/declarative/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/declarative/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.145584 autofit-2023.6.12.5/autofit/graphical/declarative/factor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/declarative/factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/declarative/factor/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/declarative/factor/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/declarative/factor/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/declarative/factor/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/declarative/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/declarative/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.145584 autofit-2023.6.12.5/autofit/graphical/expectation_propagation/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/expectation_propagation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17242 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/expectation_propagation/ep_mean_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/expectation_propagation/factor_optimiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/expectation_propagation/history.py
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/expectation_propagation/optimiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/expectation_propagation/stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/expectation_propagation/visualise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.145584 autofit-2023.6.12.5/autofit/graphical/factor_graphs/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/factor_graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/factor_graphs/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/factor_graphs/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/factor_graphs/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/factor_graphs/jacobians.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/factor_graphs/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.145584 autofit-2023.6.12.5/autofit/graphical/laplace/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/laplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/laplace/line_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/laplace/newton.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/laplace/optimiser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18909 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/mean_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/graphical/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.145584 autofit-2023.6.12.5/autofit/interpolator/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/interpolator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/interpolator/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/interpolator/covariance.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/interpolator/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/interpolator/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/interpolator/spline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.145584 autofit-2023.6.12.5/autofit/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.145584 autofit-2023.6.12.5/autofit/mapper/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/mock/mock_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/model_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/model_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    23069 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.149583 autofit-2023.6.12.5/autofit/mapper/prior/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.149583 autofit-2023.6.12.5/autofit/mapper/prior/arithmetic/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior/arithmetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior/arithmetic/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior/arithmetic/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior/arithmetic/compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior/deferred.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior/log_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior/log_uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior/tuple_prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior/uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior/width_modifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.149583 autofit-2023.6.12.5/autofit/mapper/prior_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63313 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior_model/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior_model/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior_model/attribute_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior_model/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13987 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior_model/prior_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior_model/recursion.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/prior_model/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    19865 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mapper/variable_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.149583 autofit-2023.6.12.5/autofit/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14433 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/messages/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/messages/beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/messages/composed_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/messages/fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/messages/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/messages/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/messages/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/messages/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/messages/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.149583 autofit-2023.6.12.5/autofit/non_linear/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36116 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/abstract_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.153582 autofit-2023.6.12.5/autofit/non_linear/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12394 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/analysis/combined.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/analysis/free_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/analysis/indexed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/analysis/model_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/analysis/multiprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.153582 autofit-2023.6.12.5/autofit/non_linear/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/grid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.153582 autofit-2023.6.12.5/autofit/non_linear/grid/grid_search/
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/grid/grid_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/grid/grid_search/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/grid/grid_search/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/grid/grid_search/result_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/grid/sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/grid/simple_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.153582 autofit-2023.6.12.5/autofit/non_linear/mcmc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mcmc/abstract_mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mcmc/auto_correlations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.153582 autofit-2023.6.12.5/autofit/non_linear/mcmc/emcee/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mcmc/emcee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mcmc/emcee/emcee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mcmc/emcee/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mcmc/emcee/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.153582 autofit-2023.6.12.5/autofit/non_linear/mcmc/zeus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mcmc/zeus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mcmc/zeus/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mcmc/zeus/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mcmc/zeus/zeus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.153582 autofit-2023.6.12.5/autofit/non_linear/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mock/mock_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mock/mock_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mock/mock_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/mock/mock_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.153582 autofit-2023.6.12.5/autofit/non_linear/nest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/nest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/nest/abstract_nest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.153582 autofit-2023.6.12.5/autofit/non_linear/nest/dynesty/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/nest/dynesty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/nest/dynesty/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/nest/dynesty/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/nest/dynesty/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/nest/dynesty/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/nest/dynesty/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.157581 autofit-2023.6.12.5/autofit/non_linear/nest/ultranest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/nest/ultranest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/nest/ultranest/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/nest/ultranest/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/nest/ultranest/ultranest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.157581 autofit-2023.6.12.5/autofit/non_linear/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/optimize/abstract_optimize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.157581 autofit-2023.6.12.5/autofit/non_linear/optimize/drawer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/optimize/drawer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/optimize/drawer/drawer.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/optimize/drawer/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.157581 autofit-2023.6.12.5/autofit/non_linear/optimize/lbfgs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/optimize/lbfgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/optimize/lbfgs/lbfgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/optimize/lbfgs/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.157581 autofit-2023.6.12.5/autofit/non_linear/optimize/pyswarms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/optimize/pyswarms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9683 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/optimize/pyswarms/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/optimize/pyswarms/globe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/optimize/pyswarms/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/optimize/pyswarms/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/optimize/pyswarms/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.157581 autofit-2023.6.12.5/autofit/non_linear/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/parallel/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/parallel/sneaky.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.157581 autofit-2023.6.12.5/autofit/non_linear/paths/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/paths/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/paths/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/paths/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/paths/null.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/paths/sub_directory_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.157581 autofit-2023.6.12.5/autofit/non_linear/samples/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/samples/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/samples/nest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/samples/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/samples/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/samples/stored.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/non_linear/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.157581 autofit-2023.6.12.5/autofit/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/plot/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/plot/samples_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.161580 autofit-2023.6.12.5/autofit/text/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/text/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/text/samples_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/text/text_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.161580 autofit-2023.6.12.5/autofit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/tools/add_notebook_quotes.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/tools/namer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/tools/update_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/autofit/tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.161580 autofit-2023.6.12.5/autofit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-06-12 14:10:20.000000 autofit-2023.6.12.5/autofit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:20.161580 autofit-2023.6.12.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:09.000000 autofit-2023.6.12.5/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/scripts/add_notebook_quotes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      268 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/scripts/aggregate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/scripts/update_identifiers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/scripts/update_identifiers_from_file.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-12 14:10:20.161580 autofit-2023.6.12.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-12 14:10:08.000000 autofit-2023.6.12.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.252185 autofit-2023.6.18.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/CITATIONS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-06-18 22:19:01.252185 autofit-2023.6.18.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.216183 autofit-2023.6.18.3/autofit/
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/aggregator/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/aggregator/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8944 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/aggregator/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/aggregator/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/aggregator/search_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/general.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/logging.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/config/non_linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/non_linear/GridSearch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/non_linear/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/non_linear/mcmc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/non_linear/nest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/non_linear/optimize.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/notation.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/config/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/Exponential.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/Gaussian.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/GaussianKurtosis.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/MultiLevelGaussians.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/prior.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/profiles.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/config/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/visualize/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/visualize/general.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/visualize/plots_search.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/database/aggregator/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/aggregator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/aggregator/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/aggregator/scrape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/database/migration/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/migration/migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/migration/session_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/migration/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/database/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/model/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/model/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/model/prior.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/database/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/junction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/database/query/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/query/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/query/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/query/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/query/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/sqlalchemy_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/example/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/example/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/example/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/graphical/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/graphical/declarative/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/graphical/declarative/factor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/factor/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/factor/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/factor/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/factor/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17242 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/ep_mean_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/factor_optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/visualise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/graphical/factor_graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/factor_graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/factor_graphs/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/factor_graphs/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/factor_graphs/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/factor_graphs/jacobians.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/factor_graphs/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.228184 autofit-2023.6.18.3/autofit/graphical/laplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/laplace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/laplace/line_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/laplace/newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/laplace/optimiser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18909 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/mean_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.228184 autofit-2023.6.18.3/autofit/interpolator/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/interpolator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/interpolator/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/interpolator/covariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/interpolator/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/interpolator/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/interpolator/spline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.228184 autofit-2023.6.18.3/autofit/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.228184 autofit-2023.6.18.3/autofit/mapper/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/mock/mock_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/model_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/model_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23069 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.228184 autofit-2023.6.18.3/autofit/mapper/prior/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.232184 autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/log_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/log_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/tuple_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/width_modifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.232184 autofit-2023.6.18.3/autofit/mapper/prior_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63313 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/attribute_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13987 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/prior_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/recursion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19865 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/variable_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.232184 autofit-2023.6.18.3/autofit/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14433 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/composed_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.236184 autofit-2023.6.18.3/autofit/non_linear/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38933 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/abstract_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.236184 autofit-2023.6.18.3/autofit/non_linear/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12394 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/analysis/combined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/analysis/free_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/analysis/indexed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/analysis/model_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/analysis/multiprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.236184 autofit-2023.6.18.3/autofit/non_linear/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/grid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.236184 autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/result_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/grid/sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/grid/simple_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.236184 autofit-2023.6.18.3/autofit/non_linear/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/abstract_mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/auto_correlations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.240184 autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/emcee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.240184 autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/zeus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.240184 autofit-2023.6.18.3/autofit/non_linear/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mock/mock_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mock/mock_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mock/mock_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mock/mock_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.240184 autofit-2023.6.18.3/autofit/non_linear/nest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/abstract_nest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.240184 autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.244184 autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/ultranest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.244184 autofit-2023.6.18.3/autofit/non_linear/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/abstract_optimize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.244184 autofit-2023.6.18.3/autofit/non_linear/optimize/drawer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/drawer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/drawer/drawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/drawer/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.244184 autofit-2023.6.18.3/autofit/non_linear/optimize/lbfgs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/lbfgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/lbfgs/lbfgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/lbfgs/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.244184 autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9683 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/globe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.244184 autofit-2023.6.18.3/autofit/non_linear/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/parallel/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/parallel/sneaky.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.244184 autofit-2023.6.18.3/autofit/non_linear/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/paths/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/paths/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/paths/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/paths/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/paths/sub_directory_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.248185 autofit-2023.6.18.3/autofit/non_linear/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/samples/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/samples/nest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/samples/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/samples/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/samples/stored.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.248185 autofit-2023.6.18.3/autofit/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/plot/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/plot/samples_plotters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.248185 autofit-2023.6.18.3/autofit/text/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/text/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/text/samples_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/text/text_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.248185 autofit-2023.6.18.3/autofit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/tools/add_notebook_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/tools/namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/tools/update_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/tools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.252185 autofit-2023.6.18.3/autofit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-06-18 22:19:01.000000 autofit-2023.6.18.3/autofit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.252185 autofit-2023.6.18.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/scripts/add_notebook_quotes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      268 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/scripts/aggregate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/scripts/update_identifiers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/scripts/update_identifiers_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-18 22:19:01.252185 autofit-2023.6.18.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/setup.py
```

### Comparing `autofit-2023.6.12.5/CITATIONS.rst` & `autofit-2023.6.18.3/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/LICENSE` & `autofit-2023.6.18.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/PKG-INFO` & `autofit-2023.6.18.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofit
-Version: 2023.6.12.5
+Version: 2023.6.18.3
 Summary: Classy Probabilistic Programming
 Home-page: https://github.com/rhayes777/PyAutoFit
 Author: James Nightingale and Richard Hayes
 Author-email: richard@rghsoftware.co.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
@@ -66,15 +66,15 @@
 
 The following links are useful for new starters:
 
 - `The introduction Jupyter Notebook on Binder <https://mybinder.org/v2/gh/Jammy2211/autofit_workspace/release?filepath=introduction.ipynb>`_, where you can try **PyAutoFit** in a web browser (without installation).
 
 - `The PyAutoFit readthedocs <https://pyautofit.readthedocs.io/en/latest>`_, which includes an `installation guide <https://pyautofit.readthedocs.io/en/latest/installation/overview.html>`_ and an overview of **PyAutoFit**'s core features.
 
-- `The autofit_workspace GitHub repository <https://github.com/Jammy2211/autofit_workspace>`_, which includes example scripts and the `HowToFit Jupyter notebook tutorials <https://github.com/Jammy2211/autofit_workspace/tree/master/notebooks/howtofit>`_ which give new users a step-by-step introduction to **PyAutoFit**.
+- `The autofit_workspace GitHub repository <https://github.com/Jammy2211/autofit_workspace>`_, which includes example scripts and the `HowToFit Jupyter notebook lectures <https://github.com/Jammy2211/autofit_workspace/tree/master/notebooks/howtofit>`_ which give new users a step-by-step introduction to **PyAutoFit**.
 
 Why PyAutoFit?
 --------------
 
 **PyAutoFit** began as an Astronomy project for fitting large imaging datasets of galaxies after the developers found that existing PPLs
 (e.g., `PyMC3 <https://github.com/pymc-devs/pymc3>`_, `Pyro <https://github.com/pyro-ppl/pyro>`_, `STAN <https://github.com/stan-dev/stan>`_)
 were not suited to the model fitting problems many Astronomers faced. This includes:
```

### Comparing `autofit-2023.6.12.5/README.rst` & `autofit-2023.6.18.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 The following links are useful for new starters:
 
 - `The introduction Jupyter Notebook on Binder <https://mybinder.org/v2/gh/Jammy2211/autofit_workspace/release?filepath=introduction.ipynb>`_, where you can try **PyAutoFit** in a web browser (without installation).
 
 - `The PyAutoFit readthedocs <https://pyautofit.readthedocs.io/en/latest>`_, which includes an `installation guide <https://pyautofit.readthedocs.io/en/latest/installation/overview.html>`_ and an overview of **PyAutoFit**'s core features.
 
-- `The autofit_workspace GitHub repository <https://github.com/Jammy2211/autofit_workspace>`_, which includes example scripts and the `HowToFit Jupyter notebook tutorials <https://github.com/Jammy2211/autofit_workspace/tree/master/notebooks/howtofit>`_ which give new users a step-by-step introduction to **PyAutoFit**.
+- `The autofit_workspace GitHub repository <https://github.com/Jammy2211/autofit_workspace>`_, which includes example scripts and the `HowToFit Jupyter notebook lectures <https://github.com/Jammy2211/autofit_workspace/tree/master/notebooks/howtofit>`_ which give new users a step-by-step introduction to **PyAutoFit**.
 
 Why PyAutoFit?
 --------------
 
 **PyAutoFit** began as an Astronomy project for fitting large imaging datasets of galaxies after the developers found that existing PPLs
 (e.g., `PyMC3 <https://github.com/pymc-devs/pymc3>`_, `Pyro <https://github.com/pyro-ppl/pyro>`_, `STAN <https://github.com/stan-dev/stan>`_)
 were not suited to the model fitting problems many Astronomers faced. This includes:
```

### Comparing `autofit-2023.6.12.5/autofit/__init__.py` & `autofit-2023.6.18.3/autofit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,8 +110,9 @@
 @register(abc.ABCMeta)
 def save_abc(pickler, obj):
     pickle._Pickler.save_type(pickler, obj)
 
 
 conf.instance.register(__file__)
 
-__version__ = "2023.6.12.5"
+__version__ = "2023.6.18.3"
+
```

### Comparing `autofit-2023.6.12.5/autofit/aggregator/aggregator.py` & `autofit-2023.6.18.3/autofit/aggregator/aggregator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/aggregator/predicate.py` & `autofit-2023.6.18.3/autofit/aggregator/predicate.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/aggregator/search_output.py` & `autofit-2023.6.18.3/autofit/aggregator/search_output.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/config/README.rst` & `autofit-2023.6.18.3/autofit/config/README.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/config/general.yaml` & `autofit-2023.6.18.3/autofit/config/general.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/config/non_linear/mcmc.yaml` & `autofit-2023.6.18.3/autofit/config/non_linear/mcmc.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/config/non_linear/nest.yaml` & `autofit-2023.6.18.3/autofit/config/non_linear/nest.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/config/non_linear/optimize.yaml` & `autofit-2023.6.18.3/autofit/config/non_linear/optimize.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/config/notation.yaml` & `autofit-2023.6.18.3/autofit/config/notation.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/config/priors/Gaussian.yaml` & `autofit-2023.6.18.3/autofit/config/priors/Gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/config/priors/GaussianKurtosis.yaml` & `autofit-2023.6.18.3/autofit/config/priors/GaussianKurtosis.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/config/priors/README.rst` & `autofit-2023.6.18.3/autofit/config/priors/README.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/config/priors/model.yaml` & `autofit-2023.6.18.3/autofit/config/priors/model.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/config/priors/profiles.yaml` & `autofit-2023.6.18.3/autofit/config/priors/profiles.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/config/priors/template.yaml` & `autofit-2023.6.18.3/autofit/config/priors/template.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/config/visualize/plots_search.yaml` & `autofit-2023.6.18.3/autofit/config/visualize/plots_search.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/__init__.py` & `autofit-2023.6.18.3/autofit/database/__init__.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/aggregator/aggregator.py` & `autofit-2023.6.18.3/autofit/database/aggregator/aggregator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/aggregator/scrape.py` & `autofit-2023.6.18.3/autofit/database/aggregator/scrape.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/migration/migration.py` & `autofit-2023.6.18.3/autofit/database/migration/migration.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/migration/session_wrapper.py` & `autofit-2023.6.18.3/autofit/database/migration/session_wrapper.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/model/fit.py` & `autofit-2023.6.18.3/autofit/database/model/fit.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/model/instance.py` & `autofit-2023.6.18.3/autofit/database/model/instance.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/model/model.py` & `autofit-2023.6.18.3/autofit/database/model/model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/model/prior.py` & `autofit-2023.6.18.3/autofit/database/model/prior.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/query/condition.py` & `autofit-2023.6.18.3/autofit/database/query/condition.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/query/junction.py` & `autofit-2023.6.18.3/autofit/database/query/junction.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/query/query/abstract.py` & `autofit-2023.6.18.3/autofit/database/query/query/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/query/query/attribute.py` & `autofit-2023.6.18.3/autofit/database/query/query/attribute.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/query/query/info.py` & `autofit-2023.6.18.3/autofit/database/query/query/info.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/query/query/named.py` & `autofit-2023.6.18.3/autofit/database/query/query/named.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/database/sqlalchemy_.py` & `autofit-2023.6.18.3/autofit/database/sqlalchemy_.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/example/analysis.py` & `autofit-2023.6.18.3/autofit/example/analysis.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/example/model.py` & `autofit-2023.6.18.3/autofit/example/model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/example/util.py` & `autofit-2023.6.18.3/autofit/example/util.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/exc.py` & `autofit-2023.6.18.3/autofit/exc.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/fixtures.py` & `autofit-2023.6.18.3/autofit/fixtures.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/__init__.py` & `autofit-2023.6.18.3/autofit/graphical/__init__.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/declarative/abstract.py` & `autofit-2023.6.18.3/autofit/graphical/declarative/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/declarative/collection.py` & `autofit-2023.6.18.3/autofit/graphical/declarative/collection.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/declarative/factor/abstract.py` & `autofit-2023.6.18.3/autofit/graphical/declarative/factor/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/declarative/factor/analysis.py` & `autofit-2023.6.18.3/autofit/graphical/declarative/factor/analysis.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/declarative/factor/hierarchical.py` & `autofit-2023.6.18.3/autofit/graphical/declarative/factor/hierarchical.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/declarative/factor/prior.py` & `autofit-2023.6.18.3/autofit/graphical/declarative/factor/prior.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/declarative/graph.py` & `autofit-2023.6.18.3/autofit/graphical/declarative/graph.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/declarative/result.py` & `autofit-2023.6.18.3/autofit/graphical/declarative/result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/expectation_propagation/ep_mean_field.py` & `autofit-2023.6.18.3/autofit/graphical/expectation_propagation/ep_mean_field.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/expectation_propagation/factor_optimiser.py` & `autofit-2023.6.18.3/autofit/graphical/expectation_propagation/factor_optimiser.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/expectation_propagation/history.py` & `autofit-2023.6.18.3/autofit/graphical/expectation_propagation/history.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/expectation_propagation/optimiser.py` & `autofit-2023.6.18.3/autofit/graphical/expectation_propagation/optimiser.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/expectation_propagation/stochastic.py` & `autofit-2023.6.18.3/autofit/graphical/expectation_propagation/stochastic.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/expectation_propagation/visualise.py` & `autofit-2023.6.18.3/autofit/graphical/expectation_propagation/visualise.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/factor_graphs/abstract.py` & `autofit-2023.6.18.3/autofit/graphical/factor_graphs/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/factor_graphs/factor.py` & `autofit-2023.6.18.3/autofit/graphical/factor_graphs/factor.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/factor_graphs/graph.py` & `autofit-2023.6.18.3/autofit/graphical/factor_graphs/graph.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/factor_graphs/jacobians.py` & `autofit-2023.6.18.3/autofit/graphical/factor_graphs/jacobians.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/factor_graphs/transform.py` & `autofit-2023.6.18.3/autofit/graphical/factor_graphs/transform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/laplace/line_search.py` & `autofit-2023.6.18.3/autofit/graphical/laplace/line_search.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/laplace/newton.py` & `autofit-2023.6.18.3/autofit/graphical/laplace/newton.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/laplace/optimiser.py` & `autofit-2023.6.18.3/autofit/graphical/laplace/optimiser.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/mean_field.py` & `autofit-2023.6.18.3/autofit/graphical/mean_field.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/graphical/utils.py` & `autofit-2023.6.18.3/autofit/graphical/utils.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/interpolator/abstract.py` & `autofit-2023.6.18.3/autofit/interpolator/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/interpolator/covariance.py` & `autofit-2023.6.18.3/autofit/interpolator/covariance.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/interpolator/query.py` & `autofit-2023.6.18.3/autofit/interpolator/query.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/identifier.py` & `autofit-2023.6.18.3/autofit/mapper/identifier.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/mock/mock_model.py` & `autofit-2023.6.18.3/autofit/mapper/mock/mock_model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/model.py` & `autofit-2023.6.18.3/autofit/mapper/model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/model_mapper.py` & `autofit-2023.6.18.3/autofit/mapper/model_mapper.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/model_object.py` & `autofit-2023.6.18.3/autofit/mapper/model_object.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/operator.py` & `autofit-2023.6.18.3/autofit/mapper/operator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior/abstract.py` & `autofit-2023.6.18.3/autofit/mapper/prior/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior/arithmetic/arithmetic.py` & `autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/arithmetic.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior/arithmetic/assertion.py` & `autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/assertion.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior/arithmetic/compound.py` & `autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/compound.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior/deferred.py` & `autofit-2023.6.18.3/autofit/mapper/prior/deferred.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior/gaussian.py` & `autofit-2023.6.18.3/autofit/mapper/prior/gaussian.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior/log_gaussian.py` & `autofit-2023.6.18.3/autofit/mapper/prior/log_gaussian.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior/log_uniform.py` & `autofit-2023.6.18.3/autofit/mapper/prior/log_uniform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior/tuple_prior.py` & `autofit-2023.6.18.3/autofit/mapper/prior/tuple_prior.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior/uniform.py` & `autofit-2023.6.18.3/autofit/mapper/prior/uniform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior/width_modifier.py` & `autofit-2023.6.18.3/autofit/mapper/prior/width_modifier.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior_model/abstract.py` & `autofit-2023.6.18.3/autofit/mapper/prior_model/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior_model/annotation.py` & `autofit-2023.6.18.3/autofit/mapper/prior_model/annotation.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior_model/attribute_pair.py` & `autofit-2023.6.18.3/autofit/mapper/prior_model/attribute_pair.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior_model/collection.py` & `autofit-2023.6.18.3/autofit/mapper/prior_model/collection.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior_model/prior_model.py` & `autofit-2023.6.18.3/autofit/mapper/prior_model/prior_model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/prior_model/recursion.py` & `autofit-2023.6.18.3/autofit/mapper/prior_model/recursion.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/variable.py` & `autofit-2023.6.18.3/autofit/mapper/variable.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mapper/variable_operator.py` & `autofit-2023.6.18.3/autofit/mapper/variable_operator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/messages/abstract.py` & `autofit-2023.6.18.3/autofit/messages/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/messages/beta.py` & `autofit-2023.6.18.3/autofit/messages/beta.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/messages/composed_transform.py` & `autofit-2023.6.18.3/autofit/messages/composed_transform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/messages/fixed.py` & `autofit-2023.6.18.3/autofit/messages/fixed.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/messages/gamma.py` & `autofit-2023.6.18.3/autofit/messages/gamma.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/messages/interface.py` & `autofit-2023.6.18.3/autofit/messages/interface.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/messages/normal.py` & `autofit-2023.6.18.3/autofit/messages/normal.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/messages/transform.py` & `autofit-2023.6.18.3/autofit/messages/transform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/messages/utils.py` & `autofit-2023.6.18.3/autofit/messages/utils.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/mock.py` & `autofit-2023.6.18.3/autofit/mock.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/abstract_search.py` & `autofit-2023.6.18.3/autofit/non_linear/abstract_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,14 +142,18 @@
 
         self.prior_passer = prior_passer or PriorPasser.from_config(config=self._config)
 
         self.force_pickle_overwrite = conf.instance["general"]["output"][
             "force_pickle_overwrite"
         ]
 
+        self.force_visualize_overwrite = conf.instance["general"]["output"][
+            "force_visualize_overwrite"
+        ]
+
         if initializer is None:
             self.logger.debug("Creating initializer ")
             self.initializer = Initializer.from_config(config=self._config)
         else:
             self.initializer = initializer
 
         self.iterations_per_update = iterations_per_update or self._config(
@@ -573,20 +577,22 @@
         model = analysis.modify_model(model)
         self.paths.model = model
         self.paths.unique_tag = self.unique_tag
         self.paths.restore()
 
         analysis = analysis.modify_before_fit(paths=self.paths, model=model)
 
-        analysis.visualize_before_fit(
-            paths=self.paths, model=model,
-        )
-        analysis.visualize_before_fit_combined(
-            analyses=None, paths=self.paths, model=model,
-        )
+        if analysis.should_visualize(paths=self.paths):
+
+            analysis.visualize_before_fit(
+                paths=self.paths, model=model,
+            )
+            analysis.visualize_before_fit_combined(
+                analyses=None, paths=self.paths, model=model,
+            )
 
         if not self.paths.is_complete or self.force_pickle_overwrite:
             self.logger.info("Saving path info")
 
             self.paths.save_all(
                 search_config_dict=self.config_dict_search,
                 info=info,
@@ -624,14 +630,17 @@
             self.paths.save_object("samples", samples)
 
         else:
             self.logger.info(f"Already completed, skipping non-linear search.")
 
             samples = self.paths.load_object("samples")
 
+            if self.force_visualize_overwrite:
+                self.perform_visualization(model=model, analysis=analysis, during_analysis=False)
+
             result = analysis.make_result(
                 samples=samples,
                 model=model,
                 sigma=self.prior_passer.sigma,
                 use_errors=self.prior_passer.use_errors,
                 use_widths=self.prior_passer.use_widths,
             )
@@ -729,60 +738,58 @@
         Returns
         -------
         attribute
             An attribute for the key with the specified type.
         """
         return self._class_config[section][attribute_name]
 
-    def perform_update(self, model, analysis, during_analysis):
+    def perform_update(self, model : Collection, analysis : Analysis, during_analysis : bool):
         """
-        Perform an update of the `NonLinearSearch` results, which occurs every *iterations_per_update* of the
-        non-linear search. The update performs the following tasks:
+        Perform an update of the non-linear search's model-fitting results.
+
+        This occurs every `iterations_per_update` of the non-linear search and once it is complete.
 
-        1) Visualize the maximum log likelihood model.
-        2) Output the model results to the model.reults file.
+        The update performs the following tasks (if the settings indicate they should be performed):
+
+        1) Visualize the search results (e.g. a cornerplot).
+        2) Visualize the maximum log likelihood model using model-specific visualization implented via the `Analysis`
+           object.
+        3) Perform profiling of the analysis object `log_likelihood_function` and ouptut run-time information.
+        4) Output the `search.summary` file which contains information on model-fitting so far.
+        5) Output the `model.results` file which contains a concise text summary of the model results so far.
 
         Parameters
         ----------
-        model : ModelMapper
+        model
             The model which generates instances for different points in parameter space.
-        analysis : Analysis
+        analysis
             Contains the data and the log likelihood function which fits an instance of the model to the data, returning
             the log likelihood the `NonLinearSearch` maximizes.
         during_analysis
             If the update is during a non-linear search, in which case tasks are only performed after a certain number
-             of updates and only a subset of visualization may be performed.
+            of updates and only a subset of visualization may be performed.
         """
 
         self.iterations += self.iterations_per_update
         self.logger.info(
             f"{self.iterations} Iterations: Performing update (Visualization, outputting samples, etc.)."
         )
 
         self.timer.update()
 
         samples = self.samples_from(model=model)
 
         self.paths.save_object("samples", samples)
 
-        if not isinstance(self.paths, NullPaths):
-            self.plot_results(samples=samples)
-
         try:
             instance = samples.max_log_likelihood()
         except exc.FitException:
             return samples
 
-        self.logger.debug("Visualizing")
-        analysis.visualize(
-            paths=self.paths, instance=instance, during_analysis=during_analysis
-        )
-        analysis.visualize_combined(
-            analyses=None, paths=self.paths, instance=instance, during_analysis=during_analysis
-        )
+        self.perform_visualization(model=model, analysis=analysis, during_analysis=during_analysis)
 
         if self.should_profile:
             self.logger.debug("Profiling Maximum Likelihood Model")
             analysis.profile_log_likelihood_function(
                 paths=self.paths, instance=instance,
             )
 
@@ -805,14 +812,62 @@
             try:
                 self.remove_state_files()
             except FileNotFoundError:
                 pass
 
         return samples
 
+    def perform_visualization(self, model, analysis, during_analysis):
+        """
+        Perform visualization of the non-linear search's model-fitting results.
+
+        This occurs every `iterations_per_update` of the non-linear search, when the search is complete and can
+        also be forced to occur even though a search is completed on a rerun, to update the visualization
+        with different `matplotlib` settings.
+
+        The update performs the following tasks (if the settings indicate they should be performed):
+
+        1) Visualize the search results (e.g. a cornerplot).
+        2) Visualize the maximum log likelihood model using model-specific visualization implented via the `Analysis`
+           object.
+
+        Parameters
+        ----------
+        model
+            The model which generates instances for different points in parameter space.
+        analysis
+            Contains the data and the log likelihood function which fits an instance of the model to the data, returning
+            the log likelihood the `NonLinearSearch` maximizes.
+        during_analysis
+            If the update is during a non-linear search, in which case tasks are only performed after a certain number
+            of updates and only a subset of visualization may be performed.
+        """
+        try:
+            samples = self.samples_from(model=model)
+        except FileNotFoundError:
+            samples = self.paths.load_object(name="samples")
+
+        try:
+            instance = samples.max_log_likelihood()
+        except exc.FitException:
+            return samples
+
+        if analysis.should_visualize(paths=self.paths, during_analysis=during_analysis):
+            if not isinstance(self.paths, NullPaths):
+                self.plot_results(samples=samples)
+
+        self.logger.debug("Visualizing")
+        if analysis.should_visualize(paths=self.paths, during_analysis=during_analysis):
+            analysis.visualize(
+                paths=self.paths, instance=instance, during_analysis=during_analysis
+            )
+            analysis.visualize_combined(
+                analyses=None, paths=self.paths, instance=instance, during_analysis=during_analysis
+            )
+
     @property
     def samples_cls(self):
         raise NotImplementedError()
 
     def remove_state_files(self):
         pass
```

### Comparing `autofit-2023.6.12.5/autofit/non_linear/analysis/analysis.py` & `autofit-2023.6.18.3/autofit/non_linear/analysis/analysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,24 +37,28 @@
         """
         from .model_analysis import ModelAnalysis
         return ModelAnalysis(
             analysis=self,
             model=model
         )
 
-    def should_visualize(self, paths: AbstractPaths) -> bool:
+    def should_visualize(self, paths: AbstractPaths, during_analysis : bool = True) -> bool:
         """
-        Whether a visualize method should continue and perform visualization, or be terminated early.
+        Whether a visualize method should be called perform visualization, which depends on the following:
 
-        If a model-fit has already completed, the default behaviour is for visualization to be bypassed in order
-        to make model-fits run faster. However, visualization can be forced to run via
-        the `force_visualization_overwrite`, for example if a user wants to plot additional images that were not
-        output on the original run.
+        1) If a model-fit has already completed, the default behaviour is for visualization to be bypassed in order
+        to make model-fits run faster.
 
-        PyAutoFit test mode also disables visualization, irrespective of the `force_visualization_overwite`
+        2) If a model-fit has completed, but it is the final visualization output where `during_analysis` is False,
+        it should be performed.
+
+        3) Visualization can be forced to run via the `force_visualization_overwrite`, for example if a user
+        wants to plot additional images that were not output on the original run.
+
+        4) If PyAutoFit test mode is on visualization is disabled, irrespective of the `force_visualization_overwite`
         config input.
 
         Parameters
         ----------
         paths
             The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
             visualization and the pickled objects used by the aggregator output by this function.
@@ -64,15 +68,21 @@
         -------
         A bool determining whether visualization should be performed or not.
         """
 
         if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
             return False
 
-        return not paths.is_complete or conf.instance["general"]["output"]["force_visualize_overwrite"]
+        if conf.instance["general"]["output"]["force_visualize_overwrite"]:
+            return True
+
+        if not during_analysis:
+            return True
+
+        return not paths.is_complete
 
     def log_likelihood_function(self, instance):
         raise NotImplementedError()
 
     def visualize_before_fit(self, paths: AbstractPaths, model: AbstractPriorModel):
         pass
```

### Comparing `autofit-2023.6.12.5/autofit/non_linear/analysis/combined.py` & `autofit-2023.6.18.3/autofit/non_linear/analysis/combined.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/analysis/free_parameter.py` & `autofit-2023.6.18.3/autofit/non_linear/analysis/free_parameter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/analysis/indexed.py` & `autofit-2023.6.18.3/autofit/non_linear/analysis/indexed.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/analysis/model_analysis.py` & `autofit-2023.6.18.3/autofit/non_linear/analysis/model_analysis.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/analysis/multiprocessing.py` & `autofit-2023.6.18.3/autofit/non_linear/analysis/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/grid/grid_search/__init__.py` & `autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/__init__.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/grid/grid_search/job.py` & `autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/job.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/grid/grid_search/result.py` & `autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/grid/grid_search/result_builder.py` & `autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/result_builder.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/grid/sensitivity.py` & `autofit-2023.6.18.3/autofit/non_linear/grid/sensitivity.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/grid/simple_grid.py` & `autofit-2023.6.18.3/autofit/non_linear/grid/simple_grid.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/initializer.py` & `autofit-2023.6.18.3/autofit/non_linear/initializer.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/mcmc/abstract_mcmc.py` & `autofit-2023.6.18.3/autofit/non_linear/mcmc/abstract_mcmc.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/mcmc/auto_correlations.py` & `autofit-2023.6.18.3/autofit/non_linear/mcmc/auto_correlations.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/mcmc/emcee/emcee.py` & `autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/emcee.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/mcmc/emcee/plotter.py` & `autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/mcmc/emcee/samples.py` & `autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/mcmc/zeus/plotter.py` & `autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/mcmc/zeus/samples.py` & `autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/mcmc/zeus/zeus.py` & `autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/zeus.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/mock/mock_analysis.py` & `autofit-2023.6.18.3/autofit/non_linear/mock/mock_analysis.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/mock/mock_result.py` & `autofit-2023.6.18.3/autofit/non_linear/mock/mock_result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/mock/mock_samples.py` & `autofit-2023.6.18.3/autofit/non_linear/mock/mock_samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/mock/mock_search.py` & `autofit-2023.6.18.3/autofit/non_linear/mock/mock_search.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/nest/abstract_nest.py` & `autofit-2023.6.18.3/autofit/non_linear/nest/abstract_nest.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/nest/dynesty/abstract.py` & `autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -432,15 +432,19 @@
                 path=path.join(self.paths.image_path, "search"), format="png"
             ),
         )
 
         if should_plot("cornerplot"):
             plotter.cornerplot()
 
-        if should_plot("runplot"):
-            plotter.runplot()
-
         if should_plot("traceplot"):
             plotter.traceplot()
 
-        if should_plot("cornerpoints"):
-            plotter.cornerpoints()
+        # There is currently a bug internal in dynesty where the matplotlib figure produced after these plots
+        # is not closed, and has weird extra stuff on. I have commented these out for now, in the hope that dynesty
+        # fix this bug in the future.
+
+        # if should_plot("runplot"):
+        #     plotter.runplot()
+
+        # if should_plot("cornerpoints"):
+        #     plotter.cornerpoints()
```

### Comparing `autofit-2023.6.12.5/autofit/non_linear/nest/dynesty/dynamic.py` & `autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/dynamic.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/nest/dynesty/plotter.py` & `autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/nest/dynesty/samples.py` & `autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/nest/dynesty/static.py` & `autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/static.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/nest/ultranest/plotter.py` & `autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/nest/ultranest/samples.py` & `autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/nest/ultranest/ultranest.py` & `autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/ultranest.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/optimize/abstract_optimize.py` & `autofit-2023.6.18.3/autofit/non_linear/optimize/abstract_optimize.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/optimize/drawer/drawer.py` & `autofit-2023.6.18.3/autofit/non_linear/optimize/drawer/drawer.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/optimize/lbfgs/lbfgs.py` & `autofit-2023.6.18.3/autofit/non_linear/optimize/lbfgs/lbfgs.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/optimize/lbfgs/samples.py` & `autofit-2023.6.18.3/autofit/non_linear/optimize/lbfgs/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/optimize/pyswarms/abstract.py` & `autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/optimize/pyswarms/globe.py` & `autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/globe.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/optimize/pyswarms/local.py` & `autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/local.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/optimize/pyswarms/plotter.py` & `autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/optimize/pyswarms/samples.py` & `autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/parallel/process.py` & `autofit-2023.6.18.3/autofit/non_linear/parallel/process.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/parallel/sneaky.py` & `autofit-2023.6.18.3/autofit/non_linear/parallel/sneaky.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/paths/abstract.py` & `autofit-2023.6.18.3/autofit/non_linear/paths/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/paths/database.py` & `autofit-2023.6.18.3/autofit/non_linear/paths/database.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/paths/directory.py` & `autofit-2023.6.18.3/autofit/non_linear/paths/directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import json
 import os
 import shutil
 from os import path
 from typing import Optional
+import logging
 
 import dill
 
 from autoconf import conf
 from autofit.text import formatter
 from autofit.tools.util import open_
 from .abstract import AbstractPaths
 from ..samples import load_from_table
 from autofit.non_linear.samples.pdf import SamplesPDF
 
+logger = logging.getLogger(__name__)
+
 
 class DirectoryPaths(AbstractPaths):
     def save_named_instance(self, name: str, instance):
         """
         Save an instance, such as that at a given sigma
         """
         self.save_object(name, instance)
@@ -100,15 +103,20 @@
         """
         Save the final-result samples associated with the phase as a pickle
         """
         if conf.instance["general"]["output"]["samples_to_csv"]:
             samples.write_table(filename=self._samples_file)
             samples.info_to_json(filename=self._info_file)
             if isinstance(samples, SamplesPDF):
-                samples.save_covariance_matrix(self._covariance_file)
+                try:
+                    samples.save_covariance_matrix(self._covariance_file)
+                except ValueError as e:
+                    logger.warning(
+                        f"Could not save covariance matrix because of the following error:\n{e}"
+                    )
 
     def load_samples_info(self):
         with open_(self._info_file) as infile:
             return json.load(infile)
 
     def save_all(self, search_config_dict=None, info=None, pickle_files=None):
         search_config_dict = search_config_dict or {}
```

### Comparing `autofit-2023.6.12.5/autofit/non_linear/paths/null.py` & `autofit-2023.6.18.3/autofit/non_linear/paths/null.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/paths/sub_directory_paths.py` & `autofit-2023.6.18.3/autofit/non_linear/paths/sub_directory_paths.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/result.py` & `autofit-2023.6.18.3/autofit/non_linear/result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/samples/mcmc.py` & `autofit-2023.6.18.3/autofit/non_linear/samples/mcmc.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/samples/nest.py` & `autofit-2023.6.18.3/autofit/non_linear/samples/nest.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/samples/pdf.py` & `autofit-2023.6.18.3/autofit/non_linear/samples/pdf.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/samples/sample.py` & `autofit-2023.6.18.3/autofit/non_linear/samples/sample.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/samples/samples.py` & `autofit-2023.6.18.3/autofit/non_linear/samples/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/samples/stored.py` & `autofit-2023.6.18.3/autofit/non_linear/samples/stored.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/settings.py` & `autofit-2023.6.18.3/autofit/non_linear/settings.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/non_linear/timer.py` & `autofit-2023.6.18.3/autofit/non_linear/timer.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/plot/output.py` & `autofit-2023.6.18.3/autofit/plot/output.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/plot/samples_plotters.py` & `autofit-2023.6.18.3/autofit/plot/samples_plotters.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/text/formatter.py` & `autofit-2023.6.18.3/autofit/text/formatter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/text/samples_text.py` & `autofit-2023.6.18.3/autofit/text/samples_text.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/text/text_util.py` & `autofit-2023.6.18.3/autofit/text/text_util.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/tools/add_notebook_quotes.py` & `autofit-2023.6.18.3/autofit/tools/add_notebook_quotes.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/tools/update_identifiers.py` & `autofit-2023.6.18.3/autofit/tools/update_identifiers.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit/tools/util.py` & `autofit-2023.6.18.3/autofit/tools/util.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/autofit.egg-info/SOURCES.txt` & `autofit-2023.6.18.3/autofit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/scripts/update_identifiers.py` & `autofit-2023.6.18.3/scripts/update_identifiers.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/scripts/update_identifiers_from_file.py` & `autofit-2023.6.18.3/scripts/update_identifiers_from_file.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.12.5/setup.py` & `autofit-2023.6.18.3/setup.py`

 * *Files identical despite different names*

