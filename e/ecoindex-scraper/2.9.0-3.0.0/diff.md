# Comparing `tmp/ecoindex_scraper-2.9.0.tar.gz` & `tmp/ecoindex_scraper-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoindex_scraper-2.9.0.tar", max compression
+gzip compressed data, was "ecoindex_scraper-3.0.0.tar", max compression
```

## Comparing `ecoindex_scraper-2.9.0.tar` & `ecoindex_scraper-3.0.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    18648 2022-11-29 10:09:55.139264 ecoindex_scraper-2.9.0/LICENSE
--rw-r--r--   0        0        0     3251 2022-11-29 10:09:55.139264 ecoindex_scraper-2.9.0/README.md
--rw-r--r--   0        0        0       35 2022-11-29 10:09:55.139264 ecoindex_scraper-2.9.0/ecoindex_scraper/__init__.py
--rw-r--r--   0        0        0     6584 2022-11-29 10:09:55.139264 ecoindex_scraper-2.9.0/ecoindex_scraper/scrap.py
--rw-r--r--   0        0        0      680 2022-11-29 10:09:55.139264 ecoindex_scraper-2.9.0/ecoindex_scraper/utils.py
--rw-r--r--   0        0        0      757 2022-11-29 10:09:55.139264 ecoindex_scraper-2.9.0/pyproject.toml
--rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 ecoindex_scraper-2.9.0/setup.py
--rw-r--r--   0        0        0     4019 1970-01-01 00:00:00.000000 ecoindex_scraper-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0    18648 2023-06-19 12:22:51.400187 ecoindex_scraper-3.0.0/LICENSE
+-rw-r--r--   0        0        0     4500 2023-06-19 12:22:51.400187 ecoindex_scraper-3.0.0/README.md
+-rw-r--r--   0        0        0       35 2023-06-19 12:22:51.400187 ecoindex_scraper-3.0.0/ecoindex_scraper/__init__.py
+-rw-r--r--   0        0        0     8105 2023-06-19 12:22:51.400187 ecoindex_scraper-3.0.0/ecoindex_scraper/scrap.py
+-rw-r--r--   0        0        0      667 2023-06-19 12:22:51.404187 ecoindex_scraper-3.0.0/ecoindex_scraper/utils.py
+-rw-r--r--   0        0        0      771 2023-06-19 12:22:51.404187 ecoindex_scraper-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 ecoindex_scraper-3.0.0/PKG-INFO
```

### Comparing `ecoindex_scraper-2.9.0/LICENSE` & `ecoindex_scraper-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-2.9.0/README.md` & `ecoindex_scraper-3.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 ```python
 Result(width=1920, height=1080, url=HttpUrl('http://ecoindex.fr', ), size=549.253, nodes=52, requests=12, grade='A', score=90.0, ges=1.2, water=1.8, ecoindex_version='5.0.0', date=datetime.datetime(2022, 9, 12, 10, 54, 46, 773443), page_type=None)
 ```
 
 > **Default behaviour:** By default, the page analysis simulates:
 >
+> - Uses the last version of chrome (can be set with parameter `chrome_version_main` to a given version. IE `107`)
 > - Window size of **1920x1080** pixels (can be set with parameter `window_size`)
 > - Wait for **1 second when page is loaded** (can be set with parameter `wait_before_scroll`)
 > - Scroll to the bottom of the page (if it is possible)
 > - Wait for **1 second after** having scrolled to the bottom of the page (can be set with parameter `wait_after_scroll`)
 
 ### Get a page analysis and generate a screenshot
 
@@ -77,14 +78,54 @@
         )
         .init_chromedriver()
         .get_page_analysis()
     )
 )
 ```
 
+## Async analysis
+
+You can also run the analysis asynchronously:
+
+```python
+import asyncio
+from concurrent.futures import ThreadPoolExecutor, as_completed
+
+from ecoindex_scraper.scrap import EcoindexScraper
+
+def run_page_analysis(url):
+    return asyncio.run(
+        EcoindexScraper(url=url)
+        .init_chromedriver()
+        .get_page_analysis()
+    )
+
+
+with ThreadPoolExecutor(max_workers=8) as executor:
+    future_to_analysis = {}
+
+    url = "https://www.ecoindex.fr"
+
+    for i in range(10):
+        future_to_analysis[
+            executor.submit(
+                run_page_analysis,
+                url,
+            )
+        ] = (url)
+
+    for future in as_completed(future_to_analysis):
+        try:
+            print(future.result())
+        except Exception as e:
+            print(e)
+```
+
+> **Note:** In this case, it is highly recommanded to use a fixed `chromedriver` version. You can set it with the parameter `chrome_version_main` (IE `107`) and `driver_executable_path` (IE `/usr/bin/chromedriver`). Otherwise undected-chromedriver will download the latest version of chromedriver and patch it for each analysis.
+
 ## Contribute
 
 You need [poetry](https://python-poetry.org/) to install and manage dependencies. Once poetry installed, run :
 
 ```bash
 poetry install
 ```
```

### Comparing `ecoindex_scraper-2.9.0/ecoindex_scraper/scrap.py` & `ecoindex_scraper-3.0.0/ecoindex_scraper/scrap.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,84 @@
 from datetime import datetime
 from json import loads
-from sys import getsizeof
 from time import sleep
-from typing import Dict, List, Tuple
-from warnings import filterwarnings
+from typing import Dict, Tuple
 
-import undetected_chromedriver.v2 as uc
+import undetected_chromedriver as uc
 from ecoindex.ecoindex import get_ecoindex
 from ecoindex.models import PageMetrics, PageType, Result, ScreenShot, WindowSize
 from pydantic.networks import HttpUrl
 from selenium.common.exceptions import JavascriptException, NoSuchElementException
 from selenium.webdriver import DesiredCapabilities
 
 from ecoindex_scraper.utils import convert_screenshot_to_webp, set_screenshot_rights
 
 
 class EcoindexScraper:
     def __init__(
         self,
         url: HttpUrl,
-        window_size: WindowSize | None = WindowSize(width=1920, height=1080),
-        wait_before_scroll: int | None = 1,
-        wait_after_scroll: int | None = 1,
+        chrome_version_main: int | None = None,
+        driver_executable_path: str | None = None,
+        window_size: WindowSize = WindowSize(width=1920, height=1080),
+        wait_before_scroll: float = 1,
+        wait_after_scroll: float = 1,
         screenshot: ScreenShot | None = None,
         screenshot_uid: int | None = None,
         screenshot_gid: int | None = None,
+        page_load_timeout: int = 20,
     ):
-        filterwarnings(action="ignore")
-
         self.url = url
         self.window_size = window_size
         self.wait_before_scroll = wait_before_scroll
         self.wait_after_scroll = wait_after_scroll
         self.screenshot = screenshot
         self.screenshot_uid = screenshot_uid
         self.screenshot_gid = screenshot_gid
+        self.chrome_version_main = chrome_version_main
+        self.driver_executable_path = driver_executable_path
+        self.page_load_timeout = page_load_timeout
 
         self.chrome_options = uc.ChromeOptions()
         self.chrome_options.headless = True
         self.chrome_options.add_argument(f"--window-size={self.window_size}")
         self.chrome_options.add_argument("--no-sandbox")
         self.chrome_options.add_argument("--disable-dev-shm-usage")
+        self.chrome_options.add_argument("--ignore-certificate-errors")
 
         self.capbs = DesiredCapabilities.CHROME.copy()
-        self.capbs["goog:loggingPrefs"] = {"performance": "ALL"}
+
+        self.capbs["goog:loggingPrefs"] = {"performance": "ALL"}  # type: ignore
 
     def __del__(self):
         if hasattr(self, "driver"):
             self.driver.quit()
 
     def init_chromedriver(self):
         self.driver = uc.Chrome(
-            options=self.chrome_options, desired_capabilities=self.capbs
+            options=self.chrome_options,
+            desired_capabilities=self.capbs,
+            version_main=self.chrome_version_main,
+            driver_executable_path=self.driver_executable_path,
         )
 
+        if self.page_load_timeout is not None:
+            self.driver.set_page_load_timeout(float(self.page_load_timeout))
+
         return self
 
     async def get_page_analysis(
         self,
     ) -> Result:
-        page_metrics, page_type = await self.scrap_page()
+        try:
+            page_metrics, page_type = await self.scrap_page()
+        except Exception as e:
+            self.__del__()
+            raise e
+
         ecoindex = await get_ecoindex(
             dom=page_metrics.nodes,
             size=page_metrics.size,
             requests=page_metrics.requests,
         )
         return Result(
             score=ecoindex.score,
@@ -76,15 +91,15 @@
             height=self.window_size.height,
             nodes=page_metrics.nodes,
             size=page_metrics.size,
             requests=page_metrics.requests,
             page_type=page_type,
         )
 
-    async def scrap_page(self) -> Tuple[PageMetrics, PageType]:
+    async def scrap_page(self) -> Tuple[PageMetrics, PageType | None]:
         self.driver.set_script_timeout(10)
         self.driver.get(self.url)
         sleep(self.wait_before_scroll)
 
         await self.generate_screenshot()
         await self.scroll_to_bottom()
 
@@ -104,89 +119,110 @@
                 uid=self.screenshot_uid,
                 gid=self.screenshot_gid,
             )
 
     async def scroll_to_bottom(self) -> None:
         try:
             self.driver.execute_script(
-                "window.scrollTo({ top: document.body.scrollHeight, behavior: 'smooth' })"
+                (
+                    "window.scrollTo({ top: "
+                    "document.body.scrollHeight, behavior: 'smooth' })"
+                )
             )
         except JavascriptException:
             pass
 
     async def get_page_metrics(self) -> PageMetrics:
-        outer_html = self.driver.execute_script(
-            "return document.documentElement.outerHTML"
-        )
         nodes = self.driver.find_elements("xpath", "//*")
-
         nb_svg_children = await self.get_svg_children_count()
-        downloaded_data = await self.parse_logs()
+        all_requests = await self.get_all_requests()
+
+        downloaded_data = [request["size"] for request in all_requests.values()]
 
         return PageMetrics(
-            size=(await self.get_page_size(downloaded_data, outer_html)),
+            size=sum(downloaded_data) / (10**3),
             nodes=(len(nodes) - nb_svg_children),
-            requests=len(downloaded_data),
+            requests=len(all_requests),
         )
 
-    @staticmethod
-    async def get_page_size(downloaded_data: List[int], outer_html: str) -> float:
-        result = (sum(downloaded_data) + getsizeof(outer_html)) / (10**3)
-
-        return result
-
-    async def parse_logs(self) -> List[int]:
-        downloaded_data = []
+    async def get_all_requests(self) -> Dict:
+        all_requests = {}
         page_response = False
+        performance_logs = self.driver.get_log("performance")
 
-        for log in self.driver.get_log("performance"):
+        for log in performance_logs:
             message = loads(log["message"])
 
             if (
                 "INFO" == log["level"]
                 and "Network.responseReceived" == message["message"]["method"]
-                and not page_response
+                and message["message"]["params"]["response"]["url"].startswith("http")
             ):
-                page_response = True
-                await self.check_page_response(message["message"]["params"]["response"])
+                all_requests[message["message"]["params"]["requestId"]] = {
+                    "url": message["message"]["params"]["response"]["url"],
+                    "size": 0,
+                    "type": message["message"]["params"]["type"],
+                }
+
+                if not page_response:
+                    page_response = True
+                    await self.check_page_response(
+                        message["message"]["params"]["response"]
+                    )
+
+            if (
+                "INFO" == log["level"]
+                and "Network.dataReceived" == message["message"]["method"]
+                and message["message"]["params"]["requestId"] in all_requests
+            ):
+                all_requests[message["message"]["params"]["requestId"]][
+                    "size"
+                ] += message["message"]["params"]["encodedDataLength"]
 
             if (
                 "INFO" == log["level"]
                 and "Network.loadingFinished" == message["message"]["method"]
+                and message["message"]["params"]["requestId"] in all_requests
             ):
-                downloaded_data.append(
-                    loads(log["message"])["message"]["params"]["encodedDataLength"]
-                )
+                all_requests[message["message"]["params"]["requestId"]][
+                    "size"
+                ] = message["message"]["params"]["encodedDataLength"]
 
-        return downloaded_data
+        return all_requests
 
     @staticmethod
     async def check_page_response(response: Dict) -> None:
         if response["mimeType"] != "text/html":
             raise TypeError(
                 {
                     "mimetype": response["mimeType"],
-                    "message": "This resource is not a standard page with mimeType 'text/html'",
+                    "message": (
+                        "This resource is not "
+                        "a standard page with mimeType 'text/html'"
+                    ),
                 }
             )
 
         if response["status"] != 200:
             raise ConnectionError(
                 {
                     "status": response["status"],
-                    "message": "This page can not be analyzed because the response status code is not 200",
+                    "message": (
+                        "This page can not be analyzed "
+                        "because the response status code is not 200"
+                    ),
                 }
             )
 
     async def get_page_type(self) -> PageType | None:
         try:
             return self.driver.find_element(
                 "xpath", "//meta[@property='og:type']"
             ).get_attribute("content")
-        except (NoSuchElementException):
+        except NoSuchElementException:
             return None
 
     async def get_svg_children_count(self) -> int:
         try:
-            return len(self.driver.find_elements("xpath", "//*[local-name()='svg']/*"))
-        except (NoSuchElementException):
+            return len(self.driver.find_elements("xpath", "//*[local-name()='svg']//*"))
+        except NoSuchElementException:
             return 0
```

### Comparing `ecoindex_scraper-2.9.0/ecoindex_scraper/utils.py` & `ecoindex_scraper-3.0.0/ecoindex_scraper/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from os import chown, unlink
+import os
 
 from ecoindex.models import ScreenShot
 from PIL import Image
 
 
 def convert_screenshot_to_webp(screenshot: ScreenShot) -> None:
     image = Image.open(rf"{screenshot.get_png()}")
     width, height = image.size
     ratio = 800 / height if width > height else 600 / width
 
     image.convert("RGB").resize(size=(int(width * ratio), int(height * ratio))).save(
         rf"{screenshot.get_webp()}",
         format="webp",
     )
-    unlink(screenshot.get_png())
+    os.unlink(screenshot.get_png())
 
 
 def set_screenshot_rights(
     screenshot: ScreenShot, uid: int | None = None, gid: int | None = None
 ) -> None:
     if uid and gid:
-        chown(path=screenshot.get_webp(), uid=uid, gid=gid)
+        os.chown(path=screenshot.get_webp(), uid=uid, gid=gid)
```

### Comparing `ecoindex_scraper-2.9.0/pyproject.toml` & `ecoindex_scraper-3.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "ecoindex_scraper"
-version = "v2.9.0"
+version = "3.0.0"
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
-ecoindex = {version = "^5.3.0", allow-prereleases = true}
-undetected-chromedriver = "^3.1.6"
+ecoindex = {version = "^5.4.2", allow-prereleases = true}
+undetected-chromedriver = "3.4.7"
 Pillow = "^9.2.0"
+selenium = "4.9"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1"
-black = {version = "^22.10.0", allow-prereleases = true}
+pytest = "^7.3"
+black = {version = "^23.3.0", allow-prereleases = true}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ecoindex_scraper-2.9.0/PKG-INFO` & `ecoindex_scraper-3.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: ecoindex-scraper
-Version: 2.9.0
+Version: 3.0.0
 Summary: Ecoindex_scraper module provides a way to scrape data from given website while simulating a real web browser
 Home-page: http://www.ecoindex.fr
 License: MIT
 Author: Vincent Vatelot
 Author-email: vincent.vatelot@ik.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
-Requires-Dist: ecoindex (>=5.3.0,<6.0.0)
-Requires-Dist: undetected-chromedriver (>=3.1.6,<4.0.0)
+Requires-Dist: ecoindex (>=5.4.2,<6.0.0)
+Requires-Dist: selenium (==4.9)
+Requires-Dist: undetected-chromedriver (==3.4.7)
 Project-URL: Repository, https://github.com/cnumr/ecoindex_scraper_python
 Description-Content-Type: text/markdown
 
 # ECOINDEX SCRAPER PYTHON
 
 ![Quality check](https://github.com/cnumr/ecoindex_scrap_python/workflows/Quality%20checks/badge.svg)
 [![PyPI version](https://badge.fury.io/py/ecoindex-scraper.svg)](https://badge.fury.io/py/ecoindex-scraper)
@@ -66,14 +67,15 @@
 
 ```python
 Result(width=1920, height=1080, url=HttpUrl('http://ecoindex.fr', ), size=549.253, nodes=52, requests=12, grade='A', score=90.0, ges=1.2, water=1.8, ecoindex_version='5.0.0', date=datetime.datetime(2022, 9, 12, 10, 54, 46, 773443), page_type=None)
 ```
 
 > **Default behaviour:** By default, the page analysis simulates:
 >
+> - Uses the last version of chrome (can be set with parameter `chrome_version_main` to a given version. IE `107`)
 > - Window size of **1920x1080** pixels (can be set with parameter `window_size`)
 > - Wait for **1 second when page is loaded** (can be set with parameter `wait_before_scroll`)
 > - Scroll to the bottom of the page (if it is possible)
 > - Wait for **1 second after** having scrolled to the bottom of the page (can be set with parameter `wait_after_scroll`)
 
 ### Get a page analysis and generate a screenshot
 
@@ -96,14 +98,54 @@
         )
         .init_chromedriver()
         .get_page_analysis()
     )
 )
 ```
 
+## Async analysis
+
+You can also run the analysis asynchronously:
+
+```python
+import asyncio
+from concurrent.futures import ThreadPoolExecutor, as_completed
+
+from ecoindex_scraper.scrap import EcoindexScraper
+
+def run_page_analysis(url):
+    return asyncio.run(
+        EcoindexScraper(url=url)
+        .init_chromedriver()
+        .get_page_analysis()
+    )
+
+
+with ThreadPoolExecutor(max_workers=8) as executor:
+    future_to_analysis = {}
+
+    url = "https://www.ecoindex.fr"
+
+    for i in range(10):
+        future_to_analysis[
+            executor.submit(
+                run_page_analysis,
+                url,
+            )
+        ] = (url)
+
+    for future in as_completed(future_to_analysis):
+        try:
+            print(future.result())
+        except Exception as e:
+            print(e)
+```
+
+> **Note:** In this case, it is highly recommanded to use a fixed `chromedriver` version. You can set it with the parameter `chrome_version_main` (IE `107`) and `driver_executable_path` (IE `/usr/bin/chromedriver`). Otherwise undected-chromedriver will download the latest version of chromedriver and patch it for each analysis.
+
 ## Contribute
 
 You need [poetry](https://python-poetry.org/) to install and manage dependencies. Once poetry installed, run :
 
 ```bash
 poetry install
 ```
```

