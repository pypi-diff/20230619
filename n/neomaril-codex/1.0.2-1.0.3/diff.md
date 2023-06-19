# Comparing `tmp/neomaril-codex-1.0.2.tar.gz` & `tmp/neomaril-codex-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neomaril-codex-1.0.2.tar", last modified: Thu Apr 20 18:31:18 2023, max compression
+gzip compressed data, was "neomaril-codex-1.0.3.tar", last modified: Mon Jun 19 17:22:37 2023, max compression
```

## Comparing `neomaril-codex-1.0.2.tar` & `neomaril-codex-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-04-20 18:31:18.292173 neomaril-codex-1.0.2/
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1060 2023-03-06 17:55:16.000000 neomaril-codex-1.0.2/LICENSE.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       24 2023-03-13 13:54:26.000000 neomaril-codex-1.0.2/MANIFEST.in
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      359 2023-04-20 18:31:18.292173 neomaril-codex-1.0.2/PKG-INFO
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      618 2023-03-15 18:53:09.000000 neomaril-codex-1.0.2/README.md
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       59 2023-02-08 17:56:54.000000 neomaril-codex-1.0.2/requirements.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       79 2023-04-20 18:31:18.292173 neomaril-codex-1.0.2/setup.cfg
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      928 2023-04-20 18:30:27.000000 neomaril-codex-1.0.2/setup.py
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-04-20 18:31:18.288173 neomaril-codex-1.0.2/src/
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-04-20 18:31:18.292173 neomaril-codex-1.0.2/src/neomaril_codex/
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-02-08 17:56:54.000000 neomaril-codex-1.0.2/src/neomaril_codex/__init__.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    11916 2023-03-08 12:49:14.000000 neomaril-codex-1.0.2/src/neomaril_codex/base.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      755 2023-02-08 17:56:54.000000 neomaril-codex-1.0.2/src/neomaril_codex/exceptions.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     4487 2023-03-06 17:39:34.000000 neomaril-codex-1.0.2/src/neomaril_codex/logging.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    38969 2023-03-15 18:52:32.000000 neomaril-codex-1.0.2/src/neomaril_codex/model.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    12504 2023-03-08 12:49:14.000000 neomaril-codex-1.0.2/src/neomaril_codex/pipeline.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    28919 2023-04-20 18:30:54.000000 neomaril-codex-1.0.2/src/neomaril_codex/training.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      655 2023-03-07 18:36:14.000000 neomaril-codex-1.0.2/src/neomaril_codex/utils.py
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-04-20 18:31:18.292173 neomaril-codex-1.0.2/src/neomaril_codex.egg-info/
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      359 2023-04-20 18:31:18.000000 neomaril-codex-1.0.2/src/neomaril_codex.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      558 2023-04-20 18:31:18.000000 neomaril-codex-1.0.2/src/neomaril_codex.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-04-20 18:31:18.000000 neomaril-codex-1.0.2/src/neomaril_codex.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-02-07 14:57:39.000000 neomaril-codex-1.0.2/src/neomaril_codex.egg-info/not-zip-safe
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       60 2023-04-20 18:31:18.000000 neomaril-codex-1.0.2/src/neomaril_codex.egg-info/requires.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       15 2023-04-20 18:31:18.000000 neomaril-codex-1.0.2/src/neomaril_codex.egg-info/top_level.txt
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-19 17:22:37.341009 neomaril-codex-1.0.3/
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1060 2023-03-06 17:55:16.000000 neomaril-codex-1.0.3/LICENSE.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       24 2023-03-13 13:54:26.000000 neomaril-codex-1.0.3/MANIFEST.in
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1018 2023-06-19 17:22:37.341009 neomaril-codex-1.0.3/PKG-INFO
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      618 2023-03-15 18:53:09.000000 neomaril-codex-1.0.3/README.md
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       59 2023-02-08 17:56:54.000000 neomaril-codex-1.0.3/requirements.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       79 2023-06-19 17:22:37.341009 neomaril-codex-1.0.3/setup.cfg
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1028 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3/setup.py
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-19 17:22:37.337009 neomaril-codex-1.0.3/src/
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-19 17:22:37.341009 neomaril-codex-1.0.3/src/neomaril_codex/
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-02-08 17:56:54.000000 neomaril-codex-1.0.3/src/neomaril_codex/__init__.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    12206 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3/src/neomaril_codex/base.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      755 2023-02-08 17:56:54.000000 neomaril-codex-1.0.3/src/neomaril_codex/exceptions.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     4487 2023-03-06 17:39:34.000000 neomaril-codex-1.0.3/src/neomaril_codex/logging.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    44245 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3/src/neomaril_codex/model.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    12562 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3/src/neomaril_codex/pipeline.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    32065 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3/src/neomaril_codex/training.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      655 2023-03-07 18:36:14.000000 neomaril-codex-1.0.3/src/neomaril_codex/utils.py
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-19 17:22:37.341009 neomaril-codex-1.0.3/src/neomaril_codex.egg-info/
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1018 2023-06-19 17:22:37.000000 neomaril-codex-1.0.3/src/neomaril_codex.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      558 2023-06-19 17:22:37.000000 neomaril-codex-1.0.3/src/neomaril_codex.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-06-19 17:22:37.000000 neomaril-codex-1.0.3/src/neomaril_codex.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-02-07 14:57:39.000000 neomaril-codex-1.0.3/src/neomaril_codex.egg-info/not-zip-safe
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       60 2023-06-19 17:22:37.000000 neomaril-codex-1.0.3/src/neomaril_codex.egg-info/requires.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       15 2023-06-19 17:22:37.000000 neomaril-codex-1.0.3/src/neomaril_codex.egg-info/top_level.txt
```

### Comparing `neomaril-codex-1.0.2/LICENSE.txt` & `neomaril-codex-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.2/README.md` & `neomaril-codex-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.2/setup.py` & `neomaril-codex-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from os.path import join
 
 from setuptools import setup, find_packages
 
 MODULE_NAME = 'neomaril-codex'
 MODULE_NAME_IMPORT = 'neomaril_codex'
 REPO_NAME = 'mlops-neomaril-codex'
-MODULE_VERSION='1.0.2'
+MODULE_VERSION='1.0.3'
 
 def requirements_from_pip(filename='requirements.txt'):
     with open(filename, 'r') as pip:
         return [l.strip() for l in pip if not l.startswith('#') and l.strip()]
 
 
 setup(name=MODULE_NAME,
       description="Python tools for interact with Neomaril",
-      url='https://github.com/datarisk-io/{:s}'.format(REPO_NAME),
+      url='https://datarisk-io.github.io/mlops-neomaril-codex/',
       author="Datarisk",
+      long_description=open('README.md').read(),
+      long_description_content_type='text/markdown',
       package_dir={'': 'src'},
       packages=find_packages('src'),
       version=MODULE_VERSION,
       download_url=f'https://github.com/datarisk-io/mlops-neomaril-codex/archive/refs/tags/v{MODULE_VERSION}.tar.gz',
       install_requires=requirements_from_pip(),
       include_package_data=True,
       zip_safe=False,
```

### Comparing `neomaril-codex-1.0.2/src/neomaril_codex/base.py` & `neomaril-codex-1.0.3/src/neomaril_codex/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,24 +145,24 @@
 		bool
 			Returns True if the group was successfully created and False if not
 		"""
 		data = {"name": name, "description": description}
 
 		url = f"{self.base_url}/groups"
 		response = requests.post(url, data=data,
-														 headers={'Authorization': 'Bearer ' + self.__credentials})
+								headers={'Authorization': 'Bearer ' + self.__credentials})
 
 		if response.status_code == 201:
-				logger.info(response.json()['Message'])
-				return True
-		elif response.status_code == 400:
-				logger.error("Group already exist, nothing was changed.")
-				return False
+			logger.info(response.json()['Message'])
+			return True
+		elif response.status_code < 500:
+			logger.error("Group already exist, nothing was changed.")
+			return False
 		else:
-				raise ServerError('Unexpected server error: ', response.text)
+			raise ServerError('Unexpected server error: ', response.text)
 
 	def refresh_group_token(self, name:str, force:bool=False) -> bool:
 		"""
 		Refresh the group token. If the the token its still valid it wont be changed, unless you use parameter force = True.
 		At the end a message with the token for that group will be returned as a INFO message.
 		You should keep this new token information to be able to run the model of that group afterwards.
 
@@ -258,23 +258,25 @@
 			execution = model.predict(data_path+'input.csv')
 
 			execution.get_status()
 
 			execution.download_result()	
 	"""	
 
-	def __init__(self, parent_id:str, exec_type:str, group:Optional[str]=None, exec_id:Optional[str]=None, password:Optional[str]=None, url:str=None) -> None:
+	def __init__(self, parent_id:str, exec_type:str, group:Optional[str]=None, exec_id:Optional[str]=None, password:Optional[str]=None, url:str=None, group_token:Optional[str]=None) -> None:
 		super().__init__()
 		self.base_url = os.getenv('NEOMARIL_URL') if os.getenv('NEOMARIL_URL') else url
 		self.base_url = parse_url(self.base_url)
 		self.exec_type = exec_type
 		self.exec_id = exec_id
 		self.status = 'Requested'
+		self.group = group
 		load_dotenv()
 		self.__credentials = os.getenv('NEOMARIL_TOKEN') if os.getenv('NEOMARIL_TOKEN') else password
+		self.__token = os.getenv('NEOMARIL_GROUP_TOKEN') if os.getenv('NEOMARIL_GROUP_TOKEN') else group_token
 
 		try_login(self.__credentials, self.base_url)
 
 		if exec_type == 'AsyncModel':
 				self.__url_path = 'model/async'
 		elif exec_type == 'Training':
 				self.__url_path = 'training'
@@ -312,24 +314,25 @@
 
 		Returns
 		-------
 		dict
 			Returns the execution status.
 		"""
 
-		url = f"{self.base_url}/{self.__url_path}/status/{self.exec_id}"
-		response = requests.get(url, headers={'Authorization': 'Bearer ' + self.__credentials})
+		url = f"{self.base_url}/{self.__url_path}/status/{self.group}/{self.exec_id}"
+
+		response = requests.get(url, headers={'Authorization': 'Bearer ' + self.__token})
 		if response.status_code not in [200, 410]:
 				logger.error(response.text)
 				raise ExecutionError(f'Execution "{self.exec_id}" unavailable')
 
 		result = response.json()
 
 		self.status = result['Status']
-		self.execution_data['Status'] = result['Status']
+		self.execution_data['ExecutionState'] = result['Status']
 
 		return result
 
 	def download_result(self, path:Optional[str]='./') -> dict:
 		"""
 		Gets the output of the execution.
 
@@ -346,27 +349,32 @@
 		Returns
 		-------
 		dict
 			Returns the path for the result file.
 		"""
 		if self.status in ['Running', 'Requested']:
 			self.status = self.get_status()['Status']
+		
+		if self.exec_type == 'AsyncModel':
+			token = self.__token
+		elif self.exec_type == 'Training':
+			token = self.__credentials
 
 		if self.status == 'Succeeded':
-				url = f"{self.base_url}/{self.__url_path}/result/{self.exec_id}"
-				response = requests.get(url, headers={'Authorization': 'Bearer ' + self.__credentials})
+				url = f"{self.base_url}/{self.__url_path}/result/{self.group}/{self.exec_id}"
+				response = requests.get(url, headers={'Authorization': 'Bearer ' + token})
 				if response.status_code not in [200, 410]:
 						logger.error(response.text)
 						raise ExecutionError(f'Execution "{self.exec_id}" unavailable')
 
 				filename = f'output_{self.exec_id}.zip'
 				if not path.endswith('/'):
 						filename = '/'+filename
 
 				with open(path+filename, 'wb') as f:
 						f.write(response.content)
 
 				logger.info(f'Output saved in {path+filename}')
 		elif self.status == 'Failed':
-				raise ExecutionError("Execution failed")
+			raise ExecutionError("Execution failed")
 		else:
-				logger.info(f'Execution not ready. Status is {self.status}')
+			logger.info(f'Execution not ready. Status is {self.status}')
```

### Comparing `neomaril-codex-1.0.2/src/neomaril_codex/exceptions.py` & `neomaril-codex-1.0.3/src/neomaril_codex/exceptions.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.2/src/neomaril_codex/logging.py` & `neomaril-codex-1.0.3/src/neomaril_codex/logging.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.2/src/neomaril_codex/model.py` & `neomaril-codex-1.0.3/src/neomaril_codex/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,27 @@
 
 class NeomarilModel(BaseNeomaril):
     """
     Class to manage Models deployed inside Neomaril
 
     Attributes
     ----------
-	password : str
-		Password for authenticating with the client. You can also use the env variable NEOMARIL_TOKEN to set this
-    model_id: str
+    password : str
+        Password for authenticating with the client. You can also use the env variable NEOMARIL_TOKEN to set this
+    model_id : str
         Model id (hash) from the model you want to access
     group : str
         Group the model is inserted. Default is 'datarisk' (public group)
     group_token : str
         Token for executing the model (show when creating a group). It can be informed when getting the model or when running predictions, or using the env variable NEOMARIL_GROUP_TOKEN
-	url : str
+    url : str
 		URL to Neomaril Server. Default value is https://neomaril.staging.datarisk.net, use it to test your deployment first before changing to production. You can also use the env variable NEOMARIL_URL to set this
-
+    docs : str
+        URL for the model Swagger page
+    
     Raises
     ------
     ModelError
         When the model can't be acessed in the server
     AuthenticationError
         Unvalid credentials
 
@@ -51,14 +53,15 @@
         if model.health() = 'OK':
             model.wait_ready()
             model.predict(model.schema)
         else:
             model.restart_model(False)
             model.wait_ready()
             model.predict(model.schema)
+    
     """
 
     def __init__(self, model_id:str, password:Optional[str]=None, group:str="datarisk", group_token:Optional[str]=None, url:str='https://neomaril.staging.datarisk.net/') -> None:
 
         load_dotenv()
         logger.info('Loading .env')
 
@@ -83,14 +86,17 @@
             raise ModelError(f'Unable to retrive model "{model_id}"')
     
         self.model_data = response.json()['Description']
         self.name = self.model_data['Name']
         self.status = self.model_data['Status']
         self.schema = self.model_data['Schema']
         self.operation = self.model_data['Operation'].lower()
+        self.docs = f'{self.base_url}/model/{self.operation}/docs/{self.group}/{self.model_id}'
+        if self.operation == 'sync':
+            self.docs = self.docs.replace('localhost:7070', 'localhost:7071') 
         self.__model_ready = self.status == "Deployed"
 
     def __repr__(self) -> str:
         return f"""NeomarilModel(name="{self.name}", group="{self.group}", 
                                 status="{self.status}",
                                 model_id="{self.model_id}",
                                 operation="{self.operation.title()}",
@@ -114,31 +120,31 @@
 		str
             The model status
 
 		"""
         url = f"{self.base_url}/model/status/{self.group}/{self.model_id}"
         response = requests.get(url, headers={'Authorization': 'Bearer ' + self.__credentials})
         if response.status_code < 300:
-            return response.json()['Status']
+            return response.json()
         else:
             raise ModelError(response.text)
 
     def wait_ready(self):
         """
-        Waits the model to be with status 'Ready'
+        Waits the model to be with status 'Deployed'
         
         Example
         -------
         >>> model.wait_ready()
         """
         if self.status in ['Ready', 'Building']:
-            self.status = self.__get_status()
+            self.status = self.__get_status()['Status']
             while self.status == 'Building':
                 sleep(30)
-                self.status = self.__get_status()
+                self.status = self.__get_status()['Status']
 
     def health(self) -> str:
         """
         Get the model deployment process health state.
 
         Returns
         -------
@@ -181,20 +187,20 @@
         >>> model.restart_model()
         """
         if (self.operation == "sync") and (self.status == "Deployed"):
             url = f"{self.base_url.replace('localhost:7070', 'localhost:7071')}/model/sync/restart/{self.group}/{self.model_id}"
             response = requests.get(url, headers={'Authorization': 'Bearer ' + self.__credentials})
             if response.status_code < 300:
                 logger.info("Model is restarting")
-                self.status = self.__get_status()
+                self.status = self.__get_status()['Status']
                 if wait_for_ready:
                     print('Wating for deploy to be ready.', end='')
                     while self.status == 'Building':
                         sleep(30)
-                        self.status = self.__get_status()
+                        self.status = self.__get_status()['Status']
                         print('.', end='', flush=True)
 
     def get_logs(self, start:Optional[str]=None, end:Optional[str]=None, routine:Optional[str]=None, type:Optional[str]=None):
         """
         Get the logs 
 
         Parameters
@@ -202,15 +208,15 @@
         start : str, optional
             Date to start filter. At the format aaaa-mm-dd
         end : str, optional
             Date to end filter. At the format aaaa-mm-dd
         routine : str, optional
             Type of routine beeing executed, can assume values Host or Run
         type : str, optional
-            Defines the type of the logs that are going to be filtered, can assume the vaues Ok, Error, Debug or Warning
+            Defines the type of the logs that are going to be filtered, can assume the values Ok, Error, Debug or Warning
 
         Raises
         ------
         ServerError    
             Unexpected server error
 
         Returns
@@ -310,16 +316,18 @@
         -------
         Union[dict, NeomarilExecution]
             The return of the scoring function in the source file for Sync models or the execution class for Async models.
         """
         if self.__model_ready:
             if (group_token is not None) | (self.__token is not None):
                 url = f"{self.base_url}/model/{self.operation}/run/{self.group}/{self.model_id}"
-                if self.__token:
+                if self.__token and not group_token:
                     group_token = self.__token
+                if group_token and not self.__token:
+                    self.__token = group_token
                 if self.operation == 'sync':
                     url = url.replace('localhost:7070', 'localhost:7071')
                     model_input = {
                             "Input": data
                     }
 
                     req = requests.post(url, data=json.dumps(model_input), headers={'Authorization': 'Bearer ' + group_token})
@@ -332,23 +340,27 @@
                                                     headers={'Authorization': 'Bearer ' + group_token})
 
                     if req.status_code == 202:
                         message = req.json()
                         logger.info(message['Message'])
                         exec_id = message['ExecutionId']
                         run = NeomarilExecution(self.model_id, 'AsyncModel', exec_id=exec_id, password=self.__credentials, 
-                                                url=self.base_url, group=self.group)
-                        status = run.get_status()['Status']
+                                                url=self.base_url, group=self.group, group_token=group_token)
+                        response = run.get_status()
+                        status = response['Status']
                         if wait_complete:
                             print('Wating the training run.', end='')
                             while status in ['Running', 'Requested']:
                                 sleep(30)
                                 print('.', end='', flush=True)
-                                status = run.get_status()['Status']
-                        return run
+                                response = run.get_status()
+                                status = response['Status']
+                        if status == 'Failed':
+                            logger.error(response['Message'])
+                            raise ExecutionError("Training execution failed")
                     else:
                         raise ServerError(req.text)
                 
             else:
                 raise AuthenticationError("Group token not informed")
         else:
             url = f"{self.base_url}/model/describe/{self.group}/{self.model_id}"
@@ -357,14 +369,125 @@
                 self.model_data = response
                 self.status = response['Status']
                 self.__model_ready = True
                 return self.predict(data)
     
             else:
                 raise ModelError('Model is not available to predictions')
+            
+    def generate_predict_code(self, language:str='curl') -> str:
+        """
+        Generates predict code for the model to be used outside Neomaril Codex
+
+        Arguments
+        ---------
+        language : str
+            The generated code language. Supported languages are 'curl', 'python' or 'javascript'
+
+        Raises
+        ------
+        InputError
+            Unsupported language
+
+        Returns
+        -------
+        str
+            The generated code.
+        """
+        if language not in ['curl', 'python', 'javascript']:
+            raise InputError("Suported languages are curl, python or javascript")
+
+        if self.operation == 'sync':
+            payload = json.dumps({"Input": self.schema})
+            base_url = self.base_url.replace('localhost:7070', 'localhost:7071') 
+            if language == 'curl':
+                return f"""curl --request POST \\
+                    --url {base_url}/model/sync/run/{self.group}/{self.model_id} \\
+                    --header 'Authorization: Bearer {self.__token}' \\
+                    --header 'Content-Type: application/json' \\
+                    --data '{payload}'
+                """
+            if language == 'python':
+                return f"""
+                    import requests
+
+                    url = "{base_url}/model/sync/run/{self.group}/{self.model_id}"
+
+                    payload = {payload}
+                    headers = {{
+                        "Content-Type": "application/json",
+                        "Authorization": "Bearer {self.__token}"
+                    }}
+
+                    response = requests.request("POST", url, json=payload, headers=headers)
+
+                    print(response.text)
+                """
+            if language == 'javascript':
+                return f"""
+                    const options = {{
+                    method: 'POST',
+                    headers: {{'Content-Type': 'application/json', Authorization: 'Bearer {self.__token}'}},
+                    body: '{payload}'
+                    }};
+
+                    fetch('{base_url}/model/sync/run/{self.group}/{self.model_id}', options)
+                    .then(response => response.json())
+                    .then(response => console.log(response))
+                    .catch(err => console.error(err));
+
+                """
+        if self.operation == 'async':
+            if language == 'curl':
+                return f"""
+                    curl --request POST \
+                    --url {self.base_url}/model/async/run/{self.group}/{self.model_id} \\
+                    --header 'Authorization: Bearer {self.__token}' \\
+                    --header 'Content-Type: multipart/form-data' \\
+                    --form "input=@/path/to/file"
+                """
+            if language == 'python':
+                return f"""
+                    import requests
+
+                    url = "{self.base_url}/model/async/run/{self.group}/{self.model_id}"
+
+                    upload_data = [
+                        ("input", ('filename', open('/path/to/file', 'r'))),
+                    ]
+
+                    headers = {{
+                        "Content-Type": "multipart/form-data",
+                        "Authorization": "Bearer {self.__token}"
+                    }}
+
+                    response = requests.request("POST", url, files=upload_data, headers=headers)
+
+                    print(response.text)
+                """
+            if language == 'javascript':
+                return f"""
+                    const form = new FormData();
+                    form.append("input", "/path/to/file");
+
+                    const options = {{
+                    method: 'POST',
+                    headers: {{
+                        'Content-Type': 'multipart/form-data',
+                        Authorization: 'Bearer {self.__token}'
+                    }}
+                    }};
+
+                    options.body = form;
+
+                    fetch('{self.base_url}/model/async/run/{self.group}/{self.model_id}', options)
+                    .then(response => response.json())
+                    .then(response => console.log(response))
+                    .catch(err => console.error(err));
+                """
 
     def __call__(self, data: dict) -> dict:
         return self.predict(data)
 
     def get_model_execution(self, exec_id:str) -> None:
         """
         Get a execution instace for that model.
@@ -385,26 +508,26 @@
         """
         if self.operation == 'async':
             return NeomarilExecution(self.model_id, 'AsyncModel', exec_id, password=self.__credentials, 
                                      url=self.base_url, group=self.group)
         else:
             raise ModelError("Sync models don't have executions")
 
-    def register_monitoring(self, preprocess_reference:str, shap_reference:str, configuration_file:str, preprocess_file:Optional[str]=None,
+    def register_monitoring(self, preprocess_reference:str, shap_reference:str, configuration_file:Union[str, dict], preprocess_file:Optional[str]=None,
                             requirements_file:Optional[str]=None) -> str:
         """
         Register the model monitoring configuration at the database
 
         Arguments
         ---------
         preprocess_reference : str
             Name of the preprocess reference
         shap_reference : str
             Name of the preprocess function
-        configuration_file : str
+        configuration_file : str or dict
             Path of the configuration file, but it could be a dict
         preprocess_file : str, optional
             Path of the preprocess script
         requirements_file : str
             Path of the requirements file
 
 
@@ -420,16 +543,21 @@
 
         Example
         -------
         >>> model.register_monitoring('parse', 'get_shap', configuration_file=PATH+'configuration.json', preprocess_file=PATH+'preprocess.py', requirements_file=PATH+'requirements.txt')
         """
         url = f"{self.base_url}/monitoring/register/{self.group}/{self.model_id}"
     
+        if isinstance(configuration_file, str):
+            conf = open(configuration_file, "r")
+        elif isinstance(configuration_file, dict):
+            conf = json.dumps(configuration_file)
+
         upload_data = [
-            ("configuration", ('conf.json', open(configuration_file, "r"))),
+            ("configuration", ('conf.json', conf)),
         ]
 
         form_data = {'preprocess_reference': preprocess_reference, 'shap_reference': shap_reference}
 
         if preprocess_file:
             upload_data.append(("source", ('preprocess.'+preprocess_file.split('.')[-1], open(preprocess_file, "r"))))
             
@@ -640,19 +768,21 @@
         
         status = response['Status']
         
         if status == 'Building':
             if wait_for_ready:
                 print('Wating for deploy to be ready.', end='')
                 while status == 'Building':
-                    status = self.__get_model_status(model_id, group)['Status']
+                    response = self.__get_model_status(model_id, group)
+                    status = response['Status']
                     print('.', end='', flush=True)
                     sleep(10)
             else:
-                raise ModelError(f'Model "{model_id}" not ready yet')
+                logger.info("Returning model, but model is not ready.")
+                NeomarilModel(model_id, password=self.__credentials, group=group, url=self.base_url, group_token=group_token)
             
         if status in ['Disabled', 'Ready']:
             raise ModelError(f'Model "{model_id}" unavailable (disabled or deploy process is incomplete)')
         elif status == 'Failed':
             logger.error(str(response['Message']))
             raise ModelError(f'Model "{model_id}" deploy failed, so model is unavailable.')
         elif status == 'Deployed': 
@@ -684,15 +814,15 @@
 
         Returns
         -------
         list
             List with the models data, it can works like a filter depending on the arguments values
         Example
         -------
-        >>> model.search_models(group='ex_group', only_deployed=True)
+        >>> client.search_models(group='ex_group', only_deployed=True)
         """
         url = f"{self.base_url}/model/search"
 
         query = {}
 
         if name:
             query['name'] = name
@@ -730,17 +860,17 @@
         model_id : str
             Model id (hash)
         start : str, optional
             Date to start filter. At the format aaaa-mm-dd
         end : str, optional
             Date to end filter. At the format aaaa-mm-dd
         routine : str, optional
-            Type of routine beeing executed, can assume values Host or Run
+            Type of routine being executed, can assume values 'Host' (for deployment logs) or 'Run' (for execution logs)
         type : str, optional
-            Defines the type of the logs that are going to be filtered, can assume the vaues Ok, Error, Debug or Warning
+            Defines the type of the logs that are going to be filtered, can assume the values 'Ok', 'Error', 'Debug' or 'Warning'
 
         Raises
         ------
         ServerError    
             Unexpected server error
 
         Returns
@@ -820,16 +950,16 @@
 
         if operation=="Sync":
             input_type = "json"
             if schema:
                 if isinstance(schema, str):
                     schema_file = open(schema, "r")
                 elif isinstance(schema, dict):
-                    schema_file = io.StringIO()
-                    json.dump(schema, schema_file).seek(0)
+                    schema_file = json.dumps(schema)
+                    
                 upload_data.append(("schema", ("schema.json", schema_file)))
             else:
                 raise InputError("Schema file is mandatory for Sync models")
 
         else:
             if input_type == 'json|csv|parquet':
                 raise InputError("Choose a input type from "+input_type)
@@ -957,22 +1087,20 @@
         model_id = self.__upload_model(model_name, model_reference, source_file, 
                                                 model_file, requirements_file, schema=schema, group=group,
                                                 extra_files=extra_files, python_version=python_version,env=env,
                                                 operation=operation, input_type=input_type)
                 
         self.__host_model(operation.lower(), model_id, group)
         
-        if wait_for_ready:
-            return self.get_model(model_id, group)
-        else:
-            return "Model deployment in progress"
+        return self.get_model(model_id, group, wait_for_ready=wait_for_ready)
+   
 
     def get_model_execution(self, model_id:str, exec_id:str, group:Optional[str]=None) -> NeomarilExecution:
         """
-        Get a execution instace.
+        Get a execution instace (Async model only).
 
         Arguments
         ---------
         model_id : str
             Model id (hash)
         exec_id : str
             Execution id
@@ -984,8 +1112,8 @@
         NeomarilExecution
             The new execution
         
         Example
         -------
         >>> model.get_model_execution( model_id='M9c3af308c754ee7b96b2f4a273984414d40a33be90242908f9fc4aa28ba8ec4', exec_id = '1')
         """
-        return NeomarilExecution(model_id,'AsyncModel', exec_id, password=self.__credentials, url=self.base_url, group=group)
+        return self.get_model(model_id=model_id, group=group).get_model_execution(exec_id)
```

### Comparing `neomaril-codex-1.0.2/src/neomaril_codex/pipeline.py` & `neomaril-codex-1.0.3/src/neomaril_codex/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,16 +117,18 @@
 
         load_dotenv()
         logger.info('Loading .env')
 
         token = os.getenv("NEOMARIL_TOKEN")
         if not token:
             raise PipelineError("When using a config file the environment variable NEOMARIL_TOKEN must be defined")
+        
+        url = os.getenv('NEOMARIL_URL', conf.get('url'))
 
-        pipeline = NeomarilPipeline(conf['group'], password=token, url=conf['url'], python_version=conf['python_version'])
+        pipeline = NeomarilPipeline(conf['group'], password=token, url=url, python_version=conf['python_version'])
 
         if 'training' in conf.keys():
             pipeline.register_train_config(**conf['training'])
 
         if 'deploy' in conf.keys():
             pipeline.register_deploy_config(**conf['deploy'])
```

### Comparing `neomaril-codex-1.0.2/src/neomaril_codex/training.py` & `neomaril-codex-1.0.3/src/neomaril_codex/training.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 import io
 import re
-from typing import Union, Optional
+from typing import Union, Optional, List
 import requests
 import json
 from time import sleep
 from neomaril_codex.base import *
 from neomaril_codex.model import NeomarilModel
 from neomaril_codex.utils import *
 from neomaril_codex.exceptions import *
 
 patt = re.compile(r'(\d+)')
 
 class NeomarilTrainingExecution(NeomarilExecution):
     """
     Class to manage trained models.
 
-    Arguments
-    ---------
+    Attributes
+    ----------
     training_id : str
         Training id (hash) from the experiment you want to access
     group : str
         Group the training is inserted. Default is 'datarisk' (public group)
     exec_id : str
         Executiong id for that especific training run
     password : str
         Password for authenticating with the client
     environment : str
         Enviroment of Neomaril you are using. 
+    run_data : dict
+        Metadata from the execution. 
 
     Raises
     ------
     TrainingError
         When the training can't be acessed in the server
     AuthenticationError
         Unvalid credentials
@@ -54,26 +56,27 @@
         data_path = './samples/train/'
 
         run = training.run_training('First test', data_path+'dados.csv', training_reference='train_model', python_version='3.9', requirements_file=data_path+'requirements.txt', wait_complete=True)
         
         print(run.get_training_execution(run.exec_id))
         print(run.download_result())
 
-        run.promote('Teste notebook promoted custom', 'score', data_path+'app.py', data_path+'schema.json',  'csv')
+        run.promote_model('Teste notebook promoted custom', 'score', data_path+'app.py', data_path+'schema.json',  'csv')
     """
 
     def __init__(self, training_id:str, group:str, exec_id:str, password:Optional[str]=None, url:str=None) -> None:
         super().__init__(training_id, 'Training', exec_id=exec_id, password=password, url=url, group=group)
         load_dotenv()
         self.__credentials = os.getenv('NEOMARIL_TOKEN') if os.getenv('NEOMARIL_TOKEN') else password
 
         self.training_id = training_id
         self.group = group
     
         self.training_type = self.execution_data['TrainingType']
+        self.run_data = self.execution_data['RunData']
 
     def __upload_model(self, model_name:str, model_reference:Optional[str]=None, source_file:Optional[str]=None, 
                                          schema:Optional[Union[str, dict]]=None, extra_files:Optional[list]=None, 
                                          env:Optional[str]=None, operation:str='Sync', input_type:str=None) -> str:
         """
         Upload the files to the server
 
@@ -158,14 +161,48 @@
             data = response.json()
             model_id = data["ModelHash"]
             logger.info(f'{data["Message"]} - Hash: "{model_id}"')
             return model_id
         else:
             logger.error('Upload error: ' + response.text)
             raise InputError('Invalid parameters for model creation')
+        
+    def get_status(self) -> dict:
+        """
+		Gets the status of the related execution.
+
+		Raises
+		------
+		ExecutionError
+			Execution unavailable
+
+		Returns
+		-------
+		dict
+			Returns the execution status.
+		"""
+
+        url = f"{self.base_url}/training/status/{self.group}/{self.exec_id}"
+
+        response = requests.get(url, headers={'Authorization': 'Bearer ' + self.__credentials})
+        if response.status_code not in [200, 410]:
+            logger.error(response.text)
+            raise ExecutionError(f'Execution "{self.exec_id}" unavailable')
+
+        result = response.json()
+
+        self.status = result['Status']
+        self.execution_data['ExecutionState'] = result['Status']
+        if self.status == 'Succeeded':
+            url = f"{self.base_url}/training/describe/{self.group}/{self.training_id}/{self.exec_id}"
+            response = requests.get(url, headers={'Authorization': 'Bearer ' + self.__credentials})
+            self.execution_data = response.json()['Description']
+            self.run_data = self.execution_data['RunData']
+            del self.run_data['tags']
+        return result
 
     def __host_model(self, operation:str, model_id:str) -> None:
         """
         Builds the model execution environment
 
         Arguments
         ----------
@@ -245,24 +282,27 @@
             return NeomarilModel(model_id, password=self.__credentials, group=self.group, url=self.base_url)
 
         
 class NeomarilTrainingExperiment(BaseNeomaril):
     """
     Class to manage models being trained inside Neomaril
 
-    Arguments
-    ---------
+    Attributes
+    ----------
     password : str
         Password for authenticating with the client
     training_id : str
         Training id (hash) from the experiment you want to access
     group : str
         Group the training is inserted. Default is 'datarisk' (public group)
     environment : str
         Flag that choose which environment of Neomaril you are using. Test your deployment first before changing to production. Default is True
+    executions : List[int]
+        Ids for the executions in that training
+
 
     Raises
     ------
     TrainingError
         When the training can't be acessed in the server
     AuthenticationError
         Unvalid credentials
@@ -308,14 +348,15 @@
         elif response.status_code >= 500:
             raise ModelError(f'Unable to retrive experiment "{training_id}"')
     
         self.training_data = response.json()['Description']
         self.model_type = self.training_data['ModelType']
         self.training_type = self.training_data['TrainingType']
         self.experiment_name = self.training_data['ExperimentName']
+        self.executions = self.training_data['Executions']
 
     def __repr__(self) -> str:
             return f"""NeomarilTrainingExperiment(name="{self.experiment_name}", 
                                                         group="{self.group}", 
                                                         training_id="{self.training_id}",
                                                         training_type="{self.training_type}",
                                                         model_type={str(self.model_type)}
@@ -428,14 +469,27 @@
         url = f"{self.base_url}/training/execute/{self.group}/{self.training_id}/{exec_id}"
         response = requests.get(url, headers={'Authorization': 'Bearer ' + self.__credentials})
         if response.status_code == 200:
             logger.info(f"Model training starting - Hash: {self.training_id}")
         else:
             logger.error(response.text)
             raise InputError('Invalid parameters for training execution')
+        
+    def __refresh_execution_list(self):
+        url = f"{self.base_url}/training/describe/{self.group}/{self.training_id}"
+        response = requests.get(url, headers={'Authorization': 'Bearer ' + self.__credentials})
+    
+        if response.status_code == 404:
+            raise ModelError(f'Experiment "{self.training_id}" not found.')
+            
+        elif response.status_code >= 500:
+            raise ModelError(f'Unable to retrive experiment "{self.training_id}"')
+    
+        self.training_data = response.json()['Description']
+        self.executions = self.training_data['Executions']
 
     def run_training(self, run_name:str, train_data:str, training_reference:Optional[str]=None, 
                      python_version:str='3.8', conf_dict:Optional[Union[str, dict]]=None,
                      source_file:Optional[str]=None, requirements_file:Optional[str]=None,
                      extra_files:Optional[list]=None, wait_complete:Optional[bool]=False) -> Union[dict, NeomarilExecution]:
         """
         Runs a prediction from the current model.
@@ -487,49 +541,80 @@
             exec_id = self.__upload_training(run_name, train_data, conf_dict=conf_dict)
 
         else:
             raise InputError('Invalid training type')
 
         if exec_id:
             self.__execute_training(exec_id)
+            self.__refresh_execution_list()
             run = NeomarilTrainingExecution(self.training_id, self.group, exec_id, password=self.__credentials, url=self.base_url)
-            status = run.get_status()['Status']
+            response = run.get_status()
+            status = response['Status']
             if wait_complete:
                 print('Wating the training run.', end='')
                 while status in ['Running', 'Requested']:
                     sleep(30)
                     print('.', end='', flush=True)
-                    status = run.get_status()['Status']
-            return run
+                    response = run.get_status()
+                    status = response['Status']
+            if status == 'Failed':
+                logger.error(response['Message'])
+                raise ExecutionError("Training execution failed")
+            else:
+                return run
 
     def __call__(self, data: dict) -> dict:
             return self.predict(data)
 
-    def get_training_execution(self, exec_id:str) -> None:
+    def get_training_execution(self, exec_id:Optional[str]=None) -> NeomarilTrainingExecution:
         """
         Get a execution instace.
 
         Arguments
         ---------
-        exec_id : str
-            Execution id
+        exec_id : str, optional
+            Execution id. If not informed we get the last execution.
 
         Returns
         -------
         NeomarilExecution
-            The new execution
+            The choosen execution
         """
-        return NeomarilTrainingExecution(self.training_id, self.group, exec_id, password=self.__credentials, url=self.base_url)
+        if not exec_id:
+            self.__refresh_execution_list()
+            logger.info("Execution id not informed. Getting last execution")
+            exec_id = max(self.executions)
+        try:
+            int(exec_id)
+        except:
+            InputError("Unvalid execution Id informed or this training dont have a successful execution yet.")
+
+        exec = NeomarilTrainingExecution(self.training_id, self.group, exec_id, password=self.__credentials, url=self.base_url)
+        exec.get_status()
+        
+        return exec
+
+    def get_all_training_executions(self) -> List[NeomarilTrainingExecution]:
+        """
+        Get all executions from that experiment.
+
+        Returns
+        -------
+        List[NeomarilExecution]
+            All executions from that training
+        """
+        self.__refresh_execution_list()
+        return [self.get_training_execution(e) for e in self.executions]
 
 class NeomarilTrainingClient(BaseNeomarilClient):
     """
     Class for client for acessing Neomaril and manage models
 
-    Arguments
-    ---------
+    Attributes
+    ----------
 	password : str
 		Password for authenticating with the client. You can also use the env variable NEOMARIL_TOKEN to set this
 	url : str
 		URL to Neomaril Server. Default value is https://neomaril.staging.datarisk.net, use it to test your deployment first before changing to production. You can also use the env variable NEOMARIL_URL to set this
 
     Raises
     ------
@@ -661,17 +746,17 @@
         url = f"{self.base_url}/training/register/{group}"
 
         data = {'experiment_name': experiment_name, 'model_type': model_type, 'training_type': training_type}
 
         response = requests.post(url, data=data,
                                                          headers={'Authorization': 'Bearer ' + self.__credentials})
 
-        if response.status_code == 200:
-            message = response.json()['Message']
-            logger.info(message)
-            training_id = message.replace('New Training inserted with hash ', '').replace('.', '')
+        if response.status_code < 300:
+            response_data = response.json()
+            logger.info(response_data['Message'])
+            training_id = response_data['TrainingHash']
         else:
             logger.error(response.text)
             raise ServerError('')
 
         
         return NeomarilTrainingExperiment(training_id, password=self.__credentials, group=group, url=self.base_url)
```

### Comparing `neomaril-codex-1.0.2/src/neomaril_codex/utils.py` & `neomaril-codex-1.0.3/src/neomaril_codex/utils.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.2/src/neomaril_codex.egg-info/SOURCES.txt` & `neomaril-codex-1.0.3/src/neomaril_codex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

