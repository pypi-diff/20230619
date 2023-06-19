# Comparing `tmp/purplecaffeine-0.1.1.tar.gz` & `tmp/purplecaffeine-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purplecaffeine-0.1.1.tar", last modified: Mon Jun  5 16:55:27 2023, max compression
+gzip compressed data, was "purplecaffeine-0.2.0.tar", last modified: Mon Jun 19 21:13:23 2023, max compression
```

## Comparing `purplecaffeine-0.1.1.tar` & `purplecaffeine-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.025554 purplecaffeine-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-05 16:55:27.025554 purplecaffeine-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.021554 purplecaffeine-0.1.1/purplecaffeine/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/purplecaffeine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17993 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/purplecaffeine/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/purplecaffeine/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.021554 purplecaffeine-0.1.1/purplecaffeine/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/purplecaffeine/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/purplecaffeine/helpers/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.021554 purplecaffeine-0.1.1/purplecaffeine/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/purplecaffeine/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/purplecaffeine/utils/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.021554 purplecaffeine-0.1.1/purplecaffeine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-05 16:55:26.000000 purplecaffeine-0.1.1/purplecaffeine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-05 16:55:26.000000 purplecaffeine-0.1.1/purplecaffeine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:55:26.000000 purplecaffeine-0.1.1/purplecaffeine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 16:55:26.000000 purplecaffeine-0.1.1/purplecaffeine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 16:55:26.000000 purplecaffeine-0.1.1/purplecaffeine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:55:27.025554 purplecaffeine-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.021554 purplecaffeine-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.021554 purplecaffeine-0.1.1/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/tests/helpers/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/tests/test_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.021554 purplecaffeine-0.1.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/tests/utils/test_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:13:23.222534 purplecaffeine-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-19 21:13:23.222534 purplecaffeine-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:13:23.222534 purplecaffeine-0.2.0/purplecaffeine/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/purplecaffeine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20856 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/purplecaffeine/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/purplecaffeine/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:13:23.222534 purplecaffeine-0.2.0/purplecaffeine/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/purplecaffeine/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/purplecaffeine/helpers/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:13:23.222534 purplecaffeine-0.2.0/purplecaffeine/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/purplecaffeine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/purplecaffeine/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/purplecaffeine/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:13:23.222534 purplecaffeine-0.2.0/purplecaffeine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-19 21:13:23.000000 purplecaffeine-0.2.0/purplecaffeine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-19 21:13:23.000000 purplecaffeine-0.2.0/purplecaffeine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:13:23.000000 purplecaffeine-0.2.0/purplecaffeine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-19 21:13:23.000000 purplecaffeine-0.2.0/purplecaffeine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-19 21:13:23.000000 purplecaffeine-0.2.0/purplecaffeine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 21:13:23.222534 purplecaffeine-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:13:23.222534 purplecaffeine-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:13:23.222534 purplecaffeine-0.2.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/tests/helpers/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/tests/test_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/tests/test_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:13:23.222534 purplecaffeine-0.2.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-19 21:13:14.000000 purplecaffeine-0.2.0/tests/utils/test_json.py
```

### Comparing `purplecaffeine-0.1.1/PKG-INFO` & `purplecaffeine-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purplecaffeine
-Version: 0.1.1
+Version: 0.2.0
 Summary: PurpleCaffeine: tracking of quantum programs and experiments
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum tracking experiments
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `purplecaffeine-0.1.1/README.md` & `purplecaffeine-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.1.1/purplecaffeine/core.py` & `purplecaffeine-0.2.0/purplecaffeine/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,26 +63,48 @@
             artifacts (List[(str, Any)]): list of artifact, any external files
             texts (List[(str, str)]): list of text, any descriptions
             arrays (List[(str, Union[np.ndarray, List[Any]])]):
                 list of array, like quantum circuit results
             tags (List[str]): list of tags in string format
         """
         self.uuid = uuid or str(uuid4())
-        self.name = name
-        self.storage = storage or LocalStorage(path="./")
+        self.name = name or os.environ.get("PURPLE_CAFFEINE_TRIAL_NAME")
+        if self.name is None:
+            raise PurpleCaffeineException(
+                "Please specify name of trial or configure it using env variables"
+            )
+
+        if storage is None:
+            storage_type = os.environ.get(
+                "PURPLE_CAFFEINE_STORAGE_CLASS", "LocalStorage"
+            )
+            storage_mapping: Dict[str, BaseStorage] = {
+                "LocalStorage": LocalStorage,
+                "S3Storage": S3Storage,
+                "ApiStorage": ApiStorage,
+            }
+            self.storage = storage_mapping.get(storage_type)()
+        else:
+            self.storage = storage
 
-        self.description = description or ""
+        self.description = description or os.environ.get(
+            "PURPLE_CAFFEINE_TRIAL_DESCRIPTION", ""
+        )
         self.metrics = metrics or []
         self.parameters = parameters or []
         self.circuits = circuits or []
         self.operators = operators or []
         self.artifacts = artifacts or []
         self.texts = texts or []
         self.arrays = arrays or []
-        self.tags = tags or []
+        self.tags = tags or (
+            os.environ.get("PURPLE_CAFFEINE_TRIAL_TAGS", "").split(",")
+            if os.environ.get("PURPLE_CAFFEINE_TRIAL_TAGS")
+            else []
+        )
 
     def __repr__(self):
         return f"<Trial [{self.name}] {self.uuid}>"
 
     def __enter__(self):
         return self
 
@@ -265,33 +287,55 @@
         """
         raise NotImplementedError
 
 
 class ApiStorage(BaseStorage):
     """API storage class."""
 
-    def __init__(self, username: str, password: str, host: str):
+    def __init__(
+        self,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        host: Optional[str] = None,
+    ):
         """Creates storage for APIServer.
 
         Example:
             >>> storage = ApiStorage(
             >>>     host="http://localhost:8000/",
             >>>     username="admin",
             >>>     password="123"
             >>> )
 
         Args:
             username: username
             password: password
             host: host of api server
         """
-        self.username = username
-        self.host = host
+        self.username = username or os.environ.get(
+            "PURPLE_CAFFEINE_API_STORAGE_USERNAME"
+        )
+        if self.username is None:
+            raise PurpleCaffeineException(
+                "Please specify api storage username or configure it using env variables"
+            )
+        self.password = password or os.environ.get(
+            "PURPLE_CAFFEINE_API_STORAGE_PASSWORD"
+        )
+        if self.password is None:
+            raise PurpleCaffeineException(
+                "Please specify api storage Password or configure it using env variables"
+            )
+        self.host = host or os.environ.get("PURPLE_CAFFEINE_API_STORAGE_HOST")
+        if self.host is None:
+            raise PurpleCaffeineException(
+                "Please specify api storage host or configure it using env variables"
+            )
 
-        self.token = self._get_token(username, password)
+        self.token = self._get_token(self.username, self.password)
 
     def _get_token(self, username: str, password: str) -> str:
         """Returns token based on username and password
 
         Returns:
             authorization token
         """
@@ -392,25 +436,25 @@
 
         return trials
 
 
 class LocalStorage(BaseStorage):
     """Local storage."""
 
-    def __init__(self, path: str):
+    def __init__(self, path: Optional[str] = None):
         """Creates local storage for storing trial data
         at local folder.
 
         Example:
             >>> storage = LocalStorage("./")
 
         Args:
             path: path for the local storage folder
         """
-        self.path = path
+        self.path = path or os.environ.get("PURPLE_CAFFEINE_LOCAL_STORAGE_PATH", "./")
         if not os.path.exists(self.path):
             Path(self.path).mkdir(parents=True, exist_ok=True)
 
     def save(self, trial: Trial) -> str:
         """Saves given trial.
 
         Args:
@@ -462,14 +506,15 @@
         Returns:
             list of trials
         """
         offset = offset or 0
         limit = limit or 10
 
         trials_path = glob.glob(f"{self.path}/**.json")
+        trials_path.sort(key=os.path.getmtime, reverse=True)
         trials = []
         for path in trials_path:
             with open(path, "r", encoding="utf-8") as trial_file:
                 trial_dict = json.load(trial_file, cls=TrialDecoder)
                 trials.append(Trial(**trial_dict))
 
         if query:
@@ -477,24 +522,24 @@
                 trial
                 for trial in trials
                 if (query in trial.tags)
                 or (trial.name.find(query) != -1)
                 or (trial.description.find(query) != -1)
             ]
 
-        trials = trials[offset:limit]
+        trials = trials[offset : offset + limit]
         return trials
 
 
 class S3Storage(BaseStorage):
     """S3 storage."""
 
     def __init__(
         self,
-        bucket_name: str,
+        bucket_name: Optional[str] = None,
         access_key: Optional[str] = None,
         secret_access_key: Optional[str] = None,
         directory: Optional[str] = None,
         endpoint_url: Optional[str] = None,
     ):
         """Storage storage for s3 buckets.
 
@@ -506,23 +551,42 @@
         Args:
             bucket_name: bucket name
             access_key: aws key
             secret_access_key: aws access key
             directory: optional directory within bucket
             endpoint_url: optional endpoint url for custom S3 location
         """
+        self.bucket_name = bucket_name or os.environ.get("PURPLE_CAFFEINE_S3_BUCKET")
+        if self.bucket_name is None:
+            raise PurpleCaffeineException(
+                "Please specify name of S3 Bucket or configure it using env variables"
+            )
+        self.access_key = os.environ.get("PURPLE_CAFFEINE_S3_ACCESS_KEY")
+        if access_key is not None:
+            self.access_key = access_key
+
+        self.secret_access_key = os.environ.get("PURPLE_CAFFEINE_S3_SECRET_ACCESS_KEY")
+        if secret_access_key is not None:
+            self.secret_access_key = secret_access_key
+
+        if self.secret_access_key is None or self.access_key is None:
+            raise PurpleCaffeineException(
+                "Please specify Access key of S3 Bucket or configure it using env variables"
+            )
+        self.directory = directory or os.environ.get("PURPLE_CAFFEINE_S3_DIRECTORY")
+        self.endpoint_url = endpoint_url or os.environ.get(
+            "PURPLE_CAFFEINE_S3_ENDPOINT"
+        )
         client_s3 = boto3.client(
             "s3",
-            aws_access_key_id=access_key,
-            aws_secret_access_key=secret_access_key,
+            aws_access_key_id=self.access_key,
+            aws_secret_access_key=self.secret_access_key,
             endpoint_url=endpoint_url,
         )
         self.client_s3 = client_s3
-        self.bucket_name = bucket_name
-        self.directory = directory
 
     def save(self, trial: Trial) -> str:
         """Saves given trial.
 
         Args:
             trial: trial to save
```

### Comparing `purplecaffeine-0.1.1/purplecaffeine/helpers/conf.py` & `purplecaffeine-0.2.0/purplecaffeine/helpers/conf.py`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.1.1/purplecaffeine/utils/json.py` & `purplecaffeine-0.2.0/purplecaffeine/utils/json.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 # pylint: disable=no-else-return, import-outside-toplevel, cyclic-import
 class TrialEncoder(RuntimeEncoder):
     """Json encoder for trial."""
 
     def default(self, obj: Any) -> Any:
+        "custom encoder"
         from purplecaffeine.core import BaseStorage
 
         if isinstance(obj, Backend):
             return {
                 "__type__": "Backend",
                 "__value__": pickle.dumps(obj),
             }
@@ -23,14 +24,15 @@
         return super().default(obj)
 
 
 class TrialDecoder(RuntimeDecoder):
     """Json decoder for trial."""
 
     def object_hook(self, obj: Any) -> Any:
+        "custom decoder"
         if "__type__" in obj:
             obj_type = obj["__type__"]
 
             if obj_type == "Backend":
                 return pickle.loads(obj["__value__"])
             elif obj_type == "PurpleCaffeineStorage":
                 # we should not recover trial backend
```

### Comparing `purplecaffeine-0.1.1/purplecaffeine.egg-info/PKG-INFO` & `purplecaffeine-0.2.0/purplecaffeine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purplecaffeine
-Version: 0.1.1
+Version: 0.2.0
 Summary: PurpleCaffeine: tracking of quantum programs and experiments
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum tracking experiments
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `purplecaffeine-0.1.1/purplecaffeine.egg-info/SOURCES.txt` & `purplecaffeine-0.2.0/purplecaffeine.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 README.md
 setup.py
 purplecaffeine/__init__.py
 purplecaffeine/core.py
 purplecaffeine/exception.py
+purplecaffeine/widget.py
 purplecaffeine.egg-info/PKG-INFO
 purplecaffeine.egg-info/SOURCES.txt
 purplecaffeine.egg-info/dependency_links.txt
 purplecaffeine.egg-info/requires.txt
 purplecaffeine.egg-info/top_level.txt
 purplecaffeine/helpers/__init__.py
 purplecaffeine/helpers/conf.py
 purplecaffeine/utils/__init__.py
 purplecaffeine/utils/json.py
 tests/__init__.py
 tests/test_storage.py
 tests/test_trial.py
+tests/test_widget.py
 tests/helpers/__init__.py
 tests/helpers/test_conf.py
 tests/utils/__init__.py
 tests/utils/test_json.py
```

### Comparing `purplecaffeine-0.1.1/setup.py` & `purplecaffeine-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.1.1/tests/helpers/test_conf.py` & `purplecaffeine-0.2.0/tests/helpers/test_conf.py`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.1.1/tests/test_storage.py` & `purplecaffeine-0.2.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.1.1/tests/test_trial.py` & `purplecaffeine-0.2.0/tests/test_trial.py`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.1.1/tests/utils/test_json.py` & `purplecaffeine-0.2.0/tests/utils/test_json.py`

 * *Files identical despite different names*

