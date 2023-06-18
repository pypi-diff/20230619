# Comparing `tmp/adafruit-circuitpython-bitmapsaver-1.2.8.tar.gz` & `tmp/adafruit-circuitpython-bitmapsaver-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bitmapsaver-1.2.8.tar", last modified: Thu May 11 18:22:49 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-bitmapsaver-1.2.9.tar", last modified: Fri May 26 16:23:07 2023, max compression
```

## Comparing `adafruit-circuitpython-bitmapsaver-1.2.8.tar` & `adafruit-circuitpython-bitmapsaver-1.2.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:49.368620 adafruit-circuitpython-bitmapsaver-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:49.356619 adafruit-circuitpython-bitmapsaver-1.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:49.360619 adafruit-circuitpython-bitmapsaver-1.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:49.360619 adafruit-circuitpython-bitmapsaver-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:49.360619 adafruit-circuitpython-bitmapsaver-1.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-11 18:22:49.368620 adafruit-circuitpython-bitmapsaver-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-11 18:22:40.000000 adafruit-circuitpython-bitmapsaver-1.2.8/adafruit_bitmapsaver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:49.360619 adafruit-circuitpython-bitmapsaver-1.2.8/adafruit_circuitpython_bitmapsaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-11 18:22:49.000000 adafruit-circuitpython-bitmapsaver-1.2.8/adafruit_circuitpython_bitmapsaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-11 18:22:49.000000 adafruit-circuitpython-bitmapsaver-1.2.8/adafruit_circuitpython_bitmapsaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:22:49.000000 adafruit-circuitpython-bitmapsaver-1.2.8/adafruit_circuitpython_bitmapsaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 18:22:49.000000 adafruit-circuitpython-bitmapsaver-1.2.8/adafruit_circuitpython_bitmapsaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 18:22:49.000000 adafruit-circuitpython-bitmapsaver-1.2.8/adafruit_circuitpython_bitmapsaver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:49.364620 adafruit-circuitpython-bitmapsaver-1.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:49.364620 adafruit-circuitpython-bitmapsaver-1.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:49.364620 adafruit-circuitpython-bitmapsaver-1.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-11 18:22:40.000000 adafruit-circuitpython-bitmapsaver-1.2.8/examples/bitmapsaver_screenshot_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-11 18:22:40.000000 adafruit-circuitpython-bitmapsaver-1.2.8/examples/bitmapsaver_screenshot_tft_featherwing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-11 18:22:40.000000 adafruit-circuitpython-bitmapsaver-1.2.8/examples/bitmapsaver_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:49.368620 adafruit-circuitpython-bitmapsaver-1.2.8/guide/
--rw-r--r--   0 runner    (1001) docker     (123)    61494 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/guide/pygamer_screenshot.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/guide/pygamer_screenshot.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)   230454 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/guide/pyportal_screenshot.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/guide/pyportal_screenshot.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)   460854 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/guide/tft_featherwing_screenshot1.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/guide/tft_featherwing_screenshot1.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)   460854 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/guide/tft_featherwing_screenshot2.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/guide/tft_featherwing_screenshot2.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-11 18:22:40.000000 adafruit-circuitpython-bitmapsaver-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-11 18:22:27.000000 adafruit-circuitpython-bitmapsaver-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:22:49.368620 adafruit-circuitpython-bitmapsaver-1.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:07.030006 adafruit-circuitpython-bitmapsaver-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:07.022006 adafruit-circuitpython-bitmapsaver-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:07.026006 adafruit-circuitpython-bitmapsaver-1.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:07.026006 adafruit-circuitpython-bitmapsaver-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:07.026006 adafruit-circuitpython-bitmapsaver-1.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-26 16:23:07.030006 adafruit-circuitpython-bitmapsaver-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-26 16:23:00.000000 adafruit-circuitpython-bitmapsaver-1.2.9/adafruit_bitmapsaver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:07.026006 adafruit-circuitpython-bitmapsaver-1.2.9/adafruit_circuitpython_bitmapsaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-26 16:23:06.000000 adafruit-circuitpython-bitmapsaver-1.2.9/adafruit_circuitpython_bitmapsaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-26 16:23:07.000000 adafruit-circuitpython-bitmapsaver-1.2.9/adafruit_circuitpython_bitmapsaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:23:06.000000 adafruit-circuitpython-bitmapsaver-1.2.9/adafruit_circuitpython_bitmapsaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:23:06.000000 adafruit-circuitpython-bitmapsaver-1.2.9/adafruit_circuitpython_bitmapsaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 16:23:06.000000 adafruit-circuitpython-bitmapsaver-1.2.9/adafruit_circuitpython_bitmapsaver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:07.026006 adafruit-circuitpython-bitmapsaver-1.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:07.026006 adafruit-circuitpython-bitmapsaver-1.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:07.026006 adafruit-circuitpython-bitmapsaver-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-26 16:23:00.000000 adafruit-circuitpython-bitmapsaver-1.2.9/examples/bitmapsaver_screenshot_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 16:23:00.000000 adafruit-circuitpython-bitmapsaver-1.2.9/examples/bitmapsaver_screenshot_tft_featherwing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-26 16:23:00.000000 adafruit-circuitpython-bitmapsaver-1.2.9/examples/bitmapsaver_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:07.030006 adafruit-circuitpython-bitmapsaver-1.2.9/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    61494 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/guide/pygamer_screenshot.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/guide/pygamer_screenshot.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)   230454 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/guide/pyportal_screenshot.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/guide/pyportal_screenshot.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)   460854 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/guide/tft_featherwing_screenshot1.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/guide/tft_featherwing_screenshot1.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)   460854 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/guide/tft_featherwing_screenshot2.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/guide/tft_featherwing_screenshot2.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-26 16:23:00.000000 adafruit-circuitpython-bitmapsaver-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:22:50.000000 adafruit-circuitpython-bitmapsaver-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:23:07.030006 adafruit-circuitpython-bitmapsaver-1.2.9/setup.cfg
```

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bitmapsaver-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/.gitignore` & `adafruit-circuitpython-bitmapsaver-1.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-bitmapsaver-1.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/.pylintrc` & `adafruit-circuitpython-bitmapsaver-1.2.9/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -392,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bitmapsaver-1.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/LICENSE` & `adafruit-circuitpython-bitmapsaver-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bitmapsaver-1.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-bitmapsaver-1.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bitmapsaver-1.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/PKG-INFO` & `adafruit-circuitpython-bitmapsaver-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bitmapsaver
-Version: 1.2.8
+Version: 1.2.9
 Summary: Save a displayio.Bitmap (and associated displayio.Palette) into a BMP file.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BitmapSaver
 Keywords: adafruit,blinka,circuitpython,micropython,bitmapsaver,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/README.rst` & `adafruit-circuitpython-bitmapsaver-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/adafruit_bitmapsaver.py` & `adafruit-circuitpython-bitmapsaver-1.2.9/adafruit_bitmapsaver.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 try:
     from typing import Tuple, Optional, Union
     from io import BufferedWriter
 except ImportError:
     pass
 
-__version__ = "1.2.8"
+__version__ = "1.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BitmapSaver.git"
 
 
 def _write_bmp_header(output_file: BufferedWriter, filesize: int) -> None:
     output_file.write(bytes("BM", "ascii"))
     output_file.write(struct.pack("<I", filesize))
     output_file.write(b"\00\x00")
```

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/adafruit_circuitpython_bitmapsaver.egg-info/PKG-INFO` & `adafruit-circuitpython-bitmapsaver-1.2.9/adafruit_circuitpython_bitmapsaver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bitmapsaver
-Version: 1.2.8
+Version: 1.2.9
 Summary: Save a displayio.Bitmap (and associated displayio.Palette) into a BMP file.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BitmapSaver
 Keywords: adafruit,blinka,circuitpython,micropython,bitmapsaver,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/adafruit_circuitpython_bitmapsaver.egg-info/SOURCES.txt` & `adafruit-circuitpython-bitmapsaver-1.2.9/adafruit_circuitpython_bitmapsaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-bitmapsaver-1.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/docs/conf.py` & `adafruit-circuitpython-bitmapsaver-1.2.9/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
```

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/docs/index.rst` & `adafruit-circuitpython-bitmapsaver-1.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/examples/bitmapsaver_screenshot_simpletest.py` & `adafruit-circuitpython-bitmapsaver-1.2.9/examples/bitmapsaver_screenshot_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/examples/bitmapsaver_screenshot_tft_featherwing.py` & `adafruit-circuitpython-bitmapsaver-1.2.9/examples/bitmapsaver_screenshot_tft_featherwing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/examples/bitmapsaver_simpletest.py` & `adafruit-circuitpython-bitmapsaver-1.2.9/examples/bitmapsaver_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/guide/pygamer_screenshot.bmp` & `adafruit-circuitpython-bitmapsaver-1.2.9/guide/pygamer_screenshot.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/guide/pyportal_screenshot.bmp` & `adafruit-circuitpython-bitmapsaver-1.2.9/guide/pyportal_screenshot.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/guide/tft_featherwing_screenshot1.bmp` & `adafruit-circuitpython-bitmapsaver-1.2.9/guide/tft_featherwing_screenshot1.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/guide/tft_featherwing_screenshot2.bmp` & `adafruit-circuitpython-bitmapsaver-1.2.9/guide/tft_featherwing_screenshot2.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmapsaver-1.2.8/pyproject.toml` & `adafruit-circuitpython-bitmapsaver-1.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bitmapsaver"
 description = "Save a displayio.Bitmap (and associated displayio.Palette) into a BMP file."
-version = "1.2.8"
+version = "1.2.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BitmapSaver"}
 keywords = [
     "adafruit",
```

