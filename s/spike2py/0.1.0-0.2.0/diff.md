# Comparing `tmp/spike2py-0.1.0.tar.gz` & `tmp/spike2py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spike2py-0.1.0.tar", last modified: Sun Sep 13 13:02:00 2020, max compression
+gzip compressed data, was "spike2py-0.2.0.tar", last modified: Mon Jun 19 05:34:37 2023, max compression
```

## Comparing `spike2py-0.1.0.tar` & `spike2py-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,31 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-09-13 13:02:00.253881 spike2py-0.1.0/
--rw-rw-r--   0 martin    (1000) martin    (1000)     3494 2020-09-13 13:02:00.253881 spike2py-0.1.0/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     2595 2020-09-13 12:53:05.000000 spike2py-0.1.0/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2020-09-13 13:02:00.253881 spike2py-0.1.0/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)      989 2020-09-13 13:01:42.000000 spike2py-0.1.0/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-09-13 13:02:00.253881 spike2py-0.1.0/spike2py/
--rw-rw-r--   0 martin    (1000) martin    (1000)      166 2020-09-13 13:01:35.000000 spike2py-0.1.0/spike2py/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     7329 2020-09-13 11:28:32.000000 spike2py-0.1.0/spike2py/channels.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1264 2020-09-13 11:28:32.000000 spike2py-0.1.0/spike2py/demo.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     7504 2020-09-13 11:28:32.000000 spike2py-0.1.0/spike2py/plot.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     7263 2020-09-13 11:28:32.000000 spike2py-0.1.0/spike2py/read.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     6980 2020-08-23 13:22:48.000000 spike2py-0.1.0/spike2py/sig_proc.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     6056 2020-09-13 11:28:32.000000 spike2py-0.1.0/spike2py/trial.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      865 2020-09-13 11:28:32.000000 spike2py-0.1.0/spike2py/types.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-09-13 13:02:00.253881 spike2py-0.1.0/spike2py.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     3494 2020-09-13 13:02:00.000000 spike2py-0.1.0/spike2py.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      327 2020-09-13 13:02:00.000000 spike2py-0.1.0/spike2py.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2020-09-13 13:02:00.000000 spike2py-0.1.0/spike2py.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       45 2020-09-13 13:02:00.000000 spike2py-0.1.0/spike2py.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        9 2020-09-13 13:02:00.000000 spike2py-0.1.0/spike2py.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 05:34:37.577507 spike2py-0.2.0/
+-rw-r--r--   0 martin    (1000) martin    (1000)    35149 2023-04-08 08:32:31.000000 spike2py-0.2.0/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3069 2023-06-19 05:34:37.573507 spike2py-0.2.0/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)     2595 2023-04-08 08:32:31.000000 spike2py-0.2.0/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-06-19 05:34:37.577507 spike2py-0.2.0/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)      945 2023-06-19 05:34:18.000000 spike2py-0.2.0/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 05:34:37.573507 spike2py-0.2.0/spike2py/
+-rw-r--r--   0 martin    (1000) martin    (1000)      166 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     7329 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/channels.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     1264 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/demo.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     7464 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/plot.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     7263 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/read.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     1569 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/reflex.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     6980 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/sig_proc.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      606 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/temp_script.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     6056 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/trial.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      865 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/types.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 05:34:37.573507 spike2py-0.2.0/spike2py.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)     3069 2023-06-19 05:34:37.000000 spike2py-0.2.0/spike2py.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      532 2023-06-19 05:34:37.000000 spike2py-0.2.0/spike2py.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-19 05:34:37.000000 spike2py-0.2.0/spike2py.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       23 2023-06-19 05:34:37.000000 spike2py-0.2.0/spike2py.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        9 2023-06-19 05:34:37.000000 spike2py-0.2.0/spike2py.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 05:34:37.573507 spike2py-0.2.0/tests/
+-rw-r--r--   0 martin    (1000) martin    (1000)     3305 2023-04-08 08:32:31.000000 spike2py-0.2.0/tests/test_channels.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      858 2023-04-08 08:32:31.000000 spike2py-0.2.0/tests/test_demo.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     1725 2023-04-08 08:32:31.000000 spike2py-0.2.0/tests/test_figures.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      773 2023-04-08 08:32:31.000000 spike2py-0.2.0/tests/test_plot.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     3350 2023-04-08 08:32:31.000000 spike2py-0.2.0/tests/test_read.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     9162 2023-04-08 08:32:31.000000 spike2py-0.2.0/tests/test_signal_processing.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     1844 2023-04-08 08:32:31.000000 spike2py-0.2.0/tests/test_trial.py
```

### Comparing `spike2py-0.1.0/PKG-INFO` & `spike2py-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 Metadata-Version: 2.1
 Name: spike2py
-Version: 0.1.0
+Version: 0.2.0
 Summary: Import, parse and process data collected with Spike2
 Home-page: https://github.com/MartinHeroux/spike2py
 Author: Martin Héroux
 Author-email: heroux.martin@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
-Description: [![spike2py](https://raw.githubusercontent.com/MartinHeroux/spike2py/master/docs/source/img/spike2py_icon_600x300.png)](https://github.com/MartinHeroux/spike2py)
-        
-        
-        [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        ![coverage](https://img.shields.io/badge/coverage-96%25-yellowgreen)
-            [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md)
-        [![Documentation Status](https://readthedocs.org/projects/spike2py/badge/?version=latest)](https://spike2py.readthedocs.io/en/latest/?badge=latest)
-        
-        **spike2py** provides a simple interface to analyse and visualise data collected using [Spike2](http://ced.co.uk/products/spkovin) software and [Cambridge Electronics Design (CED)](http://ced.co.uk/) data acquisition boards. With it you can easily plot individual channels or all channels from a given trial. In addition, you can easily apply various signal processing methods to your `waveform` data. Finally, you can easily save your data at any point, allowing you to re-open and continue your work from where they left off.
-        
-        To demonstrate, the following snippet of code shows you how to:
-        
-        1. Read a file
-        2. Plot the electromyography (EMG) signal from one of the channels
-        2. Remove the mean of the first 500 samples and rectify EMG signal, and plot the result
-        
-        ```python
-        >>> from spike2py.trial import TrialInfo, Trial
-        >>> trial_info = TrialInfo(file="sample.mat")
-        >>> sample = Trial(trial_info)
-        >>> sample.muscle_emg.plot()
-        >>> sample.muscle_emg.remove_mean(first_n_samples=500).rect().plot()
-        ```
-        
-        [![emg_raw](https://raw.githubusercontent.com/MartinHeroux/spike2py/master/docs/source/img/EMG_400x132.png)](https://github.com/MartinHeroux/spike2py)
-        
-        ## Documentation
-        
-        Introductory tutorials, how-to's and other useful documentation are available on [Read the Docs](https://spike2py.readthedocs.io/en/latest/index.html)
-        
-        ## Installing
-        
-        **spike2py** is available on PyPI:
-        
-        ```console
-        $ python -m pip install spike2py
-        ```
-        
-        **spike2py** officially supports Python 3.8+.
-        
-        ## Contributing
-        
-        Like this project? Want to help? We would love to have your contribution! Please see [CONTRIBUTING](CONTRIBUTING.md) to get started.
-        
-        ## Code of conduct
-        
-        This project adheres to the Contributor Covenant code of conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to [heroux.martin@gmail.com](heroux.martin@gmail.com).
-        
-        ## License
-        
-        [GPLv3](./LICENSE)
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![spike2py](https://raw.githubusercontent.com/MartinHeroux/spike2py/master/docs/source/img/spike2py_icon_600x300.png)](https://github.com/MartinHeroux/spike2py)
+
+
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![coverage](https://img.shields.io/badge/coverage-96%25-yellowgreen)
+    [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md)
+[![Documentation Status](https://readthedocs.org/projects/spike2py/badge/?version=latest)](https://spike2py.readthedocs.io/en/latest/?badge=latest)
+
+**spike2py** provides a simple interface to analyse and visualise data collected using [Spike2](http://ced.co.uk/products/spkovin) software and [Cambridge Electronics Design (CED)](http://ced.co.uk/) data acquisition boards. With it you can easily plot individual channels or all channels from a given trial. In addition, you can easily apply various signal processing methods to your `waveform` data. Finally, you can easily save your data at any point, allowing you to re-open and continue your work from where they left off.
+
+To demonstrate, the following snippet of code shows you how to:
+
+1. Read a file
+2. Plot the electromyography (EMG) signal from one of the channels
+2. Remove the mean of the first 500 samples and rectify EMG signal, and plot the result
+
+```python
+>>> from spike2py.trial import TrialInfo, Trial
+>>> trial_info = TrialInfo(file="sample.mat")
+>>> sample = Trial(trial_info)
+>>> sample.muscle_emg.plot()
+>>> sample.muscle_emg.remove_mean(first_n_samples=500).rect().plot()
+```
+
+[![emg_raw](https://raw.githubusercontent.com/MartinHeroux/spike2py/master/docs/source/img/EMG_400x132.png)](https://github.com/MartinHeroux/spike2py)
+
+## Documentation
+
+Introductory tutorials, how-to's and other useful documentation are available on [Read the Docs](https://spike2py.readthedocs.io/en/latest/index.html)
+
+## Installing
+
+**spike2py** is available on PyPI:
+
+```console
+$ python -m pip install spike2py
+```
+
+**spike2py** officially supports Python 3.8+.
+
+## Contributing
+
+Like this project? Want to help? We would love to have your contribution! Please see [CONTRIBUTING](CONTRIBUTING.md) to get started.
+
+## Code of conduct
+
+This project adheres to the Contributor Covenant code of conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to [heroux.martin@gmail.com](heroux.martin@gmail.com).
+
+## License
+
+[GPLv3](./LICENSE)
```

### Comparing `spike2py-0.1.0/README.md` & `spike2py-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `spike2py-0.1.0/setup.py` & `spike2py-0.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="spike2py",
-    version="0.1.0",
+    version="0.2.0",
     description="Import, parse and process data collected with Spike2",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/MartinHeroux/spike2py",
     author="Martin Héroux",
     author_email="heroux.martin@gmail.com",
     license="GNU General Public License v3 or later (GPLv3+)",
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3.8",
     ],
     packages=["spike2py"],
     include_package_data=False,
-    install_requires=["numpy>=1.19.1", "scipy>=1.5.2", "matplotlib>=3.3.1"],
-    tests_require=["pytest>=6.0.1", "pytest-cov>=2.10.1", "pytest-mpl>= 0.11"]
+    install_requires=["numpy", "scipy", "matplotlib"],
+    tests_require=["pytest", "pytest-cov", "pytest-mpl"]
 )
```

### Comparing `spike2py-0.1.0/spike2py/channels.py` & `spike2py-0.2.0/spike2py/channels.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.1.0/spike2py/demo.py` & `spike2py-0.2.0/spike2py/demo.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.1.0/spike2py/plot.py` & `spike2py-0.2.0/spike2py/plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from typing import Literal, Tuple
 
 import numpy as np
 import matplotlib
-from matplotlib.axes._subplots import Subplot
-
 import matplotlib.pyplot as plt
 
 
 from spike2py import channels, trial
 from spike2py.types import all_channels, ticksline_channels
 
 LINE_WIDTH = 2
@@ -73,15 +71,15 @@
 
 def _get_color(index: int) -> str:
     return COLORS[index % len(COLORS)]
 
 
 def _plot_waveform(
     waveform: "channels.Waveform",
-    ax: Subplot,
+    ax: plt.Axes,
     color: str = _get_color(0),
 ) -> None:
     ax.plot(waveform.times, waveform.values, label=waveform.info.name, color=color)
     ax.set_xlim(waveform.times[0], waveform.times[-1])
     units = waveform.info.units if waveform.info.units is True else "a.u."
     ax.set_ylabel(f"amplitude ({units})")
     ax.legend(loc=LEGEND_LOC)
@@ -126,15 +124,15 @@
         self.offset = y_offset
 
         self.ch_type = repr(ticks_line_channel).split()[0]
         self.line_start_end = (self.ch.times[0], self.ch.times[-1])
         self.line_y_vals = (0.5 + y_offset, 0.5 + y_offset)
         self.tick_y_vals = (0.2 + y_offset, 0.8 + y_offset)
 
-    def plot(self, ax: Subplot):
+    def plot(self, ax: plt.Axes):
         if isinstance(ax, np.ndarray):
             ax1 = ax[0]
             ax2 = ax[1]
         else:
             ax1 = ax
             ax2 = None
 
@@ -144,40 +142,40 @@
         if self.ch_type == "Keyboard":
             self._plot_codes(ax1)
         if (self.ch_type == "Wavemark") and ax2:
             self._plot_action_potentials(ax2)
 
         plt.tight_layout()
 
-    def _plot_ticks_line(self, ax1: Subplot):
+    def _plot_ticks_line(self, ax1: plt.Axes):
         for time in self.ch.times:
             ax1.plot(
                 (time, time), self.tick_y_vals, linewidth=LINE_WIDTH, color=self.color
             )
         ax1.plot(
             self.line_start_end,
             self.line_y_vals,
             linewidth=LINE_WIDTH,
             label=self.ch.info.name,
             color=self.color,
         )
 
-    def _plot_codes(self, ax1: Subplot):
+    def _plot_codes(self, ax1: plt.Axes):
         for time, code in zip(self.ch.times, self.ch.codes):
             ax1.text(
                 time, self.tick_y_vals[1] + 0.2, code, color=self.color, fontsize=10
             )
 
-    def _plot_action_potentials(self, ax2: Subplot):
+    def _plot_action_potentials(self, ax2: plt.Axes):
         for action_potential in self.ch.action_potentials:
             ax2.plot(action_potential, color=self.color, alpha=0.5)
         ax2.get_yaxis().set_visible(False)
         ax2.get_xaxis().set_visible(False)
 
-    def _finalise_plot(self, ax1: Subplot):
+    def _finalise_plot(self, ax1: plt.Axes):
         ax1.legend(loc=LEGEND_LOC)
         ax1.set_xlabel("time (s)")
         ax1.get_yaxis().set_visible(False)
         ax1.grid()
 
 
 def plot_trial(spike2py_trial: "trial.Trial", save: Literal[True, False]) -> None:
@@ -219,15 +217,15 @@
         elif channel_type == "waveform":
             fig_height += 2
             n_subplots += 1
     fig_height = min(fig_height, MAX_TRIAL_FIG_HEIGHT)
     return fig_height, n_subplots
 
 
-def _plot_trial(spike2py_trial: "trial.Trial", ax: Subplot):
+def _plot_trial(spike2py_trial: "trial.Trial", ax: plt.Axes):
     waveform_counter = 1
     other_ch_counter = 0
     n_subplots = len(ax)
     for channel, channel_type in spike2py_trial.channels:
         current_channel = spike2py_trial.__getattribute__(channel)
         if channel_type == "waveform":
             _plot_waveform(
```

### Comparing `spike2py-0.1.0/spike2py/read.py` & `spike2py-0.2.0/spike2py/read.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.1.0/spike2py/sig_proc.py` & `spike2py-0.2.0/spike2py/sig_proc.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.1.0/spike2py/trial.py` & `spike2py-0.2.0/spike2py/trial.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.1.0/spike2py/types.py` & `spike2py-0.2.0/spike2py/types.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.1.0/spike2py.egg-info/PKG-INFO` & `spike2py-0.2.0/spike2py.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 Metadata-Version: 2.1
 Name: spike2py
-Version: 0.1.0
+Version: 0.2.0
 Summary: Import, parse and process data collected with Spike2
 Home-page: https://github.com/MartinHeroux/spike2py
 Author: Martin Héroux
 Author-email: heroux.martin@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
-Description: [![spike2py](https://raw.githubusercontent.com/MartinHeroux/spike2py/master/docs/source/img/spike2py_icon_600x300.png)](https://github.com/MartinHeroux/spike2py)
-        
-        
-        [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        ![coverage](https://img.shields.io/badge/coverage-96%25-yellowgreen)
-            [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md)
-        [![Documentation Status](https://readthedocs.org/projects/spike2py/badge/?version=latest)](https://spike2py.readthedocs.io/en/latest/?badge=latest)
-        
-        **spike2py** provides a simple interface to analyse and visualise data collected using [Spike2](http://ced.co.uk/products/spkovin) software and [Cambridge Electronics Design (CED)](http://ced.co.uk/) data acquisition boards. With it you can easily plot individual channels or all channels from a given trial. In addition, you can easily apply various signal processing methods to your `waveform` data. Finally, you can easily save your data at any point, allowing you to re-open and continue your work from where they left off.
-        
-        To demonstrate, the following snippet of code shows you how to:
-        
-        1. Read a file
-        2. Plot the electromyography (EMG) signal from one of the channels
-        2. Remove the mean of the first 500 samples and rectify EMG signal, and plot the result
-        
-        ```python
-        >>> from spike2py.trial import TrialInfo, Trial
-        >>> trial_info = TrialInfo(file="sample.mat")
-        >>> sample = Trial(trial_info)
-        >>> sample.muscle_emg.plot()
-        >>> sample.muscle_emg.remove_mean(first_n_samples=500).rect().plot()
-        ```
-        
-        [![emg_raw](https://raw.githubusercontent.com/MartinHeroux/spike2py/master/docs/source/img/EMG_400x132.png)](https://github.com/MartinHeroux/spike2py)
-        
-        ## Documentation
-        
-        Introductory tutorials, how-to's and other useful documentation are available on [Read the Docs](https://spike2py.readthedocs.io/en/latest/index.html)
-        
-        ## Installing
-        
-        **spike2py** is available on PyPI:
-        
-        ```console
-        $ python -m pip install spike2py
-        ```
-        
-        **spike2py** officially supports Python 3.8+.
-        
-        ## Contributing
-        
-        Like this project? Want to help? We would love to have your contribution! Please see [CONTRIBUTING](CONTRIBUTING.md) to get started.
-        
-        ## Code of conduct
-        
-        This project adheres to the Contributor Covenant code of conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to [heroux.martin@gmail.com](heroux.martin@gmail.com).
-        
-        ## License
-        
-        [GPLv3](./LICENSE)
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![spike2py](https://raw.githubusercontent.com/MartinHeroux/spike2py/master/docs/source/img/spike2py_icon_600x300.png)](https://github.com/MartinHeroux/spike2py)
+
+
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![coverage](https://img.shields.io/badge/coverage-96%25-yellowgreen)
+    [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md)
+[![Documentation Status](https://readthedocs.org/projects/spike2py/badge/?version=latest)](https://spike2py.readthedocs.io/en/latest/?badge=latest)
+
+**spike2py** provides a simple interface to analyse and visualise data collected using [Spike2](http://ced.co.uk/products/spkovin) software and [Cambridge Electronics Design (CED)](http://ced.co.uk/) data acquisition boards. With it you can easily plot individual channels or all channels from a given trial. In addition, you can easily apply various signal processing methods to your `waveform` data. Finally, you can easily save your data at any point, allowing you to re-open and continue your work from where they left off.
+
+To demonstrate, the following snippet of code shows you how to:
+
+1. Read a file
+2. Plot the electromyography (EMG) signal from one of the channels
+2. Remove the mean of the first 500 samples and rectify EMG signal, and plot the result
+
+```python
+>>> from spike2py.trial import TrialInfo, Trial
+>>> trial_info = TrialInfo(file="sample.mat")
+>>> sample = Trial(trial_info)
+>>> sample.muscle_emg.plot()
+>>> sample.muscle_emg.remove_mean(first_n_samples=500).rect().plot()
+```
+
+[![emg_raw](https://raw.githubusercontent.com/MartinHeroux/spike2py/master/docs/source/img/EMG_400x132.png)](https://github.com/MartinHeroux/spike2py)
+
+## Documentation
+
+Introductory tutorials, how-to's and other useful documentation are available on [Read the Docs](https://spike2py.readthedocs.io/en/latest/index.html)
+
+## Installing
+
+**spike2py** is available on PyPI:
+
+```console
+$ python -m pip install spike2py
+```
+
+**spike2py** officially supports Python 3.8+.
+
+## Contributing
+
+Like this project? Want to help? We would love to have your contribution! Please see [CONTRIBUTING](CONTRIBUTING.md) to get started.
+
+## Code of conduct
+
+This project adheres to the Contributor Covenant code of conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to [heroux.martin@gmail.com](heroux.martin@gmail.com).
+
+## License
+
+[GPLv3](./LICENSE)
```

