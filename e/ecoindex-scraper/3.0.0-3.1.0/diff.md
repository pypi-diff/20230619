# Comparing `tmp/ecoindex_scraper-3.0.0.tar.gz` & `tmp/ecoindex_scraper-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoindex_scraper-3.0.0.tar", max compression
+gzip compressed data, was "ecoindex_scraper-3.1.0.tar", max compression
```

## Comparing `ecoindex_scraper-3.0.0.tar` & `ecoindex_scraper-3.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    18648 2023-06-19 12:22:51.400187 ecoindex_scraper-3.0.0/LICENSE
--rw-r--r--   0        0        0     4500 2023-06-19 12:22:51.400187 ecoindex_scraper-3.0.0/README.md
--rw-r--r--   0        0        0       35 2023-06-19 12:22:51.400187 ecoindex_scraper-3.0.0/ecoindex_scraper/__init__.py
--rw-r--r--   0        0        0     8105 2023-06-19 12:22:51.400187 ecoindex_scraper-3.0.0/ecoindex_scraper/scrap.py
--rw-r--r--   0        0        0      667 2023-06-19 12:22:51.404187 ecoindex_scraper-3.0.0/ecoindex_scraper/utils.py
--rw-r--r--   0        0        0      771 2023-06-19 12:22:51.404187 ecoindex_scraper-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 ecoindex_scraper-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    18648 2023-06-19 15:57:41.764360 ecoindex_scraper-3.1.0/LICENSE
+-rw-r--r--   0        0        0     4500 2023-06-19 15:57:41.764360 ecoindex_scraper-3.1.0/README.md
+-rw-r--r--   0        0        0       35 2023-06-19 15:57:41.764360 ecoindex_scraper-3.1.0/ecoindex_scraper/__init__.py
+-rw-r--r--   0        0        0     8450 2023-06-19 15:57:41.764360 ecoindex_scraper-3.1.0/ecoindex_scraper/scrap.py
+-rw-r--r--   0        0        0      667 2023-06-19 15:57:41.764360 ecoindex_scraper-3.1.0/ecoindex_scraper/utils.py
+-rw-r--r--   0        0        0      733 2023-06-19 15:57:41.764360 ecoindex_scraper-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 ecoindex_scraper-3.1.0/PKG-INFO
```

### Comparing `ecoindex_scraper-3.0.0/LICENSE` & `ecoindex_scraper-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.0.0/README.md` & `ecoindex_scraper-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.0.0/ecoindex_scraper/scrap.py` & `ecoindex_scraper-3.1.0/ecoindex_scraper/scrap.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from datetime import datetime
 from json import loads
+from os import remove
+from shutil import copyfile
 from time import sleep
 from typing import Dict, Tuple
+from uuid import uuid4
 
 import undetected_chromedriver as uc
 from ecoindex.ecoindex import get_ecoindex
 from ecoindex.models import PageMetrics, PageType, Result, ScreenShot, WindowSize
 from pydantic.networks import HttpUrl
 from selenium.common.exceptions import JavascriptException, NoSuchElementException
 from selenium.webdriver import DesiredCapabilities
@@ -31,32 +34,40 @@
         self.window_size = window_size
         self.wait_before_scroll = wait_before_scroll
         self.wait_after_scroll = wait_after_scroll
         self.screenshot = screenshot
         self.screenshot_uid = screenshot_uid
         self.screenshot_gid = screenshot_gid
         self.chrome_version_main = chrome_version_main
-        self.driver_executable_path = driver_executable_path
         self.page_load_timeout = page_load_timeout
 
         self.chrome_options = uc.ChromeOptions()
         self.chrome_options.headless = True
         self.chrome_options.add_argument(f"--window-size={self.window_size}")
         self.chrome_options.add_argument("--no-sandbox")
         self.chrome_options.add_argument("--disable-dev-shm-usage")
         self.chrome_options.add_argument("--ignore-certificate-errors")
 
         self.capbs = DesiredCapabilities.CHROME.copy()
 
         self.capbs["goog:loggingPrefs"] = {"performance": "ALL"}  # type: ignore
 
+        if driver_executable_path:
+            self.driver_executable_path = f"/tmp/chromedriver_{uuid4()}"
+            copyfile(driver_executable_path, self.driver_executable_path)
+        else:
+            self.driver_executable_path = None
+
     def __del__(self):
         if hasattr(self, "driver"):
             self.driver.quit()
 
+        if self.driver_executable_path:
+            remove(self.driver_executable_path)
+
     def init_chromedriver(self):
         self.driver = uc.Chrome(
             options=self.chrome_options,
             desired_capabilities=self.capbs,
             version_main=self.chrome_version_main,
             driver_executable_path=self.driver_executable_path,
         )
```

### Comparing `ecoindex_scraper-3.0.0/ecoindex_scraper/utils.py` & `ecoindex_scraper-3.1.0/ecoindex_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.0.0/pyproject.toml` & `ecoindex_scraper-3.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "ecoindex_scraper"
-version = "3.0.0"
+version = "3.1.0"
 description = "Ecoindex_scraper module provides a way to scrape data from given website while simulating a real web browser"
 authors = ["Vincent Vatelot <vincent.vatelot@ik.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://www.ecoindex.fr"
 repository = "https://github.com/cnumr/ecoindex_scraper_python"
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-ecoindex = {version = "^5.4.2", allow-prereleases = true}
+ecoindex = "^5.4.2"
 undetected-chromedriver = "3.4.7"
 Pillow = "^9.2.0"
 selenium = "4.9"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3"
 black = {version = "^23.3.0", allow-prereleases = true}
```

### Comparing `ecoindex_scraper-3.0.0/PKG-INFO` & `ecoindex_scraper-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoindex-scraper
-Version: 3.0.0
+Version: 3.1.0
 Summary: Ecoindex_scraper module provides a way to scrape data from given website while simulating a real web browser
 Home-page: http://www.ecoindex.fr
 License: MIT
 Author: Vincent Vatelot
 Author-email: vincent.vatelot@ik.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

