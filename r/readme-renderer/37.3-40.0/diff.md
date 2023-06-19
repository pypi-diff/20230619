# Comparing `tmp/readme_renderer-37.3.tar.gz` & `tmp/readme_renderer-40.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readme_renderer-37.3.tar", last modified: Mon Oct 31 20:54:53 2022, max compression
+gzip compressed data, was "readme_renderer-40.0.tar", last modified: Mon Jun 19 14:03:03 2023, max compression
```

## Comparing `readme_renderer-37.3.tar` & `readme_renderer-40.0.tar`

### file list

```diff
@@ -1,159 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:54:53.200729 readme_renderer-37.3/
--rw-r--r--   0 runner    (1001) docker     (121)     5047 2022-10-31 20:54:28.000000 readme_renderer-37.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9694 2022-10-31 20:54:28.000000 readme_renderer-37.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-10-31 20:54:28.000000 readme_renderer-37.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2518 2022-10-31 20:54:53.200729 readme_renderer-37.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-10-31 20:54:28.000000 readme_renderer-37.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-10-31 20:54:28.000000 readme_renderer-37.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:54:53.184728 readme_renderer-37.3/readme_renderer/
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-10-31 20:54:28.000000 readme_renderer-37.3/readme_renderer/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-10-31 20:54:28.000000 readme_renderer-37.3/readme_renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-10-31 20:54:28.000000 readme_renderer-37.3/readme_renderer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4290 2022-10-31 20:54:28.000000 readme_renderer-37.3/readme_renderer/clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     3595 2022-10-31 20:54:28.000000 readme_renderer-37.3/readme_renderer/markdown.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 20:54:28.000000 readme_renderer-37.3/readme_renderer/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4460 2022-10-31 20:54:28.000000 readme_renderer-37.3/readme_renderer/rst.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-10-31 20:54:28.000000 readme_renderer-37.3/readme_renderer/txt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:54:53.188729 readme_renderer-37.3/readme_renderer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2518 2022-10-31 20:54:53.000000 readme_renderer-37.3/readme_renderer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5036 2022-10-31 20:54:53.000000 readme_renderer-37.3/readme_renderer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 20:54:53.000000 readme_renderer-37.3/readme_renderer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-10-31 20:54:53.000000 readme_renderer-37.3/readme_renderer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-31 20:54:53.000000 readme_renderer-37.3/readme_renderer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-31 20:54:53.204730 readme_renderer-37.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2022-10-31 20:54:28.000000 readme_renderer-37.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:54:53.188729 readme_renderer-37.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:54:53.200729 readme_renderer-37.3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_001.html
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_001.md
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_002.html
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_002.md
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_003.html
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_003.md
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_004.html
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_004.md
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_005.html
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_005.md
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_006.html
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_006.md
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_007.html
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_007.md
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_008.html
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_008.md
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_009.html
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_009.md
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_smart_strong.html
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_smart_strong.md
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_strong.html
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_strong.md
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_style.html
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_CommonMark_style.md
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_001.html
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_001.md
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_002.html
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_002.md
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_003.html
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_003.md
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_004.html
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_004.md
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_005.html
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_005.md
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_006.html
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_006.md
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_007.html
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_007.md
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_008.html
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_008.md
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_009.html
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_009.md
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_010.html
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_010.md
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_011.html
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_011.md
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_012.html
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_012.md
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_013.html
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_013.md
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_014.html
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_014.md
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_015.html
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_015.md
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_016.html
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_016.md
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_017.html
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_017.md
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_018.html
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_018.md
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_019.html
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_019.md
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_020.html
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_020.md
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_021.html
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_021.md
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_022.html
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_022.md
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_023.html
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_023.md
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_024.html
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_024.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_025.html
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_025.md
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_doublequotes.html
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_doublequotes.md
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_highlight.html
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_highlight.md
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_highlight_default_py.html
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_highlight_default_py.md
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_img.html
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_img.md
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_malicious_pre.html
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_malicious_pre.md
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_style.html
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_GFM_style.md
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_003.html
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_003.rst
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_004.html
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_004.rst
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_005.html
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_005.rst
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_006.html
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_006.rst
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_007.html
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_007.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_008.html
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_008.rst
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_admonitions.html
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_bibtex.html
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_bibtex.rst
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_caption.html
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_caption.rst
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_contents.html
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_contents.rst
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_docinfo.html
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_docinfo.rst
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_figure.html
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_figure.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3671 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_linkify.html
--rw-r--r--   0 runner    (1001) docker     (121)     2787 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_linkify.rst
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_math.html
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_math.rst
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_png.html
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_png.rst
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_png_attrs.html
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_png_attrs.rst
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_svg.html
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_svg.rst
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_svg_attrs.html
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_svg_attrs.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_tables.html
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_rst_tables.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8087 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_txt_001.html
--rw-r--r--   0 runner    (1001) docker     (121)     7123 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/fixtures/test_txt_001.txt
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/test_clean.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      784 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/test_markdown.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      520 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/test_noextra.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1840 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/test_rst.py
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-10-31 20:54:28.000000 readme_renderer-37.3/tests/test_txt.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-10-31 20:54:28.000000 readme_renderer-37.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:03:03.852100 readme_renderer-40.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-19 14:02:50.000000 readme_renderer-40.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-06-19 14:02:50.000000 readme_renderer-40.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-19 14:02:50.000000 readme_renderer-40.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-19 14:03:03.852100 readme_renderer-40.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-19 14:02:50.000000 readme_renderer-40.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-19 14:02:50.000000 readme_renderer-40.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:03:03.820099 readme_renderer-40.0/readme_renderer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-19 14:02:50.000000 readme_renderer-40.0/readme_renderer/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-19 14:02:50.000000 readme_renderer-40.0/readme_renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-19 14:02:50.000000 readme_renderer-40.0/readme_renderer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-19 14:02:50.000000 readme_renderer-40.0/readme_renderer/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-19 14:02:50.000000 readme_renderer-40.0/readme_renderer/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:02:50.000000 readme_renderer-40.0/readme_renderer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-19 14:02:50.000000 readme_renderer-40.0/readme_renderer/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-19 14:02:50.000000 readme_renderer-40.0/readme_renderer/txt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:03:03.820099 readme_renderer-40.0/readme_renderer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-19 14:03:03.000000 readme_renderer-40.0/readme_renderer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-19 14:03:03.000000 readme_renderer-40.0/readme_renderer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:03:03.000000 readme_renderer-40.0/readme_renderer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-19 14:03:03.000000 readme_renderer-40.0/readme_renderer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 14:03:03.000000 readme_renderer-40.0/readme_renderer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-19 14:03:03.852100 readme_renderer-40.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-19 14:02:50.000000 readme_renderer-40.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:03:03.820099 readme_renderer-40.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:03:03.852100 readme_renderer-40.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_001.html
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_001.md
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_002.html
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_002.md
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_003.html
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_003.md
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_004.html
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_004.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_005.html
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_005.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_006.html
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_006.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_007.html
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_007.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_008.html
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_008.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_009.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_009.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_smart_strong.html
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_smart_strong.md
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_strong.html
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_strong.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_style.html
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_CommonMark_style.md
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_001.html
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_001.md
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_002.html
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_002.md
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_003.html
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_003.md
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_004.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_004.md
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_005.html
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_005.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_006.html
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_006.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_007.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_007.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_008.html
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_008.md
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_009.html
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_009.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_010.html
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_010.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_011.html
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_011.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_012.html
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_012.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_013.html
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_013.md
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_014.html
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_014.md
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_015.html
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_015.md
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_016.html
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_016.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_017.html
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_017.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_018.html
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_018.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_019.html
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_019.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_020.html
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_020.md
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_021.html
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_021.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_022.html
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_022.md
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_023.html
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_023.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_024.html
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_024.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_025.html
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_025.md
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_doublequotes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_doublequotes.md
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_highlight.html
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_highlight.md
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_highlight_default_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_highlight_default_py.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_img.html
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_img.md
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_malicious_pre.html
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_malicious_pre.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_style.html
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_GFM_style.md
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_003.html
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_003.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_004.html
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_004.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_005.html
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_005.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_006.html
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_006.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_007.html
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_007.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_008.html
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_008.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_admonitions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_bibtex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_bibtex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_caption.html
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_caption.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_citations.html
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_citations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_contents.html
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_docinfo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_docinfo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_figure.html
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_figure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_footnotes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_footnotes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_linkify.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_linkify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_math.html
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_math.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_png.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_png.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_png_attrs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_png_attrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_svg.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_svg.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_svg_attrs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_svg_attrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_tables.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_rst_tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_txt_001.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/fixtures/test_txt_001.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/test_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      784 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/test_markdown.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      520 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/test_noextra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1840 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/test_rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-19 14:02:50.000000 readme_renderer-40.0/tests/test_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-19 14:02:50.000000 readme_renderer-40.0/tox.ini
```

### Comparing `readme_renderer-37.3/CHANGES.rst` & `readme_renderer-40.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changes
 =======
 
+40.0 (2023-06-16)
+-----------------
+
+* Add CLI option to render package README. (#271)
+* Adapt tests to pygments 2.14.0 (#272)
+* Update release process to use Trusted Publishing (#276)
+* Replace usage of deprecated `pkg_resources` with `importlib.metadata` (#281)
+* Drop support for Python 3.7 (#282), Test against Python 3.11 (#280)
+
 37.3 (2022-10-31)
 -----------------
 
 * Allow HTML5 `figure` tag through cleaner (#265)
 
 37.2 (2022-09-24)
 -----------------
```

### Comparing `readme_renderer-37.3/LICENSE` & `readme_renderer-40.0/LICENSE`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/PKG-INFO` & `readme_renderer-40.0/readme_renderer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: readme_renderer
-Version: 37.3
+Name: readme-renderer
+Version: 40.0
 Summary: readme_renderer is a library for rendering "readme" descriptions for Warehouse
 Home-page: https://github.com/pypa/readme_renderer
 Author: The Python Packaging Authority
 Author-email: admin@mail.pypi.org
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,22 +13,22 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: md
 License-File: LICENSE
 
 Readme Renderer
 ===============
 
 .. image:: https://badge.fury.io/py/readme-renderer.svg
```

### Comparing `readme_renderer-37.3/README.rst` & `readme_renderer-40.0/README.rst`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/pyproject.toml` & `readme_renderer-40.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/readme_renderer/__about__.py` & `readme_renderer-40.0/readme_renderer/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,14 @@
 
 __title__ = "readme_renderer"
 __summary__ = (
     'readme_renderer is a library for rendering "readme" ' "descriptions for Warehouse"
 )
 __uri__ = "https://github.com/pypa/readme_renderer"
 
-__version__ = "37.3"
+__version__ = "40.0"
 
 __author__ = "The Python Packaging Authority"
 __email__ = "admin@mail.pypi.org"
 
 __license__ = "Apache License, Version 2.0"
 __copyright__ = "Copyright 2014 %s" % __author__
```

### Comparing `readme_renderer-37.3/readme_renderer/__init__.py` & `readme_renderer-40.0/readme_renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/readme_renderer/clean.py` & `readme_renderer-40.0/readme_renderer/clean.py`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/readme_renderer/markdown.py` & `readme_renderer-40.0/readme_renderer/markdown.py`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/readme_renderer/rst.py` & `readme_renderer-40.0/readme_renderer/rst.py`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/readme_renderer/txt.py` & `readme_renderer-40.0/readme_renderer/txt.py`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/readme_renderer.egg-info/PKG-INFO` & `readme_renderer-40.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: readme-renderer
-Version: 37.3
+Name: readme_renderer
+Version: 40.0
 Summary: readme_renderer is a library for rendering "readme" descriptions for Warehouse
 Home-page: https://github.com/pypa/readme_renderer
 Author: The Python Packaging Authority
 Author-email: admin@mail.pypi.org
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,22 +13,22 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: md
 License-File: LICENSE
 
 Readme Renderer
 ===============
 
 .. image:: https://badge.fury.io/py/readme-renderer.svg
```

### Comparing `readme_renderer-37.3/readme_renderer.egg-info/SOURCES.txt` & `readme_renderer-40.0/readme_renderer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 readme_renderer.egg-info/PKG-INFO
 readme_renderer.egg-info/SOURCES.txt
 readme_renderer.egg-info/dependency_links.txt
 readme_renderer.egg-info/requires.txt
 readme_renderer.egg-info/top_level.txt
 tests/__init__.py
 tests/test_clean.py
+tests/test_cli.py
 tests/test_markdown.py
 tests/test_noextra.py
 tests/test_rst.py
 tests/test_txt.py
 tests/fixtures/test_CommonMark_001.html
 tests/fixtures/test_CommonMark_001.md
 tests/fixtures/test_CommonMark_002.html
@@ -125,20 +126,24 @@
 tests/fixtures/test_rst_008.rst
 tests/fixtures/test_rst_admonitions.html
 tests/fixtures/test_rst_admonitions.rst
 tests/fixtures/test_rst_bibtex.html
 tests/fixtures/test_rst_bibtex.rst
 tests/fixtures/test_rst_caption.html
 tests/fixtures/test_rst_caption.rst
+tests/fixtures/test_rst_citations.html
+tests/fixtures/test_rst_citations.rst
 tests/fixtures/test_rst_contents.html
 tests/fixtures/test_rst_contents.rst
 tests/fixtures/test_rst_docinfo.html
 tests/fixtures/test_rst_docinfo.rst
 tests/fixtures/test_rst_figure.html
 tests/fixtures/test_rst_figure.rst
+tests/fixtures/test_rst_footnotes.html
+tests/fixtures/test_rst_footnotes.rst
 tests/fixtures/test_rst_linkify.html
 tests/fixtures/test_rst_linkify.rst
 tests/fixtures/test_rst_math.html
 tests/fixtures/test_rst_math.rst
 tests/fixtures/test_rst_png.html
 tests/fixtures/test_rst_png.rst
 tests/fixtures/test_rst_png_attrs.html
```

### Comparing `readme_renderer-37.3/setup.py` & `readme_renderer-40.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,21 +43,21 @@
         "Operating System :: POSIX",
         "Operating System :: POSIX :: BSD",
         "Operating System :: POSIX :: Linux",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Typing :: Typed",
     ],
     install_requires=["bleach>=2.1.0", "docutils>=0.13.1", "Pygments>=2.5.1"],
     include_package_data=True,
     extras_require={"md": "cmarkgfm>=0.8.0"},
     packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

### Comparing `readme_renderer-37.3/tests/fixtures/test_CommonMark_008.html` & `readme_renderer-40.0/tests/fixtures/test_CommonMark_008.html`

 * *Files 8% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 
     <span class="k">def</span> <span class="nf">make_sound</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Ruff!&#39;</span><span class="p">)</span>
 
 <span class="n">dog</span> <span class="o">=</span> <span class="n">Dog</span><span class="p">(</span><span class="s1">&#39;Fido&#39;</span><span class="p">)</span>
 </pre>
 <p>and then here is some bash:</p>
-<pre lang="bash"><span class="k">if</span> <span class="o">[</span> <span class="s2">&quot;</span><span class="nv">$1</span><span class="s2">&quot;</span> <span class="o">=</span> <span class="s2">&quot;--help&quot;</span> <span class="o">]</span><span class="p">;</span> <span class="k">then</span>
-    <span class="nb">echo</span> <span class="s2">&quot;OK&quot;</span>
+<pre lang="bash"><span class="k">if</span><span class="w"> </span><span class="o">[</span><span class="w"> </span><span class="s2">&quot;</span><span class="nv">$1</span><span class="s2">&quot;</span><span class="w"> </span><span class="o">=</span><span class="w"> </span><span class="s2">&quot;--help&quot;</span><span class="w"> </span><span class="o">]</span><span class="p">;</span><span class="w"> </span><span class="k">then</span>
+<span class="w">    </span><span class="nb">echo</span><span class="w"> </span><span class="s2">&quot;OK&quot;</span>
 <span class="k">fi</span>
 </pre>
 <p>or click <a href="http://www.surveymonkey.com" rel="nofollow">SurveyMonkey</a></p>
```

### Comparing `readme_renderer-37.3/tests/fixtures/test_GFM_doublequotes.html` & `readme_renderer-40.0/tests/fixtures/test_GFM_doublequotes.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <p>This is normal text.</p>
 <pre><code>This is code text.
 </code></pre>
 <pre lang="python3"><span class="k">def</span> <span class="nf">this_is_python</span><span class="p">():</span>
-    <span class="sd">&quot;&quot;&quot;This is a docstring.&quot;&quot;&quot;</span>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;This is a docstring.&quot;&quot;&quot;</span>
     <span class="k">pass</span>
 </pre>
-<pre lang="go"><span class="kd">func</span><span class="w"> </span><span class="nx">ThisIsGo</span><span class="p">(){</span><span class="w"></span>
-<span class="w">    </span><span class="k">return</span><span class="w"></span>
-<span class="p">}</span><span class="w"></span>
+<pre lang="go"><span class="kd">func</span><span class="w"> </span><span class="nx">ThisIsGo</span><span class="p">(){</span>
+<span class="w">    </span><span class="k">return</span>
+<span class="p">}</span>
 </pre>
```

### Comparing `readme_renderer-37.3/tests/fixtures/test_GFM_highlight.html` & `readme_renderer-40.0/tests/fixtures/test_GFM_malicious_pre.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,6 @@
 <p>This is normal text.</p>
-<pre><code>This is code text.
-</code></pre>
 <pre lang="python3"><span class="k">def</span> <span class="nf">this_is_python</span><span class="p">():</span>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;This is a docstring.&quot;&quot;&quot;</span>
     <span class="k">pass</span>
-</pre>
-<pre lang="go"><span class="kd">func</span><span class="w"> </span><span class="nx">ThisIsGo</span><span class="p">(){</span><span class="w"></span>
-<span class="w">    </span><span class="k">return</span><span class="w"></span>
-<span class="p">}</span><span class="w"></span>
-</pre>
-<pre lang="abc">An unknown code fence block
+<span class="o">&lt;</span><span class="n">script</span> <span class="nb">type</span><span class="o">=</span><span class="s2">&quot;text/javascript&quot;</span><span class="o">&gt;</span><span class="n">alert</span><span class="p">(</span><span class="s1">&#39;I am evil.&#39;</span><span class="p">);</span><span class="o">&lt;/</span><span class="n">script</span><span class="o">&gt;</span>
 </pre>
```

### Comparing `readme_renderer-37.3/tests/fixtures/test_rst_caption.html` & `readme_renderer-40.0/tests/fixtures/test_rst_caption.html`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/tests/fixtures/test_rst_contents.html` & `readme_renderer-40.0/tests/fixtures/test_rst_contents.html`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/tests/fixtures/test_rst_docinfo.html` & `readme_renderer-40.0/tests/fixtures/test_rst_docinfo.html`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/tests/fixtures/test_rst_linkify.html` & `readme_renderer-40.0/tests/fixtures/test_rst_linkify.html`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/tests/fixtures/test_rst_linkify.rst` & `readme_renderer-40.0/tests/fixtures/test_rst_linkify.rst`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/tests/fixtures/test_rst_tables.html` & `readme_renderer-40.0/tests/fixtures/test_rst_tables.html`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/tests/fixtures/test_rst_tables.rst` & `readme_renderer-40.0/tests/fixtures/test_rst_tables.rst`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/tests/fixtures/test_txt_001.html` & `readme_renderer-40.0/tests/fixtures/test_txt_001.html`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/tests/fixtures/test_txt_001.txt` & `readme_renderer-40.0/tests/fixtures/test_txt_001.txt`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/tests/test_markdown.py` & `readme_renderer-40.0/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/tests/test_noextra.py` & `readme_renderer-40.0/tests/test_noextra.py`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/tests/test_rst.py` & `readme_renderer-40.0/tests/test_rst.py`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/tests/test_txt.py` & `readme_renderer-40.0/tests/test_txt.py`

 * *Files identical despite different names*

### Comparing `readme_renderer-37.3/tox.ini` & `readme_renderer-40.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py37,py38,py39,py310,pep8,packaging,noextra,mypy
+envlist = py38,py39,py310,py311,pep8,packaging,noextra,mypy
 isolated_build = True
 
 [testenv]
 deps =
     pytest
     pytest-cov
 commands =
```

