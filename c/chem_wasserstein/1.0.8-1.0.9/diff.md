# Comparing `tmp/chem_wasserstein-1.0.8.tar.gz` & `tmp/chem_wasserstein-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chem_wasserstein-1.0.8.tar", last modified: Wed Dec 22 08:59:18 2021, max compression
+gzip compressed data, was "chem_wasserstein-1.0.9.tar", last modified: Thu Feb 17 04:41:24 2022, max compression
```

## Comparing `chem_wasserstein-1.0.8.tar` & `chem_wasserstein-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1498 2021-12-14 11:15:43.252189 chem_wasserstein-1.0.8/.github/workflows/conda-build-pytest.yml
--rw-r--r--   0        0        0      958 2021-12-14 11:15:43.257175 chem_wasserstein-1.0.8/.github/workflows/flit-install-test.yml
--rw-r--r--   0        0        0     2772 2021-12-14 11:15:43.262192 chem_wasserstein-1.0.8/.github/workflows/test-publish-release.yml
--rw-r--r--   0        0        0     2053 2021-10-30 20:12:35.342117 chem_wasserstein-1.0.8/.gitignore
--rw-r--r--   0        0        0    35823 2021-10-30 11:21:41.722213 chem_wasserstein-1.0.8/LICENSE
--rw-r--r--   0        0        0     6828 2021-12-14 11:15:43.271170 chem_wasserstein-1.0.8/README.md
--rw-r--r--   0        0        0    33228 2021-11-20 05:44:57.879593 chem_wasserstein-1.0.8/chem_wasserstein/ElM2D_.py
--rw-r--r--   0        0        0  6250500 2021-10-31 00:54:50.212554 chem_wasserstein-1.0.8/chem_wasserstein/ElM2D_0-4-0_ElMD_0-4-3.csv
--rw-r--r--   0        0        0      135 2021-12-14 11:21:49.235690 chem_wasserstein-1.0.8/chem_wasserstein/__init__.py
--rw-r--r--   0        0        0     1068 2021-12-14 11:17:44.061649 chem_wasserstein-1.0.8/chem_wasserstein/meta.yaml
--rw-r--r--   0        0        0     5534 2021-11-01 13:52:15.005859 chem_wasserstein-1.0.8/chem_wasserstein/stable-mp-500.csv
--rw-r--r--   0        0        0     5015 2021-11-01 13:52:07.338169 chem_wasserstein-1.0.8/chem_wasserstein/test_ElM2D.py
--rw-r--r--   0        0        0     3669 2021-10-31 00:54:50.235492 chem_wasserstein-1.0.8/chem_wasserstein/train-debug.csv
--rw-r--r--   0        0        0     1019 2021-12-14 11:15:30.719765 chem_wasserstein-1.0.8/chem_wasserstein/utils/Timer.py
--rw-r--r--   0        0        0     1169 2021-12-14 11:21:44.461175 chem_wasserstein-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      172 2021-11-01 13:51:39.646837 chem_wasserstein-1.0.8/requirements.txt
--rw-r--r--   0        0        0      518 2021-10-31 04:27:04.831685 chem_wasserstein-1.0.8/run_grayskull.py
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 chem_wasserstein-1.0.8/setup.py
--rw-r--r--   0        0        0     7796 1970-01-01 00:00:00.000000 chem_wasserstein-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1498 2021-12-14 11:15:43.252189 chem_wasserstein-1.0.9/.github/workflows/conda-build-pytest.yml
+-rw-r--r--   0        0        0      958 2021-12-14 11:15:43.257175 chem_wasserstein-1.0.9/.github/workflows/flit-install-test.yml
+-rw-r--r--   0        0        0     2772 2021-12-14 11:15:43.262192 chem_wasserstein-1.0.9/.github/workflows/test-publish-release.yml
+-rw-r--r--   0        0        0     2053 2021-10-30 20:12:35.342117 chem_wasserstein-1.0.9/.gitignore
+-rw-r--r--   0        0        0    35823 2021-10-30 11:21:41.722213 chem_wasserstein-1.0.9/LICENSE
+-rw-r--r--   0        0        0     6828 2021-12-14 11:15:43.271170 chem_wasserstein-1.0.9/README.md
+-rw-r--r--   0        0        0    33228 2021-11-20 05:44:57.879593 chem_wasserstein-1.0.9/chem_wasserstein/ElM2D_.py
+-rw-r--r--   0        0        0  6250500 2021-10-31 00:54:50.212554 chem_wasserstein-1.0.9/chem_wasserstein/ElM2D_0-4-0_ElMD_0-4-3.csv
+-rw-r--r--   0        0        0      135 2022-02-17 04:40:47.227127 chem_wasserstein-1.0.9/chem_wasserstein/__init__.py
+-rw-r--r--   0        0        0     1084 2021-12-22 08:59:45.087418 chem_wasserstein-1.0.9/chem_wasserstein/meta.yaml
+-rw-r--r--   0        0        0     5534 2021-11-01 13:52:15.005859 chem_wasserstein-1.0.9/chem_wasserstein/stable-mp-500.csv
+-rw-r--r--   0        0        0     5015 2021-11-01 13:52:07.338169 chem_wasserstein-1.0.9/chem_wasserstein/test_ElM2D.py
+-rw-r--r--   0        0        0     3669 2021-10-31 00:54:50.235492 chem_wasserstein-1.0.9/chem_wasserstein/train-debug.csv
+-rw-r--r--   0        0        0     1019 2021-12-14 11:15:30.719765 chem_wasserstein-1.0.9/chem_wasserstein/utils/Timer.py
+-rw-r--r--   0        0        0     1169 2022-02-17 04:40:08.942839 chem_wasserstein-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      172 2021-11-01 13:51:39.646837 chem_wasserstein-1.0.9/requirements.txt
+-rw-r--r--   0        0        0      518 2021-10-31 04:27:04.831685 chem_wasserstein-1.0.9/run_grayskull.py
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 chem_wasserstein-1.0.9/setup.py
+-rw-r--r--   0        0        0     7796 1970-01-01 00:00:00.000000 chem_wasserstein-1.0.9/PKG-INFO
```

### Comparing `chem_wasserstein-1.0.8/.github/workflows/conda-build-pytest.yml` & `chem_wasserstein-1.0.9/.github/workflows/conda-build-pytest.yml`

 * *Files identical despite different names*

### Comparing `chem_wasserstein-1.0.8/.github/workflows/flit-install-test.yml` & `chem_wasserstein-1.0.9/.github/workflows/flit-install-test.yml`

 * *Files identical despite different names*

### Comparing `chem_wasserstein-1.0.8/.github/workflows/test-publish-release.yml` & `chem_wasserstein-1.0.9/.github/workflows/test-publish-release.yml`

 * *Files identical despite different names*

### Comparing `chem_wasserstein-1.0.8/.gitignore` & `chem_wasserstein-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `chem_wasserstein-1.0.8/LICENSE` & `chem_wasserstein-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chem_wasserstein-1.0.8/README.md` & `chem_wasserstein-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `chem_wasserstein-1.0.8/chem_wasserstein/ElM2D_.py` & `chem_wasserstein-1.0.9/chem_wasserstein/ElM2D_.py`

 * *Files identical despite different names*

### Comparing `chem_wasserstein-1.0.8/chem_wasserstein/ElM2D_0-4-0_ElMD_0-4-3.csv` & `chem_wasserstein-1.0.9/chem_wasserstein/ElM2D_0-4-0_ElMD_0-4-3.csv`

 * *Files identical despite different names*

### Comparing `chem_wasserstein-1.0.8/chem_wasserstein/meta.yaml` & `chem_wasserstein-1.0.9/chem_wasserstein/meta.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 {% set name = "chem_wasserstein" %}
-{% set version = "1.0.7" %}
+{% set version = "1.0.8" %}
 
 
 package:
   name: {{ name|lower }}
   version: {{ version }}
 
 source:
   url: https://pypi.io/packages/source/{{ name[0] }}/{{ name }}/chem_wasserstein-{{ version }}.tar.gz
-  sha256: dc5d788f1b7d7b6ac3974c7b651b68acf87c546ee7636e893b5931cda8cebd3b
+  sha256: 61dfd2069eb2579870f31d16ca156553757cc84824e2356e038cf1ae0bbf2fcf
 
 build:
   number: 0
   noarch: python
   script: {{ PYTHON }} -m pip install . -vv
 
 requirements:
   host:
     - pip
     - flit
     - python >=3.6,<3.10
   run:
+    - colorama
     - dist_matrix >=1.0.2
     - elmd ==0.4.8
     - numba >=0.53.1
     - pandas
     - plotly
     - pqdm ==0.1.0
     - python >=3.6,<3.10
```

### Comparing `chem_wasserstein-1.0.8/chem_wasserstein/stable-mp-500.csv` & `chem_wasserstein-1.0.9/chem_wasserstein/stable-mp-500.csv`

 * *Files identical despite different names*

### Comparing `chem_wasserstein-1.0.8/chem_wasserstein/test_ElM2D.py` & `chem_wasserstein-1.0.9/chem_wasserstein/test_ElM2D.py`

 * *Files identical despite different names*

### Comparing `chem_wasserstein-1.0.8/chem_wasserstein/train-debug.csv` & `chem_wasserstein-1.0.9/chem_wasserstein/train-debug.csv`

 * *Files identical despite different names*

### Comparing `chem_wasserstein-1.0.8/chem_wasserstein/utils/Timer.py` & `chem_wasserstein-1.0.9/chem_wasserstein/utils/Timer.py`

 * *Files identical despite different names*

### Comparing `chem_wasserstein-1.0.8/pyproject.toml` & `chem_wasserstein-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 00000310: 3a3a 2033 2e37 270d 0a20 2020 205d 0d0a  :: 3.7'..    ]..
 00000320: 6479 6e61 6d69 6320 3d20 5b22 7665 7273  dynamic = ["vers
 00000330: 696f 6e22 2c20 2264 6573 6372 6970 7469  ion", "descripti
 00000340: 6f6e 225d 0d0a 0d0a 7265 7175 6972 6573  on"]....requires
 00000350: 2d70 7974 686f 6e20 3d20 223e 3d33 2e37  -python = ">=3.7
 00000360: 2c3c 332e 3130 220d 0a0d 0a64 6570 656e  ,<3.10"....depen
 00000370: 6465 6e63 6965 7320 3d20 5b0d 0a20 2020  dencies = [..   
-00000380: 2022 7071 646d 203d 3d30 2e31 2e30 222c   "pqdm ==0.1.0",
+00000380: 2022 7071 646d 203e 3d30 2e31 2e30 222c   "pqdm >=0.1.0",
 00000390: 0d0a 2020 2020 2270 6c6f 746c 7922 2c0d  ..    "plotly",.
 000003a0: 0a20 2020 2022 7061 6e64 6173 222c 0d0a  .    "pandas",..
 000003b0: 2020 2020 226e 756d 6261 203e 3d30 2e35      "numba >=0.5
 000003c0: 332e 3122 2c0d 0a20 2020 2022 7363 6970  3.1",..    "scip
 000003d0: 7922 2c0d 0a20 2020 2022 7471 646d 222c  y",..    "tqdm",
 000003e0: 0d0a 2020 2020 2263 6f6c 6f72 616d 6122  ..    "colorama"
 000003f0: 2c0d 0a20 2020 2022 756d 6170 2d6c 6561  ,..    "umap-lea
```

### Comparing `chem_wasserstein-1.0.8/run_grayskull.py` & `chem_wasserstein-1.0.9/run_grayskull.py`

 * *Files identical despite different names*

### Comparing `chem_wasserstein-1.0.8/setup.py` & `chem_wasserstein-1.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 packages = \
 ['chem_wasserstein']
 
 package_data = \
 {'': ['*'], 'chem_wasserstein': ['utils/*']}
 
 setup(name='chem_wasserstein',
-      version='1.0.8',
+      version='1.0.9',
       description='A high performance mapping class to construct ElM2D plots from large datasets of inorganic compositions.',
       author=None,
       author_email='Cameron Hagreaves <cameron.h@rgreaves.me.uk>, "Sterling G. Baird" <sterling.baird@utah.edu>',
       url=None,
       packages=packages,
       package_data=package_data,
       python_requires='>=3.7,<3.10',
```

### Comparing `chem_wasserstein-1.0.8/PKG-INFO` & `chem_wasserstein-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: chem_wasserstein
-Version: 1.0.8
+Version: 1.0.9
 Summary: A high performance mapping class to construct ElM2D plots from large datasets of inorganic compositions.
 Author-email: Cameron Hagreaves <cameron.h@rgreaves.me.uk>, "Sterling G. Baird" <sterling.baird@utah.edu>
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Requires-Dist: pqdm ==0.1.0
+Requires-Dist: pqdm >=0.1.0
 Requires-Dist: plotly
 Requires-Dist: pandas
 Requires-Dist: numba >=0.53.1
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: colorama
 Requires-Dist: umap-learn
```

