# Comparing `tmp/hsmm_mvpy-0.1.0b1.tar.gz` & `tmp/hsmm_mvpy-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsmm_mvpy-0.1.0b1.tar", last modified: Wed Jun  7 12:10:05 2023, max compression
+gzip compressed data, was "hsmm_mvpy-0.1.0b3.tar", last modified: Mon Jun 19 15:42:44 2023, max compression
```

## Comparing `hsmm_mvpy-0.1.0b1.tar` & `hsmm_mvpy-0.1.0b3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-07 12:10:05.863505 hsmm_mvpy-0.1.0b1/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b1/LICENSE.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    23839 2023-06-07 12:10:05.863505 hsmm_mvpy-0.1.0b1/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    21473 2023-06-06 12:45:29.000000 hsmm_mvpy-0.1.0b1/README.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      845 2023-06-07 12:09:30.000000 hsmm_mvpy-0.1.0b1/pyproject.toml
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-06-07 12:10:05.863505 hsmm_mvpy-0.1.0b1/setup.cfg
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-07 12:10:05.863505 hsmm_mvpy-0.1.0b1/src/
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-07 12:10:05.863505 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      171 2022-09-28 08:31:43.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/__init__.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    56703 2023-06-07 12:06:48.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/models.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    10494 2023-05-30 15:57:35.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/simulations.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    40133 2023-06-06 09:51:30.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/utils.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    21011 2023-06-06 10:51:18.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/visu.py
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-07 12:10:05.863505 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy.egg-info/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    23839 2023-06-07 12:10:05.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy.egg-info/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      343 2023-06-07 12:10:05.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy.egg-info/SOURCES.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-06-07 12:10:05.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy.egg-info/dependency_links.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       83 2023-06-07 12:10:05.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy.egg-info/requires.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-06-07 12:10:05.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy.egg-info/top_level.txt
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:42:44.580909 hsmm_mvpy-0.1.0b3/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b3/LICENSE.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 15:42:44.580909 hsmm_mvpy-0.1.0b3/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22740 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b3/README.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      830 2023-06-19 15:42:17.000000 hsmm_mvpy-0.1.0b3/pyproject.toml
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-06-19 15:42:44.580909 hsmm_mvpy-0.1.0b3/setup.cfg
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:42:44.580909 hsmm_mvpy-0.1.0b3/src/
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:42:44.580909 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      194 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/__init__.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    57323 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/models.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     5735 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/resample.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    11044 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/simulations.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    41499 2023-06-19 15:42:15.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/utils.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22654 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/visu.py
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:42:44.580909 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy.egg-info/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 15:42:44.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy.egg-info/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      369 2023-06-19 15:42:44.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-06-19 15:42:44.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       71 2023-06-19 15:42:44.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy.egg-info/requires.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-06-19 15:42:44.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy.egg-info/top_level.txt
```

### Comparing `hsmm_mvpy-0.1.0b1/LICENSE.md` & `hsmm_mvpy-0.1.0b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b1/PKG-INFO` & `hsmm_mvpy-0.1.0b3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm_mvpy
-Version: 0.1.0b1
+Version: 0.1.0b3
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
         
@@ -42,34 +42,34 @@
 License-File: LICENSE.md
 
 HsMM MVpy
 ==========
 
 ![](plots/general_illustration.png)
 
-HsMM MVpy is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HMP) of neural time-series (e.g. EEG) based on the method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)), Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf)) and Weindel, van Maanen & Borst (in preparation).
+HsMM MVpy is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HMP) of neural time-series (e.g. EEG) based on the HsMM-MVPA method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030); see Borst & Anderson, [2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf), for an accessible introduction). HMP is described in Weindel, van Maanen & Borst (in preparation).
 
-As a summary of the method, an HMP model parses the reaction time into a number of successive stages determined based on patterns in a neural time-serie. Hence any reaction time can then be described by a number of stage  and their duration estimated using hsmm_mvpy. The important aspect of HMP is that it is a whole-brain analysis (or whole scalp analysis) that estimates the onset of stages on a single-trial basis. This by-trial estimations allows you then to further dig into any aspect you are interested in a signal:
+As a summary of the method, an HMP model parses the reaction time into a number of successive stages determined based on patterns in a neural time-serie. Hence any reaction time can then be described by a number of stages and their duration estimated using HMP. The important aspect of HMP is that it is a whole-brain analysis (or whole scalp analysis) that estimates the onset of stages on a single-trial basis. These by-trial estimates allow you then to further dig into any aspect you are interested in a signal:
 - Describing an experiment or a clinical sample in terms of stages detected in the EEG signal
 - Describing experimental effects based on a particular stage duration
 - Estimating the effect of trial-wise manipuations on the identified stages (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
 - Time-lock EEG signal to the onset of a given stage and perform classical ERPs or time-frequency analysis based on the onset of a new stage
 - And many more (e.g. evidence accumulation models on decision stage, classification based on the number of transition events in the signal,...)
 
 
 # Documentation
-**Important note** The current tutorials are based on the latest (unstable) version not yet default in _pip_, installing through github is therefore recommended or specify the beta version when installing through _pip_: ```pip install hsmm-mvpy==0.1.0b0```
+**Important note** The current tutorials are based on the latest (unstable) version not yet default in _pip_, installing through github is therefore recommended or specify the beta version when installing through _pip_: ```pip install hsmm-mvpy==0.1.0b1```
 
 The package is available through *pip*. 
 A recommended way of using the package is to use a conda environment (see [anaconda](https://www.anaconda.com/products/distribution>) for how to install conda):
 
     $ conda create -n hmp 
     $ conda activate hmp
     $ conda install pip #if not already installed
-    $ pip install hsmm-mvpy==0.1.0b0
+    $ pip install hsmm-mvpy==0.1.0b1
 
 Then import hsmm-mvpy in your favorite python IDE through:
 
 ```python
     import hsmm_mvpy as hmp
 ```
 
@@ -84,71 +84,81 @@
     $ pip install -e .
 
 
 ## To get started
 To get started with the code:
 - Check the demo below 
 - Inspect the tutorials in the tutorials repository
-    - Load EEG data (tutorial 1)
-    - Estimating a HMP with given number of stages (tutorial 2)
-    - Test for the number of stages that best explains the data (tutorial 3)
-    - Testing differences across conditions (tutorial 4)
-
-To further learn about the method be sure to check the paper by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) as well as the book chapter by Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf)). The following list also contains a non-exhaustive list of papers published using HMP:
+    - Tutorial 1: Loading EEG data 
+    - Tutorial 2: Estimating a HMP with given number of stages
+    - Tutorial 3: Test for the number of stages that best explains the data
+    - Tutorial 4: Testing differences across conditions
+
+To further learn about the oriignal HsMM-MVPA method be sure to check the paper by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) as well as the book chapter by Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf)). The following list contains a non-exhaustive list of papers published using the original HsMM-MVPA method:
+- Anderson, J.R., Borst, J.P., Fincham, J.M., Ghuman, A.S., Tenison, C., & Zhang, Q. (2018). The Common Time Course of Memory Processes Revealed. Psychological Science 29(9), pp. 1463-1474. [link](https://doi.org/10.1177/0956797618774526)
+- Berberyan, H.S., Van Rijn, H., & Borst, J.P. (2021). Discovering the brain stages of lexical decision: Behavioral effects originate from a single neural decision process. Brain and Cognition 153: 105786. [link](https://www.sciencedirect.com/science/article/pii/S0278262621001068)
 - Berberyan, H. S., van Maanen, L., van Rijn, H., & Borst, J. (2021). EEG-based identification of evidence accumulation stages in decision-making. Journal of Cognitive Neuroscience, 33(3), 510-527. [link](https://doi.org/10.1162/jocn_a_01663)
 - Van Maanen, L., Portoles, O., & Borst, J. P. (2021). The discovery and interpretation of evidence accumulation stages. Computational brain & behavior, 4(4), 395-415. [link](https://link.springer.com/article/10.1007/s42113-021-00105-2)
 - Portoles, O., Blesa, M., van Vugt, M., Cao, M., & Borst, J. P. (2022). Thalamic bursts modulate cortical synchrony locally to switch between states of global functional connectivity in a cognitive task. PLoS computational biology, 18(3), e1009407. [link](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009407)
+- Portoles, O., Borst, J.P., & Van Vugt, M.K. (2018). Characterizing synchrony patterns across cognitive task stages of associative recognition memory. European Journal of Neuroscience 48, pp. 2759-2769. [link](http://onlinelibrary.wiley.com/doi/10.1111/ejn.13817/epdf)
+- Zhang, Q., van Vugt, M.K., Borst, J.P., & Anderson, J.R. (2018). Mapping Working Memory Retrieval in Space and in Time: A Combined Electroencephalography and Electrocorticography Approach. NeuroImage 174, pp. 472-484. [link](https://www.sciencedirect.com/science/article/pii/S1053811918302490)
+
+
 
 ## Demo on simulated data
 
 The following section will quickly walk you through an example usage in simulated data (using [MNE](https://mne.tools/dev/auto_examples/simulation/index.html)'s simulation functions and tutorials)
 
 First we load the libraries necessary for the demo on simulated data
 
 ### Importing libraries
 
+
+
 ```python
 ## Importing these packages is specific for this simulation case
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 from scipy.stats import gamma
 
 ## Importing HMP
 import hsmm_mvpy as hmp
 from hsmm_mvpy import simulations
 ```
 
+
 ### Simulating data
 
-In the following code block we simulate 50 trials from four known sources, this is not code you would need for your own analysis except if you want to simulate and test properties of HMP models. All these four sources are defined by a localization, an activation amplitude and a distribution (here a gamma with shape and scale parameters) for the onsets of the stages on each trial. The simulation functions are based on this [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
+In the following code block we simulate 50 trials from four known sources, this is not code you would need for your own analysis except if you'd want to simulate and test properties of HMP models. All four sources are defined by a location, an activation amplitude and a distribution in time (here a gamma with shape and scale parameters) for the onsets of the stages on each trial. The simulation functions are based on this [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
 
 _If you're running this for the first time a 1.65 G file will be downloaded in order to perform the simulation but this will be done only once (alternatively you can just download the corresponding simulation file and place it in the same folder from where you are running this notebook)_
 
 
 
 ```python
 cpus = 5 # For multiprocessing, usually a good idea to use multiple CPUs as long as you have enough RAM
 
 n_trials = 50 #Number of trials to simulate
 
 ##### Here we define the sources of the brain activity (event) for each trial
+# Because the last source determines the response, we will get four events during the trials, and therefore five stages
+n_sources = 5
 frequency = 10.#Frequency of the event defining its duration, half-sine of 10Hz = 50ms
-amplitude = .5e-6 #Amplitude of the event in Volt, defining signal to noise ratio
+amplitude = .5e-6 #Amplitude of the event in nAm, defining signal to noise ratio
 shape = 2 #shape of the gamma distribution
 means = np.array([60, 150, 200, 100, 80])/shape #Mean duration of the stages in ms
-names = ['bankssts-rh','posteriorcingulate-lh','parahippocampal-lh',\
-         'pericalcarine-rh','postcentral-lh']#Which source to activate at each stage (see atlas when calling simulations.available_sources())
+names = simulations.available_sources()[:n_sources]#Which source to activate at each stage (see atlas when calling simulations.available_sources())
 
 sources = []
 for source in zip(names, means):#One source = one frequency, one amplitude and a given by-trial variability distribution
     sources.append([source[0], frequency, amplitude, gamma(shape, scale=source[1])])
 
 # Function used to generate the data
-file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', location=25, overwrite=True)
+file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', location=25, overwrite=True) #location indicates the middle of the event after the stage start time in ms
 #Recovering sampling frequency of the simulated dataset
 sfreq = simulations.simulation_sfreq()
 #load electrode position, specific to the simulations
 positions = simulations.simulation_positions()
 ```
 
     Simulating ./dataset_README_raw.fif
@@ -172,27 +182,20 @@
 events = generating_events[(generating_events[:,2] == 1) | (generating_events[:,2] == resp_trigger)]#only retain stimulus and response triggers
 
 #Visualising the raw simulated EEG data
 import mne
 raw = mne.io.read_raw_fif(file[0], preload=False, verbose=False)
 raw.pick_types(eeg=True).plot(scalings=dict(eeg=1e-5), events=events, block=True);
 ```
-
-    Using qt as 2D backend.
-    Channels marked as bad:
-    none
-    
 ![png](README_files/README_7_1.png)
 
 
-
 ### Recovering number of stages as well as actual by-trial variation
 
-To compare the by-trial duration of bumps that we will estimate later on we first recover the actual number of stages or sources used in the simulation as well as the actual by-trial variation in the onset of the bumps. Again with a typical dataset you wouldn't need that part as you ignore the ground truth.
-
+To see how well HMP does at recovering by-trial stages below, here we get the ground truth from our simulation. Unfortunately, with an actual dataset you don’t have access to this, of course. 
 
 ```python
 %matplotlib inline
 number_of_sources = len(np.unique(generating_events[:,2])[1:])#one trigger = one source
 #Recover the actual time of the simulated events
 random_source_times = np.reshape(np.ediff1d(generating_events[:,0],to_begin=0)[generating_events[:,2] > 1], \
            (n_trials, number_of_sources))
@@ -207,37 +210,39 @@
 # Reading the data
 eeg_data = hmp.utils.read_mne_data(file[0], event_id=event_id, resp_id=resp_id, sfreq=sfreq, 
             events_provided=events, verbose=False)
 
 ```
 
     Processing participant ./dataset_README_raw.fif's continuous eeg
-    Reading 0 ... 153075  =      0.000 ...   254.864 secs...
+    Reading 0 ... 143915  =      0.000 ...   239.613 secs...
     50 trials were retained for participant ./dataset_README_raw.fif
 
 
-The package uses [xarray](https://docs.xarray.dev/en/stable/) named dimension matrices, allowing to directly manipulate the data using the name of the dimensions:
+HMP uses [xarray](https://docs.xarray.dev/en/stable/) named dimension matrices, allowing to directly manipulate the data using the name of the dimensions:
 
 
 ```python
 #example of usage of xarray
 print(eeg_data)
 eeg_data.sel(electrodes=['EEG 001','EEG 002','EEG 003'], samples=range(400))\
     .data.groupby('samples').mean(['participant','epochs']).plot.line(hue='electrodes');
 ```
 
     <xarray.Dataset>
-    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 711)
+    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 783)
     Coordinates:
       * epochs       (epochs) int64 0 1 2 3 4 5 6 7 8 ... 41 42 43 44 45 46 47 48 49
       * electrodes   (electrodes) <U7 'EEG 001' 'EEG 002' ... 'EEG 059' 'EEG 060'
-      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 704 705 706 707 708 709 710
+      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 776 777 778 779 780 781 782
       * participant  (participant) <U2 'S0'
     Data variables:
-        data         (participant, epochs, electrodes, samples) float64 1.96e-06 ...
+        data         (participant, epochs, electrodes, samples) float64 -3.747e-0...
+        event_name   (participant, epochs) object 'stimulus' ... 'stimulus'
+        rt           (participant, epochs) float64 0.5444 0.641 ... 0.8991 1.304
     Attributes:
         sfreq:    600.614990234375
         offset:   0
 
 
 
     
@@ -251,38 +256,37 @@
 Note that if the number of components to retain is not specified, the scree plot of the PCA is displayed and a prompt ask how many PCs should be retained (in this case we specify it as building the README does not allow for prompts)
 
 
 ```python
 hmp_data = hmp.utils.transform_data(eeg_data, apply_standard=False, n_comp=4)
 ```
 
-Once the data is in the expected format, we can initialize an HMP
+# HMP model
 
+Once the data is in the expected format, we can initialize an HMP object; note that no estimation is performed yet.
 
 ```python
 init = hmp.models.hmp(hmp_data, eeg_data, event_width=50, cpus=cpus)#Initialization of the model
 ```
 
-# HMP model
-
 We are looking for stages in the data (**Hidden Markov**) and assume that transitions between stages are signaled by a template in the data (**pattern analysis**). By default we use the same template as Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet'.apa.org/doi/10.1037/rev0000030)), a 10 Hz half-sine, resulting in a 50ms duration bump-like shape:
 
 
 
 ```python
 plt.plot(init.template,'x');
 ```
 
 
     
 ![png](README_files/README_18_0.png)
     
 
 
-This pattern is assumed to be present in multiple electrodes (**multivariate**). In order to find it, we apply a cross-correlation between that shape and the (normalized) EEG data:
+This pattern is assumed to be present across several electrodes (**multivariate**). In order to find it, we apply a cross-correlation between that shape and the (normalized) EEG data:
 
 
 
 ```python
 epoch = 0 #illustrating the first trial
 hmp_data.unstack().sel(component=[0,1,2], epochs=epoch).squeeze().plot.line(hue='component');
 plt.vlines(random_source_times[epoch,:-1].cumsum()-1, -3, 3, 'k')#overlaying the simulated stage transition times
@@ -291,69 +295,69 @@
 
     
 ![png](README_files/README_20_1.png)
     
 
 
 
-The by-trial onset of this transition event is assumed to be captured by a probability distribution (**semi-Markov**), e.g. in this application a gamma with a shape of 2:
+The by-trial onset of this transition pattern event is assumed to be captured by a probability distribution (**semi-Markov**), e.g. in this application a gamma with a shape of 2:
 
 
 ```python
 T = 350
 plt.plot(np.linspace(0,T,1001),gamma.pdf(np.linspace(0,T,1001), 2, scale=50)) 
 plt.xlabel('t');
 ```
 
 
     
 ![png](README_files/README_22_0.png)
     
 
 
-And this is then the full explanation of an HMP model: Looking for a transition event across several electrodes and trials that signals a transition to the next stage and which onset is expected to follow a probability distribution (in this case a gamma).
+And this is then the full explanation of an HMP model: Looking for a transition event across several electrodes and trials that signals a transition to the next stage and which onset is expected to follow a probability distribution (by default a gamma distribution).
 
 # Estimating an HMP model
 
-We can directly fit an HMP model without giving any info on the number of stages (see tutorial 2 for the explanation of the following cell)
+We can directly fit an HMP model without giving any info on the number of stages (see tutorial 2 for a detailed explanation of the following cell)
 
 
 
 ```python
 estimates = init.fit(step=20, verbose=True)
 ```
 
 
+
+    Transition event 1 found around sample 37
     Transition event 2 found around sample 137
-    Transition event 3 found around sample 258
-    Transition event 4 found around sample 330
+    Transition event 3 found around sample 277
+    Transition event 4 found around sample 348
     Estimating 4 events model
     Parameters estimated for 4 events model
 
 
 ### Visualizing results of the fit
 
-In the previous cell we initiated an HMP model looking for 50ms bumps in the EEG signal and parsing the EEG data into a signal with 4 Transition events and 5 gamma distributed stages with a fixed shape of 2 and a scale estimated by stage. We can now inspect the results of the fit.
+In the previous cell we initiated an HMP model looking for default 50ms bumps – the transition events – in the EEG signal. The method discovered four events, and therefore five gamma-distributed stages with a fixed shape of 2 and an estimated scale. We can now inspect the results of the fit.
 
 We can directly take a look to the topologies and latencies of the events by calling ```hmp.visu.plot_topo_timecourse```
 
 
-We can directly take a look to the topologies and latencies of the events by calling ```hmp.visu.plot_topo_timecourse```
-
 
 ```python
 hmp.visu.plot_topo_timecourse(eeg_data, estimates, #Data and estimations 
                                positions, init,#position of the electrodes and initialized model
                                magnify=1, sensors=False, time_step=1000/init.sfreq,#Display control parameters
                                times_to_display = np.mean(init.ends - init.starts))#plot reaction times
 ```
 
 
     
-![png](README_files/README_27_0.png)
+![png](README_files/README_26_0.png)
     
 
 
 This shows us the electrode activity on the scalp as well as the average time of occurence of the events based on the stage distributions.
 
 As we are estimating the event onsets on a by-trial basis we can look at the by-trial variation in stage duration.
 
@@ -362,15 +366,15 @@
 event_times_estimates = init.compute_times(init, estimates, mean=False, add_rt=True).dropna('event')#computing predicted event times
 ax = hmp.visu.plot_latencies_average(event_times_estimates, init.event_width_samples, 1, errs='ci', times_to_display = np.mean(init.ends - init.starts))
 ax.set_ylabel('your label here');
 ```
 
 
     
-![png](README_files/README_29_0.png)
+![png](README_files/README_28_0.png)
     
 
 
 For the same reason we can also inspect the probability distribution of event onsets:
 
 
 
@@ -384,21 +388,21 @@
 
     <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
-![png](README_files/README_31_1.png)
+![png](README_files/README_30_1.png)
     
 
 
 
     
-![png](README_files/README_31_2.png)
+![png](README_files/README_30_2.png)
     
 
 
 As HMP estimated stage onset per trial we can also look at the predicted stage onsets for a given trial.
 
 
 ```python
@@ -411,23 +415,23 @@
 
     <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
-![png](README_files/README_33_1.png)
+![png](README_files/README_32_1.png)
     
 
 
 This then shows the likeliest stage onset location in time for the first trial!
 
 ## Comparing with ground truth
 
-As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HMP-MVpy. As in the beginning, this code is specific to the case where you simulate data.
+As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HMP. Perhaps to state the obvious, this code is specific to the case where you simulate data.
 
 
 ```python
 colors = sns.color_palette(None, number_of_sources)
 plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.prod(axis=1), color=colors,s=50)
 plt.plot([np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],
          [np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],'--');
@@ -436,34 +440,34 @@
 plt.ylabel('Estimated stage duration')
 plt.show()
 
 ```
 
 
     
-![png](README_files/README_35_0.png)
+![png](README_files/README_34_0.png)
     
 
 
-Or also overlay actual bumps onset with predicted one
+We can also overlay actual bumps onset with predicted one
 
 
 
 ```python
 hmp.visu.plot_topo_timecourse(eeg_data, estimates, positions, init, magnify=1, sensors=False, figsize=(13,1), title='Actual vs estimated event onsets',
         times_to_display = np.mean(np.cumsum(random_source_times,axis=1),axis=0))
 ```
 
 
     
-![png](README_files/README_37_0.png)
+![png](README_files/README_36_0.png)
     
 
 
-We see that the HSMM-MVpy package recovers the exact average location of the bumps defined in the simulated data.
+We see that the HMP recovered the exact average location of the bumps defined in the simulated data.
 
 We can further test how well the package did by comparing the generated single trial onsets with those estimated from the HMP model
 
 
 ```python
 fig, ax= plt.subplots(number_of_sources,1, figsize=(5,3.5*number_of_sources), dpi=300)
 ax[0].set_title('Comparing true vs estimated single trial stage durations')
@@ -475,15 +479,15 @@
     ax[i].set_ylabel(f'Estimated by-trial stage duration for stage {i+1}')
     ax[i].set_xlabel(f'Simulated by-trial stage duration for stage {i+1}')
     i+= 1
 ```
 
 
     
-![png](README_files/README_39_0.png)
+![png](README_files/README_38_0.png)
     
 
 
 We see that every stage gets nicely recovered even on a by-trial basis!
 
 # Beyond summary statistics for EEG analysis
 
@@ -510,19 +514,19 @@
 plt.xlim(0,500)
 plt.ylim(-3e-6,3e-6);
 
 ```
 
 
     
-![png](README_files/README_41_0.png)
+![png](README_files/README_40_0.png)
     
 
 
-Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is very close to traditional ERPs with very clear signal in the beginning of a trial (as events are more in phase) and summed and blurried in later stages of the reaction times (as event are off phase).
+Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is similar to traditional ERPs that have a very clear signal in the beginning of a trial (as events are more in phase) and summed and blurred further away from the stimulus (as events are off phase).
 
 Now things can get better if we first parse, by-trial, the signal into the different stages based on the HMP estimates:
 
 
 ```python
 BRP_times = init.compute_times(init, estimates.dropna('event'), fill_value=0, add_rt=True)
 
@@ -539,20 +543,20 @@
     df = pd.DataFrame(BRP).melt(var_name='Time')
     sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkblue') 
     plt.xlim(0,100)
 ```
 
 
     
-![png](README_files/README_43_0.png)
+![png](README_files/README_42_0.png)
     
 
 
 
-In this case we clearly see at each stage the half-sin (of 50ms hence ~ 30 samples for the sampling frequency used) we simulated in the first step and the preceding period of silence (hence the first stage doesn't contain such a half-sin). Note that the end of the stages tend to be noisier because less trial are defining the average signal (also why the confidence interval grows).
+In this case we clearly see at each stage the half-sine (of 50ms hence ~ 30 samples for the sampling frequency used) we simulated in the first step and the preceding period of silence (hence the first stage doesn't contain such a half-sine). Note that the end of the stages tend to be noisier because fewer trials are defining the average signal.
 
 
 ### Follow-up
 
 For examples on how to use the package when the number of transition events/stages is unkown, or to compare stage durations across conditions see the tutorial notebooks:
 - Load EEG data (tutorial 1)
 - Estimating a given number of events (tutorial 2)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hsmm_mvpy-0.1.0b1/README.md` & `hsmm_mvpy-0.1.0b3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 HsMM MVpy
 ==========
 
 ![](plots/general_illustration.png)
 
-HsMM MVpy is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HMP) of neural time-series (e.g. EEG) based on the method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)), Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf)) and Weindel, van Maanen & Borst (in preparation).
+HsMM MVpy is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HMP) of neural time-series (e.g. EEG) based on the HsMM-MVPA method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030); see Borst & Anderson, [2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf), for an accessible introduction). HMP is described in Weindel, van Maanen & Borst (in preparation).
 
-As a summary of the method, an HMP model parses the reaction time into a number of successive stages determined based on patterns in a neural time-serie. Hence any reaction time can then be described by a number of stage  and their duration estimated using hsmm_mvpy. The important aspect of HMP is that it is a whole-brain analysis (or whole scalp analysis) that estimates the onset of stages on a single-trial basis. This by-trial estimations allows you then to further dig into any aspect you are interested in a signal:
+As a summary of the method, an HMP model parses the reaction time into a number of successive stages determined based on patterns in a neural time-serie. Hence any reaction time can then be described by a number of stages and their duration estimated using HMP. The important aspect of HMP is that it is a whole-brain analysis (or whole scalp analysis) that estimates the onset of stages on a single-trial basis. These by-trial estimates allow you then to further dig into any aspect you are interested in a signal:
 - Describing an experiment or a clinical sample in terms of stages detected in the EEG signal
 - Describing experimental effects based on a particular stage duration
 - Estimating the effect of trial-wise manipuations on the identified stages (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
 - Time-lock EEG signal to the onset of a given stage and perform classical ERPs or time-frequency analysis based on the onset of a new stage
 - And many more (e.g. evidence accumulation models on decision stage, classification based on the number of transition events in the signal,...)
 
 
 # Documentation
-**Important note** The current tutorials are based on the latest (unstable) version not yet default in _pip_, installing through github is therefore recommended or specify the beta version when installing through _pip_: ```pip install hsmm-mvpy==0.1.0b0```
+**Important note** The current tutorials are based on the latest (unstable) version not yet default in _pip_, installing through github is therefore recommended or specify the beta version when installing through _pip_: ```pip install hsmm-mvpy==0.1.0b1```
 
 The package is available through *pip*. 
 A recommended way of using the package is to use a conda environment (see [anaconda](https://www.anaconda.com/products/distribution>) for how to install conda):
 
     $ conda create -n hmp 
     $ conda activate hmp
     $ conda install pip #if not already installed
-    $ pip install hsmm-mvpy==0.1.0b0
+    $ pip install hsmm-mvpy==0.1.0b1
 
 Then import hsmm-mvpy in your favorite python IDE through:
 
 ```python
     import hsmm_mvpy as hmp
 ```
 
@@ -41,71 +41,81 @@
     $ pip install -e .
 
 
 ## To get started
 To get started with the code:
 - Check the demo below 
 - Inspect the tutorials in the tutorials repository
-    - Load EEG data (tutorial 1)
-    - Estimating a HMP with given number of stages (tutorial 2)
-    - Test for the number of stages that best explains the data (tutorial 3)
-    - Testing differences across conditions (tutorial 4)
-
-To further learn about the method be sure to check the paper by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) as well as the book chapter by Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf)). The following list also contains a non-exhaustive list of papers published using HMP:
+    - Tutorial 1: Loading EEG data 
+    - Tutorial 2: Estimating a HMP with given number of stages
+    - Tutorial 3: Test for the number of stages that best explains the data
+    - Tutorial 4: Testing differences across conditions
+
+To further learn about the oriignal HsMM-MVPA method be sure to check the paper by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) as well as the book chapter by Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf)). The following list contains a non-exhaustive list of papers published using the original HsMM-MVPA method:
+- Anderson, J.R., Borst, J.P., Fincham, J.M., Ghuman, A.S., Tenison, C., & Zhang, Q. (2018). The Common Time Course of Memory Processes Revealed. Psychological Science 29(9), pp. 1463-1474. [link](https://doi.org/10.1177/0956797618774526)
+- Berberyan, H.S., Van Rijn, H., & Borst, J.P. (2021). Discovering the brain stages of lexical decision: Behavioral effects originate from a single neural decision process. Brain and Cognition 153: 105786. [link](https://www.sciencedirect.com/science/article/pii/S0278262621001068)
 - Berberyan, H. S., van Maanen, L., van Rijn, H., & Borst, J. (2021). EEG-based identification of evidence accumulation stages in decision-making. Journal of Cognitive Neuroscience, 33(3), 510-527. [link](https://doi.org/10.1162/jocn_a_01663)
 - Van Maanen, L., Portoles, O., & Borst, J. P. (2021). The discovery and interpretation of evidence accumulation stages. Computational brain & behavior, 4(4), 395-415. [link](https://link.springer.com/article/10.1007/s42113-021-00105-2)
 - Portoles, O., Blesa, M., van Vugt, M., Cao, M., & Borst, J. P. (2022). Thalamic bursts modulate cortical synchrony locally to switch between states of global functional connectivity in a cognitive task. PLoS computational biology, 18(3), e1009407. [link](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009407)
+- Portoles, O., Borst, J.P., & Van Vugt, M.K. (2018). Characterizing synchrony patterns across cognitive task stages of associative recognition memory. European Journal of Neuroscience 48, pp. 2759-2769. [link](http://onlinelibrary.wiley.com/doi/10.1111/ejn.13817/epdf)
+- Zhang, Q., van Vugt, M.K., Borst, J.P., & Anderson, J.R. (2018). Mapping Working Memory Retrieval in Space and in Time: A Combined Electroencephalography and Electrocorticography Approach. NeuroImage 174, pp. 472-484. [link](https://www.sciencedirect.com/science/article/pii/S1053811918302490)
+
+
 
 ## Demo on simulated data
 
 The following section will quickly walk you through an example usage in simulated data (using [MNE](https://mne.tools/dev/auto_examples/simulation/index.html)'s simulation functions and tutorials)
 
 First we load the libraries necessary for the demo on simulated data
 
 ### Importing libraries
 
+
+
 ```python
 ## Importing these packages is specific for this simulation case
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 from scipy.stats import gamma
 
 ## Importing HMP
 import hsmm_mvpy as hmp
 from hsmm_mvpy import simulations
 ```
 
+
 ### Simulating data
 
-In the following code block we simulate 50 trials from four known sources, this is not code you would need for your own analysis except if you want to simulate and test properties of HMP models. All these four sources are defined by a localization, an activation amplitude and a distribution (here a gamma with shape and scale parameters) for the onsets of the stages on each trial. The simulation functions are based on this [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
+In the following code block we simulate 50 trials from four known sources, this is not code you would need for your own analysis except if you'd want to simulate and test properties of HMP models. All four sources are defined by a location, an activation amplitude and a distribution in time (here a gamma with shape and scale parameters) for the onsets of the stages on each trial. The simulation functions are based on this [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
 
 _If you're running this for the first time a 1.65 G file will be downloaded in order to perform the simulation but this will be done only once (alternatively you can just download the corresponding simulation file and place it in the same folder from where you are running this notebook)_
 
 
 
 ```python
 cpus = 5 # For multiprocessing, usually a good idea to use multiple CPUs as long as you have enough RAM
 
 n_trials = 50 #Number of trials to simulate
 
 ##### Here we define the sources of the brain activity (event) for each trial
+# Because the last source determines the response, we will get four events during the trials, and therefore five stages
+n_sources = 5
 frequency = 10.#Frequency of the event defining its duration, half-sine of 10Hz = 50ms
-amplitude = .5e-6 #Amplitude of the event in Volt, defining signal to noise ratio
+amplitude = .5e-6 #Amplitude of the event in nAm, defining signal to noise ratio
 shape = 2 #shape of the gamma distribution
 means = np.array([60, 150, 200, 100, 80])/shape #Mean duration of the stages in ms
-names = ['bankssts-rh','posteriorcingulate-lh','parahippocampal-lh',\
-         'pericalcarine-rh','postcentral-lh']#Which source to activate at each stage (see atlas when calling simulations.available_sources())
+names = simulations.available_sources()[:n_sources]#Which source to activate at each stage (see atlas when calling simulations.available_sources())
 
 sources = []
 for source in zip(names, means):#One source = one frequency, one amplitude and a given by-trial variability distribution
     sources.append([source[0], frequency, amplitude, gamma(shape, scale=source[1])])
 
 # Function used to generate the data
-file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', location=25, overwrite=True)
+file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', location=25, overwrite=True) #location indicates the middle of the event after the stage start time in ms
 #Recovering sampling frequency of the simulated dataset
 sfreq = simulations.simulation_sfreq()
 #load electrode position, specific to the simulations
 positions = simulations.simulation_positions()
 ```
 
     Simulating ./dataset_README_raw.fif
@@ -129,27 +139,20 @@
 events = generating_events[(generating_events[:,2] == 1) | (generating_events[:,2] == resp_trigger)]#only retain stimulus and response triggers
 
 #Visualising the raw simulated EEG data
 import mne
 raw = mne.io.read_raw_fif(file[0], preload=False, verbose=False)
 raw.pick_types(eeg=True).plot(scalings=dict(eeg=1e-5), events=events, block=True);
 ```
-
-    Using qt as 2D backend.
-    Channels marked as bad:
-    none
-    
 ![png](README_files/README_7_1.png)
 
 
-
 ### Recovering number of stages as well as actual by-trial variation
 
-To compare the by-trial duration of bumps that we will estimate later on we first recover the actual number of stages or sources used in the simulation as well as the actual by-trial variation in the onset of the bumps. Again with a typical dataset you wouldn't need that part as you ignore the ground truth.
-
+To see how well HMP does at recovering by-trial stages below, here we get the ground truth from our simulation. Unfortunately, with an actual dataset you don’t have access to this, of course. 
 
 ```python
 %matplotlib inline
 number_of_sources = len(np.unique(generating_events[:,2])[1:])#one trigger = one source
 #Recover the actual time of the simulated events
 random_source_times = np.reshape(np.ediff1d(generating_events[:,0],to_begin=0)[generating_events[:,2] > 1], \
            (n_trials, number_of_sources))
@@ -164,37 +167,39 @@
 # Reading the data
 eeg_data = hmp.utils.read_mne_data(file[0], event_id=event_id, resp_id=resp_id, sfreq=sfreq, 
             events_provided=events, verbose=False)
 
 ```
 
     Processing participant ./dataset_README_raw.fif's continuous eeg
-    Reading 0 ... 153075  =      0.000 ...   254.864 secs...
+    Reading 0 ... 143915  =      0.000 ...   239.613 secs...
     50 trials were retained for participant ./dataset_README_raw.fif
 
 
-The package uses [xarray](https://docs.xarray.dev/en/stable/) named dimension matrices, allowing to directly manipulate the data using the name of the dimensions:
+HMP uses [xarray](https://docs.xarray.dev/en/stable/) named dimension matrices, allowing to directly manipulate the data using the name of the dimensions:
 
 
 ```python
 #example of usage of xarray
 print(eeg_data)
 eeg_data.sel(electrodes=['EEG 001','EEG 002','EEG 003'], samples=range(400))\
     .data.groupby('samples').mean(['participant','epochs']).plot.line(hue='electrodes');
 ```
 
     <xarray.Dataset>
-    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 711)
+    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 783)
     Coordinates:
       * epochs       (epochs) int64 0 1 2 3 4 5 6 7 8 ... 41 42 43 44 45 46 47 48 49
       * electrodes   (electrodes) <U7 'EEG 001' 'EEG 002' ... 'EEG 059' 'EEG 060'
-      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 704 705 706 707 708 709 710
+      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 776 777 778 779 780 781 782
       * participant  (participant) <U2 'S0'
     Data variables:
-        data         (participant, epochs, electrodes, samples) float64 1.96e-06 ...
+        data         (participant, epochs, electrodes, samples) float64 -3.747e-0...
+        event_name   (participant, epochs) object 'stimulus' ... 'stimulus'
+        rt           (participant, epochs) float64 0.5444 0.641 ... 0.8991 1.304
     Attributes:
         sfreq:    600.614990234375
         offset:   0
 
 
 
     
@@ -208,38 +213,37 @@
 Note that if the number of components to retain is not specified, the scree plot of the PCA is displayed and a prompt ask how many PCs should be retained (in this case we specify it as building the README does not allow for prompts)
 
 
 ```python
 hmp_data = hmp.utils.transform_data(eeg_data, apply_standard=False, n_comp=4)
 ```
 
-Once the data is in the expected format, we can initialize an HMP
+# HMP model
 
+Once the data is in the expected format, we can initialize an HMP object; note that no estimation is performed yet.
 
 ```python
 init = hmp.models.hmp(hmp_data, eeg_data, event_width=50, cpus=cpus)#Initialization of the model
 ```
 
-# HMP model
-
 We are looking for stages in the data (**Hidden Markov**) and assume that transitions between stages are signaled by a template in the data (**pattern analysis**). By default we use the same template as Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet'.apa.org/doi/10.1037/rev0000030)), a 10 Hz half-sine, resulting in a 50ms duration bump-like shape:
 
 
 
 ```python
 plt.plot(init.template,'x');
 ```
 
 
     
 ![png](README_files/README_18_0.png)
     
 
 
-This pattern is assumed to be present in multiple electrodes (**multivariate**). In order to find it, we apply a cross-correlation between that shape and the (normalized) EEG data:
+This pattern is assumed to be present across several electrodes (**multivariate**). In order to find it, we apply a cross-correlation between that shape and the (normalized) EEG data:
 
 
 
 ```python
 epoch = 0 #illustrating the first trial
 hmp_data.unstack().sel(component=[0,1,2], epochs=epoch).squeeze().plot.line(hue='component');
 plt.vlines(random_source_times[epoch,:-1].cumsum()-1, -3, 3, 'k')#overlaying the simulated stage transition times
@@ -248,69 +252,69 @@
 
     
 ![png](README_files/README_20_1.png)
     
 
 
 
-The by-trial onset of this transition event is assumed to be captured by a probability distribution (**semi-Markov**), e.g. in this application a gamma with a shape of 2:
+The by-trial onset of this transition pattern event is assumed to be captured by a probability distribution (**semi-Markov**), e.g. in this application a gamma with a shape of 2:
 
 
 ```python
 T = 350
 plt.plot(np.linspace(0,T,1001),gamma.pdf(np.linspace(0,T,1001), 2, scale=50)) 
 plt.xlabel('t');
 ```
 
 
     
 ![png](README_files/README_22_0.png)
     
 
 
-And this is then the full explanation of an HMP model: Looking for a transition event across several electrodes and trials that signals a transition to the next stage and which onset is expected to follow a probability distribution (in this case a gamma).
+And this is then the full explanation of an HMP model: Looking for a transition event across several electrodes and trials that signals a transition to the next stage and which onset is expected to follow a probability distribution (by default a gamma distribution).
 
 # Estimating an HMP model
 
-We can directly fit an HMP model without giving any info on the number of stages (see tutorial 2 for the explanation of the following cell)
+We can directly fit an HMP model without giving any info on the number of stages (see tutorial 2 for a detailed explanation of the following cell)
 
 
 
 ```python
 estimates = init.fit(step=20, verbose=True)
 ```
 
 
+
+    Transition event 1 found around sample 37
     Transition event 2 found around sample 137
-    Transition event 3 found around sample 258
-    Transition event 4 found around sample 330
+    Transition event 3 found around sample 277
+    Transition event 4 found around sample 348
     Estimating 4 events model
     Parameters estimated for 4 events model
 
 
 ### Visualizing results of the fit
 
-In the previous cell we initiated an HMP model looking for 50ms bumps in the EEG signal and parsing the EEG data into a signal with 4 Transition events and 5 gamma distributed stages with a fixed shape of 2 and a scale estimated by stage. We can now inspect the results of the fit.
+In the previous cell we initiated an HMP model looking for default 50ms bumps – the transition events – in the EEG signal. The method discovered four events, and therefore five gamma-distributed stages with a fixed shape of 2 and an estimated scale. We can now inspect the results of the fit.
 
 We can directly take a look to the topologies and latencies of the events by calling ```hmp.visu.plot_topo_timecourse```
 
 
-We can directly take a look to the topologies and latencies of the events by calling ```hmp.visu.plot_topo_timecourse```
-
 
 ```python
 hmp.visu.plot_topo_timecourse(eeg_data, estimates, #Data and estimations 
                                positions, init,#position of the electrodes and initialized model
                                magnify=1, sensors=False, time_step=1000/init.sfreq,#Display control parameters
                                times_to_display = np.mean(init.ends - init.starts))#plot reaction times
 ```
 
 
     
-![png](README_files/README_27_0.png)
+![png](README_files/README_26_0.png)
     
 
 
 This shows us the electrode activity on the scalp as well as the average time of occurence of the events based on the stage distributions.
 
 As we are estimating the event onsets on a by-trial basis we can look at the by-trial variation in stage duration.
 
@@ -319,15 +323,15 @@
 event_times_estimates = init.compute_times(init, estimates, mean=False, add_rt=True).dropna('event')#computing predicted event times
 ax = hmp.visu.plot_latencies_average(event_times_estimates, init.event_width_samples, 1, errs='ci', times_to_display = np.mean(init.ends - init.starts))
 ax.set_ylabel('your label here');
 ```
 
 
     
-![png](README_files/README_29_0.png)
+![png](README_files/README_28_0.png)
     
 
 
 For the same reason we can also inspect the probability distribution of event onsets:
 
 
 
@@ -341,21 +345,21 @@
 
     <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
-![png](README_files/README_31_1.png)
+![png](README_files/README_30_1.png)
     
 
 
 
     
-![png](README_files/README_31_2.png)
+![png](README_files/README_30_2.png)
     
 
 
 As HMP estimated stage onset per trial we can also look at the predicted stage onsets for a given trial.
 
 
 ```python
@@ -368,23 +372,23 @@
 
     <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
-![png](README_files/README_33_1.png)
+![png](README_files/README_32_1.png)
     
 
 
 This then shows the likeliest stage onset location in time for the first trial!
 
 ## Comparing with ground truth
 
-As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HMP-MVpy. As in the beginning, this code is specific to the case where you simulate data.
+As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HMP. Perhaps to state the obvious, this code is specific to the case where you simulate data.
 
 
 ```python
 colors = sns.color_palette(None, number_of_sources)
 plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.prod(axis=1), color=colors,s=50)
 plt.plot([np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],
          [np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],'--');
@@ -393,34 +397,34 @@
 plt.ylabel('Estimated stage duration')
 plt.show()
 
 ```
 
 
     
-![png](README_files/README_35_0.png)
+![png](README_files/README_34_0.png)
     
 
 
-Or also overlay actual bumps onset with predicted one
+We can also overlay actual bumps onset with predicted one
 
 
 
 ```python
 hmp.visu.plot_topo_timecourse(eeg_data, estimates, positions, init, magnify=1, sensors=False, figsize=(13,1), title='Actual vs estimated event onsets',
         times_to_display = np.mean(np.cumsum(random_source_times,axis=1),axis=0))
 ```
 
 
     
-![png](README_files/README_37_0.png)
+![png](README_files/README_36_0.png)
     
 
 
-We see that the HSMM-MVpy package recovers the exact average location of the bumps defined in the simulated data.
+We see that the HMP recovered the exact average location of the bumps defined in the simulated data.
 
 We can further test how well the package did by comparing the generated single trial onsets with those estimated from the HMP model
 
 
 ```python
 fig, ax= plt.subplots(number_of_sources,1, figsize=(5,3.5*number_of_sources), dpi=300)
 ax[0].set_title('Comparing true vs estimated single trial stage durations')
@@ -432,15 +436,15 @@
     ax[i].set_ylabel(f'Estimated by-trial stage duration for stage {i+1}')
     ax[i].set_xlabel(f'Simulated by-trial stage duration for stage {i+1}')
     i+= 1
 ```
 
 
     
-![png](README_files/README_39_0.png)
+![png](README_files/README_38_0.png)
     
 
 
 We see that every stage gets nicely recovered even on a by-trial basis!
 
 # Beyond summary statistics for EEG analysis
 
@@ -467,19 +471,19 @@
 plt.xlim(0,500)
 plt.ylim(-3e-6,3e-6);
 
 ```
 
 
     
-![png](README_files/README_41_0.png)
+![png](README_files/README_40_0.png)
     
 
 
-Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is very close to traditional ERPs with very clear signal in the beginning of a trial (as events are more in phase) and summed and blurried in later stages of the reaction times (as event are off phase).
+Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is similar to traditional ERPs that have a very clear signal in the beginning of a trial (as events are more in phase) and summed and blurred further away from the stimulus (as events are off phase).
 
 Now things can get better if we first parse, by-trial, the signal into the different stages based on the HMP estimates:
 
 
 ```python
 BRP_times = init.compute_times(init, estimates.dropna('event'), fill_value=0, add_rt=True)
 
@@ -496,20 +500,20 @@
     df = pd.DataFrame(BRP).melt(var_name='Time')
     sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkblue') 
     plt.xlim(0,100)
 ```
 
 
     
-![png](README_files/README_43_0.png)
+![png](README_files/README_42_0.png)
     
 
 
 
-In this case we clearly see at each stage the half-sin (of 50ms hence ~ 30 samples for the sampling frequency used) we simulated in the first step and the preceding period of silence (hence the first stage doesn't contain such a half-sin). Note that the end of the stages tend to be noisier because less trial are defining the average signal (also why the confidence interval grows).
+In this case we clearly see at each stage the half-sine (of 50ms hence ~ 30 samples for the sampling frequency used) we simulated in the first step and the preceding period of silence (hence the first stage doesn't contain such a half-sine). Note that the end of the stages tend to be noisier because fewer trials are defining the average signal.
 
 
 ### Follow-up
 
 For examples on how to use the package when the number of transition events/stages is unkown, or to compare stage durations across conditions see the tutorial notebooks:
 - Load EEG data (tutorial 1)
 - Estimating a given number of events (tutorial 2)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hsmm_mvpy-0.1.0b1/pyproject.toml` & `hsmm_mvpy-0.1.0b3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "hsmm_mvpy"
-version = "0.1.0-beta1"
+version = "0.1.0-beta3"
 authors = [
   { name="Gabriel Weindel", email="gabriel.weindel@gmail.com" },
   { name="Leendert van Maanen", email="e@mail.com" },
   { name="Jelmer Borst", email="e@mail.com" },
 ]
 description = "Package for fitting Hidden Semi-Markov Models to electro-encephalographic data"
 readme = "README.md"
@@ -22,13 +22,12 @@
 dependencies=["mne >=1.0.0",
 "numpy",
 "xarray",
 "scikit-learn",
 "statsmodels",
 "seaborn",
 "scipy",
-"netcdf4",
-"xskillscore"]
+"netcdf4"]
 
 [project.urls]
 "Homepage" = "https://github.com/GWeindel/hmp"
 "Bug Tracker" = "https://github.com/GWeindel/hmp/issues"
```

### Comparing `hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/models.py` & `hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,19 +230,20 @@
         if multiple_n_events is not None and len(pars) != multiple_n_events+1:#align all dimensions
             pars = np.concatenate((pars, np.tile(np.nan, (multiple_n_events+1-len(pars),2))))
             mags = np.concatenate((mags, np.tile(np.nan, 
                 (multiple_n_events-len(mags), np.shape(mags)[1]))),axis=0)
             eventprobs = np.concatenate((eventprobs, np.tile(np.nan, (np.shape(eventprobs)[0],\
                     np.shape(eventprobs)[1], multiple_n_events-np.shape(eventprobs)[2]))),axis=2)
             n_events = multiple_n_events
-            # print(np.shape(eventprobs))
         
         xrlikelihoods = xr.DataArray(lkh , name="likelihoods")
-        xrparams = xr.DataArray(pars, dims=("stage",'parameter'), name="parameters")
-        xrmags = xr.DataArray(mags, dims=("event","component"), name="magnitudes")
+        xrparams = xr.DataArray(pars, dims=("stage",'parameter'), name="parameters", 
+                        coords = [range(len(pars)), ['shape','scale']])
+        xrmags = xr.DataArray(mags, dims=("event","component"), name="magnitudes",
+                    coords = [range(len(mags)), range(np.shape(mags)[1])])
         part, trial = self.coords['participant'].values, self.coords['trials'].values
         if n_events>0:
             n_samples, n_participant_x_trials,_ = np.shape(eventprobs)
         else:
             n_samples, n_participant_x_trials = np.shape(eventprobs)
         if n_participant_x_trials >1 and n_events >0:
             xreventprobs = xr.Dataset({'eventprobs': (('event', 'trial_x_participant','samples'), 
@@ -666,26 +667,29 @@
             if not cumulative:
                 times = times.diff(dim='stage')
         if mean:
             times = times.mean('trial_x_participant')
         return times
    
     @staticmethod
-    def compute_topologies(electrodes, estimated, event_width_samples, extra_dim=False):
-        shifted_times = estimated.eventprobs.shift(samples=event_width_samples//2+1, fill_value=0).copy()#Shifts to compute electrode topology at the peak of the event
+    def compute_topologies(channels, estimated, event_width_samples, extra_dim=False, mean=True):
+        shifted_times = estimated.eventprobs.shift(samples=event_width_samples//2+1, fill_value=0).copy()#Shifts to compute channel topology at the peak of the event
         if extra_dim:
-            return xr.dot(electrodes.rename({'epochs':'trials'}).\
-                      stack(trial_x_participant=['participant','trials']).data.fillna(0), \
-                      shifted_times.fillna(0), dims=['samples']).mean('trial_x_participant').\
-                      transpose(extra_dim,'event','electrodes')
-        else:
-            return xr.dot(electrodes.rename({'epochs':'trials'}).\
-                      stack(trial_x_participant=['participant','trials']).data.fillna(0), \
-                      shifted_times.fillna(0), dims=['samples']).mean('trial_x_participant').\
-                      transpose('event','electrodes')
+            data =  xr.dot(channels.rename({'epochs':'trials'}).\
+                      stack(trial_x_participant=['participant','trials']).data.fillna(0).drop_duplicates('trial_x_participant'), \
+                      shifted_times.fillna(0), dims=['samples']).\
+                      transpose(extra_dim,'trial_x_participant','event','channels')
+        else:
+            data = xr.dot(channels.rename({'epochs':'trials'}).\
+                      stack(trial_x_participant=['participant','trials']).data.fillna(0).drop_duplicates('trial_x_participant'), \
+                      shifted_times.fillna(0), dims=['samples']).\
+                      transpose('trial_x_participant','event','channels')
+        if mean:
+            data = data.mean('trial_x_participant')
+        return data
     
     def gen_random_stages(self, n_events, mean_d):
         '''
         Returns random stage duration between 0 and mean RT by iteratively drawind sample from a 
         uniform distribution between the last stage duration (equal to 0 for first iteration) and 1.
         Last stage is equal to 1-previous stage duration.
         The stages are then scaled to the mean RT
@@ -880,61 +884,65 @@
                 estimates.append(self.EM(1, mags, pars, threshold, magnitudes_to_fix, parameters_to_fix))
         lkhs_sp = np.array([x[0] for x in estimates])
         mags_sp = np.array([x[1] for x in estimates])
         pars_sp = np.array([x[2] for x in estimates])
         eventprobs_sp = np.array([x[3] for x in estimates])
         return lkhs_sp, mags_sp, pars_sp, eventprobs_sp
     
-    def fit(self, step=1, verbose=True, figsize=(12,3), end=None, stdev=None, threshold=1, trace=False):
+    def fit(self, step=1, verbose=True, figsize=(12,3), end=None, threshold=None, trace=False):
         '''
         '''
         if end is None:
             end = self.mean_d
         n_points = int(end//step)
         if threshold is None:
-            threshold = (stdev/np.sqrt(self.n_trials))
-            print(threshold)
+            means = np.array([np.mean(self.events[np.random.choice(range(len(self.events)), self.n_trials),:], axis=0) for x in range(1000)])
+            threshold = np.abs(np.max(np.percentile(means, [0.01, 99.99], axis=0)))
         end = step*(n_points)#Rounding up to step size  
         lkh = -np.inf
         pars = np.zeros((n_points-1,2))
         pars[:,0] = self.shape
         pars[0,1] = 0.5#initialize with one event
         mags = np.zeros((n_points-1, self.n_dims))
         pbar = tqdm(total = end)
-        n_events, j, time = 1,1,0
+        n_events, j, time = 0,1,0
         last_stage = end
         if trace:
             all_pars, all_mags, all_mags_prop, all_pars_prop, all_diffs = [],[],[],[],[]
         pars_accepted, mags_accepted = pars.copy(), mags.copy()
         pars_prop = pars_accepted[:n_events+2].copy()#cumulative
         pars_prop[n_events,1] = step*j/self.shape
         last_stage = end/self.shape - np.sum(pars_prop[:n_events+1,1])
         pars_prop[n_events+1,1] = last_stage
         while last_stage*self.shape > self.location+step:
             prev_n_events, prev_lkh, prev_time = n_events, lkh, time
-            mags_prop = mags[:n_events+1].copy()
+            mags_prop = mags[:n_events+1].copy()#cumulative
             lkh, mags[:n_events+1], pars[:n_events+2], _ = \
                 self.EM(n_events+1, mags_prop, pars_prop.copy(), 1, [], [])
-            diffs = np.diff(mags[:n_events+1], axis=0)
-            if np.all(np.any(np.abs(diffs) > threshold, axis=1)):
+            signif = True# np.all(np.any(np.abs(mags[:n_events+1]) > threshold, axis=1))
+            if n_events > 0:
+                diffs = np.all(np.any(np.abs(np.diff(mags[:n_events+1], axis=0)) > threshold, axis=1))
+            else:
+                diffs = True
+            if signif and diffs:
                 n_events += 1
                 pars_accepted = pars[:n_events+2].copy()
                 mags_accepted = mags[:n_events+2].copy()
                 mags_accepted[n_events] =  np.zeros(self.n_dims)
                 j = 0
                 if verbose:
                     print(f'Transition event {n_events} found around sample {int(np.round(np.sum(pars_accepted[:n_events,:].prod(axis=1))))}')#: Transition event samples = {np.round(pars[:n_events].prod(axis=1).cumsum())+self.location*np.arange(n_events)}')
             if trace:
                 all_mags_prop.append(mags_prop.copy())
                 all_pars_prop.append(pars_prop.copy())
                 all_mags.append(mags_accepted[:n_events].copy())
                 all_pars.append(pars_accepted[:n_events+1].copy())
-                all_diffs.append(diffs)
+                all_diffs.append(np.abs(np.diff(mags[:n_events+1], axis=0)))
             j += 1
-            pars_prop = pars[:n_events+2].copy()#cumulative
+            pars_prop = pars_accepted[:n_events+2].copy()
             pars_prop[n_events,1] = step*j/self.shape
             last_stage = end/self.shape - np.sum(pars_prop[:n_events+1,1])
             pars_prop[n_events+1,1] = last_stage
             time = np.sum(pars_prop[:n_events,1])*self.shape + \
                 self.location*n_events + step*j/self.shape
             try:
                 pbar.update(int(np.round(time-prev_time+1)))
```

### Comparing `hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/simulations.py` & `hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/simulations.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 import os
 import numpy as np
 import mne
 from mne.datasets import sample
 from warnings import warn
 
 
-def available_sources():
+def available_sources(subselection=True):
     '''
     list available sources for sample subject in MNE
     '''
     data_path = sample.data_path()
     subjects_dir = op.join(data_path, 'subjects')
-    labels = mne.read_labels_from_annot('sample', subjects_dir=subjects_dir)
+    labels = mne.read_labels_from_annot('sample', subjects_dir=subjects_dir, verbose=False)
     named_labels = []
     for label in range(len(labels)):
         named_labels.append(labels[label].name)
+    #Here we select sources with different topologies on HMP and relativ equal contribution on channels, not checked on MEG
+    named_labels = np.array(named_labels)
+    if subselection:
+        named_labels = named_labels[[0,1,3,5,7,15,17,22,30,33,37,40,42,46,50,54,57,59,65,67]]
     return named_labels
 
 def simulation_sfreq():
     data_path = sample.data_path()
     subjects_dir = op.join(data_path, 'subjects')
     evoked_fname = op.join(data_path, 'MEG', 'sample', 'sample_audvis-ave.fif')
     info = mne.io.read_info(evoked_fname, verbose=False)
@@ -32,29 +36,29 @@
 def simulation_positions():
     from mne import channels
     data_path = sample.data_path()
     subjects_dir = op.join(data_path, 'subjects')
     subject = 'sample'
     evoked_fname = op.join(data_path, 'MEG', subject, 'sample_audvis-ave.fif')
     info = mne.io.read_info(evoked_fname, verbose=False)
-    positions = np.delete(channels.layout._find_topomap_coords(info, 'eeg'),52,axis=0)#inferring electrode location using MNE    
+    positions = np.delete(channels.layout._find_topomap_coords(info, 'eeg'),52,axis=0)#inferring channel location using MNE    
     return positions
 
 def bump_shape(bump_width, bump_width_samples, steps):
     '''
     Computes the template of a half-sine (bump) with given frequency f and sampling frequency
     '''
     bump_idx = np.arange(bump_width_samples)*steps+steps/2
     bump_frequency = 1000/(bump_width*2)#gives bump frequency given that bumps are defined as half-sines
     template = np.sin(2*np.pi*bump_idx/1000*bump_frequency)#bump morph based on a half sine with given bump width and sampling frequency
     template = template/np.sum(template**2)#Weight normalized
     return template
 
 
-def simulate(sources, n_trials, n_jobs, file, data_type='eeg', n_subj=1, path='./', overwrite=False, verbose=False, noise=True, times=None, location=1): 
+def simulate(sources, n_trials, n_jobs, file, data_type='eeg', n_subj=1, path='./', overwrite=False, verbose=False, noise=True, times=None, location=1, seed=None): 
     '''
     Simulates n_trials of EEG and/or MEG using MNE's tools based on the specified sources
     
     Parameters
     ----------
     sources : list
         2D or 3D list with dimensions (n_subjects *) sources * source_parameters
@@ -89,14 +93,16 @@
     Returns
     -------
     generating_events: ndarray
         Times of the simulated bumps used to test for accurate recovery compared to estimation
     files: list
         list of file names (file + number of subject)
     '''
+    if seed is not None:
+        random_state = np.random.RandomState(seed)
     sources = np.array(sources, dtype=object)
     if len(np.shape(sources)) == 2:
         sources = [sources]#If only one subject
     if np.shape(sources)[0] != n_subj:
         raise ValueError('Number of subject is not coherent with the sources provided')
     #Infer max duration of a trial from the specified sources
     percentiles = np.empty(len(sources[0]))
@@ -128,14 +134,15 @@
     info = mne.pick_info(info, picked_type)
     tstep = 1. / info['sfreq']
     # To simulate sources, we also need a source space. It can be obtained from the
     # forward solution of the sample subject.
     fwd_fname = op.join(data_path, 'MEG', subject,'sample_audvis-meg-eeg-oct-6-fwd.fif')
     fwd = mne.read_forward_solution(fwd_fname, verbose=verbose)
     src = fwd['src']
+
     
     #For each subject, simulate associated sources
     files = []
     for subj in range(n_subj):
         #Build simulator
         files_subj = []
         source_simulator = mne.simulation.SourceSimulator(src, tstep=tstep, first_samp=0, \
@@ -157,36 +164,36 @@
             stim_onsets =  2000+max_trial_length * np.arange(n_trials)#2000 = offset of first stim
             events[:,0] = stim_onsets#last event 
             events[:,2] = 1#trigger 1 = stimulus 
 
             #Fake source, actually stimulus onset
             selected_label = mne.read_labels_from_annot(
                     subject, regexp=sources_subj[0][0], subjects_dir=subjects_dir, verbose=verbose)[0]
-            label = mne.label.select_sources(subject, selected_label, subjects_dir=subjects_dir)
+            label = mne.label.select_sources(subject, selected_label, subjects_dir=subjects_dir, random_state=random_state)
             source_time_series = np.array([1e-99])#stim trigger
             source_simulator.add_data(label, source_time_series, events)
             source_simulator.add_data(label, source_time_series, events)
 
             trigger = 2
             random_source_times = []
             generating_events = events
             for source in sources_subj:
                 selected_label = mne.read_labels_from_annot(
                     subject, regexp=source[0], subjects_dir=subjects_dir, verbose=verbose)[0]
-                label = mne.label.select_sources(subject, selected_label, subjects_dir=subjects_dir, location='random', extent=1)
+                label = mne.label.select_sources(subject, selected_label, subjects_dir=subjects_dir, location=0, grow_outside=False, random_state=random_state)
                 #last two parameters ensure sources that are different enough
                 # Define the time course of the activity for each source of the region to
                 # activate
                 bump_duration = int(((1/source[1])/2)*info['sfreq'])
                 source_time_series = bump_shape(((1000/source[1])/2),bump_duration,1000/info['sfreq'])*source[2]
 
                 #adding source event
                 events = events.copy()
                 if times is None:
-                    rand_i = np.round(source[-1].rvs(size=n_trials)/(tstep*1000),decimals=0)
+                    rand_i = np.round(source[-1].rvs(size=n_trials, random_state=random_state)/(tstep*1000),decimals=0)
                 else:
                     rand_i = times[:,trigger-2]
                 if len(sources_subj)+1 > trigger > 2:
                     rand_i += location/(tstep*1000)
                 else:
                     rand_i += 1
                 if 0 in rand_i:
@@ -208,18 +215,20 @@
                 raw = raw.pick_types(meg=False, eeg=True, stim=True)
             elif data_type == 'meg':
                 raw = raw.pick_types(meg=True, eeg=False, stim=True)
             elif data_type == 'eeg/meg':
                 raw = raw.pick_types(meg=True, eeg=True, stim=True)
             if noise:
                 cov = mne.make_ad_hoc_cov(raw.info, verbose=verbose)
-                mne.simulation.add_noise(raw, cov, iir_filter=[0.2, -0.2, 0.04], verbose=verbose)
+                mne.simulation.add_noise(raw, cov, iir_filter=[0.2, -0.2, 0.04], verbose=verbose, random_state=random_state)
+            data = raw.get_data()
             raw.save(subj_file, overwrite=True)
             files_subj.append(subj_file)
             np.save(subj_file.split('.fif')[0]+'_generating_events.npy', generating_events)
             files_subj.append(subj_file.split('.fif')[0]+'_generating_events.npy')
             files.append(files_subj)
             print(f'{subj_file} simulated')
     if n_subj == 1:
         return files[0]
     else:
-        return files
+        return files
+
```

### Comparing `hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/utils.py` & `hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import xarray as xr
 import multiprocessing as mp
 import itertools
 import pandas as pd
 import warnings
 from warnings import warn, filterwarnings
 
+filterwarnings('ignore', 'Degrees of freedom <= 0 for slice.', )#weird warning, likely due to nan in xarray, not important but better fix it later 
+
 def read_mne_EEG(pfiles, event_id=None, resp_id=None, epoched=False, sfreq=None, 
                  subj_idx=None, metadata = None, events_provided=None, rt_col='response',
                  verbose=True, tmin=-.2, tmax=5, offset_after_resp = 0, 
                  high_pass=.5, low_pass = None, pick_channels = 'eeg', baseline=(None, 0),
                  upper_limit_RT=5, lower_limit_RT=0.001, reject_threshold=None):
     warn('This method is deprecated and will be removed in future version, use read_mne_data instead', DeprecationWarning, stacklevel=2)
     return read_mne_data(pfiles, event_id, resp_id, epoched, sfreq, 
@@ -23,15 +25,15 @@
                  high_pass, low_pass, pick_channels, baseline,
                  upper_limit_RT, lower_limit_RT, reject_threshold)
 
 def read_mne_data(pfiles, event_id=None, resp_id=None, epoched=False, sfreq=None, 
                  subj_idx=None, metadata=None, events_provided=None, rt_col='rt', rts=None,
                  verbose=True, tmin=-.2, tmax=5, offset_after_resp = 0, 
                  high_pass=.5, low_pass = None, pick_channels = 'eeg', baseline=(None, 0),
-                 upper_limit_RT=5, lower_limit_RT=0.001, reject_threshold=None, scale=1):
+                 upper_limit_RT=np.inf, lower_limit_RT=0, reject_threshold=None, scale=1):
     ''' 
     Reads EEG/MEG data format (.fif or .bdf) using MNE's integrated function .
     
     Notes: 
     - Only EEG or MEG data are selected (other channel types are discarded)
     - All times are expressed on the second scale.
     - If multiple files in pfiles the data of the group is read and seqentially processed.
@@ -41,15 +43,15 @@
     if data not already epoched:
         0.1) the data is filtered with filters specified in low_pass and high_pass. Parameters of the filter are
         determined by MNE's filter function.
         0.2) if no events is provided, detect events in stumulus channel and keep events with id in event_id and resp_id.
         0.3) eventual downsampling is performed if sfreq is lower than the data's sampling frequency. The event structure is
         passed at the resample() function of MNE to ensure that events are approriately timed after downsampling.
         0.4) epochs are created based on stimulus onsets (event_id) and tmin and tmax. Epoching removes any epoch where a 
-        'BAD' annotiation is present and all epochs where an electrode exceeds reject_threshold. Epochs are baseline 
+        'BAD' annotiation is present and all epochs where an channel exceeds reject_threshold. Epochs are baseline 
         corrected from tmin to stimulus onset (time 0).)
     1) Reaction times (RT) are computed based on the sample difference between onset of stimulus and response triggers. 
         If no response event happens after a stimulus or if RT > upper_limit_RT & < upper_limit_RT, RT is 0.
     2) all the non-rejected epochs with positive RTs are cropped to stimulus onset to stimulus_onset + RT.
     
     Parameters
     ----------
@@ -93,32 +95,37 @@
         Rejection threshold to apply when creating epochs, expressed in microvolt
     scale: float
         Scale to apply to the RT data (e.g. 1000 if ms)
         
     Returns
     -------
     epoch_data : xarray
-        Returns an xarray Dataset with all the data, events, electrodes, participant. 
-        All eventual participant/electrodes naming and epochs index are kept. 
+        Returns an xarray Dataset with all the data, events, channels, participant. 
+        All eventual participant/channels naming and epochs index are kept. 
         The choosen sampling frequnecy is stored as attribute.
     '''
     import mne
     dict_datatype = {False:'continuous', True:'epoched'}
     epoch_data = [] 
     if isinstance(pfiles,str):#only one participant
         pfiles = [pfiles]
     if not subj_idx:
         subj_idx = ["S"+str(x) for x in np.arange(len(pfiles))]
     if isinstance(subj_idx,str):
         subj_idx = [subj_idx]
+    if upper_limit_RT<0 or lower_limit_RT<0:
+        raise ValueError('Limit to RTs cannot be negative')
     y = 0
-    metadata_i = None
+    if metadata is not None:
+        if len(pfiles)> 1 and len(metadata) != len(pfiles):
+            raise ValueError(f'Incompatible dimension between the provided metadata {len(metadata)} and the number of eeg files provided {len(pfiles)}')
+    else:
+        metadata_i = None
     for participant in pfiles:
-        if metadata_i is not None:
-            metadata = None#avoids confusion of metadata infered for prev_subj
+
         print(f"Processing participant {participant}'s {dict_datatype[epoched]} {pick_channels}")
 
         # loading data
         if epoched == False:# performs epoching on raw data
             if '.fif' in participant:
                 data = mne.io.read_raw_fif(participant, preload=False, verbose=verbose)
             elif '.bdf' in participant:
@@ -161,58 +168,72 @@
 
             offset_after_resp_samples = int(offset_after_resp*sfreq)
             if metadata is None:
                 metadata_i, meta_events, event_id = mne.epochs.make_metadata(
                     events=events, event_id=combined, tmin=tmin, tmax=tmax,
                     sfreq=data.info["sfreq"], row_events=stim, keep_first=["response"])
                 metadata_i = metadata_i[["event_name","response"]]#only keep event_names and rts
+            else:
+                metadata_i = metadata[y]
             epochs = mne.Epochs(data, meta_events, event_id, tmin, tmax, proj=False,
                     baseline=baseline, preload=True, picks=pick_channels,
                     verbose=verbose, detrend=1, on_missing = 'warn', event_repeated='drop',
                     metadata=metadata_i, reject_by_annotation=True, reject=reject_threshold)
             epochs.metadata.rename({'response':'rt'}, axis=1, inplace=True)
-            rts = epochs.metadata.rt
+            metadata_i = epochs.metadata
         else:
             if '.fif' in participant:
                 epochs = mne.read_epochs(participant, preload=True, verbose=verbose)
                 if sfreq is None: 
                     sfreq = epochs.info['sfreq']
                 elif sfreq  < epochs.info['sfreq']:
                     if verbose:
                         print(f'Resampling data at {sfreq}')
                     epochs = epochs.resample(sfreq)
             else:
                 raise ValueError('Incorrect file format')
             _pick_channels(pick_channels,epochs, stim=False)
-            if metadata is not None and not isinstance(metadata, pd.DataFrame):
-                raise ValueError('Metadata should be a pandas data-frame as generated by mne')
-            metadata = epochs.metadata#accounts for dropped epochs
+            if metadata is None:
+                try:
+                    metadata_i = epochs.metadata#accounts for dropped epochs
+                except:
+                    raise ValueError('Missing metadata in the epoched data')
+            elif isinstance(metadata, pd.DataFrame):
+                if len(pfiles)>1:
+                    metadata_i = metadata[y].copy()#TODO, better account for participant's wide provided metadata
+                else:
+                    metadata_i = metadata.copy()
+            else:
+                raise ValueError('Metadata should be a pandas data-frame as generated by mne or be contained in the passed epoch data')
         offset_after_resp_samples = np.rint(offset_after_resp*sfreq).astype(int)
         valid_epoch_index = [x for x,y in enumerate(epochs.drop_log) if len(y) == 0]
         data_epoch = epochs.get_data()#preserves index
-        if isinstance(metadata, pd.DataFrame):
-            if len(metadata) > len(data_epoch):#assumes metadata contains rejected epochs
-                metadata = metadata.iloc[valid_epoch_index]
-                metadata.reset_index(drop=True, inplace=True)
+        rts = metadata_i[rt_col]
+        if isinstance(metadata_i, pd.DataFrame):
+            if len(metadata_i) > len(data_epoch):#assumes metadata contains rejected epochs
+                print(True)
+                metadata_i = metadata_i.iloc[valid_epoch_index]
+                metadata_i.reset_index(drop=True, inplace=True)
+                rts = metadata_i[rt_col]
             try:
-                rts = metadata[rt_col]/scale
+                rts = rts/scale
             except:
                 raise ValueError(f'Expected column named {rt_col} in the provided metadata file, alternative names can be passed through the rt_col parameter')
         elif rts is None:
             raise ValueError(f'Expected either a metadata Dataframe or an array of Reaction Times')
         rts_arr = np.array(rts)
         if verbose:
             print(f'Applying reaction time trim to keep RTs between {lower_limit_RT} and {upper_limit_RT} seconds')
         rts_arr[rts_arr > upper_limit_RT] = 0 #removes RT above x sec
         rts_arr[rts_arr < lower_limit_RT] = 0 #removes RT below x sec, important as determines max events
         rts_arr[np.isnan(rts_arr)] = 0#too long trial
         rts_arr = np.rint(rts_arr*sfreq).astype(int)
         if verbose:
             print(f'{len(rts_arr[rts_arr > 0])} RTs kept of {len(rts_arr)} clean epochs')
-        triggers = epochs.metadata.iloc[:,0].values#assumes first col is trigger
+        triggers = metadata_i.iloc[:,0].values#assumes first col is trigger
         cropped_data_epoch = np.empty([len(rts_arr[rts_arr>0]), len(epochs.ch_names), max(rts_arr)+offset_after_resp_samples])
         cropped_data_epoch[:] = np.nan
         cropped_trigger = []
         epochs_idx = []
         j = 0
         time0 = epochs.time_as_index(0)[0]
         for i in range(len(data_epoch)):
@@ -228,30 +249,32 @@
             cropped_data_epoch = cropped_data_epoch[:-1]
             x += 1
         if x > 0:
             print(f'RTs > 0 longer than expected ({x})')
         print(f'{len(cropped_data_epoch)} trials were retained for participant {participant}')
         if verbose:
             print(f'End sampling frequency is {sfreq} Hz')
-        epoch_data.append(hmp_data_format(cropped_data_epoch, cropped_trigger, epochs.info['sfreq'], offset_after_resp_samples, epochs=[int(x) for x in epochs_idx], electrodes = epochs.ch_names, metadata = metadata))
+
+        epoch_data.append(hmp_data_format(cropped_data_epoch, epochs.info['sfreq'], None, offset_after_resp_samples, epochs=[int(x) for x in epochs_idx], electrodes = epochs.ch_names, metadata = metadata_i))
+
         y += 1
     epoch_data = xr.concat(epoch_data, dim = xr.DataArray(subj_idx, dims='participant'),
                           fill_value={'event':'', 'data':np.nan})
     return epoch_data
 
 def _pick_channels(pick_channels,data,stim=True):
     if isinstance(pick_channels, list):
         try:
-            data = data.pick_channels(pick_channels)
+            data = data.pick(pick_channels)
         except:
-            raise ValueError('incorrect electrode pick specified')
-    elif pick_channels == 'eeg':
-            data = data.pick_types(meg=False, eeg=True, stim=stim, eog=False, misc=False, exclude='bads') 
+            raise ValueError('incorrect channel pick specified')
+    elif pick_channels == 'eeg' or pick_channels == 'meg':
+            data = data.pick(pick_channels)
     else:
-         raise ValueError('incorrect electrode pick specified')
+         raise ValueError('incorrect channel pick specified')
     return data
 
 def parsing_epoched_eeg(data, rts, conditions, sfreq, start_time=0, offset_after_resp=0.1):
     '''
     Function to parse epochs and crop them to start_time (usually stimulus onset so 0) up to the reaction time of the trial.
     The returned object is a xarray Dataset allowing further processing using built-in methods
 
@@ -260,22 +283,22 @@
     by np.nan (e.g. rts[rts < 200] = np.nan) or 0
     2) RTs and conditions need to be ordered in the same way as the epochs
     
     
     Parameters
     ----------
     data: pandas.dataframe
-        pandas dataframe with columns time (in milliseconds), epoch number and one column for each electrode 
-        (column name will be taken as electrode names)
+        pandas dataframe with columns time (in milliseconds), epoch number and one column for each channel 
+        (column name will be taken as channel names)
     rts: list or 1d array
         list of reaction times in milliseconds for each epoch 
     epoch_index: list or 1d array
         number of the index (important for eventual dropped trials during the prepro154,cessing
-    electrode_index: list or 1d array
-        list of name of the electrodes
+    channel_index: list or 1d array
+        list of name of the channels
     condition: list or 1d array
         list of condition associated with each epoch
     sfreq: float
         sampling frequency of the data
     start_time: float
         time defining the onset of a trial (default is 0 as trial usually defined from event/stimulus onset) in milliseconds
     offset_after_resp: float
@@ -301,18 +324,18 @@
     rts = np.array([int(x) for x in rts/tstep])
     data = data[data.time >= start_time]#remove all baseline values
     epochs = data.epoch.unique()
     rts = rts[epochs]
     conditions = conditions[epochs]
     times = data.time.unique()
     data = data.drop(columns=['time', 'epoch'])
-    #electrode names/columns are assumed to be remaining columns affter removing time and epoch columns
-    electrode_columns = [x for x in data.columns]
+    #channel names/columns are assumed to be remaining columns affter removing time and epoch columns
+    channel_columns = [x for x in data.columns]
     data = data.values.flatten()
-    data = data.reshape((len(epochs), len(times),len(electrode_columns)))
+    data = data.reshape((len(epochs), len(times),len(channel_columns)))
     data = np.swapaxes(data,1,2)
 
     nan_con = np.array([i for i,x in enumerate(conditions) if isinstance(x, float) and np.isnan(x)])
     if len(nan_con) > 0:
         print(f'NaN present in condition array, removing associated epoch and RT ({nan_con})')
         data = np.delete(data, nan_con, axis=0)
         conditions = np.delete(conditions, nan_con, axis=0)
@@ -324,88 +347,96 @@
             data[epoch,:,:] = np.nan
             conditions[epoch] = ''
             #rts[epoch] = None#np.nan#np.delete(rts, epoch, axis=0)
             #epochs[epoch] = np.nan#np.delete(epochs, epoch, axis=0)
         epoch += 1
     cropped_conditions = []
     epoch_idx = []
-    cropped_data_epoch = np.empty([len(epochs), len(electrode_columns), max(rts)+offset_after_resp_samples])
+    cropped_data_epoch = np.empty([len(epochs), len(channel_columns), max(rts)+offset_after_resp_samples])
     cropped_data_epoch[:] = np.nan
     j = 0
     for epoch in np.arange(len(data)):
         #Crops the epochs up to RT
         cropped_data_epoch[j,:,:rts[epoch]+offset_after_resp_samples] = \
         (data[epoch,:,:rts[epoch]+offset_after_resp_samples])
         j += 1
     print(f'Totaling {len(cropped_data_epoch)} valid trials')
-    data_xr = hmp_data_format(cropped_data_epoch, conditions, sfreq, offset_after_resp_samples, epochs=epochs, electrodes = electrode_columns)
+
+    data_xr = hmp_data_format(cropped_data_epoch, sfreq, conditions, offset_after_resp_samples, epochs=epochs, electrodes = electrode_columns)
     return data_xr
 
-def hmp_data_format(data, events, sfreq, offset=0, participants=[], epochs=None, electrodes=None, metadata=None):
+def hmp_data_format(data, sfreq, events=None, offset=0, participants=[], epochs=None, electrodes=None, metadata=None):
+
     '''
-    Converting 3D matrix with dimensions (participant) * trials * electrodes * sample into xarray Dataset
+    Converting 3D matrix with dimensions (participant) * trials * channels * sample into xarray Dataset
     
     Parameters
     ----------
     data : ndarray
-        4/3D matrix with dimensions (participant) * trials * electrodes * sample  
+        4/3D matrix with dimensions (participant) * trials * channels * sample  
     events : ndarray
         np.array with 3 columns -> [samples of the event, initial value of the channel, event code]. To use if the
         automated event detection method of MNE is not appropriate 
     sfreq : float
         Sampling frequency of the data
     participants : list
         List of participant index
     epochs : list
         List of epochs index
-    electrodes : list
-        List of electrode index
+    channels : list
+        List of channel index
     '''
     if len(np.shape(data)) == 4:#means group
-        n_subj, n_epochs, n_electrodes, n_samples = np.shape(data)
+        n_subj, n_epochs, n_channels, n_samples = np.shape(data)
     elif len(np.shape(data)) == 3:
-        n_epochs, n_electrodes, n_samples = np.shape(data)
+        n_epochs, n_channels, n_samples = np.shape(data)
+        n_subj = 1
     else:
         raise ValueError(f'Unknown data format with dimensions {np.shape(data)}')
-    if events is None:
-        events = np.repeat(np.nan, n_epochs)
     if electrodes is None:
         electrodes = np.arange(n_electrodes)
     if epochs is None:
          epochs = np.arange(n_epochs)
-    if len(participants) < 2:
+    if n_subj < 2:
         data = xr.Dataset(
                 {
-                    "data": (["epochs", "electrodes", "samples"],data),
+                    "data": (["epochs", "channels", "samples"],data),
                 },
                 coords={
                     "epochs" :epochs,
-                    "electrodes":  electrodes,
+                    "channels":  channels,
                     "samples": np.arange(n_samples)
                 },
                 attrs={'sfreq':sfreq,'offset':offset}
                 )
     else:
         data = xr.Dataset(
                 {
-                    "data": (['participant',"epochs", "electrodes", "samples"],data),
+                    "data": (['participant',"epochs", "channels", "samples"],data),
                 },
                 coords={
                     'participant':participants,
                     "epochs" :epochs,
-                    "electrodes":  electrodes,
+                    "channels":  channels,
                     "samples": np.arange(n_samples)
                 },
                 attrs={'sfreq':sfreq,'offset':offset}
                 )
     if metadata is not None:
         metadata = metadata.to_xarray()
         metadata = metadata.rename_dims({'index':'epochs'})
         metadata = metadata.rename_vars({'index':'epochs'})
         data = data.merge(metadata)
+        data = data.set_coords(list(metadata.data_vars))
+    if events is not None:
+        data['events'] = xr.DataArray(
+            events,
+            dims=("participant", "epochs"),
+            coords={"participant": participants, "epochs": epochs})
+        data = data.set_coords('events')
     return data
 
 def standardize(x):
     '''
     Scaling variances to mean variance of the group
     '''
     return ((x.data / x.data.std(dim=...))*x.mean_std)
@@ -421,58 +452,58 @@
 def zscore(data):
     '''
     zscore of the data
     '''
     return (data - data.mean()) / data.std()
 
 
-def stack_data(data, subjects_variable='participant', electrode_variable='component', single=False):
+def stack_data(data, subjects_variable='participant', channel_variable='component', single=False):
     '''
-    Stacks the data going from format [participant * epochs * samples * electrodes] to [samples * electrodes]
+    Stacks the data going from format [participant * epochs * samples * channels] to [samples * channels]
     with sample indexes starts and ends to delimitate the epochs.
     
     
     Parameters
     ----------
     data : xarray
         unstacked xarray data from transform_data() or anyother source yielding an xarray with dimensions 
-        [participant * epochs * samples * electrodes] 
+        [participant * epochs * samples * channels] 
     subjects_variable : str
         name of the dimension for subjects ID
     single : bool 
         Whether participant is unique (True) or a group of participant (False)
     
     Returns
     -------
     data : xarray.Dataset
-        xarray dataset [samples * electrodes]
+        xarray dataset [samples * channels]
     '''    
     if isinstance(data, (xr.DataArray,xr.Dataset)) and 'component' not in data.dims:
-        data = data.rename_dims({'electrodes':'component'})
+        data = data.rename_dims({'channels':'component'})
         print(data.participant)
     if "participant" not in data.dims:
         data = data.expand_dims("participant")
     data = data.stack(all_samples=['participant','epochs',"samples"]).dropna(dim="all_samples")
     return data #xr.Dataset({'data':data, 'durations':durations})
     #return data, durations
 
 def transform_data(data, subjects_variable="participant", apply_standard=True,  apply_zscore=True, method='pca', n_comp=None, return_weights=False):
     '''
     Adapts EEG epoched data (in xarray format) to the expected data format for hmps. 
     First this code can apply standardization of individual variances (if apply_standard=True).
     Second, a spatial PCA on the average variance-covariance matrix is performed (if method='pca', more methods in development)
-    Third,stacks the data going from format [participant * epochs * samples * electrodes] to [samples * electrodes]
+    Third,stacks the data going from format [participant * epochs * samples * channels] to [samples * channels]
     Last, performs z-scoring on each epoch and for each principal component (PC)
     
     
     Parameters
     ----------
     data : xarray
         unstacked xarray data from transform_data() or anyother source yielding an xarray with dimensions 
-        [participant * epochs * samples * electrodes] 
+        [participant * epochs * samples * channels] 
     subjects_variable : str
         name of the dimension for subjects ID
     apply_standard : bool 
         Whether to apply standardization
     apply_zscore : bool 
         Whether to apply z-scoring
     method : str
@@ -482,32 +513,32 @@
         to specify how many PCs should be retained
 
     Returns
     -------
     data : xarray.Dataset
         xarray dataset [n_samples * n_comp] data expressed in the PC space, ready for hsMM fit
     pca_data : xarray.Dataset
-        loadings of the PCA, used to retrieve electrode space
+        loadings of the PCA, used to retrieve channel space
     pca.explained_variance_ : ndarray
         explained variance for each component
     means : xarray.DataArray
-        means of the electrodes before PCA/zscore
+        means of the channels before PCA/zscore
     '''
     if isinstance(data, xr.DataArray):
         raise ValueError('Expected a xarray Dataset with data and event as DataArrays, check the data format')
     if apply_standard:
         mean_std = data.groupby(subjects_variable).std(dim=...).data.mean()
         data = data.assign(mean_std=mean_std.data)
         data = data.groupby(subjects_variable).map(standardize)
     if method == 'pca':
         from sklearn.decomposition import PCA
         var_cov_matrices = []
         if isinstance(data, xr.Dataset):
             data = data.data
-        for i,trial_dat in data.stack(trial=("participant", "epochs")).groupby('trial'):
+        for i,trial_dat in data.stack(trial=("participant", "epochs")).drop_duplicates('trial').groupby('trial'):
             var_cov_matrices.append(vcov_mat(trial_dat)) #Would be nice not to have a for loop but groupby.map seem to fal
         var_cov_matrix = np.mean(var_cov_matrices,axis=0)
         # Performing spatial PCA on the average var-cov matrix
         if n_comp == None:
             import matplotlib.pyplot as plt
             n_comp = np.shape(var_cov_matrix)[0]-1
             fig, ax = plt.subplots(1,2, figsize=(.2*n_comp, 4))
@@ -526,22 +557,22 @@
             n_comp = int(input(f'How many PCs (90 and 99% explained variance at component n{np.where(np.cumsum(var/np.sum(var)) >= .90)[0][0]+1} and n{np.where(np.cumsum(var/np.sum(var)) >= .99)[0][0]+1})?'))
 
         pca = PCA(n_components=n_comp, svd_solver='full')#selecting Principale components (PC)
 
         pca_data = pca.fit_transform(var_cov_matrix)/pca.explained_variance_ # divided by explained var for compatibility with matlab's PCA
         
         #Rebuilding pca PCs as xarray to ease computation
-        coords = dict(electrodes=("electrodes", data.coords["electrodes"].values),
+        coords = dict(channels=("channels", data.coords["channels"].values),
                      component=("component", np.arange(n_comp)))
-        pca_data = xr.DataArray(pca_data, dims=("electrodes","component"), coords=coords)
-        means = data.groupby('electrodes').mean(...)
+        pca_data = xr.DataArray(pca_data, dims=("channels","component"), coords=coords)
+        means = data.groupby('channels').mean(...)
         data = data @ pca_data
 
     elif method is None:
-        data = data.rename({'electrodes':'component'})
+        data = data.rename({'channels':'component'})
         data['component'] = np.arange(len(data.component ))
     if apply_zscore:
         data = data.stack(trial=[subjects_variable,'epochs','component']).groupby('trial').map(zscore).unstack()
     if stack_data:
         data = stack_data(data)
     if return_weights:
         return data, pca_data, pca.explained_variance_, means
@@ -724,41 +755,41 @@
 
     loocv = xr.DataArray(np.array(loocv)[:,:,0].astype(np.float64), coords={"n_event":np.arange(1,bests.n_events.max().values+1)[::-1],
                                                            "participants":np.array(loocv)[0,:,1]}, name="loo_likelihood")
     return loocv
 
 def reconstruct(magnitudes, PCs, eigen, means):
     '''
-    Reconstruct electrode activity from PCA
+    Reconstruct channel activity from PCA
     
     Parameters
     ----------
     magnitudes :  
         2D or 3D ndarray with [n_components * n_events] can also contain several estimations [estimation * n_components * n_events]
     PCs : 
         2D ndarray with PCA loadings [channels x n_components]
     eigen : 
         PCA eigenvalues of the covariance matrix of data [n_components]
     means : 
         Grand mean [channels]
         
     Returns
     -------
-    electrodes : ndarray
-        a 2D ndarray with [electrodes * events]
+    channels : ndarray
+        a 2D ndarray with [channels * events]
     '''
     if len(np.shape(magnitudes))==2:
         magnitudes = np.array([magnitudes])
     n_iter, n_comp, n_events = np.shape(magnitudes)
-    list_electrodes = []
+    list_channels = []
     for iteration in np.arange(n_iter): 
-        #electrodes = np.array(magnitudes[iteration].T * 
-        electrodes =  np.array(magnitudes[iteration, ].T * np.tile(np.sqrt(eigen[:n_comp]).T, (n_events,1))) @ np.array(PCs[:,:n_comp]).T
-        list_electrodes.append(electrodes + np.tile(means,(n_events,1)))#add means for each electrode
-    return np.array(list_electrodes)
+        #channels = np.array(magnitudes[iteration].T * 
+        channels =  np.array(magnitudes[iteration, ].T * np.tile(np.sqrt(eigen[:n_comp]).T, (n_events,1))) @ np.array(PCs[:,:n_comp]).T
+        list_channels.append(channels + np.tile(means,(n_events,1)))#add means for each channel
+    return np.array(list_channels)
 
 def stage_durations(times):
     '''
     Returns the stage durations from the event onset times by substracting each stage to the previous
     
     Parameters
     ----------
@@ -793,42 +824,42 @@
     '''
     Saves eventprobs to filename csv file
     '''
     eventprobs = eventprobs.unstack()
     eventprobs.to_dataframe().to_csv(filename)
     print(f"Saved at {filename}")
 
-def event_times(data, times, electrode, stage):
+def event_times(data, times, channel, stage):
     '''
-    Event times parses the single trial EEG signal of a given electrode in a given stage, from event onset to the next one. If requesting the last
+    Event times parses the single trial EEG signal of a given channel in a given stage, from event onset to the next one. If requesting the last
     stage it is defined as the onset of the last event until the response of the participants.
 
     Parameters
     ----------
     data : xr.Dataset
         HMP EEG data (untransformed but with trial and participant stacked)
     times : xr.DataArray
         Onset times as computed using onset_times()
-    electrode : str
-        Electrode to pick for the parsing of the signal
+    channel : str
+        channel to pick for the parsing of the signal
     stage : float | ndarray
         Which stage to parse the signal into
 
     Returns
     -------
     brp_data : ndarray
         Matrix with trial_x_participant * samples with sample dimension given by the maximum stage duration
     '''
 
     brp_data = np.tile(np.nan, (len(data.trial_x_participant), int(round(max(times.sel(event=stage+1).data- times.sel(event=stage).data)))+1))
     i=0
     for trial, trial_dat in data.groupby('trial_x_participant'):
         trial_time = slice(times.sel(event=stage, trial_x_participant=trial), \
                                                  times.sel(event=stage+1, trial_x_participant=trial))
-        trial_elec = trial_dat.sel(electrodes = electrode, samples=trial_time).squeeze()
+        trial_elec = trial_dat.sel(channels = channel, samples=trial_time).squeeze()
         try:
             brp_data[i, :len(trial_elec)] = trial_elec
         except:
             brp_data[i, :1] = trial_elec
             
         i += 1
 
@@ -845,35 +876,39 @@
     
 def participant_selection(hmp_data, eeg_data, participant):
     unstacked = hmp_data.unstack().sel(participant = participant)
     stacked = stack_data(unstacked)
     return stacked
 
 def bootstrapping(init, hmp_data, general_run, positions, eeg_data, iterations, threshold=1, verbose=True, plots=True, cpus=1):
+    warn('This method is inaccurate and will be removed in future version, see the bootstraping function in the resample module instead', DeprecationWarning, stacklevel=2)
     from hsmm_mvpy.models import hmp
     from hsmm_mvpy.visu import plot_topo_timecourse
-    import xskillscore as xs
+    try:
+        import xskillscore as xs#Todo remove from dependency list
+    except:
+        raise ValueError('xskillscore should be installed to run this (deprecated) function')
     fitted_mags = general_run.magnitudes.values[np.unique(np.where(np.isfinite(general_run.magnitudes))[0]),:]#remove NAs
-    mags_boot_mat = np.tile(np.nan, (iterations, init.compute_max_events(), init.n_dims))
-    pars_boot_mat = np.tile(np.nan, (iterations, init.compute_max_events()+1, 2))
+    mags_boot_mat = []#np.tile(np.nan, (iterations, init.compute_max_events(), init.n_dims))
+    pars_boot_mat = []#np.tile(np.nan, (iterations, init.compute_max_events()+1, 2))
 
     for i in range(iterations):
         bootstapped = xs.resample_iterations(hmp_data.unstack(), iterations=1, dim='epochs')
         hmp_data_boot = stack_data(bootstapped.squeeze())
-        init_boot = hmp(hmp_data_boot, sfreq=eeg_data.sfreq, event_width=50, cpus=15)
-        estimates_boot = init_boot.fit(verbose=verbose, threshold=1)
-        mags_boot_mat[i, :len(estimates_boot.magnitudes),:] = estimates_boot.magnitudes
-        pars_boot_mat[i, :len(estimates_boot.parameters),:] = estimates_boot.parameters
+        init_boot = hmp(hmp_data_boot, sfreq=eeg_data.sfreq, event_width=init.event_width, cpus=init.cpus)
+        estimates_boot = init_boot.fit(verbose=verbose, threshold=threshold)
+        mags_boot_mat.append(estimates_boot.magnitudes)
+        pars_boot_mat.append(estimates_boot.parameters)
         if plots:
             plot_topo_timecourse(eeg_data, estimates_boot, positions, init_boot)
 
     all_pars_aligned = np.tile(np.nan, (iterations, np.max([len(x) for x in pars_boot_mat]), 2))
     all_mags_aligned = np.tile(np.nan, (iterations, np.max([len(x) for x in mags_boot_mat]), init.n_dims))
     for iteration, _i in enumerate(zip(pars_boot_mat, mags_boot_mat)):
         all_pars_aligned[iteration, :len(_i[0]), :] = _i[0]
         all_mags_aligned[iteration, :len(_i[1]), :] = _i[1]
 
     booted = xr.Dataset({'parameters': (('iteration', 'stage','parameter'), 
                                  all_pars_aligned),
                         'magnitudes': (('iteration', 'event','component'), 
                                  all_mags_aligned)})
-    return booted
+    return booted
```

### Comparing `hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/visu.py` & `hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/visu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 '''
 
 '''
 
 import matplotlib.pyplot as plt
 import numpy as np
+import xarray as xr
 from itertools import cycle
 default_colors =  ['cornflowerblue','indianred','orange','darkblue','darkgreen','gold']
 
-def plot_topo_timecourse(electrodes, estimated, channel_position, init, time_step=1, ydim=None,
-                        figsize=None, dpi=100, magnify=1, times_to_display=None, cmap='Spectral_r',
-                        ylabels=[], max_time = None, vmin=None, vmax=None, title=False, ax=False, 
-                        sensors=False, skip_electrodes_computation=False):
+def plot_topo_timecourse(channels, estimated, channel_position, init, time_step=1, ydim=None,
+                figsize=None, dpi=100, magnify=1, times_to_display=None, cmap='Spectral_r',
+                ylabels=[], max_time = None, vmin=None, vmax=None, title=False, ax=None, 
+                sensors=False, skip_channels_computation=False):
     '''
     Plotting the event topologies at the average time of the end of the previous stage.
     
     Parameters
     ----------
-    electrodes : ndarray | xr.Dataarray 
-        a 2D or 3D matrix of electrode activity with electrodes and event as dimension (+ eventually a varying dimension) OR
+    channels : ndarray | xr.Dataarray 
+        a 2D or 3D matrix of channel activity with channels and event as dimension (+ eventually a varying dimension) OR
         the original EEG data in HMP format
     estimated : ndarray
         a 1D or 2D matrix of times with event as dimension OR directly the results from a fitted hmp 
     channel_position : ndarray
-        Either a 2D array with dimension electrode and [x,y] storing electrode location in meters or an info object from
-        the mne package containning digit. points for electrode location
+        Either a 2D array with dimension channel and [x,y] storing channel location in meters or an info object from
+        the mne package containning digit. points for channel location
     init : float
         initialized HMP object
     time_step : float
         What unit to multiply all the times with, if you want to go on the second or millisecond scale you can provide 
         1/sf or 1000/sf where sf is the sampling frequency of the data
     figsize : list | tuple | ndarray
         Length and heigth of the matplotlib plot
@@ -63,61 +64,58 @@
     '''
     
     from mne.viz import plot_topomap
     from mpl_toolkits.axes_grid1.inset_locator import inset_axes
     return_ax = True
     if times_to_display is None:
         times_to_display = init.mean_d*time_step
-    if 'event' in estimated:
-        #This is to keep backward compatibility but supplyng externally computed electrodes and times will probably be
-        # DEPRECATED
+    if isinstance(estimated, (xr.DataArray, xr.Dataset)) and 'event' in estimated:
         if ydim is None and 'n_events' in estimated.dims:
             if estimated.n_events.count() > 1:
                 ydim = 'n_events'
-        if ydim is not None and not skip_electrodes_computation:
-            electrodes = init.compute_topologies(electrodes, estimated, init.event_width_samples, ydim).data
-        elif not skip_electrodes_computation:
-            electrodes = init.compute_topologies(electrodes, estimated, init.event_width_samples).data
-        electrodes[electrodes == 0] = np.nan
+        if ydim is not None and not skip_channels_computation:
+            channels = init.compute_topologies(channels, estimated, init.event_width_samples, ydim).data
+        elif not skip_channels_computation:
+            channels = init.compute_topologies(channels, estimated, init.event_width_samples).data
+        channels[channels == 0] = np.nan
         times = init.compute_times(init, estimated, mean=True).data
     else:#assumes times already computed
         times = estimated
-    if len(np.shape(electrodes)) == 2:
-        electrodes = electrodes[np.newaxis]
-    n_iter = np.shape(electrodes)[0]
-    if isinstance(ax, bool):
+    if len(np.shape(channels)) == 2:
+        channels = channels[np.newaxis]
+    n_iter = np.shape(channels)[0]
+    if ax is None:
         if figsize == None:
             figsize = (12, 1*n_iter)
         fig, ax = plt.subplots(1, 1, figsize=figsize, dpi=dpi)
         return_ax = False
     event_size = init.event_width_samples*time_step*magnify
     yoffset =.25*magnify
     axes = []
     if n_iter == 1:
         times = [times]
     times = np.array(times, dtype=object)
     for iteration in np.arange(n_iter):
         times_iteration = times[iteration]*time_step
-        electrodes_ = electrodes[iteration,:,:]
-        n_event = int(sum(np.isfinite(electrodes_[:,0])))
-        electrodes_ = electrodes_[:n_event,:]
+        channels_ = channels[iteration,:,:]
+        n_event = int(sum(np.isfinite(channels_[:,0])))
+        channels_ = channels_[:n_event,:]
         for event in np.arange(n_event):
-            # if np.sum(electrodes_[event,:]) != 0:
             axes.append(ax.inset_axes([times_iteration[event],iteration-yoffset,
-                                       (event_size),yoffset*2], transform=ax.transData))
-            plot_topomap(electrodes_[event,:], channel_position, axes=axes[-1], show=False,
+                                (event_size),yoffset*2], transform=ax.transData))
+            plot_topomap(channels_[event,:], channel_position, axes=axes[-1], show=False,
                          cmap=cmap, vlim=(vmin, vmax), sensors=sensors)
     if isinstance(ylabels, dict):
         ax.set_yticks(np.arange(len(list(ylabels.values())[0])),
                       [str(x) for x in list(ylabels.values())[0]])
         ax.set_ylabel(str(list(ylabels.keys())[0]))
     else:
         ax.set_yticks([])
         ax.spines['left'].set_visible(False)
-    __display_times(ax, times_to_display, 0, time_step, max_time, times)
+    __display_times(ax, times_to_display, 0, time_step, max_time, times, n_iter)
     if not return_ax:
         ax.spines['top'].set_visible(False)
         ax.spines['right'].set_visible(False)
         ax.set_ylim(0-yoffset, n_iter-1+yoffset)
         if time_step == 1:
             ax.set_xlabel('Time (in samples)')
         else:
@@ -129,15 +127,15 @@
     if return_ax:
         ax.set_ylim(0-yoffset, n_iter-1+yoffset)
         return ax
     else:
         plt.show()    
 
 
-def plot_loocv(loocv_estimates, pvals=True, test='t-test', figsize=(16,5), indiv=True, ax=False, mean=False):
+def plot_loocv(loocv_estimates, pvals=True, test='t-test', figsize=(16,5), indiv=True, ax=None, mean=False):
     '''
     Plotting the LOOCV results
     
     Parameters
     ----------
     loocv_estimates : ndarray or xarra.DataArray
         results from a call to hmp.utils.loocv()
@@ -161,15 +159,15 @@
     if pvals:
         if test == 'sign':
             from statsmodels.stats.descriptivestats import sign_test 
         elif test == 't-test':
             from scipy.stats import ttest_1samp
         else:
             raise ValueError('Expected sign or t-test argument to test parameter')
-    if isinstance(ax, bool):
+    if ax is None:
         fig, ax = plt.subplots(1,2, figsize=figsize)
         return_ax = False
     else:
         return_ax = True
     loocv_estimates = loocv_estimates.dropna('n_event', how='all')
     if mean:
         alpha = .2#for the indiv plot
@@ -316,23 +314,23 @@
                 axs.plot(stage,color=next(cycol) )
     axs.set_ylabel('p(event)')
     axs.set_xlabel('Time (in samples)')
     if xlims:
         axs.set_xlim(xlims[0], xlims[1])
     return axs
 
-def __display_times(ax, times_to_display, yoffset, time_step, max_time, times):
+def __display_times(ax, times_to_display, yoffset, time_step, max_time, times, ymax=1):
     n_iter = len(times)
     times = np.asarray(times,dtype=object)
     if isinstance(times_to_display, (np.ndarray, np.generic)):
         if isinstance(times_to_display, np.ndarray):
-            ax.vlines(times_to_display*time_step, yoffset-1.1, yoffset+1.1, ls='--')
+            ax.vlines(times_to_display*time_step, yoffset-1.1, yoffset+ymax+1.1, ls='--')
             ax.set_xlim(-1*time_step, max(times_to_display)*time_step+((max(times_to_display)*time_step)/15))
         else:
-            ax.vlines(times_to_display*time_step, yoffset-1.1, yoffset+1.1, ls='--')
+            ax.vlines(times_to_display*time_step, yoffset-1.1, yoffset+ymax+1.1, ls='--')
             ax.set_xlim(-1*time_step, times_to_display*time_step+(times_to_display*time_step)/15)
     if max_time:
         ax.set_xlim(-1*time_step, max_time)
     return ax
 
 def plot_latencies_gamma(gammas, event_width=0, time_step=1, labels=[''], colors=default_colors, 
                          figsize=False, times_to_display=None, max_time=None, kind='bar', legend=False):
@@ -472,18 +470,55 @@
     # Only show ticks on the left and bottom spines
     axs.yaxis.set_ticks_position('left')
     axs.xaxis.set_ticks_position('bottom')
     if legend:
         axs.legend()
     return axs
 
-def plot_iterations(iterations, eeg_data, init, positions, dims):
+def plot_iterations(iterations, eeg_data, init, positions, dims=['magnitudes','parameters'], alpha=1, ax=None):
     from hsmm_mvpy.models import hmp
+    if 'iteration' not in iterations.dims:
+        try:
+            iterations['iteration'] = [0]
+        except:
+            iterations = iterations.expand_dims({'iteration':[0]}, axis=1)
+            iterations['iteration'] = [0]
     for iteration in iterations.iteration[:-1]:
         selected = init.fit_single(iterations.sel(iteration=iteration)[dims[0]].dropna(dim='event').event[-1].values+1,\
             magnitudes = iterations.sel(iteration=iteration)[dims[0]].dropna(dim='event'),\
             parameters = iterations.sel(iteration=iteration)[dims[1]].dropna(dim='stage'),\
             threshold=0, verbose=False)
-
         #Visualizing
-        plot_topo_timecourse(eeg_data, selected, positions,  init, magnify=1, sensors=False)
-    
+        plot_topo_timecourse(eeg_data, selected, positions,  init, magnify=1, sensors=False,ax=ax)
+    
+
+def plot_bootstrap_results(bootstrapped, info, init, model_to_compare=None, epoch_data=None):
+    from hsmm_mvpy.resample import percent_event_occurence
+    maxboot_model, labels, counts, event_number, label_event_num = percent_event_occurence(bootstrapped, model_to_compare)
+    fig, axes = plt.subplot_mosaic([['a', 'a'], ['b', 'c'], ['b', 'c']],
+                              layout='constrained')
+    if model_to_compare is None: 
+        plot_topo_timecourse(maxboot_model.channels_activity.values, maxboot_model.event_times.values, info, init,ax=axes['a'])
+        times = maxboot_model.event_times#init.compute_times(init, maxboot_model, mean=True)#computing predicted event times
+    else:
+        plot_topo_timecourse(epoch_data, model_to_compare, info, init,ax=axes['a'])
+        times = init.compute_times(init, model_to_compare, mean=True)
+        maxboot_model = model_to_compare
+    axes['a'].set_xlabel('Time (samples)')
+    axes['b'].bar(maxboot_model.event+1,counts)
+    axes['b'].set_xlabel('Event number')
+    axes['b'].set_xticks(maxboot_model.event+1)
+    axes['b'].set_ylabel('Frequency')
+    axes['b'].set_ylim(0,1)
+    
+    axes['c'].bar(label_event_num,event_number)
+    axes['c'].set_xlabel('Number of events')
+    
+    axes['c'].set_ylabel('Frequency')
+    axes['c'].set_ylim(0,1)
+    axes['a'].spines[['right', 'top']].set_visible(False)
+    axes['b'].spines[['right', 'top']].set_visible(False)
+    axes['c'].spines[['right', 'top']].set_visible(False)
+    # plt.tight_layout()
+    plt.show()
+    
+
```

### Comparing `hsmm_mvpy-0.1.0b1/src/hsmm_mvpy.egg-info/PKG-INFO` & `hsmm_mvpy-0.1.0b3/src/hsmm_mvpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm-mvpy
-Version: 0.1.0b1
+Version: 0.1.0b3
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
         
@@ -42,34 +42,34 @@
 License-File: LICENSE.md
 
 HsMM MVpy
 ==========
 
 ![](plots/general_illustration.png)
 
-HsMM MVpy is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HMP) of neural time-series (e.g. EEG) based on the method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)), Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf)) and Weindel, van Maanen & Borst (in preparation).
+HsMM MVpy is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HMP) of neural time-series (e.g. EEG) based on the HsMM-MVPA method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030); see Borst & Anderson, [2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf), for an accessible introduction). HMP is described in Weindel, van Maanen & Borst (in preparation).
 
-As a summary of the method, an HMP model parses the reaction time into a number of successive stages determined based on patterns in a neural time-serie. Hence any reaction time can then be described by a number of stage  and their duration estimated using hsmm_mvpy. The important aspect of HMP is that it is a whole-brain analysis (or whole scalp analysis) that estimates the onset of stages on a single-trial basis. This by-trial estimations allows you then to further dig into any aspect you are interested in a signal:
+As a summary of the method, an HMP model parses the reaction time into a number of successive stages determined based on patterns in a neural time-serie. Hence any reaction time can then be described by a number of stages and their duration estimated using HMP. The important aspect of HMP is that it is a whole-brain analysis (or whole scalp analysis) that estimates the onset of stages on a single-trial basis. These by-trial estimates allow you then to further dig into any aspect you are interested in a signal:
 - Describing an experiment or a clinical sample in terms of stages detected in the EEG signal
 - Describing experimental effects based on a particular stage duration
 - Estimating the effect of trial-wise manipuations on the identified stages (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
 - Time-lock EEG signal to the onset of a given stage and perform classical ERPs or time-frequency analysis based on the onset of a new stage
 - And many more (e.g. evidence accumulation models on decision stage, classification based on the number of transition events in the signal,...)
 
 
 # Documentation
-**Important note** The current tutorials are based on the latest (unstable) version not yet default in _pip_, installing through github is therefore recommended or specify the beta version when installing through _pip_: ```pip install hsmm-mvpy==0.1.0b0```
+**Important note** The current tutorials are based on the latest (unstable) version not yet default in _pip_, installing through github is therefore recommended or specify the beta version when installing through _pip_: ```pip install hsmm-mvpy==0.1.0b1```
 
 The package is available through *pip*. 
 A recommended way of using the package is to use a conda environment (see [anaconda](https://www.anaconda.com/products/distribution>) for how to install conda):
 
     $ conda create -n hmp 
     $ conda activate hmp
     $ conda install pip #if not already installed
-    $ pip install hsmm-mvpy==0.1.0b0
+    $ pip install hsmm-mvpy==0.1.0b1
 
 Then import hsmm-mvpy in your favorite python IDE through:
 
 ```python
     import hsmm_mvpy as hmp
 ```
 
@@ -84,71 +84,81 @@
     $ pip install -e .
 
 
 ## To get started
 To get started with the code:
 - Check the demo below 
 - Inspect the tutorials in the tutorials repository
-    - Load EEG data (tutorial 1)
-    - Estimating a HMP with given number of stages (tutorial 2)
-    - Test for the number of stages that best explains the data (tutorial 3)
-    - Testing differences across conditions (tutorial 4)
-
-To further learn about the method be sure to check the paper by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) as well as the book chapter by Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf)). The following list also contains a non-exhaustive list of papers published using HMP:
+    - Tutorial 1: Loading EEG data 
+    - Tutorial 2: Estimating a HMP with given number of stages
+    - Tutorial 3: Test for the number of stages that best explains the data
+    - Tutorial 4: Testing differences across conditions
+
+To further learn about the oriignal HsMM-MVPA method be sure to check the paper by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) as well as the book chapter by Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HMP_MVPA_BorstAnderson_preprint.pdf)). The following list contains a non-exhaustive list of papers published using the original HsMM-MVPA method:
+- Anderson, J.R., Borst, J.P., Fincham, J.M., Ghuman, A.S., Tenison, C., & Zhang, Q. (2018). The Common Time Course of Memory Processes Revealed. Psychological Science 29(9), pp. 1463-1474. [link](https://doi.org/10.1177/0956797618774526)
+- Berberyan, H.S., Van Rijn, H., & Borst, J.P. (2021). Discovering the brain stages of lexical decision: Behavioral effects originate from a single neural decision process. Brain and Cognition 153: 105786. [link](https://www.sciencedirect.com/science/article/pii/S0278262621001068)
 - Berberyan, H. S., van Maanen, L., van Rijn, H., & Borst, J. (2021). EEG-based identification of evidence accumulation stages in decision-making. Journal of Cognitive Neuroscience, 33(3), 510-527. [link](https://doi.org/10.1162/jocn_a_01663)
 - Van Maanen, L., Portoles, O., & Borst, J. P. (2021). The discovery and interpretation of evidence accumulation stages. Computational brain & behavior, 4(4), 395-415. [link](https://link.springer.com/article/10.1007/s42113-021-00105-2)
 - Portoles, O., Blesa, M., van Vugt, M., Cao, M., & Borst, J. P. (2022). Thalamic bursts modulate cortical synchrony locally to switch between states of global functional connectivity in a cognitive task. PLoS computational biology, 18(3), e1009407. [link](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009407)
+- Portoles, O., Borst, J.P., & Van Vugt, M.K. (2018). Characterizing synchrony patterns across cognitive task stages of associative recognition memory. European Journal of Neuroscience 48, pp. 2759-2769. [link](http://onlinelibrary.wiley.com/doi/10.1111/ejn.13817/epdf)
+- Zhang, Q., van Vugt, M.K., Borst, J.P., & Anderson, J.R. (2018). Mapping Working Memory Retrieval in Space and in Time: A Combined Electroencephalography and Electrocorticography Approach. NeuroImage 174, pp. 472-484. [link](https://www.sciencedirect.com/science/article/pii/S1053811918302490)
+
+
 
 ## Demo on simulated data
 
 The following section will quickly walk you through an example usage in simulated data (using [MNE](https://mne.tools/dev/auto_examples/simulation/index.html)'s simulation functions and tutorials)
 
 First we load the libraries necessary for the demo on simulated data
 
 ### Importing libraries
 
+
+
 ```python
 ## Importing these packages is specific for this simulation case
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 from scipy.stats import gamma
 
 ## Importing HMP
 import hsmm_mvpy as hmp
 from hsmm_mvpy import simulations
 ```
 
+
 ### Simulating data
 
-In the following code block we simulate 50 trials from four known sources, this is not code you would need for your own analysis except if you want to simulate and test properties of HMP models. All these four sources are defined by a localization, an activation amplitude and a distribution (here a gamma with shape and scale parameters) for the onsets of the stages on each trial. The simulation functions are based on this [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
+In the following code block we simulate 50 trials from four known sources, this is not code you would need for your own analysis except if you'd want to simulate and test properties of HMP models. All four sources are defined by a location, an activation amplitude and a distribution in time (here a gamma with shape and scale parameters) for the onsets of the stages on each trial. The simulation functions are based on this [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
 
 _If you're running this for the first time a 1.65 G file will be downloaded in order to perform the simulation but this will be done only once (alternatively you can just download the corresponding simulation file and place it in the same folder from where you are running this notebook)_
 
 
 
 ```python
 cpus = 5 # For multiprocessing, usually a good idea to use multiple CPUs as long as you have enough RAM
 
 n_trials = 50 #Number of trials to simulate
 
 ##### Here we define the sources of the brain activity (event) for each trial
+# Because the last source determines the response, we will get four events during the trials, and therefore five stages
+n_sources = 5
 frequency = 10.#Frequency of the event defining its duration, half-sine of 10Hz = 50ms
-amplitude = .5e-6 #Amplitude of the event in Volt, defining signal to noise ratio
+amplitude = .5e-6 #Amplitude of the event in nAm, defining signal to noise ratio
 shape = 2 #shape of the gamma distribution
 means = np.array([60, 150, 200, 100, 80])/shape #Mean duration of the stages in ms
-names = ['bankssts-rh','posteriorcingulate-lh','parahippocampal-lh',\
-         'pericalcarine-rh','postcentral-lh']#Which source to activate at each stage (see atlas when calling simulations.available_sources())
+names = simulations.available_sources()[:n_sources]#Which source to activate at each stage (see atlas when calling simulations.available_sources())
 
 sources = []
 for source in zip(names, means):#One source = one frequency, one amplitude and a given by-trial variability distribution
     sources.append([source[0], frequency, amplitude, gamma(shape, scale=source[1])])
 
 # Function used to generate the data
-file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', location=25, overwrite=True)
+file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', location=25, overwrite=True) #location indicates the middle of the event after the stage start time in ms
 #Recovering sampling frequency of the simulated dataset
 sfreq = simulations.simulation_sfreq()
 #load electrode position, specific to the simulations
 positions = simulations.simulation_positions()
 ```
 
     Simulating ./dataset_README_raw.fif
@@ -172,27 +182,20 @@
 events = generating_events[(generating_events[:,2] == 1) | (generating_events[:,2] == resp_trigger)]#only retain stimulus and response triggers
 
 #Visualising the raw simulated EEG data
 import mne
 raw = mne.io.read_raw_fif(file[0], preload=False, verbose=False)
 raw.pick_types(eeg=True).plot(scalings=dict(eeg=1e-5), events=events, block=True);
 ```
-
-    Using qt as 2D backend.
-    Channels marked as bad:
-    none
-    
 ![png](README_files/README_7_1.png)
 
 
-
 ### Recovering number of stages as well as actual by-trial variation
 
-To compare the by-trial duration of bumps that we will estimate later on we first recover the actual number of stages or sources used in the simulation as well as the actual by-trial variation in the onset of the bumps. Again with a typical dataset you wouldn't need that part as you ignore the ground truth.
-
+To see how well HMP does at recovering by-trial stages below, here we get the ground truth from our simulation. Unfortunately, with an actual dataset you don’t have access to this, of course. 
 
 ```python
 %matplotlib inline
 number_of_sources = len(np.unique(generating_events[:,2])[1:])#one trigger = one source
 #Recover the actual time of the simulated events
 random_source_times = np.reshape(np.ediff1d(generating_events[:,0],to_begin=0)[generating_events[:,2] > 1], \
            (n_trials, number_of_sources))
@@ -207,37 +210,39 @@
 # Reading the data
 eeg_data = hmp.utils.read_mne_data(file[0], event_id=event_id, resp_id=resp_id, sfreq=sfreq, 
             events_provided=events, verbose=False)
 
 ```
 
     Processing participant ./dataset_README_raw.fif's continuous eeg
-    Reading 0 ... 153075  =      0.000 ...   254.864 secs...
+    Reading 0 ... 143915  =      0.000 ...   239.613 secs...
     50 trials were retained for participant ./dataset_README_raw.fif
 
 
-The package uses [xarray](https://docs.xarray.dev/en/stable/) named dimension matrices, allowing to directly manipulate the data using the name of the dimensions:
+HMP uses [xarray](https://docs.xarray.dev/en/stable/) named dimension matrices, allowing to directly manipulate the data using the name of the dimensions:
 
 
 ```python
 #example of usage of xarray
 print(eeg_data)
 eeg_data.sel(electrodes=['EEG 001','EEG 002','EEG 003'], samples=range(400))\
     .data.groupby('samples').mean(['participant','epochs']).plot.line(hue='electrodes');
 ```
 
     <xarray.Dataset>
-    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 711)
+    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 783)
     Coordinates:
       * epochs       (epochs) int64 0 1 2 3 4 5 6 7 8 ... 41 42 43 44 45 46 47 48 49
       * electrodes   (electrodes) <U7 'EEG 001' 'EEG 002' ... 'EEG 059' 'EEG 060'
-      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 704 705 706 707 708 709 710
+      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 776 777 778 779 780 781 782
       * participant  (participant) <U2 'S0'
     Data variables:
-        data         (participant, epochs, electrodes, samples) float64 1.96e-06 ...
+        data         (participant, epochs, electrodes, samples) float64 -3.747e-0...
+        event_name   (participant, epochs) object 'stimulus' ... 'stimulus'
+        rt           (participant, epochs) float64 0.5444 0.641 ... 0.8991 1.304
     Attributes:
         sfreq:    600.614990234375
         offset:   0
 
 
 
     
@@ -251,38 +256,37 @@
 Note that if the number of components to retain is not specified, the scree plot of the PCA is displayed and a prompt ask how many PCs should be retained (in this case we specify it as building the README does not allow for prompts)
 
 
 ```python
 hmp_data = hmp.utils.transform_data(eeg_data, apply_standard=False, n_comp=4)
 ```
 
-Once the data is in the expected format, we can initialize an HMP
+# HMP model
 
+Once the data is in the expected format, we can initialize an HMP object; note that no estimation is performed yet.
 
 ```python
 init = hmp.models.hmp(hmp_data, eeg_data, event_width=50, cpus=cpus)#Initialization of the model
 ```
 
-# HMP model
-
 We are looking for stages in the data (**Hidden Markov**) and assume that transitions between stages are signaled by a template in the data (**pattern analysis**). By default we use the same template as Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet'.apa.org/doi/10.1037/rev0000030)), a 10 Hz half-sine, resulting in a 50ms duration bump-like shape:
 
 
 
 ```python
 plt.plot(init.template,'x');
 ```
 
 
     
 ![png](README_files/README_18_0.png)
     
 
 
-This pattern is assumed to be present in multiple electrodes (**multivariate**). In order to find it, we apply a cross-correlation between that shape and the (normalized) EEG data:
+This pattern is assumed to be present across several electrodes (**multivariate**). In order to find it, we apply a cross-correlation between that shape and the (normalized) EEG data:
 
 
 
 ```python
 epoch = 0 #illustrating the first trial
 hmp_data.unstack().sel(component=[0,1,2], epochs=epoch).squeeze().plot.line(hue='component');
 plt.vlines(random_source_times[epoch,:-1].cumsum()-1, -3, 3, 'k')#overlaying the simulated stage transition times
@@ -291,69 +295,69 @@
 
     
 ![png](README_files/README_20_1.png)
     
 
 
 
-The by-trial onset of this transition event is assumed to be captured by a probability distribution (**semi-Markov**), e.g. in this application a gamma with a shape of 2:
+The by-trial onset of this transition pattern event is assumed to be captured by a probability distribution (**semi-Markov**), e.g. in this application a gamma with a shape of 2:
 
 
 ```python
 T = 350
 plt.plot(np.linspace(0,T,1001),gamma.pdf(np.linspace(0,T,1001), 2, scale=50)) 
 plt.xlabel('t');
 ```
 
 
     
 ![png](README_files/README_22_0.png)
     
 
 
-And this is then the full explanation of an HMP model: Looking for a transition event across several electrodes and trials that signals a transition to the next stage and which onset is expected to follow a probability distribution (in this case a gamma).
+And this is then the full explanation of an HMP model: Looking for a transition event across several electrodes and trials that signals a transition to the next stage and which onset is expected to follow a probability distribution (by default a gamma distribution).
 
 # Estimating an HMP model
 
-We can directly fit an HMP model without giving any info on the number of stages (see tutorial 2 for the explanation of the following cell)
+We can directly fit an HMP model without giving any info on the number of stages (see tutorial 2 for a detailed explanation of the following cell)
 
 
 
 ```python
 estimates = init.fit(step=20, verbose=True)
 ```
 
 
+
+    Transition event 1 found around sample 37
     Transition event 2 found around sample 137
-    Transition event 3 found around sample 258
-    Transition event 4 found around sample 330
+    Transition event 3 found around sample 277
+    Transition event 4 found around sample 348
     Estimating 4 events model
     Parameters estimated for 4 events model
 
 
 ### Visualizing results of the fit
 
-In the previous cell we initiated an HMP model looking for 50ms bumps in the EEG signal and parsing the EEG data into a signal with 4 Transition events and 5 gamma distributed stages with a fixed shape of 2 and a scale estimated by stage. We can now inspect the results of the fit.
+In the previous cell we initiated an HMP model looking for default 50ms bumps – the transition events – in the EEG signal. The method discovered four events, and therefore five gamma-distributed stages with a fixed shape of 2 and an estimated scale. We can now inspect the results of the fit.
 
 We can directly take a look to the topologies and latencies of the events by calling ```hmp.visu.plot_topo_timecourse```
 
 
-We can directly take a look to the topologies and latencies of the events by calling ```hmp.visu.plot_topo_timecourse```
-
 
 ```python
 hmp.visu.plot_topo_timecourse(eeg_data, estimates, #Data and estimations 
                                positions, init,#position of the electrodes and initialized model
                                magnify=1, sensors=False, time_step=1000/init.sfreq,#Display control parameters
                                times_to_display = np.mean(init.ends - init.starts))#plot reaction times
 ```
 
 
     
-![png](README_files/README_27_0.png)
+![png](README_files/README_26_0.png)
     
 
 
 This shows us the electrode activity on the scalp as well as the average time of occurence of the events based on the stage distributions.
 
 As we are estimating the event onsets on a by-trial basis we can look at the by-trial variation in stage duration.
 
@@ -362,15 +366,15 @@
 event_times_estimates = init.compute_times(init, estimates, mean=False, add_rt=True).dropna('event')#computing predicted event times
 ax = hmp.visu.plot_latencies_average(event_times_estimates, init.event_width_samples, 1, errs='ci', times_to_display = np.mean(init.ends - init.starts))
 ax.set_ylabel('your label here');
 ```
 
 
     
-![png](README_files/README_29_0.png)
+![png](README_files/README_28_0.png)
     
 
 
 For the same reason we can also inspect the probability distribution of event onsets:
 
 
 
@@ -384,21 +388,21 @@
 
     <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
-![png](README_files/README_31_1.png)
+![png](README_files/README_30_1.png)
     
 
 
 
     
-![png](README_files/README_31_2.png)
+![png](README_files/README_30_2.png)
     
 
 
 As HMP estimated stage onset per trial we can also look at the predicted stage onsets for a given trial.
 
 
 ```python
@@ -411,23 +415,23 @@
 
     <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
-![png](README_files/README_33_1.png)
+![png](README_files/README_32_1.png)
     
 
 
 This then shows the likeliest stage onset location in time for the first trial!
 
 ## Comparing with ground truth
 
-As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HMP-MVpy. As in the beginning, this code is specific to the case where you simulate data.
+As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HMP. Perhaps to state the obvious, this code is specific to the case where you simulate data.
 
 
 ```python
 colors = sns.color_palette(None, number_of_sources)
 plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.prod(axis=1), color=colors,s=50)
 plt.plot([np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],
          [np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],'--');
@@ -436,34 +440,34 @@
 plt.ylabel('Estimated stage duration')
 plt.show()
 
 ```
 
 
     
-![png](README_files/README_35_0.png)
+![png](README_files/README_34_0.png)
     
 
 
-Or also overlay actual bumps onset with predicted one
+We can also overlay actual bumps onset with predicted one
 
 
 
 ```python
 hmp.visu.plot_topo_timecourse(eeg_data, estimates, positions, init, magnify=1, sensors=False, figsize=(13,1), title='Actual vs estimated event onsets',
         times_to_display = np.mean(np.cumsum(random_source_times,axis=1),axis=0))
 ```
 
 
     
-![png](README_files/README_37_0.png)
+![png](README_files/README_36_0.png)
     
 
 
-We see that the HSMM-MVpy package recovers the exact average location of the bumps defined in the simulated data.
+We see that the HMP recovered the exact average location of the bumps defined in the simulated data.
 
 We can further test how well the package did by comparing the generated single trial onsets with those estimated from the HMP model
 
 
 ```python
 fig, ax= plt.subplots(number_of_sources,1, figsize=(5,3.5*number_of_sources), dpi=300)
 ax[0].set_title('Comparing true vs estimated single trial stage durations')
@@ -475,15 +479,15 @@
     ax[i].set_ylabel(f'Estimated by-trial stage duration for stage {i+1}')
     ax[i].set_xlabel(f'Simulated by-trial stage duration for stage {i+1}')
     i+= 1
 ```
 
 
     
-![png](README_files/README_39_0.png)
+![png](README_files/README_38_0.png)
     
 
 
 We see that every stage gets nicely recovered even on a by-trial basis!
 
 # Beyond summary statistics for EEG analysis
 
@@ -510,19 +514,19 @@
 plt.xlim(0,500)
 plt.ylim(-3e-6,3e-6);
 
 ```
 
 
     
-![png](README_files/README_41_0.png)
+![png](README_files/README_40_0.png)
     
 
 
-Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is very close to traditional ERPs with very clear signal in the beginning of a trial (as events are more in phase) and summed and blurried in later stages of the reaction times (as event are off phase).
+Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is similar to traditional ERPs that have a very clear signal in the beginning of a trial (as events are more in phase) and summed and blurred further away from the stimulus (as events are off phase).
 
 Now things can get better if we first parse, by-trial, the signal into the different stages based on the HMP estimates:
 
 
 ```python
 BRP_times = init.compute_times(init, estimates.dropna('event'), fill_value=0, add_rt=True)
 
@@ -539,20 +543,20 @@
     df = pd.DataFrame(BRP).melt(var_name='Time')
     sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkblue') 
     plt.xlim(0,100)
 ```
 
 
     
-![png](README_files/README_43_0.png)
+![png](README_files/README_42_0.png)
     
 
 
 
-In this case we clearly see at each stage the half-sin (of 50ms hence ~ 30 samples for the sampling frequency used) we simulated in the first step and the preceding period of silence (hence the first stage doesn't contain such a half-sin). Note that the end of the stages tend to be noisier because less trial are defining the average signal (also why the confidence interval grows).
+In this case we clearly see at each stage the half-sine (of 50ms hence ~ 30 samples for the sampling frequency used) we simulated in the first step and the preceding period of silence (hence the first stage doesn't contain such a half-sine). Note that the end of the stages tend to be noisier because fewer trials are defining the average signal.
 
 
 ### Follow-up
 
 For examples on how to use the package when the number of transition events/stages is unkown, or to compare stage durations across conditions see the tutorial notebooks:
 - Load EEG data (tutorial 1)
 - Estimating a given number of events (tutorial 2)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

