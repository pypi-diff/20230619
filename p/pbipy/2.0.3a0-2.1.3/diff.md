# Comparing `tmp/pbipy-2.0.3a0.tar.gz` & `tmp/pbipy-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbipy-2.0.3a0.tar", last modified: Sun Jun 18 05:31:15 2023, max compression
+gzip compressed data, was "pbipy-2.1.3.tar", last modified: Mon Jun 19 05:49:13 2023, max compression
```

## Comparing `pbipy-2.0.3a0.tar` & `pbipy-2.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 05:31:15.364409 pbipy-2.0.3a0/
--rw-rw-rw-   0        0        0    11523 2022-10-28 08:16:15.000000 pbipy-2.0.3a0/LICENSE
--rw-rw-rw-   0        0        0     8991 2023-06-18 05:31:15.363410 pbipy-2.0.3a0/PKG-INFO
--rw-rw-rw-   0        0        0     8205 2023-06-18 05:21:13.000000 pbipy-2.0.3a0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 05:31:15.355410 pbipy-2.0.3a0/pbipy/
--rw-rw-rw-   0        0        0       29 2022-10-28 07:52:32.000000 pbipy-2.0.3a0/pbipy/__init__.py
--rw-rw-rw-   0        0        0      341 2023-06-18 05:25:30.000000 pbipy-2.0.3a0/pbipy/__version__.py
--rw-rw-rw-   0        0        0     4240 2023-06-18 05:21:13.000000 pbipy-2.0.3a0/pbipy/powerbi.py
--rw-rw-rw-   0        0        0    20774 2023-06-18 05:21:13.000000 pbipy-2.0.3a0/pbipy/resources.py
--rw-rw-rw-   0        0        0      110 2023-06-18 05:21:13.000000 pbipy-2.0.3a0/pbipy/settings.py
--rw-rw-rw-   0        0        0    10220 2023-06-18 05:21:13.000000 pbipy-2.0.3a0/pbipy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-18 05:31:15.362409 pbipy-2.0.3a0/pbipy.egg-info/
--rw-rw-rw-   0        0        0     8991 2023-06-18 05:31:15.000000 pbipy-2.0.3a0/pbipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-06-18 05:31:15.000000 pbipy-2.0.3a0/pbipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 05:31:15.000000 pbipy-2.0.3a0/pbipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-18 05:31:15.000000 pbipy-2.0.3a0/pbipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-18 05:31:15.000000 pbipy-2.0.3a0/pbipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 05:31:15.364409 pbipy-2.0.3a0/setup.cfg
--rw-rw-rw-   0        0        0     3594 2022-12-05 03:27:44.000000 pbipy-2.0.3a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:49:13.549757 pbipy-2.1.3/
+-rw-rw-rw-   0        0        0    11523 2022-10-28 08:16:15.000000 pbipy-2.1.3/LICENSE
+-rw-rw-rw-   0        0        0    10195 2023-06-19 05:49:13.548762 pbipy-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9411 2023-06-19 05:21:11.000000 pbipy-2.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 05:49:13.536758 pbipy-2.1.3/pbipy/
+-rw-rw-rw-   0        0        0       29 2022-10-28 07:52:32.000000 pbipy-2.1.3/pbipy/__init__.py
+-rw-rw-rw-   0        0        0      335 2023-06-19 05:22:36.000000 pbipy-2.1.3/pbipy/__version__.py
+-rw-rw-rw-   0        0        0     7848 2023-06-19 04:55:25.000000 pbipy-2.1.3/pbipy/powerbi.py
+-rw-rw-rw-   0        0        0    26494 2023-06-19 05:06:21.000000 pbipy-2.1.3/pbipy/resources.py
+-rw-rw-rw-   0        0        0      110 2023-06-18 05:21:13.000000 pbipy-2.1.3/pbipy/settings.py
+-rw-rw-rw-   0        0        0    10236 2023-06-19 04:16:26.000000 pbipy-2.1.3/pbipy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:49:13.546756 pbipy-2.1.3/pbipy.egg-info/
+-rw-rw-rw-   0        0        0    10195 2023-06-19 05:49:13.000000 pbipy-2.1.3/pbipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-06-19 05:49:13.000000 pbipy-2.1.3/pbipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 05:49:13.000000 pbipy-2.1.3/pbipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-19 05:49:13.000000 pbipy-2.1.3/pbipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 05:49:13.000000 pbipy-2.1.3/pbipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 05:49:13.549757 pbipy-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     3594 2022-12-05 03:27:44.000000 pbipy-2.1.3/setup.py
```

### Comparing `pbipy-2.0.3a0/LICENSE` & `pbipy-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pbipy-2.0.3a0/PKG-INFO` & `pbipy-2.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbipy
-Version: 2.0.3a0
+Version: 2.1.3
 Summary: A Python Library for interacting with the Power BI Rest API.
 Home-page: https://github.com/andrewvillazon/pbipy
 Author: Andrew Villazon
 Author-email: andrew.villazon@gmail.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -106,14 +106,28 @@
 print(type(sales))
 print(hasattr(sales, "configured_by"))
 
 # <class 'pbipy.resources.Dataset'>
 # True
 ```
 
+Most methods take in an object id...
+
+```python
+dataset = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229", group="a2f89923-421a-464e-bf4c-25eab39bb09f")
+```
+
+... or just pass in the object itself.
+
+```python
+group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
+
+dataset = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229", group=group)
+```
+
 If you need to access the raw json representation, this is supported to.
 
 ```python
 sales = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 
 print(sales.raw)
 
@@ -135,15 +149,15 @@
 ```python
 sales = pbi.dataset(id="cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 print(sales)
 
 # <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
 ```
 
-#### Get a list of Datasets in a Group (aka Workspace)
+#### Get a list of Datasets in a Workspace (Group)
 
 ```python
 datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
 
 for dataset in datasets:
     print(dataset)
 
@@ -194,30 +208,68 @@
 #               "MyTable[Year]": 2010,
 #               "MyTable[Quarter]": "Q1"
 #             },
 # ...
 # }
 ```
 
+### Workspaces (Groups) *
+
+*\* In the Power BI Rest API, workspaces are referred to as "groups".*
+
+#### List Workspaces
+
+```python
+groups = pbi.groups()
+
+for group in groups:
+    print(group)
+
+# <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
+# <Group id='3d9b93c6-7b6d-4801-a491-1738910904fd', name='marketing'>
+```
+
+#### Create a Workspace
+
+```python
+group = pbi.create_group("contoso")
+print(group)
+
+# <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
+```
+
+#### Users and their access
+
+```python
+group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
+users = group.users()
+
+for user in users:
+    print(user)
+
+# {"identifier": "john@contoso.com", "groupUserAccessRight": "Admin", ... }
+# {"identifier": "Adam@contoso.com", "groupUserAccessRight": "Member", ... }
+```
+
 ## Power BI Rest API Operations
 
 `pbipy` methods wrap around the Operations described in the Power BI Rest API Reference:
 
 [Power BI REST APIs for embedded analytics and automation - Power BI REST API](https://learn.microsoft.com/en-us/rest/api/power-bi/)
 
 
 ## Development Progress
 
 `pbipy` is in the early stages of development so expect a few features to be missing. The aim is to cover off most of the core stuff like Datasets, Workspaces (Groups), Reports, Apps, etc., and the rest later on. Check back regularly to see what's been added or still in the pipeline.
 
 | PowerBI Component   	| Progress 	| Notes 	|
 |---------------------	|----------	|-------	|
 | Datasets            	| Done     	|       	|
-| Groups (Workspaces) 	| Doing    	|       	|
-| Reports             	| Next     	|       	|
+| Groups (Workspaces) 	| Done    	|       	|
+| Reports             	| Doing     |       	|
 | Apps                	| Todo     	|       	|
 | Dataflows           	| Todo     	|       	|
 | Dashboards          	| Todo     	|       	|
 | Everything else     	| Backlog  	|       	|
 
 ## Contributing
 
@@ -229,15 +281,15 @@
 
 Pull requests are the best way to make a contribution to the code:
 
 1. Fork the repo and create your branch from master.
 2. If you've added code that should be tested, add tests.
 3. Add docstrings.
 4. Ensure the test suite passes.
-5. Format your code (`pbipy` uses [black](https://github.com/psf/black).
+5. Format your code (`pbipy` uses [black](https://github.com/psf/black)).
 6. Issue that pull request!
 
 ### Reporting a bug
 
 Great Bug Reports tend to have:
 
 * A quick summary and/or background
```

### Comparing `pbipy-2.0.3a0/README.md` & `pbipy-2.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -86,14 +86,28 @@
 print(type(sales))
 print(hasattr(sales, "configured_by"))
 
 # <class 'pbipy.resources.Dataset'>
 # True
 ```
 
+Most methods take in an object id...
+
+```python
+dataset = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229", group="a2f89923-421a-464e-bf4c-25eab39bb09f")
+```
+
+... or just pass in the object itself.
+
+```python
+group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
+
+dataset = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229", group=group)
+```
+
 If you need to access the raw json representation, this is supported to.
 
 ```python
 sales = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 
 print(sales.raw)
 
@@ -115,15 +129,15 @@
 ```python
 sales = pbi.dataset(id="cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 print(sales)
 
 # <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
 ```
 
-#### Get a list of Datasets in a Group (aka Workspace)
+#### Get a list of Datasets in a Workspace (Group)
 
 ```python
 datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
 
 for dataset in datasets:
     print(dataset)
 
@@ -174,30 +188,68 @@
 #               "MyTable[Year]": 2010,
 #               "MyTable[Quarter]": "Q1"
 #             },
 # ...
 # }
 ```
 
+### Workspaces (Groups) *
+
+*\* In the Power BI Rest API, workspaces are referred to as "groups".*
+
+#### List Workspaces
+
+```python
+groups = pbi.groups()
+
+for group in groups:
+    print(group)
+
+# <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
+# <Group id='3d9b93c6-7b6d-4801-a491-1738910904fd', name='marketing'>
+```
+
+#### Create a Workspace
+
+```python
+group = pbi.create_group("contoso")
+print(group)
+
+# <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
+```
+
+#### Users and their access
+
+```python
+group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
+users = group.users()
+
+for user in users:
+    print(user)
+
+# {"identifier": "john@contoso.com", "groupUserAccessRight": "Admin", ... }
+# {"identifier": "Adam@contoso.com", "groupUserAccessRight": "Member", ... }
+```
+
 ## Power BI Rest API Operations
 
 `pbipy` methods wrap around the Operations described in the Power BI Rest API Reference:
 
 [Power BI REST APIs for embedded analytics and automation - Power BI REST API](https://learn.microsoft.com/en-us/rest/api/power-bi/)
 
 
 ## Development Progress
 
 `pbipy` is in the early stages of development so expect a few features to be missing. The aim is to cover off most of the core stuff like Datasets, Workspaces (Groups), Reports, Apps, etc., and the rest later on. Check back regularly to see what's been added or still in the pipeline.
 
 | PowerBI Component   	| Progress 	| Notes 	|
 |---------------------	|----------	|-------	|
 | Datasets            	| Done     	|       	|
-| Groups (Workspaces) 	| Doing    	|       	|
-| Reports             	| Next     	|       	|
+| Groups (Workspaces) 	| Done    	|       	|
+| Reports             	| Doing     |       	|
 | Apps                	| Todo     	|       	|
 | Dataflows           	| Todo     	|       	|
 | Dashboards          	| Todo     	|       	|
 | Everything else     	| Backlog  	|       	|
 
 ## Contributing
 
@@ -209,15 +261,15 @@
 
 Pull requests are the best way to make a contribution to the code:
 
 1. Fork the repo and create your branch from master.
 2. If you've added code that should be tested, add tests.
 3. Add docstrings.
 4. Ensure the test suite passes.
-5. Format your code (`pbipy` uses [black](https://github.com/psf/black).
+5. Format your code (`pbipy` uses [black](https://github.com/psf/black)).
 6. Issue that pull request!
 
 ### Reporting a bug
 
 Great Bug Reports tend to have:
 
 * A quick summary and/or background
```

### Comparing `pbipy-2.0.3a0/pbipy/resources.py` & `pbipy-2.1.3/pbipy/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,26 @@
+from requests import Session
+
 from pbipy import settings
 from pbipy.utils import RequestsMixin, remove_no_values, to_snake_case
 
 
 class Resource(RequestsMixin):
     BASE_URL = settings.BASE_URL
 
-    def __init__(self, session, **kwargs) -> None:
+    def __init__(
+        self,
+        id: str,
+        session: Session,
+        **kwargs,
+    ) -> None:
+        self.id = id
         self.session = session
         self.raw = None
 
-        if "group_id" in kwargs:
-            group_id = kwargs.get("group_id")
-            setattr(self, "group_id", group_id)
-
-        if self.group_id:
-            self.group_path = f"/groups/{self.group_id}"
-        else:
-            self.group_path = ""
-
-        self._base_path = f"{self.BASE_URL}{self.group_path}"
-
     def __repr__(
         self,
     ) -> str:
         """
         Provide a readable representation of the class. Looks to the class'
         `self._REPR` to determine what to show.
 
@@ -64,24 +61,32 @@
         "group_id",
         "configured_by",
         "created_date",
     ]
 
     def __init__(
         self,
-        id,
-        session,
+        id: str,
+        session: Session,
         group_id=None,
         raw=None,
     ) -> None:
-        self.id = id
+        super().__init__(id, session)
 
-        super().__init__(session, group_id=group_id)
+        if group_id:
+            self.group_id = group_id
+        else:
+            self.group_id = None
+
+        if self.group_id:
+            self.resource_path = f"/groups/{self.group_id}/datasets/{self.id}"
+        else:
+            self.resource_path = f"/datasets/{self.id}"
 
-        self.base_path = f"{self._base_path}/datasets/{self.id}"
+        self.base_path = f"{self.BASE_URL}{self.resource_path}"
 
         # Supports creating from a list of js, e.g., get_datasets endpoint
         if raw:
             self._load_from_raw(raw)
 
     def add_user(
         self,
@@ -666,7 +671,193 @@
         `list[dict]`
             List of principals, e.g., Users, Groups, with access to the
             dataset.
         """
 
         resource = self.base_path + "/users"
         return self.get_raw(resource, self.session)
+
+
+class Group(Resource):
+    _REPR = [
+        "id",
+        "name",
+    ]
+
+    def __init__(
+        self,
+        id: str,
+        session: Session,
+        raw=None,
+        **kwargs,
+    ) -> None:
+        super().__init__(id, session, **kwargs)
+
+        self.base_path = f"{self.BASE_URL}/groups/{self.id}"
+
+        if raw:
+            self._load_from_raw(raw)
+
+    def add_user(
+        self,
+        identifier: str,
+        principal_type: str,
+        access_right: str,
+        display_name: str = None,
+        email_address: str = None,
+        graph_id: str = None,
+        profile: dict = None,
+        user_type: str = None,
+    ) -> None:
+        """
+        Grants the specified user the specified permissions to the workspace.
+
+        Parameters
+        ----------
+        `identifier` : `str`
+            Identifier of the principal.
+        `principal_type` : `str`
+            The principal type, e.g., "App", "Group", "None", or "User".
+        `access_right` : `str`
+            The access right (permission level) that a user has on the
+            workspace, e.g., "Admin", "Contributor", "Member", "None",
+            or "Viewer".
+        `display_name` : `str`, optional
+            Display name of the principal.
+        `email_address` : `str`, optional
+            Email address of the user.
+        `graph_id` : `str`, optional
+            Identifier of the principal in Microsoft Graph. Only available
+            for admin APIs.
+        `profile` : `dict`, optional
+            A Power BI service principal profile. Only relevant for Power
+            BI Embedded multi-tenancy solution.
+        `user_type` : `str`, optional
+            Type of the user.
+        """
+
+        payload = {
+            "identifier": identifier,
+            "groupUserAccessRight": access_right,
+            "principalType": principal_type,
+            "displayName": display_name,
+            "emailAddress": email_address,
+            "graphId": graph_id,
+            "profile": profile,
+            "userType": user_type,
+        }
+
+        prepared_payload = remove_no_values(payload)
+        resource = self.base_path + "/users"
+
+        self.post(resource, self.session, prepared_payload)
+
+    def delete_user(
+        self,
+        user: str,
+        profile: str = None,
+    ) -> None:
+        """
+        Deletes the specified user permissions from the specified workspace.
+
+        Parameters
+        ----------
+        `user` : `str`
+            The email address of the user or object ID of the service principal
+            to delete.
+        `profile` : `str`, optional
+            The service principal profile ID to delete.
+        """
+
+        if profile:
+            resource = self.base_path + f"/users/{user}?profileId={profile}"
+        else:
+            resource = self.base_path + f"/users/{user}"
+
+        self.delete(resource, self.session)
+
+    def update_user(
+        self,
+        identifier: str,
+        principal_type: str,
+        access_right: str,
+        display_name: str = None,
+        email_address: str = None,
+        graph_id: str = None,
+        profile: dict = None,
+        user_type: str = None,
+    ) -> None:
+        """
+        Updates the specified user permissions on the workspace.
+
+        Parameters
+        ----------
+        `identifier` : `str`
+            Identifier of the principal.
+        `principal_type` : `str`
+            The principal type, e.g., "App", "Group", "None", or "User".
+        `access_right` : `str`
+            The access right (permission level) that a user has on the
+            workspace, e.g., "Admin", "Contributor", "Member", "None",
+            or "Viewer".
+        `display_name` : `str`, optional
+            Display name of the principal.
+        `email_address` : `str`, optional
+            Email address of the user.
+        `graph_id` : `str`, optional
+            Identifier of the principal in Microsoft Graph. Only available
+            for admin APIs.
+        `profile` : `dict`, optional
+            A Power BI service principal profile. Only relevant for Power
+            BI Embedded multi-tenancy solution.
+        `user_type` : `str`, optional
+            Type of the user.
+        """
+
+        payload = {
+            "identifier": identifier,
+            "groupUserAccessRight": access_right,
+            "principalType": principal_type,
+            "displayName": display_name,
+            "emailAddress": email_address,
+            "graphId": graph_id,
+            "profile": profile,
+            "userType": user_type,
+        }
+
+        prepared_payload = remove_no_values(payload)
+        resource = self.base_path + "/users"
+
+        self.put(resource, self.session, prepared_payload)
+
+    def users(
+        self,
+        skip: int = None,
+        top: int = None,
+    ) -> list[dict]:
+        """
+        Returns a list of users that have access to the workspace.
+
+        Parameters
+        ----------
+        `skip` : `int`, optional
+            Skips the first n results.
+        `top` : `int`, optional
+            Returns onl the first n results.
+
+        Returns
+        -------
+        `list[dict]`
+            List of users that have access to the workspace.
+        """
+
+        params = {
+            "$skip": skip,
+            "$top": top,
+        }
+
+        prepared_params = remove_no_values(params)
+        resource = self.base_path + "/users"
+
+        raw = self.get_raw(resource, self.session, params=prepared_params)
+
+        return raw
```

### Comparing `pbipy-2.0.3a0/pbipy/utils.py` & `pbipy-2.1.3/pbipy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,15 @@
             If encountered error with the request.
         """
 
         try:
             response = self.post(resource, session, payload, **kwargs)
             raw = response.json()
 
-            return raw
+            return self.parse_raw(raw)
 
         except Exception as e:
             raise e
 
     def put(
         self,
         resource: str,
```

### Comparing `pbipy-2.0.3a0/pbipy.egg-info/PKG-INFO` & `pbipy-2.1.3/pbipy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbipy
-Version: 2.0.3a0
+Version: 2.1.3
 Summary: A Python Library for interacting with the Power BI Rest API.
 Home-page: https://github.com/andrewvillazon/pbipy
 Author: Andrew Villazon
 Author-email: andrew.villazon@gmail.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -106,14 +106,28 @@
 print(type(sales))
 print(hasattr(sales, "configured_by"))
 
 # <class 'pbipy.resources.Dataset'>
 # True
 ```
 
+Most methods take in an object id...
+
+```python
+dataset = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229", group="a2f89923-421a-464e-bf4c-25eab39bb09f")
+```
+
+... or just pass in the object itself.
+
+```python
+group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
+
+dataset = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229", group=group)
+```
+
 If you need to access the raw json representation, this is supported to.
 
 ```python
 sales = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 
 print(sales.raw)
 
@@ -135,15 +149,15 @@
 ```python
 sales = pbi.dataset(id="cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 print(sales)
 
 # <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
 ```
 
-#### Get a list of Datasets in a Group (aka Workspace)
+#### Get a list of Datasets in a Workspace (Group)
 
 ```python
 datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
 
 for dataset in datasets:
     print(dataset)
 
@@ -194,30 +208,68 @@
 #               "MyTable[Year]": 2010,
 #               "MyTable[Quarter]": "Q1"
 #             },
 # ...
 # }
 ```
 
+### Workspaces (Groups) *
+
+*\* In the Power BI Rest API, workspaces are referred to as "groups".*
+
+#### List Workspaces
+
+```python
+groups = pbi.groups()
+
+for group in groups:
+    print(group)
+
+# <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
+# <Group id='3d9b93c6-7b6d-4801-a491-1738910904fd', name='marketing'>
+```
+
+#### Create a Workspace
+
+```python
+group = pbi.create_group("contoso")
+print(group)
+
+# <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
+```
+
+#### Users and their access
+
+```python
+group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
+users = group.users()
+
+for user in users:
+    print(user)
+
+# {"identifier": "john@contoso.com", "groupUserAccessRight": "Admin", ... }
+# {"identifier": "Adam@contoso.com", "groupUserAccessRight": "Member", ... }
+```
+
 ## Power BI Rest API Operations
 
 `pbipy` methods wrap around the Operations described in the Power BI Rest API Reference:
 
 [Power BI REST APIs for embedded analytics and automation - Power BI REST API](https://learn.microsoft.com/en-us/rest/api/power-bi/)
 
 
 ## Development Progress
 
 `pbipy` is in the early stages of development so expect a few features to be missing. The aim is to cover off most of the core stuff like Datasets, Workspaces (Groups), Reports, Apps, etc., and the rest later on. Check back regularly to see what's been added or still in the pipeline.
 
 | PowerBI Component   	| Progress 	| Notes 	|
 |---------------------	|----------	|-------	|
 | Datasets            	| Done     	|       	|
-| Groups (Workspaces) 	| Doing    	|       	|
-| Reports             	| Next     	|       	|
+| Groups (Workspaces) 	| Done    	|       	|
+| Reports             	| Doing     |       	|
 | Apps                	| Todo     	|       	|
 | Dataflows           	| Todo     	|       	|
 | Dashboards          	| Todo     	|       	|
 | Everything else     	| Backlog  	|       	|
 
 ## Contributing
 
@@ -229,15 +281,15 @@
 
 Pull requests are the best way to make a contribution to the code:
 
 1. Fork the repo and create your branch from master.
 2. If you've added code that should be tested, add tests.
 3. Add docstrings.
 4. Ensure the test suite passes.
-5. Format your code (`pbipy` uses [black](https://github.com/psf/black).
+5. Format your code (`pbipy` uses [black](https://github.com/psf/black)).
 6. Issue that pull request!
 
 ### Reporting a bug
 
 Great Bug Reports tend to have:
 
 * A quick summary and/or background
```

### Comparing `pbipy-2.0.3a0/setup.py` & `pbipy-2.1.3/setup.py`

 * *Files identical despite different names*

