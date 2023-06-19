# Comparing `tmp/igz_mgmt-0.0.7.tar.gz` & `tmp/igz_mgmt-0.0.8.tar.gz`

## Comparing `igz_mgmt-0.0.7.tar` & `igz_mgmt-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/__init__.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/__version__.py
--rw-r--r--   0        0        0    16097 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/client.py
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/constants.py
--rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/cruds.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/exceptions.py
--rw-r--r--   0        0        0    10302 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/operations.py
--rw-r--r--   0        0        0    47741 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/resources.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/common/__init__.py
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/common/helpers.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/logger/__init__.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/logger/logger.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/schemas/__init__.py
--rw-r--r--   0        0        0    11993 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/schemas/app_services.py
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/schemas/manual_events.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/LICENSE
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/README.md
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/__init__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/__version__.py
+-rw-r--r--   0        0        0    16269 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/client.py
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/constants.py
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/cruds.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/exceptions.py
+-rw-r--r--   0        0        0    10302 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/operations.py
+-rw-r--r--   0        0        0    47741 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/resources.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/common/__init__.py
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/common/helpers.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/logger/__init__.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/logger/logger.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/schemas/__init__.py
+-rw-r--r--   0        0        0    11993 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/schemas/app_services.py
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/schemas/manual_events.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/LICENSE
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/README.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/PKG-INFO
```

### Comparing `igz_mgmt-0.0.7/igz_mgmt/__init__.py` & `igz_mgmt-0.0.8/igz_mgmt/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.7/igz_mgmt/__version__.py` & `igz_mgmt-0.0.8/igz_mgmt/__version__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # limitations under the License.
 #
 
 # version can be either one of the following:
 # x.y.z
 # x.y.z.rcN
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
```

### Comparing `igz_mgmt-0.0.7/igz_mgmt/client.py` & `igz_mgmt-0.0.8/igz_mgmt/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,16 +173,17 @@
         if password and not username or access_key and not username:
             raise ValueError(
                 "Must provide username when providing password or access key"
             )
 
         self._logger = igz_mgmt.get_or_create_logger(level="INFO", name="apic")
 
-        # TODO: type of Session
-        self._session_obj: typing.Optional[dict] = None
+        # enriched once authenticated
+        self._tenant_id: typing.Optional[str] = None
+
         self._client = _BaseHTTPClient(
             self._logger,
             igz_mgmt.common.helpers.get_endpoint(endpoint, default_scheme="https"),
             timeout=timeout,
             retries=retries,
         )
 
@@ -368,15 +369,14 @@
                     "username": username,
                     "password": password,
                     "plane": igz_mgmt.constants.SessionPlanes.control.value,
                 },
             ),
         )
         self._set_auth(username=username, session=response.cookies.get("session"))
-        self._session_obj = response.json().get("data", {})
 
     def _set_auth(self, username: str, access_key: str = "", session: str = ""):
         if access_key and session:
             raise ValueError("Cannot set both access_key and session")
         self._client._cookies.set(
             "session",
             f'j:{{"sid": "{access_key}"}}' if access_key else session,
@@ -386,15 +386,17 @@
             encoded_auth = f"{username}:{access_key}"
             base64_encoded_auth = base64.b64encode(encoded_auth.encode("utf-8")).decode(
                 "utf-8"
             )
             self._client._headers[
                 igz_mgmt.constants._RequestHeaders.authorization_header
             ] = f"Basic {base64_encoded_auth}"
+
         self._version = self._get_external_versions()
+        self._enrich_tenant_id()
 
     def _try_resolve_external_version(self, node):
         try:
             # get external version via tunnel
             response = self._client.get(
                 "/tunnel/{0}.version.0/external_versions/{0}".format(node),
                 "Failed to get external version from node {0}".format(node),
@@ -419,29 +421,34 @@
         self._logger.info(
             "Failed to resolve auto detect iguazio external version, use `client.version = x.y.z` for explicitness"
         )
 
         # oldest supported GA version
         return self.__DEFAULT_EXTERNAL_VERSION_NUMBER
 
+    def _enrich_tenant_id(self):
+        response = self.request("POST", "/sessions/verifications/planes/any/internal")
+        self._tenant_id = (
+            response.get("data", {})
+            .get("attributes", {})
+            .get("context", {})
+            .get("authentication", {})
+            .get("tenant_id")
+        )
+
     @property
     def tenant_id(self) -> str:
-        """Resolves the tenant id from session.
+        """Authenticated session tenant id.
 
         Returns:
             tenant id
         """
         if not self._authenticated:
             raise RuntimeError("Must .login() first")
-        return (
-            self._session_obj.get("relationships", {})
-            .get("tenant", {})
-            .get("data", {})
-            .get("id")
-        )
+        return self._tenant_id
 
     @property
     def version(self) -> semver.VersionInfo:
         """Iguazio system version info.
 
         Returns:
             semver.VersionInfo: Iguazio version
```

### Comparing `igz_mgmt-0.0.7/igz_mgmt/constants.py` & `igz_mgmt-0.0.8/igz_mgmt/constants.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.7/igz_mgmt/cruds.py` & `igz_mgmt-0.0.8/igz_mgmt/cruds.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.7/igz_mgmt/exceptions.py` & `igz_mgmt-0.0.8/igz_mgmt/exceptions.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.7/igz_mgmt/operations.py` & `igz_mgmt-0.0.8/igz_mgmt/operations.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.7/igz_mgmt/resources.py` & `igz_mgmt-0.0.8/igz_mgmt/resources.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.7/igz_mgmt/common/__init__.py` & `igz_mgmt-0.0.8/igz_mgmt/common/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.7/igz_mgmt/common/helpers.py` & `igz_mgmt-0.0.8/igz_mgmt/common/helpers.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.7/igz_mgmt/logger/__init__.py` & `igz_mgmt-0.0.8/igz_mgmt/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.7/igz_mgmt/logger/logger.py` & `igz_mgmt-0.0.8/igz_mgmt/logger/logger.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.7/igz_mgmt/schemas/__init__.py` & `igz_mgmt-0.0.8/igz_mgmt/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.7/igz_mgmt/schemas/app_services.py` & `igz_mgmt-0.0.8/igz_mgmt/schemas/app_services.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.7/igz_mgmt/schemas/manual_events.py` & `igz_mgmt-0.0.8/igz_mgmt/schemas/manual_events.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.7/LICENSE` & `igz_mgmt-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.7/pyproject.toml` & `igz_mgmt-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.7/PKG-INFO` & `igz_mgmt-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igz-mgmt
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python SDK For Iguazio Management API
 Project-URL: Homepage, https://github.com/iguazio/igz-mgmt-sdk
 Author-email: Iguazio Platform Team <liranb@iguazio.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

