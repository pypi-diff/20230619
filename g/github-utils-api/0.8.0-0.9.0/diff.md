# Comparing `tmp/github-utils-api-0.8.0.tar.gz` & `tmp/github-utils-api-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github-utils-api-0.8.0.tar", last modified: Wed Feb 16 20:59:48 2022, max compression
+gzip compressed data, was "github-utils-api-0.9.0.tar", last modified: Sat Mar 12 22:53:52 2022, max compression
```

## Comparing `github-utils-api-0.8.0.tar` & `github-utils-api-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 20:59:48.153297 github-utils-api-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-02-16 20:59:36.000000 github-utils-api-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-02-16 20:59:48.153297 github-utils-api-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-02-16 20:59:36.000000 github-utils-api-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 20:59:48.149297 github-utils-api-0.8.0/github-utils-api/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 20:59:48.149297 github-utils-api-0.8.0/github-utils-api/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 20:59:48.153297 github-utils-api-0.8.0/github-utils-api/src/github_utils_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-02-16 20:59:48.000000 github-utils-api-0.8.0/github-utils-api/src/github_utils_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-02-16 20:59:48.000000 github-utils-api-0.8.0/github-utils-api/src/github_utils_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-16 20:59:48.000000 github-utils-api-0.8.0/github-utils-api/src/github_utils_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-16 20:59:48.000000 github-utils-api-0.8.0/github-utils-api/src/github_utils_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-02-16 20:59:48.000000 github-utils-api-0.8.0/github-utils-api/src/github_utils_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5669 2022-02-16 20:59:36.000000 github-utils-api-0.8.0/github-utils-api/src/githubutilsapi.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-16 20:59:48.153297 github-utils-api-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-02-16 20:59:47.000000 github-utils-api-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 22:53:52.602507 github-utils-api-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-03-12 22:53:39.000000 github-utils-api-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-03-12 22:53:52.602507 github-utils-api-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2022-03-12 22:53:39.000000 github-utils-api-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 22:53:52.602507 github-utils-api-0.9.0/github-utils-api/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 22:53:52.602507 github-utils-api-0.9.0/github-utils-api/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 22:53:52.602507 github-utils-api-0.9.0/github-utils-api/src/github_utils_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-03-12 22:53:52.000000 github-utils-api-0.9.0/github-utils-api/src/github_utils_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-03-12 22:53:52.000000 github-utils-api-0.9.0/github-utils-api/src/github_utils_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-12 22:53:52.000000 github-utils-api-0.9.0/github-utils-api/src/github_utils_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-03-12 22:53:52.000000 github-utils-api-0.9.0/github-utils-api/src/github_utils_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-12 22:53:52.000000 github-utils-api-0.9.0/github-utils-api/src/github_utils_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6844 2022-03-12 22:53:39.000000 github-utils-api-0.9.0/github-utils-api/src/githubutilsapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-12 22:53:52.602507 github-utils-api-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-03-12 22:53:52.000000 github-utils-api-0.9.0/setup.py
```

### Comparing `github-utils-api-0.8.0/LICENSE` & `github-utils-api-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `github-utils-api-0.8.0/PKG-INFO` & `github-utils-api-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-utils-api
-Version: 0.8.0
+Version: 0.9.0
 Summary: Small library to cover non provided methods by pygithub
 Home-page: UNKNOWN
 Author: Pablo Toledo
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `github-utils-api-0.8.0/README.md` & `github-utils-api-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `github-utils-api-0.8.0/github-utils-api/src/github_utils_api.egg-info/PKG-INFO` & `github-utils-api-0.9.0/github-utils-api/src/github_utils_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-utils-api
-Version: 0.8.0
+Version: 0.9.0
 Summary: Small library to cover non provided methods by pygithub
 Home-page: UNKNOWN
 Author: Pablo Toledo
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `github-utils-api-0.8.0/github-utils-api/src/githubutilsapi.py` & `github-utils-api-0.9.0/github-utils-api/src/githubutilsapi.py`

 * *Files 10% similar despite different names*

```diff
@@ -108,8 +108,31 @@
         :param organization_name: string; name of the current organization created at github
         :param team_slug_name: string; Github Team slug name
         :param github_username: string; Github Username
         :return: request
         '''
         params = {}
         url = self.github_url + "/orgs/" + organization_name + "/teams/" + team_slug_name + "/memberships/" + github_username
-        return self.__request("DELETE", url, params)
+        return self.__request("DELETE", url, params)
+
+    def list_repositories(self, organization_name=None, type="all", sort="created", per_page=100, page=1):
+        '''
+        This method allows to list all repositories in a GitHub organization
+        According API docs: https://docs.github.com/es/rest/reference/repos#list-organization-repositories
+        :param organization_name: string; name of the current organization created at github
+        :param type: Specifies the types of repositories you want returned. Can be one of all, public, private, forks, sources, member, internal. Default: all
+        :param sort: Can be one of created, updated, pushed, full_name. Default: created
+        :param per_page: Results per page (max 100). Default: 100
+        :param page: Page number of the results to fetch. Default: 1
+        :return: request
+        '''
+        params = {}
+        if type:
+            params['type'] = type
+        if sort:
+            params['sort'] = sort
+        if per_page:
+            params['per_page'] = per_page
+        if page:
+            params['page'] = page
+        url = self.github_url + "/orgs/" + organization_name + "/repos"
+        return self.__request("GET", url, params)
```

### Comparing `github-utils-api-0.8.0/setup.py` & `github-utils-api-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="github-utils-api",                 # This is the name of the package
-    version='0.8.0',
+    version='0.9.0',
     author="Pablo Toledo",                  # Full name of the author
     description="Small library to cover non provided methods by pygithub",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

