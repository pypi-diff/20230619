# Comparing `tmp/krisi-1.1.0.tar.gz` & `tmp/krisi-1.1.1.tar.gz`

## Comparing `krisi-1.1.0.tar` & `krisi-1.1.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-1.1.0/.flake8
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-1.1.0/.isort.cfg
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 krisi-1.1.0/mkdocs.yaml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-1.1.0/.vscode/launch.json
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 krisi-1.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/analyse/__init__.py
--rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/analyse/correlations.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/analyse/dataset.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/analyse/utils.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/__init__.py
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/assertions.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/compare.py
--rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/group.py
--rw-r--r--   0        0        0    13942 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/metric.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/score.py
--rw-r--r--   0        0        0    23731 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/scorecard.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/type.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/utils.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/library/__init__.py
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/library/benchmarking.py
--rw-r--r--   0        0        0    12386 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/library/default_metrics_classification.py
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/library/default_metrics_regression.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/library/diagrams.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/library/metric_wrappers.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/__init__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/console.py
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/graph.py
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/interactive.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/pdf.py
--rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/report.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/type.py
--rw-r--r--   0        0        0     6582 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/vizualise.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/library/console/diagrams.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.css
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.html
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/console_plot.py
--rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/data.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/enums.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/environment.py
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/io.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/iterable_helpers.py
--rw-r--r--   0        0        0     6973 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/printing.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/state.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/devutils/environment_checks.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/devutils/generate_from_examples.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/devutils/timing.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/devutils/type.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 krisi-1.1.0/.gitignore
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-1.1.0/LICENSE
--rw-r--r--   0        0        0    61727 2020-02-02 00:00:00.000000 krisi-1.1.0/README.md
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 krisi-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    66463 2020-02-02 00:00:00.000000 krisi-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-1.1.1/.flake8
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-1.1.1/.isort.cfg
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 krisi-1.1.1/mkdocs.yaml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-1.1.1/.vscode/launch.json
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 krisi-1.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/sharedtypes.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/analyse/__init__.py
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/analyse/correlations.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/analyse/dataset.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/analyse/utils.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/__init__.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/assertions.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/compare.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/group.py
+-rw-r--r--   0        0        0    13443 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/metric.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/score.py
+-rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/scorecard.py
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/type.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/utils.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/library/__init__.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/library/benchmarking.py
+-rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/library/default_metrics_classification.py
+-rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/library/default_metrics_regression.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/library/diagrams.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/library/metric_wrappers.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/__init__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/console.py
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/graph.py
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/interactive.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/pdf.py
+-rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/report.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/type.py
+-rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/vizualise.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/library/console/diagrams.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.css
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.html
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/console_plot.py
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/data.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/enums.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/environment.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/io.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/iterable_helpers.py
+-rw-r--r--   0        0        0     6973 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/printing.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/state.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/devutils/environment_checks.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/devutils/generate_from_examples.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/devutils/timing.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 krisi-1.1.1/.gitignore
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-1.1.1/LICENSE
+-rw-r--r--   0        0        0    61727 2020-02-02 00:00:00.000000 krisi-1.1.1/README.md
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 krisi-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    66463 2020-02-02 00:00:00.000000 krisi-1.1.1/PKG-INFO
```

### Comparing `krisi-1.1.0/mkdocs.yaml` & `krisi-1.1.1/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/.vscode/settings.json` & `krisi-1.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/analyse/correlations.py` & `krisi-1.1.1/src/krisi/analyse/correlations.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
 def plot_corr_over_time(
     df: pd.DataFrame,
     window: int,
     step: int = 1,
     name: str = "",
     save_or_display: List[Literal["save", "display"]] = ["display"],
-    save_location: str = "structured_data/plots",
+    save_location: str = "output/structured_data/plots",
     top_k: int = 2,
 ) -> None:
     (
         coor_unrolled_in_time,
         corr_std,
         corr_mean,
     ) = get_rolled_corr_metrics(df, window, step)
```

### Comparing `krisi-1.1.0/src/krisi/analyse/dataset.py` & `krisi-1.1.1/src/krisi/analyse/dataset.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/evaluate/assertions.py` & `krisi-1.1.1/src/krisi/evaluate/assertions.py`

 * *Files 11% similar despite different names*

```diff
@@ -73,15 +73,21 @@
 
 def infer_dataset_type(y: Targets) -> DatasetType:
     # TODO: Should work with booleans
     def infer_exact_type(is_classification: bool, y: Targets) -> DatasetType:
         if is_classification is False:
             return DatasetType.regression
         if len(set(y)) == 2:
-            return DatasetType.classification_binary
+            class_1 = y[0]
+            no_of_class_1 = np.count_nonzero(y == class_1)
+            ratio = no_of_class_1 / len(y)
+            if ratio < 0.2 or ratio > 0.8:
+                return DatasetType.classification_binary_imbalanced
+            else:
+                return DatasetType.classification_binary_balanced
         else:
             return DatasetType.classification_multiclass
 
     if isinstance(y, pd.Series):
         y = y.to_numpy()
     if isinstance(y, np.ndarray):
         if hasattr(y[0], "is_integer"):
```

### Comparing `krisi-1.1.0/src/krisi/evaluate/compare.py` & `krisi-1.1.1/src/krisi/evaluate/compare.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/evaluate/group.py` & `krisi-1.1.1/src/krisi/evaluate/group.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,38 +23,41 @@
     postprocess_metric._evaluation(
         metric.result_rolling if rolling else metric.result, sample_weight=sample_weight
     )
     return postprocess_metric
 
 
 class Group(Metric, Generic[MetricResult]):
+    metrics: List[Metric]
+
     def __init__(
         self,
         name: str,
         key: str,
         metrics: List[Metric],
         calculation: Union[str, Calculation] = Calculation.both,
         preprocess_func: Optional[MetricFunction] = None,
         postprocess_funcs: Optional[
             Union[List[PostProcessFunction], PostProcessFunction]
         ] = None,
         purpose: Purpose = Purpose.group,
+        append_key: bool = True,
     ) -> None:
         self.calculation = Calculation.from_str(calculation)
         self.preprocess_func = preprocess_func
         self.postprocess_funcs = (
             wrap_in_list(postprocess_funcs) if postprocess_funcs else None
         )
         self.key = key
         self.name = name
         self.metrics = deepcopy(metrics)
         self.purpose = purpose
-
-        # for metric in self.metrics:
-        #     metric.key = f"{metric.key}_{self.key}"
+        if append_key:
+            for metric in self.metrics:
+                metric.key = f"{metric.key}_{self.key}"
 
     def _preprocess(
         self,
         y: TargetsDS,
         predictions: PredictionsDS,
         probabilities: ProbabilitiesDF,
         sample_weights: WeightsDS,
@@ -90,15 +93,20 @@
                     predictions,
                     probabilities,
                     sample_weight=sample_weight,
                     rolling=rolling,
                 )
 
             all_metrics = all_metrics_
-        return all_metrics
+        self.metrics = all_metrics
+
+        return self.metrics
+
+    def get_all_metrics(self) -> List[Metric]:
+        return self.metrics
 
     def __handle_args_to_pass_in(
         self,
         result: Any,
         y: TargetsDS,
         predictions: PredictionsDS,
         probabilities: ProbabilitiesDF,
@@ -111,43 +119,45 @@
                 else:
                     return [y, probabilities]
             else:
                 return [y, predictions]
         else:
             return result
 
+    def evaluate_rolling_properties(self):
+        for metric in self.metrics:
+            metric.evaluate_rolling_properties()
+
     def evaluate(
         self,
         y: TargetsDS,
         predictions: PredictionsDS,
         probabilities: ProbabilitiesDF,
         sample_weight: WeightsDS,
     ) -> List[Metric]:
         if self.calculation == Calculation.rolling:
             return []
         results = self._preprocess(y, predictions, probabilities, sample_weight)
 
-        all_metrics = []
         for metric in self.metrics:
             args_to_pass = self.__handle_args_to_pass_in(
                 results,
                 y,
                 predictions,
                 probabilities,
                 metric.accepts_probabilities,
             )
             if args_to_pass is not None:
                 metric._evaluation(
                     *args_to_pass,
                     sample_weight=sample_weight,
                 )
-            all_metrics.append(metric)
 
         return self._postprocess(
-            all_metrics,
+            self.metrics,
             y,
             predictions,
             probabilities,
             sample_weight=sample_weight,
             rolling=False,
         )
 
@@ -159,33 +169,31 @@
         sample_weight: WeightsDS,
         rolling_args: Dict[str, Any],
     ) -> List[Metric]:
         if self.calculation == Calculation.single:
             return []
         results = self._preprocess(y, predictions, probabilities, sample_weight)
 
-        all_metrics = []
         for metric in self.metrics:
             args_to_pass = self.__handle_args_to_pass_in(
                 results,
                 y,
                 predictions,
                 probabilities,
                 metric.accepts_probabilities,
             )
             if args_to_pass is not None:
                 metric._rolling_evaluation(
                     *args_to_pass,
                     sample_weight=sample_weight,
                     rolling_args=rolling_args,
                 )
-            all_metrics.append(metric)
 
         return self._postprocess(
-            all_metrics,
+            self.metrics,
             y,
             predictions,
             probabilities,
             sample_weight=sample_weight,
             rolling=True,
         )
```

### Comparing `krisi-1.1.0/src/krisi/evaluate/metric.py` & `krisi-1.1.1/src/krisi/evaluate/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
     def evaluate(
         self,
         y: TargetsDS,
         predictions: PredictionsDS,
         probabilities: Optional[ProbabilitiesDF] = None,
         sample_weight: Optional[WeightsDS] = None,
-    ) -> Metric:
+    ) -> None:
         assert (
             self.func is not None
         ), "`func` has to be set on Metric to calculate result."
         if self.accepts_probabilities:
             if probabilities is not None:
                 self._evaluation(y, probabilities, sample_weight=sample_weight)
             else:
@@ -155,15 +155,14 @@
                     ),
                     key="result",
                 )
         else:
             self._evaluation(y, predictions, sample_weight=sample_weight)
         if sample_weight is not None:
             self.__dict__["diagnostics"] = dict(used_sample_weight=True)
-        return self
 
     @staticmethod
     def __handle_window(
         window: pd.DataFrame,
     ) -> Tuple[Union[dict, Tuple], WeightsDS]:
         sample_weight = (
             window.pop("sample_weight") if "sample_weight" in window else None
@@ -251,15 +250,15 @@
     def evaluate_over_time(
         self,
         y: TargetsDS,
         predictions: PredictionsDS,
         probabilities: Optional[ProbabilitiesDF] = None,
         sample_weight: Optional[WeightsDS] = None,
         rolling_args: dict = dict(),
-    ) -> Metric:
+    ) -> None:
         if self.accepts_probabilities and probabilities is not None:
             self._rolling_evaluation(
                 y=y,
                 predictions=predictions,
                 probabilities=probabilities,
                 sample_weight=sample_weight,
                 rolling_args=rolling_args,
@@ -267,15 +266,14 @@
         else:
             self._rolling_evaluation(
                 y=y,
                 predictions=predictions,
                 sample_weight=sample_weight,
                 rolling_args=rolling_args,
             )
-        return self
 
     def evaluate_rolling_properties(self):
         if check_iterable_with_number(self.result_rolling):
             self.__safe_set(
                 pd.Series(
                     data=dict(
                         mean=np.mean(self.result_rolling),
@@ -316,28 +314,14 @@
         key: str,
     ):
         if self.__dict__[key] is not None:
             raise ValueError("This metric already contains a result.")
         else:
             self.__dict__[key] = result
 
-    # def __add__(self, other):
-    #     result = getattr(self, "result", 0)
-    #     result_rolling = getattr(self, "result_rolling", 0)
-    #     result += other
-    #     result_rolling += other
-
-    # object.__sub__(self, other)
-    # object.__mul__(self, other)
-    # object.__matmul__(self, other)
-    # object.__truediv__(self, other)
-    # object.__floordiv__(self, other)
-    # object.__mod__(self, other)
-    # object.__divmod__(self, other)
-
 
 def create_diagram_rolling(obj: Metric) -> Optional[List[InteractiveFigure]]:
     if obj.plot_funcs_rolling is None:
         logging.info("No plot_funcs_rolling (Plotting Function Rolling) specified")
         return None
     elif isinstance(obj.result_rolling, Exception) or obj.result_rolling is None:
         return None
```

### Comparing `krisi-1.1.0/src/krisi/evaluate/score.py` & `krisi-1.1.1/src/krisi/evaluate/score.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,21 +17,21 @@
     y: Targets,
     predictions: Predictions,
     probabilities: Optional[Probabilities] = None,
     sample_weight: Optional[Weights] = None,
     model_name: Optional[str] = None,
     dataset_name: Optional[str] = None,
     project_name: Optional[str] = None,
-    default_metrics: Optional[List[Metric]] = None,
-    custom_metrics: Optional[List[Metric]] = None,
+    default_metrics: Optional[Union[List[Metric], Metric]] = None,
+    custom_metrics: Optional[Union[List[Metric], Metric]] = None,
     dataset_type: Optional[Union[DatasetType, str]] = None,
     sample_type: SampleTypes = SampleTypes.outofsample,
     calculation: Union[Calculation, str] = Calculation.single,
     rolling_args: Optional[Dict[str, Any]] = None,
-    surpress_warnings: bool = False,
+    raise_exceptions: bool = False,
     **kwargs,
 ) -> ScoreCard:
     """
     Creates a ScoreCard based on the passed in arguments, evaluates and then returns the ScoreCard.
 
     Parameters
     ----------
@@ -92,22 +92,24 @@
         dataset_name=dataset_name,
         project_name=project_name,
         sample_type=sample_type,
         dataset_type=dataset_type,
         default_metrics=default_metrics,
         custom_metrics=custom_metrics,
         rolling_args=rolling_args,
-        surpress_warnings=surpress_warnings,
+        raise_exceptions=raise_exceptions,
         **kwargs,
     )
 
     if calculation == Calculation.single:
         sc.evaluate()
     elif calculation == Calculation.rolling:
         sc.evaluate_over_time()
     elif calculation == Calculation.both:
         sc.evaluate()
         sc.evaluate_over_time()
+
     else:
         raise ValueError(f"Calculation type {calculation} not recognized.")
 
+    sc.cleanup_group()
     return sc
```

### Comparing `krisi-1.1.0/src/krisi/evaluate/scorecard.py` & `krisi-1.1.1/src/krisi/evaluate/scorecard.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,19 @@
     get_summary,
 )
 from krisi.report.report import create_report_from_scorecard
 from krisi.report.type import DisplayModes, InteractiveFigure
 from krisi.utils.environment import is_notebook
 from krisi.utils.io import ensure_path, save_console, save_minimal_summary, save_object
 from krisi.utils.iterable_helpers import (
-    empty_if_None,
+    empty_if_none,
     flatten,
     map_newdict_on_olddict,
     remove_nans,
-    replace_if_None,
+    replace_if_none,
     strip_builtin_functions,
     wrap_in_list,
 )
 from krisi.utils.state import RunType, get_global_state, set_global_state
 
 logger = logging.getLogger("krisi")
 
@@ -140,35 +140,35 @@
         model_description: str = "",
         dataset_name: Optional[str] = None,
         dataset_description: str = "",
         project_name: Optional[str] = None,
         project_description: str = "",
         dataset_type: Optional[Union[DatasetType, str]] = None,
         sample_type: SampleTypes = SampleTypes.outofsample,
-        default_metrics: Optional[List[Metric]] = None,
-        custom_metrics: Optional[List[Metric]] = None,
+        default_metrics: Optional[Union[List[Metric], Metric]] = None,
+        custom_metrics: Optional[Union[List[Metric], Metric]] = None,
         rolling_args: Optional[Dict[str, Any]] = None,
-        surpress_warnings: bool = False,
+        raise_exceptions: bool = False,
     ) -> None:
-        if surpress_warnings:
+        if raise_exceptions:
             state = get_global_state()
-            state.run_type = RunType.dev
+            state.run_type = RunType.test
             set_global_state(state)
 
         dataset_type = DatasetType.from_str(dataset_type) if dataset_type else None
         check_valid_pred_target(y, predictions, sample_weight)
         default_metrics = (
             wrap_in_list(default_metrics) if default_metrics is not None else None
         )
         custom_metrics = (
             wrap_in_list(custom_metrics) if custom_metrics is not None else None
         )
 
         check_no_duplicate_metrics(
-            empty_if_None(default_metrics) + empty_if_None(custom_metrics)
+            empty_if_none(default_metrics) + empty_if_none(custom_metrics)
         )
         self.__dict__["y"] = convert_to_series(y, "y")
         self.__dict__["predictions"] = convert_to_series(predictions, "predictions")
         self.__dict__["probabilities"] = (
             rename_probs_columns(ensure_df(probabilities, "probabilities"))
             if probabilities is not None
             else None
@@ -419,41 +419,25 @@
         func_key_evaluate: Literal["evaluate", "evaluate_over_time"],
         result_key: Literal["result", "result_rolling"],
         defaults: bool = True,
         rolling_args: Optional[Dict[str, Any]] = dict(),
     ):
         for metric in self.get_all_metrics(defaults=defaults):
             if metric.restrict_to_sample is not self.sample_type:
-                if isinstance(metric, Group):
-                    group = metric
-                    for metric_in_group in getattr(group, func_key_evaluate)(
-                        self.y,
-                        self.predictions,
-                        self.probabilities,
-                        self.sample_weight,
-                        **rolling_args,
-                    ):
-                        if metric_in_group.key not in self.__dict__:
-                            metric_in_group._from_group = True
-                            self[metric_in_group.key] = metric_in_group
-                        else:
-                            self[metric_in_group.key] = {
-                                result_key: metric_in_group.result,
-                                "_from_group": True,
-                            }
-                else:
-                    getattr(metric, func_key_evaluate)(
-                        self.y,
-                        self.predictions,
-                        self.probabilities,
-                        self.sample_weight,
-                        **rolling_args,
-                    )
-            if func_key_evaluate == "evaluate_over_time":
-                metric.evaluate_rolling_properties()
+                getattr(metric, func_key_evaluate)(
+                    self.y,
+                    self.predictions,
+                    self.probabilities,
+                    self.sample_weight,
+                    **rolling_args,
+                )
+
+    def evaluate_rolling_properties(self):
+        for metric in self.get_all_metrics(defaults=True):
+            metric.evaluate_rolling_properties()
 
     def evaluate(self, defaults: bool = True) -> None:
         """
         Evaluates `Metric`s present on the `ScoreCard`
 
         Parameters
         ----------
@@ -489,14 +473,15 @@
         """
         self.__evaluate(
             "evaluate_over_time",
             "result_rolling",
             defaults=defaults,
             rolling_args={"rolling_args": self.rolling_args},
         )
+        self.evaluate_rolling_properties()
 
     def print(
         self,
         mode: Union[str, PrintMode, List[PrintMode], List[str]] = PrintMode.extended,
         with_info: bool = False,
         with_parameters: bool = True,
         with_diagnostics: bool = False,
@@ -549,14 +534,31 @@
             if isinstance(to_display, (pd.DataFrame, pd.Series)) and is_notebook():
                 from IPython.display import display
 
                 display(to_display)
             else:
                 print(to_display)
 
+    def cleanup_group(self) -> None:
+        for metric in self.get_all_metrics(defaults=True):
+            if isinstance(metric, Group):
+                group = metric
+                for metric_in_group in group.get_all_metrics():
+                    if metric_in_group.key not in self.__dict__:
+                        metric_in_group._from_group = True
+                        self[metric_in_group.key] = metric_in_group
+                    else:
+                        self[metric_in_group.key] = {
+                            f"result_{group.key}": metric_in_group.__dict__["result"],
+                            f"result_rolling_{group.key}": metric_in_group.__dict__[
+                                "result_rolling"
+                            ],
+                            "_from_group": True,
+                        }
+
     def save(
         self,
         with_info: bool = False,
         with_parameters: bool = True,
         with_diagnostics: bool = False,
         save_modes: List[Union[SaveModes, str]] = [
             SaveModes.minimal,
@@ -568,15 +570,15 @@
     ) -> "ScoreCard":
         if override_base_path is None:
             if timestamp_no_overwrite is False:
                 dir_model_name = self.metadata.model_name
             else:
                 dir_model_name = datetime.datetime.now().strftime("%H-%M-%S-%f")
 
-        path = replace_if_None(
+        path = replace_if_none(
             override_base_path,
             os.path.join(
                 self.metadata.save_path,
                 os.path.join(
                     PathConst.default_save_output_path,
                     Path(dir_model_name),
                 ),
@@ -613,27 +615,27 @@
         ],
         html_template_url: Path = PathConst.html_report_template_url,
         css_template_url: Path = PathConst.css_report_template_url,
         author: str = "",
         report_title: Optional[str] = None,
         override_base_path: Optional[Path] = None,
     ) -> None:
-        save_path = replace_if_None(override_base_path, self.metadata.save_path)
+        save_path = replace_if_none(override_base_path, self.metadata.save_path)
         ensure_path(save_path)
 
         display_modes = [
             DisplayModes.from_str(mode) for mode in wrap_in_list(display_modes)
         ]
         report = create_report_from_scorecard(
             self,
             display_modes,
             html_template_url,
             css_template_url,
             author=author,
-            report_title=replace_if_None(
+            report_title=replace_if_none(
                 report_title, f"Report on {self.metadata.project_name}"
             ),
             save_path=save_path,
         )
         report.generate_launch()
```

### Comparing `krisi-1.1.0/src/krisi/evaluate/type.py` & `krisi-1.1.1/src/krisi/evaluate/type.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,29 +50,19 @@
 
 
 class SampleTypes(Enum):
     insample = "insample"
     outofsample = "outofsample"
 
 
-class Calculation(Enum):
+class Calculation(ParsableEnum):
     single = "single"
     rolling = "rolling"
     both = "both"
 
-    @staticmethod
-    def from_str(value: Union[str, Calculation]) -> Calculation:
-        if isinstance(value, Calculation):
-            return value
-        for calc in Calculation:
-            if calc.value == value:
-                return calc
-        else:
-            raise ValueError(f"Unknown Calculation: {value}")
-
 
 class SaveModes(Enum):
     svg = "svg"
     html = "html"
     text = "text"
     obj = "obj"
     minimal = "minimal"
@@ -107,54 +97,36 @@
             self.save_path = Path(
                 os.path.join(PathConst.default_eval_output_path, item)
             )
 
         super().__setattr__(key, item)
 
 
-class PrintMode(Enum):
+class PrintMode(ParsableEnum):
     extended = "extended"
     minimal = "minimal"
     minimal_table = "minimal_table"
 
-    @staticmethod
-    def from_str(value: Union[str, PrintMode]) -> PrintMode:
-        if isinstance(value, PrintMode):
-            return value
-        for strategy in PrintMode:
-            if strategy.value == value:
-                return strategy
-        else:
-            raise ValueError(f"Unknown PrintMode: {value}")
-
 
 class NamingPrefixes:
     model = "Model_"
     dataset = "Dataset_"
     project = "Project_"
 
 
-class DatasetType(Enum):
+class DatasetType(ParsableEnum):
     regression = "regression"
-    classification_binary = "classification_binary"
+    classification_binary_balanced = "classification_binary_balanced"
+    classification_binary_imbalanced = "classification_binary_imbalanced"
     classification_multiclass = "classification_multiclass"
 
-    @staticmethod
-    def from_str(value: Union[str, DatasetType]) -> DatasetType:
-        if isinstance(value, DatasetType):
-            return value
-        for strategy in DatasetType:
-            if strategy.value == value:
-                return strategy
-        else:
-            raise ValueError(f"Unknown DatasetType: {value}")
-
     def is_classification(self):
         return self in [
-            DatasetType.classification_binary,
+            DatasetType.classification_binary_balanced,
+            DatasetType.classification_binary_imbalanced,
             DatasetType.classification_multiclass,
         ]
 
 
 class Purpose(ParsableEnum):
     objective = "objective"
     loss = "loss"
```

### Comparing `krisi-1.1.0/src/krisi/evaluate/utils.py` & `krisi-1.1.1/src/krisi/evaluate/utils.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/evaluate/library/__init__.py` & `krisi-1.1.1/src/krisi/evaluate/library/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from typing import List
 
 from krisi.evaluate.metric import Metric
 from krisi.evaluate.type import DatasetType
 
 from .default_metrics_classification import (
-    binary_classification_metrics,
-    binary_classification_metrics_benchmarking,
+    binary_classification_balanced_metrics,
+    binary_classification_imbalanced_metrics,
+    binary_classification_metrics_balanced_benchmarking,
+    binary_classification_metrics_imbalanced_benchmarking,
     minimal_binary_classification_metrics,
     minimal_multiclass_classification_metrics,
     multiclass_classification_metrics,
 )
 from .default_metrics_regression import (
     all_regression_metrics,
     low_computation_regression_metrics,
     minimal_regression_metrics,
 )
 
 
 def get_default_metrics_for_dataset_type(type: DatasetType) -> List[Metric]:
-    if type == DatasetType.classification_binary:
-        return binary_classification_metrics_benchmarking
+    if type == DatasetType.classification_binary_balanced:
+        return binary_classification_metrics_balanced_benchmarking
+    elif type == DatasetType.classification_binary_imbalanced:
+        return binary_classification_metrics_imbalanced_benchmarking
     elif type == DatasetType.classification_multiclass:
         return multiclass_classification_metrics
     elif type == DatasetType.regression:
         return all_regression_metrics
     else:
         raise ValueError(f"Unknown dataset type {type}")
```

### Comparing `krisi-1.1.0/src/krisi/evaluate/library/benchmarking.py` & `krisi-1.1.1/src/krisi/evaluate/library/benchmarking.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         y: TargetsDS,
         predictions: Optional[PredictionsDS],
         probabilities: Optional[ProbabilitiesDF],
         sample_weight: Optional[WeightsDS],
         rolling: bool,
     ) -> List[Metric]:
         if rolling:
-            return []
+            return all_metrics
         benchmark_predictions, benchmark_probabilities = model.predict(y, sample_weight)
 
         for metric in all_metrics:
             if metric.purpose == Purpose.group or metric.purpose == Purpose.diagram:
                 continue
             benchmark_metric = deepcopy(metric)
             benchmark_metric.result = None
```

### Comparing `krisi-1.1.0/src/krisi/evaluate/library/default_metrics_classification.py` & `krisi-1.1.1/src/krisi/evaluate/library/default_metrics_classification.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pandas as pd
 from sklearn.metrics import (
     accuracy_score,
+    balanced_accuracy_score,
+    cohen_kappa_score,
     f1_score,
     log_loss,
     matthews_corrcoef,
     precision_score,
     recall_score,
 )
 
@@ -32,14 +34,25 @@
     info="In multilabel classification, this function computes subset accuracy: the set of labels predicted for a sample must exactly match the corresponding set of labels in y_true. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.accuracy_score.html",
     func=accuracy_score,
     plot_funcs=[(display_single_value, dict(width=750.0))],
     plot_funcs_rolling=(display_time_series, dict(width=1500.0)),
     purpose=Purpose.objective,
 )
 """ ~ """
+accuracy_binary_balanced = Metric[float](
+    name="Balanced Accuracy",
+    key="balanced_accuracy",
+    category=MetricCategories.class_err,
+    info="Compute the balanced accuracy. The balanced accuracy in binary and multiclass classification problems to deal with imbalanced datasets. It is defined as the average of recall obtained on each class.",
+    func=balanced_accuracy_score,
+    plot_funcs=[(display_single_value, dict(width=750.0))],
+    plot_funcs_rolling=(display_time_series, dict(width=1500.0)),
+    purpose=Purpose.objective,
+)
+""" ~ """
 
 recall_binary, recall_macro = [
     Metric[float](
         name=f"Recall ({mode})",
         key=f"recall_{mode}",
         category=MetricCategories.class_err,
         info="The recall is the ratio tp / (tp + fn) where tp is the number of true positives and fn the number of false negatives. The recall is intuitively the ability of the classifier to find all the positive samples.\nThe best value is 1 and the worst value is 0. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.recall_score.html",
@@ -62,14 +75,26 @@
         func=precision_score,
         plot_funcs=[(display_single_value, dict(width=750.0))],
         plot_funcs_rolling=(display_time_series, dict(width=1500.0)),
         purpose=Purpose.objective,
     )
     for mode in ["binary", "macro"]
 ]
+
+kappa = Metric[float](
+    name="Cohen's Kappa",
+    key="kappa",
+    category=MetricCategories.class_err,
+    info="Compute Cohen’s kappa: a statistic that measures inter-annotator agreement. This function computes Cohen’s kappa [1], a score that expresses the level of agreement between two annotators on a classification problem. ",
+    func=cohen_kappa_score,
+    plot_funcs=[(display_single_value, dict(width=750.0))],
+    plot_funcs_rolling=(display_time_series, dict(width=1500.0)),
+    purpose=Purpose.objective,
+)
+
 """~"""
 f_one_score_binary, f_one_score_macro, f_one_score_micro, f_one_score_weighted = [
     Metric[float](
         name=f"F1 Score ({mode})",
         key=f"f_one_score_{mode}",
         category=MetricCategories.class_err,
         info="The F1 score can be interpreted as a harmonic mean of the precision and recall, where an F1 score reaches its best value at 1 and worst score at 0. The relative contribution of precision and recall to the F1 score are equal. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.f1_score.html",
@@ -220,39 +245,65 @@
 #     plot_funcs=[(display_single_value, dict(width=750.0))],
 #     plot_funcs_rolling=(display_time_series, dict(width=1500.0)),
 #     accepts_probabilities=False,
 #     supports_multiclass=True,
 # )
 
 
-binary_classification_metrics = [
+binary_classification_balanced_metrics = [
     accuracy_binary,
     recall_binary,
     precision_binary,
     f_one_score_binary,
     f_one_score_macro,
     f_one_score_micro,
     f_one_score_weighted,
+    kappa,
     matthew_corr,
     brier_score,
     calibration,
     roc_auc_binary_macro,
     roc_auc_binary_micro,
     roc_auc_binary_weighted,
     cross_entropy,
     s_score,
 ]
-benchmarking = Group[pd.Series](
-    name="benchmarking",
-    key="benchmarking",
-    metrics=binary_classification_metrics,
-    postprocess_funcs=[model_benchmarking(RandomClassifier())],
-)
 
-binary_classification_metrics_benchmarking = [benchmarking]
+binary_classification_imbalanced_metrics = [
+    accuracy_binary_balanced,
+    recall_macro,
+    precision_macro,
+    f_one_score_binary,
+    f_one_score_macro,
+    kappa,
+    matthew_corr,
+    brier_score,
+    calibration,
+    roc_auc_binary_macro,
+    cross_entropy,
+]
+binary_classification_metrics_balanced_benchmarking = [
+    Group[pd.Series](
+        name="benchmark",
+        key="benchmark",
+        metrics=binary_classification_balanced_metrics,
+        postprocess_funcs=[model_benchmarking(RandomClassifier())],
+        append_key=False,
+    )
+]
+binary_classification_metrics_imbalanced_benchmarking = [
+    Group[pd.Series](
+        name="benchmark",
+        key="benchmark",
+        metrics=binary_classification_imbalanced_metrics,
+        postprocess_funcs=[model_benchmarking(RandomClassifier())],
+        append_key=False,
+    )
+]
+
 
 """~"""
 minimal_binary_classification_metrics = [accuracy_binary, f_one_score_binary]
 """~"""
 multiclass_classification_metrics = [
     cross_entropy,
     recall_macro,
```

### Comparing `krisi-1.1.0/src/krisi/evaluate/library/default_metrics_regression.py` & `krisi-1.1.1/src/krisi/evaluate/library/default_metrics_regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,28 +173,28 @@
 """ ~ """
 
 all_regression_metrics = [
     mae,
     mape,
     smape,
     mse,
-    # rmse,
+    rmse,
     # rmsle,
     r_two,
     residuals,
     residual_group,
     ljung_box_statistics,
 ]
 """ ~ """
 
 minimal_regression_metrics = [
     mae,
     mape,
     mse,
-    # rmse,
+    rmse,
     rmsle,
     r_two,
 ]
 """ ~ """
 
 low_computation_regression_metrics = [
     metric
```

### Comparing `krisi-1.1.0/src/krisi/evaluate/library/diagrams.py` & `krisi-1.1.1/src/krisi/evaluate/library/diagrams.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/evaluate/library/metric_wrappers.py` & `krisi-1.1.1/src/krisi/evaluate/library/metric_wrappers.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/report/console.py` & `krisi-1.1.1/src/krisi/report/console.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/report/graph.py` & `krisi-1.1.1/src/krisi/report/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         plt.savefig(f"{save_location}/{file_name}_{corr_direction}.png", format="PNG")
     if "display" in save_or_display:
         if not get_global_state().run_type == RunType.test:
             plt.show()
 
 
 def create_animation(
-    path: str = "structured_data/plots", file_suffix: str = "positive"
+    path: str = "output/structured_data/plots", file_suffix: str = "positive"
 ):
     import os
 
     import matplotlib.pyplot as plt
     from matplotlib.animation import FuncAnimation
 
     files = os.listdir(path)
```

### Comparing `krisi-1.1.0/src/krisi/report/interactive.py` & `krisi-1.1.1/src/krisi/report/interactive.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/report/pdf.py` & `krisi-1.1.1/src/krisi/report/pdf.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/report/report.py` & `krisi-1.1.1/src/krisi/report/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from krisi.report.type import DisplayModes, InteractiveFigure, PlotlyInput
 from krisi.report.vizualise import create_subplots_from_mutiple_plots
 from krisi.utils.io import ensure_path
 from krisi.utils.iterable_helpers import (
     flatten,
     group_by_categories,
     remove_nans,
-    replace_if_None,
+    replace_if_none,
     wrap_in_list,
 )
 from krisi.utils.state import RunType, get_global_state
 
 if TYPE_CHECKING:
     from krisi.evaluate.metric import Metric
     from krisi.evaluate.scorecard import ScoreCard
@@ -54,15 +54,15 @@
         self.modes = [DisplayModes.from_str(mode) for mode in wrap_in_list(modes)]
 
         self.figures = figures
         self.global_controllers = global_controllers
         self.html_template_url = html_template_url
         self.css_template_url = css_template_url
         self.get_html_elements = get_html_elements
-        self.save_path = replace_if_None(
+        self.save_path = replace_if_none(
             save_path,
             Path(os.path.join(PathConst.default_eval_output_path, Path(title))),
         )
 
     def generate_launch(self) -> None:
         figures_by_category = group_by_categories(
             self.figures, [el.value for el in MetricCategories]
```

### Comparing `krisi-1.1.0/src/krisi/report/type.py` & `krisi-1.1.1/src/krisi/report/type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import dataclass, field
-from enum import Enum
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 from typing_extensions import Literal
 
+from krisi.utils.enums import ParsableEnum
+
 if TYPE_CHECKING:
     import plotly.graph_objects as go
 
 from krisi.evaluate.type import MetricCategories, MetricResult
 
 PlotFunction = Callable[
     [List[MetricResult], str, Optional[float]],
@@ -37,31 +38,21 @@
     title: Optional[str] = ""
     width: Optional[float] = 900.0
     height: Optional[float] = 600.0
     category: Optional[MetricCategories] = None
     plot_args: Dict[str, Any] = field(default_factory=dict)
 
 
-class DisplayModes(Enum):
+class DisplayModes(ParsableEnum):
     interactive = "interactive"
     pdf = "pdf"
     direct = "direct"
     direct_save = "direct_save"
     direct_one_subplot = "direct_one_subplot"
 
-    @staticmethod
-    def from_str(value: Union[str, "DisplayModes"]) -> "DisplayModes":
-        if isinstance(value, DisplayModes):
-            return value
-        for strategy in DisplayModes:
-            if strategy.value == value:
-                return strategy
-        else:
-            raise ValueError(f"Unknown DisplayModes: {value}")
-
 
 def plotly_interactive(
     plot_function: PlotFunction,
     data_source: Union[pd.DataFrame, pd.Series],
     *args,
     **kwargs,
 ) -> Callable:
```

### Comparing `krisi-1.1.0/src/krisi/report/vizualise.py` & `krisi-1.1.1/src/krisi/report/vizualise.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,25 @@
 import pkgutil
-from enum import Enum
 from typing import TYPE_CHECKING, List, Optional, Union
 
 import pandas as pd
 
 from krisi.report.type import InteractiveFigure
+from krisi.utils.enums import ParsableEnum
 from krisi.utils.iterable_helpers import wrap_in_list
 from krisi.utils.state import RunType, get_global_state
 
 if TYPE_CHECKING:
     import plotly.graph_objects as go
 
 
-class VizualisationMethod(Enum):
+class VizualisationMethod(ParsableEnum):
     overlap = "overlap"
     seperate = "seperate"
 
-    @staticmethod
-    def from_str(value: Union[str, "VizualisationMethod"]) -> "VizualisationMethod":
-        if isinstance(value, VizualisationMethod):
-            return value
-        for strategy in VizualisationMethod:
-            if strategy.value == value:
-                return strategy
-        else:
-            raise ValueError(f"Unknown VizualisationMethod: {value}")
-
 
 def __calc_plot_names(
     df: pd.DataFrame,
     modes: List[VizualisationMethod],
     y_separate: bool,
     joint_plot_name: str,
     target_plot_name: str,
```

### Comparing `krisi-1.1.0/src/krisi/report/library/console/diagrams.py` & `krisi-1.1.1/src/krisi/report/library/console/diagrams.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.css` & `krisi-1.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.css`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.html` & `krisi-1.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.html`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/utils/console_plot.py` & `krisi-1.1.1/src/krisi/utils/console_plot.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/utils/data.py` & `krisi-1.1.1/src/krisi/utils/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from statsmodels.tsa.arima_process import ArmaProcess
 
-from krisi.utils.devutils.type import Task
+from krisi.sharedtypes import Task
 
 
 def make_it_stationary(ds: pd.Series) -> pd.Series:
     """If the ds, is a random walk with drift, take first differences to make it stationary."""
     print(f"Making the Series {ds.name} stationary.")
     return ds.diff().dropna()
```

### Comparing `krisi-1.1.0/src/krisi/utils/environment.py` & `krisi-1.1.1/src/krisi/utils/environment.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/utils/io.py` & `krisi-1.1.1/src/krisi/utils/io.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/utils/iterable_helpers.py` & `krisi-1.1.1/src/krisi/utils/iterable_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 T = TypeVar("T")
 
 
 def wrap_in_list(input: Union[T, List[T]]) -> List[T]:
     return input if isinstance(input, List) else [input]
 
 
-def replace_if_None(input: Any, replacement: Any) -> Any:
+def replace_if_none(input: Any, replacement: Any) -> Any:
     return replacement if input is None else input
 
 
 def is_int(s: Any):
     if isinstance(s, str) and "." in s:
         return False
     try:
@@ -150,13 +150,13 @@
 
 
 def del_dict_keys(d: dict, keys: Union[str, List[str]]) -> dict:
     keys = wrap_in_list(keys)
     return {k: v for k, v in d.items() if k not in keys}
 
 
-def empty_if_None(metrics: Optional[List]) -> List:
+def empty_if_none(metrics: Optional[List]) -> List:
     return metrics if metrics is not None else []
 
 
 def filter_none(list: List) -> List:
     return [el for el in list if el is not None]
```

### Comparing `krisi-1.1.0/src/krisi/utils/printing.py` & `krisi-1.1.1/src/krisi/utils/printing.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/src/krisi/utils/devutils/timing.py` & `krisi-1.1.1/src/krisi/utils/devutils/timing.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/.gitignore` & `krisi-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/LICENSE` & `krisi-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/README.md` & `krisi-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `krisi-1.1.0/pyproject.toml` & `krisi-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "krisi"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Mark Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 description = "Testing and Reporting framework for Time Series Analysis"
 readme = "README.md"
 license = { file="LICENSE" }
@@ -134,15 +134,15 @@
   "src",
   ".",
 ]
 testpaths = ["tests"] 
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "1.1.0"
+current_version = "1.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `krisi-1.1.0/PKG-INFO` & `krisi-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krisi
-Version: 1.1.0
+Version: 1.1.1
 Summary: Testing and Reporting framework for Time Series Analysis
 Project-URL: Documentation, https://dream-faster.github.io/krisi
 Project-URL: Issues, https://github.com/dream-faster/krisi/issues
 Project-URL: Source, https://github.com/dream-faster/krisi
 Author-email: Mark Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
 License: MIT License
```

