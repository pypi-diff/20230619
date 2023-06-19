# Comparing `tmp/IMDBTraktSyncer-1.5.0.tar.gz` & `tmp/IMDBTraktSyncer-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.5.0.tar", last modified: Mon Jun 19 09:53:46 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.5.1.tar", last modified: Mon Jun 19 16:13:11 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.5.0.tar` & `IMDBTraktSyncer-1.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 09:53:46.226639 IMDBTraktSyncer-1.5.0/
-drwxrwxrwx   0        0        0        0 2023-06-19 09:53:46.192153 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    35301 2023-06-19 09:48:35.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     6693 2023-06-19 09:47:56.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1511 2023-06-19 08:07:22.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0    10221 2023-06-19 09:48:14.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0    10353 2023-06-19 09:48:23.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0    12076 2023-06-19 09:48:05.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:53:46.223152 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    12155 2023-06-19 09:53:46.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-06-19 09:53:46.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 09:53:46.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-19 09:53:46.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-06-19 09:53:46.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-19 09:53:46.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.5.0/LICENSE
--rw-rw-rw-   0        0        0    12155 2023-06-19 09:53:46.225183 IMDBTraktSyncer-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0    11409 2023-06-19 09:51:38.000000 IMDBTraktSyncer-1.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 09:53:46.227154 IMDBTraktSyncer-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1377 2023-06-19 09:52:05.000000 IMDBTraktSyncer-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:13:11.126736 IMDBTraktSyncer-1.5.1/
+drwxrwxrwx   0        0        0        0 2023-06-19 16:13:11.093737 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    35208 2023-06-19 16:10:38.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     6693 2023-06-19 09:47:56.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1797 2023-06-19 16:10:23.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0    10221 2023-06-19 09:48:14.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0    10353 2023-06-19 09:48:23.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0    12192 2023-06-19 15:47:42.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:13:11.123746 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12155 2023-06-19 16:13:10.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-06-19 16:13:10.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 16:13:10.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-19 16:13:10.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-06-19 16:13:10.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-19 16:13:10.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0    12155 2023-06-19 16:13:11.125747 IMDBTraktSyncer-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11409 2023-06-19 09:51:38.000000 IMDBTraktSyncer-1.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 16:13:11.126736 IMDBTraktSyncer-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-06-19 16:12:51.000000 IMDBTraktSyncer-1.5.1/setup.py
```

### Comparing `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import json
 import requests
 import time
-import logging
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import NoSuchElementException, TimeoutException, StaleElementReferenceException
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
@@ -34,17 +33,15 @@
     try:
 
         #Get credentials
         imdb_username = VC.imdb_username
         imdb_password = VC.imdb_password
         
         directory = os.path.dirname(os.path.realpath(__file__))
-        
-        logging.getLogger('selenium.webdriver').setLevel(logging.WARNING)
-        
+                
         #Start web driver
         print('Starting webdriver...')
         options = Options()
         options.add_argument("--headless=new")
         options.add_argument('--user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3')
         options.add_experimental_option("prefs", {"download.default_directory": directory, "download.directory_upgrade": True, "download.prompt_for_download": False, "credentials_enable_service": False, "profile.password_manager_enabled": False})
         options.add_argument('--window-size=1920,1080')
```

### Comparing `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/errorLogger.py` & `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/errorLogger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import os
 import logging
 import traceback
+import selenium.webdriver
 from logging.handlers import RotatingFileHandler
 
 class CustomFormatter(logging.Formatter):
     def formatException(self, exc_info):
         result = super().formatException(exc_info)
         return f"{result}"
 
@@ -19,23 +21,29 @@
             # Add the traceback to the log message
             traceback_message = self.formatException(record.exc_info)
             return f"{'`' * 100}\n{message}\n{traceback_message}\n{'`' * 100}\n"
         else:
             message = super().format(record)
             return f"{'`' * 100}\n{message}\n{'`' * 100}\n"
 
+# Get the directory of the script
+script_dir = os.path.dirname(os.path.abspath(__file__))
+
 # Set up the logging configuration
-log_file = 'log.txt'
+log_file = os.path.join(script_dir, 'log.txt')
 max_file_size = 1024 * 1024  # 1 MB
 backup_count = 0  # Set to 0 for only one log file
 
 # Create a rotating file handler
 handler = RotatingFileHandler(log_file, maxBytes=max_file_size, backupCount=backup_count)
 handler.setLevel(logging.ERROR)
 
 # Set the log format
 formatter = CustomFormatter('%(asctime)s - %(levelname)s - %(message)s')
 handler.setFormatter(formatter)
 
 # Get the root logger and add the handler
 logger = logging.getLogger('')
-logger.addHandler(handler)
+logger.addHandler(handler)
+
+# Set the logging level for selenium.webdriver to WARNING
+logging.getLogger('selenium.webdriver').setLevel(logging.WARNING)
```

### Comparing `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/imdbData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/verifyCredentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,14 +170,17 @@
         json.dump(credentials, file)
 
     # return true or false
     return sync_watchlist_value
 
 # Last run function, used to determine when the last time IMDB reviews were submitted    
 def check_imdb_reviews_last_submitted():
+    here = os.path.abspath(os.path.dirname(__file__))
+    file_path = os.path.join(here, 'credentials.txt')
+    
     # Load credentials from credentials.txt
     if os.path.exists(file_path):
         with open(file_path, 'r', encoding='utf-8') as file:
             credentials = json.load(file)
     else:
         credentials = {}
```

### Comparing `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.5.0
+Version: 1.5.1
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.0/LICENSE` & `IMDBTraktSyncer-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.0/PKG-INFO` & `IMDBTraktSyncer-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.5.0
+Version: 1.5.1
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.5.0/README.md` & `IMDBTraktSyncer-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.0/setup.py` & `IMDBTraktSyncer-1.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.5.0'
+VERSION = '1.5.1'
 DESCRIPTION = 'A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

