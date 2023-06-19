# Comparing `tmp/prostate-nomograms-0.0.5.tar.gz` & `tmp/prostate-nomograms-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prostate-nomograms-0.0.5.tar", last modified: Fri Jun  2 20:24:26 2023, max compression
+gzip compressed data, was "prostate-nomograms-0.0.6.tar", last modified: Mon Jun 19 15:19:49 2023, max compression
```

## Comparing `prostate-nomograms-0.0.5.tar` & `prostate-nomograms-0.0.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 20:24:26.097023 prostate-nomograms-0.0.5/
--rw-rw-rw-   0        0        0    11549 2023-06-02 19:44:39.000000 prostate-nomograms-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3858 2023-06-02 20:24:26.097023 prostate-nomograms-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3248 2023-06-02 20:22:20.000000 prostate-nomograms-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 20:24:26.007168 prostate-nomograms-0.0.5/examples/
--rw-rw-rw-   0        0        0        0 2023-05-09 17:06:15.000000 prostate-nomograms-0.0.5/examples/__init__.py
--rw-rw-rw-   0        0        0      150 2023-05-09 17:06:15.000000 prostate-nomograms-0.0.5/examples/env_examples.py
--rw-rw-rw-   0        0        0     3569 2023-06-02 19:21:40.000000 prostate-nomograms-0.0.5/examples/ex01-mskcc.py
--rw-rw-rw-   0        0        0     3781 2023-06-02 19:21:40.000000 prostate-nomograms-0.0.5/examples/ex02-capra.py
--rw-rw-rw-   0        0        0     3914 2023-06-02 19:21:40.000000 prostate-nomograms-0.0.5/examples/ex03-custom.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:24:26.013167 prostate-nomograms-0.0.5/prostate_nomograms/
--rw-rw-rw-   0        0        0      465 2023-06-02 20:23:02.000000 prostate-nomograms-0.0.5/prostate_nomograms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:24:26.036335 prostate-nomograms-0.0.5/prostate_nomograms/capra/
--rw-rw-rw-   0        0        0       34 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.5/prostate_nomograms/capra/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:24:26.048856 prostate-nomograms-0.0.5/prostate_nomograms/capra/base/
--rw-rw-rw-   0        0        0      106 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.5/prostate_nomograms/capra/base/__init__.py
--rw-rw-rw-   0        0        0     1336 2023-06-01 15:55:16.000000 prostate-nomograms-0.0.5/prostate_nomograms/capra/base/logistic_regression.py
--rw-rw-rw-   0        0        0     2273 2023-05-31 23:11:28.000000 prostate-nomograms-0.0.5/prostate_nomograms/capra/base/survival_regression.py
--rw-rw-rw-   0        0        0    12184 2023-06-02 20:01:55.000000 prostate-nomograms-0.0.5/prostate_nomograms/capra/capra.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:24:26.057856 prostate-nomograms-0.0.5/prostate_nomograms/custom/
--rw-rw-rw-   0        0        0       36 2023-05-31 19:54:31.000000 prostate-nomograms-0.0.5/prostate_nomograms/custom/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:24:26.069857 prostate-nomograms-0.0.5/prostate_nomograms/custom/base/
--rw-rw-rw-   0        0        0      106 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.5/prostate_nomograms/custom/base/__init__.py
--rw-rw-rw-   0        0        0     1282 2023-06-01 15:55:16.000000 prostate-nomograms-0.0.5/prostate_nomograms/custom/base/logistic_regression.py
--rw-rw-rw-   0        0        0     2192 2023-05-31 15:13:00.000000 prostate-nomograms-0.0.5/prostate_nomograms/custom/base/survival_regression.py
--rw-rw-rw-   0        0        0     9078 2023-05-31 22:07:18.000000 prostate-nomograms-0.0.5/prostate_nomograms/custom/custom.py
--rw-rw-rw-   0        0        0     1162 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.5/prostate_nomograms/enum.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:24:26.075858 prostate-nomograms-0.0.5/prostate_nomograms/mskcc/
--rw-rw-rw-   0        0        0       86 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.5/prostate_nomograms/mskcc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:24:26.095948 prostate-nomograms-0.0.5/prostate_nomograms/mskcc/base/
--rw-rw-rw-   0        0        0       26 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.5/prostate_nomograms/mskcc/base/__init__.py
--rw-rw-rw-   0        0        0     9792 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.5/prostate_nomograms/mskcc/base/logistic_regression.py
--rw-rw-rw-   0        0        0    10577 2023-05-31 22:05:59.000000 prostate-nomograms-0.0.5/prostate_nomograms/mskcc/base/model.py
--rw-rw-rw-   0        0        0     2533 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.5/prostate_nomograms/mskcc/base/survival_regression.py
--rw-rw-rw-   0        0        0     5490 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.5/prostate_nomograms/mskcc/base/web_table_scraper.py
--rw-rw-rw-   0        0        0     2841 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.5/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:24:26.026340 prostate-nomograms-0.0.5/prostate_nomograms.egg-info/
--rw-rw-rw-   0        0        0     3858 2023-06-02 20:24:25.000000 prostate-nomograms-0.0.5/prostate_nomograms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1191 2023-06-02 20:24:25.000000 prostate-nomograms-0.0.5/prostate_nomograms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 20:24:25.000000 prostate-nomograms-0.0.5/prostate_nomograms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-06-02 20:24:25.000000 prostate-nomograms-0.0.5/prostate_nomograms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-06-02 20:24:25.000000 prostate-nomograms-0.0.5/prostate_nomograms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 20:24:26.097023 prostate-nomograms-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-06-02 20:23:02.000000 prostate-nomograms-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.928906 prostate-nomograms-0.0.6/
+-rw-rw-rw-   0        0        0    11549 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3858 2023-06-19 15:19:49.927906 prostate-nomograms-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3248 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.884771 prostate-nomograms-0.0.6/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-03 22:40:34.000000 prostate-nomograms-0.0.6/examples/__init__.py
+-rw-rw-rw-   0        0        0      150 2023-05-06 03:41:30.000000 prostate-nomograms-0.0.6/examples/env_examples.py
+-rw-rw-rw-   0        0        0     3569 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/examples/ex01-mskcc.py
+-rw-rw-rw-   0        0        0     4129 2023-06-17 14:21:21.000000 prostate-nomograms-0.0.6/examples/ex02-capra.py
+-rw-rw-rw-   0        0        0     4210 2023-06-17 14:21:21.000000 prostate-nomograms-0.0.6/examples/ex03-custom.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.889589 prostate-nomograms-0.0.6/prostate_nomograms/
+-rw-rw-rw-   0        0        0      465 2023-06-19 15:17:01.000000 prostate-nomograms-0.0.6/prostate_nomograms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.897087 prostate-nomograms-0.0.6/prostate_nomograms/capra/
+-rw-rw-rw-   0        0        0       34 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/capra/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.903732 prostate-nomograms-0.0.6/prostate_nomograms/capra/base/
+-rw-rw-rw-   0        0        0      106 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/capra/base/__init__.py
+-rw-rw-rw-   0        0        0     1336 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/capra/base/logistic_regression.py
+-rw-rw-rw-   0        0        0     2273 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/capra/base/survival_regression.py
+-rw-rw-rw-   0        0        0    12184 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/capra/capra.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.907891 prostate-nomograms-0.0.6/prostate_nomograms/custom/
+-rw-rw-rw-   0        0        0       36 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/custom/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.914048 prostate-nomograms-0.0.6/prostate_nomograms/custom/base/
+-rw-rw-rw-   0        0        0      106 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/custom/base/__init__.py
+-rw-rw-rw-   0        0        0     1282 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/custom/base/logistic_regression.py
+-rw-rw-rw-   0        0        0     2192 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/custom/base/survival_regression.py
+-rw-rw-rw-   0        0        0     7179 2023-06-17 14:21:21.000000 prostate-nomograms-0.0.6/prostate_nomograms/custom/custom.py
+-rw-rw-rw-   0        0        0     1162 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/enum.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.917561 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/
+-rw-rw-rw-   0        0        0       86 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.927906 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/
+-rw-rw-rw-   0        0        0       26 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/__init__.py
+-rw-rw-rw-   0        0        0     9792 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/logistic_regression.py
+-rw-rw-rw-   0        0        0    10577 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/model.py
+-rw-rw-rw-   0        0        0     2533 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/survival_regression.py
+-rw-rw-rw-   0        0        0     5490 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/web_table_scraper.py
+-rw-rw-rw-   0        0        0     2841 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.893063 prostate-nomograms-0.0.6/prostate_nomograms.egg-info/
+-rw-rw-rw-   0        0        0     3858 2023-06-19 15:19:49.000000 prostate-nomograms-0.0.6/prostate_nomograms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1191 2023-06-19 15:19:49.000000 prostate-nomograms-0.0.6/prostate_nomograms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 15:19:49.000000 prostate-nomograms-0.0.6/prostate_nomograms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-06-19 15:19:49.000000 prostate-nomograms-0.0.6/prostate_nomograms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-06-19 15:19:49.000000 prostate-nomograms-0.0.6/prostate_nomograms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 15:19:49.928906 prostate-nomograms-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-06-19 15:16:49.000000 prostate-nomograms-0.0.6/setup.py
```

### Comparing `prostate-nomograms-0.0.5/LICENSE` & `prostate-nomograms-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.5/PKG-INFO` & `prostate-nomograms-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prostate-nomograms
-Version: 0.0.5
+Version: 0.0.6
 Summary: Prediction tools based on existing prostate cancer nomograms.
 Home-page: https://github.com/MaxenceLarose/prostate-nomograms
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: cancer medical nomogram prediction prostate python3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prostate-nomograms-0.0.5/README.md` & `prostate-nomograms-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.5/examples/ex01-mskcc.py` & `prostate-nomograms-0.0.6/examples/ex01-mskcc.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.5/examples/ex02-capra.py` & `prostate-nomograms-0.0.6/examples/ex02-capra.py`

 * *Files 24% similar despite different names*

```diff
@@ -56,15 +56,23 @@
             )
             capra_nomogram.fit(dataframe)
             dataframe[f"PREDICTED_{outcome.name}_RISK"] = capra_nomogram.predict_risk(dataframe)
             for number_of_months in NUMBER_OF_MONTHS:
                 column_name = f"PREDICTED_{outcome.name}_{number_of_months}MONTHS"
                 dataframe[column_name] = capra_nomogram.predict_proba(dataframe, number_of_months)
         else:
-            capra_nomogram = CapraNomogram(outcome=outcome, target_column_name=col_name)
+            capra_nomogram = CapraNomogram(
+                outcome=outcome,
+                target_column_name=col_name,
+                age_column_name=AGE_COLUMN,
+                psa_column_name=PSA_COLUMN,
+                primary_gleason_column_name=GLEASON_PRIMARY_COLUMN,
+                secondary_gleason_column_name=GLEASON_SECONDARY_COLUMN,
+                clinical_stage_column_name=CLINICAL_STAGE_COLUMN
+            )
             capra_nomogram.fit(dataframe)
             dataframe[f"PREDICTED_{outcome.name}"] = capra_nomogram.predict_proba(dataframe)
 
     # ----------------------------------------------------------------------------------------------------------- #
     #                                                  Results                                                    #
     # ----------------------------------------------------------------------------------------------------------- #
     dataframe.to_csv(path_or_buf=RESULTS_PATH)
```

### Comparing `prostate-nomograms-0.0.5/examples/ex03-custom.py` & `prostate-nomograms-0.0.6/examples/ex03-custom.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,28 +45,41 @@
     # ----------------------------------------------------------------------------------------------------------- #
     for outcome, col_name in OUTCOMES.items():
         if outcome in SurvivalOutcome:
             custom_nomogram = CustomNomogram(
                 outcome=outcome,
                 event_indicator_column_name=col_name,
                 event_time_column_name=f"{col_name}_TIME",
-                age_column_name=AGE_COLUMN,
-                psa_column_name=PSA_COLUMN,
-                primary_gleason_column_name=GLEASON_PRIMARY_COLUMN,
-                secondary_gleason_column_name=GLEASON_SECONDARY_COLUMN,
-                global_gleason_column_name=GLEASON_GLOBAL_COLUMN,
-                clinical_stage_column_name=CLINICAL_STAGE_COLUMN
+                features_column_names=[
+                    AGE_COLUMN,
+                    PSA_COLUMN,
+                    GLEASON_PRIMARY_COLUMN,
+                    GLEASON_SECONDARY_COLUMN,
+                    GLEASON_GLOBAL_COLUMN,
+                    CLINICAL_STAGE_COLUMN
+                ]
             )
             custom_nomogram.fit(dataframe)
             dataframe[f"PREDICTED_{outcome.name}_RISK"] = custom_nomogram.predict_risk(dataframe)
             for number_of_months in NUMBER_OF_MONTHS:
                 column_name = f"PREDICTED_{outcome.name}_{number_of_months}MONTHS"
                 dataframe[column_name] = custom_nomogram.predict_proba(dataframe, number_of_months)
         else:
-            custom_nomogram = CustomNomogram(outcome=outcome,target_column_name=col_name)
+            custom_nomogram = CustomNomogram(
+                outcome=outcome,
+                target_column_name=col_name,
+                features_column_names=[
+                    AGE_COLUMN,
+                    PSA_COLUMN,
+                    GLEASON_PRIMARY_COLUMN,
+                    GLEASON_SECONDARY_COLUMN,
+                    GLEASON_GLOBAL_COLUMN,
+                    CLINICAL_STAGE_COLUMN
+                ]
+            )
             custom_nomogram.fit(dataframe)
             dataframe[f"PREDICTED_{outcome.name}"] = custom_nomogram.predict_proba(dataframe)
 
     # ----------------------------------------------------------------------------------------------------------- #
     #                                                  Results                                                    #
     # ----------------------------------------------------------------------------------------------------------- #
     dataframe.to_csv(path_or_buf=RESULTS_PATH)
```

### Comparing `prostate-nomograms-0.0.5/prostate_nomograms/capra/base/logistic_regression.py` & `prostate-nomograms-0.0.6/prostate_nomograms/capra/base/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.5/prostate_nomograms/capra/base/survival_regression.py` & `prostate-nomograms-0.0.6/prostate_nomograms/capra/base/survival_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.5/prostate_nomograms/capra/capra.py` & `prostate-nomograms-0.0.6/prostate_nomograms/capra/capra.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.5/prostate_nomograms/custom/base/logistic_regression.py` & `prostate-nomograms-0.0.6/prostate_nomograms/custom/base/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.5/prostate_nomograms/custom/base/survival_regression.py` & `prostate-nomograms-0.0.6/prostate_nomograms/custom/base/survival_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.5/prostate_nomograms/custom/custom.py` & `prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/logistic_regression.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,251 +1,216 @@
-from typing import List, Optional, Union
+from __future__ import annotations
+from typing import Mapping, Optional, TYPE_CHECKING
 
-import pandas as pd
-import numpy as np
+if TYPE_CHECKING:
+    from .survival_regression import SurvivalRegression
 
-from ..enum import ClassificationOutcome, SurvivalOutcome
-from .base import LogisticRegression, SurvivalRegression
+import numpy as np
+import pandas as pd
 
 
-class CustomNomogram:
-    """
-    Custom model. It can be used to create a nomogram with a custom model.
-    """
+class LogisticRegression:
 
     def __init__(
             self,
-            outcome: Union[str, ClassificationOutcome, SurvivalOutcome],
-            target_column_name: Optional[str] = None,
-            event_indicator_column_name: Optional[str] = None,
-            event_time_column_name: Optional[str] = None,
+            variables_coefficients: Mapping[str, float],
+            spline_coefficients: Mapping[str, float],
+            cores: bool,
             age_column_name: str = "AGE",
             psa_column_name: str = "PSA",
             primary_gleason_column_name: str = "GLEASON_PRIMARY",
             secondary_gleason_column_name: str = "GLEASON_SECONDARY",
-            global_gleason_column_name: str = "GLEASON_GLOBAL",
             clinical_stage_column_name: str = "CLINICAL_STAGE",
-            positive_cores_percentage_column_name: Optional[str] = None,
-            random_state: int = 0
+            number_of_positive_cores_column_name: Optional[str] = None,
+            number_of_negative_cores_column_name: Optional[str] = None,
     ):
         """
         Initializes columns names.
 
         Parameters
         ----------
-        outcome : Optional[Union[str, Outcome]]
-            Name of the outcome.
-        target_column_name : Optional[str]
-            Name of the column containing the target of the patients.
-        event_indicator_column_name : Optional[str]
-            Name of the column containing the event indicator of the patients.
-        event_time_column_name : Optional[str]
-            Name of the column containing the event time of the patients.
+        variables_coefficients : Mapping[str, float]
+            Coefficients of the variables.
+        spline_coefficients : Mapping[str, float]
+            Coefficients of the splines.
+        cores : bool
+            Whether to use the number of positive and negative cores.
         age_column_name : str
             Name of the column containing the age of the patients.
         psa_column_name : str
             Name of the column containing the PSA of the patients.
         primary_gleason_column_name : str
             Name of the column containing the primary Gleason score of the patients.
         secondary_gleason_column_name : str
             Name of the column containing the secondary Gleason score of the patients.
-        global_gleason_column_name : str
-            Name of the column containing the global Gleason score of the patients.
         clinical_stage_column_name : str
             Name of the column containing the clinical stage of the patients.
-        positive_cores_percentage_column_name : str, optional
+        number_of_positive_cores_column_name : str, optional
             Name of the column containing the number of positive cores of the patients.
-        random_state : int, optional
-            Random state.
+        number_of_negative_cores_column_name : str, optional
+            Name of the column containing the number of negative cores of the patients.
         """
-        if outcome in ClassificationOutcome:
-            self.outcome = ClassificationOutcome(outcome)
-        elif outcome in SurvivalOutcome:
-            self.outcome = SurvivalOutcome(outcome)
-        else:
-            raise ValueError(f"Invalid outcome: {outcome}")
+        self.variables_coefficients = variables_coefficients
+        self.spline_coefficients = spline_coefficients
+        self.cores = cores
 
-        self.target_column_name = target_column_name
-        self.event_indicator_column_name = event_indicator_column_name
-        self.event_time_column_name = event_time_column_name
         self.age_column_name = age_column_name
         self.psa_column_name = psa_column_name
         self.primary_gleason_column_name = primary_gleason_column_name
         self.secondary_gleason_column_name = secondary_gleason_column_name
-        self.global_gleason_column_name = global_gleason_column_name
         self.clinical_stage_column_name = clinical_stage_column_name
-        self.positive_cores_percentage_column_name = positive_cores_percentage_column_name
-        self._is_fitted = False
+        self.number_of_positive_cores = number_of_positive_cores_column_name
+        self.number_of_negative_cores = number_of_negative_cores_column_name
 
-        if self.model_type == "survival":
-            assert self.event_indicator_column_name is not None, (
-                "Event indicator column name must be specified for survival models."
-            )
-            assert self.event_time_column_name is not None, (
-                "Event time column name must be specified for survival models."
-            )
-            regressor_constructor = SurvivalRegression
-        elif self.model_type == "logistic":
-            assert self.target_column_name is not None, (
-                "Target column name must be specified for logistic models."
-            )
-            regressor_constructor = LogisticRegression
-        else:
-            raise ValueError(f"Unknown model type: {self.model_type}")
-
-        self.regressor = regressor_constructor(random_state=random_state)
+    def _get_gleason_value(self, data_dict: dict) -> np.ndarray:
+        primary_gleason = np.array(data_dict[self.primary_gleason_column_name])
+        secondary_gleason = np.array(data_dict[self.secondary_gleason_column_name])
+        total_gleason_score = primary_gleason + secondary_gleason
 
-    @property
-    def model_type(self) -> str:
-        """
-        The type of the model. It is used to determine which model to use for the prediction.
+        gleason_value = np.zeros_like(total_gleason_score, dtype=float)
+        mask_grade_2 = np.where(((primary_gleason == 3) & (secondary_gleason == 4)), True, False)
+        mask_grade_3 = np.where(((primary_gleason == 4) & (secondary_gleason == 3)), True, False)
 
-        Returns
-        -------
-        model_type : str
-            The type of the model. It is used to determine which model to use for the prediction.
-        """
-        if self.outcome in list(SurvivalOutcome):
-            return "survival"
-        else:
-            return "logistic"
+        gleason_value[mask_grade_2] = self.variables_coefficients["Biopsy Gleason Grade Group 2"]
+        gleason_value[mask_grade_3] = self.variables_coefficients["Biopsy Gleason Grade Group 3"]
+        gleason_value[total_gleason_score == 8] = self.variables_coefficients["Biopsy Gleason Grade Group 4"]
+        gleason_value[total_gleason_score == 9] = self.variables_coefficients["Biopsy Gleason Grade Group 5"]
+        gleason_value[total_gleason_score == 10] = self.variables_coefficients["Biopsy Gleason Grade Group 5"]
 
-    @property
-    def cores(self):
-        """
-        Whether the model is for cores or not.
+        return gleason_value
 
-        Returns
-        -------
-        is_cores : bool
-            Whether the model is for cores or not.
-        """
-        if self.outcome.endswith("(Cores)"):
-            return True
-        else:
-            return False
+    def _get_clinical_stage_value(self, data_dict: dict) -> np.ndarray:
+        tumor_stage = data_dict[self.clinical_stage_column_name]
 
-    @property
-    def columns(self) -> List[str]:
-        """
-        Returns the columns of the model.
+        clinical_stage_value = np.zeros_like(tumor_stage, dtype=float)
+        clinical_stage_value[list(map("T2a".__eq__, tumor_stage))] = self.variables_coefficients["Clinical Stage 2A"]
+        clinical_stage_value[list(map("T2b".__eq__, tumor_stage))] = self.variables_coefficients["Clinical Stage 2B"]
+        clinical_stage_value[list(map("T2c".__eq__, tumor_stage))] = self.variables_coefficients["Clinical Stage 2C"]
+        clinical_stage_value[list(map("T3a".__eq__, tumor_stage))] = self.variables_coefficients["Clinical Stage 3+"]
+        clinical_stage_value[list(map("T3b".__eq__, tumor_stage))] = self.variables_coefficients["Clinical Stage 3+"]
+        clinical_stage_value[list(map("T3c".__eq__, tumor_stage))] = self.variables_coefficients["Clinical Stage 3+"]
 
-        Returns
-        -------
-        columns : List[str]
-            The columns of the model.
-        """
-        columns = [
-            self.age_column_name,
-            self.psa_column_name,
-            self.primary_gleason_column_name,
-            self.secondary_gleason_column_name,
-            self.global_gleason_column_name,
-            self.clinical_stage_column_name
-        ]
+        return clinical_stage_value
 
-        if self.cores:
-            columns.append(self.positive_cores_percentage_column_name)
+    def _get_positive_cores_value(self, data_dict: dict) -> np.ndarray:
+        return np.array(data_dict[self.number_of_positive_cores])*self.variables_coefficients["No. of Positive Cores"]
 
-        return columns
+    def _get_negative_cores_value(self, data_dict: dict):
+        return np.array(data_dict[self.number_of_negative_cores])*self.variables_coefficients["No. of Negative Cores"]
 
-    def get_features(self, dataframe: pd.DataFrame) -> np.ndarray:
+    def _get_spline_term_1(self, psa: np.array) -> np.ndarray:
         """
-        Returns the features of the patients.
+        Gets the spline term 1.
 
         Parameters
         ----------
-        dataframe : pd.DataFrame
-            Dataframe containing the data of the patients.
+        psa : numpy.ndarray
+            The PSA values.
 
         Returns
         -------
-        features : np.ndarray
-            The features of the patients.
+        spline_term_1 : numpy.ndarray
+            The spline term 1.
         """
-        dataframe = dataframe[self.columns]
-        return np.array(dataframe)
+        knot1 = self.spline_coefficients["PSAPreopKnot1"]
+        knot3 = self.spline_coefficients["PSAPreopKnot3"]
+        knot4 = self.spline_coefficients["PSAPreopKnot4"]
 
-    def fit(
-            self,
-            dataset: pd.DataFrame
-    ):
+        spline_term_1 = np.maximum(psa - knot1, np.zeros_like(psa))**3
+        spline_term_1 += -(np.maximum(psa - knot3, np.zeros_like(psa))**3) * (knot4 - knot1) / (knot4 - knot3)
+        spline_term_1 += (np.maximum(psa - knot4, np.zeros_like(psa))**3) * (knot3 - knot1) / (knot4 - knot3)
+
+        return spline_term_1
+
+    def _get_spline_term_2(self, psa: np.array) -> np.ndarray:
         """
-        Fits the model.
+        Gets the spline term 2.
 
         Parameters
         ----------
-        dataset : pd.DataFrame
-            Dataframe containing the data of the patients.
+        psa : numpy.ndarray
+            The PSA values.
+
+        Returns
+        -------
+        spline_term_2 : numpy.ndarray
+            The spline term 2.
         """
-        features = self.get_features(dataset)
-        if self.model_type == "survival":
-            self.regressor.fit(
-                features,
-                np.array(dataset[self.event_indicator_column_name], dtype=bool),
-                np.array(dataset[self.event_time_column_name], dtype=float)
-            )
-        else:
-            self.regressor.fit(
-                features,
-                np.array(dataset[self.target_column_name])
-            )
+        knot2 = self.spline_coefficients["PSAPreopKnot2"]
+        knot3 = self.spline_coefficients["PSAPreopKnot3"]
+        knot4 = self.spline_coefficients["PSAPreopKnot4"]
+
+        spline_term_2 = np.maximum(psa - knot2, np.zeros_like(psa)) ** 3
+        spline_term_2 += -(np.maximum(psa - knot3, np.zeros_like(psa)) ** 3) * (knot4 - knot2) / (knot4 - knot3)
+        spline_term_2 += (np.maximum(psa - knot4, np.zeros_like(psa)) ** 3) * (knot3 - knot2) / (knot4 - knot3)
 
-        self._is_fitted = True
+        return spline_term_2
 
-    def predict_proba(
+    def get_predicted_result(
             self,
             dataframe: pd.DataFrame,
-            number_of_months: Union[np.ndarray, list, float, int] = None
-    ) -> np.ndarray:
+            regressor_as_variable: Optional[SurvivalRegression] = None
+    ) -> np.array:
         """
-        Gets the predictions. If the model is survival, the number of years must be given.
+        Gets the predicted result.
 
         Parameters
         ----------
         dataframe : pandas.DataFrame
-            The dataframe.
-        number_of_months : Union[numpy.ndarray, list, float, int], optional
-            The number of months. It is used only for survival models.
+            The dataframe that contains the patients data.
+        regressor_as_variable : Optional[SurvivalRegression]
+            The regressor as variable.
 
         Returns
         -------
-        predictions : numpy.ndarray
-            The predictions.
+        predicted_result : numpy.ndarray
+            The predicted result.
         """
-        assert self._is_fitted, "Model must be fitted first."
+        data_dict = dataframe.to_dict(orient="list")
 
-        features = self.get_features(dataframe)
-        if self.model_type == "survival":
-            if number_of_months is None:
-                raise ValueError("Number of months must be given.")
-            else:
-                return self.regressor.get_predicted_survival_probability(features, number_of_months)
-        elif self.model_type == "logistic":
-            return self.regressor.get_predicted_probability(features)
+        result = self.variables_coefficients["Intercept"]
+
+        if regressor_as_variable:
+            keys = [k for k in self.variables_coefficients.keys() if k.startswith("Survival probability")]
+            assert len(keys) == 1, "There should be only one key that starts with 'Survival probability'"
+            coefficient = self.variables_coefficients[keys[0]]
+            result += coefficient*regressor_as_variable.get_predicted_survival_probability(dataframe, 60)
+            return result
         else:
-            raise ValueError(f"Model type {self.model_type} doesn't exist.")
+            result += np.array(data_dict[self.psa_column_name]) * self.variables_coefficients["Preoperative PSA"]
+
+            spline_term_1 = self._get_spline_term_1(np.array(data_dict[self.psa_column_name]))
+            spline_term_2 = self._get_spline_term_2(np.array(data_dict[self.psa_column_name]))
+            result += spline_term_1 * self.variables_coefficients["Preoperative PSA Spline 1"]
+            result += spline_term_2 * self.variables_coefficients["Preoperative PSA Spline 2"]
 
-    def predict_risk(
+            result += np.array(data_dict[self.age_column_name]) * self.variables_coefficients["Patient Age"]
+            result += self._get_gleason_value(data_dict)
+            result += self._get_clinical_stage_value(data_dict)
+
+            if self.cores:
+                result += self._get_positive_cores_value(data_dict)
+                result += self._get_negative_cores_value(data_dict)
+            return result
+
+    def get_predicted_probability(
             self,
-            dataframe: pd.DataFrame
-    ) -> np.ndarray:
+            dataframe: pd.DataFrame,
+            regressor_as_variable: Optional[SurvivalRegression] = None
+    ) -> np.array:
         """
-        Gets the risk predictions.
+        Gets the predicted result.
 
         Parameters
         ----------
         dataframe : pandas.DataFrame
-            The dataframe.
+            The dataframe that contains the patients data.
+        regressor_as_variable : SurvivalRegression
+            The regressor as variable.
 
         Returns
         -------
-        predictions : numpy.ndarray
-            The predictions.
+        predicted_probability : numpy.ndarray
+            The predicted probability.
         """
-        if self.model_type == "survival":
-            features = self.get_features(dataframe)
-            return self.regressor.get_predicted_risk(features)
-        elif self.model_type == "logistic":
-            raise ValueError("Logistic models don't have risk predictions.")
-        else:
-            raise ValueError(f"Model type {self.model_type} doesn't exist.")
+        predicted_result = self.get_predicted_result(dataframe, regressor_as_variable)
+        return np.exp(predicted_result)/(1 + np.exp(predicted_result))
```

### Comparing `prostate-nomograms-0.0.5/prostate_nomograms/enum.py` & `prostate-nomograms-0.0.6/prostate_nomograms/enum.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.5/prostate_nomograms/mskcc/base/logistic_regression.py` & `prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-from __future__ import annotations
-from typing import Mapping, Optional, TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from .survival_regression import SurvivalRegression
+from typing import Mapping, Optional, Union
 
 import numpy as np
 import pandas as pd
 
+from ...enum import SurvivalOutcome
+from .logistic_regression import LogisticRegression
+from .survival_regression import SurvivalRegression
+from .web_table_scraper import CoefficientCategory, WebTableScraper
+
 
-class LogisticRegression:
+class Model:
 
     def __init__(
             self,
-            variables_coefficients: Mapping[str, float],
-            spline_coefficients: Mapping[str, float],
-            cores: bool,
+            outcome: str,
+            url: str,
+            json_folder_path: str,
             age_column_name: str = "AGE",
             psa_column_name: str = "PSA",
             primary_gleason_column_name: str = "GLEASON_PRIMARY",
             secondary_gleason_column_name: str = "GLEASON_SECONDARY",
             clinical_stage_column_name: str = "CLINICAL_STAGE",
             number_of_positive_cores_column_name: Optional[str] = None,
             number_of_negative_cores_column_name: Optional[str] = None,
     ):
         """
         Initializes columns names.
 
         Parameters
         ----------
-        variables_coefficients : Mapping[str, float]
-            Coefficients of the variables.
-        spline_coefficients : Mapping[str, float]
-            Coefficients of the splines.
-        cores : bool
-            Whether to use the number of positive and negative cores.
+        outcome : str
+            Name of the outcome.
+        url : str
+            URL of the web page containing the coefficients.
+        json_folder_path : str
+            Path to save the coefficients.
         age_column_name : str
             Name of the column containing the age of the patients.
         psa_column_name : str
             Name of the column containing the PSA of the patients.
         primary_gleason_column_name : str
             Name of the column containing the primary Gleason score of the patients.
         secondary_gleason_column_name : str
@@ -45,172 +46,245 @@
         clinical_stage_column_name : str
             Name of the column containing the clinical stage of the patients.
         number_of_positive_cores_column_name : str, optional
             Name of the column containing the number of positive cores of the patients.
         number_of_negative_cores_column_name : str, optional
             Name of the column containing the number of negative cores of the patients.
         """
-        self.variables_coefficients = variables_coefficients
-        self.spline_coefficients = spline_coefficients
-        self.cores = cores
-
-        self.age_column_name = age_column_name
-        self.psa_column_name = psa_column_name
-        self.primary_gleason_column_name = primary_gleason_column_name
-        self.secondary_gleason_column_name = secondary_gleason_column_name
-        self.clinical_stage_column_name = clinical_stage_column_name
-        self.number_of_positive_cores = number_of_positive_cores_column_name
-        self.number_of_negative_cores = number_of_negative_cores_column_name
-
-    def _get_gleason_value(self, data_dict: dict) -> np.ndarray:
-        primary_gleason = np.array(data_dict[self.primary_gleason_column_name])
-        secondary_gleason = np.array(data_dict[self.secondary_gleason_column_name])
-        total_gleason_score = primary_gleason + secondary_gleason
-
-        gleason_value = np.zeros_like(total_gleason_score, dtype=float)
-        mask_grade_2 = np.where(((primary_gleason == 3) & (secondary_gleason == 4)), True, False)
-        mask_grade_3 = np.where(((primary_gleason == 4) & (secondary_gleason == 3)), True, False)
-
-        gleason_value[mask_grade_2] = self.variables_coefficients["Biopsy Gleason Grade Group 2"]
-        gleason_value[mask_grade_3] = self.variables_coefficients["Biopsy Gleason Grade Group 3"]
-        gleason_value[total_gleason_score == 8] = self.variables_coefficients["Biopsy Gleason Grade Group 4"]
-        gleason_value[total_gleason_score == 9] = self.variables_coefficients["Biopsy Gleason Grade Group 5"]
-        gleason_value[total_gleason_score == 10] = self.variables_coefficients["Biopsy Gleason Grade Group 5"]
-
-        return gleason_value
-
-    def _get_clinical_stage_value(self, data_dict: dict) -> np.ndarray:
-        tumor_stage = data_dict[self.clinical_stage_column_name]
-
-        clinical_stage_value = np.zeros_like(tumor_stage, dtype=float)
-        clinical_stage_value[list(map("T2a".__eq__, tumor_stage))] = self.variables_coefficients["Clinical Stage 2A"]
-        clinical_stage_value[list(map("T2b".__eq__, tumor_stage))] = self.variables_coefficients["Clinical Stage 2B"]
-        clinical_stage_value[list(map("T2c".__eq__, tumor_stage))] = self.variables_coefficients["Clinical Stage 2C"]
-        clinical_stage_value[list(map("T3a".__eq__, tumor_stage))] = self.variables_coefficients["Clinical Stage 3+"]
-        clinical_stage_value[list(map("T3b".__eq__, tumor_stage))] = self.variables_coefficients["Clinical Stage 3+"]
-        clinical_stage_value[list(map("T3c".__eq__, tumor_stage))] = self.variables_coefficients["Clinical Stage 3+"]
-
-        return clinical_stage_value
-
-    def _get_positive_cores_value(self, data_dict: dict) -> np.ndarray:
-        return np.array(data_dict[self.number_of_positive_cores])*self.variables_coefficients["No. of Positive Cores"]
+        self.outcome = outcome
+        self.url = url
+        self.json_folder_path = json_folder_path
+
+        web_table_scrapper = WebTableScraper(url, json_folder_path)
+        coefficients_dataframe = web_table_scrapper.get_models_coefficients(CoefficientCategory.VARIABLES)
+        self._variables_coefficients_dataframe = coefficients_dataframe[coefficients_dataframe["Model"] == outcome]
+        self._splines_coefficients_dataframe = web_table_scrapper.get_models_coefficients(CoefficientCategory.SPLINE)
+
+        if self.model_type == "survival":
+            regressor_constructor = SurvivalRegression
+        elif self.model_type == "logistic":
+            regressor_constructor = LogisticRegression
+        else:
+            raise ValueError(f"Unknown model type: {self.model_type}")
 
-    def _get_negative_cores_value(self, data_dict: dict):
-        return np.array(data_dict[self.number_of_negative_cores])*self.variables_coefficients["No. of Negative Cores"]
+        self.regressor = regressor_constructor(
+            variables_coefficients=self.variables_coefficients,
+            spline_coefficients=self.spline_coefficients,
+            cores=self.cores,
+            age_column_name=age_column_name,
+            psa_column_name=psa_column_name,
+            primary_gleason_column_name=primary_gleason_column_name,
+            secondary_gleason_column_name=secondary_gleason_column_name,
+            clinical_stage_column_name=clinical_stage_column_name,
+            number_of_positive_cores_column_name=number_of_positive_cores_column_name,
+            number_of_negative_cores_column_name=number_of_negative_cores_column_name
+        )
 
-    def _get_spline_term_1(self, psa: np.array) -> np.ndarray:
+        if self.is_predicting_death:
+            self._regressor_as_variable = self._create_regressor_as_variable()
+        else:
+            self._regressor_as_variable = None
+
+    @staticmethod
+    def _get_dict_from_two_columns_of_a_dataframe(
+            dataframe: pd.DataFrame,
+            keys_column_name: str,
+            values_column_name: str
+    ) -> Mapping[str, float]:
         """
-        Gets the spline term 1.
+        Gets a dictionary from two columns of a dataframe. The first column is the keys and the second column is the
+        values.
 
         Parameters
         ----------
-        psa : numpy.ndarray
-            The PSA values.
+        dataframe : pandas.DataFrame
+            The dataframe.
+        keys_column_name : str
+            The name of the column that contains the keys.
+        values_column_name : str
+            The name of the column that contains the values.
 
         Returns
         -------
-        spline_term_1 : numpy.ndarray
-            The spline term 1.
+        dict : Mapping[str, float]
+            The dictionary.
         """
-        knot1 = self.spline_coefficients["PSAPreopKnot1"]
-        knot3 = self.spline_coefficients["PSAPreopKnot3"]
-        knot4 = self.spline_coefficients["PSAPreopKnot4"]
+        return pd.Series(data=dataframe[values_column_name].values, index=dataframe[keys_column_name]).to_dict()
 
-        spline_term_1 = np.maximum(psa - knot1, np.zeros_like(psa))**3
-        spline_term_1 += -(np.maximum(psa - knot3, np.zeros_like(psa))**3) * (knot4 - knot1) / (knot4 - knot3)
-        spline_term_1 += (np.maximum(psa - knot4, np.zeros_like(psa))**3) * (knot3 - knot1) / (knot4 - knot3)
+    @property
+    def cores(self):
+        """
+        Whether the model is for cores or not.
 
-        return spline_term_1
+        Returns
+        -------
+        is_cores : bool
+            Whether the model is for cores or not.
+        """
+        if self.outcome.endswith("(Cores)"):
+            return True
+        else:
+            return False
 
-    def _get_spline_term_2(self, psa: np.array) -> np.ndarray:
+    @property
+    def model_type(self) -> str:
         """
-        Gets the spline term 2.
+        The type of the model. It is used to determine which model to use for the prediction.
 
-        Parameters
-        ----------
-        psa : numpy.ndarray
-            The PSA values.
+        Returns
+        -------
+        model_type : str
+            The type of the model. It is used to determine which model to use for the prediction.
+        """
+        model_type = self._variables_coefficients_dataframe["Model Type"].values[0]
+
+        return model_type
+
+    @property
+    def is_predicting_death(self):
+        """
+        Whether the model is predicting death or not.
+
+        Returns
+        -------
+        is_death : bool
+            Whether the model is for predicting death or not.
+        """
+        if "Death" in self.outcome:
+            return True
+        else:
+            return False
+
+    @staticmethod
+    def _map_death_model_to_bcr_outcome() -> dict:
+        """
+        Map death model to the corresponding bcr outcome used for its prediction computation.
+
+        Returns
+        -------
+        mapping : dict
+            Map from the death model to the corresponding bcr outcome.
+        """
+        return {
+            SurvivalOutcome.PREOPERATIVE_PROSTATE_CANCER_DEATH: SurvivalOutcome.PREOPERATIVE_BCR,
+            SurvivalOutcome.PREOPERATIVE_PROSTATE_CANCER_DEATH_CORES: SurvivalOutcome.PREOPERATIVE_BCR_CORES
+        }
+
+    def _create_regressor_as_variable(self) -> SurvivalRegression:
+        """
+        Creates the regressor as a variable.
+
+        Returns
+        -------
+        model : SurvivalRegression
+            The regressor as a variable.
+        """
+        outcome = self._map_death_model_to_bcr_outcome()[self.outcome]
+        return Model(
+            outcome=outcome,
+            url=self.url,
+            json_folder_path=self.json_folder_path,
+            age_column_name=self.regressor.age_column_name,
+            psa_column_name=self.regressor.psa_column_name,
+            primary_gleason_column_name=self.regressor.primary_gleason_column_name,
+            secondary_gleason_column_name=self.regressor.secondary_gleason_column_name,
+            clinical_stage_column_name=self.regressor.clinical_stage_column_name,
+            number_of_positive_cores_column_name=self.regressor.number_of_positive_cores,
+            number_of_negative_cores_column_name=self.regressor.number_of_negative_cores
+        ).regressor
+
+    @property
+    def variables_coefficients(self) -> Mapping[str, float]:
+        """
+        Gets the variables values from the dataframe.
 
         Returns
         -------
-        spline_term_2 : numpy.ndarray
-            The spline term 2.
+        variables_values : Mapping[str, float]
+            The variables values.
         """
-        knot2 = self.spline_coefficients["PSAPreopKnot2"]
-        knot3 = self.spline_coefficients["PSAPreopKnot3"]
-        knot4 = self.spline_coefficients["PSAPreopKnot4"]
+        variables_values = self._get_dict_from_two_columns_of_a_dataframe(
+            dataframe=self._variables_coefficients_dataframe,
+            keys_column_name="Variable",
+            values_column_name="Value"
+        )
 
-        spline_term_2 = np.maximum(psa - knot2, np.zeros_like(psa)) ** 3
-        spline_term_2 += -(np.maximum(psa - knot3, np.zeros_like(psa)) ** 3) * (knot4 - knot2) / (knot4 - knot3)
-        spline_term_2 += (np.maximum(psa - knot4, np.zeros_like(psa)) ** 3) * (knot3 - knot2) / (knot4 - knot3)
+        return variables_values
 
-        return spline_term_2
+    @property
+    def spline_coefficients(self) -> Mapping[str, float]:
+        """
+        Gets the spline knots values from the dataframe.
 
-    def get_predicted_result(
+        Returns
+        -------
+        spline_knots_values : Mapping[str, float]
+            The spline knots values.
+        """
+        spline_knots_values = self._get_dict_from_two_columns_of_a_dataframe(
+            dataframe=self._splines_coefficients_dataframe,
+            keys_column_name="Knot",
+            values_column_name="Value"
+        )
+
+        return spline_knots_values
+
+    def predict_proba(
             self,
             dataframe: pd.DataFrame,
-            regressor_as_variable: Optional[SurvivalRegression] = None
-    ) -> np.array:
+            number_of_months: Union[np.ndarray, list, float, int] = None
+    ) -> np.ndarray:
         """
-        Gets the predicted result.
+        Gets the predictions. If the model is survival, the number of years must be given.
 
         Parameters
         ----------
         dataframe : pandas.DataFrame
-            The dataframe that contains the patients data.
-        regressor_as_variable : Optional[SurvivalRegression]
-            The regressor as variable.
+            The dataframe.
+        number_of_months : Union[numpy.ndarray, list, float, int], optional
+            The number of months. It is used only for survival models.
 
         Returns
         -------
-        predicted_result : numpy.ndarray
-            The predicted result.
+        predictions : numpy.ndarray
+            The predictions.
         """
-        data_dict = dataframe.to_dict(orient="list")
-
-        result = self.variables_coefficients["Intercept"]
-
-        if regressor_as_variable:
-            keys = [k for k in self.variables_coefficients.keys() if k.startswith("Survival probability")]
-            assert len(keys) == 1, "There should be only one key that starts with 'Survival probability'"
-            coefficient = self.variables_coefficients[keys[0]]
-            result += coefficient*regressor_as_variable.get_predicted_survival_probability(dataframe, 60)
-            return result
+        if self.model_type == "survival":
+            if number_of_months is None:
+                raise ValueError("Number of months must be given.")
+            else:
+                return self.regressor.get_predicted_survival_probability(
+                    dataframe,
+                    number_of_months,
+                    self._regressor_as_variable
+                )
+        elif self.model_type == "logistic":
+            return self.regressor.get_predicted_probability(
+                dataframe,
+                self._regressor_as_variable
+            )
         else:
-            result += np.array(data_dict[self.psa_column_name]) * self.variables_coefficients["Preoperative PSA"]
-
-            spline_term_1 = self._get_spline_term_1(np.array(data_dict[self.psa_column_name]))
-            spline_term_2 = self._get_spline_term_2(np.array(data_dict[self.psa_column_name]))
-            result += spline_term_1 * self.variables_coefficients["Preoperative PSA Spline 1"]
-            result += spline_term_2 * self.variables_coefficients["Preoperative PSA Spline 2"]
-
-            result += np.array(data_dict[self.age_column_name]) * self.variables_coefficients["Patient Age"]
-            result += self._get_gleason_value(data_dict)
-            result += self._get_clinical_stage_value(data_dict)
+            raise ValueError(f"Model type {self.model_type} doesn't exist.")
 
-            if self.cores:
-                result += self._get_positive_cores_value(data_dict)
-                result += self._get_negative_cores_value(data_dict)
-            return result
-
-    def get_predicted_probability(
+    def predict_risk(
             self,
-            dataframe: pd.DataFrame,
-            regressor_as_variable: Optional[SurvivalRegression] = None
-    ) -> np.array:
+            dataframe: pd.DataFrame
+    ) -> np.ndarray:
         """
-        Gets the predicted result.
+        Gets the risk predictions.
 
         Parameters
         ----------
         dataframe : pandas.DataFrame
-            The dataframe that contains the patients data.
-        regressor_as_variable : SurvivalRegression
-            The regressor as variable.
+            The dataframe.
 
         Returns
         -------
-        predicted_probability : numpy.ndarray
-            The predicted probability.
+        predictions : numpy.ndarray
+            The predictions.
         """
-        predicted_result = self.get_predicted_result(dataframe, regressor_as_variable)
-        return np.exp(predicted_result)/(1 + np.exp(predicted_result))
+        if self.model_type == "survival":
+            return self.regressor.get_predicted_risk(dataframe, self._regressor_as_variable)
+        elif self.model_type == "logistic":
+            raise ValueError("Logistic models don't have risk predictions.")
+        else:
+            raise ValueError(f"Model type {self.model_type} doesn't exist.")
```

### Comparing `prostate-nomograms-0.0.5/prostate_nomograms/mskcc/base/survival_regression.py` & `prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/survival_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.5/prostate_nomograms/mskcc/base/web_table_scraper.py` & `prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/web_table_scraper.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.5/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py` & `prostate-nomograms-0.0.6/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.5/prostate_nomograms.egg-info/PKG-INFO` & `prostate-nomograms-0.0.6/prostate_nomograms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prostate-nomograms
-Version: 0.0.5
+Version: 0.0.6
 Summary: Prediction tools based on existing prostate cancer nomograms.
 Home-page: https://github.com/MaxenceLarose/prostate-nomograms
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: cancer medical nomogram prediction prostate python3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prostate-nomograms-0.0.5/prostate_nomograms.egg-info/SOURCES.txt` & `prostate-nomograms-0.0.6/prostate_nomograms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.5/setup.py` & `prostate-nomograms-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="prostate-nomograms",
-    version="0.0.5",
+    version="0.0.6",
     author="Maxence Larose",
     author_email="maxence.larose.1@ulaval.ca",
     description="Prediction tools based on existing prostate cancer nomograms.",
     long_description=open('README.md', "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/MaxenceLarose/prostate-nomograms",
     license="Apache License 2.0",
```

