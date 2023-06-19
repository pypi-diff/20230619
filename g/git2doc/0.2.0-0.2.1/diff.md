# Comparing `tmp/git2doc-0.2.0.tar.gz` & `tmp/git2doc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2doc-0.2.0.tar", last modified: Sat Jun 17 20:03:55 2023, max compression
+gzip compressed data, was "git2doc-0.2.1.tar", last modified: Mon Jun 19 12:53:56 2023, max compression
```

## Comparing `git2doc-0.2.0.tar` & `git2doc-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 20:03:55.027524 git2doc-0.2.0/
--rw-rw-rw-   0        0        0     3025 2023-06-17 20:03:55.026485 git2doc-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2356 2023-06-17 19:48:08.000000 git2doc-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 20:03:54.976636 git2doc-0.2.0/git2doc/
--rw-rw-rw-   0        0        0        0 2023-06-09 14:25:12.000000 git2doc-0.2.0/git2doc/__init__.py
--rw-rw-rw-   0        0        0     7727 2023-06-17 00:03:27.000000 git2doc-0.2.0/git2doc/loader.py
-drwxrwxrwx   0        0        0        0 2023-06-17 20:03:55.023489 git2doc-0.2.0/git2doc.egg-info/
--rw-rw-rw-   0        0        0     3025 2023-06-17 20:03:54.000000 git2doc-0.2.0/git2doc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-06-17 20:03:54.000000 git2doc-0.2.0/git2doc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 20:03:54.000000 git2doc-0.2.0/git2doc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-17 20:03:54.000000 git2doc-0.2.0/git2doc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-17 20:03:54.000000 git2doc-0.2.0/git2doc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 20:03:55.028486 git2doc-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      983 2023-06-17 20:02:55.000000 git2doc-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:53:56.852321 git2doc-0.2.1/
+-rw-rw-rw-   0        0        0     3025 2023-06-19 12:53:56.850814 git2doc-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2356 2023-06-19 12:51:41.000000 git2doc-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 12:53:56.838128 git2doc-0.2.1/git2doc/
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:51:41.000000 git2doc-0.2.1/git2doc/__init__.py
+-rw-rw-rw-   0        0        0     9322 2023-06-19 12:52:26.000000 git2doc-0.2.1/git2doc/loader.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:53:56.848832 git2doc-0.2.1/git2doc.egg-info/
+-rw-rw-rw-   0        0        0     3025 2023-06-19 12:53:56.000000 git2doc-0.2.1/git2doc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-06-19 12:53:56.000000 git2doc-0.2.1/git2doc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 12:53:56.000000 git2doc-0.2.1/git2doc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-19 12:53:56.000000 git2doc-0.2.1/git2doc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 12:53:56.000000 git2doc-0.2.1/git2doc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 12:53:56.853328 git2doc-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      983 2023-06-19 12:53:22.000000 git2doc-0.2.1/setup.py
```

### Comparing `git2doc-0.2.0/PKG-INFO` & `git2doc-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2doc
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool for converting git repositories into documents
 Home-page: https://github.com/voynow/git2doc
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `git2doc-0.2.0/README.md` & `git2doc-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `git2doc-0.2.0/git2doc/loader.py` & `git2doc-0.2.1/git2doc/loader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import concurrent.futures
 from datetime import datetime, timedelta
 import dotenv
 import gc
 from git import Blob, Repo
+from git.exc import InvalidGitRepositoryError
 import os
 from pathlib import Path
 import requests
 import shutil
 import stat
 from typing import Callable, List, Optional, Dict
 
@@ -19,16 +20,23 @@
     ".yml",
     ".json",
     ".png",
     ".jpg",
     ".jpeg",
     ".gif",
     ".svg",
-    "csv",
+    ".csv",
     ".txt",
+    ".jsonl",
+    ".struct",
+    ".map",
+    ".obj",
+    ".cleaned",
+    ".dict",
+    ".GIF",
 ]
 REPODATA_FOLDER = "./repodata/"
 
 
 def load_file(item, output_path) -> Optional[Document]:
     """
     Loads a single file from the repository.
@@ -99,15 +107,20 @@
     :return: Repo object
     """
     if os.path.exists(output_path):
         repo = Repo(output_path)
         origin = repo.remote(name="origin")
         origin.pull()
     else:
-        repo = Repo.clone_from(clone_url, output_path)
+        repo = Repo.clone_from(
+            clone_url,
+            output_path,
+            allow_unsafe_options=True,
+            multi_options=["--config", "lfs.fetchexclude=*"],
+        )
         repo.git.checkout(branch)
     return repo
 
 
 def docs_to_str(repo_data):
     """Convert repo data to raw text"""
     raw_repo = ""
@@ -136,15 +149,14 @@
     output_path = f"{REPODATA_FOLDER}{folder_name}/"
 
     # git pull, load, and delete repo
     repo = git_pull(repo, branch, output_path)
     repo_docs = load_concurrently(repo, output_path)
 
     if delete:
-
         shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
 
     return repo_docs
 
 
 def flatten_dict(dd, separator="_", prefix=""):
     """
@@ -201,65 +213,106 @@
         "Authorization": f"Bearer {access_token}",
     }
 
     query = f"language:{language}" if language else "is:public"
     date_since = (datetime.now() - timedelta(days=last_n_days)).strftime("%Y-%m-%d")
     query += f" created:>{date_since}"
 
-    params = {"q": query, "sort": sort, "order": order, "per_page": n_repos}
+    repos = []
+    page = 1
+    while len(repos) < n_repos:
+        params = {
+            "q": query,
+            "sort": sort,
+            "order": order,
+            "per_page": 100,
+            "page": page,
+        }
 
-    with requests.Session() as session:
-        session.headers.update(headers)
+        with requests.Session() as session:
+            session.headers.update(headers)
+            try:
+                response = session.get(url, params=params)
+                response.raise_for_status()
+                data = response.json()
+                repos.extend(data.get("items", []))
+            except requests.exceptions.HTTPError as errh:
+                print(f"HTTP Error: {errh}")
+            except requests.exceptions.ConnectionError as errc:
+                print(f"Error Connecting: {errc}")
+            except requests.exceptions.Timeout as errt:
+                print(f"Timeout Error: {errt}")
+            except requests.exceptions.RequestException as err:
+                print(f"Unknown Error: {err}")
+                break
+
+        # Increment the page number for the next iteration
+        page += 1
+
+    # Return only the number of repositories requested
+    return repos[:n_repos]
+
+
+def pull_code_helper(repo_key, branch, delete, max_retries=3):
+    """rmtree and retry on intermittent errors"""
+    retries = 0
+    while retries < max_retries:
         try:
-            response = session.get(url, params=params)
-            response.raise_for_status()
-        except requests.exceptions.HTTPError as errh:
-            print(f"HTTP Error: {errh}")
-        except requests.exceptions.ConnectionError as errc:
-            print(f"Error Connecting: {errc}")
-        except requests.exceptions.Timeout as errt:
-            print(f"Timeout Error: {errt}")
-        except requests.exceptions.RequestException as err:
-            print(f"Unknown Error: {err}")
+            data = pull_code_from_repo(repo_key, branch=branch, delete=delete)
+            return data
+        except InvalidGitRepositoryError:
+            print(f"Error with {repo_key}, retrying... ({retries + 1}/{max_retries})")
+            shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
+            retries += 1
 
-    return response.json()
+    print(
+        f"Failed to pull data from {repo_key} after {max_retries} attempts. Skipping..."
+    )
+    return None
 
 
 def pipeline_fetch_and_load(
     n_repos: int,
     last_n_days: int,
     language: str = None,
     sort: str = "stars",
     order: str = "desc",
     delete: bool = False,
 ) -> Dict[str, Dict]:
-    
     # remove any old repos
     if os.path.exists(REPODATA_FOLDER):
         shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
 
     response = get_top_repos(
         n_repos=n_repos,
         last_n_days=last_n_days,
         language=language,
         sort=sort,
         order=order,
     )
 
     github_data = {}
-    for repo in response["items"]:
-        if repo["size"]:
-            repo_key = repo["html_url"]
-            github_data[repo_key] = repo
-
-            # docs attribute stored wtih metadata
-            print(f"Processing {repo_key}...")
-            github_data[repo_key]["docs"] = pull_code_from_repo(
-                repo_key, branch=repo["default_branch"], delete=delete
+    for i, repo_metadata in enumerate(response):
+        repo_key = repo_metadata["html_url"]
+
+        if repo_metadata["size"]:
+            print(f"({i}) Processing {repo_key}...")
+
+            github_data[repo_key] = {}
+            github_data[repo_key]["metadata"] = repo_metadata
+
+            response = pull_code_helper(
+                repo_key,
+                branch=repo_metadata["default_branch"],
+                delete=delete,
             )
+            if response:
+                github_data[repo_key]["docs"] = response
+            else:
+                del github_data[repo_key]
         else:
-            print(f"Skipping {repo['html_url']} as it is empty")
+            print(f"Skipping {repo_key} as it is empty")
 
     # clean up repo data
     shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
 
     return github_data
```

### Comparing `git2doc-0.2.0/git2doc.egg-info/PKG-INFO` & `git2doc-0.2.1/git2doc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2doc
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool for converting git repositories into documents
 Home-page: https://github.com/voynow/git2doc
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `git2doc-0.2.0/setup.py` & `git2doc-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='git2doc',
-    version='0.2.0',
+    version='0.2.1',
     description='A tool for converting git repositories into documents',
     author='Jamie Voynow',
     author_email='voynow99@gmail.com',
     url='https://github.com/voynow/git2doc',
     packages=find_packages(),
     install_requires=[
         'langchain',
```

