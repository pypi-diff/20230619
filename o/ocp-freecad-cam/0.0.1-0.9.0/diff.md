# Comparing `tmp/ocp-freecad-cam-0.0.1.tar.gz` & `tmp/ocp-freecad-cam-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp-freecad-cam-0.0.1.tar", last modified: Fri Jun 16 17:08:26 2023, max compression
+gzip compressed data, was "ocp-freecad-cam-0.9.0.tar", last modified: Mon Jun 19 21:00:36 2023, max compression
```

## Comparing `ocp-freecad-cam-0.0.1.tar` & `ocp-freecad-cam-0.9.0.tar`

### file list

```diff
@@ -1,53 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:08:26.000068 ocp-freecad-cam-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:08:25.996068 ocp-freecad-cam-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:08:25.996068 ocp-freecad-cam-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-16 17:08:26.000068 ocp-freecad-cam-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:08:25.996068 ocp-freecad-cam-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:08:25.996068 ocp-freecad-cam-0.0.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/docs/examples/cq_drill.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/docs/examples/cq_helix.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/docs/examples/cq_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/docs/examples/cq_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/docs/examples/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/docs/examples/generate_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:08:25.996068 ocp-freecad-cam-0.0.1/docs/examples/images/
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/docs/examples/images/cq_drill.png
--rw-r--r--   0 runner    (1001) docker     (123)    14948 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/docs/examples/images/cq_helix.png
--rw-r--r--   0 runner    (1001) docker     (123)    19952 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/docs/examples/images/cq_pocket.png
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/docs/examples/images/cq_profile.png
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 17:08:26.000068 ocp-freecad-cam-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:08:25.992068 ocp-freecad-cam-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:08:26.000068 ocp-freecad-cam-0.0.1/src/ocp_freecad_cam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/src/ocp_freecad_cam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/src/ocp_freecad_cam/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/src/ocp_freecad_cam/api_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/src/ocp_freecad_cam/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/src/ocp_freecad_cam/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/src/ocp_freecad_cam/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:08:26.000068 ocp-freecad-cam-0.0.1/src/ocp_freecad_cam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-16 17:08:25.000000 ocp-freecad-cam-0.0.1/src/ocp_freecad_cam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-16 17:08:25.000000 ocp-freecad-cam-0.0.1/src/ocp_freecad_cam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:08:25.000000 ocp-freecad-cam-0.0.1/src/ocp_freecad_cam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 17:08:25.000000 ocp-freecad-cam-0.0.1/src/ocp_freecad_cam.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:08:25.992068 ocp-freecad-cam-0.0.1/stubs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:08:26.000068 ocp-freecad-cam-0.0.1/stubs/Part/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/stubs/Part/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:08:26.000068 ocp-freecad-cam-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/tests/test_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-16 17:08:13.000000 ocp-freecad-cam-0.0.1/tests/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:00:36.928353 ocp-freecad-cam-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:00:36.924353 ocp-freecad-cam-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:00:36.924353 ocp-freecad-cam-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-19 21:00:36.928353 ocp-freecad-cam-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:00:36.924353 ocp-freecad-cam-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:00:36.924353 ocp-freecad-cam-0.9.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/docs/examples/cq_drill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/docs/examples/cq_helix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/docs/examples/cq_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/docs/examples/cq_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/docs/examples/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/docs/examples/generate_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:00:36.924353 ocp-freecad-cam-0.9.0/docs/examples/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/docs/examples/images/cq_drill.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14948 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/docs/examples/images/cq_helix.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19952 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/docs/examples/images/cq_pocket.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/docs/examples/images/cq_profile.png
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 21:00:36.928353 ocp-freecad-cam-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:00:36.920353 ocp-freecad-cam-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:00:36.928353 ocp-freecad-cam-0.9.0/src/ocp_freecad_cam/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/src/ocp_freecad_cam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33506 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/src/ocp_freecad_cam/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/src/ocp_freecad_cam/api_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/src/ocp_freecad_cam/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28152 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/src/ocp_freecad_cam/fc_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/src/ocp_freecad_cam/fc_impl_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/src/ocp_freecad_cam/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:00:36.928353 ocp-freecad-cam-0.9.0/src/ocp_freecad_cam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-19 21:00:36.000000 ocp-freecad-cam-0.9.0/src/ocp_freecad_cam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-19 21:00:36.000000 ocp-freecad-cam-0.9.0/src/ocp_freecad_cam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:00:36.000000 ocp-freecad-cam-0.9.0/src/ocp_freecad_cam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 21:00:36.000000 ocp-freecad-cam-0.9.0/src/ocp_freecad_cam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:00:36.920353 ocp-freecad-cam-0.9.0/stubs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:00:36.928353 ocp-freecad-cam-0.9.0/stubs/Part/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/stubs/Part/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:00:36.928353 ocp-freecad-cam-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/tests/test_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/tests/test_drill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/tests/test_engrave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/tests/test_helix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-19 21:00:22.000000 ocp-freecad-cam-0.9.0/tests/test_waterline.py
```

### Comparing `ocp-freecad-cam-0.0.1/.github/workflows/release.yml` & `ocp-freecad-cam-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.0.1/.readthedocs.yaml` & `ocp-freecad-cam-0.9.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.0.1/LICENSE` & `ocp-freecad-cam-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.0.1/docs/Makefile` & `ocp-freecad-cam-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.0.1/docs/conf.py` & `ocp-freecad-cam-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.0.1/docs/examples/examples.rst` & `ocp-freecad-cam-0.9.0/docs/examples/examples.rst`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.0.1/docs/examples/generate_image.py` & `ocp-freecad-cam-0.9.0/docs/examples/generate_image.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.0.1/docs/examples/images/cq_drill.png` & `ocp-freecad-cam-0.9.0/docs/examples/images/cq_drill.png`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.0.1/docs/examples/images/cq_helix.png` & `ocp-freecad-cam-0.9.0/docs/examples/images/cq_helix.png`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.0.1/docs/examples/images/cq_pocket.png` & `ocp-freecad-cam-0.9.0/docs/examples/images/cq_pocket.png`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.0.1/docs/examples/images/cq_profile.png` & `ocp-freecad-cam-0.9.0/docs/examples/images/cq_profile.png`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.0.1/pyproject.toml` & `ocp-freecad-cam-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.0.1/readme.md` & `ocp-freecad-cam-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.0.1/requirements-dev.txt` & `ocp-freecad-cam-0.9.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.0.1/src/ocp_freecad_cam/api.py` & `ocp-freecad-cam-0.9.0/src/ocp_freecad_cam/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,45 @@
 """
 This is the user facing API of ocp_freecad_cam
 """
-import io
 import logging
-import tempfile
+from copy import copy
 from typing import Literal, Optional
 
-import FreeCAD
-import Part
 import Path.Log as Log
 import PathScripts.PathUtils as PathUtils
-from OCP.BRepTools import BRepTools
-from OCP.TopoDS import TopoDS_Builder, TopoDS_Compound, TopoDS_Face, TopoDS_Shape
 from Path.Dressup import DogboneII, Tags
-from Path.Main import Job as FCJob
-from Path.Post.Command import buildPostList
-from Path.Post.Processor import PostProcessor
 from Path.Tool import Bit, Controller
 
 from ocp_freecad_cam.api_util import (
     AutoUnitKey,
     CompoundSource,
     ShapeSource,
     apply_params,
+    extract_plane,
     extract_topods_shapes,
     map_params,
-    scale_shape,
-    shape_source_to_compound_brep,
-    shape_to_brep,
-    transform_shape,
+    shape_source_to_compound,
 )
-from ocp_freecad_cam.common import FaceSource, Plane, PlaneSource
-from ocp_freecad_cam.operations import (
+from ocp_freecad_cam.common import PlaneSource, PostProcessor
+from ocp_freecad_cam.fc_impl import (
+    AdaptiveOp,
     DeburrOp,
     Dressup,
     DrillOp,
+    EngraveOp,
     FaceOp,
     HelixOp,
+    JobImpl,
     Op,
     PocketOp,
     ProfileOp,
-    Surface3DOp,
-    VCarveOp,
 )
-from ocp_freecad_cam.visualizer import visualize_fc_job
+from ocp_freecad_cam.fc_impl import Stock as StockImpl
+from ocp_freecad_cam.fc_impl import StockBase, Surface3DOp, VCarveOp, WaterlineOp
 
 try:
     import cadquery as cq
 except ImportError:
     cq = None
 try:
     import build123d as b3d
@@ -61,153 +53,76 @@
 
 
 class Job:
     def __init__(
         self,
         top_plane: PlaneSource,
         model: CompoundSource,
-        postprocessor: Literal[
-            "KineticNCBeamicon2",
-            "centroid",
-            "comparams",
-            "dxf",
-            "dynapath",
-            "fablin",
-            "fangling",
-            "fanuc",
-            "grbl",
-            "heidenhain",
-            "jtech",
-            "linuxcnc",
-            "mach3_mach4",
-            "marlin",
-            "nccad",
-            "opensbp",
-            "philips",
-            "refactored_centroid",
-            "refactored_grbl",
-            "refactored_linuxcnc",
-            "refactored_mach3_mach4",
-            "refactored_test",
-            "rml",
-            "rrf",
-            "smoothie",
-            "uccnc",
-        ] = None,
+        post_processor: PostProcessor = None,
         units: Literal["metric", "imperial"] = "metric",
         geometry_tolerance=None,
+        coolant_mode: Literal["None", "Flood", "Mist"] = "None",
+        final_depth_expression="OpFinalDepth",
+        start_depth_expression="OpStartDepth",
+        step_down_expression="OpToolDiameter",
+        clearance_height_expression="OpStockZMax+SetupSheet.ClearanceHeightOffset",
+        clearance_height_offset="5.00 mm",
+        safe_height_expression="OpStockZMax+SetupSheet.SafeHeightOffset",
+        safe_height_offset="3.00 mm",
+        stock: StockBase = StockImpl(),
     ):
-        self.top_plane = extract_plane(top_plane)
-
-        # Internal attributes
-        self.ops: list[Op] = []
-        self.fc_job = None
-        self._needs_build = True
-        self.doc = None
-        self.postprocessor = postprocessor
-        self.units = units
-
-        # FreeCAD attributes
-        self.geometry_tolerance = geometry_tolerance
-
-        # Prepare job model
         model_compounds = extract_topods_shapes(model, compound=True)
         if (model_count := len(model_compounds)) != 1:
             raise ValueError(
                 f"Job should be based around a single compound (got {model_count})"
             )
-        transformed_job_model = transform_shape(model_compounds[0], self._forward_trsf)
-        if sf := self._scale_factor:
-            transformed_job_model = scale_shape(transformed_job_model, sf)
-
-        self.job_obj_brep = shape_to_brep(transformed_job_model)
-
-    @property
-    def _scale_factor(self):
-        if self.units == "metric":
-            return None
-        elif self.units == "imperial":
-            return 25.4
-        raise ValueError(f"Unknown unit: ({self.units})")
-
-    def _build(self):
-        if self.doc:
-            FreeCAD.closeDocument(self.doc)
-
-        self.doc = FreeCAD.newDocument("ocp_freecad_cam")
-        self.set_active()
-        fc_compound = Part.Compound()
-        fc_compound.importBrepFromString(self.job_obj_brep)
-        feature = self.doc.addObject("Part::Feature", f"root_brep")
-        feature.Shape = fc_compound
-
-        job = FCJob.Create("Job", [feature])
-        self.job = job
-        self.fc_job = job.Proxy
-
-        # Remove default tools as we'll create our own later
-        # Necessary also because of  buggy FX implementation
-        tools = [tool for tool in self.job.Tools.Group]
-        for tool in tools:
-            self.job.Tools.removeObject(tool)
-        if self.postprocessor:
-            job.PostProcessor = self.postprocessor
-        job.Stock.ExtZpos = 0
-        job.Stock.ExtZneg = 0
-
-        for op in self.ops:
-            op.execute(self.doc)
-
-        self.doc.recompute()
-        self._needs_build = False
-
-    def show(self):
-        if self._needs_build:
-            self._build()
-
-        return visualize_fc_job(self.job, reverse_transform_tsrf(self.top_plane))
 
-    def to_gcode(self):
-        if self.postprocessor is None:
-            raise ValueError(
-                "No postprocessor set - set Job postprocessor to a valid value"
-            )
-        if self._needs_build:
-            self._build()
+        self.job_impl = JobImpl(
+            top=extract_plane(top_plane),
+            model=model_compounds[0],
+            post_processor=post_processor,
+            units=units,
+            geometry_tolerance=geometry_tolerance,
+            coolant_mode=coolant_mode,
+            final_depth_expression=final_depth_expression,
+            start_depth_expression=start_depth_expression,
+            step_down_expression=step_down_expression,
+            clearance_height_expression=clearance_height_expression,
+            clearance_height_offset=clearance_height_offset,
+            safe_height_expression=safe_height_expression,
+            safe_height_offset=safe_height_offset,
+            stock=stock,
+        )
 
-        job = self.job
-        postlist = buildPostList(job)
-        processor = PostProcessor.load(job.PostProcessor)
-
-        for idx, section in enumerate(postlist):
-            name, sublist = section
-            with tempfile.NamedTemporaryFile() as tmp_file:
-                options = ["--no-show-editor"]
-                if self.units == "imperial":
-                    options.append("--inches")
-
-                gcode = processor.export(sublist, tmp_file.name, " ".join(options))
-                return gcode
-
-    def save_fcstd(self, filename="debug.fcstd"):
-        if self._needs_build:
-            self._build()
+        self._needs_rebuild = True
 
-        self.doc.saveAs(filename)
+    def show(self, force_rebuild=False):
+        ais = self.job_impl.show(rebuild=self._needs_rebuild or force_rebuild)
+        self._needs_rebuild = False
+        return ais
+
+    def to_gcode(self, force_rebuild=False):
+        gcode = self.job_impl.to_gcode(rebuild=self._needs_rebuild or force_rebuild)
+        self._needs_rebuild = False
+        return gcode
+
+    def save_fcstd(self, filename="debug.fcstd", force_rebuild=False):
+        rv = self.job_impl.save_fcstd(
+            filename, rebuild=self._needs_rebuild or force_rebuild
+        )
+        self._needs_rebuild = False
+        return rv
 
     def _add_op(self, op: Op):
-        self._needs_build = True
-        self.ops.append(op)
-
-    def set_active(self):
-        FreeCAD.setActiveDocument(self.doc.Name)
-
-    @property
-    def _forward_trsf(self):
-        return forward_transform_tsrf(self.top_plane)
+        new_ops = self.job_impl.ops[:]
+        new_ops.append(op)
+        new_job = copy(self)
+        new_job.job_impl = new_job.job_impl.copy(new_ops)
+        new_job._needs_rebuild = True
+        return new_job
 
     def profile(
         self,
         shapes: ShapeSource,
         tool: "Toolbit",
         *,
         side: Literal["out", "in", "mid"] = "out",
@@ -216,14 +131,20 @@
             "collectively", "individually"
         ] = "collectively",
         offset_extra: float = 0.0,
         circles: bool = False,
         holes: bool = False,
         perimeter: bool = True,
         dressups: list["Dressup"] = None,
+        # OP depth
+        clearance_height=None,
+        final_depth=None,
+        safe_height=None,
+        start_depth=None,
+        step_down=None,
     ):
         """
         2.5D profile operation will operate on faces, wires and edges.
 
         Edges do not have to form a closed loop, and they do not have to be
         on the same Z-level. See https://wiki.freecad.org/Path_Profile
         for usage notes.
@@ -248,45 +169,51 @@
         use_comp = side != "mid"
         if not use_comp:
             # Side is irrelevant if we're not using cutter radius compensation
             # Set to some valid value
             side = "out"
 
         op = ProfileOp(
-            self,
             # Profile settings
             side=side,
             direction=direction,
             handle_multiple_features=handle_multiple_features,
             offset_extra=offset_extra,
             use_comp=use_comp,
             process_circles=circles,
             process_holes=holes,
             process_perimeter=perimeter,
             # Op settings
             tool=tool,
             dressups=dressups or [],
-            **shape_source_to_compound_brep(
-                shapes, self._forward_trsf, self._scale_factor
-            ),
+            compound_data=shape_source_to_compound(shapes),
+            clearance_height=clearance_height,
+            final_depth=final_depth,
+            safe_height=safe_height,
+            start_depth=start_depth,
+            step_down=step_down,
         )
-        self._add_op(op)
-        return self
+        return self._add_op(op)
 
     def face(
         self,
         shapes: ShapeSource,
         tool: "Toolbit",
         *,
         finish_depth: float,
         boundary: Literal["boundbox", "face", "perimeter", "stock"],
         clear_edges: bool,
         exclude_raised: bool,
         pattern: Literal["zigzag", "offset", "zigzag_offset", "line", "grid"],
-        **kwargs,
+        # OP depth
+        clearance_height=None,
+        final_depth=None,
+        safe_height=None,
+        start_depth=None,
+        step_down=None,
     ) -> "Job":
         """
         2.5D face operation to clear material from a surface
 
         :param shapes:
         :param tool:
         :param finish_depth:
@@ -295,28 +222,30 @@
         :param exclude_raised:
         :param pattern:
         :param kwargs:
         :return:
         """
 
         op = FaceOp(
-            self,
             finish_depth=finish_depth,
             boundary=boundary,
             clear_edges=clear_edges,
             exclude_raised=exclude_raised,
             pattern=pattern,
             tool=tool,
-            **shape_source_to_compound_brep(
-                shapes, self._forward_trsf, self._scale_factor
+            compound_data=shape_source_to_compound(
+                shapes,
             ),
-            **kwargs,
+            clearance_height=clearance_height,
+            final_depth=final_depth,
+            safe_height=safe_height,
+            start_depth=start_depth,
+            step_down=step_down,
         )
-        self._add_op(op)
-        return self
+        return self._add_op(op)
 
     def pocket(
         self,
         shapes: ShapeSource,
         tool: "Toolbit",
         *,
         finish_depth: float = 0,
@@ -329,14 +258,20 @@
         min_travel: bool = False,
         pocket_last_stepover: float = 0,
         start_at: Literal["center", "edge"] = "center",
         step_over: float = 100,
         use_outline: bool = False,
         zigzag_angle: float = 45.0,
         dressups: list[Dressup] = None,
+        # OP depth
+        clearance_height=None,
+        final_depth=None,
+        safe_height=None,
+        start_depth=None,
+        step_down=None,
     ) -> "Job":
         """
         2.5D pocket operation.
 
         https://wiki.freecad.org/Path_Pocket_Shape
 
         :param shapes: Shape(s) to perform this OP on.
@@ -354,157 +289,206 @@
         :param use_outline: Use outline of base geometry
         :param zigzag_angle: Valid when zigzagging
         :param dressups: Dressup operations
         :return:
         """
 
         op = PocketOp(
-            self,
             finish_depth=finish_depth,
             pattern=pattern,
             cut_mode=cut_mode,
             extra_offset=extra_offset,
             keep_tool_down=keep_tool_down,
             min_travel=min_travel,
             pocket_last_stepover=pocket_last_stepover,
             start_at=start_at,
             step_over=step_over,
             use_outline=use_outline,
             zigzag_angle=zigzag_angle,
             # OP settings
             tool=tool,
             dressups=dressups or [],
-            **shape_source_to_compound_brep(
-                shapes, self._forward_trsf, self._scale_factor
-            ),
+            compound_data=shape_source_to_compound(shapes),
+            clearance_height=clearance_height,
+            final_depth=final_depth,
+            safe_height=safe_height,
+            start_depth=start_depth,
+            step_down=step_down,
         )
-        self._add_op(op)
-        return self
+        return self._add_op(op)
 
     def drill(
         self,
         shapes: ShapeSource,
         tool: "Toolbit",
         dwell_time: Optional[float] = None,
         extra_offset: Optional[Literal["none", "1x", "2x"]] = "none",
         peck_depth: Optional[float] = None,
         keep_tool_down: Optional[bool] = False,
         retract_height: Optional[bool] = None,
         chip_break_enabled: Optional[bool] = False,
-        **kwargs,
+        # OP depth
+        clearance_height=None,
+        final_depth=None,
+        safe_height=None,
+        start_depth=None,
+        step_down=None,
     ):
         """
         Drilling OP works at least on circular edges and cylindrical
         faces.
 
         :param shapes: shapes to perform this op on
         :param tool: tool to use
         :param dwell_time: setting this to any value will enable dwell
         :param extra_offset: extend drilling depth
         :param peck_depth:
         :param keep_tool_down:
         :param retract_height:
         :param chip_break_enabled:
-        :param kwargs:
         :return:
         """
 
         op = DrillOp(
-            self,
             tool=tool,
             dwell_time=dwell_time,
             extra_offset=extra_offset,
             peck_depth=peck_depth,
             keep_tool_down=keep_tool_down,
             retract_height=retract_height,
             chip_break_enabled=chip_break_enabled,
-            **shape_source_to_compound_brep(
-                shapes, self._forward_trsf, self._scale_factor
-            ),
-            **kwargs,
+            compound_data=shape_source_to_compound(shapes),
+            clearance_height=clearance_height,
+            final_depth=final_depth,
+            safe_height=safe_height,
+            start_depth=start_depth,
+            step_down=step_down,
         )
-        self._add_op(op)
-        return self
+        return self._add_op(op)
 
     def helix(
         self,
         shapes: ShapeSource,
         tool: "Toolbit",
         *,
         direction: Optional[Literal["cw", "ccw"]] = "cw",
         offset_extra: Optional[float] = 0,
         start_radius: Optional[float] = 0,
         start_side: Optional[Literal["out", "in"]] = "out",
         step_over: Optional[float] = 50,
-        **kwargs,
+        # OP depth
+        clearance_height=None,
+        final_depth=None,
+        safe_height=None,
+        start_depth=None,
+        step_down=None,
     ):
         """
         Perform a helix plunge.
 
         :param shapes: circular shapes to perform the op on
         :param tool: tool to use
         :param direction: default clockwise helix
         :param offset_extra: negative value creates a roughing pass followed
             by a final pass with the original radius
         :param start_radius: inner radius?
         :param start_side: define where the op starts when doing multiple passes
         :param step_over: percentage of tool diameter to step over
-        :param kwargs:
         :return:
         """
 
         op = HelixOp(
-            self,
             direction=direction,
             offset_extra=offset_extra,
             start_radius=start_radius,
             start_side=start_side,
             step_over=step_over,
             # Op
             tool=tool,
-            **shape_source_to_compound_brep(
-                shapes, self._forward_trsf, self._scale_factor
+            compound_data=shape_source_to_compound(
+                shapes,
             ),
-            **kwargs,
+            clearance_height=clearance_height,
+            final_depth=final_depth,
+            safe_height=safe_height,
+            start_depth=start_depth,
+            step_down=step_down,
         )
-        self._add_op(op)
-        return self
+        return self._add_op(op)
 
     def deburr(
         self,
         shapes: ShapeSource,
         tool: "Toolbit",
         *,
         width: float | str = "1 mm",
         extra_depth: float | str = "0.5 mm",
         direction: Literal["cw", "ccw"] = "cw",
         entry_point: int = 0,
+        # OP depth
+        clearance_height=None,
+        final_depth=None,
+        safe_height=None,
+        start_depth=None,
+        step_down=None,
     ):
         op = DeburrOp(
-            self,
             width=width,
             extra_depth=extra_depth,
             direction=direction,
             entry_point=entry_point,
             # Op
             tool=tool,
-            **shape_source_to_compound_brep(
-                shapes, self._forward_trsf, self._scale_factor
-            ),
+            compound_data=shape_source_to_compound(shapes),
+            clearance_height=clearance_height,
+            final_depth=final_depth,
+            safe_height=safe_height,
+            start_depth=start_depth,
+            step_down=step_down,
         )
-        self._add_op(op)
-        return self
+        return self._add_op(op)
+
+    def engrave(
+        self,
+        shapes: ShapeSource,
+        tool: "Toolbit",
+        *,
+        start_vertex: int = 0,
+        # OP depth
+        clearance_height=None,
+        final_depth=None,
+        safe_height=None,
+        start_depth=None,
+        step_down=None,
+    ):
+        op = EngraveOp(
+            start_vertex=start_vertex,
+            tool=tool,
+            compound_data=shape_source_to_compound(shapes),
+            clearance_height=clearance_height,
+            final_depth=final_depth,
+            safe_height=safe_height,
+            start_depth=start_depth,
+            step_down=step_down,
+        )
+        return self._add_op(op)
 
     def v_carve(
         self,
         shapes: ShapeSource,
         tool: "Toolbit",
         *,
         discretize: float = 0.01,
         colinear: float = 10.0,
+        # OP depth
+        clearance_height=None,
+        final_depth=None,
+        safe_height=None,
+        start_depth=None,
+        step_down=None,
     ):
         """
         V-Carve based on voronoi diagrams.
 
         Verify the tool path carefully! This algorithm is sometimes
         unstable.
 
@@ -512,25 +496,26 @@
         :param tool:
         :param discretize: Try a smaller value if getting too many retracts.
         :param colinear:
         :return:
         """
 
         op = VCarveOp(
-            self,
             discretize=discretize,
             colinear=colinear,
             # Op
             tool=tool,
-            **shape_source_to_compound_brep(
-                shapes, self._forward_trsf, self._scale_factor
-            ),
+            compound_data=shape_source_to_compound(shapes),
+            clearance_height=clearance_height,
+            final_depth=final_depth,
+            safe_height=safe_height,
+            start_depth=start_depth,
+            step_down=step_down,
         )
-        self._add_op(op)
-        return self
+        return self._add_op(op)
 
     def surface(
         self,
         shapes: Optional[ShapeSource],
         tool: "Toolbit",
         *,
         bound_box: Literal["base_bound_box", "stock"] = "base_bound_box",
@@ -557,17 +542,22 @@
         boundary_adjustment: float | str = 0,
         boundary_enforcement: bool = True,
         multiple_features: Literal["collectively", "individually"] = "collectively",
         internal_features_adjustment: float | str = 0,
         internal_features_cut: bool = True,
         start_point: tuple[float | str, float | str, float | str] = None,
         scan_type: Literal["planar", "rotational"] = "planar",
+        # OP depth
+        clearance_height=None,
+        final_depth=None,
+        safe_height=None,
+        start_depth=None,
+        step_down=None,
     ):
         op = Surface3DOp(
-            self,
             bound_box=bound_box,
             cut_mode=cut_mode,
             cut_pattern=cut_pattern,
             cut_pattern_angle=cut_pattern_angle,
             cut_pattern_reversed=cut_pattern_reversed,
             depth_offset=depth_offset,
             layer_mode=layer_mode,
@@ -587,123 +577,116 @@
             multiple_features=multiple_features,
             internal_features_adjustment=internal_features_adjustment,
             internal_features_cut=internal_features_cut,
             start_point=start_point,
             scan_type=scan_type,
             # Op
             tool=tool,
-            **shape_source_to_compound_brep(
-                shapes, self._forward_trsf, self._scale_factor, allow_none=True
-            ),
+            compound_data=shape_source_to_compound(shapes, allow_none=True),
+            clearance_height=clearance_height,
+            final_depth=final_depth,
+            safe_height=safe_height,
+            start_depth=start_depth,
+            step_down=step_down,
         )
-        self._add_op(op)
-        return self
-
-
-def extract_plane(plane_source: PlaneSource) -> Plane:
-    if cq:
-        # ace.transformShape(job.top.fG)
-        if isinstance(plane_source, cq.Workplane):
-            return plane_source.plane
-
-        elif isinstance(plane_source, cq.Plane):
-            return plane_source
-
-        elif isinstance(plane_source, cq.Face):
-            gp_pln = plane_source.toPln()
-            ax3 = gp_pln.Position()
-            origin = cq.Vector(ax3.Location())
-            x_dir = cq.Vector(ax3.XDirection())
-            normal = cq.Vector(ax3.Direction())
-            return cq.Plane(origin, x_dir, normal)
-
-    if b3d:
-        if isinstance(plane_source, b3d.Plane):
-            return plane_source
-        elif isinstance(plane_source, b3d.Face):
-            return b3d.Plane(face=plane_source)
-
-    raise ValueError(f"Unknown type of plane: {type(plane_source)}")
-
-
-def forward_transform(plane: Plane, shape: TopoDS_Shape) -> TopoDS_Shape:
-    if cq and isinstance(plane, cq.Plane):
-        return cq.Shape(shape).transformShape(plane.fG).wrapped
-
-    elif b3d and isinstance(plane, b3d.Plane):
-        return plane.to_local_coords(b3d.Shape(shape)).wrapped
-
-    raise ValueError(f"Unknown type of plane: {type(plane)}")
-
-
-def reverse_transform(plane: Plane, shape: TopoDS_Shape) -> TopoDS_Shape:
-    if cq and isinstance(plane, cq.Plane):
-        return cq.Shape(shape).transformShape(plane.rG).wrapped
-
-    elif b3d and isinstance(plane, b3d.Plane):
-        return plane.from_local_coords(b3d.Shape(shape).wrapped)
-
-    raise ValueError(f"Unknown type of plane: {type(plane)}")
-
-
-def forward_transform_tsrf(plane: Plane):
-    if cq and isinstance(plane, cq.Plane):
-        return plane.fG.wrapped.Trsf()
-
-    elif b3d and isinstance(plane, b3d.Plane):
-        return plane.forward_transform.wrapped.Trsf()
-
-    raise ValueError(f"Unknown type of plane: {type(plane)}")
-
-
-def reverse_transform_tsrf(plane: Plane):
-    if cq and isinstance(plane, cq.Plane):
-        return plane.rG.wrapped.Trsf()
-
-    elif b3d and isinstance(plane, b3d.Plane):
-        return plane.reverse_transform.wrapped.Trsf()
-
-    raise ValueError(f"Unknown type of plane: {type(plane)}")
-
-
-def extract_faces(face_source: FaceSource) -> list[TopoDS_Face]:
-    if isinstance(face_source, list):
-        faces = []
-        for element in face_source:
-            faces += extract_faces(element)
-        return faces
-
-    if cq:
-        if isinstance(face_source, cq.Workplane):
-            return [f.wrapped for f in face_source.objects if isinstance(f, cq.Face)]
-        elif isinstance(face_source, cq.Face):
-            return [face_source.wrapped]
-    if b3d:
-        if isinstance(face_source, b3d.Face):
-            return [face_source.wrapped]
-
-    raise ValueError(f"Unknown type of face: {type(face_source)}")
-
-
-def shapes_to_compound(shapes: list[TopoDS_Shape]) -> TopoDS_Compound:
-    comp = TopoDS_Compound()
-    comp_builder = TopoDS_Builder()
-    comp_builder.MakeCompound(comp)
-
-    for s in shapes:
-        comp_builder.Add(comp, s)
-
-    return comp
+        return self._add_op(op)
 
+    def waterline(
+        self,
+        shapes: Optional[ShapeSource],
+        tool: "Toolbit",
+        *,
+        algorithm: Literal["ocl", "experimental"] = "ocl",
+        bound_box: Literal["base", "stock"] = "base",
+        cut_mode: Literal["climb", "conventional"] = "climb",
+        depth_offset: float | str = 0,
+        layer_mode: Literal["single", "multi"] = "single",
+        sample_interval: float | str = "1.00 mm",
+        angular_deflection: float | str = "0.25 mm",
+        linear_deflection: float | str = "0.01 mm",
+        # OP depth
+        clearance_height=None,
+        final_depth=None,
+        safe_height=None,
+        start_depth=None,
+        step_down=None,
+    ):
+        op = WaterlineOp(
+            algorithm=algorithm,
+            bound_box=bound_box,
+            cut_mode=cut_mode,
+            depth_offset=depth_offset,
+            layer_mode=layer_mode,
+            sample_interval=sample_interval,
+            angular_deflection=angular_deflection,
+            linear_deflection=linear_deflection,
+            # Op
+            tool=tool,
+            compound_data=shape_source_to_compound(shapes, allow_none=True),
+            clearance_height=clearance_height,
+            final_depth=final_depth,
+            safe_height=safe_height,
+            start_depth=start_depth,
+            step_down=step_down,
+        )
+        return self._add_op(op)
 
-def to_brep(shape: TopoDS_Shape):
-    data = io.BytesIO()
-    BRepTools.Write_s(shape, data)
-    data.seek(0)
-    return data.read().decode("utf8")
+    def adaptive(
+        self,
+        shapes: Optional[ShapeSource],
+        tool: "Toolbit",
+        *,
+        finishing_profile: bool = True,
+        force_inside_cut: bool = False,
+        helix_angle: float = 5,
+        helix_cone_angle: float = 0,
+        helix_diameter_limit: float | str = 0,
+        keep_tool_down_ratio: float | str = "3.00 mm",
+        lift_distance: float | str = 0,
+        operation_type: Literal["clearing", "profiling"] = "clearing",
+        side: Literal["in", "out"] = "in",
+        step_over: float = 20,
+        stock_to_leave: float | str = 0,
+        tolerance: float = 0.1,
+        use_helix_arcs: bool = False,
+        use_outline: bool = False,
+        # OP depth
+        clearance_height=None,
+        final_depth=None,
+        safe_height=None,
+        start_depth=None,
+        step_down=None,
+    ):
+        op = AdaptiveOp(
+            finishing_profile=finishing_profile,
+            force_inside_cut=force_inside_cut,
+            helix_angle=helix_angle,
+            helix_cone_angle=helix_cone_angle,
+            helix_diameter_limit=helix_diameter_limit,
+            keep_tool_down_ratio=keep_tool_down_ratio,
+            lift_distance=lift_distance,
+            operation_type=operation_type,
+            side=side,
+            step_over=step_over,
+            stock_to_leave=stock_to_leave,
+            tolerance=tolerance,
+            use_helix_arcs=use_helix_arcs,
+            use_outline=use_outline,
+            # Op
+            tool=tool,
+            compound_data=shape_source_to_compound(
+                shapes,
+            ),
+            clearance_height=clearance_height,
+            final_depth=final_depth,
+            safe_height=safe_height,
+            start_depth=start_depth,
+            step_down=step_down,
+        )
+        return self._add_op(op)
 
 
 class Toolbit:
     props: dict
     _prop_mapping = {}
 
     def __init__(self, tool_name: str, tool_file_name: str, tool_number=1, path=None):
@@ -822,14 +805,18 @@
             length=length,
             shank_diameter=shank_diameter,
             tip_angle=tip_angle,
             tip_diameter=tip_diameter,
         )
 
 
+class Chamfer(VBit):
+    _file_name = "chamfer.fcstd"
+
+
 class Drill(Toolbit):
     _file_name = "drill.fcstd"
     _prop_mapping = {
         "chip_load": "ChipLoad",
         "flutes": "Flutes",
         "material": "Material",
         "diameter": AutoUnitKey("Diameter"),
@@ -860,16 +847,167 @@
             material=material,
             diameter=diameter,
             length=length,
             tip_angle=tip_angle,
         )
 
 
+class Probe(Toolbit):
+    _file_name = "probe.fcstd"
+    _prop_mapping = {
+        "diameter": AutoUnitKey("Diameter"),
+        "length": AutoUnitKey("Length"),
+        "shank_diameter": AutoUnitKey("Shank Diameter"),
+    }
+
+    def __init__(
+        self,
+        tool_name: str = "",
+        # Bit specific
+        diameter=None,
+        length=None,
+        shank_diameter=None,
+        # TC
+        tool_number: int = 1,
+    ):
+        super().__init__(tool_name, self._file_name, tool_number=tool_number)
+
+        self.props = map_params(
+            self._prop_mapping,
+            diameter=diameter,
+            length=length,
+            shank_diameter=shank_diameter,
+        )
+
+
+class SlittingSaw(Toolbit):
+    _file_name = "slittingsaw.fcstd"
+    _prop_mapping = {
+        "blade_thickness": AutoUnitKey("BladeThickness"),
+        "cap_diameter": AutoUnitKey("CapDiameter"),
+        "cap_height": AutoUnitKey("CapHeight"),
+        "diameter": AutoUnitKey("Diameter"),
+        "length": AutoUnitKey("Length"),
+        "shank_diameter": AutoUnitKey("Shank Diameter"),
+    }
+
+    def __init__(
+        self,
+        tool_name: str = "",
+        # Bit specific
+        blade_thickness=None,
+        cap_diameter=None,
+        cap_height=None,
+        diameter=None,
+        length=None,
+        shank_diameter=None,
+        # TC
+        tool_number: int = 1,
+    ):
+        super().__init__(tool_name, self._file_name, tool_number=tool_number)
+
+        self.props = map_params(
+            self._prop_mapping,
+            blade_thickness=blade_thickness,
+            cap_diameter=cap_diameter,
+            cap_height=cap_height,
+            diameter=diameter,
+            length=length,
+            shank_diameter=shank_diameter,
+        )
+
+
 class Bullnose(Endmill):
-    pass
+    _file_name = "bullnose.fcstd"
+    _prop_mapping = {
+        **Endmill._prop_mapping,
+        "flat_radius": AutoUnitKey("FlatRadius"),
+    }
+
+    def __init__(
+        self,
+        tool_name: str = "",
+        # Generic
+        chip_load=None,
+        flutes=None,
+        material=None,
+        spindle_direction=None,
+        # Bit specific
+        cutting_edge_height=None,
+        diameter=None,
+        length=None,
+        shank_diameter=None,
+        flat_radius=None,
+        # TC
+        tool_number: int = 1,
+    ):
+        super().__init__(tool_name, self._file_name, tool_number=tool_number)
+        self.props = map_params(
+            self._prop_mapping,
+            chip_load=chip_load,
+            flutes=flutes,
+            material=material,
+            spindle_direction=spindle_direction,
+            cutting_edge_height=cutting_edge_height,
+            diameter=diameter,
+            length=length,
+            shank_diameter=shank_diameter,
+            flat_radius=flat_radius,
+        )
+
+
+class ThreadMill(Toolbit):
+    _file_name = "bullnose.fcstd"
+    _prop_mapping = {
+        "chip_load": "ChipLoad",
+        "flutes": "Flutes",
+        "material": "Material",
+        "crest": AutoUnitKey("Crest"),
+        "diameter": AutoUnitKey("Diameter"),
+        "length": AutoUnitKey("Length"),
+        "neck_diameter": AutoUnitKey("NeckDiameter"),
+        "neck_length": AutoUnitKey("NeckLength"),
+        "shank_diameter": AutoUnitKey("ShankDiameter"),
+        "cutting_angle": "cuttingAngle",
+    }
+
+    def __init__(
+        self,
+        tool_name: str = "",
+        # Generic
+        chip_load=None,
+        flutes=None,
+        material=None,
+        spindle_direction=None,
+        # Bit specific
+        crest=None,
+        diameter=None,
+        length=None,
+        neck_diameter=None,
+        neck_length=None,
+        shank_diameter=None,
+        cutting_angle=None,
+        # TC
+        tool_number: int = 1,
+    ):
+        super().__init__(tool_name, self._file_name, tool_number=tool_number)
+        self.props = map_params(
+            self._prop_mapping,
+            chip_load=chip_load,
+            flutes=flutes,
+            material=material,
+            spindle_direction=spindle_direction,
+            crest=crest,
+            diameter=diameter,
+            length=length,
+            neck_diameter=neck_diameter,
+            neck_length=neck_length,
+            shank_diameter=shank_diameter,
+            cutting_angle=cutting_angle,
+        )
 
 
 class Dogbone(Dressup):
     factory = DogboneII
     mapping = {
         "incision": "Incision",
         "custom": "Custom",
@@ -933,7 +1071,10 @@
             height=height,
             width=width,
             positions=positions,
             disabled=disabled,
             fillet_radius=fillet_radius,
             segmentation_factor=segmentation_factor,
         )
+
+
+Stock = StockImpl
```

### Comparing `ocp-freecad-cam-0.0.1/src/ocp_freecad_cam/api_util.py` & `ocp-freecad-cam-0.9.0/src/ocp_freecad_cam/api_util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import io
+from dataclasses import dataclass
 from typing import Literal, Optional, TypeAlias, Union
 
 import FreeCAD
 import Path.Base.Util as PathUtil
 from OCP.BRepBuilderAPI import BRepBuilderAPI_Transform
 from OCP.BRepTools import BRepTools
-from OCP.gp import gp_Pnt, gp_Trsf
+from OCP.gp import gp_Ax3, gp_GTrsf, gp_Pln, gp_Pnt, gp_Trsf
 from OCP.TopAbs import TopAbs_EDGE, TopAbs_FACE, TopAbs_ShapeEnum
 from OCP.TopExp import TopExp_Explorer
 from OCP.TopoDS import (
     TopoDS_Builder,
     TopoDS_Compound,
     TopoDS_Edge,
     TopoDS_Face,
     TopoDS_Shape,
     TopoDS_Solid,
     TopoDS_Vertex,
     TopoDS_Wire,
 )
 
+from ocp_freecad_cam.common import PlaneSource
+
 try:
     import cadquery as cq
 except ImportError:
     cq = None
 try:
     import build123d as b3d
 except ImportError:
@@ -219,14 +222,63 @@
         "face_count": len(faces),
         "edge_count": len(edges),
         "vertex_count": len(vertices),
         "compound_brep": shape_to_brep(compound),
     }
 
 
+@dataclass
+class CompoundData:
+    face_count: int
+    edge_count: int
+    vertex_count: int
+    compound: Optional[TopoDS_Compound]
+
+    def to_transformed_brep(
+        self, trsf: gp_Trsf, scale_factor: float = None
+    ) -> Optional[str]:
+        if self.compound is None:
+            return None
+        compound = transform_shape(self.compound, trsf)
+        if scale_factor:
+            compound = scale_shape(compound, scale_factor)
+        return shape_to_brep(compound)
+
+
+def shape_source_to_compound(
+    shape_source: ShapeSourceOrIterable,
+    allow_none=False,
+) -> CompoundData:
+    if allow_none and shape_source is None:
+        return CompoundData(0, 0, 0, None)
+
+    shapes = extract_topods_shapes(shape_source)
+    if not shapes:
+        shapes = extract_topods_shapes(shape_source, True)
+    faces, edges, vertices = split_shapes_by_type(shapes)
+
+    if not faces and not edges and not vertices:
+        raise ValueError("Empty ShapeSource")
+
+    compound = TopoDS_Compound()
+    builder = TopoDS_Builder()
+    builder.MakeCompound(compound)
+
+    for face in faces:
+        builder.Add(compound, face)
+
+    for edge in edges:
+        builder.Add(compound, edge)
+
+    for vertex in vertices:
+        builder.Add(compound, vertex)
+
+    return CompoundData(len(faces), len(edges), len(vertices), compound)
+
+
 class AutoUnitKey:
     def __init__(self, key):
         self.key = key
 
 
 class AutoUnitValue:
     def __init__(self, value):
@@ -247,14 +299,19 @@
 
         elif isinstance(value, tuple):
             return tuple(self._convert(v, unit) for v in value)
 
         return float(pq(value))
 
 
+class Expression:
+    def __init__(self, expression):
+        self.expression = expression
+
+
 ParamMapping: TypeAlias = dict[str, Union[str, AutoUnitKey, dict[str, str]]]
 
 
 def map_prop(mapping: ParamMapping, k, v):
     result = mapping[k]
     match result:
         case AutoUnitKey():
@@ -269,8 +326,31 @@
     return dict(map_prop(mapping, k, v) for k, v in kwargs.items() if v is not None)
 
 
 def apply_params(fc_obj, params, unit: Literal["metric", "imperial"]):
     for k, v in params.items():
         if isinstance(v, AutoUnitValue):
             v = v.convert(unit)
-        PathUtil.setProperty(fc_obj, k, v)
+        if isinstance(v, Expression):
+            fc_obj.setExpression(k, v)
+        else:
+            PathUtil.setProperty(fc_obj, k, v)
+
+
+def extract_plane(plane_source: PlaneSource) -> gp_Pln:
+    if cq:
+        if isinstance(plane_source, cq.Workplane):
+            return plane_source.plane.toPln()
+
+        elif isinstance(plane_source, (cq.Plane, cq.Face)):
+            return plane_source.toPln()
+
+    if b3d:
+        if isinstance(plane_source, b3d.Plane):
+            return plane_source.wrapped
+        elif isinstance(plane_source, b3d.Face):
+            return b3d.Plane(face=plane_source).wrapped
+
+    if isinstance(plane_source, gp_Pln):
+        return plane_source
+
+    raise ValueError(f"Unknown type of plane: {type(plane_source)}")
```

### Comparing `ocp-freecad-cam-0.0.1/src/ocp_freecad_cam/visualizer.py` & `ocp-freecad-cam-0.9.0/src/ocp_freecad_cam/visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class VisualCommand(ABC):
     def __init__(self, *, x, y, z, **kwargs):
         self.x = x
         self.y = y
         self.z = z
 
     def to_ais(self, start: "VisualCommand"):
-        raise NotImplemented
+        raise NotImplementedError
 
     def __eq__(self, other):
         if isinstance(other, VisualCommand):
             return self.x == other.x and self.y == other.y and self.z == other.z
         raise TypeError(f"Can not compare {type(self)} with {type(other)}")
 
 
@@ -61,19 +61,19 @@
         super().__init__(**kwargs)
         self.arc_plane = arc_plane
         self.i = i
         self.j = j
         self.k = k
 
     def circle_normal_dir(self, circle_normal: gp_Vec):
-        raise NotImplemented
+        raise NotImplementedError
 
     @property
     def clockwise(self):
-        raise NotImplemented
+        raise NotImplementedError
 
     def to_ais(self, start: VisualCommand):
         if self.arc_plane == (0, 0, 1):
             if self.i is None or self.j is None:
                 raise ValueError("I and J must be defined for XY arc")
             cx = start.x + self.i
             cy = start.y + self.j
```

### Comparing `ocp-freecad-cam-0.0.1/src/ocp_freecad_cam.egg-info/SOURCES.txt` & `ocp-freecad-cam-0.9.0/src/ocp_freecad_cam.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 .gitignore
 .readthedocs.yaml
 LICENSE
+README.md
 pyproject.toml
 pytest.ini
-readme.md
 requirements-dev.in
 requirements-dev.txt
 requirements.in
 requirements.txt
 .github/CODEOWNERS
+.github/workflows/ci.yml
 .github/workflows/release.yml
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/index.rst
 docs/examples/cq_drill.py
 docs/examples/cq_helix.py
@@ -24,16 +25,22 @@
 docs/examples/images/cq_helix.png
 docs/examples/images/cq_pocket.png
 docs/examples/images/cq_profile.png
 src/ocp_freecad_cam/__init__.py
 src/ocp_freecad_cam/api.py
 src/ocp_freecad_cam/api_util.py
 src/ocp_freecad_cam/common.py
-src/ocp_freecad_cam/operations.py
+src/ocp_freecad_cam/fc_impl.py
+src/ocp_freecad_cam/fc_impl_util.py
 src/ocp_freecad_cam/visualizer.py
 src/ocp_freecad_cam.egg-info/PKG-INFO
 src/ocp_freecad_cam.egg-info/SOURCES.txt
 src/ocp_freecad_cam.egg-info/dependency_links.txt
 src/ocp_freecad_cam.egg-info/top_level.txt
 stubs/Part/__init__.pyi
+tests/test_adaptive.py
+tests/test_drill.py
+tests/test_engrave.py
+tests/test_helix.py
 tests/test_params.py
-tests/test_profile.py
+tests/test_profile.py
+tests/test_waterline.py
```

### Comparing `ocp-freecad-cam-0.0.1/tests/test_params.py` & `ocp-freecad-cam-0.9.0/tests/test_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import FreeCAD
 import Part
 import pytest
 from Path.Main import Job as FCJob
 
 from ocp_freecad_cam.api import Endmill, VBit
 from ocp_freecad_cam.api_util import AutoUnitKey
-from ocp_freecad_cam.operations import (
+from ocp_freecad_cam.fc_impl import (
     DeburrOp,
     DrillOp,
     FaceOp,
     HelixOp,
     PocketOp,
     ProfileOp,
     Surface3DOp,
```

### Comparing `ocp-freecad-cam-0.0.1/tests/test_profile.py` & `ocp-freecad-cam-0.9.0/tests/test_profile.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,13 +12,13 @@
     ],
 )
 def test_cq_profile(test_unit, expected_gcode_1, expected_gcode_2):
     box = cq.Workplane().box(10, 10, 1)
     top = box.faces(">Z").workplane()
     profile_shape = box.faces("<Z")
     tool = Endmill("1mm", diameter=1)
-    job = Job(top, box, units=test_unit)
+    job = Job(top, box, "grbl", units=test_unit)
     job = job.profile(profile_shape, tool)
     gcode = job.to_gcode()
 
     assert expected_gcode_1 in gcode
     assert expected_gcode_2 in gcode
```

