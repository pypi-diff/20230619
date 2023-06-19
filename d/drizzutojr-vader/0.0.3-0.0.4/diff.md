# Comparing `tmp/drizzutojr_vader-0.0.3-py3-none-any.whl.zip` & `tmp/drizzutojr_vader-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 6275 bytes, number of entries: 14
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-19 16:11 vader/__init__.py
--rw-r--r--  2.0 unx     1094 b- defN 23-Jun-19 16:11 vader/core_service.py
--rw-r--r--  2.0 unx     1015 b- defN 23-Jun-19 16:11 vader/exceptions.py
--rw-r--r--  2.0 unx     1425 b- defN 23-Jun-19 16:11 vader/general.py
--rw-r--r--  2.0 unx      665 b- defN 23-Jun-19 16:11 vader/mongo.py
--rw-r--r--  2.0 unx     1730 b- defN 23-Jun-19 16:11 vader/mongo_resource.py
--rw-r--r--  2.0 unx     2496 b- defN 23-Jun-19 16:11 vader/policy_service.py
--rw-r--r--  2.0 unx      515 b- defN 23-Jun-19 16:11 vader/project_resource.py
--rw-r--r--  2.0 unx     1063 b- defN 23-Jun-19 16:11 vader/raise_exception.py
--rw-r--r--  2.0 unx      522 b- defN 23-Jun-19 16:11 vader/vault_resource.py
--rw-r--r--  2.0 unx      204 b- defN 23-Jun-19 16:13 drizzutojr_vader-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 16:13 drizzutojr_vader-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-19 16:13 drizzutojr_vader-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1101 b- defN 23-Jun-19 16:13 drizzutojr_vader-0.0.3.dist-info/RECORD
-14 files, 11928 bytes uncompressed, 4451 bytes compressed:  62.7%
+Zip file size: 6234 bytes, number of entries: 14
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-19 21:45 vader/__init__.py
+-rw-r--r--  2.0 unx     1094 b- defN 23-Jun-19 21:45 vader/core_service.py
+-rw-r--r--  2.0 unx     1015 b- defN 23-Jun-19 21:45 vader/exceptions.py
+-rw-r--r--  2.0 unx     1425 b- defN 23-Jun-19 21:45 vader/general.py
+-rw-r--r--  2.0 unx      665 b- defN 23-Jun-19 21:45 vader/mongo.py
+-rw-r--r--  2.0 unx     1730 b- defN 23-Jun-19 21:45 vader/mongo_resource.py
+-rw-r--r--  2.0 unx     2496 b- defN 23-Jun-19 21:45 vader/policy_service.py
+-rw-r--r--  2.0 unx      524 b- defN 23-Jun-19 21:45 vader/project_resource.py
+-rw-r--r--  2.0 unx      929 b- defN 23-Jun-19 21:45 vader/raise_exception.py
+-rw-r--r--  2.0 unx      522 b- defN 23-Jun-19 21:45 vader/vault_resource.py
+-rw-r--r--  2.0 unx      204 b- defN 23-Jun-19 21:47 drizzutojr_vader-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 21:47 drizzutojr_vader-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-19 21:47 drizzutojr_vader-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1100 b- defN 23-Jun-19 21:47 drizzutojr_vader-0.0.4.dist-info/RECORD
+14 files, 11802 bytes uncompressed, 4410 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: vader/raise_exception.py
 Comment: 
 
 Filename: vader/vault_resource.py
 Comment: 
 
-Filename: drizzutojr_vader-0.0.3.dist-info/METADATA
+Filename: drizzutojr_vader-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: drizzutojr_vader-0.0.3.dist-info/WHEEL
+Filename: drizzutojr_vader-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: drizzutojr_vader-0.0.3.dist-info/top_level.txt
+Filename: drizzutojr_vader-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: drizzutojr_vader-0.0.3.dist-info/RECORD
+Filename: drizzutojr_vader-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vader/project_resource.py

```diff
@@ -1,8 +1,8 @@
-from .mongo import MongoResource
+from .mongo_resource import MongoResource
 from .general import generate_project_name
 
 
 class ProjectResource(MongoResource):
     def __init__(
         self, namespace, app_id, boundary_id, requestor, collection_name, request_data
     ):
```

## vader/raise_exception.py

```diff
@@ -7,17 +7,14 @@
 MAX_DESCRIPTION_LENGTH = 100
 
 
 def raise_exception_invalid_email(email: str):
     regex = r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b"
     if not re.fullmatch(regex, email):
         raise VaderConfigError(f"Email is not a valid email: {email}")
-    value = validate_email_exists_in_system(email)
-    if not value:
-        raise VaderConfigError(f"Email does not exist: {email}")
 
 
 def raise_exception_invalid_description(
     description: str,
     min_length: int = MIN_DESCRIPTION_LENGTH,
     max_length: int = MAX_DESCRIPTION_LENGTH,
 ):
```

## Comparing `drizzutojr_vader-0.0.3.dist-info/RECORD` & `drizzutojr_vader-0.0.4.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 vader/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vader/core_service.py,sha256=VzIyTc6GAxJUk7B6bO-nP6dHNTJkIpETdznHV1HTl0I,1094
 vader/exceptions.py,sha256=qMmVOiEvdBxZ_3c-EX2kI1QIRjm2QaN7zPD1_fcle_E,1015
 vader/general.py,sha256=qrb_VaFYcL9vJ_ne2skLMDKeoPf5uQXvwx4O8VdqdXs,1425
 vader/mongo.py,sha256=cqaO7YzxuDa8SKi2wiN0yeLY4sDr53SKg5r1cqaT5so,665
 vader/mongo_resource.py,sha256=HCCjE3OqPHwaAJ1afcTgP4Tx8vTMXfIfboIXf1S8bOI,1730
 vader/policy_service.py,sha256=YOZCDml0ja4l3n6I42mqH_CS4q8TJQstKNx5HrxHa-o,2496
-vader/project_resource.py,sha256=v5CGzYU0ptCXfgRzX5TCdAg7ozdu-vG0MVvDBPjeAcM,515
-vader/raise_exception.py,sha256=_zX6KQLkcqv7B3Mmj5AfKZTSCBduMw3YeVEl4MABUj4,1063
+vader/project_resource.py,sha256=OowzfDSKV5DcRPIvBORaFcH7NkboL3eJ_E5T0VFq2lI,524
+vader/raise_exception.py,sha256=7gT1f-F8HUTZbYZ10jJtq0XGh2mkIC-SFoHdAgWxP2k,929
 vader/vault_resource.py,sha256=ycKBx2NXoFpg5m1FxYWgD5NEz6vSDDF7YGBQVJbBC8c,522
-drizzutojr_vader-0.0.3.dist-info/METADATA,sha256=qt5xE2QLW9FVIfg0z0ZQoEX5Szw-UDTmWrF8cOI4j1c,204
-drizzutojr_vader-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-drizzutojr_vader-0.0.3.dist-info/top_level.txt,sha256=wEY-qHmChGsqPB_SEURS5ewt6uoSGcuQuRwmGxr1Sqw,6
-drizzutojr_vader-0.0.3.dist-info/RECORD,,
+drizzutojr_vader-0.0.4.dist-info/METADATA,sha256=eW_rsZwJCtuOeMZLvOGa_ui4UYvvdMAQTPntUJj83D8,204
+drizzutojr_vader-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+drizzutojr_vader-0.0.4.dist-info/top_level.txt,sha256=wEY-qHmChGsqPB_SEURS5ewt6uoSGcuQuRwmGxr1Sqw,6
+drizzutojr_vader-0.0.4.dist-info/RECORD,,
```

