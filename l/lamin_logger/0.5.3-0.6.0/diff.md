# Comparing `tmp/lamin_logger-0.5.3.tar.gz` & `tmp/lamin_logger-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_logger-0.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_logger-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_logger-0.5.3.tar` & `lamin_logger-0.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.5.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.5.3/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.5.3/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.5.3/.gitignore
--rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.5.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.5.3/LICENSE
--rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.5.3/README.md
--rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.5.3/docs/api.md
--rw-r--r--   0        0        0     3652 2023-06-17 12:56:53.174044 lamin_logger-0.5.3/docs/changelog.md
--rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.5.3/docs/index.md
--rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.5.3/docs/quickstart.ipynb
--rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.5.3/lamin-project.yaml
--rw-r--r--   0        0        0      291 2023-06-17 12:56:43.924366 lamin_logger-0.5.3/lamin_logger/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.5.3/lamin_logger/_core.py
--rw-r--r--   0        0        0     7600 2023-06-17 12:43:22.076152 lamin_logger-0.5.3/lamin_logger/_logger.py
--rw-r--r--   0        0        0     4202 2023-06-17 12:43:22.076659 lamin_logger-0.5.3/lamin_logger/_lookup.py
--rw-r--r--   0        0        0     4133 2023-06-17 12:43:22.077076 lamin_logger-0.5.3/lamin_logger/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.5.3/lamin_logger/_python_version.py
--rw-r--r--   0        0        0     2758 2023-06-15 15:21:07.826983 lamin_logger-0.5.3/lamin_logger/_search.py
--rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.5.3/noxfile.py
--rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.5.3/tests/test_base.py
--rw-r--r--   0        0        0     1489 2023-06-17 12:43:22.077768 lamin_logger-0.5.3/tests/test_lookup.py
--rw-r--r--   0        0        0     3464 2023-06-17 12:43:22.078102 lamin_logger-0.5.3/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.5.3/tests/test_notebooks.py
--rw-r--r--   0        0        0     2472 2023-06-17 12:56:11.419218 lamin_logger-0.5.3/tests/test_search.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.6.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.6.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.6.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.6.0/LICENSE
+-rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.6.0/README.md
+-rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.6.0/docs/api.md
+-rw-r--r--   0        0        0     3814 2023-06-19 17:20:57.523889 lamin_logger-0.6.0/docs/changelog.md
+-rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.6.0/docs/index.md
+-rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.6.0/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.6.0/lamin-project.yaml
+-rw-r--r--   0        0        0      291 2023-06-19 17:21:03.326344 lamin_logger-0.6.0/lamin_logger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.6.0/lamin_logger/_core.py
+-rw-r--r--   0        0        0     7600 2023-06-17 12:43:22.076152 lamin_logger-0.6.0/lamin_logger/_logger.py
+-rw-r--r--   0        0        0     4202 2023-06-17 12:43:22.076659 lamin_logger-0.6.0/lamin_logger/_lookup.py
+-rw-r--r--   0        0        0     6306 2023-06-19 17:18:48.694840 lamin_logger-0.6.0/lamin_logger/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.6.0/lamin_logger/_python_version.py
+-rw-r--r--   0        0        0     3056 2023-06-19 17:18:48.695302 lamin_logger-0.6.0/lamin_logger/_search.py
+-rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.6.0/noxfile.py
+-rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.6.0/tests/test_base.py
+-rw-r--r--   0        0        0     1489 2023-06-17 12:43:22.077768 lamin_logger-0.6.0/tests/test_lookup.py
+-rw-r--r--   0        0        0     5093 2023-06-19 17:18:48.695758 lamin_logger-0.6.0/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.6.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2595 2023-06-19 17:18:48.696179 lamin_logger-0.6.0/tests/test_search.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.6.0/PKG-INFO
```

### Comparing `lamin_logger-0.5.3/.github/workflows/build.yml` & `lamin_logger-0.6.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.3/.github/workflows/latest-changes.yml` & `lamin_logger-0.6.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.3/.gitignore` & `lamin_logger-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.3/.pre-commit-config.yaml` & `lamin_logger-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.3/LICENSE` & `lamin_logger-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.3/docs/changelog.md` & `lamin_logger-0.6.0/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✨ Add case_sensitive to map_synonyms | [27](https://github.com/laminlabs/lamin-logger/pull/27) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-19 | 0.6.0
 🧪 Test every line of search | [25](https://github.com/laminlabs/lamin-logger/pull/25) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-17 | 0.5.3
 🚑️ Fix empty string input for `map_synonyms` | [24](https://github.com/laminlabs/lamin-logger/pull/24) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-17 |
 💄 Log to stdout rather than stderr | [23](https://github.com/laminlabs/lamin-logger/pull/23) | [falexwolf](https://github.com/falexwolf) | 2023-06-16 | 0.5.2
 ✨ Lookup can also return sql records | [22](https://github.com/laminlabs/lamin-logger/pull/22) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-15 | 0.5.1
 ✨ Remove loguru and replace with standard (Scanpy-based) logger | [18](https://github.com/laminlabs/lamin-logger/pull/18) | [falexwolf](https://github.com/falexwolf) | 2023-06-15 | 0.5.0
 🚚 Moved search and map_synonyms from bionty here | [21](https://github.com/laminlabs/lamin-logger/pull/21) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-15 | 0.4.0
 🚚 Temporarily added lookup | [20](https://github.com/laminlabs/lamin-logger/pull/20) | [falexwolf](https://github.com/falexwolf) | 2023-06-14 | 0.3.4
```

### Comparing `lamin_logger-0.5.3/docs/quickstart.ipynb` & `lamin_logger-0.6.0/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.3/lamin_logger/_core.py` & `lamin_logger-0.6.0/lamin_logger/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.3/lamin_logger/_logger.py` & `lamin_logger-0.6.0/lamin_logger/_logger.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.3/lamin_logger/_lookup.py` & `lamin_logger-0.6.0/lamin_logger/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.3/lamin_logger/_python_version.py` & `lamin_logger-0.6.0/lamin_logger/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.3/lamin_logger/_search.py` & `lamin_logger-0.6.0/lamin_logger/_search.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from typing import Any, Union
+from typing import Any, Literal, Union
 
 from lamin_logger import logger
 
 
 def search(
     df: Any,
     string: str,
     field: str = "name",
     synonyms_field: Union[str, None] = "synonyms",
     case_sensitive: bool = True,
     return_ranked_results: bool = False,
     synonyms_sep: str = "|",
+    keep: Literal["first", "last", False] = "first",
     tuple_name: str = "SearchResult",
 ) -> Any:
     """Search a given string against a field.
 
     Args:
         string: The input string to match against the field ontology values.
         field: The field against which the input string is matching.
@@ -24,41 +25,47 @@
         return_ranked_results: If True, return all entries ranked by matching ratios.
 
     Returns:
         Best match record of the input string.
     """
     import pandas as pd
 
-    from ._map_synonyms import explode_aggregated_column_to_expand
+    from ._map_synonyms import explode_aggregated_column_to_map
 
     def _fuzz_ratio(string: str, iterable: pd.Series, case_sensitive: bool = True):
         from rapidfuzz import fuzz, utils
 
-        if case_sensitive:
-            processor = None
-        else:
-            processor = utils.default_process
+        processor = None if case_sensitive else utils.default_process
         return iterable.apply(lambda x: fuzz.ratio(string, x, processor=processor))
 
+    # search against each of the synonyms
     if (synonyms_field in df.columns) and (synonyms_field != field):
-        df_exp = explode_aggregated_column_to_expand(
+        mapper = explode_aggregated_column_to_map(
             df,
-            aggregated_col=synonyms_field,  # type:ignore
+            agg_col=synonyms_field,  # type:ignore
             target_col=field,
+            keep=keep,
             sep=synonyms_sep,
-        ).reset_index()
+        )
+        if keep is False:
+            mapper = mapper.explode()
+        for v in df[field]:
+            if v not in mapper:
+                mapper.loc[v] = v
+        df_exp = mapper.reset_index()
         target_column = synonyms_field
     else:
         if synonyms_field == field:
             logger.warning(
                 "Input field is the same as synonyms field, skipping synonyms matching"
             )
         df_exp = df.copy()
         target_column = field
 
+    # add matching scores as a __ratio__ column
     df_exp["__ratio__"] = _fuzz_ratio(
         string=string, iterable=df_exp[target_column], case_sensitive=case_sensitive
     )
     df_exp_grouped = (
         df_exp.groupby(field).max().sort_values("__ratio__", ascending=False)
     )
     df_exp_grouped = df_exp_grouped[df_exp_grouped.index.isin(df[field])]
```

### Comparing `lamin_logger-0.5.3/pyproject.toml` & `lamin_logger-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.3/tests/test_lookup.py` & `lamin_logger-0.6.0/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.3/tests/test_search.py` & `lamin_logger-0.6.0/tests/test_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,19 @@
     res = search(df=df, string="P cells")
     assert res.name == "nodal myocyte"
 
     res = search(df=df, synonyms_field=None, string="P cells")
     assert res.name == "PP cell"
 
 
+def test_search_keep(df):
+    res = search(df=df, string="enteroendocrine", keep=False)
+    assert res.name == "PP cell"
+
+
 def test_search_return_df(df):
     res = search(df=df, string="P cells", return_ranked_results=True)
     assert res.shape == (4, 4)
     assert res.iloc[0].name == "nodal myocyte"
 
 
 def test_search_return_tie_results(df):
```

### Comparing `lamin_logger-0.5.3/PKG-INFO` & `lamin_logger-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_logger
-Version: 0.5.3
+Version: 0.6.0
 Summary: Logging setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

