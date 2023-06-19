# Comparing `tmp/htruc-1.0.6.tar.gz` & `tmp/htruc-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htruc-1.0.6.tar", last modified: Sun Jun 11 08:08:35 2023, max compression
+gzip compressed data, was "htruc-1.0.7.tar", last modified: Mon Jun 19 08:23:14 2023, max compression
```

## Comparing `htruc-1.0.6.tar` & `htruc-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-06-11 08:08:35.135407 htruc-1.0.6/
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2172 2023-06-11 08:08:35.135407 htruc-1.0.6/PKG-INFO
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1191 2023-06-11 08:04:36.000000 htruc-1.0.6/README.md
-drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-06-11 08:08:35.135407 htruc-1.0.6/htruc/
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        0 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/__init__.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)    11099 2023-06-11 08:07:33.000000 htruc-1.0.6/htruc/catalog.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     8928 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/cli.py
-drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-06-11 08:08:35.135407 htruc-1.0.6/htruc/repos/
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      118 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/repos/__init__.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      492 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/repos/_generic.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2517 2023-06-11 08:07:10.000000 htruc-1.0.6/htruc/repos/_github.py
-drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-06-11 08:08:35.135407 htruc-1.0.6/htruc/schemas/
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1220 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/schemas/__init__.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1021 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/schemas/upgrade_path.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      130 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/types.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1605 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/utils.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2875 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/validator.py
-drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-06-11 08:08:35.135407 htruc-1.0.6/htruc.egg-info/
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2172 2023-06-11 08:08:35.000000 htruc-1.0.6/htruc.egg-info/PKG-INFO
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      418 2023-06-11 08:08:35.000000 htruc-1.0.6/htruc.egg-info/SOURCES.txt
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        1 2023-06-11 08:08:35.000000 htruc-1.0.6/htruc.egg-info/dependency_links.txt
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       41 2023-06-11 08:08:35.000000 htruc-1.0.6/htruc.egg-info/entry_points.txt
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      150 2023-06-11 08:08:35.000000 htruc-1.0.6/htruc.egg-info/requires.txt
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        6 2023-06-11 08:08:35.000000 htruc-1.0.6/htruc.egg-info/top_level.txt
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       38 2023-06-11 08:08:35.135407 htruc-1.0.6/setup.cfg
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     3799 2023-06-11 08:08:20.000000 htruc-1.0.6/setup.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:23:14.347750 htruc-1.0.7/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    16725 2023-06-19 07:16:39.000000 htruc-1.0.7/LICENSE.md
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1874 2023-06-19 08:23:14.347750 htruc-1.0.7/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1191 2022-06-20 10:01:21.000000 htruc-1.0.7/README.md
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:23:14.347750 htruc-1.0.7/htruc/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-09-23 12:36:36.000000 htruc-1.0.7/htruc/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    11474 2023-06-19 07:36:30.000000 htruc-1.0.7/htruc/catalog.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     8939 2023-06-19 08:19:51.000000 htruc-1.0.7/htruc/cli.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:23:14.347750 htruc-1.0.7/htruc/repos/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      118 2022-06-21 08:16:17.000000 htruc-1.0.7/htruc/repos/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      492 2022-02-04 15:30:28.000000 htruc-1.0.7/htruc/repos/_generic.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2537 2023-06-19 07:58:45.000000 htruc-1.0.7/htruc/repos/_github.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:23:14.347750 htruc-1.0.7/htruc/schemas/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1220 2022-06-20 10:01:21.000000 htruc-1.0.7/htruc/schemas/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1021 2022-06-20 10:01:21.000000 htruc-1.0.7/htruc/schemas/upgrade_path.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      130 2022-06-20 10:01:21.000000 htruc-1.0.7/htruc/types.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2390 2023-06-19 08:19:31.000000 htruc-1.0.7/htruc/utils.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2882 2023-06-19 07:59:20.000000 htruc-1.0.7/htruc/validator.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:23:14.347750 htruc-1.0.7/htruc.egg-info/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1874 2023-06-19 08:23:14.000000 htruc-1.0.7/htruc.egg-info/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      429 2023-06-19 08:23:14.000000 htruc-1.0.7/htruc.egg-info/SOURCES.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2023-06-19 08:23:14.000000 htruc-1.0.7/htruc.egg-info/dependency_links.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       41 2023-06-19 08:23:14.000000 htruc-1.0.7/htruc.egg-info/entry_points.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      176 2023-06-19 08:23:14.000000 htruc-1.0.7/htruc.egg-info/requires.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        6 2023-06-19 08:23:14.000000 htruc-1.0.7/htruc.egg-info/top_level.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2023-06-19 08:23:14.347750 htruc-1.0.7/setup.cfg
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3799 2023-06-19 07:41:49.000000 htruc-1.0.7/setup.py
```

### Comparing `htruc-1.0.6/PKG-INFO` & `htruc-1.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 Metadata-Version: 2.1
 Name: htruc
-Version: 1.0.6
+Version: 1.0.7
 Summary: HTRUC, a toolkit for HTR-United cataloging
 Home-page: https://github.com/htr-united/htrvc
 Author: Thibault Clérice
 License: MIT
-Description: 
-        <img src="./img/HTRUC.png" width=300 align=right>
-        
-        HTRUC
-        =====
-        
-        [![Test](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml/badge.svg)](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml)
-        
-        
-        Pronunced `EuchTruc` (*ce truc*), this contains most of the tooling for the catalog records: 
-        - Parses catalog records
-        - Test the validity of the catalog according to different schemas
-        - Builds agglomerated catalog records with optional dataviz
-        - Retrieve catalog information from all repositories of a user or an organization.
-        
-        ## Install 
-        
-        Either clone and run `python setup.py install` **or** use the pip version `pip install htruc`
-        
-        ## Use
-        
-        ### Testing a catalog record
-        
-        Simply run `htruc test YourYamlFile.yml`
-        
-        ### Upgrade a previously existing catalog record
-        
-        Run `htruc upgrade yourYamlFile.yml`
-        
-        ### Upgrade a previously existing catalog record to the newest schema
-        
-        Run `htruc upgrade yourYamlFile.yml`
-        
-        ### Upgrade metrics using [HTR-United Metadata Generator (HUMg)](https://github.com/HTR-United/htr-united-metadata-generator)
-        
-        Run `htruc update-volumes YourYamlFile.yml MetricFileFromHUMG.jons --inplace`
-        ---
-        
-        Logo by [Alix Chagué](https://alix-tz.github.io).
-        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+
+<img src="./img/HTRUC.png" width=300 align=right>
+
+HTRUC
+=====
+
+[![Test](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml/badge.svg)](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml)
+
+
+Pronunced `EuchTruc` (*ce truc*), this contains most of the tooling for the catalog records: 
+- Parses catalog records
+- Test the validity of the catalog according to different schemas
+- Builds agglomerated catalog records with optional dataviz
+- Retrieve catalog information from all repositories of a user or an organization.
+
+## Install 
+
+Either clone and run `python setup.py install` **or** use the pip version `pip install htruc`
+
+## Use
+
+### Testing a catalog record
+
+Simply run `htruc test YourYamlFile.yml`
+
+### Upgrade a previously existing catalog record
+
+Run `htruc upgrade yourYamlFile.yml`
+
+### Upgrade a previously existing catalog record to the newest schema
+
+Run `htruc upgrade yourYamlFile.yml`
+
+### Upgrade metrics using [HTR-United Metadata Generator (HUMg)](https://github.com/HTR-United/htr-united-metadata-generator)
+
+Run `htruc update-volumes YourYamlFile.yml MetricFileFromHUMG.jons --inplace`
+---
+
+Logo by [Alix Chagué](https://alix-tz.github.io).
+
+
```

### Comparing `htruc-1.0.6/README.md` & `htruc-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `htruc-1.0.6/htruc/catalog.py` & `htruc-1.0.7/htruc/catalog.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,23 @@
                     logging.warning(f"Impossible to parse and understand {file}")
                     logger.info(str(E))
     if keep_valid_only:
         _clean_a_dict(out)
     return out
 
 
+def clever_catalog_update(catalog1: Dict, catalog2: Dict) -> Dict:
+    for repository in catalog2:
+        if repository in catalog1:
+            for key in ["characters", "volume"]:
+                if key in catalog2[repository]:
+                    catalog1[repository][key] = catalog2[repository][key]
+    return catalog1
+
+
 def get_all_catalogs(
     access_token: Optional[str] = None,
     local_directory: Optional[str] = None,
     get_distant: bool = True,
     organizations: Optional[Union[str, Iterable[str]]] = "htr-united",
     check_link: bool = False,
     ignore_orgs_gits: List[str] = None,
@@ -83,30 +92,31 @@
     :param check_link: If a local directory catalog record links to a github repository, scan the remote repository
         for any updates on the catalog
     :param ignore_orgs_gits: Ignore specific repositories in the scan
     :param keep_valid_only: Only Keeps valid catalog record
     :param auto_upgrade: Upgrade automatically all schemas to the latest version (Only applied if keep_valid_only is
         True)
     """
-    data = {}
+    data: Catalog = {}
     if local_directory:
         data.update(get_local_yaml(directory=local_directory, keep_valid_only=False))
         if check_link:
             for uri in data:
                 # We update the catalog if needs be by checking each repo
                 if "github.com" in uri:
                     print(f"Fetching {uri} remotely to update metrics")
                     results = get_github_repo_yaml(address=uri, access_token=access_token)
                     if results:
                         data[uri] = results
     if get_distant:
         if isinstance(organizations, str):
             organizations = (organizations, )
         for orga in organizations:
-            data.update(
+            data = clever_catalog_update(
+                data,
                 get_htr_united_repos(
                     access_token=access_token,
                     main_organization=orga,
                     exclude=ignore_orgs_gits
                 )
             )
     if keep_valid_only:
```

### Comparing `htruc-1.0.6/htruc/cli.py` & `htruc-1.0.7/htruc/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import sys
 import click
 import os.path
-import yaml
+from ruamel.yaml import YAML
 import json
 from typing import Optional, List
 
 from htruc.validator import run
 from htruc.catalog import get_all_catalogs, get_statistics, group_per_year, update_volume, _get_bibtex_and_apa
-from htruc.utils import parse_yaml, create_json_catalog, get_local_or_download
+from htruc.utils import parse_yaml, create_json_catalog, get_local_or_download, dump_yaml
 
 
 def _error(message):
     click.echo(
         click.style(message, fg="red"),
         color=True
     )
@@ -107,15 +107,15 @@
         ignore_orgs_gits=ignore_repo,
         keep_valid_only=clean,
         auto_upgrade=auto_upgrade,
         citation_cff=citation
     )
     click.echo(f"Dumping YAML output into {output}")
     with open(output, "w") as f:
-        yaml.dump(list(catalog.values()), f, sort_keys=False)
+        dump_yaml(list(catalog.values()), f)
 
     if json:
         click.echo(f"Dumping JSON output into {json}")
         from json import dump
         with open(json, "w") as f:
             dump(create_json_catalog(catalog, ids_files=ids), f)
     if graph or statistics or graph_csv:
@@ -182,15 +182,15 @@
 
     filename = f"{catalog_file.name}"
     if not inplace:
         filename = filename.split(".")
         filename = ".".join([*filename[:-1], "auto-update", filename[-1]])
     click.echo(f"Writing the update volumes in {filename}")
     with open(filename, "w") as f:
-        yaml.dump(record, f, sort_keys=False)
+        dump_yaml(record, f, sort_keys=False)
 
 
 @cli.command("upgrade")
 @click.argument("files", type=click.File(), nargs=-1)
 def upgrade(files):
     """ Upgrade [FILES] to the latest supported schema """
     for file in files:
@@ -199,12 +199,12 @@
         from htruc.schemas import recursive_update
         catalog, upgrade_order = recursive_update(catalog)
         if not upgrade_order:
             click.echo(click.style(f"--> No upgrade required", fg="yellow"))
             continue
         file.close()
         with open(file.name, "w") as f:
-            yaml.dump(catalog, f, sort_keys=False)
+            dump_yaml(catalog, f, sort_keys=False)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `htruc-1.0.6/htruc/repos/_github.py` & `htruc-1.0.7/htruc/repos/_github.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Dict, Any, Iterable
 import re
-import yaml
+from ruamel.yaml import YAML, parser
 from github import Github
 from github.GithubException import UnknownObjectException
 from htruc.utils import parse_yaml
 
 
 Catalog = Dict[str, Any]
 
@@ -26,15 +26,15 @@
     try:
         text = repo.get_contents("htr-united.yml").decoded_content.decode()
         print("--- Found htr-united.yml")
     except UnknownObjectException as e:
         return None
     try:
         return parse_yaml(text)
-    except yaml.parser.ParserError:
+    except parser.ParserError:
         print(f"Parse error on {user}/{repo_name}")
         if raise_on_parse_error:
             raise
         return None
 
 
 def get_github_repo_cff(
```

### Comparing `htruc-1.0.6/htruc/schemas/__init__.py` & `htruc-1.0.7/htruc/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.6/htruc/schemas/upgrade_path.py` & `htruc-1.0.7/htruc/schemas/upgrade_path.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.6/htruc/validator.py` & `htruc-1.0.7/htruc/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Iterable, List, TextIO, Dict, Any, Optional, Union
 from dataclasses import dataclass
 import json
 
 from jsonschema import Draft7Validator
-from yaml.parser import ParserError
+from ruamel.yaml.parser import ParserError
 
 from htruc.utils import parse_yaml, get_local_or_download
 
 
 @dataclass
 class Status:
     filename: str
```

### Comparing `htruc-1.0.6/htruc.egg-info/PKG-INFO` & `htruc-1.0.7/htruc.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 Metadata-Version: 2.1
 Name: htruc
-Version: 1.0.6
+Version: 1.0.7
 Summary: HTRUC, a toolkit for HTR-United cataloging
 Home-page: https://github.com/htr-united/htrvc
 Author: Thibault Clérice
 License: MIT
-Description: 
-        <img src="./img/HTRUC.png" width=300 align=right>
-        
-        HTRUC
-        =====
-        
-        [![Test](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml/badge.svg)](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml)
-        
-        
-        Pronunced `EuchTruc` (*ce truc*), this contains most of the tooling for the catalog records: 
-        - Parses catalog records
-        - Test the validity of the catalog according to different schemas
-        - Builds agglomerated catalog records with optional dataviz
-        - Retrieve catalog information from all repositories of a user or an organization.
-        
-        ## Install 
-        
-        Either clone and run `python setup.py install` **or** use the pip version `pip install htruc`
-        
-        ## Use
-        
-        ### Testing a catalog record
-        
-        Simply run `htruc test YourYamlFile.yml`
-        
-        ### Upgrade a previously existing catalog record
-        
-        Run `htruc upgrade yourYamlFile.yml`
-        
-        ### Upgrade a previously existing catalog record to the newest schema
-        
-        Run `htruc upgrade yourYamlFile.yml`
-        
-        ### Upgrade metrics using [HTR-United Metadata Generator (HUMg)](https://github.com/HTR-United/htr-united-metadata-generator)
-        
-        Run `htruc update-volumes YourYamlFile.yml MetricFileFromHUMG.jons --inplace`
-        ---
-        
-        Logo by [Alix Chagué](https://alix-tz.github.io).
-        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+
+<img src="./img/HTRUC.png" width=300 align=right>
+
+HTRUC
+=====
+
+[![Test](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml/badge.svg)](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml)
+
+
+Pronunced `EuchTruc` (*ce truc*), this contains most of the tooling for the catalog records: 
+- Parses catalog records
+- Test the validity of the catalog according to different schemas
+- Builds agglomerated catalog records with optional dataviz
+- Retrieve catalog information from all repositories of a user or an organization.
+
+## Install 
+
+Either clone and run `python setup.py install` **or** use the pip version `pip install htruc`
+
+## Use
+
+### Testing a catalog record
+
+Simply run `htruc test YourYamlFile.yml`
+
+### Upgrade a previously existing catalog record
+
+Run `htruc upgrade yourYamlFile.yml`
+
+### Upgrade a previously existing catalog record to the newest schema
+
+Run `htruc upgrade yourYamlFile.yml`
+
+### Upgrade metrics using [HTR-United Metadata Generator (HUMg)](https://github.com/HTR-United/htr-united-metadata-generator)
+
+Run `htruc update-volumes YourYamlFile.yml MetricFileFromHUMG.jons --inplace`
+---
+
+Logo by [Alix Chagué](https://alix-tz.github.io).
+
+
```

### Comparing `htruc-1.0.6/setup.py` & `htruc-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Package meta-data.
 NAME = 'htruc'
 DESCRIPTION = 'HTRUC, a toolkit for HTR-United cataloging'
 URL = 'https://github.com/htr-united/htrvc'
 AUTHOR = 'Thibault Clérice'
-REQUIRES_PYTHON = '>=3.7.0'
-VERSION = "1.0.6"
+REQUIRES_PYTHON = '>=3.8.0'
+VERSION = "1.0.7"
 
 # What packages are required for this module to be executed?
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     REQUIRED = f.read().splitlines()
 
 # What packages are optional?
```

