# Comparing `tmp/event2vec-0.0.4.tar.gz` & `tmp/event2vec-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event2vec-0.0.4.tar", max compression
+gzip compressed data, was "event2vec-0.0.41.tar", max compression
```

## Comparing `event2vec-0.0.4.tar` & `event2vec-0.0.41.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    15731 2023-03-14 22:29:01.448203 event2vec-0.0.4/LICENSE
--rw-r--r--   0        0        0      762 2023-03-14 22:29:01.448203 event2vec-0.0.4/README.md
--rw-r--r--   0        0        0      242 2023-03-14 22:29:01.448203 event2vec-0.0.4/bin/config.cfg
--rw-r--r--   0        0        0     5993 2023-04-21 19:43:26.765843 event2vec-0.0.4/bin/submit_i2b2.py
--rw-r--r--   0        0        0     5384 2023-04-21 19:43:24.325844 event2vec-0.0.4/bin/submit_omop.py
--rw-r--r--   0        0        0       17 2023-03-14 22:29:01.778203 event2vec-0.0.4/event2vec/__init__.py
--rw-r--r--   0        0        0     1148 2023-03-14 22:29:01.778203 event2vec-0.0.4/event2vec/concept_proximity.py
--rw-r--r--   0        0        0     1411 2023-05-25 16:23:01.245183 event2vec-0.0.4/event2vec/config.py
--rw-r--r--   0        0        0     5203 2023-05-31 16:16:31.163153 event2vec-0.0.4/event2vec/cooccurrence_matrix_pandas.py
--rw-r--r--   0        0        0     5296 2023-06-19 14:43:33.718449 event2vec-0.0.4/event2vec/cooccurrence_matrix_polars.py
--rw-r--r--   0        0        0     7099 2023-04-22 02:17:00.822933 event2vec-0.0.4/event2vec/cooccurrence_matrix_spark.py
--rw-r--r--   0        0        0     1818 2023-05-25 19:08:52.021601 event2vec-0.0.4/event2vec/datasets.py
--rw-r--r--   0        0        0    14860 2023-06-19 14:43:33.718449 event2vec-0.0.4/event2vec/event_transformer.py
--rw-r--r--   0        0        0     6425 2023-03-14 22:29:01.778203 event2vec-0.0.4/event2vec/nomenclatures.py
--rw-r--r--   0        0        0     6867 2023-05-25 20:21:37.250039 event2vec-0.0.4/event2vec/svd_ppmi.py
--rw-r--r--   0        0        0     4064 2023-06-19 14:43:33.718449 event2vec-0.0.4/event2vec/utils.py
--rw-r--r--   0        0        0     4621 2023-06-19 14:43:53.078448 event2vec-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2953 1970-01-01 00:00:00.000000 event2vec-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    15731 2023-03-14 22:29:01.448203 event2vec-0.0.41/LICENSE
+-rw-r--r--   0        0        0      762 2023-03-14 22:29:01.448203 event2vec-0.0.41/README.md
+-rw-r--r--   0        0        0      242 2023-03-14 22:29:01.448203 event2vec-0.0.41/bin/config.cfg
+-rw-r--r--   0        0        0     5993 2023-04-21 19:43:26.765843 event2vec-0.0.41/bin/submit_i2b2.py
+-rw-r--r--   0        0        0     5384 2023-04-21 19:43:24.325844 event2vec-0.0.41/bin/submit_omop.py
+-rw-r--r--   0        0        0       17 2023-03-14 22:29:01.778203 event2vec-0.0.41/event2vec/__init__.py
+-rw-r--r--   0        0        0     1148 2023-03-14 22:29:01.778203 event2vec-0.0.41/event2vec/concept_proximity.py
+-rw-r--r--   0        0        0     1411 2023-05-25 16:23:01.245183 event2vec-0.0.41/event2vec/config.py
+-rw-r--r--   0        0        0     5203 2023-05-31 16:16:31.163153 event2vec-0.0.41/event2vec/cooccurrence_matrix_pandas.py
+-rw-r--r--   0        0        0     5296 2023-06-19 14:43:33.718449 event2vec-0.0.41/event2vec/cooccurrence_matrix_polars.py
+-rw-r--r--   0        0        0     7099 2023-04-22 02:17:00.822933 event2vec-0.0.41/event2vec/cooccurrence_matrix_spark.py
+-rw-r--r--   0        0        0     1848 2023-06-19 15:48:12.938080 event2vec-0.0.41/event2vec/datasets.py
+-rw-r--r--   0        0        0    15608 2023-06-19 15:50:02.368083 event2vec-0.0.41/event2vec/event_transformer.py
+-rw-r--r--   0        0        0     6425 2023-03-14 22:29:01.778203 event2vec-0.0.41/event2vec/nomenclatures.py
+-rw-r--r--   0        0        0     6867 2023-05-25 20:21:37.250039 event2vec-0.0.41/event2vec/svd_ppmi.py
+-rw-r--r--   0        0        0     4315 2023-06-19 15:42:20.098117 event2vec-0.0.41/event2vec/utils.py
+-rw-r--r--   0        0        0     4622 2023-06-19 15:50:38.108078 event2vec-0.0.41/pyproject.toml
+-rw-r--r--   0        0        0     2954 1970-01-01 00:00:00.000000 event2vec-0.0.41/PKG-INFO
```

### Comparing `event2vec-0.0.4/LICENSE` & `event2vec-0.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.4/README.md` & `event2vec-0.0.41/README.md`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.4/bin/submit_i2b2.py` & `event2vec-0.0.41/bin/submit_i2b2.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.4/bin/submit_omop.py` & `event2vec-0.0.41/bin/submit_omop.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.4/event2vec/concept_proximity.py` & `event2vec-0.0.41/event2vec/concept_proximity.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.4/event2vec/config.py` & `event2vec-0.0.41/event2vec/config.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.4/event2vec/cooccurrence_matrix_pandas.py` & `event2vec-0.0.41/event2vec/cooccurrence_matrix_pandas.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.4/event2vec/cooccurrence_matrix_polars.py` & `event2vec-0.0.41/event2vec/cooccurrence_matrix_polars.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.4/event2vec/cooccurrence_matrix_spark.py` & `event2vec-0.0.41/event2vec/cooccurrence_matrix_spark.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.4/event2vec/datasets.py` & `event2vec-0.0.41/event2vec/datasets.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         {
             COLNAME_PERSON: [2, 3],
             "y": [0, 1],
             COLNAME_FOLLOWUP_START: [
                 "2021-01-08 00:00:00",
                 "2021-01-18 00:00:00",
             ],
+            "gender": [0, 1],
         }
     )
     person[COLNAME_FOLLOWUP_START] = pd.to_datetime(
         person[COLNAME_FOLLOWUP_START]
     )
     event = pd.DataFrame(
         {
```

### Comparing `event2vec-0.0.4/event2vec/event_transformer.py` & `event2vec-0.0.41/event2vec/event_transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     COLNAME_VALUE,
     OBSERVATION_END,
     OBSERVATION_START,
 )
 from event2vec.svd_ppmi import event2vec
 from event2vec.utils import (
     DataFrameType,
+    check_colnames_subset,
     to,
     to_lazyframe,
     to_pandas,
     to_polars,
 )
 
 
@@ -80,22 +81,29 @@
         self.colname_demographics = colname_demographics
         self.decay_half_life_in_days = decay_half_life_in_days
 
     def fit(
         self,
         X: pd.DataFrame,
         y: pd.DataFrame = None,
-        static_features: List[str] = None,
     ):
         if isinstance(self.event, pd.DataFrame):
             self.event = to_polars(self.event)
         X_event = self.event.join(
             to_polars(X[[COLNAME_PERSON]]), on=COLNAME_PERSON, how="inner"
         )
-        self.static_features_ = static_features
+
+        if check_colnames_subset(
+            colnames_subset=self.colname_demographics, colnames=X.columns
+        ):
+            self.colname_demographics_ = self.colname_demographics
+        else:
+            raise ValueError(
+                f"Demographics columns {self.colname_demographics} not in X"
+            )
         if self.vocabulary is None:
             self.vocabulary_ = build_vocabulary(
                 event=X_event,
                 n_min_events=self.n_min_events,
             )
         else:
             self.vocabulary_ = self.vocabulary
@@ -116,16 +124,16 @@
 
         X_columns = []
         for decay in self.decay_half_life_in_days:
             for code_ in self.vocabulary_:
                 X_columns.append(f"{code_}__decay_{decay}")
 
         X_df = pd.DataFrame(X_counts, columns=X_columns)
-        if self.static_features_ is not None:
-            X_df = pd.concat([X_[self.static_features_], X_df], axis=1)
+        if self.colname_demographics_ is not None:
+            X_df = pd.concat([X_[self.colname_demographics_], X_df], axis=1)
 
         return X_df
 
 
 class Event2vecFeaturizer(EventTransformerMixin, BaseEstimator):
     """
     Transformer for the event2vec model.
@@ -163,22 +171,28 @@
         self.colname_demographics = colname_demographics
         self.decay_half_life_in_days = decay_half_life_in_days
 
     def fit(
         self,
         X: pd.DataFrame,
         y: pd.DataFrame = None,
-        static_features: List[str] = None,
     ):
         if isinstance(self.event, pd.DataFrame):
             self.event = to_polars(self.event)
         X_event = self.event.join(
             to_polars(X[[COLNAME_PERSON]]), on=COLNAME_PERSON, how="inner"
         )
-        self.static_features_ = static_features
+        if check_colnames_subset(
+            colnames_subset=self.colname_demographics, colnames=X.columns
+        ):
+            self.colname_demographics_ = self.colname_demographics
+        else:
+            raise ValueError(
+                f"Demographics columns {self.colname_demographics} not in X"
+            )
         if self.vocabulary is None:
             self.vocabulary_ = build_vocabulary(
                 event=X_event,
                 n_min_events=self.n_min_events,
             )
         else:
             self.vocabulary_ = self.vocabulary
@@ -234,17 +248,17 @@
 
         X_embedded_columns = []
         embedding_dimension = embedding_array_.shape[0]
         for decay_ in self.decay_half_life_in_days:
             for i in range(embedding_dimension):
                 X_embedded_columns.append(f"dim_{i}__decay_{decay_}")
         X_embedded_df = pd.DataFrame(X_embedded, columns=X_embedded_columns)
-        if self.static_features_ is not None:
+        if self.colname_demographics_ is not None:
             X_embedded_df = pd.concat(
-                [X_[self.static_features_], X_embedded_df], axis=1
+                [X_[self.colname_demographics_], X_embedded_df], axis=1
             )
         return X_embedded_df
 
 
 class Event2vecPretrained(Event2vecFeaturizer):
     def __init__(
         self,
@@ -267,29 +281,35 @@
         else:
             self.embeddings = embeddings
 
     def fit(
         self,
         X: pd.DataFrame,
         y: pd.DataFrame = None,
-        static_features: List[str] = None,
     ):
         if isinstance(self.event, pd.DataFrame):
             self.event = to_polars(self.event)
         X_event = self.event.join(
             to_polars(X[[COLNAME_PERSON]]), on=COLNAME_PERSON, how="inner"
         )
-        self.static_features_ = static_features
+        if check_colnames_subset(
+            colnames_subset=self.colname_demographics, colnames=X.columns
+        ):
+            self.colname_demographics_ = self.colname_demographics
+        else:
+            raise ValueError(
+                f"Demographics columns {self.colname_demographics} not in X"
+            )
         if self.vocabulary is None:
-            vocabulary = build_vocabulary(
+            self.vocabulary = build_vocabulary(
                 event=X_event,
                 n_min_events=self.n_min_events,
             )
         self.vocabulary_ = list(
-            set(self.embeddings.columns).intersection(set(vocabulary))
+            set(self.embeddings.columns).intersection(set(self.vocabulary))
         )
         #
         self.embedding_ = self.embeddings
         return self
 
 
 ## Utils ##
```

### Comparing `event2vec-0.0.4/event2vec/nomenclatures.py` & `event2vec-0.0.41/event2vec/nomenclatures.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.4/event2vec/svd_ppmi.py` & `event2vec-0.0.41/event2vec/svd_ppmi.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.4/event2vec/utils.py` & `event2vec-0.0.41/event2vec/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -147,7 +147,14 @@
         return to_polars(df)
     elif backend == pd.DataFrame:
         return to_pandas(df)
     else:
         raise ValueError(
             f"backend must be one of {[pl.LazyFrame, pl.DataFrame, pd.DataFrame]}, got {backend} instead"
         )
+
+
+def check_colnames_subset(colnames_subset: List[str], colnames: List[str]):
+    if colnames_subset is None:
+        return True
+    intersect_columns = set(colnames_subset).intersection(colnames)
+    return intersect_columns == set(colnames_subset)
```

### Comparing `event2vec-0.0.4/pyproject.toml` & `event2vec-0.0.41/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "event2vec"
-version = "0.0.4"
+version = "0.0.41"
 description = "event2vec"
 authors = ["Matthieu Doutreligne <matt.dout@gmail.com>"]
 license = "EUPL-v1.2"
 readme = "README.md"
 repository = "https://gitlab.com/strayMat/event2vec"
 homepage = "https://gitlab.com/strayMat/event2vec"
 include = ["bin"]
```

### Comparing `event2vec-0.0.4/PKG-INFO` & `event2vec-0.0.41/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event2vec
-Version: 0.0.4
+Version: 0.0.41
 Summary: event2vec
 Home-page: https://gitlab.com/strayMat/event2vec
 License: EUPL-v1.2
 Author: Matthieu Doutreligne
 Author-email: matt.dout@gmail.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: Intended Audience :: Developers
```

