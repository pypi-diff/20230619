# Comparing `tmp/py-latent-profiles-0.3.tar.gz` & `tmp/py-latent-profiles-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-latent-profiles-0.3.tar", last modified: Thu Apr 20 10:52:46 2023, max compression
+gzip compressed data, was "py-latent-profiles-0.4.tar", last modified: Mon Jun 19 20:43:24 2023, max compression
```

## Comparing `py-latent-profiles-0.3.tar` & `py-latent-profiles-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 htr365     (502) staff       (20)        0 2023-04-20 10:52:46.581092 py-latent-profiles-0.3/
--rw-r--r--   0 htr365     (502) staff       (20)     1061 2023-04-20 10:26:09.000000 py-latent-profiles-0.3/LICENSE.txt
--rw-r--r--   0 htr365     (502) staff       (20)      594 2023-04-20 10:52:46.581239 py-latent-profiles-0.3/PKG-INFO
--rw-r--r--   0 htr365     (502) staff       (20)      234 2023-04-20 09:55:58.000000 py-latent-profiles-0.3/README.md
-drwxr-xr-x   0 htr365     (502) staff       (20)        0 2023-04-20 10:52:46.577670 py-latent-profiles-0.3/py_latent_profiles.egg-info/
--rw-r--r--   0 htr365     (502) staff       (20)      594 2023-04-20 10:52:46.000000 py-latent-profiles-0.3/py_latent_profiles.egg-info/PKG-INFO
--rw-r--r--   0 htr365     (502) staff       (20)      323 2023-04-20 10:52:46.000000 py-latent-profiles-0.3/py_latent_profiles.egg-info/SOURCES.txt
--rw-r--r--   0 htr365     (502) staff       (20)        1 2023-04-20 10:52:46.000000 py-latent-profiles-0.3/py_latent_profiles.egg-info/dependency_links.txt
--rw-r--r--   0 htr365     (502) staff       (20)        1 2023-04-20 10:52:46.000000 py-latent-profiles-0.3/py_latent_profiles.egg-info/not-zip-safe
--rw-r--r--   0 htr365     (502) staff       (20)       17 2023-04-20 10:52:46.000000 py-latent-profiles-0.3/py_latent_profiles.egg-info/requires.txt
--rw-r--r--   0 htr365     (502) staff       (20)        7 2023-04-20 10:52:46.000000 py-latent-profiles-0.3/py_latent_profiles.egg-info/top_level.txt
-drwxr-xr-x   0 htr365     (502) staff       (20)        0 2023-04-20 10:52:46.579790 py-latent-profiles-0.3/py_lpa/
--rw-r--r--   0 htr365     (502) staff       (20)       32 2023-01-02 13:33:55.000000 py-latent-profiles-0.3/py_lpa/__init__.py
--rw-r--r--   0 htr365     (502) staff       (20)    35935 2023-03-31 11:12:39.000000 py-latent-profiles-0.3/py_lpa/gmm.py
--rw-r--r--   0 htr365     (502) staff       (20)       79 2023-04-20 10:52:46.586425 py-latent-profiles-0.3/setup.cfg
--rw-r--r--   0 htr365     (502) staff       (20)      720 2023-04-20 10:52:23.000000 py-latent-profiles-0.3/setup.py
+drwxr-xr-x   0 htr365     (502) staff       (20)        0 2023-06-19 20:43:24.569798 py-latent-profiles-0.4/
+-rw-r--r--   0 htr365     (502) staff       (20)    14875 2023-06-13 07:17:49.000000 py-latent-profiles-0.4/LICENSE.txt
+-rw-r--r--   0 htr365     (502) staff       (20)     1197 2023-06-19 20:43:24.570157 py-latent-profiles-0.4/PKG-INFO
+-rw-r--r--   0 htr365     (502) staff       (20)      837 2023-06-13 07:18:56.000000 py-latent-profiles-0.4/README.md
+drwxr-xr-x   0 htr365     (502) staff       (20)        0 2023-06-19 20:43:24.561016 py-latent-profiles-0.4/py_latent_profiles.egg-info/
+-rw-r--r--   0 htr365     (502) staff       (20)     1197 2023-06-19 20:43:24.000000 py-latent-profiles-0.4/py_latent_profiles.egg-info/PKG-INFO
+-rw-r--r--   0 htr365     (502) staff       (20)      323 2023-06-19 20:43:24.000000 py-latent-profiles-0.4/py_latent_profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 htr365     (502) staff       (20)        1 2023-06-19 20:43:24.000000 py-latent-profiles-0.4/py_latent_profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 htr365     (502) staff       (20)        1 2023-04-20 10:52:46.000000 py-latent-profiles-0.4/py_latent_profiles.egg-info/not-zip-safe
+-rw-r--r--   0 htr365     (502) staff       (20)       17 2023-06-19 20:43:24.000000 py-latent-profiles-0.4/py_latent_profiles.egg-info/requires.txt
+-rw-r--r--   0 htr365     (502) staff       (20)        7 2023-06-19 20:43:24.000000 py-latent-profiles-0.4/py_latent_profiles.egg-info/top_level.txt
+drwxr-xr-x   0 htr365     (502) staff       (20)        0 2023-06-19 20:43:24.568470 py-latent-profiles-0.4/py_lpa/
+-rw-r--r--   0 htr365     (502) staff       (20)       32 2023-01-02 13:33:55.000000 py-latent-profiles-0.4/py_lpa/__init__.py
+-rw-r--r--   0 htr365     (502) staff       (20)    36465 2023-06-19 12:58:30.000000 py-latent-profiles-0.4/py_lpa/gmm.py
+-rw-r--r--   0 htr365     (502) staff       (20)       79 2023-06-19 20:43:24.573025 py-latent-profiles-0.4/setup.cfg
+-rw-r--r--   0 htr365     (502) staff       (20)      720 2023-06-19 20:41:20.000000 py-latent-profiles-0.4/setup.py
```

### Comparing `py-latent-profiles-0.3/py_lpa/gmm.py` & `py-latent-profiles-0.4/py_lpa/gmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import numpy as np
 from scipy import stats
 from tqdm import tqdm
 from datetime import datetime
 import itertools
 from scipy.spatial import distance_matrix
 from scipy.optimize import linear_sum_assignment
-
+import sys
+import warnings
 
 """
 Disclaimer: This code is based on the code for multivariate Gaussian Mixture Models provided here by 
 Xavier Bourret Sicotte:
 https://xavierbourretsicotte.github.io/gaussian_mixture.html
 """
 
@@ -81,38 +82,36 @@
 
         mu 
             an array of starting means for each class and dataset,
             per default these are random draws from the respective dataset
 
         sigma
             an array of starting covariances for each class and dataset
-            per default these are diagonal matrices with 1 on the diagonal
+            per default these are diagonal matrices with the variance of the respective variable on the diagonal
 
         ng
             an array containing the number of observations in each dataset
 
         W
             a list of length G with all zero arrays of dimension ng x K
             this is weighting matrix that is used for facilitating the updating of parameters
         """
+
         # if there are not multiple datasets, unlist the data
         if len(X)==1:
             X=X[0]
-        
         sigma = np.array([[np.eye(D)]*K]*G)
         pi = np.zeros((G,K))
         W = list()
         ng = [x.shape[0] for x in X]
         mu=np.zeros((G,K,D))
 
-
         for g in range(G):
             W.append(np.zeros((ng[g],K)))
             pi[g,:] = np.array([1 / K] * K)
-
         # if means are not constrained (or there is only one dataset) chhose starting value
         # at random from each dataset
         if mean_constraint == None:
             for g in range(G):
                 mu[g,:,:] = X[g][np.random.choice(ng[g],K,replace = False)]
 
         # if means are constrained to be the same across datasets, choose starting value 
@@ -135,15 +134,15 @@
             the data - this could be one dataset or a list consisting of multiple datasets with the same number of variables
 
         mu: array of floats
             an array that contains the current mean values, has to have  dimension(G,K,D) 
             i.e. number of datasets/groups x number of latent classes/Gaussians x number of manifest variables
         
         sigma: array of floats
-            aan array that contains the current covariance values, has to have dimension (G, K, D, D)
+            an array that contains the current covariance values, has to have dimension (G, K, D, D)
             i.e. number of datasets/groups x number of latent classes/Gaussians x number of manifest variables x number of manifest variables
 
         pi: array of floats
             an array that contains the current proportions for the latent lasses/Gaussians, has to have dimension (G,K)
             i.e. number of datasets/groups x number of latent classes/Gaussians
 
 
@@ -160,19 +159,22 @@
         W_s: array or list of arrays
             sum over the the observations of W, helper variable used for later calculations
 
         """
 
         K= self.K
         # probability density function of a multivariate normal distribution
+   
         P = lambda m ,s: stats.multivariate_normal.pdf(x=X, mean = m, cov = s, allow_singular=True)
-
         # calculate the likelihood of each datapoint taken the current mean, cov and proporitons for given
         W = np.zeros((X.shape[0],K))
         for k in range(K):
+            #print(np.sum(np.isnan(mu[k])))
+            #print(np.sum(np.isnan(sigma[k])))
+
             W[:, k] = pi[k] * P(mu[k], sigma[k])
         l = np.sum(np.log(np.sum(W, axis = 1)))
         W = (W.T / W.sum(axis = 1)).T
 
         # sum over the number of observations, helper variable used for later calculations
         W_s = np.nansum(W, axis = 0)
 
@@ -201,14 +203,20 @@
         G = len(X)
         # number of latent ariables
         K = self.K
         
         # no constraint
         if constraint == None:
             mu=np.zeros((G, K,D))
+            #print(W_s)
+            for ws in range(len(W_s)):
+                if any(w==0 for w in W_s[ws]):
+                    #print('success')
+                    W_s[ws][W_s[ws]==0] = 0.001
+                    #print(W_s)
             update_mu = lambda W_s,W,X: (1. / W_s) * np.sum(W.T * X.T, axis = 1).T 
             for g in range(G):
                 mu[g] = list(map(update_mu, W_s[g],W[g].T, itertools.repeat(X[g])))
         
 
         # equality within profile across groups
         elif constraint == 'groups':
@@ -220,16 +228,15 @@
                     denom[g][k] = np.sum(W[g][:,k]* np.sum(W_s[g]))
 
             mu = np.sum(nom, axis=0)/np.sum(denom,axis=0)   
             mu = np.array([mu]*G)
 
         else: 
             raise Exception('No implementation for this combination of constraints')
-
-        
+        #print(mu)
         return(mu)
 
     def mstep_sigma(self, X,W,W_s, mu,var_constraint='classes', cov_constraint='zero'):
         """
         Maximization Step - Update Covariance.
 
         Parameters:
@@ -349,15 +356,15 @@
 
         else: 
             raise Exception('No implementation for this combination of constraints')
 
 
         return pi
 
-    def run_EM(self, X,  rstarts=100, max_iter=100, tol=0.001,  n_solutions=1, init_mu=None, init_cov=None, init_pi=None, mean_constraint=None, var_constraint='groups', cov_constraint='zero', pi_constraint=None):
+    def run_EM(self, X,  rstarts=100, max_iter=100, tol=0.001,  n_solutions=1, init_mu=None, init_cov=None, init_pi=None, mean_constraint=None, var_constraint='groups', cov_constraint='zero', pi_constraint=None, stage=None):
         """
         Function to run the actual Expectation Maximization Algorithm.
 
         Parameters
         -------------
         X: array or list of arrays
             the data - this could be one dataset or a list consisting of multiple datasets with the same number of variables
@@ -400,25 +407,32 @@
         
         """
         try:
             len(np.unique([x.shape[1] for x in X]))==1
         except:
             raise Exception('The samples need to have the same number of manifest variables.')
         
+        warnings.filterwarnings("ignore")
         # number of datasets/groups
         G = len(X)
         # number of manifest variables
         D = X[0].shape[1]
         # number of latent classes/Gaussians
         K = self.K
         # variable to store maximum likelihood values 
         max_l = np.empty(0)
         solutions = []
 
-        for s in tqdm(range(rstarts)):
+        # disable progress bar for second stage optimization
+        if stage =='second':
+            disable = True
+        else:
+            disable = False
+
+        for s in tqdm(range(rstarts),disable=disable):
             # initalisation
             pi,mu,sigma,W, ng = self.initialization([x for x in X], D=D, K=K, G=G)
 
             # override initialisations if starting values are provided
             if init_mu is not None:
                 mu = init_mu
             if init_cov is not None:
@@ -441,23 +455,21 @@
                 if (len(log_likelihoods)>2 and np.abs(l - log_likelihoods[-2]) < tol): break
                 #if (not np.any(W_s)): break     
                 # Maximization Step
                 mu = self.mstep_mu(X,W,W_s, constraint=mean_constraint)
                 sigma = self.mstep_sigma(X,W,W_s,mu,var_constraint=var_constraint, cov_constraint=cov_constraint)
                 pi = self.mstep_pi(X,W,W_s, pi_constraint=pi_constraint)
   
-            #print(log_likelihoods)
             max_l = np.append(max_l, max(log_likelihoods))
             solutions.append([pi,mu,sigma,log_likelihoods, max(log_likelihoods)])
 
         # find the best solution(s)
         best_solutions = np.argpartition(max_l,-n_solutions)[-n_solutions:]
-       
-        solutions = [solutions[i] for i in best_solutions]
-        return(solutions)
+
+        return([solutions[i] for i in best_solutions])
 
 
     def fit(self,*X, rstarts=1, max_iter=100, tol=0.001, first_stage_iter=None, n_final_stage=1, init_mu=None, init_cov=None, init_pi=None, mean_constraint=None, var_constraint=None, cov_constraint=None,pi_constraint=None):
         """
         Function to fit the model.
 
         Parameters
@@ -509,19 +521,19 @@
             [Optional]: A constraint to impose on the proportions of the Gaussians/latent classes
             - None: No restriciton on the proportions
             -'groups': Proportions are restricted to be the same for all groups/datasets
         
         
         Returns
         -----------
+        """
+
+
 
 
-        
-        
-        """
         # initialize time measurement
         t1 = datetime.now()
 
        # the case where we do have a first and second stage
         if first_stage_iter is not None:
            
             if rstarts <= n_final_stage:
@@ -532,26 +544,28 @@
 
             # run first stage
             initial_solutions = self.run_EM(X,rstarts=rstarts, max_iter=first_stage_iter, init_mu=init_mu, init_cov=init_cov, init_pi=init_pi, tol=tol, n_solutions =n_final_stage, mean_constraint=mean_constraint,var_constraint=var_constraint, cov_constraint=cov_constraint,pi_constraint=pi_constraint)
             fpi, fmu, fsigma, flog_likelihoods, fmax_loglikelihood= [[i for i in element if i is not None] for element in  list(itertools.zip_longest(*initial_solutions))]
 
             
             # run second stage
-            final_solutions = list(map(self.run_EM, itertools.repeat(X),itertools.repeat(1),itertools.repeat(max_iter-first_stage_iter),itertools.repeat(tol), itertools.repeat(1),fmu,fsigma,fpi,itertools.repeat(mean_constraint),itertools.repeat(var_constraint), itertools.repeat(cov_constraint), itertools.repeat(pi_constraint)))
+            print('Running Second Stage Optimization')
+            final_solutions = list(map(self.run_EM, itertools.repeat(X),itertools.repeat(1),itertools.repeat(max_iter-first_stage_iter),itertools.repeat(tol), itertools.repeat(1),fmu,fsigma,fpi,itertools.repeat(mean_constraint),itertools.repeat(var_constraint), itertools.repeat(cov_constraint), itertools.repeat(pi_constraint),itertools.repeat('second')))
             final_solutions = [[i for i in element if i is not None] for element in  list(itertools.zip_longest(*final_solutions))]
             [fsolutions] = final_solutions
             pi, mu, sigma, log_likelihoods, max_loglikelihood = [[i for i in element if i is not None] for element in  list(itertools.zip_longest(*fsolutions))]
 
             # find best solution and retain values
             s = np.argmax(np.array(max_loglikelihood))
             pi = pi[s]
             mu = mu[s]
             sigma = sigma[s]
             log_likelihoods = [flog_likelihoods[s][:-1],log_likelihoods[s]]
         else:
+            
             solutions = self.run_EM(X,rstarts=rstarts, max_iter=max_iter, tol=tol, mean_constraint=mean_constraint,var_constraint=var_constraint, cov_constraint=cov_constraint,pi_constraint=pi_constraint)
             pi, mu, sigma, log_likelihoods, max_loglikelihood = [[i for i in element if i is not None] for element in  list(itertools.zip_longest(*solutions))]
             [pi]=pi
             [mu]=mu
             [sigma]=sigma
             [log_likelihoods] = log_likelihoods
 
@@ -570,15 +584,14 @@
         self.pi_ = pi
         self.constraints = [['Constraint on the Mean', mean_constraint], ['Constraint on the Variance', var_constraint],['Constraint on the Covariance',cov_constraint],['Constraint on Pi', pi_constraint]]
         self.run_time = run_time
         self.X = X
         self.rstarts = rstarts
         self.max_iter = max_iter
         self.tol = tol
-           # opt_loglikelihoods = max(log_likelihoods)
 
     def predict_proba(self,*x0):
         """
         Function to predict posterior probabilites for each observation to belong to a specific Gaussian/Latent Class
 
         Parameters
         --------------
@@ -663,23 +676,22 @@
         
         mu = self.means_
         cov = self.covariances_
         pi = self.pi_
 
 
         for g in range(G):
-            for i in range(nbs):
+            for i in tqdm(range(nbs)):
                 # draw a random sample from X with replacement
                 bindex = np.random.choice(X[g].shape[0],X[g].shape[0],replace=True)
                 bsample = np.array(np.take(X[g],bindex,axis=0)).astype(float)
                 bpost = np.take(preds[g],bindex,axis=0)
-                #print(bpost.shape)
-                #print(len(preds))
+        
                 try:
-                    bsrun = self.run_EM([bsample], rstarts=rstarts, max_iter=max_iter, tol =tol, mean_constraint=mean_constraint, var_constraint=var_constraint,cov_constraint=cov_constraint, pi_constraint=pi_constraint,init_pi=bpost)
+                    bsrun = self.run_EM([bsample],  max_iter=max_iter, tol =tol, mean_constraint=mean_constraint, var_constraint=var_constraint,cov_constraint=cov_constraint, pi_constraint=pi_constraint,init_pi=bpost,stage='second')
                 except:
                     i=i-1
                     pass
                 bmu = bsrun[0][1][0]
                 # calculate pairwise distance
                 #print(mu[0])
                 #print(bmu)
@@ -753,21 +765,21 @@
         cov = self.covariances_
         pi = self.pi_
 
         # calculate number of samples to draw from each distribution
         num_samples = np.round(self.pi_ * X[0].shape[0])
 
         for g in range(G):
-            for i in range(nbs):
+            for i in tqdm(range(nbs)):
                 bsample = np.empty((0,int(D)))
                 for k in range(self.K):
                 #bindex = np.random.choice(X[g].shape[0],X[g].shape[0],replace=True)
                     bsample_part = np.random.multivariate_normal(self.means_[g][k],self.covariances_[g][k], size=num_samples[0][k].astype(int))
                     bsample = np.vstack([bsample, bsample_part])
-                bsrun = self.run_EM([bsample], rstarts=rstarts, max_iter=max_iter, tol =tol, mean_constraint=mean_constraint, var_constraint=var_constraint,cov_constraint=cov_constraint, pi_constraint=pi_constraint,init_pi=self.pi_)
+                bsrun = self.run_EM([bsample], rstarts=rstarts, max_iter=max_iter, tol =tol, mean_constraint=mean_constraint, var_constraint=var_constraint,cov_constraint=cov_constraint, pi_constraint=pi_constraint,init_pi=self.pi_,stage='second')
                 
                 bmu = bsrun[0][1][0]
                 # calculate pairwise distance
                 #print(mu[0])
                 #print(bmu)
                 Dist = distance_matrix(mu[0],bmu)
                 org, reorder = linear_sum_assignment(Dist)
```

### Comparing `py-latent-profiles-0.3/setup.py` & `py-latent-profiles-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(name='py-latent-profiles',
-      version='0.3',
+      version='0.4',
       description='A package for running gaussian mixture models and latent profile analyses in Python',
       url='https://github.com/johanna-einsiedler/PyGMM',
       author='Johanna Einsiedler',
       author_email='johanna.einsiedler@sodas.ku.dk',
       license='MIT',
       packages=['py_lpa'],
       install_requires=[
```

