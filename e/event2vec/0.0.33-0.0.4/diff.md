# Comparing `tmp/event2vec-0.0.33.tar.gz` & `tmp/event2vec-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event2vec-0.0.33.tar", max compression
+gzip compressed data, was "event2vec-0.0.4.tar", max compression
```

## Comparing `event2vec-0.0.33.tar` & `event2vec-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    15731 2023-03-14 22:29:01.448203 event2vec-0.0.33/LICENSE
--rw-r--r--   0        0        0      762 2023-03-14 22:29:01.448203 event2vec-0.0.33/README.md
--rw-r--r--   0        0        0      242 2023-03-14 22:29:01.448203 event2vec-0.0.33/bin/config.cfg
--rw-r--r--   0        0        0     5993 2023-04-21 19:43:26.765843 event2vec-0.0.33/bin/submit_i2b2.py
--rw-r--r--   0        0        0     5384 2023-04-21 19:43:24.325844 event2vec-0.0.33/bin/submit_omop.py
--rw-r--r--   0        0        0       17 2023-03-14 22:29:01.778203 event2vec-0.0.33/event2vec/__init__.py
--rw-r--r--   0        0        0     1148 2023-03-14 22:29:01.778203 event2vec-0.0.33/event2vec/concept_proximity.py
--rw-r--r--   0        0        0     1411 2023-05-25 16:23:01.245183 event2vec-0.0.33/event2vec/config.py
--rw-r--r--   0        0        0     5203 2023-05-31 16:16:31.163153 event2vec-0.0.33/event2vec/cooccurrence_matrix_pandas.py
--rw-r--r--   0        0        0     7099 2023-04-22 02:17:00.822933 event2vec-0.0.33/event2vec/cooccurrence_matrix_spark.py
--rw-r--r--   0        0        0     1818 2023-05-25 19:08:52.021601 event2vec-0.0.33/event2vec/datasets.py
--rw-r--r--   0        0        0    20190 2023-06-07 15:53:22.497176 event2vec-0.0.33/event2vec/event_transformer.py
--rw-r--r--   0        0        0     6425 2023-03-14 22:29:01.778203 event2vec-0.0.33/event2vec/nomenclatures.py
--rw-r--r--   0        0        0     6867 2023-05-25 20:21:37.250039 event2vec-0.0.33/event2vec/svd_ppmi.py
--rw-r--r--   0        0        0     2040 2023-05-25 20:07:29.250350 event2vec-0.0.33/event2vec/utils.py
--rw-r--r--   0        0        0     4603 2023-06-07 16:14:27.367068 event2vec-0.0.33/pyproject.toml
--rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 event2vec-0.0.33/PKG-INFO
+-rw-r--r--   0        0        0    15731 2023-03-14 22:29:01.448203 event2vec-0.0.4/LICENSE
+-rw-r--r--   0        0        0      762 2023-03-14 22:29:01.448203 event2vec-0.0.4/README.md
+-rw-r--r--   0        0        0      242 2023-03-14 22:29:01.448203 event2vec-0.0.4/bin/config.cfg
+-rw-r--r--   0        0        0     5993 2023-04-21 19:43:26.765843 event2vec-0.0.4/bin/submit_i2b2.py
+-rw-r--r--   0        0        0     5384 2023-04-21 19:43:24.325844 event2vec-0.0.4/bin/submit_omop.py
+-rw-r--r--   0        0        0       17 2023-03-14 22:29:01.778203 event2vec-0.0.4/event2vec/__init__.py
+-rw-r--r--   0        0        0     1148 2023-03-14 22:29:01.778203 event2vec-0.0.4/event2vec/concept_proximity.py
+-rw-r--r--   0        0        0     1411 2023-05-25 16:23:01.245183 event2vec-0.0.4/event2vec/config.py
+-rw-r--r--   0        0        0     5203 2023-05-31 16:16:31.163153 event2vec-0.0.4/event2vec/cooccurrence_matrix_pandas.py
+-rw-r--r--   0        0        0     5296 2023-06-19 14:43:33.718449 event2vec-0.0.4/event2vec/cooccurrence_matrix_polars.py
+-rw-r--r--   0        0        0     7099 2023-04-22 02:17:00.822933 event2vec-0.0.4/event2vec/cooccurrence_matrix_spark.py
+-rw-r--r--   0        0        0     1818 2023-05-25 19:08:52.021601 event2vec-0.0.4/event2vec/datasets.py
+-rw-r--r--   0        0        0    14860 2023-06-19 14:43:33.718449 event2vec-0.0.4/event2vec/event_transformer.py
+-rw-r--r--   0        0        0     6425 2023-03-14 22:29:01.778203 event2vec-0.0.4/event2vec/nomenclatures.py
+-rw-r--r--   0        0        0     6867 2023-05-25 20:21:37.250039 event2vec-0.0.4/event2vec/svd_ppmi.py
+-rw-r--r--   0        0        0     4064 2023-06-19 14:43:33.718449 event2vec-0.0.4/event2vec/utils.py
+-rw-r--r--   0        0        0     4621 2023-06-19 14:43:53.078448 event2vec-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2953 1970-01-01 00:00:00.000000 event2vec-0.0.4/PKG-INFO
```

### Comparing `event2vec-0.0.33/LICENSE` & `event2vec-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.33/README.md` & `event2vec-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.33/bin/submit_i2b2.py` & `event2vec-0.0.4/bin/submit_i2b2.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.33/bin/submit_omop.py` & `event2vec-0.0.4/bin/submit_omop.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.33/event2vec/concept_proximity.py` & `event2vec-0.0.4/event2vec/concept_proximity.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.33/event2vec/config.py` & `event2vec-0.0.4/event2vec/config.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.33/event2vec/cooccurrence_matrix_pandas.py` & `event2vec-0.0.4/event2vec/cooccurrence_matrix_pandas.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.33/event2vec/cooccurrence_matrix_spark.py` & `event2vec-0.0.4/event2vec/cooccurrence_matrix_spark.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.33/event2vec/datasets.py` & `event2vec-0.0.4/event2vec/datasets.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.33/event2vec/nomenclatures.py` & `event2vec-0.0.4/event2vec/nomenclatures.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.33/event2vec/svd_ppmi.py` & `event2vec-0.0.4/event2vec/svd_ppmi.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.33/pyproject.toml` & `event2vec-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "event2vec"
-version = "0.0.33"
+version = "0.0.4"
 description = "event2vec"
 authors = ["Matthieu Doutreligne <matt.dout@gmail.com>"]
 license = "EUPL-v1.2"
 readme = "README.md"
 repository = "https://gitlab.com/strayMat/event2vec"
 homepage = "https://gitlab.com/strayMat/event2vec"
 include = ["bin"]
@@ -40,25 +40,26 @@
 # it is advised to pip install this depency after a poetry install
 pyspark = { version = "2.4.3", optional = true, python = ">=3.7.1, <3.8"}
 loguru = "^0.6.0"
 matplotlib = "^3.5.0"
 plotly = "^5.11.0"
 scikit-learn = "^1.0"
 fastparquet = "^0.8.1"
+tabulate = "^0.9.0"
+polars = "^0.18.0"
 
 # Documentation
 importlib-metadata = { version = "^4.11.3", optional = true }
 pygments = { version = "^2.11.2", optional = true }
 sphinx = { version = "^4.4.0", optional = true }
 sphinx-autodoc-typehints = { version = "^1.17.0", optional = true }
 pydata-sphinx-theme = { version = "^0.8.0", optional = true }
 sphinxcontrib-apidoc = { version = "^0.3.0", optional = true }
 sphinx-click = { version = "^3.1.0", optional = true }
 myst-nb = {version = "^0.17.1", optional = true}
-tabulate = "^0.9.0"
 
 
 [tool.poetry.dev-dependencies]
 # Testing
 pytest = "^7.1.1"
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.7.0"
```

### Comparing `event2vec-0.0.33/PKG-INFO` & `event2vec-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event2vec
-Version: 0.0.33
+Version: 0.0.4
 Summary: event2vec
 Home-page: https://gitlab.com/strayMat/event2vec
 License: EUPL-v1.2
 Author: Matthieu Doutreligne
 Author-email: matt.dout@gmail.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: Intended Audience :: Developers
@@ -28,14 +28,15 @@
 Requires-Dist: jedi (>=0.18.1,<0.19.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: matplotlib (>=3.5.0,<4.0.0)
 Requires-Dist: myst-nb (>=0.17.1,<0.18.0) ; extra == "docs"
 Requires-Dist: numpy (>=1.0.0)
 Requires-Dist: pandas (>=1.3.0)
 Requires-Dist: plotly (>=5.11.0,<6.0.0)
+Requires-Dist: polars (>=0.18.0,<0.19.0)
 Requires-Dist: pyarrow (>=0.17.0)
 Requires-Dist: pydata-sphinx-theme (>=0.8.0,<0.9.0) ; extra == "docs"
 Requires-Dist: pygments (>=2.11.2,<3.0.0) ; extra == "docs"
 Requires-Dist: pyspark (==2.4.3) ; python_full_version >= "3.7.1" and python_version < "3.8"
 Requires-Dist: python-dotenv (>=0.15.0,<0.16.0)
 Requires-Dist: scikit-learn (>=1.0,<2.0)
 Requires-Dist: sphinx (>=4.4.0,<5.0.0) ; extra == "docs"
```

