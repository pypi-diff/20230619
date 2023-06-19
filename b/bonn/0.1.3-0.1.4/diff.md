# Comparing `tmp/bonn-0.1.3-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/bonn-0.1.4-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7063740 bytes, number of entries: 11
--rw-r--r--  4.6 unx     6531 b- defN 23-Jun-18 05:05 bonn-0.1.3.dist-info/METADATA
--rw-r--r--  4.6 unx      134 b- defN 23-Jun-18 05:05 bonn-0.1.3.dist-info/WHEEL
--rw-r--r--  4.6 unx     1166 b- defN 23-Jun-18 05:05 bonn-0.1.3.dist-info/license_files/LICENSE.md
--rw-r--r--  4.6 unx      182 b- defN 23-Jun-18 05:05 bonn/__init__.py
--rw-r--r--  4.6 unx     6030 b- defN 23-Jun-18 05:05 bonn/category_manager.py
--rw-r--r--  4.6 unx     2241 b- defN 23-Jun-18 05:05 bonn/taxonomy.py
--rw-r--r--  4.6 unx     6449 b- defN 23-Jun-18 05:05 bonn/extract.py
--rw-r--r--  4.6 unx      585 b- defN 23-Jun-18 05:05 bonn/utils.py
--rw-r--r--  4.6 unx      122 b- defN 23-Jun-18 05:05 bonn/settings.py
--rwxr-xr-x  4.6 unx 30614032 b- defN 23-Jun-18 05:05 bonn/bonn.pypy39-pp73-x86_64-linux-gnu.so
--rw-r--r--  4.6 unx      841 b- defN 23-Jun-18 05:05 bonn-0.1.3.dist-info/RECORD
-11 files, 30638313 bytes uncompressed, 7062346 bytes compressed:  77.0%
+Zip file size: 1374768 bytes, number of entries: 11
+-rw-r--r--  4.6 unx     6653 b- defN 23-Jun-19 13:10 bonn-0.1.4.dist-info/METADATA
+-rw-r--r--  4.6 unx      129 b- defN 23-Jun-19 13:10 bonn-0.1.4.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1166 b- defN 23-Jun-19 13:10 bonn-0.1.4.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx        0 b- defN 23-Jun-19 13:10 bonn/__init__.py
+-rw-r--r--  4.6 unx     6147 b- defN 23-Jun-19 13:10 bonn/category_manager.py
+-rw-r--r--  4.6 unx     2222 b- defN 23-Jun-19 13:10 bonn/taxonomy.py
+-rw-r--r--  4.6 unx     6338 b- defN 23-Jun-19 13:10 bonn/extract.py
+-rw-r--r--  4.6 unx      603 b- defN 23-Jun-19 13:10 bonn/utils.py
+-rw-r--r--  4.6 unx      122 b- defN 23-Jun-19 13:10 bonn/settings.py
+-rwxr-xr-x  4.6 unx  5226384 b- defN 23-Jun-19 13:10 bonn/_bonn.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--  4.6 unx      839 b- defN 23-Jun-19 13:10 bonn-0.1.4.dist-info/RECORD
+11 files, 5250603 bytes uncompressed, 1373372 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
-Filename: bonn-0.1.3.dist-info/METADATA
+Filename: bonn-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: bonn-0.1.3.dist-info/WHEEL
+Filename: bonn-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: bonn-0.1.3.dist-info/license_files/LICENSE.md
+Filename: bonn-0.1.4.dist-info/license_files/LICENSE.md
 Comment: 
 
 Filename: bonn/__init__.py
 Comment: 
 
 Filename: bonn/category_manager.py
 Comment: 
@@ -21,14 +21,14 @@
 
 Filename: bonn/utils.py
 Comment: 
 
 Filename: bonn/settings.py
 Comment: 
 
-Filename: bonn/bonn.pypy39-pp73-x86_64-linux-gnu.so
+Filename: bonn/_bonn.cpython-37m-x86_64-linux-gnu.so
 Comment: 
 
-Filename: bonn-0.1.3.dist-info/RECORD
+Filename: bonn-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bonn/__init__.py

```diff
@@ -1,12 +0,0 @@
-00000000: 2320 696d 706f 7274 2074 6865 2063 6f6e  # import the con
-00000010: 7465 6e74 7320 6f66 2074 6865 2052 7573  tents of the Rus
-00000020: 7420 6c69 6272 6172 7920 696e 746f 2074  t library into t
-00000030: 6865 2050 7974 686f 6e20 6578 7465 6e73  he Python extens
-00000040: 696f 6e0a 2320 6f70 7469 6f6e 616c 3a20  ion.# optional: 
-00000050: 696e 636c 7564 6520 7468 6520 646f 6375  include the docu
-00000060: 6d65 6e74 6174 696f 6e20 6672 6f6d 2074  mentation from t
-00000070: 6865 2052 7573 7420 6d6f 6475 6c65 0a66  he Rust module.f
-00000080: 726f 6d20 2e62 6f6e 6e20 696d 706f 7274  rom .bonn import
-00000090: 202a 0a66 726f 6d20 2e62 6f6e 6e20 696d   *.from .bonn im
-000000a0: 706f 7274 205f 5f61 6c6c 5f5f 2c20 5f5f  port __all__, __
-000000b0: 646f 635f 5f0a                           doc__.
```

## bonn/category_manager.py

```diff
@@ -41,31 +41,38 @@
         self.bow = bow
         self._weighting = weighting
 
         self._set_vector(model)
         self._set_words()
 
     def _set_vector(self, model):
-        vector = np.mean([self._weighting[code] * model[w] for code, w in self.bow], axis=0)
-        self.vector = vector / sum([self._weighting[code] for code, _ in self.bow])
+        vector = np.mean([
+            self._weighting[code] * model[w] for code, w in self.bow
+        ], axis=0)
+        self.vector = vector / sum(
+            [self._weighting[code] for code, _ in self.bow]
+        )
 
     def _set_words(self):
         self.words = [w for _, w in self.bow]
 
 
 class CategoryManager:
     _stop_words = None
     _model = None
     _classifier_bow = None
     _topic_vectors = None
 
     def __init__(self, word_model, settings):
         self._categories = SortedDict()
         self._model = WModel(word_model)
-        stopwords_language = settings.get("STOPWORDS_LANGUAGE", DEFAULT_STOPWORDS_LANGUAGE)
+        stopwords_language = settings.get(
+            "STOPWORDS_LANGUAGE",
+            DEFAULT_STOPWORDS_LANGUAGE
+        )
         extra_stopwords = (
             settings
                 .get("EXTRA_STOPWORDS", {})
                 .get(stopwords_language, EXTRA_STOPWORDS[stopwords_language])
         )
         self._stop_words = (
             stopwords.words(stopwords_language) + extra_stopwords
@@ -76,28 +83,30 @@
         self._ltzr = WordNetLemmatizer()
         self.all_words = {}
         self._weighting = settings.get("WEIGHTING", DEFAULT_WEIGHTING)
         self._threshold = settings.get("CATEGORY_THRESHOLD", DEFAULT_THRESHOLD)
 
     def set_all_words(self, all_words):
         total = sum(all_words.values())
-        scale = lambda c: 0.25 + math.exp(1000 * (1 - c) / total) * 0.75
+        def scale(c):
+            return 0.25 + math.exp(1000 * (1 - c) / total) * 0.75
         self.all_words = {w: scale(c) for w, c in all_words.items()}
 
     def _scale_by_frequency(self, word):
         lword = self._ltzr.lemmatize(word)
         if lword in self.all_words:
             scale = self.all_words[lword]
             return scale
 
         return 1.0
 
     def add_categories_from_bow(self, name, classifier_bow):
         self._categories[name] = SortedDict(
-            (k, Category(k, bow, self._model, self._weighting)) for k, bow in classifier_bow.items()
+            (k, Category(k, bow, self._model, self._weighting))
+            for k, bow in classifier_bow.items()
         )
 
     def closest(self, text, cat, classifier_bow_vec):
         word_list = set(sum(self.strip_document(text), []))
         word_scores = [
             (
                 word,
@@ -135,15 +144,15 @@
         cat = self._categories[category_group][category]
 
         clean = self.strip_document(sentence)
 
         if not clean:
             return []
 
-        classifiers = {w: WEIGHTING[code] * self._model[w] for code, w in cat.bow}
+        classifiers = {w: self._weighting[code] * self._model[w] for code, w in cat.bow}
 
         tags = {}
         for words in clean:
             if not words:
                 continue
 
             vec = np.mean([self._model[w] for w in words], axis=0)
@@ -156,15 +165,15 @@
                 },
             }
 
         return {
             "tags": tags,
             "vector": np.linalg.norm(cat.vector),
             "significance": self._significance_for_vector(cat.vector),
-            "weightings": {w: WEIGHTING[code] for code, w in cat.bow},
+            "weightings": {w: self._weighting[code] for code, w in cat.bow},
         }
 
     @staticmethod
     def _significance_for_vector(vector):
         return min(max(0.5, np.linalg.norm(vector) * 1e2), 1.25)
 
     def test(self, sentence, category_group="dtcats"):
```

## bonn/taxonomy.py

```diff
@@ -1,10 +1,9 @@
 from sortedcontainers import SortedDict
 import json
-import numpy as np
 
 
 def get_taxonomy(taxonomy_location):
     with open(taxonomy_location, "r") as f:
         taxonomy = json.load(f)
     return taxonomy
```

## bonn/extract.py

```diff
@@ -5,15 +5,15 @@
 from collections import Counter
 from elasticsearch2 import Elasticsearch
 from elasticsearch_dsl import Search, Q
 from nltk import download
 from tqdm import tqdm
 from nltk.stem.wordnet import WordNetLemmatizer
 
-from bonn import FfModel
+from ._bonn import FfModel
 from .category_manager import CategoryManager
 from .taxonomy import get_taxonomy, taxonomy_to_categories, categories_to_classifier_bow
 
 DEFAULT_TAXONOMY_LOCATION = "/app/test_data/taxonomy.json"
 
 
 def get_datasets(cm, classifier_bow, settings):
@@ -37,46 +37,46 @@
 
     s = Search(using=client, index=elasticsearch_index).filter(
         "bool", must=[Q("exists", field="description.title")]
     )
     expecting = s.count()
     size = 50
     s = s.params(size=size)
-    n = 0
     all_words = Counter()
     with tqdm(total=expecting) as pbar:
         for hit in s.scan():
             try:
-                datasets[hit.description.title] = {
+                title = hit.description.title
+                datasets[title] = {
                     "category": tuple(hit.uri.split("/")[1:4]),
-                    "text": f"{hit.description.title} {hit.description.metaDescription}",
+                    "text": f"{title} {hit.description.metaDescription}",
                 }
-                cat = datasets[hit.description.title]["category"]
+                cat = datasets[title]["category"]
                 if cat not in classifier_bow_vec and cat[:-1] in classifier_bow_vec:
                     cat = cat[:-1]
-                    datasets[hit.description.title]["category"] = cat
+                    datasets[title]["category"] = cat
 
-                datasets[hit.description.title]["bow"] = cm.closest(
-                    datasets[hit.description.title]["text"], cat, classifier_bow_vec
+                datasets[title]["bow"] = cm.closest(
+                    datasets[title]["text"], cat, classifier_bow_vec
                 )
                 document = (
-                    hit.description.title
+                    title
                     + " "
-                    + datasets[hit.description.title]["text"]
+                    + datasets[title]["text"]
                 )
                 all_words.update(
                     {
                         ltzr.lemmatize(v)
                         for v in set(sum(cm.strip_document(document), []))
                     }
                 )
-                datasets[hit.description.title]["bow"] = cm.closest(
+                datasets[title]["bow"] = cm.closest(
                     document, cat, classifier_bow_vec
                 )
-            except AttributeError as e:
+            except AttributeError:
                 pass
             pbar.update(1)
 
     all_words = {w: v for w, v in all_words.items() if v > 100}
     return datasets, all_words
```

## bonn/utils.py

```diff
@@ -12,11 +12,11 @@
     return value * (scored_list_len - 1) / (scored_list_sum - value)
 
 
 def filter_by_snr(scored_list, snr):
     scored_list_sum = sum(s for s, _ in scored_list)
     scored_list_len = len(scored_list)
     return [
-        (s, l)
-        for s, l in scored_list
-        if _get_snr(s, scored_list_len, scored_list_sum) > snr
+        (score, item)
+        for score, item in scored_list
+        if _get_snr(score, scored_list_len, scored_list_sum) > snr
     ]
```

## Comparing `bonn-0.1.3.dist-info/METADATA` & `bonn-0.1.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: bonn
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: nltk ~=3.7
 Requires-Dist: sortedcontainers ~=2.4.0
 Requires-Dist: elasticsearch2 ~=2.5.1
 Requires-Dist: elasticsearch-dsl ~=2.0
 Requires-Dist: numpy
 Requires-Dist: finalfusion
 Requires-Dist: dynaconf
 License-File: LICENSE.md
 Summary: Created for ONS. Proof-of-concept mmap'd Rust word2vec implementation linked with category matching
+Keywords: nlp,search
 Author-email: Chris Nixon <chris.nixon@flaxandteal.co.uk>, Phil Weir <phil.weir@flaxandteal.co.uk>
+License: MIT
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Source Code, https://github.com/flaxandteal/bonn-py
 
 # bonn-py
 
 NLP Category-Matching tools
 
 A Rust microservice to match queries on the ONS Website to groupings in the ONS taxonomy
```

## Comparing `bonn-0.1.3.dist-info/license_files/LICENSE.md` & `bonn-0.1.4.dist-info/license_files/LICENSE.md`

 * *Files identical despite different names*

