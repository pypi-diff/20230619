# Comparing `tmp/Psychofit-1.0.0.tar.gz` & `tmp/Psychofit-1.0.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Psychofit-1.0.0.tar", last modified: Fri Jun 16 17:24:23 2023, max compression
+gzip compressed data, was "Psychofit-1.0.0.post0.tar", last modified: Mon Jun 19 10:09:11 2023, max compression
```

## Comparing `Psychofit-1.0.0.tar` & `Psychofit-1.0.0.post0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 17:24:23.659120 Psychofit-1.0.0/
--rw-rw-rw-   0        0        0     1108 2023-06-16 17:22:38.000000 Psychofit-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1913 2023-06-16 17:24:23.659120 Psychofit-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 17:24:23.657125 Psychofit-1.0.0/Psychofit.egg-info/
--rw-rw-rw-   0        0        0     1913 2023-06-16 17:24:22.000000 Psychofit-1.0.0/Psychofit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-06-16 17:24:23.000000 Psychofit-1.0.0/Psychofit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 17:24:22.000000 Psychofit-1.0.0/Psychofit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-16 17:24:23.000000 Psychofit-1.0.0/Psychofit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-16 17:24:23.000000 Psychofit-1.0.0/Psychofit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1435 2023-06-16 17:22:38.000000 Psychofit-1.0.0/README.md
--rw-rw-rw-   0        0        0    11465 2023-06-16 17:22:38.000000 Psychofit-1.0.0/psychofit.py
--rw-rw-rw-   0        0        0       42 2023-06-16 17:24:23.660117 Psychofit-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      791 2023-06-16 17:22:38.000000 Psychofit-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 10:09:11.211773 Psychofit-1.0.0.post0/
+-rw-rw-rw-   0        0        0     1108 2023-06-16 17:22:38.000000 Psychofit-1.0.0.post0/LICENSE
+-rw-rw-rw-   0        0        0     1983 2023-06-19 10:09:11.211773 Psychofit-1.0.0.post0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 10:09:11.209777 Psychofit-1.0.0.post0/Psychofit.egg-info/
+-rw-rw-rw-   0        0        0     1983 2023-06-19 10:09:10.000000 Psychofit-1.0.0.post0/Psychofit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-06-19 10:09:11.000000 Psychofit-1.0.0.post0/Psychofit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 10:09:10.000000 Psychofit-1.0.0.post0/Psychofit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-19 10:09:10.000000 Psychofit-1.0.0.post0/Psychofit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-19 10:09:10.000000 Psychofit-1.0.0.post0/Psychofit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1499 2023-06-19 10:07:48.000000 Psychofit-1.0.0.post0/README.md
+-rw-rw-rw-   0        0        0    11465 2023-06-16 17:22:38.000000 Psychofit-1.0.0.post0/psychofit.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 10:09:11.212772 Psychofit-1.0.0.post0/setup.cfg
+-rw-rw-rw-   0        0        0      792 2023-06-19 10:02:46.000000 Psychofit-1.0.0.post0/setup.py
```

### Comparing `Psychofit-1.0.0/LICENSE` & `Psychofit-1.0.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `Psychofit-1.0.0/PKG-INFO` & `Psychofit-1.0.0.post0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 Metadata-Version: 2.1
 Name: Psychofit
-Version: 1.0.0
+Version: 1.0.0.post0
 Summary: A module for fitting 2AFC psychometric data
 Home-page: https://github.com/cortex-lab/psychofit
 Author: Matteo Carandini & Miles Wells
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # psychofit
-[![Coverage Status](https://coveralls.io/repos/github/cortex-lab/psychofit/badge.svg?branch=main)](https://coveralls.io/github/cortex-lab/psychofit?branch=main)
-![CI workflow](https://github.com/cortex-lab/psychofit/actions/workflows/main.yaml/badge.svg?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/cortex-lab/psychofit/badge.svg?branch=master)](https://coveralls.io/github/cortex-lab/psychofit?branch=master)
+[![CI](https://github.com/cortex-lab/psychofit/actions/workflows/main.yaml/badge.svg)](https://github.com/cortex-lab/psychofit/actions/workflows/main.yaml)
 
-A module for fitting 2AFC psychometric data
+A module for fitting 2AFC psychometric data.
 
 The psychofit module contains tools to fit two-alternative psychometric
 data. The fitting is done using maximal likelihood estimation: one
 assumes that the responses of the subject are given by a binomial
 distribution whose mean is given by the psychometric function.
 
 The data can be expressed in fraction correct (from 50 to 100%) or in
 fraction of one specific choice (from 0 to 100%). To fit them you can use
 these functions:
 
- - `weibull50`          - Weibull function from 0.5 to 1, with lapse rate 
- - `weibull`            - Weibull function from 0 to 1, with lapse rate  
- - `erf_psycho`         - erf function from 0 to 1, with lapse rate
- - `erf_psycho_2gammas` - erf function from 0 to 1, with two lapse rates
+ - `weibull50`          - Weibull function from 0.5 to 1, with lapse rate.
+ - `weibull`            - Weibull function from 0 to 1, with lapse rate.
+ - `erf_psycho`         - erf function from 0 to 1, with lapse rate.
+ - `erf_psycho_2gammas` - erf function from 0 to 1, with two lapse rates.
 
 Functions in the toolbox are:
 
- - `mle_fit_psycho`     - Maximumum likelihood fit of psychometric function
- - `neg_likelihood`     - Negative likelihood of a psychometric function
+ - `mle_fit_psycho`     - Maximumum likelihood fit of psychometric function.
+ - `neg_likelihood`     - Negative likelihood of a psychometric function.
 
 For more info, see:
-  Examples           - Examples of use of psychofit toolbox
+
+ - `Examples.ipynb`     - Examples of use of psychofit toolbox.
 
 Matteo Carandini (2000-2017) initial Matlab code<br>
 Miles Wells (2017-2018) ported to Python
```

### Comparing `Psychofit-1.0.0/Psychofit.egg-info/PKG-INFO` & `Psychofit-1.0.0.post0/Psychofit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 Metadata-Version: 2.1
 Name: Psychofit
-Version: 1.0.0
+Version: 1.0.0.post0
 Summary: A module for fitting 2AFC psychometric data
 Home-page: https://github.com/cortex-lab/psychofit
 Author: Matteo Carandini & Miles Wells
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # psychofit
-[![Coverage Status](https://coveralls.io/repos/github/cortex-lab/psychofit/badge.svg?branch=main)](https://coveralls.io/github/cortex-lab/psychofit?branch=main)
-![CI workflow](https://github.com/cortex-lab/psychofit/actions/workflows/main.yaml/badge.svg?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/cortex-lab/psychofit/badge.svg?branch=master)](https://coveralls.io/github/cortex-lab/psychofit?branch=master)
+[![CI](https://github.com/cortex-lab/psychofit/actions/workflows/main.yaml/badge.svg)](https://github.com/cortex-lab/psychofit/actions/workflows/main.yaml)
 
-A module for fitting 2AFC psychometric data
+A module for fitting 2AFC psychometric data.
 
 The psychofit module contains tools to fit two-alternative psychometric
 data. The fitting is done using maximal likelihood estimation: one
 assumes that the responses of the subject are given by a binomial
 distribution whose mean is given by the psychometric function.
 
 The data can be expressed in fraction correct (from 50 to 100%) or in
 fraction of one specific choice (from 0 to 100%). To fit them you can use
 these functions:
 
- - `weibull50`          - Weibull function from 0.5 to 1, with lapse rate 
- - `weibull`            - Weibull function from 0 to 1, with lapse rate  
- - `erf_psycho`         - erf function from 0 to 1, with lapse rate
- - `erf_psycho_2gammas` - erf function from 0 to 1, with two lapse rates
+ - `weibull50`          - Weibull function from 0.5 to 1, with lapse rate.
+ - `weibull`            - Weibull function from 0 to 1, with lapse rate.
+ - `erf_psycho`         - erf function from 0 to 1, with lapse rate.
+ - `erf_psycho_2gammas` - erf function from 0 to 1, with two lapse rates.
 
 Functions in the toolbox are:
 
- - `mle_fit_psycho`     - Maximumum likelihood fit of psychometric function
- - `neg_likelihood`     - Negative likelihood of a psychometric function
+ - `mle_fit_psycho`     - Maximumum likelihood fit of psychometric function.
+ - `neg_likelihood`     - Negative likelihood of a psychometric function.
 
 For more info, see:
-  Examples           - Examples of use of psychofit toolbox
+
+ - `Examples.ipynb`     - Examples of use of psychofit toolbox.
 
 Matteo Carandini (2000-2017) initial Matlab code<br>
 Miles Wells (2017-2018) ported to Python
```

### Comparing `Psychofit-1.0.0/README.md` & `Psychofit-1.0.0.post0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 
 # psychofit
-[![Coverage Status](https://coveralls.io/repos/github/cortex-lab/psychofit/badge.svg?branch=main)](https://coveralls.io/github/cortex-lab/psychofit?branch=main)
-![CI workflow](https://github.com/cortex-lab/psychofit/actions/workflows/main.yaml/badge.svg?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/cortex-lab/psychofit/badge.svg?branch=master)](https://coveralls.io/github/cortex-lab/psychofit?branch=master)
+[![CI](https://github.com/cortex-lab/psychofit/actions/workflows/main.yaml/badge.svg)](https://github.com/cortex-lab/psychofit/actions/workflows/main.yaml)
 
-A module for fitting 2AFC psychometric data
+A module for fitting 2AFC psychometric data.
 
 The psychofit module contains tools to fit two-alternative psychometric
 data. The fitting is done using maximal likelihood estimation: one
 assumes that the responses of the subject are given by a binomial
 distribution whose mean is given by the psychometric function.
 
 The data can be expressed in fraction correct (from 50 to 100%) or in
 fraction of one specific choice (from 0 to 100%). To fit them you can use
 these functions:
 
- - `weibull50`          - Weibull function from 0.5 to 1, with lapse rate 
- - `weibull`            - Weibull function from 0 to 1, with lapse rate  
- - `erf_psycho`         - erf function from 0 to 1, with lapse rate
- - `erf_psycho_2gammas` - erf function from 0 to 1, with two lapse rates
+ - `weibull50`          - Weibull function from 0.5 to 1, with lapse rate.
+ - `weibull`            - Weibull function from 0 to 1, with lapse rate.
+ - `erf_psycho`         - erf function from 0 to 1, with lapse rate.
+ - `erf_psycho_2gammas` - erf function from 0 to 1, with two lapse rates.
 
 Functions in the toolbox are:
 
- - `mle_fit_psycho`     - Maximumum likelihood fit of psychometric function
- - `neg_likelihood`     - Negative likelihood of a psychometric function
+ - `mle_fit_psycho`     - Maximumum likelihood fit of psychometric function.
+ - `neg_likelihood`     - Negative likelihood of a psychometric function.
 
 For more info, see:
-  Examples           - Examples of use of psychofit toolbox
+
+ - `Examples.ipynb`     - Examples of use of psychofit toolbox.
 
 Matteo Carandini (2000-2017) initial Matlab code<br>
 Miles Wells (2017-2018) ported to Python
```

### Comparing `Psychofit-1.0.0/psychofit.py` & `Psychofit-1.0.0.post0/psychofit.py`

 * *Files identical despite different names*

### Comparing `Psychofit-1.0.0/setup.py` & `Psychofit-1.0.0.post0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 CURRENT_DIRECTORY = Path(__file__).parent.absolute()
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='Psychofit',
-    version='1.0.0',
+    version='1.0.0-r0',
     python_requires='>=3.7',
     description='A module for fitting 2AFC psychometric data',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Matteo Carandini & Miles Wells',
     url='https://github.com/cortex-lab/psychofit',
-    classifiers = [
+    classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=['numpy', 'scipy'],
     py_modules=['psychofit']
 )
```

