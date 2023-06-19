# Comparing `tmp/skt-0.2.89.tar.gz` & `tmp/skt-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skt-0.2.89.tar", last modified: Mon Jun 19 08:00:58 2023, max compression
+gzip compressed data, was "dist/skt-0.2.9.tar", last modified: Wed Aug 12 04:38:26 2020, max compression
```

## Comparing `skt-0.2.89.tar` & `skt-0.2.9.tar`

### file list

```diff
@@ -1,32 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 08:00:58.629227 skt-0.2.89/
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-06-19 08:00:51.000000 skt-0.2.89/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    10643 2023-06-19 08:00:58.633227 skt-0.2.89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7725 2023-06-19 08:00:51.000000 skt-0.2.89/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-19 08:00:51.000000 skt-0.2.89/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-06-19 08:00:58.633227 skt-0.2.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2231 2023-06-19 08:00:51.000000 skt-0.2.89/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 08:00:58.629227 skt-0.2.89/skt/
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-06-19 08:00:51.000000 skt-0.2.89/skt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11840 2023-06-19 08:00:51.000000 skt-0.2.89/skt/data_catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)      911 2023-06-19 08:00:51.000000 skt-0.2.89/skt/data_lineage.py
--rw-r--r--   0 runner    (1001) docker     (122)    10057 2023-06-19 08:00:51.000000 skt-0.2.89/skt/eda_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)    28992 2023-06-19 08:00:51.000000 skt-0.2.89/skt/gcp.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-06-19 08:00:51.000000 skt-0.2.89/skt/gcp_credentials.py
--rw-r--r--   0 runner    (1001) docker     (122)     3348 2023-06-19 08:00:51.000000 skt-0.2.89/skt/github_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12049 2023-06-19 08:00:51.000000 skt-0.2.89/skt/hashing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1736 2023-06-19 08:00:51.000000 skt-0.2.89/skt/lake.py
--rw-r--r--   0 runner    (1001) docker     (122)    18513 2023-06-19 08:00:51.000000 skt-0.2.89/skt/mls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 08:00:58.629227 skt-0.2.89/skt/model/
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-19 08:00:51.000000 skt-0.2.89/skt/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3944 2023-06-19 08:00:51.000000 skt-0.2.89/skt/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1726 2023-06-19 08:00:51.000000 skt-0.2.89/skt/nes.py
--rw-r--r--   0 runner    (1001) docker     (122)      692 2023-06-19 08:00:51.000000 skt-0.2.89/skt/spark_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-06-19 08:00:51.000000 skt-0.2.89/skt/vault_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    14898 2023-06-19 08:00:51.000000 skt-0.2.89/skt/ye.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 08:00:58.629227 skt-0.2.89/skt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10643 2023-06-19 08:00:58.000000 skt-0.2.89/skt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      480 2023-06-19 08:00:58.000000 skt-0.2.89/skt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 08:00:58.000000 skt-0.2.89/skt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-19 08:00:58.000000 skt-0.2.89/skt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      906 2023-06-19 08:00:58.000000 skt-0.2.89/skt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-06-19 08:00:58.000000 skt-0.2.89/skt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-12 04:38:26.000000 skt-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (116)    10442 2020-08-12 04:38:26.000000 skt-0.2.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-12 04:38:26.000000 skt-0.2.9/skt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      434 2020-08-12 04:38:26.000000 skt-0.2.9/skt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    10442 2020-08-12 04:38:26.000000 skt-0.2.9/skt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)        4 2020-08-12 04:38:26.000000 skt-0.2.9/skt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-12 04:38:26.000000 skt-0.2.9/skt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       41 2020-08-12 04:38:26.000000 skt-0.2.9/skt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      603 2020-08-12 04:38:26.000000 skt-0.2.9/skt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     7605 2020-08-12 04:38:20.000000 skt-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      190 2020-08-12 04:38:26.000000 skt-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1735 2020-08-12 04:38:20.000000 skt-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-12 04:38:26.000000 skt-0.2.9/skt/
+-rw-r--r--   0 runner    (1001) docker     (116)     1736 2020-08-12 04:38:20.000000 skt-0.2.9/skt/lake.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11362 2020-08-12 04:38:20.000000 skt-0.2.9/skt/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12049 2020-08-12 04:38:20.000000 skt-0.2.9/skt/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14734 2020-08-12 04:38:20.000000 skt-0.2.9/skt/mls.py
+-rw-r--r--   0 runner    (1001) docker     (116)      692 2020-08-12 04:38:20.000000 skt-0.2.9/skt/spark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9641 2020-08-12 04:38:20.000000 skt-0.2.9/skt/eda_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-12 04:38:26.000000 skt-0.2.9/skt/model/
+-rw-r--r--   0 runner    (1001) docker     (116)     3925 2020-08-12 04:38:20.000000 skt-0.2.9/skt/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)       20 2020-08-12 04:38:20.000000 skt-0.2.9/skt/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       87 2020-08-12 04:38:20.000000 skt-0.2.9/skt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      227 2020-08-12 04:38:20.000000 skt-0.2.9/skt/vault_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9768 2020-08-12 04:38:20.000000 skt-0.2.9/skt/ye.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11825 2020-08-12 04:38:20.000000 skt-0.2.9/skt/data_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (116)      485 2020-08-12 04:38:20.000000 skt-0.2.9/skt/data_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1676 2020-08-12 04:38:20.000000 skt-0.2.9/skt/nes.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1714 2020-08-12 04:38:20.000000 skt-0.2.9/skt/github_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `skt-0.2.89/PKG-INFO` & `skt-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skt
-Version: 0.2.89
+Version: 0.2.9
 Summary: SKT package
 Home-page: https://github.com/sktaiflow/skt
 Author: SKT
 Author-email: all@sktai.io
 License: UNKNOWN
 Description: # SKT Package
         
@@ -14,24 +14,14 @@
         This is highly site dependent package.
         Resources are abstracted into package structure.
         
         
         ## Usage
         
         
-        Hive metastore
-        ```python
-        from skt.ye import get_hms
-        
-        c = get_hms()
-        c.get_partition_names("db", "table")
-        c.close()
-        ```
-        
-        
         Hash and unhash
         ```python
         from skt.lake import hash_s
         from skt.lake import unhash_s
         
         unhashed_list = ['0000000000']
         hashed_list = hash_s(unhashed_list)
```

### Comparing `skt-0.2.89/README.md` & `skt-0.2.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,14 @@
 This is highly site dependent package.
 Resources are abstracted into package structure.
 
 
 ## Usage
 
 
-Hive metastore
-```python
-from skt.ye import get_hms
-
-c = get_hms()
-c.get_partition_names("db", "table")
-c.close()
-```
-
-
 Hash and unhash
 ```python
 from skt.lake import hash_s
 from skt.lake import unhash_s
 
 unhashed_list = ['0000000000']
 hashed_list = hash_s(unhashed_list)
```

### Comparing `skt-0.2.89/skt/data_catalog.py` & `skt-0.2.9/skt/data_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 headers = {
     "Catalog-User": os.environ.get("USER", "unknown_user"),
     "Catalog-Hostname": os.environ.get("HOSTNAME", "unknown_hostname"),
     "Catalog-NB-User": os.environ.get("NB_USER", None),
 }
 
 
-DATA_CATALOG_SECRETS_NAME = "data_catalog/client"
-DATA_LINEAGE_SECRETS_NAME = "data_catalog/lineage"
+DATA_CATALOG_SECRETS_NAME = "data_catalog"
+DATA_LINEAGE_SECRETS_NAME = "data_lineage"
 
 
 def get_lineage(table):
     secrets = get_secrets(DATA_LINEAGE_SECRETS_NAME)
     return requests.get(f"{secrets['url_prd']}/relationships/lineage/node/{table}").json()
```

### Comparing `skt-0.2.89/skt/eda_tools.py` & `skt-0.2.9/skt/eda_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,22 +22,15 @@
 
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 stream_hander.setFormatter(formatter)
 eda_logger.addHandler(stream_hander)
 
 
 def numeric_eda_plot(
-    df,
-    feature_list,
-    label_col,
-    cols=2,
-    n_samples=-1,
-    plot_type="density",
-    stat_yn=False,
-    figsize=(7, 4),
+    df, feature_list, label_col, cols=2, n_samples=-1, plot_type="density", stat_yn=False, figsize=(7, 4),
 ):
     """
     Numeric feature에 대한 EDA Plot function
 
     Args. :
         - df           :   Pandas DataFrame 형태의 EDA대상 데이터
         - feature_list :   EDA 대상 feature list (df의 columns)
@@ -136,43 +129,31 @@
                 )
                 # calculate simple stats
                 if stat_yn:
                     tmp_stats = [
                         np.mean(orig_tmp_df[orig_tmp_df[label_col] == lb][col]),
                         np.min(orig_tmp_df[orig_tmp_df[label_col] == lb][col]),
                         np.max(orig_tmp_df[orig_tmp_df[label_col] == lb][col]),
-                        np.quantile(
-                            orig_tmp_df[orig_tmp_df[label_col] == lb][col],
-                            0.25,
-                        ),
-                        np.quantile(
-                            orig_tmp_df[orig_tmp_df[label_col] == lb][col],
-                            0.75,
-                        ),
+                        np.quantile(orig_tmp_df[orig_tmp_df[label_col] == lb][col], 0.25,),
+                        np.quantile(orig_tmp_df[orig_tmp_df[label_col] == lb][col], 0.75,),
                     ]
                     tmp_stats_text = " | ".join([pattern % i for i in tmp_stats])
                     stats.append("[{}] ".format(lb) + tmp_stats_text)
 
         elif plot_type == "box":
             tmp_df = orig_tmp_df
             sns.boxplot(x=label_col, y=col, data=tmp_df, ax=temp_ax)
             if stat_yn:
                 for j, lb in enumerate(labels):
                     tmp_stats = [
                         np.mean(orig_tmp_df[orig_tmp_df[label_col] == lb][col]),
                         np.min(orig_tmp_df[orig_tmp_df[label_col] == lb][col]),
                         np.max(orig_tmp_df[orig_tmp_df[label_col] == lb][col]),
-                        np.quantile(
-                            orig_tmp_df[orig_tmp_df[label_col] == lb][col],
-                            0.25,
-                        ),
-                        np.quantile(
-                            orig_tmp_df[orig_tmp_df[label_col] == lb][col],
-                            0.75,
-                        ),
+                        np.quantile(orig_tmp_df[orig_tmp_df[label_col] == lb][col], 0.25,),
+                        np.quantile(orig_tmp_df[orig_tmp_df[label_col] == lb][col], 0.75,),
                     ]
                     tmp_stats_text = " | ".join([pattern % i for i in tmp_stats])
                     stats.append("[{}] ".format(lb) + tmp_stats_text)
             temp_ax.set_ylabel("")
 
         if stat_yn:
             stat_title = "{}".format(" | ".join(stat_names))
@@ -264,20 +245,15 @@
             .groupby(level=[0])
             .cumsum()
             .reset_index()
             .sort_values(["perc"], ascending=False)
         )
 
         sns.barplot(
-            x=label_col,
-            y="perc",
-            hue=col,
-            data=tmp_df,
-            dodge=False,
-            ax=temp_ax,
+            x=label_col, y="perc", hue=col, data=tmp_df, dodge=False, ax=temp_ax,
         )
         temp_ax.legend(title="")
 
         temp_ax.title.set_text(col)
 
     plt.close(fig)
     return fig
```

### Comparing `skt-0.2.89/skt/github_utils.py` & `skt-0.2.9/skt/github_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import base64
 
-from github import Github, GithubException
+from github import Github
 from contextlib import contextmanager
 
 
 @contextmanager
 def proxy(proxies):
     import os
 
@@ -56,52 +56,7 @@
         if self._proxies:
             with proxy(self._proxies):
                 file_data = self._download_from_git(path)
         else:
             file_data = self._download_from_git(path)
 
         return file_data
-
-    def _download(self, org_id, repo_id, ref_id, path) -> bytes:
-        g = Github(self._token)
-        org = g.get_organization(org_id)
-        repo = org.get_repo(repo_id)
-        try:
-            content = repo.get_contents(path, ref=ref_id)
-            return content.decoded_content
-        except GithubException as e:
-            if e.status == 403:
-                if e.data["errors"][0]["code"] == "too_large":
-                    parent_path = path[: path.rfind("/")]
-                    contents = repo.get_contents(parent_path, ref=ref_id)
-                    for c in contents:
-                        if c.path == path:
-                            blob = repo.get_git_blob(c.sha)
-                            return base64.b64decode(blob.raw_data["content"])
-            raise e
-
-    def download(self, org_id, repo_id, ref_id, path) -> bytes:
-        if self._proxies:
-            with proxy(self._proxies):
-                file_data = self._download(org_id, repo_id, ref_id, path)
-        else:
-            file_data = self._download(org_id, repo_id, ref_id, path)
-
-        return file_data
-
-    def _parse_url(self, url):
-        from urllib.parse import urlparse
-
-        parse_result = urlparse(url)
-        if parse_result.netloc == "github.com":
-            splits = parse_result.path.split("/")
-            org_id = splits[1]
-            repo_id = splits[2]
-            ref_id = splits[4]
-            path = "/".join(splits[5:])
-
-        return org_id, repo_id, ref_id, path
-
-    def download_from_url(self, url) -> bytes:
-        ret = self._parse_url(url)
-
-        return self.download(*ret)
```

### Comparing `skt-0.2.89/skt/hashing.py` & `skt-0.2.9/skt/hashing.py`

 * *Files identical despite different names*

### Comparing `skt-0.2.89/skt/lake.py` & `skt-0.2.9/skt/lake.py`

 * *Files identical despite different names*

### Comparing `skt-0.2.89/skt/mls.py` & `skt-0.2.9/skt/mls.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,174 +4,52 @@
 
 import requests
 import pandas as pd
 import os
 
 from skt.vault_utils import get_secrets
 
-from sktmls.meta_tables.meta_table import MetaTableClient
-
 
 MLS_MODEL_DIR = os.path.join(Path.home(), "mls_temp_dir")
 MODEL_BINARY_NAME = "model.joblib"
 MODEL_TAR_NAME = "model.tar.gz"
 MODEL_META_NAME = "model.json"
 S3_DEFAULT_PATH = get_secrets("mls")["s3_model_registry_path"]
 
 EDD_OPTIONS = get_secrets("mls")["edd_options"]
 
 MLS_COMPONENTS_API_URL = "/api/v1/components"
 MLS_META_API_URL = "/api/v1/meta_tables"
 MLS_MLMODEL_API_URL = "/api/v1/models"
 
 
-def check_client_config(config):
-    client = MetaTableClient(**config)
-    client.list_meta_tables()
-    return config
-
-
-def generate_configs(env, user):
-    import pkg_resources
-    from packaging import version
-    from skt.vault_utils import get_secrets
+def get_mls_meta_table_client(env=None):
+    from sktmls.meta_tables.meta_table import MetaTableClient
     from sktmls import MLSENV
 
-    mlsenv = MLSENV.STG
     if env == "prd":
-        mlsenv = MLSENV.PRD
-    secrets = get_secrets(path="mls")
-    config = dict(
-        env=mlsenv,
-        username=secrets.get(f"{user}_id"),
-        password=secrets.get(f"{user}_pass"),
-    )
-
-    # sktmls version upgrade 후 수정
-    mls_v = pkg_resources.get_distribution("sktmls").version
-    if version.parse(mls_v) > version.parse("2020.8.29"):
-        from sktmls import MLSRuntimeENV
-
-        return [{**config, "runtime_env": r} for r in MLSRuntimeENV.list_items() if r != MLSRuntimeENV.EDD]
-
-    return [config]
-
-
-def get_mls_config(env, user):
-    import concurrent.futures
-
-    configs = generate_configs(env=env, user=user)
-    e = concurrent.futures.ThreadPoolExecutor(max_workers=len(configs) + 1)
-    fs = [e.submit(check_client_config, conf) for conf in configs]
-    for f in concurrent.futures.as_completed(fs):
-        if f.exception() is None:
-            config = f.result()
-            break
-    e.shutdown(wait=False)
-    return config
-
-
-def get_mls_meta_table_client(env="stg", user="reco"):
-    config = get_mls_config(env, user)
-    return MetaTableClient(**config)
-
-
-def get_mls_component_client(env="stg", user="reco"):
-    from sktmls.components import ComponentClient
-
-    config = get_mls_config(env, user)
-    return ComponentClient(**config)
-
-
-def get_mls_dimension_client(env="stg", user="reco"):
-    from sktmls.dimensions import DimensionClient
-
-    config = get_mls_config(env, user)
-    return DimensionClient(**config)
-
-
-def get_mls_experiment_client(env="stg", user="reco"):
-    from sktmls.experiments import ExperimentClient
-
-    config = get_mls_config(env, user)
-    return ExperimentClient(**config)
+        env = MLSENV.PRD
 
-
-def get_mls_ml_model_client(env="stg", user="reco"):
-    from sktmls.models import MLModelClient
-
-    config = get_mls_config(env, user)
-    return MLModelClient(**config)
-
-
-def get_mls_automl_batch_prediction_client(env="stg", user="reco"):
-    from sktmls.models.automl.automl_prediction import AutoMLBatchPredictionClient
-
-    config = get_mls_config(env, user)
-    return AutoMLBatchPredictionClient(**config)
-
-
-def get_mls_model_registry(env="stg", user="reco"):
-    from sktmls import ModelRegistry
-
-    config = get_mls_config(env, user)
-    return ModelRegistry(env=config["env"], runtime_env=config["runtime_env"])
-
-
-def get_channel_client(env="stg", user="reco"):
-    from sktmls.channels import ChannelClient
-
-    config = get_mls_config(env, user)
-    return ChannelClient(**config)
-
-
-def get_mls_profile_api_client(env="stg", user="reco"):
-    from sktmls.apis.profile_api import MLSProfileAPIClient
-
-    config = dict({conf for conf in get_mls_config(env, user).items() if conf[0] in ["env", "runtime_env"]})
-    return MLSProfileAPIClient(**config, **get_secrets("mls").get("reco_api"))
-
-
-def get_mls_recommendation_api_client(env="stg", user="reco"):
-    from sktmls.apis.recommendation_api import MLSRecommendationAPIClient
-
-    config = dict({conf for conf in get_mls_config(env, user).items() if conf[0] in ["env", "runtime_env"]})
-    return MLSRecommendationAPIClient(**config, **get_secrets("mls").get("reco_api"))
-
-
-def create_or_update_meta_table(table_name, schema=None, env="stg", user="reco"):
-    c = get_mls_meta_table_client(env=env, user=user)
-    if c.meta_table_exists(name=table_name):
-        t = c.get_meta_table(name=table_name)
-        if schema:
-            c.update_meta_table(meta_table=t, schema=schema)
-    else:
-        c.create_meta_table(name=table_name, schema=schema)
-
-
-def upsert_meta_table(table_name, items_dict, env="stg", user="reco"):
-    c = get_mls_meta_table_client(env=env, user=user)
-    t = c.get_meta_table(name=table_name)
-    items = c.create_meta_items(meta_table=t, items_dict=items_dict)
-    return len(items)
+    secrets = get_secrets(path="mls")
+    reco_id = secrets["reco_id"]
+    reco_pass = secrets["reco_pass"]
+    return MetaTableClient(env=env, username=reco_id, password=reco_pass)
 
 
 def set_model_name(comm_db, params, user="reco", edd: bool = False):
     secret = get_secrets("mls")
     token = secret.get("user_token").get(user)
     if comm_db[-3:] == "dev":  # stg
         url = secret["ab_onprem_stg_url"] if edd else secret["ab_stg_url"]
         url = f"{url}{MLS_COMPONENTS_API_URL}"
     else:  # prd
         url = secret["ab_onprem_prd_url"] if edd else secret["ab_prd_url"]
         url = f"{url}{MLS_COMPONENTS_API_URL}"
     requests.post(
-        url,
-        json=params,
-        headers={"Authorization": f"Basic {{{token}}}"},
+        url, json=params, headers={"Authorization": f"Basic {{{token}}}"},
     )
 
 
 def get_all_recent_model_path(comm_db, user="reco", edd: bool = False):
     secret = get_secrets("mls")
     token = secret.get("user_token").get(user)
     if comm_db[-3:] == "dev":  # stg
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `skt-0.2.89/skt/model/utils.py` & `skt-0.2.9/skt/model/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from collections import Counter
 from skt.ye import hive_to_pandas, slack_send
 
 
 # post_filter 이후, context_mapping 을 마친 post_filter_with_context_id Table 생성
 def context_mapping(
-    meta_table=None,
-    comm_db=None,
-    reco_type=None,
-    model_name=None,
-    dt=None,
-    feature_ym=None,
+    meta_table=None, comm_db=None, reco_type=None, model_name=None, dt=None, feature_ym=None,
 ):
+
     # 0. item_reco_predict_post_filter with impression 'Y' table LOAD
     query = f"""
     select *
     from {comm_db}.item_reco_predict_post_filter
     where reco_type = '{reco_type}'
     and model = '{model_name}'
     and dt = '{dt}'
```

### Comparing `skt-0.2.89/skt/nes.py` & `skt-0.2.9/skt/nes.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import click
 
 
 nes_url = "http://nes.sktai.io/v1/runs"
 
 
 def nes_submit(
-    input_notebook,
-    parameters=None,
+    input_notebook, parameters=None,
 ):
     data = {}
     data["input_url"] = input_notebook
     if parameters:
         data["parameters"] = parameters
     res = requests.post(nes_url, json=data)
     print(f"Job submitted with: {data}")
@@ -27,16 +26,15 @@
     res = requests.get(f"{nes_url}/{id}")
     res.raise_for_status()
     status = res.json()["status"]
     return status
 
 
 def nes_execute(
-    input_notebook,
-    parameters=None,
+    input_notebook, parameters=None,
 ):
     """
     return: str
     Succeeeded or Failed or Error
     """
     from time import sleep
 
@@ -49,26 +47,18 @@
         status = nes_get_status(id)
     return status, output_url
 
 
 @click.command(context_settings=dict(help_option_names=["-h", "--help"]))
 @click.argument("input_notebook")
 @click.option(
-    "--parameters",
-    "-p",
-    nargs=2,
-    multiple=True,
-    help="Parameters to pass to the parameters cell.",
+    "--parameters", "-p", nargs=2, multiple=True, help="Parameters to pass to the parameters cell.",
 )
 def nes_cli(
-    input_notebook,
-    parameters,
+    input_notebook, parameters,
 ):
     parameters_final = {}
     for name, value in parameters or []:
         parameters_final[name] = value
-    status, output_url = nes_execute(
-        input_notebook,
-        parameters=parameters_final,
-    )
+    status, output_url = nes_execute(input_notebook, parameters=parameters_final,)
     print(f"output_url: {output_url}")
     print(f"status: {status}")
```

### Comparing `skt-0.2.89/skt/spark_utils.py` & `skt-0.2.9/skt/spark_utils.py`

 * *Files identical despite different names*

### Comparing `skt-0.2.89/skt.egg-info/PKG-INFO` & `skt-0.2.9/skt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skt
-Version: 0.2.89
+Version: 0.2.9
 Summary: SKT package
 Home-page: https://github.com/sktaiflow/skt
 Author: SKT
 Author-email: all@sktai.io
 License: UNKNOWN
 Description: # SKT Package
         
@@ -14,24 +14,14 @@
         This is highly site dependent package.
         Resources are abstracted into package structure.
         
         
         ## Usage
         
         
-        Hive metastore
-        ```python
-        from skt.ye import get_hms
-        
-        c = get_hms()
-        c.get_partition_names("db", "table")
-        c.close()
-        ```
-        
-        
         Hash and unhash
         ```python
         from skt.lake import hash_s
         from skt.lake import unhash_s
         
         unhashed_list = ['0000000000']
         hashed_list = hash_s(unhashed_list)
```

