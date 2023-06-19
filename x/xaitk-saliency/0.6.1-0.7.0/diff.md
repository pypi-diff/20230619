# Comparing `tmp/xaitk_saliency-0.6.1.tar.gz` & `tmp/xaitk_saliency-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xaitk_saliency-0.6.1.tar", max compression
+gzip compressed data, was "xaitk_saliency-0.7.0.tar", max compression
```

## Comparing `xaitk_saliency-0.6.1.tar` & `xaitk_saliency-0.7.0.tar`

### file list

```diff
@@ -1,46 +1,45 @@
--rw-r--r--   0        0        0     1476 2022-06-08 20:29:41.901960 xaitk_saliency-0.6.1/LICENSE.txt
--rw-r--r--   0        0        0     4559 2022-06-08 20:29:41.901960 xaitk_saliency-0.6.1/README.md
--rw-r--r--   0        0        0     4813 2022-06-08 20:29:41.961960 xaitk_saliency-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      943 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/__init__.py
--rw-r--r--   0        0        0      425 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/exceptions.py
--rw-r--r--   0        0        0        0 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/__init__.py
--rw-r--r--   0        0        0        0 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_classifier_conf_sal/__init__.py
--rw-r--r--   0        0        0     2172 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_classifier_conf_sal/occlusion_scoring.py
--rw-r--r--   0        0        0     2808 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_classifier_conf_sal/rise_scoring.py
--rw-r--r--   0        0        0     1957 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_classifier_conf_sal/squared_difference_scoring.py
--rw-r--r--   0        0        0        0 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_descriptor_sim_sal/__init__.py
--rw-r--r--   0        0        0     3876 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_descriptor_sim_sal/similarity_scoring.py
--rw-r--r--   0        0        0        0 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_detector_prop_sal/__init__.py
--rw-r--r--   0        0        0     5017 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_detector_prop_sal/drise_scoring.py
--rw-r--r--   0        0        0        0 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/__init__.py
--rw-r--r--   0        0        0     4215 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/occlusion_based.py
--rw-r--r--   0        0        0     3110 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/rise.py
--rw-r--r--   0        0        0     2926 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/slidingwindow.py
--rw-r--r--   0        0        0        0 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/__init__.py
--rw-r--r--   0        0        0     3970 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/occlusion_based.py
--rw-r--r--   0        0        0     3876 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/sbsm.py
--rw-r--r--   0        0        0        0 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_object_detector_blackbox_sal/__init__.py
--rw-r--r--   0        0        0     5843 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_object_detector_blackbox_sal/drise.py
--rw-r--r--   0        0        0     7028 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_object_detector_blackbox_sal/occlusion_based.py
--rw-r--r--   0        0        0        0 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/perturb_image/__init__.py
--rw-r--r--   0        0        0     4038 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/perturb_image/random_grid.py
--rw-r--r--   0        0        0     4689 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/perturb_image/rise.py
--rw-r--r--   0        0        0     3704 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/perturb_image/sliding_radial.py
--rw-r--r--   0        0        0     3054 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/impls/perturb_image/sliding_window.py
--rw-r--r--   0        0        0        0 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/interfaces/__init__.py
--rw-r--r--   0        0        0     4221 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/interfaces/gen_classifier_conf_sal.py
--rw-r--r--   0        0        0     3811 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/interfaces/gen_descriptor_sim_sal.py
--rw-r--r--   0        0        0     5054 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/interfaces/gen_detector_prop_sal.py
--rw-r--r--   0        0        0     4635 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/interfaces/gen_image_classifier_blackbox_sal.py
--rw-r--r--   0        0        0     5245 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/interfaces/gen_image_similarity_blackbox_sal.py
--rw-r--r--   0        0        0     9837 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/interfaces/gen_object_detector_blackbox_sal.py
--rw-r--r--   0        0        0     1651 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/interfaces/perturb_image.py
--rw-r--r--   0        0        0        0 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/py.typed
--rw-r--r--   0        0        0        0 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/utils/bin/__init__.py
--rw-r--r--   0        0        0     5724 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/utils/bin/sal_on_coco_dets.py
--rw-r--r--   0        0        0     2706 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/utils/coco.py
--rw-r--r--   0        0        0     2759 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/utils/detection.py
--rw-r--r--   0        0        0    14129 2022-06-08 20:29:41.965960 xaitk_saliency-0.6.1/xaitk_saliency/utils/masking.py
--rw-r--r--   0        0        0     8682 2022-06-08 20:30:02.561299 xaitk_saliency-0.6.1/setup.py
--rw-r--r--   0        0        0     6401 2022-06-08 20:30:02.561876 xaitk_saliency-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1476 2023-06-19 06:56:54.438357 xaitk_saliency-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     4559 2023-06-19 06:56:54.438357 xaitk_saliency-0.7.0/README.md
+-rw-r--r--   0        0        0     5506 2023-06-19 06:56:54.486358 xaitk_saliency-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      943 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/__init__.py
+-rw-r--r--   0        0        0      425 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_classifier_conf_sal/__init__.py
+-rw-r--r--   0        0        0     2172 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_classifier_conf_sal/occlusion_scoring.py
+-rw-r--r--   0        0        0     2808 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_classifier_conf_sal/rise_scoring.py
+-rw-r--r--   0        0        0     1957 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_classifier_conf_sal/squared_difference_scoring.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_descriptor_sim_sal/__init__.py
+-rw-r--r--   0        0        0     3876 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_descriptor_sim_sal/similarity_scoring.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_detector_prop_sal/__init__.py
+-rw-r--r--   0        0        0     5017 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_detector_prop_sal/drise_scoring.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/__init__.py
+-rw-r--r--   0        0        0     4215 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/occlusion_based.py
+-rw-r--r--   0        0        0     3110 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/rise.py
+-rw-r--r--   0        0        0     2926 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/slidingwindow.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/__init__.py
+-rw-r--r--   0        0        0     3970 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/occlusion_based.py
+-rw-r--r--   0        0        0     3876 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/sbsm.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_object_detector_blackbox_sal/__init__.py
+-rw-r--r--   0        0        0     5843 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_object_detector_blackbox_sal/drise.py
+-rw-r--r--   0        0        0     7008 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_object_detector_blackbox_sal/occlusion_based.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/__init__.py
+-rw-r--r--   0        0        0     4038 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/random_grid.py
+-rw-r--r--   0        0        0     4689 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/rise.py
+-rw-r--r--   0        0        0     3704 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/sliding_radial.py
+-rw-r--r--   0        0        0     3054 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/sliding_window.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/__init__.py
+-rw-r--r--   0        0        0     4221 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_classifier_conf_sal.py
+-rw-r--r--   0        0        0     3811 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_descriptor_sim_sal.py
+-rw-r--r--   0        0        0     5054 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_detector_prop_sal.py
+-rw-r--r--   0        0        0     4635 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_image_classifier_blackbox_sal.py
+-rw-r--r--   0        0        0     5245 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_image_similarity_blackbox_sal.py
+-rw-r--r--   0        0        0     9837 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_object_detector_blackbox_sal.py
+-rw-r--r--   0        0        0     1651 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/perturb_image.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/py.typed
+-rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/utils/bin/__init__.py
+-rw-r--r--   0        0        0     5732 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/utils/bin/sal_on_coco_dets.py
+-rw-r--r--   0        0        0     2706 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/utils/coco.py
+-rw-r--r--   0        0        0     2759 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/utils/detection.py
+-rw-r--r--   0        0        0    14129 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/utils/masking.py
+-rw-r--r--   0        0        0     6513 1970-01-01 00:00:00.000000 xaitk_saliency-0.7.0/PKG-INFO
```

### Comparing `xaitk_saliency-0.6.1/LICENSE.txt` & `xaitk_saliency-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/README.md` & `xaitk_saliency-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/pyproject.toml` & `xaitk_saliency-0.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ###############################################################################
 [tool.poetry]
 name = "xaitk_saliency"
 # REMEMBER: `distutils.version.*Version` types can be used to compare versions
 # from strings like this.
 # This package prefers to use the strict numbering standard when possible.
-version = "0.6.1"
+version = "0.7.0"
 description = """\
     Visual saliency map generation interfaces and baseline implementations \
     for explainable AI."""
 license = "BSD-3-Clause"
 authors = ["Kitware, Inc. <xaitk@kitware.com>"]
 readme = "README.md"
 repository = "https://github.com/XAITK/xaitk-saliency"
@@ -21,62 +21,78 @@
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Unix',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.10"
-numpy = "^1.20.3"
-scikit-image = "^0.18.1"
-scikit-learn = "^0.24.2"
+python = "^3.8"
+numpy = ">=1.22"
+scikit-image = [
+    # Hinge because minimum support 0.20.0 for py3.11
+    { version = ">=0.18.1", python = "<3.11" },
+    { version = ">=0.20.0", python = ">=3.11" }
+]
+scikit-learn = ">=1.2"
 smqtk-classifier = ">=0.17.0"
 smqtk-core = ">=0.18.0"
 smqtk-descriptors = ">=0.16.0"
-smqtk-detection = ">=0.18.1"
-scipy = "^1.6.3"
-click = "^8.0.3"
+smqtk-detection = ">=0.19.0"
+scipy = ">=1.8.1"
+click = ">=8.0.3"
+setuptools = "*"
 # Optionals for "example" extra
-jupyter = { version = "^1.0.0", optional = true }
-matplotlib = { version="^3.4.1", optional = true }
-papermill = { version = "^2.3.3", optional = true }
-torch = { version = "^1.9.0", optional = true }
-torchvision = { version = "^0.10.0", optional = true }
-tqdm = { version = "^4.45.0", optional = true }
+jupyter = { version = ">=1.0.0", optional = true }
+matplotlib = { version=">=3.4.1", optional = true }
+papermill = { version = ">=2.3.3", optional = true }
+torch = {version = ">=1.9.0,!=2.0.1", optional = true}
+torchvision = {version = ">=0.10.0", optional = true}
+tqdm = { version = ">=4.45.0", optional = true }
 # Optionals for "tools" extra"
-kwcoco = { version = "~0.2.18", optional = true}
+kwcoco = { version = ">=0.2.18", optional = true}
 
 [tool.poetry.extras]
 example_deps = [ "jupyter", "matplotlib", "papermill", "torch", "torchvision", "tqdm" ]
-tools = [ "kwcoco" ]
+tools = [ "kwcoco", "matplotlib" ]
 
 [tool.poetry.dev-dependencies]
 # CI
-flake8 = "^3.9.0"
-flake8-mutable = "^1.2.0"
-mypy = ">=0.812"
-types-setuptools = "^57.0.0"
+flake8 = [
+    # Hinge because 6.0 minimum supported python version is 3.8.1
+    { version = ">=5", python = "<3.8.1" },
+    { version = ">=6", python = ">=3.8.1" }
+]
+flake8-mutable = ">=1.2"
+mypy = ">=0.991"
+types-setuptools = ">=57.0.0"
 # Docs
 # - Also see: `docs/readthedocs-reqs.txt` for use by RTD
-Sphinx = "^3.5.3"
-sphinx-rtd-theme = "^0.5.1"
-sphinx-prompt = "^1.4.0"
-livereload = "^2.6.3"
+Sphinx = [
+    # Hinge because, while sphinx >=5.3 supports python <3.8.1, it requires an
+    # importlib-metadata version higher than what flake8 ^5 supports, which is
+    # the version of flake8 required for python version <3.8.1.
+    { version = ">=4.3.2", python = "<3.8.1" },
+    { version = ">=5.3", python = ">=3.8.1"}
+]
+sphinx-rtd-theme = ">=1.1.1"
+sphinx-prompt = ">=1.5"
+livereload = ">=2.6.3"
 # Testing
-coverage = "^5.5"
-pytest = "^6.2.2"
-pytest-cov = "^2.11.1"
+coverage = ">=6.5.0"
+pytest = ">=7.2.0"
+pytest-cov = ">=4.0.0"
 # Utility
-ipython = "^7.31.1"
+ipython = ">=8.6.0"
 
 [tool.poetry.scripts]
 sal-on-coco-dets= "xaitk_saliency.utils.bin.sal_on_coco_dets:sal_on_coco_dets"
 
 [tool.poetry.plugins."smqtk_plugins"]
 # Add implementation sub-module exposure here.
 "impls.perturb_image.sliding_window" = "xaitk_saliency.impls.perturb_image.sliding_window"
```

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/__init__.py` & `xaitk_saliency-0.7.0/xaitk_saliency/__init__.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_classifier_conf_sal/occlusion_scoring.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_classifier_conf_sal/occlusion_scoring.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_classifier_conf_sal/rise_scoring.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_classifier_conf_sal/rise_scoring.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_classifier_conf_sal/squared_difference_scoring.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_classifier_conf_sal/squared_difference_scoring.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_descriptor_sim_sal/similarity_scoring.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_descriptor_sim_sal/similarity_scoring.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_detector_prop_sal/drise_scoring.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_detector_prop_sal/drise_scoring.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/occlusion_based.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/occlusion_based.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/rise.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/rise.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/slidingwindow.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/slidingwindow.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/occlusion_based.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/occlusion_based.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/sbsm.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/sbsm.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_object_detector_blackbox_sal/drise.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_object_detector_blackbox_sal/drise.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/gen_object_detector_blackbox_sal/occlusion_based.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_object_detector_blackbox_sal/occlusion_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,17 +129,17 @@
 
     :returns: Matrix of detections with shape
         [nImgs x nDets x (4+1+nClasses)].
         If the number of detections for each image is not consistent, the matrix
         will be padded with rows of ones, except for the objectness which is set
         to zero.
     """
-    labels = []  # type: Sequence[Hashable]
+    labels: List[Hashable] = []
     num_classes = 0
-    dets_mat_list = []  # type: List[np.ndarray]
+    dets_mat_list: List[np.ndarray] = []
     for img_idx, img_dets in enumerate(dets):
 
         img_bboxes = np.array([])
         img_scores = np.array([])
         img_objectness = np.array([])
 
         # reshape for vertical stacking
```

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/perturb_image/random_grid.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/random_grid.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/perturb_image/rise.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/rise.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/perturb_image/sliding_radial.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/sliding_radial.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/impls/perturb_image/sliding_window.py` & `xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/sliding_window.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/interfaces/gen_classifier_conf_sal.py` & `xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_classifier_conf_sal.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/interfaces/gen_descriptor_sim_sal.py` & `xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_descriptor_sim_sal.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/interfaces/gen_detector_prop_sal.py` & `xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_detector_prop_sal.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/interfaces/gen_image_classifier_blackbox_sal.py` & `xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_image_classifier_blackbox_sal.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/interfaces/gen_image_similarity_blackbox_sal.py` & `xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_image_similarity_blackbox_sal.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/interfaces/gen_object_detector_blackbox_sal.py` & `xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_object_detector_blackbox_sal.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/interfaces/perturb_image.py` & `xaitk_saliency-0.7.0/xaitk_saliency/interfaces/perturb_image.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/utils/bin/sal_on_coco_dets.py` & `xaitk_saliency-0.7.0/xaitk_saliency/utils/bin/sal_on_coco_dets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import click  # type: ignore
 import os
 from PIL import Image  # type: ignore
 import json
-import matplotlib.pyplot as plt  # type: ignore
-from matplotlib.patches import Rectangle  # type: ignore
 import numpy as np
 from typing import TextIO
 import logging
 
 from smqtk_detection.interfaces.detect_image_objects import DetectImageObjects
 from smqtk_core.configuration import from_config_dict, make_default_config
 
 from xaitk_saliency import GenerateObjectDetectorBlackboxSaliency
 
 try:
     import kwcoco  # type: ignore
+    import matplotlib.pyplot as plt  # type: ignore
+    from matplotlib.patches import Rectangle  # type: ignore
     from xaitk_saliency.utils.coco import parse_coco_dset
     is_usable = True
 except ImportError:
     is_usable = False
 
 
 @click.command(context_settings={"help_option_names": ['-h', '--help']})
```

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/utils/coco.py` & `xaitk_saliency-0.7.0/xaitk_saliency/utils/coco.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/utils/detection.py` & `xaitk_saliency-0.7.0/xaitk_saliency/utils/detection.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/xaitk_saliency/utils/masking.py` & `xaitk_saliency-0.7.0/xaitk_saliency/utils/masking.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.6.1/PKG-INFO` & `xaitk_saliency-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 Metadata-Version: 2.1
 Name: xaitk-saliency
-Version: 0.6.1
+Version: 0.7.0
 Summary: Visual saliency map generation interfaces and baseline implementations for explainable AI.
 Home-page: https://github.com/XAITK/xaitk-saliency
 License: BSD-3-Clause
 Author: Kitware, Inc.
 Author-email: xaitk@kitware.com
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: example_deps
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: example-deps
 Provides-Extra: tools
-Requires-Dist: click (>=8.0.3,<9.0.0)
-Requires-Dist: jupyter (>=1.0.0,<2.0.0); extra == "example_deps"
-Requires-Dist: kwcoco (>=0.2.18,<0.3.0); extra == "tools"
-Requires-Dist: matplotlib (>=3.4.1,<4.0.0); extra == "example_deps"
-Requires-Dist: numpy (>=1.20.3,<2.0.0)
-Requires-Dist: papermill (>=2.3.3,<3.0.0); extra == "example_deps"
-Requires-Dist: scikit-image (>=0.18.1,<0.19.0)
-Requires-Dist: scikit-learn (>=0.24.2,<0.25.0)
-Requires-Dist: scipy (>=1.6.3,<2.0.0)
+Requires-Dist: click (>=8.0.3)
+Requires-Dist: jupyter (>=1.0.0) ; extra == "example-deps"
+Requires-Dist: kwcoco (>=0.2.18) ; extra == "tools"
+Requires-Dist: matplotlib (>=3.4.1) ; extra == "example-deps" or extra == "tools"
+Requires-Dist: numpy (>=1.22)
+Requires-Dist: papermill (>=2.3.3) ; extra == "example-deps"
+Requires-Dist: scikit-image (>=0.18.1) ; python_version < "3.11"
+Requires-Dist: scikit-image (>=0.20.0) ; python_version >= "3.11"
+Requires-Dist: scikit-learn (>=1.2)
+Requires-Dist: scipy (>=1.8.1)
+Requires-Dist: setuptools
 Requires-Dist: smqtk-classifier (>=0.17.0)
 Requires-Dist: smqtk-core (>=0.18.0)
 Requires-Dist: smqtk-descriptors (>=0.16.0)
-Requires-Dist: smqtk-detection (>=0.18.1)
-Requires-Dist: torch (>=1.9.0,<2.0.0); extra == "example_deps"
-Requires-Dist: torchvision (>=0.10.0,<0.11.0); extra == "example_deps"
-Requires-Dist: tqdm (>=4.45.0,<5.0.0); extra == "example_deps"
+Requires-Dist: smqtk-detection (>=0.19.0)
+Requires-Dist: torch (>=1.9.0,!=2.0.1) ; extra == "example-deps"
+Requires-Dist: torchvision (>=0.10.0) ; extra == "example-deps"
+Requires-Dist: tqdm (>=4.45.0) ; extra == "example-deps"
 Project-URL: Documentation, https://xaitk-saliency.readthedocs.io/
 Project-URL: Repository, https://github.com/XAITK/xaitk-saliency
 Description-Content-Type: text/markdown
 
 ![xaitk-logo](./docs/figures/xaitk-wordmark-light.png)
 
 <hr/>
```

