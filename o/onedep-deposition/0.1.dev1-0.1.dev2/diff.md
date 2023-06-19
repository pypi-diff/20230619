# Comparing `tmp/onedep_deposition-0.1.dev1.tar.gz` & `tmp/onedep_deposition-0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onedep_deposition-0.1.dev1.tar", last modified: Sat Jun 17 21:10:02 2023, max compression
+gzip compressed data, was "onedep_deposition-0.1.dev2.tar", last modified: Mon Jun 19 14:34:19 2023, max compression
```

## Comparing `onedep_deposition-0.1.dev1.tar` & `onedep_deposition-0.1.dev2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-17 21:10:02.009162 onedep_deposition-0.1.dev1/
--rw-r--r--   0 peisach    (502) staff       (20)      552 2023-06-13 13:04:02.000000 onedep_deposition-0.1.dev1/LICENSE
--rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-17 21:10:02.008865 onedep_deposition-0.1.dev1/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)     4641 2023-06-17 15:30:45.000000 onedep_deposition-0.1.dev1/README.md
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-17 21:10:02.005014 onedep_deposition-0.1.dev1/onedep_deposition/
--rw-r--r--   0 peisach    (502) staff       (20)       25 2023-06-13 13:04:02.000000 onedep_deposition-0.1.dev1/onedep_deposition/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-17 21:10:02.008093 onedep_deposition-0.1.dev1/onedep_deposition/cli/
--rw-r--r--   0 peisach    (502) staff       (20)        0 2023-06-17 17:42:03.000000 onedep_deposition-0.1.dev1/onedep_deposition/cli/__init__.py
--rw-r--r--   0 peisach    (502) staff       (20)    12091 2023-06-17 17:38:06.000000 onedep_deposition-0.1.dev1/onedep_deposition/cli/cli.py
--rw-r--r--   0 peisach    (502) staff       (20)    16794 2023-06-17 16:20:15.000000 onedep_deposition-0.1.dev1/onedep_deposition/constants.py
--rw-r--r--   0 peisach    (502) staff       (20)    14441 2023-06-17 16:32:54.000000 onedep_deposition-0.1.dev1/onedep_deposition/deposit_api.py
--rw-r--r--   0 peisach    (502) staff       (20)     9006 2023-06-15 13:32:19.000000 onedep_deposition-0.1.dev1/onedep_deposition/enum.py
--rw-r--r--   0 peisach    (502) staff       (20)      159 2023-06-08 16:58:15.000000 onedep_deposition-0.1.dev1/onedep_deposition/exceptions.py
--rw-r--r--   0 peisach    (502) staff       (20)    17365 2023-06-17 16:16:35.000000 onedep_deposition-0.1.dev1/onedep_deposition/models.py
--rw-r--r--   0 peisach    (502) staff       (20)     5349 2023-06-15 13:32:19.000000 onedep_deposition-0.1.dev1/onedep_deposition/rest_adapter.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-17 21:10:02.007434 onedep_deposition-0.1.dev1/onedep_deposition.egg-info/
--rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-17 21:10:01.000000 onedep_deposition-0.1.dev1/onedep_deposition.egg-info/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)      557 2023-06-17 21:10:01.000000 onedep_deposition-0.1.dev1/onedep_deposition.egg-info/SOURCES.txt
--rw-r--r--   0 peisach    (502) staff       (20)        1 2023-06-17 21:10:01.000000 onedep_deposition-0.1.dev1/onedep_deposition.egg-info/dependency_links.txt
--rw-r--r--   0 peisach    (502) staff       (20)       68 2023-06-17 21:10:01.000000 onedep_deposition-0.1.dev1/onedep_deposition.egg-info/entry_points.txt
--rw-r--r--   0 peisach    (502) staff       (20)       15 2023-06-17 21:10:01.000000 onedep_deposition-0.1.dev1/onedep_deposition.egg-info/requires.txt
--rw-r--r--   0 peisach    (502) staff       (20)       18 2023-06-17 21:10:01.000000 onedep_deposition-0.1.dev1/onedep_deposition.egg-info/top_level.txt
--rw-r--r--   0 peisach    (502) staff       (20)     1039 2023-06-17 17:50:36.000000 onedep_deposition-0.1.dev1/pyproject.toml
--rw-r--r--   0 peisach    (502) staff       (20)       38 2023-06-17 21:10:02.009249 onedep_deposition-0.1.dev1/setup.cfg
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 14:34:19.875651 onedep_deposition-0.1.dev2/
+-rw-r--r--   0 peisach    (502) staff       (20)      552 2023-06-13 13:04:02.000000 onedep_deposition-0.1.dev2/LICENSE
+-rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-19 14:34:19.875110 onedep_deposition-0.1.dev2/PKG-INFO
+-rw-r--r--   0 peisach    (502) staff       (20)     4641 2023-06-17 15:30:45.000000 onedep_deposition-0.1.dev2/README.md
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 14:34:19.870230 onedep_deposition-0.1.dev2/onedep_deposition/
+-rw-r--r--   0 peisach    (502) staff       (20)       25 2023-06-19 14:21:15.000000 onedep_deposition-0.1.dev2/onedep_deposition/__init__.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 14:34:19.874408 onedep_deposition-0.1.dev2/onedep_deposition/cli/
+-rw-r--r--   0 peisach    (502) staff       (20)        0 2023-06-17 17:42:03.000000 onedep_deposition-0.1.dev2/onedep_deposition/cli/__init__.py
+-rw-r--r--   0 peisach    (502) staff       (20)    12091 2023-06-17 17:38:06.000000 onedep_deposition-0.1.dev2/onedep_deposition/cli/cli.py
+-rw-r--r--   0 peisach    (502) staff       (20)    16794 2023-06-17 16:20:15.000000 onedep_deposition-0.1.dev2/onedep_deposition/constants.py
+-rw-r--r--   0 peisach    (502) staff       (20)    14441 2023-06-19 14:33:49.000000 onedep_deposition-0.1.dev2/onedep_deposition/deposit_api.py
+-rw-r--r--   0 peisach    (502) staff       (20)     9006 2023-06-15 13:32:19.000000 onedep_deposition-0.1.dev2/onedep_deposition/enum.py
+-rw-r--r--   0 peisach    (502) staff       (20)      159 2023-06-08 16:58:15.000000 onedep_deposition-0.1.dev2/onedep_deposition/exceptions.py
+-rw-r--r--   0 peisach    (502) staff       (20)    12949 2023-06-19 14:32:24.000000 onedep_deposition-0.1.dev2/onedep_deposition/models.py
+-rw-r--r--   0 peisach    (502) staff       (20)     5806 2023-06-19 14:21:05.000000 onedep_deposition-0.1.dev2/onedep_deposition/rest_adapter.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 14:34:19.873368 onedep_deposition-0.1.dev2/onedep_deposition.egg-info/
+-rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-19 14:34:19.000000 onedep_deposition-0.1.dev2/onedep_deposition.egg-info/PKG-INFO
+-rw-r--r--   0 peisach    (502) staff       (20)      557 2023-06-19 14:34:19.000000 onedep_deposition-0.1.dev2/onedep_deposition.egg-info/SOURCES.txt
+-rw-r--r--   0 peisach    (502) staff       (20)        1 2023-06-19 14:34:19.000000 onedep_deposition-0.1.dev2/onedep_deposition.egg-info/dependency_links.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       68 2023-06-19 14:34:19.000000 onedep_deposition-0.1.dev2/onedep_deposition.egg-info/entry_points.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       15 2023-06-19 14:34:19.000000 onedep_deposition-0.1.dev2/onedep_deposition.egg-info/requires.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       18 2023-06-19 14:34:19.000000 onedep_deposition-0.1.dev2/onedep_deposition.egg-info/top_level.txt
+-rw-r--r--   0 peisach    (502) staff       (20)     1039 2023-06-17 17:50:36.000000 onedep_deposition-0.1.dev2/pyproject.toml
+-rw-r--r--   0 peisach    (502) staff       (20)       38 2023-06-19 14:34:19.875802 onedep_deposition-0.1.dev2/setup.cfg
```

### Comparing `onedep_deposition-0.1.dev1/LICENSE` & `onedep_deposition-0.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev1/PKG-INFO` & `onedep_deposition-0.1.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedep_deposition
-Version: 0.1.dev1
+Version: 0.1.dev2
 Summary: Package for wrapping the OneDep deposition API services
 Author-email: Neli Jose da Fonseca Junior <neli@ebi.ac.uk>
 License: apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `onedep_deposition-0.1.dev1/README.md` & `onedep_deposition-0.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev1/onedep_deposition/cli/cli.py` & `onedep_deposition-0.1.dev2/onedep_deposition/cli/cli.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev1/onedep_deposition/constants.py` & `onedep_deposition-0.1.dev2/onedep_deposition/constants.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev1/onedep_deposition/deposit_api.py` & `onedep_deposition-0.1.dev2/onedep_deposition/deposit_api.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev1/onedep_deposition/enum.py` & `onedep_deposition-0.1.dev2/onedep_deposition/enum.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev1/onedep_deposition/models.py` & `onedep_deposition-0.1.dev2/onedep_deposition/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,34 +16,22 @@
         self._message = str(message)
         self._data = data if data else []
 
     @property
     def status_code(self) -> int:
         return self._status_code
 
-    @status_code.setter
-    def status_code(self, value: int):
-        self._status_code = int(value)
-
     @property
     def message(self) -> str:
         return self._message
 
-    @message.setter
-    def message(self, value: str):
-        self._message = str(value)
-
     @property
     def data(self) -> List[Dict]:
         return self._data
 
-    @data.setter
-    def data(self, value: List[Dict]):
-        self._data = value if value else []
-
     def __str__(self):
         """
         Override string parser
         :return: String text
         """
         return f"STATUS: {self._status_code}, MESSAGE: {self._message}\n{self._data}"
 
@@ -61,54 +49,38 @@
         """
         self._type = None
         self._subtype = None
         self._related_emdb = str(related_emdb) if related_emdb is not None else None
         self._related_bmrb = str(related_bmrb) if related_bmrb is not None else None
 
         if type(exp_type) == ExperimentType:
-            self.type = exp_type
+            self._type = exp_type
         elif exp_type:
-            self.type = ExperimentType(exp_type)
+            self._type = ExperimentType(exp_type)
         if type(subtype) == EMSubType:
-            self.subtype = subtype
+            self._subtype = subtype
         elif subtype:
-            self.subtype = EMSubType(subtype)
+            self._subtype = EMSubType(subtype)
 
     @property
     def type(self) -> Union[ExperimentType, None]:
         return self._type
 
-    @type.setter
-    def type(self, value: Union[ExperimentType, None]):
-        self._type = value
-
     @property
     def subtype(self) -> Union[EMSubType, None]:
         return self._subtype
 
-    @subtype.setter
-    def subtype(self, value: Union[EMSubType, None]):
-        self._subtype = value
-
     @property
     def related_emdb(self) -> str:
         return self._related_emdb
 
-    @related_emdb.setter
-    def related_emdb(self, value: str):
-        self._related_emdb = str(value)
-
     @property
     def related_bmrb(self) -> str:
         return self._related_bmrb
 
-    @related_bmrb.setter
-    def related_bmrb(self, value: str):
-        self._related_bmrb = str(value)
-
     def __str__(self):
         message = f"TYPE: {self._type}"
         if self.subtype:
             message += f" ({self._subtype})"
         if self.related_emdb:
             message += f" [{self._related_emdb}]"
         elif self.related_bmrb:
@@ -139,34 +111,22 @@
         self._message = str(message)
         self._extras = extras
 
     @property
     def code(self) -> str:
         return self._code
 
-    @code.setter
-    def code(self, value: str):
-        self._code = str(value)
-
     @property
     def message(self) -> str:
         return self._message
 
-    @message.setter
-    def message(self, value: str):
-        self._message = str(value)
-
     @property
     def extras(self) -> str:
         return self._extras
 
-    @extras.setter
-    def extras(self, value: str):
-        self._extras = value
-
     def json(self):
         json_object = self.__dict__.copy()
         json_object = {key[1:]: value for key, value in json_object.items() if value is not None}
         return json_object
 
     def __str__(self):
         return f"CODE: {self._code}, MESSAGE: {self._message}\nEXTRAS: {self._extras}"
@@ -214,98 +174,54 @@
             for error in errors:
                 self._errors.append(DepositError(**error))
 
     @property
     def email(self) -> str:
         return self._email
 
-    @email.setter
-    def email(self, value: str):
-        self._email = str(value)
-
     @property
     def dep_id(self) -> str:
         return self._id
 
-    @dep_id.setter
-    def dep_id(self, value: str):
-        self._id = str(value)
-
     @property
     def entry_id(self) -> str:
         return self._entry_id
 
-    @entry_id.setter
-    def entry_id(self, value: str):
-        self._entry_id = str(value)
-
     @property
     def title(self) -> str:
         return self._title
 
-    @title.setter
-    def title(self, value: str):
-        self._title = str(value)
-
     @property
     def created(self) -> datetime:
         return self._created
 
-    @created.setter
-    def created(self, value: str):
-        self._created = datetime.fromisoformat(value)
-
     @property
     def last_login(self) -> datetime:
         return self._last_login
 
-    @last_login.setter
-    def last_login(self, value: str):
-        self._last_login = datetime.fromisoformat(value)
-
     @property
     def site(self) -> str:
         return self._site
 
-    @site.setter
-    def site(self, value: str):
-        self._site = str(value)
-
     @property
     def status(self) -> Status:
         return self._status
 
-    @status.setter
-    def status(self, value: Status):
-        self._status = value
-
     @property
     def experiments(self) -> List[Experiment]:
         return self._experiments
 
-    @experiments.setter
-    def experiments(self, value: List[Experiment]):
-        self._experiments = value if value else []
-
     @property
     def errors(self) -> List[DepositError]:
         return self._errors
 
-    @errors.setter
-    def errors(self, value: List[DepositError]):
-        self._errors = value if value else []
-
     @property
     def site_url(self) -> str:
         return self._site_url
 
-    @site_url.setter
-    def site_url(self, value: str):
-        self._site_url = str(value)
-
     def __str__(self):
         experiments_text = [str(exp) for exp in self._experiments]
         return f"ID: {self._id}\nE-mail: {self._email}\nEntry ID: {self._entry_id}\nTitle: {self._title}\nCreated: {self._created}\nLast login: {self._last_login}\nSite: {self._site}\nStatus: {self._status}\nSite URL: {self._site_url}\nExperiments: {experiments_text}\nErrors: {self._errors}"  # noqa: E501
 
     def json(self):
         json_object = self.__dict__.copy()
         json_object = {key[1:]: value for key, value in json_object.items() if value is not None}
@@ -344,58 +260,34 @@
             for deposition in depositions:
                 self._depositions.append(**deposition)
 
     @property
     def orcid(self) -> str:
         return self._orcid
 
-    @orcid.setter
-    def orcid(self, value: str):
-        self._orcid = str(value)
-
     @property
     def id(self) -> int:
         return self._id
 
-    @id.setter
-    def id(self, value: int):
-        self._id = int(value)
-
     @property
     def full_name(self) -> str:
         return self._full_name
 
-    @full_name.setter
-    def full_name(self, value: str):
-        self._full_name = str(value)
-
     @property
     def last_login(self) -> datetime:
         return self._last_login
 
-    @last_login.setter
-    def last_login(self, value: str):
-        self._last_login = datetime.fromisoformat(value) if value else None
-
     @property
     def date_joined(self) -> datetime:
         return self._date_joined
 
-    @date_joined.setter
-    def date_joined(self, value: str):
-        self._date_joined = datetime.fromisoformat(value) if value else None
-
     @property
     def depositions(self) -> List[Deposit]:
         return self._depositions
 
-    @depositions.setter
-    def depositions(self, value: List[Deposit]):
-        self._depositions = value if value else []
-
     def __str__(self):
         return f"Name: {self._full_name} [{self._id}]\nORCID: {self._orcid}\nDate joined: {self._date_joined}\nLast login: {self._last_login}\nDepositions: {self._depositions}"
 
     def json(self):
         json_object = self.__dict__.copy()
         json_object = {key[1:]: value for key, value in json_object.items() if value is not None}
         json_object["depositions"] = []
@@ -443,62 +335,34 @@
 
         return message
 
     @property
     def id(self) -> int:
         return self._id
 
-    @id.setter
-    def id(self, value: int):
-        self._id = int(value)
-
     @property
     def created(self) -> datetime:
         return self._created
 
-    @created.setter
-    def created(self, value: str):
-        date_format = "%A, %B %d, %Y %H:%M:%S"
-        self._created = datetime.strptime(value, date_format)
-
     @property
     def name(self) -> str:
         return self._name
 
-    @name.setter
-    def name(self, value: str):
-        self._name = str(value)
-
     @property
     def file_type(self) -> FileType:
         return self._type
 
-    @file_type.setter
-    def file_type(self, value: Union[str, FileType]):
-        if isinstance(value, str):
-            self._type = FileType(value)
-        else:
-            self._type = value
-
     @property
     def errors(self) -> List[str]:
         return self._errors
 
-    @errors.setter
-    def errors(self, value: List[str]):
-        self._errors = [DepositError(**error) for error in value if error != ""] if value else []
-
     @property
     def warnings(self) -> List[str]:
         return self._warnings
 
-    @warnings.setter
-    def warnings(self, value: List[str]):
-        self._warnings = [warning for warning in value if warning != ""] if value else []
-
 
 class DepositedFilesSet:
     """
     Class representing a set of deposited files
     """
     def __init__(self, files: List[Dict], errors: List[str] = None, warnings: List[str] = None):
         """Constructor for deposited files set"""
@@ -529,34 +393,22 @@
             return item
         raise StopIteration
 
     @property
     def files(self) -> List[DepositedFile]:
         return self._files
 
-    @files.setter
-    def files(self, value: List[DepositedFile]):
-        self._files = value if value else []
-
     @property
     def errors(self) -> List[str]:
         return self._errors
 
-    @errors.setter
-    def errors(self, value: List[str]):
-        self._errors = [DepositError(**error) for error in value if error != ""] if value else []
-
     @property
     def warnings(self) -> List[str]:
         return self._warnings
 
-    @warnings.setter
-    def warnings(self, value: List[str]):
-        self._warnings = [warning for warning in value if warning != ""] if value else []
-
 
 class DepositStatus:
     def __init__(self, status: str, action: str, step: str, details: str, date: str):
         self._status = str(status)
         self._action = str(action)
         self._step = str(step)
         self._details = str(details)
@@ -565,42 +417,23 @@
     def __str__(self):
         return f"STATUS: {self._status}\nSTEP: {self._step}\nDATE: {self._date}\nACTION: {self._action}\nDETAILS: {self._details}"
 
     @property
     def status(self) -> str:
         return self._status
 
-    @status.setter
-    def status(self, value: str):
-        self._status = str(value)
-
     @property
     def action(self) -> str:
         return self._action
 
-    @action.setter
-    def action(self, value: str):
-        self._action = str(value)
-
     @property
     def step(self) -> str:
         return self._step
 
-    @step.setter
-    def step(self, value: str):
-        self._step = str(value)
-
     @property
     def details(self) -> str:
         return self._details
 
-    @details.setter
-    def details(self, value: str):
-        self._details = str(value)
-
     @property
     def date(self) -> datetime:
         return self._date
 
-    @date.setter
-    def date(self, value: str):
-        self._date = datetime.fromisoformat(value)
```

### Comparing `onedep_deposition-0.1.dev1/onedep_deposition/rest_adapter.py` & `onedep_deposition-0.1.dev2/onedep_deposition/rest_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,21 +16,40 @@
         :param api_key: (optional) string used for authentication when POSTing or DELETEing
         :param ver: always v1
         :param ssl_verify: Normally set to True, but if having SSL/TLS cert validation issues, can turn off with False
         :param timeout: (optional) Timeout in seconds for API calls
         :param logger: (optional) If your app has a logger, pass it in here.
         """
         self._logger = logger or logging.getLogger(__name__)
+        self._version = ver
+        self._hostname = hostname
         self.url = "{}/api/{}/".format(hostname, ver)
         self._api_key = api_key
         self._ssl_verify = ssl_verify
         self._timeout = timeout
         if not ssl_verify:
             requests.packages.urllib3.disable_warnings()  # pylint: disable=no-member
 
+    @property
+    def hostname(self) -> str:
+        """
+        Getter for hostname
+        :return: hostname
+        """
+        return self._hostname
+
+    @hostname.setter
+    def hostname(self, hostname: str) -> None:
+        """
+        Setter for hostname
+        :param hostname: hostname
+        :return: None
+        """
+        self.url = "{}/api/{}/".format(hostname, self._version)
+
     def _do(self, http_method: str, endpoint: str, params: Dict = None, data: Union[Dict, List] = None, files: Dict = None, content_type: str = "application/json") -> Response:
         """
         Private method to perform API calls
         :param http_method: GET/POST/DELETE
         :param endpoint: endpoint path
         :param params: Dictionary with requests params
         :param data: Dictionary with request data
```

### Comparing `onedep_deposition-0.1.dev1/onedep_deposition.egg-info/PKG-INFO` & `onedep_deposition-0.1.dev2/onedep_deposition.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedep-deposition
-Version: 0.1.dev1
+Version: 0.1.dev2
 Summary: Package for wrapping the OneDep deposition API services
 Author-email: Neli Jose da Fonseca Junior <neli@ebi.ac.uk>
 License: apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `onedep_deposition-0.1.dev1/onedep_deposition.egg-info/SOURCES.txt` & `onedep_deposition-0.1.dev2/onedep_deposition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev1/pyproject.toml` & `onedep_deposition-0.1.dev2/pyproject.toml`

 * *Files identical despite different names*

