# Comparing `tmp/drizzutojr_vader-0.0.1-py3-none-any.whl.zip` & `tmp/drizzutojr_vader-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,16 @@
-Zip file size: 4772 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 02:31 vader/__init__.py
--rw-r--r--  2.0 unx     1127 b- defN 23-Jun-13 02:31 vader/common_exception_cases.py
--rw-r--r--  2.0 unx      947 b- defN 23-Jun-13 02:31 vader/core_service.py
--rw-r--r--  2.0 unx     1102 b- defN 23-Jun-13 02:31 vader/exceptions.py
--rw-r--r--  2.0 unx     1335 b- defN 23-Jun-13 02:31 vader/general.py
--rw-r--r--  2.0 unx      767 b- defN 23-Jun-13 02:31 vader/mongo.py
--rw-r--r--  2.0 unx     2538 b- defN 23-Jun-13 02:31 vader/policy_service.py
--rw-r--r--  2.0 unx      163 b- defN 23-Jun-13 02:32 drizzutojr_vader-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 02:32 drizzutojr_vader-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-13 02:32 drizzutojr_vader-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      867 b- defN 23-Jun-13 02:32 drizzutojr_vader-0.0.1.dist-info/RECORD
-11 files, 8944 bytes uncompressed, 3304 bytes compressed:  63.1%
+Zip file size: 6275 bytes, number of entries: 14
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-19 16:11 vader/__init__.py
+-rw-r--r--  2.0 unx     1094 b- defN 23-Jun-19 16:11 vader/core_service.py
+-rw-r--r--  2.0 unx     1015 b- defN 23-Jun-19 16:11 vader/exceptions.py
+-rw-r--r--  2.0 unx     1425 b- defN 23-Jun-19 16:11 vader/general.py
+-rw-r--r--  2.0 unx      665 b- defN 23-Jun-19 16:11 vader/mongo.py
+-rw-r--r--  2.0 unx     1730 b- defN 23-Jun-19 16:11 vader/mongo_resource.py
+-rw-r--r--  2.0 unx     2496 b- defN 23-Jun-19 16:11 vader/policy_service.py
+-rw-r--r--  2.0 unx      515 b- defN 23-Jun-19 16:11 vader/project_resource.py
+-rw-r--r--  2.0 unx     1063 b- defN 23-Jun-19 16:11 vader/raise_exception.py
+-rw-r--r--  2.0 unx      522 b- defN 23-Jun-19 16:11 vader/vault_resource.py
+-rw-r--r--  2.0 unx      204 b- defN 23-Jun-19 16:13 drizzutojr_vader-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 16:13 drizzutojr_vader-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-19 16:13 drizzutojr_vader-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1101 b- defN 23-Jun-19 16:13 drizzutojr_vader-0.0.3.dist-info/RECORD
+14 files, 11928 bytes uncompressed, 4451 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -1,34 +1,43 @@
 Filename: vader/__init__.py
 Comment: 
 
-Filename: vader/common_exception_cases.py
-Comment: 
-
 Filename: vader/core_service.py
 Comment: 
 
 Filename: vader/exceptions.py
 Comment: 
 
 Filename: vader/general.py
 Comment: 
 
 Filename: vader/mongo.py
 Comment: 
 
+Filename: vader/mongo_resource.py
+Comment: 
+
 Filename: vader/policy_service.py
 Comment: 
 
-Filename: drizzutojr_vader-0.0.1.dist-info/METADATA
+Filename: vader/project_resource.py
+Comment: 
+
+Filename: vader/raise_exception.py
+Comment: 
+
+Filename: vader/vault_resource.py
+Comment: 
+
+Filename: drizzutojr_vader-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: drizzutojr_vader-0.0.1.dist-info/WHEEL
+Filename: drizzutojr_vader-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: drizzutojr_vader-0.0.1.dist-info/top_level.txt
+Filename: drizzutojr_vader-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: drizzutojr_vader-0.0.1.dist-info/RECORD
+Filename: drizzutojr_vader-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vader/core_service.py

```diff
@@ -1,37 +1,41 @@
 import os
 import json
 import requests
 
 from .general import generate_project_name
-from .exceptions import VaderGeneralException
+from .exceptions import VaderGenericError
 
 SERVICE_URL = os.environ["CORE_SERVICE_URL"]
 
 
 def get_project(app_id, boundary_id):
     url = f"{SERVICE_URL}/{app_id}/{boundary_id}/project"
     response = requests.get(url)
 
     if response.status_code != 200:
         project_name = generate_project_name(app_id, boundary_id)
-        raise VaderGeneralException(
-            f"Could not fetch project {project_name}: {str(response.content)}"
+        raise VaderGenericError(
+            f"Could not fetch project {project_name}",
+            details={str(response.content)},
+            status_code=response.status_code,
         )
 
     return json.loads(response.content)
 
 
 def get_provisioner(name):
     url = f"{SERVICE_URL}/provisioner/{name}"
     response = requests.get(url)
 
     if response.status_code != 200:
-        raise VaderGeneralException(
-            f"Could not fetch provisioner {name}: {str(response.content)}"
+        raise VaderGenericError(
+            f"Could not fetch provisioner {name}: {str(response.content)}",
+            details={str(response.content)},
+            status_code=response.status_code,
         )
 
     return json.loads(response.content)
 
 
 def get_limit(app_id, boundary_id, limit_name):
     return {}
```

## vader/exceptions.py

```diff
@@ -1,37 +1,43 @@
+DEFAULT_STATUS_CODE = 400
+
+
 def vader_exception_handler(exception):
-    if type(exception.message) == dict:
-        exception.message["internal_code"] = exception.internal_code
-        return exception.message, exception.status_code
-    else:
-        return {
-            "message": str(exception.message),
-            "internal_code": exception.internal_code,
-        }, exception.status_code
+    return {
+        "message": str(exception.message),
+        "status": exception.status_code,
+        "details": exception.details,
+    }, exception.status_code
 
 
-class VaderCommonException(Exception):
-    def __init__(self, message, internal_code=None, status_code=400):
+class VaderCommonError(Exception):
+    def __init__(
+        self, message: str, details: str = "", status_code: int = DEFAULT_STATUS_CODE
+    ):
         self.message = message
-        self.internal_code = internal_code
+        self.details = details
         self.status_code = status_code
-        super().__init__()
+        super().__init__(self.message)
 
 
-class VaderConfigException(VaderCommonException):
+class VaderConfigError(VaderCommonError):
     """Bad Configuration passed to Vader"""
 
 
-class VaderUnauthorizedException(VaderCommonException):
+class VaderUnauthorizedError(VaderCommonError):
     """Unauthorized request to a project"""
 
 
-class VaderMongoException(VaderCommonException):
-    """Unauthorized request to a project"""
+class VaderMongoError(VaderCommonError):
+    """Error with Mongo"""
 
 
-class VaderVaultException(VaderCommonException):
-    """Unauthorized request to a project"""
+class VaderVaultError(VaderCommonError):
+    """Error with Vault"""
+
+
+class VaderNotFoundError(VaderCommonError):
+    """Resource not found in Vader"""
 
 
-class VaderGeneralException(VaderCommonException):
+class VaderGenericError(VaderCommonError):
     """Unauthorized request to a project"""
```

## vader/general.py

```diff
@@ -1,12 +1,13 @@
 import re
+import copy
 
 SPECIAL_CHARACTERS = "[-@!#$%^&*()<>?/\\\|}{~:]"
-
 BLACKLIST_KEYS = ["password", "token", "secret_id", "secret-id", "credential"]
+SANITIZE_VALUE = "SANITIZE"
 
 
 def contains_special_character(
     custom_string: str, special_characters: str = SPECIAL_CHARACTERS
 ):
     regex = re.compile(special_characters)
     if regex.search(custom_string):
@@ -27,17 +28,18 @@
 
 
 def generate_vault_policy_name(app_id, boundary_id, category, unique_name):
     return f"{app_id}-{boundary_id}-{category}-{unique_name}"
 
 
 def sanitize_dict(the_dict, whitelist_keys=[], blacklist_keys=[]):
+    the_dict = copy.deepcopy(the_dict)
     blacklist_keys = list(set(blacklist_keys + BLACKLIST_KEYS))
     blacklist_keys = list(filter(lambda x: x not in whitelist_keys, blacklist_keys))
 
     for key, value in the_dict.items():
         if isinstance(value, dict):
             the_dict[key] = sanitize_dict(value, whitelist_keys, blacklist_keys)
-        elif key in blacklist_keys:
-            the_dict[key] = "SANITIZE"
+        elif key.lower() in blacklist_keys:
+            the_dict[key] = SANITIZE_VALUE
 
     return the_dict
```

## vader/mongo.py

```diff
@@ -4,32 +4,24 @@
 MONGO_ADDRESS = os.environ["MONGO_ADDRESS"]
 MONGO_PORT = os.environ["MONGO_PORT"]
 MONGO_DB = os.environ["MONGO_DB"]
 MONGO_USER_PATH = os.environ["MONGO_USER_PATH"]
 MONGO_PASSWORD_PATH = os.environ["MONGO_PASSWORD_PATH"]
 
 
-def get_creds():
+def connect():
     user, password = None, None
     with open(MONGO_USER_PATH, "r") as f:
         user = f.read().strip()
 
     with open(MONGO_PASSWORD_PATH, "r") as f:
         password = f.read().strip()
 
-    return user, password
-
-
-def connect():
-    user, password = _get_creds()
-
     my_client = pymongo.MongoClient(
         host=MONGO_ADDRESS,
         port=int(MONGO_PORT),
         username=user,
         password=password,
         authSource=MONGO_DB,
     )
 
-    print(my_client)
-
     return my_client[MONGO_DB]
```

## vader/policy_service.py

```diff
@@ -1,13 +1,13 @@
 import os
 import requests
 import json
 
 from .general import generate_vault_policy_name
-from .exceptions import VaderGeneralException
+from .exceptions import VaderGenericError
 
 SERVICE_URL = os.environ["POLICY_SERVICE_URL"]
 
 
 def create_policy(
     namespace,
     app_id,
@@ -30,15 +30,15 @@
     url = f"{SERVICE_URL}/{app_id}/{boundary_id}/policy/{category}/{unique_name}"
     response = requests.post(url, headers=headers, json=data)
 
     if response.status_code != 200:
         policy_name = generate_vault_policy_name(
             app_id, boundary_id, category, unique_name
         )
-        raise VaderGeneralException(
+        raise VaderGenericError(
             f"Could not create policy {policy_name}: {str(response.conent)}"
         )
 
     return json.loads(response.content)
 
 
 def delete_policy(namespace, app_id, boundary_id, category, unique_name):
@@ -46,41 +46,39 @@
     headers = {"namespace": namespace}
     response = requests.delete(url, headers=headers)
 
     if response.status_code != 204:
         policy_name = generate_vault_policy_name(
             app_id, boundary_id, category, unique_name
         )
-        raise VaderGeneralException(
+        raise VaderGenericError(
             f"Could not delete policy {policy_name}: {str(response.conent)}"
         )
 
     return {}
 
 
 def get_policy_by_name(namespace, name):
     headers = {"namespace": namespace}
     url = f"{SERVICE_URL}/policy/{name}"
     response = requests.get(url)
 
     if response.status_code != 200:
-        raise VaderGeneralException(
-            f"Could not get policy {name}: {str(response.conent)}"
-        )
+        raise VaderGenericError(f"Could not get policy {name}: {str(response.conent)}")
 
     return json.loads(response.content)
 
 
 def get_policy_by_project(namespace, app_id, boundary_id, category, unique_name):
     headers = {"namespace": namespace}
     url = f"{SERVICE_URL}/{app_id}/{boundary_id}/policy/{category}/{unique_name}"
     response = requests.get(url, headers=headers)
 
     if response.status_code != 200:
         policy_name = generate_vault_policy_name(
             app_id, boundary_id, category, unique_name
         )
-        raise VaderGeneralException(
+        raise VaderGenericError(
             f"Could not get policy {policy_name}: {str(response.conent)}"
         )
 
     return json.loads(response.content)
```

## Comparing `vader/common_exception_cases.py` & `vader/raise_exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,32 +6,28 @@
 MIN_DESCRIPTION_LENGTH = 20
 MAX_DESCRIPTION_LENGTH = 100
 
 
 def raise_exception_invalid_email(email: str):
     regex = r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b"
     if not re.fullmatch(regex, email):
-        raise VaderConfigException(f"Email is not a valid email: {email}")
+        raise VaderConfigError(f"Email is not a valid email: {email}")
     value = validate_email_exists_in_system(email)
     if not value:
-        raise VaderConfigException(f"Email does not exist: {email}")
+        raise VaderConfigError(f"Email does not exist: {email}")
 
 
 def raise_exception_invalid_description(
     description: str,
     min_length: int = MIN_DESCRIPTION_LENGTH,
     max_length: int = MAX_DESCRIPTION_LENGTH,
 ):
     if len(description) < min_length:
-        raise VaderConfigException(
-            f"Description may not be under {min_length} characters"
-        )
+        raise VaderConfigError(f"Description may not be under {min_length} characters")
 
     if len(description) > max_length:
-        raise VaderConfigException(
-            f"Description may not be over {max_length} characters"
-        )
+        raise VaderConfigError(f"Description may not be over {max_length} characters")
 
 
 def raise_exception_invalid_version(version):
     if not semver.VersionInfo.is_valid(version):
-        raise VaderConfigException(f"Version number is not a valid version: {version}")
+        raise VaderConfigError(f"Version number is not a valid version: {version}")
```

## Comparing `drizzutojr_vader-0.0.1.dist-info/RECORD` & `drizzutojr_vader-0.0.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 vader/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-vader/common_exception_cases.py,sha256=KdahKU_VBw5WLMOuc6_rsw1aH8k_0XlWj2ThqNrsiEA,1127
-vader/core_service.py,sha256=k5d_KIi-9yvNY9JpLVkD37n9XJjd2AaHjd9yfzYpcIw,947
-vader/exceptions.py,sha256=Tm6ow-pQK2N7klTt3TDPBSEmxyC7MeHexCuQ_BhhzkU,1102
-vader/general.py,sha256=wtiIayRWqY__YlV3ILkb0vIz3MV1kHxRMM0mpL-CW6M,1335
-vader/mongo.py,sha256=-2IJCcz805eq3wey_C6LlS87kL3COvcynOQW79a6dJA,767
-vader/policy_service.py,sha256=iutF4Nnl6QWP_TNDnJD2xyGQbfgXfpwsFGt4LUhpZa4,2538
-drizzutojr_vader-0.0.1.dist-info/METADATA,sha256=s0moPIfVnLBz1QmfFKVr4WLIqiu0hsJ64YCFPx3Oi9k,163
-drizzutojr_vader-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-drizzutojr_vader-0.0.1.dist-info/top_level.txt,sha256=wEY-qHmChGsqPB_SEURS5ewt6uoSGcuQuRwmGxr1Sqw,6
-drizzutojr_vader-0.0.1.dist-info/RECORD,,
+vader/core_service.py,sha256=VzIyTc6GAxJUk7B6bO-nP6dHNTJkIpETdznHV1HTl0I,1094
+vader/exceptions.py,sha256=qMmVOiEvdBxZ_3c-EX2kI1QIRjm2QaN7zPD1_fcle_E,1015
+vader/general.py,sha256=qrb_VaFYcL9vJ_ne2skLMDKeoPf5uQXvwx4O8VdqdXs,1425
+vader/mongo.py,sha256=cqaO7YzxuDa8SKi2wiN0yeLY4sDr53SKg5r1cqaT5so,665
+vader/mongo_resource.py,sha256=HCCjE3OqPHwaAJ1afcTgP4Tx8vTMXfIfboIXf1S8bOI,1730
+vader/policy_service.py,sha256=YOZCDml0ja4l3n6I42mqH_CS4q8TJQstKNx5HrxHa-o,2496
+vader/project_resource.py,sha256=v5CGzYU0ptCXfgRzX5TCdAg7ozdu-vG0MVvDBPjeAcM,515
+vader/raise_exception.py,sha256=_zX6KQLkcqv7B3Mmj5AfKZTSCBduMw3YeVEl4MABUj4,1063
+vader/vault_resource.py,sha256=ycKBx2NXoFpg5m1FxYWgD5NEz6vSDDF7YGBQVJbBC8c,522
+drizzutojr_vader-0.0.3.dist-info/METADATA,sha256=qt5xE2QLW9FVIfg0z0ZQoEX5Szw-UDTmWrF8cOI4j1c,204
+drizzutojr_vader-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+drizzutojr_vader-0.0.3.dist-info/top_level.txt,sha256=wEY-qHmChGsqPB_SEURS5ewt6uoSGcuQuRwmGxr1Sqw,6
+drizzutojr_vader-0.0.3.dist-info/RECORD,,
```

