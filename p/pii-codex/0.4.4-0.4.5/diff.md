# Comparing `tmp/pii_codex-0.4.4.tar.gz` & `tmp/pii_codex-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pii_codex-0.4.4.tar", max compression
+gzip compressed data, was "pii_codex-0.4.5.tar", max compression
```

## Comparing `pii_codex-0.4.4.tar` & `pii_codex-0.4.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1522 2023-04-25 01:18:04.404435 pii_codex-0.4.4/LICENSE
--rw-r--r--   0        0        0     8623 2023-04-25 01:18:04.404435 pii_codex-0.4.4/README.md
--rw-r--r--   0        0        0       22 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/__init__.py
--rw-r--r--   0        0        0      185 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/config.py
--rw-r--r--   0        0        0     6019 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/data/v1/pii_type_mappings.csv
--rw-r--r--   0        0        0        0 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/models/__init__.py
--rw-r--r--   0        0        0     4413 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/models/analysis.py
--rw-r--r--   0        0        0     2035 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/models/aws_pii.py
--rw-r--r--   0        0        0    21249 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/models/azure_pii.py
--rw-r--r--   0        0        0     4031 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/models/common.py
--rw-r--r--   0        0        0     1289 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/models/microsoft_presidio_pii.py
--rw-r--r--   0        0        0        0 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/__init__.py
--rw-r--r--   0        0        0     3853 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/aws_detection_adapter.py
--rw-r--r--   0        0        0     1702 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/azure_detection_adapter.py
--rw-r--r--   0        0        0      766 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/detection_adapter_base.py
--rw-r--r--   0        0        0     2011 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/presidio_detection_adapter.py
--rw-r--r--   0        0        0    14870 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/analysis_service.py
--rw-r--r--   0        0        0        0 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/analyzers/__init__.py
--rw-r--r--   0        0        0     8658 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/analyzers/presidio_analysis.py
--rw-r--r--   0        0        0     2744 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/assessment_service.py
--rw-r--r--   0        0        0        0 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/utils/__init__.py
--rw-r--r--   0        0        0     4099 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/utils/file_util.py
--rw-r--r--   0        0        0      460 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/utils/logging.py
--rw-r--r--   0        0        0      157 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/utils/package_installer_util.py
--rw-r--r--   0        0        0     6300 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/utils/pii_mapping_util.py
--rw-r--r--   0        0        0     1248 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/utils/statistics_util.py
--rw-r--r--   0        0        0     2486 2023-04-25 01:18:04.412435 pii_codex-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     9823 1970-01-01 00:00:00.000000 pii_codex-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1522 2022-09-08 02:13:55.077785 pii_codex-0.4.5/LICENSE
+-rw-r--r--   0        0        0    13307 2023-06-18 23:14:06.926721 pii_codex-0.4.5/README.md
+-rw-r--r--   0        0        0       22 2022-09-07 01:58:01.158467 pii_codex-0.4.5/pii_codex/__init__.py
+-rw-r--r--   0        0        0      185 2022-12-27 04:49:41.109488 pii_codex-0.4.5/pii_codex/config.py
+-rw-r--r--   0        0        0     6019 2022-12-27 04:49:41.109694 pii_codex-0.4.5/pii_codex/data/v1/pii_type_mappings.csv
+-rw-r--r--   0        0        0        0 2022-09-07 01:34:03.205843 pii_codex-0.4.5/pii_codex/models/__init__.py
+-rw-r--r--   0        0        0     4652 2023-06-18 23:14:06.935798 pii_codex-0.4.5/pii_codex/models/analysis.py
+-rw-r--r--   0        0        0     2091 2023-06-18 23:14:06.935966 pii_codex-0.4.5/pii_codex/models/aws_pii.py
+-rw-r--r--   0        0        0    21303 2023-06-18 23:14:06.936262 pii_codex-0.4.5/pii_codex/models/azure_pii.py
+-rw-r--r--   0        0        0     4802 2023-06-18 23:14:06.936507 pii_codex-0.4.5/pii_codex/models/common.py
+-rw-r--r--   0        0        0     1309 2023-06-18 23:14:06.936694 pii_codex-0.4.5/pii_codex/models/microsoft_presidio_pii.py
+-rw-r--r--   0        0        0        0 2022-09-08 17:25:31.250185 pii_codex-0.4.5/pii_codex/services/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-08 14:26:22.202772 pii_codex-0.4.5/pii_codex/services/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-16 00:27:31.209902 pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/__init__.py
+-rw-r--r--   0        0        0     3853 2022-10-23 00:19:08.465829 pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/aws_detection_adapter.py
+-rw-r--r--   0        0        0     1702 2023-05-05 23:01:51.720018 pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/azure_detection_adapter.py
+-rw-r--r--   0        0        0      766 2022-10-16 00:27:31.210271 pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/detection_adapter_base.py
+-rw-r--r--   0        0        0     2011 2022-10-23 00:19:08.466105 pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/presidio_detection_adapter.py
+-rw-r--r--   0        0        0    14792 2023-06-18 23:14:06.936949 pii_codex-0.4.5/pii_codex/services/analysis_service.py
+-rw-r--r--   0        0        0        0 2022-10-08 14:26:22.204086 pii_codex-0.4.5/pii_codex/services/analyzers/__init__.py
+-rw-r--r--   0        0        0     8715 2023-06-18 23:14:06.937251 pii_codex-0.4.5/pii_codex/services/analyzers/presidio_analysis.py
+-rw-r--r--   0        0        0     2742 2023-06-18 23:14:06.937476 pii_codex-0.4.5/pii_codex/services/assessment_service.py
+-rw-r--r--   0        0        0        0 2022-09-07 02:11:25.687758 pii_codex-0.4.5/pii_codex/utils/__init__.py
+-rw-r--r--   0        0        0     4289 2023-06-18 23:14:06.937704 pii_codex-0.4.5/pii_codex/utils/file_util.py
+-rw-r--r--   0        0        0      587 2023-06-18 23:14:06.937907 pii_codex-0.4.5/pii_codex/utils/logging.py
+-rw-r--r--   0        0        0      265 2023-06-18 23:14:06.938084 pii_codex-0.4.5/pii_codex/utils/package_installer_util.py
+-rw-r--r--   0        0        0     6422 2023-06-18 23:14:06.938254 pii_codex-0.4.5/pii_codex/utils/pii_mapping_util.py
+-rw-r--r--   0        0        0     1248 2023-04-27 01:04:58.475940 pii_codex-0.4.5/pii_codex/utils/statistics_util.py
+-rw-r--r--   0        0        0     2557 2023-06-18 23:14:06.940526 pii_codex-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0    14600 1970-01-01 00:00:00.000000 pii_codex-0.4.5/PKG-INFO
```

### Comparing `pii_codex-0.4.4/LICENSE` & `pii_codex-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.4/pii_codex/data/v1/pii_type_mappings.csv` & `pii_codex-0.4.5/pii_codex/data/v1/pii_type_mappings.csv`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.4/pii_codex/models/analysis.py` & `pii_codex-0.4.5/pii_codex/models/analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,35 @@
 
 
 # PII detection, risk assessment, and analysis models
 
 
 @dataclass
 class RiskAssessment:
+    """
+    Singular risk assessment for a string token
+    """
+
     pii_type_detected: Optional[str] = None
     risk_level: int = RiskLevel.LEVEL_ONE.value
     risk_level_definition: str = (
         RiskLevelDefinition.LEVEL_ONE.value
     )  # Default if it's not semi or fully identifiable
     cluster_membership_type: Optional[str] = None
     hipaa_category: Optional[str] = None
     dhs_category: Optional[str] = None
     nist_category: Optional[str] = None
 
 
 @dataclass
 class RiskAssessmentList:
+    """
+    Risk Assessments and the average risk score of all list items
+    """
+
     risk_assessments: List[RiskAssessment]
     average_risk_score: float
 
 
 @dataclass
 class DetectionResultItem:
     """
@@ -40,14 +48,18 @@
     score: float = 0.0  # metadata detections don't have confidence score values
     start: int = 0  # metadata detections don't have offset values
     end: int = 0  # metadata detections don't have offset values
 
 
 @dataclass
 class DetectionResult:
+    """
+    List of detection results and the index of the string they pertain to
+    """
+
     detections: List[DetectionResultItem]
     index: int = 0
 
 
 @dataclass
 class AnalysisResultItem:
     """
```

### Comparing `pii_codex-0.4.4/pii_codex/models/aws_pii.py` & `pii_codex-0.4.5/pii_codex/models/aws_pii.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 # PII Types and Models as expanded in research
 # Research Page:
 # AWS Comprehend PII Docs: https://docs.aws.amazon.com/comprehend/latest/dg/how-pii.html
 
 
 class AWSComprehendPIIType(Enum):
+    """
+    AWS Comprehend-Supported PII types
+    """
+
     EMAIL_ADDRESS: str = "EMAIL"
     ADDRESS: str = "ADDRESS"
     PERSON: str = "NAME"
     PHONE_NUMBER: str = "PHONE"
     DATE: str = "DATE_TIME"
     URL: str = "URL"
     AGE: str = "AGE"
```

### Comparing `pii_codex-0.4.4/pii_codex/models/azure_pii.py` & `pii_codex-0.4.5/pii_codex/models/azure_pii.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Research Page:
 # https://azuresdkdocs.blob.core.windows.net/$web/python/azure-ai-textanalytics/latest/
 # azure.ai.textanalytics.html#azure.ai.textanalytics.TextAnalyticsClient.recognize_pii_entities
 
 
 class AzureDetectionType(Enum):
     """
-    The values fed into the Azure service for detection
+    Azure-supported PII Types: The values fed into the Azure service for detection
     """
 
     ABA_ROUTING_NUMBER: str = "ABARoutingNumber"
     ADDRESS: str = "Address"
     AGE: str = "Age"
     AR_NATIONAL_IDENTITY_NUMBER: str = "ARNationalIdentityNumber"
     AT_IDENTITY_CARD: str = "ATIdentityCard"
@@ -197,15 +197,15 @@
     US_SOCIAL_SECURITY_NUMBER: str = "USSocialSecurityNumber"
     ZA_IDENTIFICATION_NUMBER: str = "ZAIdentificationNumber"
     ALL: str = "All"
 
 
 class AzurePIIType(Enum):
     """
-    The values of types returned from the Azure Cognition PII Detection API
+    Azure-supported PII Types: The values of types returned from the Azure Cognition PII Detection API
     """
 
     ABA_ROUTING_NUMBER: str = "ABA Routing Number"
     ADDRESS: str = "Address"
     AGE: str = "Age"
     AR_NATIONAL_IDENTITY_NUMBER: str = "AR National Identity Number"
     AT_IDENTITY_CARD: str = "ATIdentityCard"
```

### Comparing `pii_codex-0.4.4/pii_codex/models/common.py` & `pii_codex-0.4.5/pii_codex/models/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,41 +3,60 @@
 from enum import Enum
 
 # All listed PII Types from Milne et al (2018) and a few others along with
 # models used for PII categorization for DHS, NIST, and HIPAA
 
 
 class AnalysisProviderType(Enum):
+    """
+    Analysis Provider Types - software and cloud service APIs providing PII detection results
+    """
+
     AZURE: str = "AZURE"
     AWS: str = "AWS"
     PRESIDIO: str = "PRESIDIO"
 
 
 class RiskLevel(Enum):
+    """
+    Numerical values assigned to the levels on the continuum presented by Schwartz and Solove (2011)
+    """
+
     LEVEL_ONE: int = 1  # Not-Identifiable
     LEVEL_TWO: int = 2  # Semi-Identifiable
     LEVEL_THREE: int = 3  # Identifiable
 
 
 class RiskLevelDefinition(Enum):
-    # Levels on the continuum presented by Schwartz and Solove (2011)
+    """
+    Levels on the continuum presented by Schwartz and Solove (2011)
+    """
+
     LEVEL_ONE: str = "Non-Identifiable"  # Default if no entities were detected, risk level is set to this
     LEVEL_TWO: str = "Semi-Identifiable"
     LEVEL_THREE: str = "Identifiable"  # Level associated with Directly PII, PHI, and Standalone PII info types
 
 
 class MetadataType(Enum):
+    """
+    Common metadata types associated with social media posts and other online platforms
+    """
+
     SCREEN_NAME: str = "screen_name"
     NAME: str = "name"
     LOCATION: str = "location"
     URL: str = "url"
     USER_ID: str = "user_id"
 
 
 class PIIType(Enum):
+    """
+    Commonly observed PII types across services and software
+    """
+
     PHONE_NUMBER: str = "PHONE"
     WORK_PHONE_NUMBER: str = "PHONE"
     EMAIL_ADDRESS: str = "EMAIL"
     ABA_ROUTING_NUMBER: str = "ABA_ROUTING_NUMBER"
     IP_ADDRESS: str = "IP_ADDRESS"
     DATE: str = "DATE"
     ADDRESS: str = "ADDRESS"
@@ -87,29 +106,45 @@
     US_INDIVIDUAL_TAXPAYER_IDENTIFICATION: str = "US_INDIVIDUAL_TAXPAYER_IDENTIFICATION"
     INTERNATIONAL_BANKING_ACCOUNT_NUMBER: str = "INTERNATIONAL_BANKING_ACCOUNT_NUMBER"
     SWIFT_CODE: str = "SWIFTCode"
     NRP: str = "NRP"  # A person's nationality, religion, or political group
 
 
 class NISTCategory(Enum):
+    """
+    Information Categories presented by NIST as noted in Milne et al., 2016
+    """
+
     LINKABLE: str = "Linkable"
     DIRECTLY_PII: str = "Directly PII"
 
 
 class DHSCategory(Enum):
+    """
+    Information Categories presented by DHS as noted in Milne et al., 2016
+    """
+
     NOT_MENTIONED: str = "Not Mentioned"
     LINKABLE: str = "Linkable"
     STAND_ALONE_PII: str = "Stand Alone PII"
 
 
 class HIPAACategory(Enum):
+    """
+    Information Categories presented by HIPAA guidelines
+    """
+
     NON_PHI: str = "Not Protected Health Information"
     PHI: str = "Protected Health Information"
 
 
 class ClusterMembershipType(Enum):
+    """
+    Information Cluster Memberships presented by Milne et al., 2016
+    """
+
     BASIC_DEMOGRAPHICS: str = "Basic Demographics"
     PERSONAL_PREFERENCES: str = "Personal Preferences"
     CONTACT_INFORMATION: str = "Contact Information"
     COMMUNITY_INTERACTION: str = "Community Interaction"
     FINANCIAL_INFORMATION: str = "Financial Information"
     SECURE_IDENTIFIERS: str = "Secure Identifiers"
```

### Comparing `pii_codex-0.4.4/pii_codex/models/microsoft_presidio_pii.py` & `pii_codex-0.4.5/pii_codex/models/microsoft_presidio_pii.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 from enum import Enum
 
-# PII Types associated with Microsoft Presidio Analyzer
-# Supported Entities: https://microsoft.github.io/presidio/supported_entities/
-
 
 class MSFTPresidioPIIType(Enum):
+    """
+    PII Types associated with Microsoft Presidio Analyzer
+    Supported Entities: https://microsoft.github.io/presidio/supported_entities/
+    """
+
     PHONE_NUMBER: str = "PHONE_NUMBER"
     EMAIL_ADDRESS: str = "EMAIL_ADDRESS"
     ABA_ROUTING_NUMBER: str = "ABA_ROUTING_NUMBER"
     IP_ADDRESS: str = "IP_ADDRESS"
     DATE: str = "DATE_TIME"
     ADDRESS: str = "LOCATION"
     AGE: str = "AGE"
```

### Comparing `pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/aws_detection_adapter.py` & `pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/aws_detection_adapter.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/azure_detection_adapter.py` & `pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/azure_detection_adapter.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/detection_adapter_base.py` & `pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/detection_adapter_base.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/presidio_detection_adapter.py` & `pii_codex-0.4.5/pii_codex/services/adapters/detection_adapters/presidio_detection_adapter.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.4/pii_codex/services/analysis_service.py` & `pii_codex-0.4.5/pii_codex/services/analysis_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,20 @@
     get_mean,
     get_standard_deviation,
     get_variance,
     get_mode,
     get_median,
 )
 
-from ..utils.logging import timed_operation
-
 
 class PIIAnalysisService:
+    """
+    Class for PII analysis of singular text strings or collections thereof.
+    """
+
     def __init__(
         self,
         pii_token_replacement_value: str = DEFAULT_TOKEN_REPLACEMENT_VALUE,
         analysis_provider: str = AnalysisProviderType.PRESIDIO.name,
     ):
         """
         PIIAnalysisService constructor.
@@ -48,15 +50,14 @@
         self._pii_assessment_service = PIIAssessmentService()
         self._analyzer = (
             PresidioPIIAnalyzer(pii_token_replacement_value=pii_token_replacement_value)
             if analysis_provider == AnalysisProviderType.PRESIDIO.name
             else None
         )
 
-    @timed_operation
     def analyze_item(
         self,
         text: str,
         metadata: dict = None,
         language_code: str = "en",
     ) -> AnalysisResult:
         """
@@ -84,15 +85,14 @@
             analysis=analysis,
             sanitized_text=sanitized_text,
             risk_score_mean=get_mean(
                 [item.risk_assessment.risk_level for item in analysis]
             ),
         )
 
-    @timed_operation
     def analyze_collection(
         self,
         texts: Optional[List[str]] = None,
         data: Optional[pd.DataFrame] = None,
         language_code: str = "en",
         collection_name: str = "",
         collection_type: str = "population",
@@ -171,15 +171,14 @@
 
         return self._format_result_set_item(
             analysis_items=analysis,
             sanitized_text=sanitized_text,
             index=idx,
         )
 
-    @timed_operation
     def analyze_detection_collection(
         self,
         detection_collection: List[DetectionResult],
         collection_name: str = "",
         collection_type: str = "population",
     ) -> AnalysisResultSet:
         """
@@ -203,15 +202,14 @@
 
         return self._build_analysis_result_set(
             collection_name=collection_name,
             collection_type=collection_type,
             analysis_set=analysis_set,
         )
 
-    @timed_operation
     def analyze_detection_result(
         self, detection_result: DetectionResult, index: int = 0
     ) -> AnalysisResult:
         """
         Transforms a Detection Result to an AnalysisResult with RiskAssessments for all detections
         found in a string/document.
 
@@ -227,15 +225,14 @@
             index=index,
             analysis=detection_analyses,
             risk_score_mean=get_mean(
                 [analysis.risk_assessment.risk_level for analysis in detection_analyses]
             ),
         )
 
-    @timed_operation
     def analyze_detection_result_item(
         self,
         detection_result_item: DetectionResultItem,
     ) -> AnalysisResultItem:
         """
         Transforms a Detection Result Item to an AnalysisResultItem with its associated RiskAssessment for the singular
         detection within a string/document.
@@ -289,15 +286,14 @@
                 )
                 for detection in detections
             ]
             if detections
             else [AnalysisResultItem(detection=None, risk_assessment=RiskAssessment())]
         ), sanitized_text
 
-    @timed_operation
     def analyze_metadata(self, metadata: dict):
         """
         Create an analysis result item per metadata entry
 
         @param metadata:
         @return:
         """
```

### Comparing `pii_codex-0.4.4/pii_codex/services/analyzers/presidio_analysis.py` & `pii_codex-0.4.5/pii_codex/services/analyzers/presidio_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # pylint: disable=broad-except,unused-argument,import-outside-toplevel,unused-variable
 from typing import List, Tuple
 
 from ...config import PII_MAPPER, DEFAULT_LANG, DEFAULT_TOKEN_REPLACEMENT_VALUE
 from ...models.analysis import DetectionResultItem, DetectionResult
 from ...utils.package_installer_util import install_spacy_package
 from ...utils.pii_mapping_util import PIIMapper
-from ...utils.logging import logger, timed_operation
+from ...utils.logging import logger
 
 
 class PresidioPIIAnalyzer:
+    """
+    Presidio PII Analyzer - a wrapper for the Microsoft Presidio Analyzer and Anonymization functions
+    """
+
     def __init__(
         self, pii_token_replacement_value: str = DEFAULT_TOKEN_REPLACEMENT_VALUE
     ):
         """
         Since installing Spacy, the en_core_web_lg model, and the MSFT Presidio package are optional installs
         the imports are wrapped to prevent any failures
         @param pii_token_replacement_value: str to replace detected pii token with (e.g. <REDACTED>)
         """
+
         try:
             import spacy
             from presidio_analyzer import AnalyzerEngine
             from presidio_anonymizer import AnonymizerEngine
             from presidio_anonymizer.entities import OperatorConfig
 
             if not spacy.util.is_package("en_core_web_lg"):
@@ -56,15 +61,14 @@
         """
         Retrieves a list of loaded recognizers, narrowing down the list of what is available for a given language
         @param language_code:
         @return:
         """
         return self.analyzer.get_recognizers(language=language_code)  # type: ignore
 
-    @timed_operation
     def analyze_item(
         self, text: str, language_code: str = DEFAULT_LANG, entities: List[str] = None
     ) -> Tuple[List[DetectionResultItem], str]:
         """
         Uses Microsoft Presidio (spaCy module) to analyze given a set of entities to analyze the provided text against.
         Will log an error if the identifier or entity recognizer is not added to Presidio's base recognizers or
         a custom recognizer created. Returns the list of detected items and the sanitized string
@@ -116,15 +120,14 @@
 
             return anonymization_result.text
 
         except Exception as ex:
             logger.error("An error occurred sanitizing the string")
             return ""
 
-    @timed_operation
     def analyze_collection(
         self, texts: List[str], language_code: str = "en", entities: List[str] = None
     ) -> List[DetectionResult]:
         """
         Uses Microsoft Presidio (spaCy module) to analyze given a set of entities to analyze the provided text against.
         Will log an error if the identifier or entity recognizer is not added to Presidio's base recognizers or
         a custom recognizer created.
@@ -166,15 +169,14 @@
 
         except Exception as ex:
             logger.error(ex)
 
         return detection_results
 
     @classmethod
-    @timed_operation
     def convert_analyzed_item(cls, pii_detection) -> List[DetectionResultItem]:
         """
         Converts a single Presidio analysis attempt into a collection of DetectionResultItem objects. One string
         analysis by Presidio returns an array of RecognizerResult objects.
 
         @param pii_detection: RecognizerResult from presidio analyzer
         @return: List[DetectionResultItem]
@@ -189,22 +191,21 @@
                 start=result.start,
                 end=result.end,
             )
             for result in pii_detection
         ]
 
     @classmethod
-    @timed_operation
     def convert_analyzed_collection(cls, pii_detections) -> List[DetectionResult]:
         """
         Converts a collection of Presidio analysis results to a collection of DetectionResult. A collection of Presidio
         analysis results ends up being a 2D array.
 
         @param pii_detections: List[RecognizerResult] from Presidio analyzer
-
+        @return: List[DetectionResult]
         """
 
         detection_results: List[DetectionResult] = []
         for i, result in enumerate(pii_detections):
             # Return results in formatted Analysis Result List object
             detections = []
             for entity in result:
```

### Comparing `pii_codex-0.4.4/pii_codex/services/assessment_service.py` & `pii_codex-0.4.5/pii_codex/services/assessment_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from typing import List, Tuple
 from collections import Counter
 from itertools import chain
 
 from ..config import PII_MAPPER
 from ..models.analysis import RiskAssessment, AnalysisResult
-from ..utils.logging import timed_operation
 from ..utils.statistics_util import get_mean, get_sum
 
 
 class PIIAssessmentService:
-    @timed_operation
+    """
+    Class for mapping PII types to categories and extracting them.
+    """
+
     def assess_pii_type(self, detected_pii_type: str) -> RiskAssessment:
         """
         Assesses a singular detected PII type given a type name string from common.PIIType enum
         @param detected_pii_type: type name strings from common.PIIType enum
         @return: RiskAssessment
         """
         return PII_MAPPER.map_pii_type(detected_pii_type)
 
-    @timed_operation
     def assess_pii_type_list(
         self, detected_pii_types: List[str]
     ) -> List[RiskAssessment]:
         """
         Assesses a list of detected PII types given an array of type name strings from common.PIIType enum
         @param detected_pii_types: array type name strings from common.PIIType
         enum (e.g. ["PHONE_NUMBER", "US_SOCIAL_SECURITY_NUMBER"])
```

### Comparing `pii_codex-0.4.4/pii_codex/utils/file_util.py` & `pii_codex-0.4.5/pii_codex/utils/file_util.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 dirname = os.path.dirname(__file__)
 
 
 def get_relative_path(path_to_file: str):
     """
     Returns the file_path relative to the project
 
-    @param path_to_file:
-    @return:
+    @param path_to_file: str
+    @return: Path
     """
     filename = os.path.join(dirname, path_to_file)
 
     return Path(__file__).parent / filename
 
 
 def write_json_file(folder_name: str, file_name: str, json_data):
     """
     Writes json file given json data, a folder name, and a file name.
 
-    @param folder_name:
-    @param file_name:
+    @param folder_name: str
+    @param file_name: str
     @param json_data:
     """
     # Create a new directory because it does not exist
     if not os.path.exists(folder_name):
         os.makedirs(folder_name)
 
         logger.info(f"A new version directory has been created: {folder_name}")
@@ -48,16 +48,15 @@
 
 def delete_file(
     file_path: str = "pii_type_mappings",
 ):
     """
     Deletes a version file if it exists
 
-    @param file_path:
-    @return:
+    @param file_path: str
     """
 
     # Delete file if it exists
     if os.path.exists(file_path):
         os.remove(file_path)
 
         logger.info(f"The file {file_path} has been deleted")
@@ -67,15 +66,15 @@
 
 def delete_folder(
     folder_path: str,
 ):
     """
     Deletes a folder if it exists and nothing is within it
 
-    @param folder_path:
+    @param folder_path: str
     """
 
     # Delete folder if it exists
     if os.path.exists(folder_path):
         os.rmdir(folder_path)
 
         logger.info(f"The folder {folder_path} has been deleted")
@@ -86,33 +85,34 @@
 # region MAPPING FILE UTILS
 
 
 def open_pii_type_mapping_csv(
     mapping_file_version: str = "v1", mapping_file_name: str = "pii_type_mappings"
 ):
     """
+    Opens the PII type mappings CSV file and returns a Pandas DataFrame
 
-    @param mapping_file_name:
-    @param mapping_file_version:
+    @param mapping_file_name: str
+    @param mapping_file_version: str
     """
     file_path = get_relative_path(
         f"../data/{mapping_file_version}/{mapping_file_name}.csv"
     )
     with file_path.open() as file:
         return pd.read_csv(file)
 
 
 def open_pii_type_mapping_json(
     mapping_file_version: str = "v1", mapping_file_name: str = "pii_type_mappings"
 ):
     """
+    Opens the PII type mappings JSON file and returns a Pandas DataFrame
 
-    @param mapping_file_name:
-    @param mapping_file_version:
-    @return:
+    @param mapping_file_name: str
+    @param mapping_file_version: str
     """
 
     file_path = get_relative_path(
         f"../data/{mapping_file_version}/{mapping_file_name}.json"
     )
     with file_path.open() as file:
         json_file_dataframe = pd.read_json(file)
@@ -125,17 +125,17 @@
     data_frame: pd.DataFrame,
     mapping_file_version: str = "v1",
     json_file_name: str = "pii_type_mappings",
 ):
     """
     Writes JSON mapping file given a dataframe. Used primarily to update data folder with new versions
 
-    @param data_frame:
-    @param mapping_file_version:
-    @param json_file_name:
+    @param data_frame: DataFrame
+    @param mapping_file_version: str
+    @param json_file_name: str
     """
 
     folder_path = get_relative_path(f"../data/{mapping_file_version}")
 
     file_path = get_relative_path(
         f"../data/{mapping_file_version}/{json_file_name}.json"
     )
@@ -150,16 +150,16 @@
 def delete_json_mapping_file(
     mapping_file_version: str = "v1",
     json_file_name: str = "pii_type_mappings",
 ):
     """
     Deletes a version file within a data version folder
 
-    @param mapping_file_version:
-    @param json_file_name:
+    @param mapping_file_version: str
+    @param json_file_name: str
     """
 
     file_path = get_relative_path(
         f"../data/{mapping_file_version}/{json_file_name}.json"
     )
 
     delete_file(file_path)
@@ -167,15 +167,15 @@
 
 def delete_json_mapping_folder(
     mapping_file_version: str,
 ):
     """
     Deletes a version folder within the data folder
 
-    @param mapping_file_version:
+    @param mapping_file_version: str
     """
 
     folder_path = get_relative_path(f"../data/{mapping_file_version}")
     delete_folder(folder_path)
 
 
 # endregion
```

### Comparing `pii_codex-0.4.4/pii_codex/utils/pii_mapping_util.py` & `pii_codex-0.4.5/pii_codex/utils/pii_mapping_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 from pii_codex.models.analysis import RiskAssessment
 from pii_codex.models.microsoft_presidio_pii import MSFTPresidioPIIType
 
 from pii_codex.utils.file_util import open_pii_type_mapping_csv
 
 
 class PIIMapper:
+    """
+    Class to map PII types listed as Common Types, Azure Types, AWS Comprehend Types, and Presidio Types
+    """
+
     def __init__(self):
         self._pii_mapping_data_frame = open_pii_type_mapping_csv("v1")
 
     def map_pii_type(self, pii_type: str) -> RiskAssessment:
         """
         Maps the PII Type to a full RiskAssessment including categories it belongs to, risk level, and
         its location in the text. This cross-references some of the types listed by Milne et al. (2016)
```

### Comparing `pii_codex-0.4.4/pii_codex/utils/statistics_util.py` & `pii_codex-0.4.5/pii_codex/utils/statistics_util.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.4/pyproject.toml` & `pii_codex-0.4.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pii-codex"
-version = "0.4.4"
-description = ""
+version = "0.4.5"
+description = "PII Detection, Categorization, and Severity Assessment"
 authors = ["Eidan J. Rosado"]
 license = "BSD 3-Clause"
 readme = "README.md"
 homepage = "https://github.com/EdyVision/pii-codex"
 repository = "https://github.com/EdyVision/pii-codex"
 keywords = ["PII", "PII topology", "risk categories", "personal identifiable information", "risk assessment"]
 classifiers = [
@@ -23,14 +23,15 @@
 pillow = "^9.3.0"  # security dependency
 
 # Optional items for analyses - users have the option to use the integrated Presidio analyzer or
 # avoid installing the following and bring their own detector, using the adapters
 spacy = { version = "^3.5.2", optional = true }
 presidio-analyzer = { version = "^2.2.32", optional = true }
 presidio-anonymizer = { version ="^2.2.32", optional = true }
+pdoc = "^13.1.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 black = "22.12.0"
 pylint = "^2.15.4"
 mypy = "^0.982"
 coverage = "^6.4.4"
```

### Comparing `pii_codex-0.4.4/PKG-INFO` & `pii_codex-0.4.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,90 @@
-Metadata-Version: 2.1
-Name: pii-codex
-Version: 0.4.4
-Summary: 
-Home-page: https://github.com/EdyVision/pii-codex
-License: BSD 3-Clause
-Keywords: PII,PII topology,risk categories,personal identifiable information,risk assessment
-Author: Eidan J. Rosado
-Requires-Python: >=3.9,<3.11
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
-Provides-Extra: detections
-Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
-Requires-Dist: pandas (>=1.4.4,<2.0.0)
-Requires-Dist: pillow (>=9.3.0,<10.0.0)
-Requires-Dist: presidio-analyzer (>=2.2.32,<3.0.0) ; extra == "detections"
-Requires-Dist: presidio-anonymizer (>=2.2.32,<3.0.0) ; extra == "detections"
-Requires-Dist: pydantic[dotenv] (>=1.10.2,<2.0.0)
-Requires-Dist: spacy (>=3.5.2,<4.0.0) ; extra == "detections"
-Project-URL: Repository, https://github.com/EdyVision/pii-codex
-Description-Content-Type: text/markdown
-
 <div align="center">
 
 ![alt text](https://github.com/EdyVision/pii-codex/blob/main/docs/PII_Codex_Logo.svg?raw=true)
 
 PII Detection, Categorization, and Severity Assessment
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 ![](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/EdyVision/pii-codex/graphs/commit-activity)
 [![codecov](https://codecov.io/gh/EdyVision/pii-codex/branch/main/graph/badge.svg?token=QO7DNMP87X)](https://codecov.io/gh/EdyVision/pii-codex)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![DOI](https://zenodo.org/badge/533554671.svg)](https://zenodo.org/badge/latestdoi/533554671)
+[![status](https://joss.theoj.org/papers/5296a84bba0925e682dcddf14bec5880/status.svg)](https://joss.theoj.org/papers/5296a84bba0925e682dcddf14bec5880)
 
 </div>
 
 ---
+
+Author: Eidan Rosado - [@EdyVision](https://github.com/EdyVision)  <br/>
+Affiliation: Nova Southeastern University, College of Computing and Engineering
+
+## Project Background
 The <em>PII Codex</em> project was built as a core part of an ongoing research effort in Personal Identifiable Information (PII) detection and risk assessment (to be publicly released later in 2023). There was a need to not only detect PII in text, but also identify its severity, associated categorizations in cybersecurity research and policy documentation, and provide a way for others in similar research efforts to reproduce or extend the research. PII Codex is a combination of systematic research, conceptual frameworks, third-party open source software, and cloud service provider integrations. The categorizations are directly influenced by the research of Milne et al. (2016) while the ranking is a result of category severities on the scale provided by Schwartz and Solove (2012) from Non-Identifiable, Semi-Identifiable, and Identifiable.
 
 The outputs of the primary PII Codex analysis and adapter functions are AnalysisResult or AnalysisResultSet objects that will provide a listing of detections, severities, mean risk scores for each string processed, and summary statistics on the analysis made. The final outputs do not contain the original texts but instead will provide where to find the detections should the end-user care for this information in their analysis.
 
-## Statement of Need
+### Statement of Need
 
 The general knowledge base of identifiable data, the usage restrictions of this data, and the associated policies surrounding it have shifted drastically over the years. The tech industry has had to adjust to many policy changes regarding the tracking of individuals, the usage of data from online profiles and platforms, and the right to be forgotten entirely from a service or platform (GDPR). While the shift has provided data protections around the globe, the majority of technology users continue to have little to no control over their personal information with third-party data consumers (Trepte, 2020). 
 
 Understanding if identifiable data types exist in a data set can prevent accidental sharing of such data by allowing its detection in the first place and, in the case of this software package, present sanitized strings, the reasons to why the token was considered to be PII, and permit for the results to be publishable.
 
-## Potential Usages
+### Potential Usages
 Potential usages include sanitizing of dataset strings (e.g. a collection of social media posts), presenting results to users for software examining their interactions (e.g. UX research on user-awareness in cybersecurity applications), etc.
 
 <hr/>
 
-## Running Locally
+## Running Locally with Poetry
 This project uses Poetry. To run this project, install `poetry` and proceed to follow the instructions under `/docs/LOCAL_SETUP.md`.
 
-`Note: This project has only been tested with Ubuntu and MacOS.`
+`Note: This project has only been tested with Ubuntu and MacOS and with Python versions 3.9 and 3.10. You may need to upgrade pip ahead of installation.`
+
+## Installing with PIP
+Video capture of install provided in LOCAL_SETUP.md file. Make sure you set up a virtual environment with either python 3.9 or 3.10 and upgrade pip with:
+
+```bash
+pip install --upgrade pip
+pip install -U pip setuptools wheel # only needed if you haven't already done so 
+```
 
-## Importing
 Before adding `pii-codex` on your project, download the spaCy `en_core_web_lg` model:
 
 ```bash
+pip install -U spacy
 python3 -m spacy download en_core_web_lg
 ```
 
+For more details on spaCy installation and usage, refer to their <a href="https://spacy.io/usage">docs</a>.
 
-The repository releases are hosted on PyPi.
-
-Using pip (must have latest pip version and running Python 3.9 or 3.10):
+The repository releases are hosted on PyPi and can be installed with:
 
 ```bash
-pip install --upgrade pip
 pip install pii-codex
-pip install pii-codex[detections]
+pip install "pii-codex[detections]"
 ```
 
+`Note: The extras installed with pii-codex[detections] are the spaCy, Micrisoft Presidio Analyzer, and Microsoft Anonymzer packages.`
+
 Using Poetry:
 
 ```bash
 poetry update
 poetry add pii-codex
 poetry install pii-codex --extras="detections"
 ```
 
 For those using Google Collab, check out the example notebook:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/EdyVision/802ce21aab21eb5d9afa9e43d301eef7/pii-codex-sample-notebook.ipynb)
 
 ## Usage
+Video capture of usage provided in LOCAL_SETUP.md.
 
 ### Sample Input / Output
 The built-in analyzer uses Microsoft Presidio. Feed in a collection of strings with analyze_collection() or just a single string with analyze_item(). Those analyzing a collection of strings will also be provided with statistics calculated on the risk scores for detected items.
 ```python
 from pii_codex.services.analysis_service import PIIAnalysisService
 PIIAnalysisService().analyze_collection(
     texts=["your collection of strings"],
@@ -160,19 +147,39 @@
     },
 }
 ```
 
 ### Docs
 For more information on usage, check out the respective documentation for guidance on using PII-Codex.
 
-| Topic                       | Document                                                     | Description                                                                              |
-|-----------------------------|--------------------------------------------------------------|------------------------------------------------------------------------------------------|
-| PII Type Mappings           | [PII Mappings](docs/MAPPING.md)                              | Overview of how to perform mappings between PII types and how to review store PII types. |
-| PII Detections and Analysis | [PII Detection and Analysis](docs/DETECTION_AND_ANALYSIS.md) | Overview of how to detect and analyze strings                                            |
-| Local Repo Setup            | [Local Repo Setup](docs/LOCAL_SETUP.md)                      | Instructions for local repository setup                                                  |
-| Example Analysis            | [Example Analysis Notebook](notebooks/pii-analysis-ms-presidio.ipynb)  | Notebook with example analysis using MSFT Presidio                             |
+| Topic                       | Document                                                              | Description                                                                              |
+|-----------------------------|-----------------------------------------------------------------------|------------------------------------------------------------------------------------------|
+| PII Type Mappings           | [PII Mappings](docs/MAPPING.md)                                       | Overview of how to perform mappings between PII types and how to review store PII types. |
+| PII Detections and Analysis | [PII Detection and Analysis](docs/DETECTION_AND_ANALYSIS.md)          | Overview of how to detect and analyze strings                                            |
+| Local Repo Setup            | [Local Repo Setup](docs/LOCAL_SETUP.md)                               | Instructions for local repository setup                                                  |
+| Example Analysis            | [Example Analysis Notebook](notebooks/pii-analysis-ms-presidio.ipynb) | Notebook with example analysis using MSFT Presidio                                       |
+| PII-Codex Docs              | docs/pii_codex/index.html                                             | Autogenerated docs on classes, services, and models                                      |
 
 <hr/>
 
 ## Attributions
-This project benefited greatly from a number of PII research works like that from Milne et al (2016) with the definition of the types and categories, Schwartz and Solove (2012) with the severity levels of Non-Identifiable, Semi-Identifiable, and Identifiable, and the documentation by NIST, DHS (2012), and HIPAA. A special thanks to all the open source projects, and frameworks that made the setup and structuring of this project much easier like Poetry, Microsoft Presidio, spaCy (2017), Jupyter, and several others.
+This project benefited greatly from a number of PII research works like that from Milne et al (2016) with the definition of the types and categories, Schwartz and Solove (2012) with the severity levels of Non-Identifiable, Semi-Identifiable, and Identifiable, and the documentation by NIST, DHS (2012), and HIPAA (full list of foundational publications provided below). A special thanks to all the open source projects, and frameworks that made the setup and structuring of this project much easier like Poetry, Microsoft Presidio, spaCy (2017), Jupyter, and several others.
+
+### Foundational Publications
+The following publications that inspired and provided a foundation for this repository:
+
+| Concept                                   | Document                                                                                                                                          | Description                                                                    |
+|-------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------|
+| PII Type Mappings                         | [Milne et al., (2016)](https://onlinelibrary.wiley.com/doi/abs/10.1111/joca.12111)                                                                | PII token categories and NIST and DHS categorizations.                         |
+| Risk Continuum                            | [Schwartz & Solove, (2011)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1909366)                                                          | Risk continuum concept and definition (what lead to the ranking in PII-Codex). |
+| Privacy and Affordances                   | [Trepte, (2020)](https://academic.oup.com/ct/article-abstract/31/4/549/5828289?redirectedFrom=fulltext)                                           | Third-Party data consumption and user control (lack thereof) background.       |
+| Social Media and Privacy                  | [Beigi & Liu, (2010)](https://dl.acm.org/doi/10.1145/3343038)                                                                                     | Privacy issues with social media and third-party data consumption.             |
+| Privacy Settings and Data Access          | [Moura & Serrão, (2016)](https://www.researchgate.net/publication/332996823_Security_and_Privacy_Issues_of_Big_Data)                              | Privacy settings, data access, and unauthorized usage.                         |
+| Information Privacy Review                | [Bélanger & Crossler, (2011)](https://www.jstor.org/stable/41409971)                                                                              | Concept of aggregation of data to identify individuals.                        |
+| Big Data and Third Party Data Consumption | [Tene & Polonetsky, (2013)](https://www.researchgate.net/publication/256035043_Big_Data_for_All_Privacy_and_User_Control_in_the_Age_of_Analytics) | Third-party data usage, user control, and privacy.                             |
+| PII and Confidentiality                   | [McCallister et al., (2010)](https://csrc.nist.gov/publications/detail/sp/800-122/final)                                                          | NIST guidance on PII confidentiality protections for federal agencies.         |
+| Data Capitalism and Privacy               | [West, (2017)](https://journals.sagepub.com/doi/pdf/10.1177/0007650317718185)                                                                     | Data capitalism, surveillance, and privacy.                |
+
+The remaining resources such as python library citations, cloud service provider docs, and cybersecurity guidelines are included in the paper.bib file.
 
+## Community Guidelines
+For community guidelines and contribution instructions, please view the [CONTRIBUTING.md](./CONTRIBUTING.md) file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

