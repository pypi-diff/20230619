# Comparing `tmp/alohomora-3.0.0.tar.gz` & `tmp/alohomora-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alohomora-3.0.0.tar", last modified: Fri Jun  3 18:49:33 2022, max compression
+gzip compressed data, was "alohomora-3.0.1.tar", last modified: Mon Jun 19 21:57:33 2023, max compression
```

## Comparing `alohomora-3.0.0.tar` & `alohomora-3.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 18:49:33.028174 alohomora-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-06-03 18:49:18.000000 alohomora-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-06-03 18:49:33.028174 alohomora-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6988 2022-06-03 18:49:18.000000 alohomora-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 18:49:33.028174 alohomora-3.0.0/alohomora/
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-06-03 18:49:18.000000 alohomora-3.0.0/alohomora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3108 2022-06-03 18:49:18.000000 alohomora-3.0.0/alohomora/keys.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10395 2022-06-03 18:49:18.000000 alohomora-3.0.0/alohomora/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    31655 2022-06-03 18:49:18.000000 alohomora-3.0.0/alohomora/req.py
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-06-03 18:49:18.000000 alohomora-3.0.0/alohomora/saml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 18:49:33.028174 alohomora-3.0.0/alohomora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-06-03 18:49:32.000000 alohomora-3.0.0/alohomora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-06-03 18:49:33.000000 alohomora-3.0.0/alohomora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 18:49:32.000000 alohomora-3.0.0/alohomora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-06-03 18:49:32.000000 alohomora-3.0.0/alohomora.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-06-03 18:49:32.000000 alohomora-3.0.0/alohomora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-06-03 18:49:32.000000 alohomora-3.0.0/alohomora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-06-03 18:49:33.028174 alohomora-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-06-03 18:49:18.000000 alohomora-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:33.910606 alohomora-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-19 21:57:18.000000 alohomora-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-19 21:57:33.910606 alohomora-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-19 21:57:18.000000 alohomora-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:33.906606 alohomora-3.0.1/alohomora/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-19 21:57:18.000000 alohomora-3.0.1/alohomora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-19 21:57:18.000000 alohomora-3.0.1/alohomora/keys.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10395 2023-06-19 21:57:18.000000 alohomora-3.0.1/alohomora/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31655 2023-06-19 21:57:18.000000 alohomora-3.0.1/alohomora/req.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-19 21:57:18.000000 alohomora-3.0.1/alohomora/saml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:33.910606 alohomora-3.0.1/alohomora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-19 21:57:33.000000 alohomora-3.0.1/alohomora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-19 21:57:33.000000 alohomora-3.0.1/alohomora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:57:33.000000 alohomora-3.0.1/alohomora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 21:57:33.000000 alohomora-3.0.1/alohomora.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-19 21:57:33.000000 alohomora-3.0.1/alohomora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-19 21:57:33.000000 alohomora-3.0.1/alohomora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-19 21:57:33.910606 alohomora-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-19 21:57:18.000000 alohomora-3.0.1/setup.py
```

### Comparing `alohomora-3.0.0/LICENSE` & `alohomora-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alohomora-3.0.0/README.md` & `alohomora-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alohomora-3.0.0/alohomora/__init__.py` & `alohomora-3.0.1/alohomora/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
-__version__ = '3.0.0'
+__version__ = '3.0.1'
 __author__ = 'Viasat'
 __author_email__ = 'vice-support@viasat.com'
 __license__ = '(c) 2022 Viasat, Inc. See the LICENSE file for more details.'
 __url__ = 'https://github.com/Viasat/alohomora'
 __description__ = 'Get AWS API keys for a SAML-federated identity'
```

### Comparing `alohomora-3.0.0/alohomora/keys.py` & `alohomora-3.0.1/alohomora/keys.py`

 * *Files identical despite different names*

### Comparing `alohomora-3.0.0/alohomora/main.py` & `alohomora-3.0.1/alohomora/main.py`

 * *Files identical despite different names*

### Comparing `alohomora-3.0.0/alohomora/req.py` & `alohomora-3.0.1/alohomora/req.py`

 * *Files identical despite different names*

### Comparing `alohomora-3.0.0/alohomora/saml.py` & `alohomora-3.0.1/alohomora/saml.py`

 * *Files identical despite different names*

### Comparing `alohomora-3.0.0/setup.py` & `alohomora-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,10 +33,10 @@
     },
     install_requires=[
         "boto3>=1.3.1",
         "beautifulsoup4>=4.5.1",
         "requests>=2.11.1",
     ],
     extras_require={
-        "fido2": ["fido2>=0.9.3"]
+        "fido2": ["fido2==0.9.3"]
     }
 )
```

