# Comparing `tmp/pii_codex-0.4.5.tar.gz` & `tmp/pii_codex-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pii_codex-0.4.5.tar", max compression
+gzip compressed data, was "pii_codex-0.4.6.tar", max compression
```

## Comparing `pii_codex-0.4.5.tar` & `pii_codex-0.4.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1522 2022-09-08 02:13:55.077785 pii_codex-0.4.5/LICENSE
--rw-r--r--   0        0        0    13307 2023-06-18 23:14:06.926721 pii_codex-0.4.5/README.md
--rw-r--r--   0        0        0       22 2022-09-07 01:58:01.158467 pii_codex-0.4.5/pii_codex/__init__.py
--rw-r--r--   0        0        0      185 2022-12-27 04:49:41.109488 pii_codex-0.4.5/pii_codex/config.py
--rw-r--r--   0        0        0     6019 2022-12-27 04:49:41.109694 pii_codex-0.4.5/pii_codex/data/v1/pii_type_mappings.csv
--rw-r--r--   0        0        0        0 2022-09-07 01:34:03.205843 pii_codex-0.4.5/pii_codex/models/__init__.py
--rw-r--r--   0        0        0     4652 2023-06-18 23:14:06.935798 pii_codex-0.4.5/pii_codex/models/analysis.py
--rw-r--r--   0        0        0     2091 2023-06-18 23:14:06.935966 pii_codex-0.4.5/pii_codex/models/aws_pii.py
--rw-r--r--   0        0        0    21303 2023-06-18 23:14:06.936262 pii_codex-0.4.5/pii_codex/models/azure_pii.py
--rw-r--r--   0        0        0     4802 2023-06-18 23:14:06.936507 pii_codex-0.4.5/pii_codex/models/common.py
--rw-r--r--   0        0        0     1309 2023-06-18 23:14:06.936694 pii_codex-0.4.5/pii_codex/models/microsoft_presidio_pii.py
--rw-r--r--   0        0        0        0 2022-09-08 17:25:31.250185 pii_codex-0.4.5/pii_codex/services/__init__.py
--rw-r--r--   0        0        0        0 2022-10-08 14:26:22.202772 pii_codex-0.4.5/pii_codex/services/adapters/__init__.py
--rw-r--r--   0        0        0        0 2022-10-16 00:27:31.209902 pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/__init__.py
--rw-r--r--   0        0        0     3853 2022-10-23 00:19:08.465829 pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/aws_detection_adapter.py
--rw-r--r--   0        0        0     1702 2023-05-05 23:01:51.720018 pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/azure_detection_adapter.py
--rw-r--r--   0        0        0      766 2022-10-16 00:27:31.210271 pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/detection_adapter_base.py
--rw-r--r--   0        0        0     2011 2022-10-23 00:19:08.466105 pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/presidio_detection_adapter.py
--rw-r--r--   0        0        0    14792 2023-06-18 23:14:06.936949 pii_codex-0.4.5/pii_codex/services/analysis_service.py
--rw-r--r--   0        0        0        0 2022-10-08 14:26:22.204086 pii_codex-0.4.5/pii_codex/services/analyzers/__init__.py
--rw-r--r--   0        0        0     8715 2023-06-18 23:14:06.937251 pii_codex-0.4.5/pii_codex/services/analyzers/presidio_analysis.py
--rw-r--r--   0        0        0     2742 2023-06-18 23:14:06.937476 pii_codex-0.4.5/pii_codex/services/assessment_service.py
--rw-r--r--   0        0        0        0 2022-09-07 02:11:25.687758 pii_codex-0.4.5/pii_codex/utils/__init__.py
--rw-r--r--   0        0        0     4289 2023-06-18 23:14:06.937704 pii_codex-0.4.5/pii_codex/utils/file_util.py
--rw-r--r--   0        0        0      587 2023-06-18 23:14:06.937907 pii_codex-0.4.5/pii_codex/utils/logging.py
--rw-r--r--   0        0        0      265 2023-06-18 23:14:06.938084 pii_codex-0.4.5/pii_codex/utils/package_installer_util.py
--rw-r--r--   0        0        0     6422 2023-06-18 23:14:06.938254 pii_codex-0.4.5/pii_codex/utils/pii_mapping_util.py
--rw-r--r--   0        0        0     1248 2023-04-27 01:04:58.475940 pii_codex-0.4.5/pii_codex/utils/statistics_util.py
--rw-r--r--   0        0        0     2557 2023-06-18 23:14:06.940526 pii_codex-0.4.5/pyproject.toml
--rw-r--r--   0        0        0    14600 1970-01-01 00:00:00.000000 pii_codex-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1522 2023-06-18 23:38:25.548306 pii_codex-0.4.6/LICENSE
+-rw-r--r--   0        0        0    13307 2023-06-18 23:38:25.548306 pii_codex-0.4.6/README.md
+-rw-r--r--   0        0        0       22 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/__init__.py
+-rw-r--r--   0        0        0      185 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/config.py
+-rw-r--r--   0        0        0     6019 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/data/v1/pii_type_mappings.csv
+-rw-r--r--   0        0        0        0 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/models/__init__.py
+-rw-r--r--   0        0        0     4652 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/models/analysis.py
+-rw-r--r--   0        0        0     2091 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/models/aws_pii.py
+-rw-r--r--   0        0        0    21303 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/models/azure_pii.py
+-rw-r--r--   0        0        0     4802 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/models/common.py
+-rw-r--r--   0        0        0     1309 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/models/microsoft_presidio_pii.py
+-rw-r--r--   0        0        0        0 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/services/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/services/adapters/detection_adapters/__init__.py
+-rw-r--r--   0        0        0     3853 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/services/adapters/detection_adapters/aws_detection_adapter.py
+-rw-r--r--   0        0        0     1702 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/services/adapters/detection_adapters/azure_detection_adapter.py
+-rw-r--r--   0        0        0      766 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/services/adapters/detection_adapters/detection_adapter_base.py
+-rw-r--r--   0        0        0     2011 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/services/adapters/detection_adapters/presidio_detection_adapter.py
+-rw-r--r--   0        0        0    14792 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/services/analysis_service.py
+-rw-r--r--   0        0        0        0 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/services/analyzers/__init__.py
+-rw-r--r--   0        0        0     8715 2023-06-18 23:38:25.552306 pii_codex-0.4.6/pii_codex/services/analyzers/presidio_analysis.py
+-rw-r--r--   0        0        0     2742 2023-06-18 23:38:25.556306 pii_codex-0.4.6/pii_codex/services/assessment_service.py
+-rw-r--r--   0        0        0        0 2023-06-18 23:38:25.556306 pii_codex-0.4.6/pii_codex/utils/__init__.py
+-rw-r--r--   0        0        0     4289 2023-06-18 23:38:25.556306 pii_codex-0.4.6/pii_codex/utils/file_util.py
+-rw-r--r--   0        0        0      587 2023-06-18 23:38:25.556306 pii_codex-0.4.6/pii_codex/utils/logging.py
+-rw-r--r--   0        0        0      265 2023-06-18 23:38:25.556306 pii_codex-0.4.6/pii_codex/utils/package_installer_util.py
+-rw-r--r--   0        0        0     6422 2023-06-18 23:38:25.556306 pii_codex-0.4.6/pii_codex/utils/pii_mapping_util.py
+-rw-r--r--   0        0        0     1248 2023-06-18 23:38:25.556306 pii_codex-0.4.6/pii_codex/utils/statistics_util.py
+-rw-r--r--   0        0        0     2557 2023-06-18 23:38:25.556306 pii_codex-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0    14552 1970-01-01 00:00:00.000000 pii_codex-0.4.6/PKG-INFO
```

### Comparing `pii_codex-0.4.5/LICENSE` & `pii_codex-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/README.md` & `pii_codex-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/data/v1/pii_type_mappings.csv` & `pii_codex-0.4.6/pii_codex/data/v1/pii_type_mappings.csv`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/models/analysis.py` & `pii_codex-0.4.6/pii_codex/models/analysis.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/models/aws_pii.py` & `pii_codex-0.4.6/pii_codex/models/aws_pii.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/models/azure_pii.py` & `pii_codex-0.4.6/pii_codex/models/azure_pii.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/models/common.py` & `pii_codex-0.4.6/pii_codex/models/common.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/models/microsoft_presidio_pii.py` & `pii_codex-0.4.6/pii_codex/models/microsoft_presidio_pii.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/aws_detection_adapter.py` & `pii_codex-0.4.6/pii_codex/services/adapters/detection_adapters/aws_detection_adapter.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/azure_detection_adapter.py` & `pii_codex-0.4.6/pii_codex/services/adapters/detection_adapters/azure_detection_adapter.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/detection_adapter_base.py` & `pii_codex-0.4.6/pii_codex/services/adapters/detection_adapters/detection_adapter_base.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/presidio_detection_adapter.py` & `pii_codex-0.4.6/pii_codex/services/adapters/detection_adapters/presidio_detection_adapter.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/services/analysis_service.py` & `pii_codex-0.4.6/pii_codex/services/analysis_service.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/services/analyzers/presidio_analysis.py` & `pii_codex-0.4.6/pii_codex/services/analyzers/presidio_analysis.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/services/assessment_service.py` & `pii_codex-0.4.6/pii_codex/services/assessment_service.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/utils/file_util.py` & `pii_codex-0.4.6/pii_codex/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/utils/logging.py` & `pii_codex-0.4.6/pii_codex/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/utils/pii_mapping_util.py` & `pii_codex-0.4.6/pii_codex/utils/pii_mapping_util.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pii_codex/utils/statistics_util.py` & `pii_codex-0.4.6/pii_codex/utils/statistics_util.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.5/pyproject.toml` & `pii_codex-0.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pii-codex"
-version = "0.4.5"
+version = "0.4.6"
 description = "PII Detection, Categorization, and Severity Assessment"
 authors = ["Eidan J. Rosado"]
 license = "BSD 3-Clause"
 readme = "README.md"
 homepage = "https://github.com/EdyVision/pii-codex"
 repository = "https://github.com/EdyVision/pii-codex"
 keywords = ["PII", "PII topology", "risk categories", "personal identifiable information", "risk assessment"]
```

### Comparing `pii_codex-0.4.5/PKG-INFO` & `pii_codex-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: pii-codex
-Version: 0.4.5
+Version: 0.4.6
 Summary: PII Detection, Categorization, and Severity Assessment
 Home-page: https://github.com/EdyVision/pii-codex
 License: BSD 3-Clause
 Keywords: PII,PII topology,risk categories,personal identifiable information,risk assessment
 Author: Eidan J. Rosado
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
 Provides-Extra: detections
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: pandas (>=1.4.4,<2.0.0)
 Requires-Dist: pdoc (>=13.1.1,<14.0.0)
 Requires-Dist: pillow (>=9.3.0,<10.0.0)
 Requires-Dist: presidio-analyzer (>=2.2.32,<3.0.0) ; extra == "detections"
 Requires-Dist: presidio-anonymizer (>=2.2.32,<3.0.0) ; extra == "detections"
```

