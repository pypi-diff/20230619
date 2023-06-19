# Comparing `tmp/qctrl_client-7.0.0.tar.gz` & `tmp/qctrl_client-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_client-7.0.0.tar", max compression
+gzip compressed data, was "qctrl_client-7.0.1.tar", max compression
```

## Comparing `qctrl_client-7.0.0.tar` & `qctrl_client-7.0.1.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0    36653 2023-05-01 06:27:49.675506 qctrl_client-7.0.0/LICENSE
--rw-r--r--   0        0        0      214 2023-05-01 06:27:49.675506 qctrl_client-7.0.0/README.md
--rw-r--r--   0        0        0     2614 2023-05-01 06:28:12.876545 qctrl_client-7.0.0/pyproject.toml
--rw-r--r--   0        0        0      747 2023-05-01 06:28:12.892546 qctrl_client-7.0.0/qctrlclient/__init__.py
--rw-r--r--   0        0        0      686 2023-05-01 06:28:12.888546 qctrl_client-7.0.0/qctrlclient/auth/__init__.py
--rw-r--r--   0        0        0     1831 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/base.py
--rw-r--r--   0        0        0     5885 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/cli.py
--rw-r--r--   0        0        0      972 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/helpers.py
--rw-r--r--   0        0        0     1042 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/keycloak.py
--rw-r--r--   0        0        0     4308 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/oidc.py
--rw-r--r--   0        0        0     1801 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/password.py
--rw-r--r--   0        0        0     3096 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/redirect_listener.py
--rw-r--r--   0        0        0     1516 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/service_account.py
--rw-r--r--   0        0        0     7742 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/client.py
--rw-r--r--   0        0        0      809 2023-05-01 06:28:12.892546 qctrl_client-7.0.0/qctrlclient/core/__init__.py
--rw-r--r--   0        0        0     2999 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/core/functions.py
--rw-r--r--   0        0        0      995 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/core/products.py
--rw-r--r--   0        0        0      638 2023-05-01 06:28:12.896546 qctrl_client-7.0.0/qctrlclient/core/router/__init__.py
--rw-r--r--   0        0        0    11628 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/core/router/api.py
--rw-r--r--   0        0        0     1189 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/core/router/base.py
--rw-r--r--   0        0        0     1197 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/core/router/local.py
--rw-r--r--   0        0        0     2677 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/core/settings.py
--rw-r--r--   0        0        0     1154 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/core/utils.py
--rw-r--r--   0        0        0     1329 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/defaults.py
--rw-r--r--   0        0        0     2172 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/exceptions.py
--rw-r--r--   0        0        0     1357 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/globals.py
--rw-r--r--   0        0        0     1424 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/pytest_plugin.py
--rw-r--r--   0        0        0      601 2023-05-01 06:28:12.888546 qctrl_client-7.0.0/qctrlclient/transports/__init__.py
--rw-r--r--   0        0        0     4625 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/transports/requests_transport.py
--rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 qctrl_client-7.0.0/setup.py
--rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 qctrl_client-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/LICENSE
+-rw-r--r--   0        0        0      214 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/README.md
+-rw-r--r--   0        0        0     2614 2023-06-19 04:54:10.237695 qctrl_client-7.0.1/pyproject.toml
+-rw-r--r--   0        0        0      747 2023-06-19 04:54:10.245695 qctrl_client-7.0.1/qctrlclient/__init__.py
+-rw-r--r--   0        0        0      686 2023-06-19 04:54:10.253695 qctrl_client-7.0.1/qctrlclient/auth/__init__.py
+-rw-r--r--   0        0        0     1831 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/qctrlclient/auth/base.py
+-rw-r--r--   0        0        0     4969 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/qctrlclient/auth/cli.py
+-rw-r--r--   0        0        0      972 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/qctrlclient/auth/helpers.py
+-rw-r--r--   0        0        0     1042 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/qctrlclient/auth/keycloak.py
+-rw-r--r--   0        0        0     4308 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/qctrlclient/auth/oidc.py
+-rw-r--r--   0        0        0     1801 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/qctrlclient/auth/password.py
+-rw-r--r--   0        0        0     3096 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/qctrlclient/auth/redirect_listener.py
+-rw-r--r--   0        0        0     1516 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/qctrlclient/auth/service_account.py
+-rw-r--r--   0        0        0     7742 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/qctrlclient/client.py
+-rw-r--r--   0        0        0      809 2023-06-19 04:54:10.249695 qctrl_client-7.0.1/qctrlclient/core/__init__.py
+-rw-r--r--   0        0        0     2999 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/qctrlclient/core/functions.py
+-rw-r--r--   0        0        0      995 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/qctrlclient/core/products.py
+-rw-r--r--   0        0        0      638 2023-06-19 04:54:10.249695 qctrl_client-7.0.1/qctrlclient/core/router/__init__.py
+-rw-r--r--   0        0        0    11628 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/qctrlclient/core/router/api.py
+-rw-r--r--   0        0        0     1189 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/qctrlclient/core/router/base.py
+-rw-r--r--   0        0        0     1197 2023-06-19 04:53:50.833501 qctrl_client-7.0.1/qctrlclient/core/router/local.py
+-rw-r--r--   0        0        0     2677 2023-06-19 04:53:50.837501 qctrl_client-7.0.1/qctrlclient/core/settings.py
+-rw-r--r--   0        0        0     1179 2023-06-19 04:53:50.837501 qctrl_client-7.0.1/qctrlclient/core/utils.py
+-rw-r--r--   0        0        0     1329 2023-06-19 04:53:50.837501 qctrl_client-7.0.1/qctrlclient/defaults.py
+-rw-r--r--   0        0        0     2172 2023-06-19 04:53:50.837501 qctrl_client-7.0.1/qctrlclient/exceptions.py
+-rw-r--r--   0        0        0     1357 2023-06-19 04:53:50.837501 qctrl_client-7.0.1/qctrlclient/globals.py
+-rw-r--r--   0        0        0     1424 2023-06-19 04:53:50.837501 qctrl_client-7.0.1/qctrlclient/pytest_plugin.py
+-rw-r--r--   0        0        0      601 2023-06-19 04:54:10.253695 qctrl_client-7.0.1/qctrlclient/transports/__init__.py
+-rw-r--r--   0        0        0     4625 2023-06-19 04:53:50.837501 qctrl_client-7.0.1/qctrlclient/transports/requests_transport.py
+-rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 qctrl_client-7.0.1/PKG-INFO
```

### Comparing `qctrl_client-7.0.0/LICENSE` & `qctrl_client-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/pyproject.toml` & `qctrl_client-7.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-client"
-version = "7.0.0"
+version = "7.0.1"
 description = "Q-CTRL Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
```

### Comparing `qctrl_client-7.0.0/qctrlclient/__init__.py` & `qctrl_client-7.0.1/qctrlclient/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/auth/__init__.py` & `qctrl_client-7.0.1/qctrlclient/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/auth/base.py` & `qctrl_client-7.0.1/qctrlclient/auth/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/auth/cli.py` & `qctrl_client-7.0.1/qctrlclient/auth/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         self._redirect_uri = (
             redirect_uri or f"http://localhost:{self._redirect_uri_port}"
         )
 
         super().__init__()
 
         try:
-            self._authenticate_if_needed()
+            self._get_access_token()
         except InvalidGrantError as exc:
             LOGGER.error("%s", exc, exc_info=True)
             self._authenticate()
 
     def _get_urls(self):
         return get_keycloak_oidc_urls(self._base_url)
 
@@ -141,42 +141,14 @@
         complete_login(
             self._redirect_uri_port,
             authorization_url,
             self._fetch_token_from_authorization_response,
         )
         print("Successful authentication!")
 
-    def _authenticate_if_needed(self):
-        """
-        Verify if the `access_token` is still valid or can be refreshed, if not
-        starts the `authenticate` flow.
-        """
-
-        # if token already exists
-        if self._oidc_session.access_token:
-
-            # if token expires soon, try to refresh
-            if self._expires_soon(self._oidc_session.access_token):
-                try:
-                    self._oidc_session.refresh_token(self._urls.token_url)
-
-                # unable to refresh, need to re-authenticate
-                except Warning:  # TODO review how this gets thrown
-                    self._authenticate()
-
-                # no refresh url, need to re-authenticate
-                else:
-                    self._authenticate()
-
-        # no token, need to authenticate
-        else:
-            self._authenticate()
-
-        return self._oidc_session.access_token
-
     def _fetch_token_from_authorization_response(self, authorization_response):
         """
         Fetch token from authorization response and save it if `token_updater`
         is present.
         """
         print("Finalizing authentication...")
         self._oidc_session.fetch_token(
```

### Comparing `qctrl_client-7.0.0/qctrlclient/auth/helpers.py` & `qctrl_client-7.0.1/qctrlclient/auth/helpers.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/auth/keycloak.py` & `qctrl_client-7.0.1/qctrlclient/auth/keycloak.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/auth/oidc.py` & `qctrl_client-7.0.1/qctrlclient/auth/oidc.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/auth/password.py` & `qctrl_client-7.0.1/qctrlclient/auth/password.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/auth/redirect_listener.py` & `qctrl_client-7.0.1/qctrlclient/auth/redirect_listener.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/auth/service_account.py` & `qctrl_client-7.0.1/qctrlclient/auth/service_account.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/client.py` & `qctrl_client-7.0.1/qctrlclient/client.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/core/__init__.py` & `qctrl_client-7.0.1/qctrlclient/core/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/core/functions.py` & `qctrl_client-7.0.1/qctrlclient/core/functions.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/core/products.py` & `qctrl_client-7.0.1/qctrlclient/core/products.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/core/router/__init__.py` & `qctrl_client-7.0.1/qctrlclient/core/router/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/core/router/api.py` & `qctrl_client-7.0.1/qctrlclient/core/router/api.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/core/router/base.py` & `qctrl_client-7.0.1/qctrlclient/core/router/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/core/router/local.py` & `qctrl_client-7.0.1/qctrlclient/core/router/local.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/core/settings.py` & `qctrl_client-7.0.1/qctrlclient/core/settings.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/core/utils.py` & `qctrl_client-7.0.1/qctrlclient/core/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,31 +8,34 @@
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 import sys
+from importlib.metadata import (
+    PackageNotFoundError,
+    version,
+)
 from typing import Optional
 
 import click
-import pkg_resources
 
 
 def get_installed_version(package: str) -> Optional[str]:
     """Get the installed version of the package. If
     the version cannot be found (e.g. package not installed)
     then None is returned.
     """
     try:
-        version = pkg_resources.get_distribution(package).version
+        pkg_version = version(package)
 
-    except pkg_resources.ResolutionError:
-        version = None
+    except PackageNotFoundError:
+        pkg_version = None
 
-    return version
+    return pkg_version
 
 
 def show_error_message(error_message: str):
     """Displays the error message and stops execution."""
     click.echo(error_message, err=True)
     sys.exit(1)
```

### Comparing `qctrl_client-7.0.0/qctrlclient/defaults.py` & `qctrl_client-7.0.1/qctrlclient/defaults.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/exceptions.py` & `qctrl_client-7.0.1/qctrlclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/globals.py` & `qctrl_client-7.0.1/qctrlclient/globals.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/pytest_plugin.py` & `qctrl_client-7.0.1/qctrlclient/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/transports/__init__.py` & `qctrl_client-7.0.1/qctrlclient/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/qctrlclient/transports/requests_transport.py` & `qctrl_client-7.0.1/qctrlclient/transports/requests_transport.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.0.0/PKG-INFO` & `qctrl_client-7.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-client
-Version: 7.0.0
+Version: 7.0.1
 Summary: Q-CTRL Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
```

