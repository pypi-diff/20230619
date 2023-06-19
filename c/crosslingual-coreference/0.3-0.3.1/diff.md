# Comparing `tmp/crosslingual_coreference-0.3.tar.gz` & `tmp/crosslingual-coreference-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslingual_coreference-0.3.tar", max compression
+gzip compressed data, was "crosslingual-coreference-0.3.1.tar", max compression
```

## Comparing `crosslingual_coreference-0.3.tar` & `crosslingual-coreference-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1077 2023-04-05 14:15:00.905016 crosslingual_coreference-0.3/LICENSE
--rw-r--r--   0        0        0     4784 2023-04-05 14:15:00.905016 crosslingual_coreference-0.3/README.md
--rw-r--r--   0        0        0     4861 2023-04-05 14:15:00.905016 crosslingual_coreference-0.3/crosslingual_coreference/CorefResolver.py
--rw-r--r--   0        0        0    10116 2023-04-05 14:15:00.905016 crosslingual_coreference-0.3/crosslingual_coreference/CrossLingualPredictor.py
--rw-r--r--   0        0        0     2311 2023-04-05 14:15:00.905016 crosslingual_coreference-0.3/crosslingual_coreference/CrossLingualPredictorSpacy.py
--rw-r--r--   0        0        0     1028 2023-04-05 14:15:00.905016 crosslingual_coreference-0.3/crosslingual_coreference/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 14:15:00.905016 crosslingual_coreference-0.3/crosslingual_coreference/examples/__init__.py
--rw-r--r--   0        0        0     1623 2023-04-05 14:15:00.905016 crosslingual_coreference-0.3/crosslingual_coreference/examples/data.py
--rw-r--r--   0        0        0      187 2023-04-05 14:15:00.905016 crosslingual_coreference-0.3/crosslingual_coreference/examples/test_chunking.py
--rw-r--r--   0        0        0      153 2023-04-05 14:15:00.905016 crosslingual_coreference-0.3/crosslingual_coreference/examples/test_individual.py
--rw-r--r--   0        0        0      273 2023-04-05 14:15:00.905016 crosslingual_coreference-0.3/crosslingual_coreference/examples/test_spacy.py
--rw-r--r--   0        0        0     1617 2023-04-05 14:15:00.909016 crosslingual_coreference-0.3/pyproject.toml
--rw-r--r--   0        0        0     6348 1970-01-01 00:00:00.000000 crosslingual_coreference-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-11-14 20:15:47.673854 crosslingual-coreference-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4719 2023-06-19 13:11:33.233396 crosslingual-coreference-0.3.1/README.md
+-rw-r--r--   0        0        0     4861 2022-11-14 20:15:47.674075 crosslingual-coreference-0.3.1/crosslingual_coreference/CorefResolver.py
+-rw-r--r--   0        0        0    10116 2023-06-19 12:58:16.093856 crosslingual-coreference-0.3.1/crosslingual_coreference/CrossLingualPredictor.py
+-rw-r--r--   0        0        0     2311 2022-11-14 20:15:47.674290 crosslingual-coreference-0.3.1/crosslingual_coreference/CrossLingualPredictorSpacy.py
+-rw-r--r--   0        0        0     1028 2023-01-05 16:15:44.513333 crosslingual-coreference-0.3.1/crosslingual_coreference/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-14 20:15:47.674431 crosslingual-coreference-0.3.1/crosslingual_coreference/examples/__init__.py
+-rw-r--r--   0        0        0     1623 2022-11-14 20:15:47.674520 crosslingual-coreference-0.3.1/crosslingual_coreference/examples/data.py
+-rw-r--r--   0        0        0      187 2022-11-14 20:15:47.674587 crosslingual-coreference-0.3.1/crosslingual_coreference/examples/test_chunking.py
+-rw-r--r--   0        0        0      153 2022-11-14 20:15:47.674656 crosslingual-coreference-0.3.1/crosslingual_coreference/examples/test_individual.py
+-rw-r--r--   0        0        0      273 2022-11-14 20:15:47.674729 crosslingual-coreference-0.3.1/crosslingual_coreference/examples/test_spacy.py
+-rw-r--r--   0        0        0     1810 2023-06-19 12:58:40.892438 crosslingual-coreference-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5974 1970-01-01 00:00:00.000000 crosslingual-coreference-0.3.1/setup.py
+-rw-r--r--   0        0        0     6234 1970-01-01 00:00:00.000000 crosslingual-coreference-0.3.1/PKG-INFO
```

### Comparing `crosslingual_coreference-0.3/LICENSE` & `crosslingual-coreference-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crosslingual_coreference-0.3/README.md` & `crosslingual-coreference-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,14 @@
 )
 ```
 
 ## Use spaCy pipeline
 ```python
 import spacy
 
-import crosslingual_coreference
-
 text = (
     "Do not forget about Momofuku Ando! He created instant noodles in Osaka. At"
     " that location, Nissin was founded. Many students survived by eating these"
     " noodles, but they don't even know him."
 )
 
 
@@ -102,15 +100,14 @@
 # Nissin: [21, 21],
 # Many students: [26, 27]}
 ```
 ### Visualize spacy pipeline
 This only works with spacy >= 3.3.
 ```python
 import spacy
-import crosslingual_coreference
 from spacy.tokens import Span
 from spacy import displacy
 
 text = (
     "Do not forget about Momofuku Ando! He created instant noodles in Osaka. At"
     " that location, Nissin was founded. Many students survived by eating these"
     " noodles, but they don't even know him."
```

### Comparing `crosslingual_coreference-0.3/crosslingual_coreference/CorefResolver.py` & `crosslingual-coreference-0.3.1/crosslingual_coreference/CorefResolver.py`

 * *Files identical despite different names*

### Comparing `crosslingual_coreference-0.3/crosslingual_coreference/CrossLingualPredictor.py` & `crosslingual-coreference-0.3.1/crosslingual_coreference/CrossLingualPredictor.py`

 * *Files identical despite different names*

### Comparing `crosslingual_coreference-0.3/crosslingual_coreference/CrossLingualPredictorSpacy.py` & `crosslingual-coreference-0.3.1/crosslingual_coreference/CrossLingualPredictorSpacy.py`

 * *Files identical despite different names*

### Comparing `crosslingual_coreference-0.3/crosslingual_coreference/__init__.py` & `crosslingual-coreference-0.3.1/crosslingual_coreference/__init__.py`

 * *Files identical despite different names*

### Comparing `crosslingual_coreference-0.3/crosslingual_coreference/examples/data.py` & `crosslingual-coreference-0.3.1/crosslingual_coreference/examples/data.py`

 * *Files identical despite different names*

### Comparing `crosslingual_coreference-0.3/pyproject.toml` & `crosslingual-coreference-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crosslingual-coreference"
-version = "0.3"
+version = "0.3.1"
 description = "A multi-lingual approach to AllenNLP CoReference Resolution, along with a wrapper for spaCy."
 authors = ["David Berenstein <david.m.berenstein@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pandora-intelligence/crosslingual-coreference"
 repository = "https://github.com/pandora-intelligence/crosslingual-coreference"
 documentation = "https://github.com/pandora-intelligence/crosslingual-coreference"
@@ -17,24 +17,29 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development"
 ]
+packages = [{include = "crosslingual_coreference"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 allennlp = "~2.9"
 allennlp-models = "~2.9"
 spacy = "~3.1"
 scipy = "^1.7"
 cached-path = "1.1.2"
 protobuf = "^3.20"
 
+[tool.poetry.plugins]
+
+[tool.poetry.plugins."spacy_factories"]
+"spacy" = "crosslingual_coreference.__init__:make_crosslingual_coreference"
 
 [tool.poetry.dev-dependencies]
 pytest = "~7.0"
 flake8 = "~4.0"
 black = "~22.3"
 flake8-bugbear = "~22.3"
 flake8-docstrings = "~1.6"
```

### Comparing `crosslingual_coreference-0.3/PKG-INFO` & `crosslingual-coreference-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosslingual-coreference
-Version: 0.3
+Version: 0.3.1
 Summary: A multi-lingual approach to AllenNLP CoReference Resolution, along with a wrapper for spaCy.
 Home-page: https://github.com/pandora-intelligence/crosslingual-coreference
 License: MIT
 Keywords: AllenNLP,spaCy,NLP
 Author: David Berenstein
 Author-email: david.m.berenstein@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -12,15 +12,14 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Dist: allennlp (>=2.9,<2.10)
@@ -94,16 +93,14 @@
 )
 ```
 
 ## Use spaCy pipeline
 ```python
 import spacy
 
-import crosslingual_coreference
-
 text = (
     "Do not forget about Momofuku Ando! He created instant noodles in Osaka. At"
     " that location, Nissin was founded. Many students survived by eating these"
     " noodles, but they don't even know him."
 )
 
 
@@ -137,15 +134,14 @@
 # Nissin: [21, 21],
 # Many students: [26, 27]}
 ```
 ### Visualize spacy pipeline
 This only works with spacy >= 3.3.
 ```python
 import spacy
-import crosslingual_coreference
 from spacy.tokens import Span
 from spacy import displacy
 
 text = (
     "Do not forget about Momofuku Ando! He created instant noodles in Osaka. At"
     " that location, Nissin was founded. Many students survived by eating these"
     " noodles, but they don't even know him."
```

