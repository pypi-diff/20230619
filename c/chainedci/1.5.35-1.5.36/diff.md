# Comparing `tmp/chainedci-1.5.35.tar.gz` & `tmp/chainedci-1.5.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainedci-1.5.35.tar", last modified: Tue Jun 13 07:11:02 2023, max compression
+gzip compressed data, was "chainedci-1.5.36.tar", last modified: Mon Jun 19 10:11:19 2023, max compression
```

## Comparing `chainedci-1.5.35.tar` & `chainedci-1.5.36.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:11:02.777854 chainedci-1.5.35/
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-06-13 07:10:46.000000 chainedci-1.5.35/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      923 2023-06-13 07:11:02.777854 chainedci-1.5.35/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-13 07:10:46.000000 chainedci-1.5.35/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:11:02.774854 chainedci-1.5.35/chainedci/
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11472 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/artifact.py
--rw-rw-rw-   0 root         (0) root         (0)     9356 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/artifact_src.py
--rwxrwxrwx   0 root         (0) root         (0)      131 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/chainedci
--rw-rw-rw-   0 root         (0) root         (0)     6338 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     6819 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3663 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/default_chainedci.yml
--rw-rw-rw-   0 root         (0) root         (0)     3926 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/env_vars.py
--rw-rw-rw-   0 root         (0) root         (0)     2924 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/http_adapter.py
--rw-rw-rw-   0 root         (0) root         (0)     3932 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/init_project.py
--rw-rw-rw-   0 root         (0) root         (0)     4174 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     4850 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/log.py
--rw-rw-rw-   0 root         (0) root         (0)     5935 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/options.py
--rw-rw-rw-   0 root         (0) root         (0)     3888 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/parser.py
--rw-rw-rw-   0 root         (0) root         (0)    10532 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4890 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/scenario.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:11:02.776854 chainedci-1.5.35/chainedci/static/
--rw-rw-rw-   0 root         (0) root         (0)        8 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/static/inventory
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/static/projectA.yml
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/static/projectA_config1.yml
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/static/projectA_config2.yml
--rw-rw-rw-   0 root         (0) root         (0)    15020 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:11:02.776854 chainedci-1.5.35/chainedci/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1165 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/templates/all.yml.tpl
--rw-rw-rw-   0 root         (0) root         (0)     3974 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/templates/main.yml.tpl
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/templates/scenario.yml.tpl
--rw-rw-rw-   0 root         (0) root         (0)     2782 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/tools.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-06-13 07:10:46.000000 chainedci-1.5.35/chainedci/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:11:02.775854 chainedci-1.5.35/chainedci.egg-info/
--rw-r--r--   0 root         (0) root         (0)      923 2023-06-13 07:11:02.000000 chainedci-1.5.35/chainedci.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      924 2023-06-13 07:11:02.000000 chainedci-1.5.35/chainedci.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 07:11:02.000000 chainedci-1.5.35/chainedci.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 07:11:02.000000 chainedci-1.5.35/chainedci.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       99 2023-06-13 07:11:02.000000 chainedci-1.5.35/chainedci.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 07:11:02.000000 chainedci-1.5.35/chainedci.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-06-13 07:11:02.777854 chainedci-1.5.35/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1241 2023-06-13 07:10:46.000000 chainedci-1.5.35/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:11:02.777854 chainedci-1.5.35/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 07:10:46.000000 chainedci-1.5.35/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1318 2023-06-13 07:10:46.000000 chainedci-1.5.35/tests/tests_lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:11:19.571069 chainedci-1.5.36/
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-06-19 10:11:02.000000 chainedci-1.5.36/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      923 2023-06-19 10:11:19.571069 chainedci-1.5.36/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-19 10:11:02.000000 chainedci-1.5.36/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:11:19.568069 chainedci-1.5.36/chainedci/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11472 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/artifact.py
+-rw-rw-rw-   0 root         (0) root         (0)     9356 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/artifact_src.py
+-rwxrwxrwx   0 root         (0) root         (0)      131 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/chainedci
+-rw-rw-rw-   0 root         (0) root         (0)     6338 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     6819 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/default_chainedci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3926 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/env_vars.py
+-rw-rw-rw-   0 root         (0) root         (0)     2924 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/http_adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3932 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/init_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     4174 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     5935 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     3888 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    10532 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4890 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/scenario.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:11:19.570069 chainedci-1.5.36/chainedci/static/
+-rw-rw-rw-   0 root         (0) root         (0)        8 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/static/inventory
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/static/projectA.yml
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/static/projectA_config1.yml
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/static/projectA_config2.yml
+-rw-rw-rw-   0 root         (0) root         (0)    15020 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:11:19.571069 chainedci-1.5.36/chainedci/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/templates/all.yml.tpl
+-rw-rw-rw-   0 root         (0) root         (0)     3974 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/templates/main.yml.tpl
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/templates/scenario.yml.tpl
+-rw-rw-rw-   0 root         (0) root         (0)     2782 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-06-19 10:11:02.000000 chainedci-1.5.36/chainedci/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:11:19.569069 chainedci-1.5.36/chainedci.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      923 2023-06-19 10:11:19.000000 chainedci-1.5.36/chainedci.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      924 2023-06-19 10:11:19.000000 chainedci-1.5.36/chainedci.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 10:11:19.000000 chainedci-1.5.36/chainedci.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 10:11:19.000000 chainedci-1.5.36/chainedci.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       99 2023-06-19 10:11:19.000000 chainedci-1.5.36/chainedci.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-19 10:11:19.000000 chainedci-1.5.36/chainedci.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-06-19 10:11:19.572069 chainedci-1.5.36/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2023-06-19 10:11:02.000000 chainedci-1.5.36/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:11:19.571069 chainedci-1.5.36/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 10:11:02.000000 chainedci-1.5.36/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2023-06-19 10:11:02.000000 chainedci-1.5.36/tests/tests_lib.py
```

### Comparing `chainedci-1.5.35/PKG-INFO` & `chainedci-1.5.36/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainedci
-Version: 1.5.35
+Version: 1.5.36
 Summary: Chaine Gitlab CI pipelines
 Home-page: https://gitlab.com/Orange-OpenSource/lfn/ci_cd/chained-ci
 Author: Orange OpenSource
 License: Apache 2.0
 Description-Content-Type: text/markdown
 
 # Chained-ci-py
```

### Comparing `chainedci-1.5.35/README.md` & `chainedci-1.5.36/README.md`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/artifact.py` & `chainedci-1.5.36/chainedci/artifact.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/artifact_src.py` & `chainedci-1.5.36/chainedci/artifact_src.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/cli.py` & `chainedci-1.5.36/chainedci/cli.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/config.py` & `chainedci-1.5.36/chainedci/config.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/default_chainedci.yml` & `chainedci-1.5.36/chainedci/default_chainedci.yml`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/env_vars.py` & `chainedci-1.5.36/chainedci/env_vars.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/http_adapter.py` & `chainedci-1.5.36/chainedci/http_adapter.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/init_project.py` & `chainedci-1.5.36/chainedci/init_project.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/inventory.py` & `chainedci-1.5.36/chainedci/inventory.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/log.py` & `chainedci-1.5.36/chainedci/log.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/options.py` & `chainedci-1.5.36/chainedci/options.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/parser.py` & `chainedci-1.5.36/chainedci/parser.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/pipeline.py` & `chainedci-1.5.36/chainedci/pipeline.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/scenario.py` & `chainedci-1.5.36/chainedci/scenario.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/step.py` & `chainedci-1.5.36/chainedci/step.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/templates/all.yml.tpl` & `chainedci-1.5.36/chainedci/templates/all.yml.tpl`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/templates/main.yml.tpl` & `chainedci-1.5.36/chainedci/templates/main.yml.tpl`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/templates/scenario.yml.tpl` & `chainedci-1.5.36/chainedci/templates/scenario.yml.tpl`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/tools.py` & `chainedci-1.5.36/chainedci/tools.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/chainedci/version.py` & `chainedci-1.5.36/chainedci/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 """Version module."""
 
-__version__ = "1.5.35"
+__version__ = "1.5.36"
```

### Comparing `chainedci-1.5.35/chainedci.egg-info/PKG-INFO` & `chainedci-1.5.36/chainedci.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainedci
-Version: 1.5.35
+Version: 1.5.36
 Summary: Chaine Gitlab CI pipelines
 Home-page: https://gitlab.com/Orange-OpenSource/lfn/ci_cd/chained-ci
 Author: Orange OpenSource
 License: Apache 2.0
 Description-Content-Type: text/markdown
 
 # Chained-ci-py
```

### Comparing `chainedci-1.5.35/chainedci.egg-info/SOURCES.txt` & `chainedci-1.5.36/chainedci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.35/setup.py` & `chainedci-1.5.36/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 def readme():
     """Set Readme from file."""
     with open('README.md', encoding="utf-8") as f:
         return f.read()
 
 
 setup(name='chainedci',
-      version='1.5.35',
+      version='1.5.36',
       description='Chaine Gitlab CI pipelines',
       long_description=readme(),
       long_description_content_type='text/markdown',
       url='https://gitlab.com/Orange-OpenSource/lfn/ci_cd/chained-ci',
       author='Orange OpenSource',
       license='Apache 2.0',
       packages=find_packages(),
```

### Comparing `chainedci-1.5.35/tests/tests_lib.py` & `chainedci-1.5.36/tests/tests_lib.py`

 * *Files identical despite different names*

