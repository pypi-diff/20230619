# Comparing `tmp/jax-dataloader-0.0.4.tar.gz` & `tmp/jax-dataloader-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-dataloader-0.0.4.tar", last modified: Sun May 14 02:06:35 2023, max compression
+gzip compressed data, was "jax-dataloader-0.0.5.tar", last modified: Mon Jun 19 05:29:16 2023, max compression
```

## Comparing `jax-dataloader-0.0.4.tar` & `jax-dataloader-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-14 02:06:35.471787 jax-dataloader-0.0.4/
--rw-rw-r--   0 birk      (1000) birk      (1000)    11337 2022-09-05 16:31:43.000000 jax-dataloader-0.0.4/LICENSE
--rw-rw-r--   0 birk      (1000) birk      (1000)      111 2022-09-05 16:31:43.000000 jax-dataloader-0.0.4/MANIFEST.in
--rw-r--r--   0 birk      (1000) birk      (1000)     6155 2023-05-14 02:06:35.471787 jax-dataloader-0.0.4/PKG-INFO
--rw-r--r--   0 birk      (1000) birk      (1000)     5184 2023-05-14 01:39:23.000000 jax-dataloader-0.0.4/README.md
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-14 02:06:35.471787 jax-dataloader-0.0.4/jax_dataloader/
--rw-r--r--   0 birk      (1000) birk      (1000)      112 2023-05-14 02:05:00.000000 jax-dataloader-0.0.4/jax_dataloader/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)    15604 2023-05-14 02:05:00.000000 jax-dataloader-0.0.4/jax_dataloader/_modidx.py
--rw-r--r--   0 birk      (1000) birk      (1000)     5077 2023-05-14 02:05:00.000000 jax-dataloader-0.0.4/jax_dataloader/core.py
--rw-r--r--   0 birk      (1000) birk      (1000)     2910 2023-05-14 02:05:00.000000 jax-dataloader-0.0.4/jax_dataloader/datasets.py
--rw-r--r--   0 birk      (1000) birk      (1000)      758 2023-04-06 01:20:29.000000 jax-dataloader-0.0.4/jax_dataloader/imports.py
--rw-r--r--   0 birk      (1000) birk      (1000)     6464 2023-05-14 02:05:00.000000 jax-dataloader-0.0.4/jax_dataloader/loaders.py
--rw-r--r--   0 birk      (1000) birk      (1000)     3317 2023-05-14 02:05:00.000000 jax-dataloader-0.0.4/jax_dataloader/utils.py
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-14 02:06:35.471787 jax-dataloader-0.0.4/jax_dataloader.egg-info/
--rw-r--r--   0 birk      (1000) birk      (1000)     6155 2023-05-14 02:06:35.000000 jax-dataloader-0.0.4/jax_dataloader.egg-info/PKG-INFO
--rw-r--r--   0 birk      (1000) birk      (1000)      497 2023-05-14 02:06:35.000000 jax-dataloader-0.0.4/jax_dataloader.egg-info/SOURCES.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-05-14 02:06:35.000000 jax-dataloader-0.0.4/jax_dataloader.egg-info/dependency_links.txt
--rw-r--r--   0 birk      (1000) birk      (1000)       50 2023-05-14 02:06:35.000000 jax-dataloader-0.0.4/jax_dataloader.egg-info/entry_points.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-01-12 03:15:10.000000 jax-dataloader-0.0.4/jax_dataloader.egg-info/not-zip-safe
--rw-r--r--   0 birk      (1000) birk      (1000)      284 2023-05-14 02:06:35.000000 jax-dataloader-0.0.4/jax_dataloader.egg-info/requires.txt
--rw-r--r--   0 birk      (1000) birk      (1000)       15 2023-05-14 02:06:35.000000 jax-dataloader-0.0.4/jax_dataloader.egg-info/top_level.txt
--rw-r--r--   0 birk      (1000) birk      (1000)     1101 2023-05-14 02:05:00.000000 jax-dataloader-0.0.4/settings.ini
--rw-r--r--   0 birk      (1000) birk      (1000)       38 2023-05-14 02:06:35.471787 jax-dataloader-0.0.4/setup.cfg
--rw-r--r--   0 birk      (1000) birk      (1000)     3133 2023-05-14 01:31:28.000000 jax-dataloader-0.0.4/setup.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-06-19 05:29:16.360000 jax-dataloader-0.0.5/
+-rw-r--r--   0 birk      (1000) birk      (1000)    11337 2023-02-25 10:09:10.000000 jax-dataloader-0.0.5/LICENSE
+-rw-r--r--   0 birk      (1000) birk      (1000)      111 2023-02-25 10:09:10.000000 jax-dataloader-0.0.5/MANIFEST.in
+-rw-r--r--   0 birk      (1000) birk      (1000)     6159 2023-06-19 05:29:16.350000 jax-dataloader-0.0.5/PKG-INFO
+-rw-r--r--   0 birk      (1000) birk      (1000)     5188 2023-06-19 05:25:24.000000 jax-dataloader-0.0.5/README.md
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-06-19 05:29:16.350000 jax-dataloader-0.0.5/jax_dataloader/
+-rw-r--r--   0 birk      (1000) birk      (1000)      112 2023-06-19 05:28:06.000000 jax-dataloader-0.0.5/jax_dataloader/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    15604 2023-06-19 05:28:06.000000 jax-dataloader-0.0.5/jax_dataloader/_modidx.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     5077 2023-06-19 05:28:06.000000 jax-dataloader-0.0.5/jax_dataloader/core.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     2910 2023-06-19 05:28:06.000000 jax-dataloader-0.0.5/jax_dataloader/datasets.py
+-rw-r--r--   0 birk      (1000) birk      (1000)      727 2023-04-06 17:19:14.000000 jax-dataloader-0.0.5/jax_dataloader/imports.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     6464 2023-06-19 05:28:06.000000 jax-dataloader-0.0.5/jax_dataloader/loaders.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     3318 2023-06-19 05:28:06.000000 jax-dataloader-0.0.5/jax_dataloader/utils.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-06-19 05:29:16.350000 jax-dataloader-0.0.5/jax_dataloader.egg-info/
+-rw-r--r--   0 birk      (1000) birk      (1000)     6159 2023-06-19 05:29:16.000000 jax-dataloader-0.0.5/jax_dataloader.egg-info/PKG-INFO
+-rw-r--r--   0 birk      (1000) birk      (1000)      497 2023-06-19 05:29:16.000000 jax-dataloader-0.0.5/jax_dataloader.egg-info/SOURCES.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-06-19 05:29:16.000000 jax-dataloader-0.0.5/jax_dataloader.egg-info/dependency_links.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)       50 2023-06-19 05:29:16.000000 jax-dataloader-0.0.5/jax_dataloader.egg-info/entry_points.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-02-25 11:37:50.000000 jax-dataloader-0.0.5/jax_dataloader.egg-info/not-zip-safe
+-rw-r--r--   0 birk      (1000) birk      (1000)      377 2023-06-19 05:29:16.000000 jax-dataloader-0.0.5/jax_dataloader.egg-info/requires.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)       15 2023-06-19 05:29:16.000000 jax-dataloader-0.0.5/jax_dataloader.egg-info/top_level.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)     1113 2023-06-19 05:28:06.000000 jax-dataloader-0.0.5/settings.ini
+-rw-r--r--   0 birk      (1000) birk      (1000)       38 2023-06-19 05:29:16.360000 jax-dataloader-0.0.5/setup.cfg
+-rw-r--r--   0 birk      (1000) birk      (1000)     3066 2023-06-18 12:11:28.000000 jax-dataloader-0.0.5/setup.py
```

### Comparing `jax-dataloader-0.0.4/LICENSE` & `jax-dataloader-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jax-dataloader-0.0.4/PKG-INFO` & `jax-dataloader-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-dataloader
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dataloader for jax
 Home-page: https://github.com/birkhoffg/jax-dataloader
 Author: BirkhoffG
 Author-email: 26811230+BirkhoffG@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: python jax dataloader pytorch tensorflow datasets huggingface
 Classifier: Development Status :: 4 - Beta
@@ -21,15 +21,15 @@
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: tensorflow
 Provides-Extra: huggingface
 Provides-Extra: torch
 License-File: LICENSE
 
-# Jax-Dataloader
+# Dataloader for JAX
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ![Python](https://img.shields.io/pypi/pyversions/jax-dataloader.svg)
 ![CI
 status](https://github.com/BirkhoffG/jax-dataloader/actions/workflows/nbdev.yaml/badge.svg)
 ![Docs](https://github.com/BirkhoffG/jax-dataloader/actions/workflows/deploy.yaml/badge.svg)
```

### Comparing `jax-dataloader-0.0.4/README.md` & `jax-dataloader-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Jax-Dataloader
+# Dataloader for JAX
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ![Python](https://img.shields.io/pypi/pyversions/jax-dataloader.svg)
 ![CI
 status](https://github.com/BirkhoffG/jax-dataloader/actions/workflows/nbdev.yaml/badge.svg)
 ![Docs](https://github.com/BirkhoffG/jax-dataloader/actions/workflows/deploy.yaml/badge.svg)
```

### Comparing `jax-dataloader-0.0.4/jax_dataloader/_modidx.py` & `jax-dataloader-0.0.5/jax_dataloader/_modidx.py`

 * *Files identical despite different names*

### Comparing `jax-dataloader-0.0.4/jax_dataloader/core.py` & `jax-dataloader-0.0.5/jax_dataloader/core.py`

 * *Files identical despite different names*

### Comparing `jax-dataloader-0.0.4/jax_dataloader/datasets.py` & `jax-dataloader-0.0.5/jax_dataloader/datasets.py`

 * *Files identical despite different names*

### Comparing `jax-dataloader-0.0.4/jax_dataloader/loaders.py` & `jax-dataloader-0.0.5/jax_dataloader/loaders.py`

 * *Files identical despite different names*

### Comparing `jax-dataloader-0.0.4/jax_dataloader/utils.py` & `jax-dataloader-0.0.5/jax_dataloader/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/utils.ipynb.
 
-# %% ../nbs/utils.ipynb 3
+# %% ../nbs/utils.ipynb 4
 from __future__ import print_function, division, annotations
 from .imports import *
 import jax_dataloader as jdl
 
 # %% auto 0
 __all__ = ['Config', 'get_config', 'PRNGSequence', 'check_pytorch_installed', 'has_pytorch_tensor', 'check_hf_installed',
            'check_tf_installed', 'is_hf_dataset', 'is_torch_dataset', 'is_jdl_dataset', 'is_tf_dataset']
 
-# %% ../nbs/utils.ipynb 4
+# %% ../nbs/utils.ipynb 5
 @dataclass
 class Config:
     """Global configuration for the library"""
     rng_reserve_size: int
     global_seed: int
 
     @classmethod
     def default(cls) -> Config:
         return cls(rng_reserve_size=1, global_seed=42)
 
-# %% ../nbs/utils.ipynb 5
+# %% ../nbs/utils.ipynb 6
 main_config = Config.default()
 
-# %% ../nbs/utils.ipynb 6
+# %% ../nbs/utils.ipynb 7
 def get_config() -> Config:
     return main_config
 
-# %% ../nbs/utils.ipynb 7
+# %% ../nbs/utils.ipynb 8
 class PRNGSequence(Iterator[PRNGKey]):
     """An Interator of Jax PRNGKey (minimal version of `haiku.PRNGSequence`)."""
 
     def __init__(self, seed: int):
         self._key = jax.random.PRNGKey(seed)
         self._subkeys = collections.deque()
 
@@ -43,58 +43,58 @@
             self._subkeys.extend(new_keys[1:])
             
     def __next__(self):
         if not self._subkeys:
             self.reserve(get_config().rng_reserve_size)
         return self._subkeys.popleft()
 
-# %% ../nbs/utils.ipynb 9
+# %% ../nbs/utils.ipynb 10
 def check_pytorch_installed():
     if torch_data is None:
         raise ModuleNotFoundError("`pytorch` library needs to be installed. "
             "Try `pip install torch`. Please refer to pytorch documentation for details: "
             "https://pytorch.org/get-started/.")
 
 
-# %% ../nbs/utils.ipynb 11
+# %% ../nbs/utils.ipynb 12
 def has_pytorch_tensor(batch) -> bool:
     if isinstance(batch[0], torch.Tensor):
         return True
     elif isinstance(batch[0], (tuple, list)):
         transposed = zip(*batch)
         return any([has_pytorch_tensor(samples) for samples in transposed])
     else:
         return False
 
-# %% ../nbs/utils.ipynb 12
+# %% ../nbs/utils.ipynb 13
 def check_hf_installed():
     if hf_datasets is None:
         raise ModuleNotFoundError("`datasets` library needs to be installed. "
             "Try `pip install datasets`. Please refer to huggingface documentation for details: "
             "https://huggingface.co/docs/datasets/installation.html.")
 
-# %% ../nbs/utils.ipynb 14
+# %% ../nbs/utils.ipynb 15
 def check_tf_installed():
     if tf is None:
         raise ModuleNotFoundError("`tensorflow` library needs to be installed. "
             "Try `pip install tensorflow`. Please refer to tensorflow documentation for details: "
             "https://www.tensorflow.org/install/pip.")
 
-# %% ../nbs/utils.ipynb 16
+# %% ../nbs/utils.ipynb 17
 def is_hf_dataset(dataset):
     return hf_datasets and (
         isinstance(dataset, hf_datasets.Dataset) 
         or isinstance(dataset, hf_datasets.DatasetDict)
     )
 
 
-# %% ../nbs/utils.ipynb 17
+# %% ../nbs/utils.ipynb 18
 def is_torch_dataset(dataset):
     return torch_data and isinstance(dataset, torch_data.Dataset)
 
-# %% ../nbs/utils.ipynb 18
+# %% ../nbs/utils.ipynb 19
 def is_jdl_dataset(dataset):
     return isinstance(dataset, jdl.Dataset)
 
-# %% ../nbs/utils.ipynb 19
+# %% ../nbs/utils.ipynb 20
 def is_tf_dataset(dataset):
     return tf and isinstance(dataset, tf.data.Dataset)
```

### Comparing `jax-dataloader-0.0.4/jax_dataloader.egg-info/PKG-INFO` & `jax-dataloader-0.0.5/jax_dataloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-dataloader
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dataloader for jax
 Home-page: https://github.com/birkhoffg/jax-dataloader
 Author: BirkhoffG
 Author-email: 26811230+BirkhoffG@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: python jax dataloader pytorch tensorflow datasets huggingface
 Classifier: Development Status :: 4 - Beta
@@ -21,15 +21,15 @@
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: tensorflow
 Provides-Extra: huggingface
 Provides-Extra: torch
 License-File: LICENSE
 
-# Jax-Dataloader
+# Dataloader for JAX
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ![Python](https://img.shields.io/pypi/pyversions/jax-dataloader.svg)
 ![CI
 status](https://github.com/BirkhoffG/jax-dataloader/actions/workflows/nbdev.yaml/badge.svg)
 ![Docs](https://github.com/BirkhoffG/jax-dataloader/actions/workflows/deploy.yaml/badge.svg)
```

### Comparing `jax-dataloader-0.0.4/settings.ini` & `jax-dataloader-0.0.5/settings.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [DEFAULT]
 repo = jax-dataloader
 lib_name = jax-dataloader
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 doc_path = _docs
 lib_path = jax_dataloader
 nbs_path = nbs
 recursive = True
 tst_flags = notest torch tf hf
 put_version_in_init = True
 branch = master
-custom_sidebar = False
+custom_sidebar = True
 doc_host = https://birkhoffg.github.io
 doc_baseurl = /jax-dataloader
 git_url = https://github.com/birkhoffg/jax-dataloader
-title = Jax-Dataloader
+title = JAX-Dataloader
 audience = Developers
 author = BirkhoffG
 author_email = 26811230+BirkhoffG@users.noreply.github.com
 copyright = 2023 onwards, BirkhoffG
 description = Dataloader for jax
 keywords = python jax dataloader pytorch tensorflow datasets huggingface
 language = English
 status = 3
 user = birkhoffg
 requirements = jax[cpu]
-dev_requirements = scikit-learn pandas nbdev jupyter dm-haiku optax
+dev_requirements = scikit-learn pandas nbdev jupyter dm-haiku optax nbdev-mkdocs
 torch_requirements = torch torchvision
 tensorflow_requirements = tensorflow tensorflow-datasets
 huggingface_requirements = datasets
 black_formatting = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys =
```

### Comparing `jax-dataloader-0.0.4/setup.py` & `jax-dataloader-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from pkg_resources import parse_version
-from configparser import ConfigParser
-import setuptools
-assert parse_version(setuptools.__version__)>=parse_version('36.2')
-
-# note: all settings are in settings.ini; edit there, not here
-config = ConfigParser(delimiters=['='])
-config.read('settings.ini')
-cfg = config['DEFAULT']
-
-cfg_keys = 'version description keywords author author_email'.split()
-expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
-for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
-setup_cfg = {o:cfg[o] for o in cfg_keys}
-
-licenses = {
-    'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
-    'mit': ('MIT License', 'OSI Approved :: MIT License'),
-    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
-    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
-    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
-}
-statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
-    '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
-py_versions = '3.7 3.8 3.9 3.10 3.11'.split()
-
-requirements = cfg.get('requirements','').split()
-if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
-min_python = cfg['min_python']
-lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
-
-tensorflow_requirements = (cfg.get('tensorflow_requirements') or '').split()
-huggingface_requirements = (cfg.get('huggingface_requirements') or '').split()
-torch_requirements = (cfg.get('torch_requirements') or '').split()
-dev_requirements = (cfg.get('dev_requirements') or '').split()
-all_requirements = requirements + tensorflow_requirements + huggingface_requirements + torch_requirements + dev_requirements
-
-extras_require = {
-    'all': all_requirements, 'dev': dev_requirements,
-    'tensorflow': tensorflow_requirements, 'huggingface': huggingface_requirements, 'torch': torch_requirements
-}
-
-setuptools.setup(
-    name = cfg['lib_name'],
-    license = lic[0],
-    classifiers = [
-        'Development Status :: ' + statuses[int(cfg['status'])],
-        'Intended Audience :: ' + cfg['audience'].title(),
-        'Natural Language :: ' + cfg['language'].title(),
-    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
-    url = cfg['git_url'],
-    packages = setuptools.find_packages(),
-    include_package_data = True,
-    install_requires = requirements,
-    extras_require=extras_require,
-    dependency_links = cfg.get('dep_links','').split(),
-    python_requires  = '>=' + cfg['min_python'],
-    long_description = open('README.md').read(),
-    long_description_content_type = 'text/markdown',
-    zip_safe = False,
-    entry_points = {
-        'console_scripts': cfg.get('console_scripts','').split(),
-        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
-    },
-    **setup_cfg)
-
-
+from pkg_resources import parse_version
+from configparser import ConfigParser
+import setuptools
+assert parse_version(setuptools.__version__)>=parse_version('36.2')
+
+# note: all settings are in settings.ini; edit there, not here
+config = ConfigParser(delimiters=['='])
+config.read('settings.ini')
+cfg = config['DEFAULT']
+
+cfg_keys = 'version description keywords author author_email'.split()
+expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
+for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
+setup_cfg = {o:cfg[o] for o in cfg_keys}
+
+licenses = {
+    'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
+    'mit': ('MIT License', 'OSI Approved :: MIT License'),
+    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
+    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
+    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
+}
+statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
+    '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
+py_versions = '3.7 3.8 3.9 3.10 3.11'.split()
+
+requirements = cfg.get('requirements','').split()
+if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
+min_python = cfg['min_python']
+lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
+
+tensorflow_requirements = (cfg.get('tensorflow_requirements') or '').split()
+huggingface_requirements = (cfg.get('huggingface_requirements') or '').split()
+torch_requirements = (cfg.get('torch_requirements') or '').split()
+dev_requirements = (cfg.get('dev_requirements') or '').split()
+all_requirements = requirements + tensorflow_requirements + huggingface_requirements + torch_requirements + dev_requirements
+
+extras_require = {
+    'all': all_requirements, 'dev': all_requirements,
+    'tensorflow': tensorflow_requirements, 'huggingface': huggingface_requirements, 'torch': torch_requirements
+}
+
+setuptools.setup(
+    name = cfg['lib_name'],
+    license = lic[0],
+    classifiers = [
+        'Development Status :: ' + statuses[int(cfg['status'])],
+        'Intended Audience :: ' + cfg['audience'].title(),
+        'Natural Language :: ' + cfg['language'].title(),
+    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
+    url = cfg['git_url'],
+    packages = setuptools.find_packages(),
+    include_package_data = True,
+    install_requires = requirements,
+    extras_require=extras_require,
+    dependency_links = cfg.get('dep_links','').split(),
+    python_requires  = '>=' + cfg['min_python'],
+    long_description = open('README.md').read(),
+    long_description_content_type = 'text/markdown',
+    zip_safe = False,
+    entry_points = {
+        'console_scripts': cfg.get('console_scripts','').split(),
+        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
+    },
+    **setup_cfg)
+
+
```

