# Comparing `tmp/drizzutojr_vapi-0.0.3-py3-none-any.whl.zip` & `tmp/drizzutojr_vapi-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3986 bytes, number of entries: 8
--rw-r--r--  2.0 unx       49 b- defN 23-Jun-18 21:46 vapi/__init__.py
--rw-r--r--  2.0 unx     1107 b- defN 23-Jun-18 21:46 vapi/exceptions.py
--rw-r--r--  2.0 unx     5449 b- defN 23-Jun-18 21:46 vapi/vapi.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jun-18 21:48 drizzutojr_vapi-0.0.3.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      200 b- defN 23-Jun-18 21:48 drizzutojr_vapi-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-18 21:48 drizzutojr_vapi-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-18 21:48 drizzutojr_vapi-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      642 b- defN 23-Jun-18 21:48 drizzutojr_vapi-0.0.3.dist-info/RECORD
-8 files, 8605 bytes uncompressed, 2860 bytes compressed:  66.8%
+Zip file size: 4036 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-18 22:29 vapi/__init__.py
+-rw-r--r--  2.0 unx     1164 b- defN 23-Jun-18 22:29 vapi/exceptions.py
+-rw-r--r--  2.0 unx     5798 b- defN 23-Jun-18 22:29 vapi/vapi.py
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jun-18 22:31 drizzutojr_vapi-0.0.4.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      200 b- defN 23-Jun-18 22:31 drizzutojr_vapi-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-18 22:31 drizzutojr_vapi-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-18 22:31 drizzutojr_vapi-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      642 b- defN 23-Jun-18 22:31 drizzutojr_vapi-0.0.4.dist-info/RECORD
+8 files, 9011 bytes uncompressed, 2910 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: vapi/exceptions.py
 Comment: 
 
 Filename: vapi/vapi.py
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.3.dist-info/LICENSE.md
+Filename: drizzutojr_vapi-0.0.4.dist-info/LICENSE.md
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.3.dist-info/METADATA
+Filename: drizzutojr_vapi-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.3.dist-info/WHEEL
+Filename: drizzutojr_vapi-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.3.dist-info/top_level.txt
+Filename: drizzutojr_vapi-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.3.dist-info/RECORD
+Filename: drizzutojr_vapi-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vapi/exceptions.py

```diff
@@ -26,16 +26,20 @@
         self.message = message
         self.errors = errors
         self.status_code = status_code
         super().__init__(self.message)
 
 
 class VAPIPermissionDeniedError(VAPIVaultError):
-    """Vault returned permission denied"""
+    """Vault returned 403"""
+
+
+class VAPIPathError(VAPIVaultError):
+    """Vault returned 404"""
 
 
 class VAPISealedError(VAPIVaultError):
-    """Vault is sealed"""
+    """Vault returned 503"""
 
 
 class VAPIAcceptedStatusCodeError(VAPIVaultError):
     """The Status Code returned from Vault does match the accepted status codes set by the user"""
```

## vapi/vapi.py

```diff
@@ -75,31 +75,36 @@
                 else:
                     return json_response
             except ValueError:
                 return {}
         else:
             if response.status_code == 403:
                 raise VAPIPermissionDeniedError(
-                    f"Vault returned 403 for path {self.current_path}",
+                    f"Vault returned 403 for path {self.current_path} indicating permission issues",
+                    response.status_code,
+                    errors=response.json()["errors"],
+                )
+            if response.status_code == 404:
+                raise VAPIPathError(
+                    f"Vault returned 404 for path {self.current_path} indicating an issue with the path",
                     response.status_code,
                     errors=response.json()["errors"],
                 )
             if response.status_code == 503:
                 raise VAPISealedError(
                     f"Vault returned 503 for path {self.current_path} and is likely sealed",
                     response.status_code,
                     errors=response.json()["errors"],
                 )
             if response.status_code in [200, 204]:
                 raise VAPIAcceptedStatusCodeError(
                     f"Vault Response Status Code {response.status_code} for path {self.current_path} not in Accepted Range {', '.join(item) for item in accepted_status_codes}",
                     response.status_code,
                 )
-
-            raise VAPIGenericError(response.text)
+            raise VAPIVaultError(response.text, response.status_code)
 
         try:
             return response.json()
         except ValueError:
             return {}
 
     def token_lookup(self, raw=False, accepted_status_codes=[204, 200]):
```

## Comparing `drizzutojr_vapi-0.0.3.dist-info/LICENSE.md` & `drizzutojr_vapi-0.0.4.dist-info/LICENSE.md`

 * *Files identical despite different names*

