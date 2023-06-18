# Comparing `tmp/hidden-py-1.0.0.tar.gz` & `tmp/hidden-py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hidden-py-1.0.0.tar", last modified: Sun Jun 18 01:33:18 2023, max compression
+gzip compressed data, was "hidden-py-1.0.1.tar", last modified: Sun Jun 18 22:49:40 2023, max compression
```

## Comparing `hidden-py-1.0.0.tar` & `hidden-py-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:33:18.701549 hidden-py-1.0.0/
--rw-r--r--   0 stevelarge   (501) staff       (20)     1068 2022-03-05 13:45:02.000000 hidden-py-1.0.0/LICENSE.txt
--rw-r--r--   0 stevelarge   (501) staff       (20)     6141 2023-06-18 01:33:18.701330 hidden-py-1.0.0/PKG-INFO
--rw-r--r--   0 stevelarge   (501) staff       (20)     5521 2023-06-17 15:00:50.000000 hidden-py-1.0.0/README.md
-drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:33:18.697097 hidden-py-1.0.0/hidden_py/
--rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.0/hidden_py/__init__.py
--rw-r--r--   0 stevelarge   (501) staff       (20)     5515 2023-06-18 01:27:25.000000 hidden-py-1.0.0/hidden_py/dynamics.py
-drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:33:18.698438 hidden-py-1.0.0/hidden_py/filters/
--rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.0/hidden_py/filters/__init__.py
--rw-r--r--   0 stevelarge   (501) staff       (20)     9279 2023-06-18 01:27:25.000000 hidden-py-1.0.0/hidden_py/filters/bayesian.py
--rw-r--r--   0 stevelarge   (501) staff       (20)    11471 2023-06-18 01:27:25.000000 hidden-py-1.0.0/hidden_py/infer.py
-drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:33:18.700341 hidden-py-1.0.0/hidden_py/optimize/
--rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.0/hidden_py/optimize/__init__.py
--rw-r--r--   0 stevelarge   (501) staff       (20)    11349 2023-06-18 01:27:25.000000 hidden-py-1.0.0/hidden_py/optimize/base.py
--rw-r--r--   0 stevelarge   (501) staff       (20)      170 2023-06-18 01:27:25.000000 hidden-py-1.0.0/hidden_py/optimize/config.py
--rw-r--r--   0 stevelarge   (501) staff       (20)    19441 2023-06-18 01:27:25.000000 hidden-py-1.0.0/hidden_py/optimize/optimization.py
--rw-r--r--   0 stevelarge   (501) staff       (20)      281 2023-06-18 01:27:25.000000 hidden-py-1.0.0/hidden_py/optimize/registry.py
--rw-r--r--   0 stevelarge   (501) staff       (20)     2318 2023-06-18 01:27:25.000000 hidden-py-1.0.0/hidden_py/optimize/results.py
--rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.0/hidden_py/optimize/types.py
-drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:33:18.698148 hidden-py-1.0.0/hidden_py.egg-info/
--rw-r--r--   0 stevelarge   (501) staff       (20)     6141 2023-06-18 01:33:18.000000 hidden-py-1.0.0/hidden_py.egg-info/PKG-INFO
--rw-r--r--   0 stevelarge   (501) staff       (20)      623 2023-06-18 01:33:18.000000 hidden-py-1.0.0/hidden_py.egg-info/SOURCES.txt
--rw-r--r--   0 stevelarge   (501) staff       (20)        1 2023-06-18 01:33:18.000000 hidden-py-1.0.0/hidden_py.egg-info/dependency_links.txt
--rw-r--r--   0 stevelarge   (501) staff       (20)       52 2023-06-18 01:33:18.000000 hidden-py-1.0.0/hidden_py.egg-info/requires.txt
--rw-r--r--   0 stevelarge   (501) staff       (20)       10 2023-06-18 01:33:18.000000 hidden-py-1.0.0/hidden_py.egg-info/top_level.txt
--rw-r--r--   0 stevelarge   (501) staff       (20)       38 2023-06-18 01:33:18.701611 hidden-py-1.0.0/setup.cfg
--rw-r--r--   0 stevelarge   (501) staff       (20)     1230 2023-06-18 01:32:46.000000 hidden-py-1.0.0/setup.py
-drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:33:18.701039 hidden-py-1.0.0/tests/
--rw-r--r--   0 stevelarge   (501) staff       (20)     3644 2023-06-18 01:27:25.000000 hidden-py-1.0.0/tests/test_dynamics.py
--rw-r--r--   0 stevelarge   (501) staff       (20)    10667 2023-06-18 01:27:25.000000 hidden-py-1.0.0/tests/test_filters.py
--rw-r--r--   0 stevelarge   (501) staff       (20)     5702 2023-06-18 01:27:25.000000 hidden-py-1.0.0/tests/test_inferrence.py
--rw-r--r--   0 stevelarge   (501) staff       (20)     7563 2023-06-18 01:27:25.000000 hidden-py-1.0.0/tests/test_optimizers.py
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-06-18 22:49:40.845954 hidden-py-1.0.1/
+-rw-r--r--   0 stevelarge   (501) staff       (20)     1068 2022-03-05 13:45:02.000000 hidden-py-1.0.1/LICENSE.txt
+-rw-r--r--   0 stevelarge   (501) staff       (20)     9348 2023-06-18 22:49:40.845727 hidden-py-1.0.1/PKG-INFO
+-rw-r--r--   0 stevelarge   (501) staff       (20)     8728 2023-06-18 22:41:49.000000 hidden-py-1.0.1/README.md
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-06-18 22:49:40.842017 hidden-py-1.0.1/hidden_py/
+-rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.1/hidden_py/__init__.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)     5515 2023-06-18 01:27:25.000000 hidden-py-1.0.1/hidden_py/dynamics.py
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-06-18 22:49:40.843185 hidden-py-1.0.1/hidden_py/filters/
+-rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.1/hidden_py/filters/__init__.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)     9279 2023-06-18 01:27:25.000000 hidden-py-1.0.1/hidden_py/filters/bayesian.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)    11471 2023-06-18 01:27:25.000000 hidden-py-1.0.1/hidden_py/infer.py
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-06-18 22:49:40.844683 hidden-py-1.0.1/hidden_py/optimize/
+-rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.1/hidden_py/optimize/__init__.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)    11349 2023-06-18 01:27:25.000000 hidden-py-1.0.1/hidden_py/optimize/base.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)      170 2023-06-18 01:27:25.000000 hidden-py-1.0.1/hidden_py/optimize/config.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)    19441 2023-06-18 01:27:25.000000 hidden-py-1.0.1/hidden_py/optimize/optimization.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)      281 2023-06-18 01:27:25.000000 hidden-py-1.0.1/hidden_py/optimize/registry.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)     2318 2023-06-18 01:27:25.000000 hidden-py-1.0.1/hidden_py/optimize/results.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.1/hidden_py/optimize/types.py
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-06-18 22:49:40.842917 hidden-py-1.0.1/hidden_py.egg-info/
+-rw-r--r--   0 stevelarge   (501) staff       (20)     9348 2023-06-18 22:49:40.000000 hidden-py-1.0.1/hidden_py.egg-info/PKG-INFO
+-rw-r--r--   0 stevelarge   (501) staff       (20)      623 2023-06-18 22:49:40.000000 hidden-py-1.0.1/hidden_py.egg-info/SOURCES.txt
+-rw-r--r--   0 stevelarge   (501) staff       (20)        1 2023-06-18 22:49:40.000000 hidden-py-1.0.1/hidden_py.egg-info/dependency_links.txt
+-rw-r--r--   0 stevelarge   (501) staff       (20)       52 2023-06-18 22:49:40.000000 hidden-py-1.0.1/hidden_py.egg-info/requires.txt
+-rw-r--r--   0 stevelarge   (501) staff       (20)       10 2023-06-18 22:49:40.000000 hidden-py-1.0.1/hidden_py.egg-info/top_level.txt
+-rw-r--r--   0 stevelarge   (501) staff       (20)       38 2023-06-18 22:49:40.846007 hidden-py-1.0.1/setup.cfg
+-rw-r--r--   0 stevelarge   (501) staff       (20)     1230 2023-06-18 22:42:28.000000 hidden-py-1.0.1/setup.py
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-06-18 22:49:40.845448 hidden-py-1.0.1/tests/
+-rw-r--r--   0 stevelarge   (501) staff       (20)     3644 2023-06-18 01:27:25.000000 hidden-py-1.0.1/tests/test_dynamics.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)    10667 2023-06-18 01:27:25.000000 hidden-py-1.0.1/tests/test_filters.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)     5702 2023-06-18 01:27:25.000000 hidden-py-1.0.1/tests/test_inferrence.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)     7563 2023-06-18 01:27:25.000000 hidden-py-1.0.1/tests/test_optimizers.py
```

### Comparing `hidden-py-1.0.0/LICENSE.txt` & `hidden-py-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.0/README.md` & `hidden-py-1.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,57 @@
-# **Hidden**
-
-#### A Hidden Markov Model package for python
-
----
+# **A Hidden Markov Model package for python**
 
 ### Installation
 
 To install this package simply run the command:
 
-`pip install hidden`
+`pip install hidden-py`
 
 <br />
 
+## Table of Contents
+
+- [Overview](#overview)
+  - [Dynamics/Simulation](#dynamicssimulation)
+  - [System Identification](#system-identification)
+  - [Signal Processing](#signal-processing)
+- [Roadmap](#roadmap)
+
 ---
 
 ## Overview
 
 This package contains logic for inferring, simulating, and fitting Hidden Markov Models with discrete states and obserfvations. In contrast to more common HMM packages that deal primarily with _mixture models_, output symbols are continuous, and drawn from a distriubtion of values that is somehow conditional on the hidden state.
 
 Here, we have thusfar considered primarily scenarios where the observation value is an integer, and one of the possible hidden states. There are three major use-cases for this codebase: dynamics/simulation, system identification/parameter fitting, and signal processing. In all cases, these functionalities are outlined in several tutorial notebooks in the `notebooks/tutorials` location of the [github repository](https://github.com/StevenJLarge/hmm)
 
 <br />
 
+## Hidden Markov Models
+
+Markov Models are a class of stochastic models for characterizing the behaviour of systems that transition between states randomly, with a probability that depends only on the curent state of the system (_i.e._ they are memoryless). Because if this simplification, the dynamics on a set of discrete states can be captured entirely by a single matrix, known as the _transition matrix_, $A$, with elements $A_{ij} = p(x_t=i | x_{t-1} = j)$ quantifying the probability that during timestep $t-1 \to t$, the system will transition from state $j\to i$.
+
+Because of the normalization of probability, the columns of $A$ are constrained to be qual to unity.
+
+A hidden Markov model (HMM), on the other hand, is a probabilistic function of a Markov model. This means that the output of an HMM is an observation $y$, that is correlated with the underlying (hidden/unobserved) state of the Markov model, but only probabilitsically so. For a set of discrete possible observations (as we capture in this package), the observation process can also be modelled by a matrix (the _observation matrix_) $B$ with elemetnts $B_{ij} = p(y_t = i | x_{t} = j)$ quantifying the probability that our measurement/observation $y_t$ at time $t$ is equal to $i$ given the hidden system is in state $j$. Here, the diagonal elements represent our probability of observing the _correct_ state, while off-diagonals represent the probability of error.
+
+The goal of simulation is simply to generate trajectories of both the hidden state and observation time-series that is conistent with these probabilities.
+
+The goal for system identification/parameter fitting is to fit the most likely parameters (elements of the $A$ and $B$) matrices, given only a time series of observations.
+
+Finally, the goal if signal processing is to make use of the observation sequence to infer what the hidden state is at a particular point in time.
+
 ### Dynamics/Simulation
 
 The `hidden.dynamics` submodule contains the code necessary to simulate the hidden state and observation dynamics as specified by a state transition matrix $A$ (with elements that quantify the rate of transitions between states) and an observation matrix $B$, with elements that quantify the probability of observing a given output symbol, given the current hidden state.
 
 For instance, the code necessary to initialize a hidden Markov model, run the dyanamics, and extract the observation and state time-series
 
 ```
-from hidden import dynamics
+from hidden_py import dynamics
 
 # 2 hidden states, 2 possible observation values
 hmm = dynamics.HMM(2, 2)
 
 # Helper routine to initialize A and B matrices
 hmm.init_uniform_cycle()
 
@@ -52,15 +70,15 @@
 ### System Identification
 
 The `infer` submodule contains the code that wraps lower-level functionality (primarily in the `filters/bayesian.py` and `optimize/optimization.py` files) for both signal processing and system identification/parameter fitting.
 
 There are two separate means of performing system identification: Local/Global partial likelihood optimization, and complete-data likelihood optimization. While more comprehensive details are contained in the github notebooks, broadly speaking partial data likelihood optimization performs relatively standard optimizations on the likelihood function $\mathcal{L}(\theta | Y)$ which considers only the observations as the _data_. Effectively, these optimizers wrap the `scipy.opt.minimize` functions by encoding and decoding the $A$ and $B$ matrices into a parameter vector (ensuring that their column-normalization is preserved) and calculating the negative log-likelihood of a particular parameter vector. In practice, given a set of observations, we can initialize an `analyzer` and run either local (using, by default, the `scipy.opt.minimize` function with the `L-BFGS-B` algorithm) or global (using the `scipy` SHGO algorithm) as:
 
 ```
-from hidden import infer
+from hidden_py import infer
 
 # Input the dimensions of the HMM and observations
 analyzer = infer.MarkovInfer(2, 2)
 
 # Initial estimates of the A and B matrices
 A_est = np.array([
     [0.8, 0.1],
@@ -79,16 +97,16 @@
 opt_global = analyzer.optimize(observations, A_est, B_est, symmetric=False, opt_type=OptClass.Global)
 
 ```
 
 Now, for the complete-data likeihood optimization, the interface is very similar, but behind the scenes the code will implement an implementation of the Baum-Welch reparameterization algorithm (an instance of an Expectation-Maximization algorithm) to find the optimal parameter values. In practice, this can be done as:
 
 ```
-from hidden import infer
-from hidden.optimize.base import OptClass
+from hidden_py import infer
+from hidden_py.optimize.base import OptClass
 
 analyzer = infer.MarkovInfer(2, 2)
 
 res_bw = analyzer.optimize(observations, A_est, B_est, opt_type=OptClass.ExpMax)
 
 ```
 
@@ -107,12 +125,27 @@
 
 <br />
 
 ---
 
 ### Signal Processing
 
+The `infer` submodule can also be used for the purposes of signal processing: given a valid estimate of the model parameters, how can we best estimate the hidden state value, given the observations. There are two distinct domains of application, first would be prediction in real time, where only observations in the past are available for inferring the current hidden state (this would use the so-called forward-filtered estiamte). There is also an _ex post_ approach, which uses the entirety of observations from a given period of time to estimate the hidden state at a particular point within that time period. This is the so-called Bayesian smoothec estiamte of the hidden state.
+
+Quantitatively the forward filter and Bayesian smoothed estimates of a given HMM sequence of observations can be calculated in the following way:
+
+```
+from hidden_py import infer
+
+analyzer = infer.MarkovInfer(2, 2)
+
+# Gets the forward algorithm results
+analyzer.forward_algo(observations, A, B)
+
+# Gets the Bayesian-smoothed estimate of the hidden state
+analyzer.bayesian_smooth(observations, A, B)
+
+```
+
 <br />
 
 ---
-
-## Roadmap
```

### Comparing `hidden-py-1.0.0/hidden_py/dynamics.py` & `hidden-py-1.0.1/hidden_py/dynamics.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.0/hidden_py/filters/bayesian.py` & `hidden-py-1.0.1/hidden_py/filters/bayesian.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.0/hidden_py/infer.py` & `hidden-py-1.0.1/hidden_py/infer.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.0/hidden_py/optimize/base.py` & `hidden-py-1.0.1/hidden_py/optimize/base.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.0/hidden_py/optimize/optimization.py` & `hidden-py-1.0.1/hidden_py/optimize/optimization.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.0/hidden_py/optimize/results.py` & `hidden-py-1.0.1/hidden_py/optimize/results.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.0/hidden_py.egg-info/SOURCES.txt` & `hidden-py-1.0.1/hidden_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.0/setup.py` & `hidden-py-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # README contents
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='hidden-py',
     packages=find_packages(),
-    version="1.0.0",
+    version="1.0.1",
     long_description=long_description,
     long_description_content_type='text/markdown',
     desription='''
         Implementation of methods used for analysis of hidden markov
         models, both on the system identification (parameter fitting)
         and inferrence (filtering)
     ''',
```

### Comparing `hidden-py-1.0.0/tests/test_dynamics.py` & `hidden-py-1.0.1/tests/test_dynamics.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.0/tests/test_filters.py` & `hidden-py-1.0.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.0/tests/test_inferrence.py` & `hidden-py-1.0.1/tests/test_inferrence.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.0/tests/test_optimizers.py` & `hidden-py-1.0.1/tests/test_optimizers.py`

 * *Files identical despite different names*

