# Comparing `tmp/pinscrape-2.0.1.tar.gz` & `tmp/pinscrape-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinscrape-2.0.1.tar", last modified: Tue Apr 18 07:26:25 2023, max compression
+gzip compressed data, was "pinscrape-3.0.3.tar", last modified: Mon Jun 19 15:47:46 2023, max compression
```

## Comparing `pinscrape-2.0.1.tar` & `pinscrape-3.0.3.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-04-18 07:26:25.574910 pinscrape-2.0.1/
--rw-r--r--   0 atul       (501) staff       (20)     1078 2023-04-18 07:24:22.000000 pinscrape-2.0.1/LICENSE
--rw-r--r--   0 atul       (501) staff       (20)     1469 2023-04-18 07:26:25.574798 pinscrape-2.0.1/PKG-INFO
--rw-r--r--   0 atul       (501) staff       (20)     1042 2023-04-18 07:24:22.000000 pinscrape-2.0.1/README.md
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-04-18 07:26:25.574066 pinscrape-2.0.1/pinscrape/
--rw-r--r--   0 atul       (501) staff       (20)      226 2023-04-18 07:24:22.000000 pinscrape-2.0.1/pinscrape/__init__.py
--rw-r--r--   0 atul       (501) staff       (20)       22 2023-04-18 07:26:14.000000 pinscrape-2.0.1/pinscrape/_version.py
--rw-r--r--   0 atul       (501) staff       (20)     6130 2023-04-18 07:24:22.000000 pinscrape-2.0.1/pinscrape/pinscrape.py
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-04-18 07:26:25.574636 pinscrape-2.0.1/pinscrape.egg-info/
--rw-r--r--   0 atul       (501) staff       (20)     1469 2023-04-18 07:26:25.000000 pinscrape-2.0.1/pinscrape.egg-info/PKG-INFO
--rw-r--r--   0 atul       (501) staff       (20)      257 2023-04-18 07:26:25.000000 pinscrape-2.0.1/pinscrape.egg-info/SOURCES.txt
--rw-r--r--   0 atul       (501) staff       (20)        1 2023-04-18 07:26:25.000000 pinscrape-2.0.1/pinscrape.egg-info/dependency_links.txt
--rw-r--r--   0 atul       (501) staff       (20)       76 2023-04-18 07:26:25.000000 pinscrape-2.0.1/pinscrape.egg-info/requires.txt
--rw-r--r--   0 atul       (501) staff       (20)       10 2023-04-18 07:26:25.000000 pinscrape-2.0.1/pinscrape.egg-info/top_level.txt
--rw-r--r--   0 atul       (501) staff       (20)       38 2023-04-18 07:26:25.574945 pinscrape-2.0.1/setup.cfg
--rw-r--r--   0 atul       (501) staff       (20)      813 2023-04-18 07:24:22.000000 pinscrape-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:47:46.580795 pinscrape-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-19 15:47:27.000000 pinscrape-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-19 15:47:46.580795 pinscrape-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-19 15:47:27.000000 pinscrape-3.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:47:46.580795 pinscrape-3.0.3/pinscrape/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-19 15:47:27.000000 pinscrape-3.0.3/pinscrape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 15:47:27.000000 pinscrape-3.0.3/pinscrape/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-06-19 15:47:27.000000 pinscrape-3.0.3/pinscrape/pinscrape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:47:46.580795 pinscrape-3.0.3/pinscrape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-19 15:47:46.000000 pinscrape-3.0.3/pinscrape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-19 15:47:46.000000 pinscrape-3.0.3/pinscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:47:46.000000 pinscrape-3.0.3/pinscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 15:47:46.000000 pinscrape-3.0.3/pinscrape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 15:47:46.000000 pinscrape-3.0.3/pinscrape.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 15:47:46.580795 pinscrape-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-19 15:47:27.000000 pinscrape-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:47:46.580795 pinscrape-3.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:47:27.000000 pinscrape-3.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-19 15:47:27.000000 pinscrape-3.0.3/tests/e2e.py
```

### Comparing `pinscrape-2.0.1/LICENSE` & `pinscrape-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pinscrape-2.0.1/PKG-INFO` & `pinscrape-3.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinscrape
-Version: 2.0.1
+Version: 3.0.3
 Summary: Pinterest data scraper
 Home-page: https://github.com/iamatulsingh/pinscrape
 Author: Atul Singh
 Author-email: atulsingh0401@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,13 +27,13 @@
     print(f"\nTotal urls found: {len(details['extracted_urls'])}")
     print(f"\nTotal images downloaded (including duplicate images): {len(details['url_list'])}")
     print(details)
 else:
     print("\nNothing to download !!")
 ```
 
-`scrape("messi", "output", {}, 10)` <br/>
+`scrape("messi", "output", {}, 10, 15)` <br/>
 - `"messi"` is keyword
 - `"output"` is path to a folder where you want to save images
 - `{}` is proxy list if you want to add one (optional)
 - `10` is a number of threads you want to use for downloading those images (optional)
 - `15` is the maximum number of images you want to download (optional)
```

### Comparing `pinscrape-2.0.1/README.md` & `pinscrape-3.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,13 +13,13 @@
     print(f"\nTotal urls found: {len(details['extracted_urls'])}")
     print(f"\nTotal images downloaded (including duplicate images): {len(details['url_list'])}")
     print(details)
 else:
     print("\nNothing to download !!")
 ```
 
-`scrape("messi", "output", {}, 10)` <br/>
+`scrape("messi", "output", {}, 10, 15)` <br/>
 - `"messi"` is keyword
 - `"output"` is path to a folder where you want to save images
 - `{}` is proxy list if you want to add one (optional)
 - `10` is a number of threads you want to use for downloading those images (optional)
 - `15` is the maximum number of images you want to download (optional)
```

### Comparing `pinscrape-2.0.1/pinscrape/pinscrape.py` & `pinscrape-3.0.3/pinscrape/pinscrape.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,20 +116,24 @@
         searched_urls = PinterestImageScraper.get_pinterest_links(res.content,max_images)
 
         return searched_urls, key.replace(" ", "_")
 
 
     def scrape(self, key=None, output_folder="", proxies={}, threads=10, max_images: int = None):
         extracted_urls, keyword = PinterestImageScraper.start_scraping(max_images,key, proxies)
+        return_data = {}
+        self.unique_img = []
+        self.json_data_list = []
 
         for i in extracted_urls:
             self.get_source(i, proxies)
 
         # get all urls of images and save in a list
         url_list = self.save_image_url(max_images)
+
         return_data = {
             "isDownloaded": False,
             "url_list": url_list,
             "extracted_urls": extracted_urls,
             "keyword": key
         }
```

### Comparing `pinscrape-2.0.1/pinscrape.egg-info/PKG-INFO` & `pinscrape-3.0.3/pinscrape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinscrape
-Version: 2.0.1
+Version: 3.0.3
 Summary: Pinterest data scraper
 Home-page: https://github.com/iamatulsingh/pinscrape
 Author: Atul Singh
 Author-email: atulsingh0401@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,13 +27,13 @@
     print(f"\nTotal urls found: {len(details['extracted_urls'])}")
     print(f"\nTotal images downloaded (including duplicate images): {len(details['url_list'])}")
     print(details)
 else:
     print("\nNothing to download !!")
 ```
 
-`scrape("messi", "output", {}, 10)` <br/>
+`scrape("messi", "output", {}, 10, 15)` <br/>
 - `"messi"` is keyword
 - `"output"` is path to a folder where you want to save images
 - `{}` is proxy list if you want to add one (optional)
 - `10` is a number of threads you want to use for downloading those images (optional)
 - `15` is the maximum number of images you want to download (optional)
```

### Comparing `pinscrape-2.0.1/setup.py` & `pinscrape-3.0.3/setup.py`

 * *Files identical despite different names*

