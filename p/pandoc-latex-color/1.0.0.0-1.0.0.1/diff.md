# Comparing `tmp/pandoc_latex_color-1.0.0.0.tar.gz` & `tmp/pandoc_latex_color-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc_latex_color-1.0.0.0.tar", max compression
+gzip compressed data, was "pandoc_latex_color-1.0.0.1.tar", max compression
```

## Comparing `pandoc_latex_color-1.0.0.0.tar` & `pandoc_latex_color-1.0.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1521 2023-06-18 20:38:34.130010 pandoc_latex_color-1.0.0.0/LICENSE
--rw-r--r--   0        0        0     2830 2023-06-18 20:38:34.130010 pandoc_latex_color-1.0.0.0/README.md
--rw-r--r--   0        0        0    11481 2023-06-18 20:38:34.134010 pandoc_latex_color-1.0.0.0/pandoc_latex_color.py
--rw-r--r--   0        0        0     2900 2023-06-18 20:38:34.134010 pandoc_latex_color-1.0.0.0/pyproject.toml
--rw-r--r--   0        0        0     3919 1970-01-01 00:00:00.000000 pandoc_latex_color-1.0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-06-19 11:35:11.055587 pandoc_latex_color-1.0.0.1/LICENSE
+-rw-r--r--   0        0        0     3158 2023-06-19 11:35:11.055587 pandoc_latex_color-1.0.0.1/README.md
+-rw-r--r--   0        0        0    11481 2023-06-19 11:35:11.055587 pandoc_latex_color-1.0.0.1/pandoc_latex_color.py
+-rw-r--r--   0        0        0     2900 2023-06-19 11:35:11.055587 pandoc_latex_color-1.0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4247 1970-01-01 00:00:00.000000 pandoc_latex_color-1.0.0.1/PKG-INFO
```

### Comparing `pandoc_latex_color-1.0.0.0/LICENSE` & `pandoc_latex_color-1.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandoc_latex_color-1.0.0.0/README.md` & `pandoc_latex_color-1.0.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 [![Python package](https://github.com/chdemko/pandoc-latex-color/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-latex-color/actions/workflows/python-package.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-color/develop.svg)](https://coveralls.io/github/chdemko/pandoc-latex-color?branch=develop)
 [![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-latex-color.svg)](https://scrutinizer-ci.com/g/chdemko/pandoc-latex-color/)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
 [![License](https://img.shields.io/pypi/l/pandoc-latex-color.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-color/develop/LICENSE)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
+[![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
+[![Pandoc version](https://img.shields.io/badge/pandoc-2.11%20|%202.12%20|%202.13%20|%202.14%20|%202.15%20|%202.16%20|%202.17%20|%202.18%20|%202.19%20|%203.0%20|%203.1-blue.svg)](https://pandoc.org/)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
 [![Docs](https://img.shields.io/readthedocs/pandoc-latex-color.svg?logo=read-the-docs&logoColor=white)](http://pandoc-latex-color.readthedocs.io/en/latest/)
 
 *pandoc-latex-color* is a [pandoc] filter for setting the color to `Span`, and `Div` that have speficied classes or `latex-color` attribute.
 
 [pandoc]: http://pandoc.org/
```

### Comparing `pandoc_latex_color-1.0.0.0/pandoc_latex_color.py` & `pandoc_latex_color-1.0.0.1/pandoc_latex_color.py`

 * *Files identical despite different names*

### Comparing `pandoc_latex_color-1.0.0.0/pyproject.toml` & `pandoc_latex_color-1.0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["poetry-core>=1.2"]
     build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
     name = "pandoc-latex-color"
-    version = "1.0.0.0"
+    version = "1.0.0.1"
     description="A pandoc filter for changing color in LaTeX"
     authors = ["Christophe Demko <chdemko@gmail.com>"]
     license = "BSD-3-Clause"
     readme = "README.md"
     homepage="https://github.com/chdemko/pandoc-latex-color"
     keywords=["pandoc", "filters", "latex", "color"]
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
```

### Comparing `pandoc_latex_color-1.0.0.0/PKG-INFO` & `pandoc_latex_color-1.0.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandoc-latex-color
-Version: 1.0.0.0
+Version: 1.0.0.1
 Summary: A pandoc filter for changing color in LaTeX
 Home-page: https://github.com/chdemko/pandoc-latex-color
 License: BSD-3-Clause
 Keywords: pandoc,filters,latex,color
 Author: Christophe Demko
 Author-email: chdemko@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -30,14 +30,16 @@
 [![Python package](https://github.com/chdemko/pandoc-latex-color/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-latex-color/actions/workflows/python-package.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-color/develop.svg)](https://coveralls.io/github/chdemko/pandoc-latex-color?branch=develop)
 [![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-latex-color.svg)](https://scrutinizer-ci.com/g/chdemko/pandoc-latex-color/)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
 [![License](https://img.shields.io/pypi/l/pandoc-latex-color.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-color/develop/LICENSE)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
+[![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
+[![Pandoc version](https://img.shields.io/badge/pandoc-2.11%20|%202.12%20|%202.13%20|%202.14%20|%202.15%20|%202.16%20|%202.17%20|%202.18%20|%202.19%20|%203.0%20|%203.1-blue.svg)](https://pandoc.org/)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
 [![Docs](https://img.shields.io/readthedocs/pandoc-latex-color.svg?logo=read-the-docs&logoColor=white)](http://pandoc-latex-color.readthedocs.io/en/latest/)
 
 *pandoc-latex-color* is a [pandoc] filter for setting the color to `Span`, and `Div` that have speficied classes or `latex-color` attribute.
 
 [pandoc]: http://pandoc.org/
```

