# Comparing `tmp/solo_epd_loader-0.2.4.tar.gz` & `tmp/solo_epd_loader-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-j6ozfh3i/solo_epd_loader-0.2.4.tar", last modified: Mon Jun 19 07:28:16 2023, max compression
+gzip compressed data, was "solo_epd_loader-0.2.5.tar", last modified: Mon Jun 19 08:26:15 2023, max compression
```

## Comparing `solo_epd_loader-0.2.4.tar` & `solo_epd_loader-0.2.5.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 07:28:16.060250 solo_epd_loader-0.2.4/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.4/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.4/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    17529 2023-06-19 07:28:16.060250 solo_epd_loader-0.2.4/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16581 2023-05-23 14:42:04.000000 solo_epd_loader-0.2.4/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.4/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 07:28:16.052250 solo_epd_loader-0.2.4/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.4/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.4/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.4/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.4/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 07:28:16.056250 solo_epd_loader-0.2.4/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.4/examples/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.4/examples/ws2021_fig_2d.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.4/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.4/gh2021_fig_2a.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 07:28:16.056250 solo_epd_loader-0.2.4/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.4/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.4/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.4/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2306 2023-06-19 07:28:16.060250 solo_epd_loader-0.2.4/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.4/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 07:28:16.056250 solo_epd_loader-0.2.4/solo_epd_loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    37798 2022-11-16 14:15:40.000000 solo_epd_loader-0.2.4/solo_epd_loader/__init__ (STEP UPDATE).py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    54378 2023-06-19 07:20:29.000000 solo_epd_loader-0.2.4/solo_epd_loader/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 07:28:16.060250 solo_epd_loader-0.2.4/solo_epd_loader/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.4/solo_epd_loader/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-06-19 07:28:15.000000 solo_epd_loader-0.2.4/solo_epd_loader/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 07:28:16.056250 solo_epd_loader-0.2.4/solo_epd_loader.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    17529 2023-06-19 07:28:15.000000 solo_epd_loader-0.2.4/solo_epd_loader.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      653 2023-06-19 07:28:16.000000 solo_epd_loader-0.2.4/solo_epd_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-06-19 07:28:15.000000 solo_epd_loader-0.2.4/solo_epd_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.4/solo_epd_loader.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      192 2023-06-19 07:28:15.000000 solo_epd_loader-0.2.4/solo_epd_loader.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-06-19 07:28:15.000000 solo_epd_loader-0.2.4/solo_epd_loader.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.4/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 08:26:15.181496 solo_epd_loader-0.2.5/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.5/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.5/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-19 08:26:15.181496 solo_epd_loader-0.2.5/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15847 2023-06-19 08:20:58.000000 solo_epd_loader-0.2.5/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.5/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 08:26:15.173496 solo_epd_loader-0.2.5/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.5/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.5/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.5/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.5/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 08:26:15.177496 solo_epd_loader-0.2.5/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.5/examples/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.5/examples/ws2021_fig_2d.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.5/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.5/gh2021_fig_2a.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 08:26:15.177496 solo_epd_loader-0.2.5/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.5/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.5/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.5/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2306 2023-06-19 08:26:15.185496 solo_epd_loader-0.2.5/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.5/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 08:26:15.177496 solo_epd_loader-0.2.5/solo_epd_loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    54423 2023-06-19 08:10:34.000000 solo_epd_loader-0.2.5/solo_epd_loader/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 08:26:15.181496 solo_epd_loader-0.2.5/solo_epd_loader/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.5/solo_epd_loader/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-06-19 08:26:15.000000 solo_epd_loader-0.2.5/solo_epd_loader/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 08:26:15.181496 solo_epd_loader-0.2.5/solo_epd_loader.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-19 08:26:15.000000 solo_epd_loader-0.2.5/solo_epd_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      611 2023-06-19 08:26:15.000000 solo_epd_loader-0.2.5/solo_epd_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-06-19 08:26:15.000000 solo_epd_loader-0.2.5/solo_epd_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.5/solo_epd_loader.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      192 2023-06-19 08:26:15.000000 solo_epd_loader-0.2.5/solo_epd_loader.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-06-19 08:26:15.000000 solo_epd_loader-0.2.5/solo_epd_loader.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.5/tox.ini
```

### Comparing `solo_epd_loader-0.2.4/LICENSE.rst` & `solo_epd_loader-0.2.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.4/PKG-INFO` & `solo_epd_loader-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo_epd_loader
-Version: 0.2.4
+Version: 0.2.5
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -80,30 +80,29 @@
 containing information on the energy channels.
 
 .. code:: python
 
    from solo_epd_loader import epd_load
 
    df_1, df_2, energies = epd_load(sensor, startdate, enddate=None, level='l2', viewing=None, path=None, 
-                                   autodownload=False, only_averages=False, contamination_threshold=2)
+                                   autodownload=False, only_averages=False)
 
 Input
 ~~~~~
 
 -  ``sensor``: ``'ept'``, ``'het'``, or ``'step'`` (string)
 -  ``startdate``, ``enddate``: Datetime object (e.g., ``dt.date(2021,12,31)`` or ``dt.datetime(2021,4,15)``) or integer of the form yyyymmdd with empty positions filled with zeros, e.g. ``20210415`` (if no ``enddate`` is provided, ``enddate = startdate`` will be used)
 -  ``level``: ``'l2'`` or ``'ll'`` (string); defines level of data product: level 2 (``'l2'``) or low-latency (``'ll'``). By default ``'l2'``.
 -  ``viewing``: ``'sun'``, ``'asun'``, ``'north'``, ``'south'`` (string) or ``None``; not
    needed for ``sensor = 'step'``
 -  ``path``: directory in which Solar Orbiter data is/should be
    organized; e.g. ``'/home/userxyz/solo/data/'`` (string). See `Data folder structure`_ for more details.
 -  ``autodownload``: if ``True``, will try to download missing data files
    from SOAR (bolean)
 - ``only_averages``: If ``True``, will for STEP only return the averaged fluxes, and not the data of each of the 15 Pixels. This will reduce the memory consumption. By default ``False``.
-- ``contamination_threshold``: If integer, mask electron data that probably is contaminated (i.e., set it to ``nan``) using an integer contamination threshold following the equation ``Integral_Flux - Magnet_Flux > contamination_threshold * Integral_Uncertainty``. If ``False``, don't alter the data at all. Only implemented for new STEP data (after Oct 2021) so far. By default ``2``.
 
 Return
 ~~~~~~
 
 -  For ``sensor`` = ``'ept'`` or ``'het'``:
 
    1. Pandas dataframe with proton fluxes and errors (for EPT also alpha
@@ -127,20 +126,14 @@
       -  Value of energy bin width in MeV
 
 SupraThermal Electron Proton (STEP) sensor electron measurements
 ----------------------------------------------------------------
 
 Please note that the STEP electron measurements are not directly provided in the publically released data, but need to be calculated from them. This process is not straightforward, and the resulting data is prone to uncertainties (like contamination). **Thus it should only be used scientifically with caution! Please refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
 
-The ``contamination_threshold`` option can be used when calling ``epd_load()`` to mask STEP electron data that probably is contaminated (i.e., it is set to nan) following the equation:
-
-   Integral_Flux - Magnet_Flux > contamination_threshold * Integral_Uncertainty
-
-The default setting is ``contamination_threshold=2``.
-
 
 Data folder structure
 ---------------------
 
 The ``path`` variable provided to the module should be the base
 directory where the corresponding cdf data files should be placed in
 subdirectories. First subfolder defines the data product ``level``
```

### Comparing `solo_epd_loader-0.2.4/README.rst` & `solo_epd_loader-0.2.5/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -55,30 +55,29 @@
 containing information on the energy channels.
 
 .. code:: python
 
    from solo_epd_loader import epd_load
 
    df_1, df_2, energies = epd_load(sensor, startdate, enddate=None, level='l2', viewing=None, path=None, 
-                                   autodownload=False, only_averages=False, contamination_threshold=2)
+                                   autodownload=False, only_averages=False)
 
 Input
 ~~~~~
 
 -  ``sensor``: ``'ept'``, ``'het'``, or ``'step'`` (string)
 -  ``startdate``, ``enddate``: Datetime object (e.g., ``dt.date(2021,12,31)`` or ``dt.datetime(2021,4,15)``) or integer of the form yyyymmdd with empty positions filled with zeros, e.g. ``20210415`` (if no ``enddate`` is provided, ``enddate = startdate`` will be used)
 -  ``level``: ``'l2'`` or ``'ll'`` (string); defines level of data product: level 2 (``'l2'``) or low-latency (``'ll'``). By default ``'l2'``.
 -  ``viewing``: ``'sun'``, ``'asun'``, ``'north'``, ``'south'`` (string) or ``None``; not
    needed for ``sensor = 'step'``
 -  ``path``: directory in which Solar Orbiter data is/should be
    organized; e.g. ``'/home/userxyz/solo/data/'`` (string). See `Data folder structure`_ for more details.
 -  ``autodownload``: if ``True``, will try to download missing data files
    from SOAR (bolean)
 - ``only_averages``: If ``True``, will for STEP only return the averaged fluxes, and not the data of each of the 15 Pixels. This will reduce the memory consumption. By default ``False``.
-- ``contamination_threshold``: If integer, mask electron data that probably is contaminated (i.e., set it to ``nan``) using an integer contamination threshold following the equation ``Integral_Flux - Magnet_Flux > contamination_threshold * Integral_Uncertainty``. If ``False``, don't alter the data at all. Only implemented for new STEP data (after Oct 2021) so far. By default ``2``.
 
 Return
 ~~~~~~
 
 -  For ``sensor`` = ``'ept'`` or ``'het'``:
 
    1. Pandas dataframe with proton fluxes and errors (for EPT also alpha
@@ -102,20 +101,14 @@
       -  Value of energy bin width in MeV
 
 SupraThermal Electron Proton (STEP) sensor electron measurements
 ----------------------------------------------------------------
 
 Please note that the STEP electron measurements are not directly provided in the publically released data, but need to be calculated from them. This process is not straightforward, and the resulting data is prone to uncertainties (like contamination). **Thus it should only be used scientifically with caution! Please refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
 
-The ``contamination_threshold`` option can be used when calling ``epd_load()`` to mask STEP electron data that probably is contaminated (i.e., it is set to nan) following the equation:
-
-   Integral_Flux - Magnet_Flux > contamination_threshold * Integral_Uncertainty
-
-The default setting is ``contamination_threshold=2``.
-
 
 Data folder structure
 ---------------------
 
 The ``path`` variable provided to the module should be the base
 directory where the corresponding cdf data files should be placed in
 subdirectories. First subfolder defines the data product ``level``
```

### Comparing `solo_epd_loader-0.2.4/code_of_conduct.md` & `solo_epd_loader-0.2.5/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.4/docs/Makefile` & `solo_epd_loader-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.4/docs/conf.py` & `solo_epd_loader-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.4/docs/make.bat` & `solo_epd_loader-0.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.4/examples/gh2021_fig_2.png` & `solo_epd_loader-0.2.5/examples/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.4/examples/ws2021_fig_2d.png` & `solo_epd_loader-0.2.5/examples/ws2021_fig_2d.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.4/gh2021_fig_2.png` & `solo_epd_loader-0.2.5/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.4/gh2021_fig_2a.png` & `solo_epd_loader-0.2.5/gh2021_fig_2a.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.4/licenses/LICENSE.rst` & `solo_epd_loader-0.2.5/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.4/licenses/TEMPLATE_LICENSE.rst` & `solo_epd_loader-0.2.5/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.4/setup.cfg` & `solo_epd_loader-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.4/setup.py` & `solo_epd_loader-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.4/solo_epd_loader/__init__.py` & `solo_epd_loader-0.2.5/solo_epd_loader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,14 +480,15 @@
         If True, will try to download missing data files from SOAR, by default
         False.
     only_averages : bool, optional
         If True, will for STEP only return the averaged fluxes, and not the data
         of each of the 15 Pixels. This will reduce the memory consumption. By
         default False.
     contamination_threshold : int or False, optional
+        >> NOT IN USE AS OF VERSION 0.2.4 <<
         If int, mask electron data that probably is contaminated (i.e., set it
         to nan) using an integer contamination threshold following the equation:
         Integral_Flux - Magnet_Flux > contamination_threshold * Integral_Uncertainty
         If False, don't alter the data at all. Only implemented for new STEP
         data (after Oct 2021) so far. By default 2.
 
     Returns
```

### Comparing `solo_epd_loader-0.2.4/solo_epd_loader.egg-info/PKG-INFO` & `solo_epd_loader-0.2.5/solo_epd_loader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo-epd-loader
-Version: 0.2.4
+Version: 0.2.5
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -80,30 +80,29 @@
 containing information on the energy channels.
 
 .. code:: python
 
    from solo_epd_loader import epd_load
 
    df_1, df_2, energies = epd_load(sensor, startdate, enddate=None, level='l2', viewing=None, path=None, 
-                                   autodownload=False, only_averages=False, contamination_threshold=2)
+                                   autodownload=False, only_averages=False)
 
 Input
 ~~~~~
 
 -  ``sensor``: ``'ept'``, ``'het'``, or ``'step'`` (string)
 -  ``startdate``, ``enddate``: Datetime object (e.g., ``dt.date(2021,12,31)`` or ``dt.datetime(2021,4,15)``) or integer of the form yyyymmdd with empty positions filled with zeros, e.g. ``20210415`` (if no ``enddate`` is provided, ``enddate = startdate`` will be used)
 -  ``level``: ``'l2'`` or ``'ll'`` (string); defines level of data product: level 2 (``'l2'``) or low-latency (``'ll'``). By default ``'l2'``.
 -  ``viewing``: ``'sun'``, ``'asun'``, ``'north'``, ``'south'`` (string) or ``None``; not
    needed for ``sensor = 'step'``
 -  ``path``: directory in which Solar Orbiter data is/should be
    organized; e.g. ``'/home/userxyz/solo/data/'`` (string). See `Data folder structure`_ for more details.
 -  ``autodownload``: if ``True``, will try to download missing data files
    from SOAR (bolean)
 - ``only_averages``: If ``True``, will for STEP only return the averaged fluxes, and not the data of each of the 15 Pixels. This will reduce the memory consumption. By default ``False``.
-- ``contamination_threshold``: If integer, mask electron data that probably is contaminated (i.e., set it to ``nan``) using an integer contamination threshold following the equation ``Integral_Flux - Magnet_Flux > contamination_threshold * Integral_Uncertainty``. If ``False``, don't alter the data at all. Only implemented for new STEP data (after Oct 2021) so far. By default ``2``.
 
 Return
 ~~~~~~
 
 -  For ``sensor`` = ``'ept'`` or ``'het'``:
 
    1. Pandas dataframe with proton fluxes and errors (for EPT also alpha
@@ -127,20 +126,14 @@
       -  Value of energy bin width in MeV
 
 SupraThermal Electron Proton (STEP) sensor electron measurements
 ----------------------------------------------------------------
 
 Please note that the STEP electron measurements are not directly provided in the publically released data, but need to be calculated from them. This process is not straightforward, and the resulting data is prone to uncertainties (like contamination). **Thus it should only be used scientifically with caution! Please refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
 
-The ``contamination_threshold`` option can be used when calling ``epd_load()`` to mask STEP electron data that probably is contaminated (i.e., it is set to nan) following the equation:
-
-   Integral_Flux - Magnet_Flux > contamination_threshold * Integral_Uncertainty
-
-The default setting is ``contamination_threshold=2``.
-
 
 Data folder structure
 ---------------------
 
 The ``path`` variable provided to the module should be the base
 directory where the corresponding cdf data files should be placed in
 subdirectories. First subfolder defines the data product ``level``
```

### Comparing `solo_epd_loader-0.2.4/solo_epd_loader.egg-info/SOURCES.txt` & `solo_epd_loader-0.2.5/solo_epd_loader.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 docs/conf.py
 docs/index.rst
 docs/make.bat
 examples/gh2021_fig_2.png
 examples/ws2021_fig_2d.png
 licenses/LICENSE.rst
 licenses/TEMPLATE_LICENSE.rst
-solo_epd_loader/__init__ (STEP UPDATE).py
 solo_epd_loader/__init__.py
 solo_epd_loader/version.py
 solo_epd_loader.egg-info/PKG-INFO
 solo_epd_loader.egg-info/SOURCES.txt
 solo_epd_loader.egg-info/dependency_links.txt
 solo_epd_loader.egg-info/not-zip-safe
 solo_epd_loader.egg-info/requires.txt
```

### Comparing `solo_epd_loader-0.2.4/tox.ini` & `solo_epd_loader-0.2.5/tox.ini`

 * *Files identical despite different names*

