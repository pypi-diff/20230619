# Comparing `tmp/amazon-scraper-toolkit-0.0.1.tar.gz` & `tmp/amazon-scraper-toolkit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-scraper-toolkit-0.0.1.tar", last modified: Mon Jun  5 05:00:12 2023, max compression
+gzip compressed data, was "amazon-scraper-toolkit-1.0.0.tar", last modified: Mon Jun 19 14:20:05 2023, max compression
```

## Comparing `amazon-scraper-toolkit-0.0.1.tar` & `amazon-scraper-toolkit-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 05:00:12.334916 amazon-scraper-toolkit-0.0.1/
--rw-rw-rw-   0        0        0     1100 2023-06-05 04:51:21.000000 amazon-scraper-toolkit-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2026 2023-06-05 05:00:12.332917 amazon-scraper-toolkit-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-04 02:35:50.000000 amazon-scraper-toolkit-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 05:00:12.303933 amazon-scraper-toolkit-0.0.1/amazon_scrape_toolkit/
--rw-rw-rw-   0        0        0      138 2023-06-04 02:23:01.000000 amazon-scraper-toolkit-0.0.1/amazon_scrape_toolkit/__init__.py
--rw-rw-rw-   0        0        0    11966 2023-06-04 02:23:03.000000 amazon-scraper-toolkit-0.0.1/amazon_scrape_toolkit/main.py
-drwxrwxrwx   0        0        0        0 2023-06-05 05:00:12.326921 amazon-scraper-toolkit-0.0.1/amazon_scraper_toolkit.egg-info/
--rw-rw-rw-   0        0        0     2026 2023-06-05 05:00:12.000000 amazon-scraper-toolkit-0.0.1/amazon_scraper_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-06-05 05:00:12.000000 amazon-scraper-toolkit-0.0.1/amazon_scraper_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 05:00:12.000000 amazon-scraper-toolkit-0.0.1/amazon_scraper_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-05 05:00:12.000000 amazon-scraper-toolkit-0.0.1/amazon_scraper_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-05 05:00:12.000000 amazon-scraper-toolkit-0.0.1/amazon_scraper_toolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2023-06-05 04:43:16.000000 amazon-scraper-toolkit-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-05 05:00:12.335915 amazon-scraper-toolkit-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 14:20:05.446330 amazon-scraper-toolkit-1.0.0/
+-rw-rw-rw-   0        0        0     1100 2023-06-05 04:51:21.000000 amazon-scraper-toolkit-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2026 2023-06-19 14:20:05.446330 amazon-scraper-toolkit-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-04 02:35:50.000000 amazon-scraper-toolkit-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 14:20:05.425937 amazon-scraper-toolkit-1.0.0/amazon_scrape_toolkit/
+-rw-rw-rw-   0        0        0      138 2023-06-04 02:23:01.000000 amazon-scraper-toolkit-1.0.0/amazon_scrape_toolkit/__init__.py
+-rw-rw-rw-   0        0        0    12265 2023-06-19 14:02:48.000000 amazon-scraper-toolkit-1.0.0/amazon_scrape_toolkit/main.py
+drwxrwxrwx   0        0        0        0 2023-06-19 14:20:05.446330 amazon-scraper-toolkit-1.0.0/amazon_scraper_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     2026 2023-06-19 14:20:05.000000 amazon-scraper-toolkit-1.0.0/amazon_scraper_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-06-19 14:20:05.000000 amazon-scraper-toolkit-1.0.0/amazon_scraper_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 14:20:05.000000 amazon-scraper-toolkit-1.0.0/amazon_scraper_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-19 14:20:05.000000 amazon-scraper-toolkit-1.0.0/amazon_scraper_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-19 14:20:05.000000 amazon-scraper-toolkit-1.0.0/amazon_scraper_toolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1353 2023-06-19 14:18:27.000000 amazon-scraper-toolkit-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 14:20:05.452042 amazon-scraper-toolkit-1.0.0/setup.cfg
```

### Comparing `amazon-scraper-toolkit-0.0.1/LICENSE` & `amazon-scraper-toolkit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-scraper-toolkit-0.0.1/PKG-INFO` & `amazon-scraper-toolkit-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-scraper-toolkit
-Version: 0.0.1
+Version: 1.0.0
 Summary: Some Helpful Classes and Functions for Scraping Amazon Data
 Author: Tejas
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `amazon-scraper-toolkit-0.0.1/amazon_scrape_toolkit/main.py` & `amazon-scraper-toolkit-1.0.0/amazon_scrape_toolkit/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import time
 import json
 import logging
 from functools import wraps
 from dataclasses import dataclass
 import requests
 
+logger = logging.getLogger()
+
 
 @dataclass
 class AmazonHeaders:
     """Data class representing the headers for making requests to Amazon"""
 
     user_agent: str
     accept_lang: str
@@ -54,15 +56,17 @@
     """
 
     start_time = time.monotonic()
     yield start_time
     yield round(time.monotonic() - start_time, 3)
 
 
-def get_all_product_ids(link: str, headers: AmazonHeaders, max_products=10000000000000):
+def get_all_product_ids(
+    link: str, headers: AmazonHeaders, pages_to_scrape=10000000000000
+):
     """
     Fetches all product IDs from the given Amazon search link.
 
     Args:
         link (str): The Amazon search link.
         headers (AmazonHeaders): The headers to be used for making requests.
         max_products (int, optional): The maximum number of products to fetch. Defaults to As many as possible (10000000000000).
@@ -79,16 +83,18 @@
     page_link = link
     no_of_pages = 0
 
     fetch_times = []
     start_time = time.monotonic()
     soup_pages = []
 
+    i = 0
+
     try:
-        for _ in set(range(max_products)):
+        while i < pages_to_scrape:
             fetch_timer = timer()
             next(fetch_timer)
 
             no_of_pages += 1
             page = session.get(page_link, headers=headers.req)
             page.raise_for_status()
 
@@ -102,45 +108,50 @@
                     "span.s-pagination-item.s-pagination-selected"
                 )
                 next_page_a = current_page.find_next_sibling(
                     "a", class_="s-pagination-item s-pagination-button"
                 )
 
             page_link = f"https://www.amazon.in{next_page_a['href']}"
+            logger.info(f"found page idx: {no_of_pages}")
             soup_pages.append(soup)
+            i += 1
 
     except (TypeError, AttributeError):
-        logging.warn(f"final_page: {page_link}")
+        logger.warn(f"final_page: {page_link}")
 
-    logging.info(f"full fetch duration: {time.monotonic() - start_time}")
-    logging.info(f"scraped {no_of_pages} pages")
-    logging.debug(f"avg page fetch time: {sum(fetch_times) / len(fetch_times)}")
-    logging.debug(f"max page fetch time: {max(fetch_times)}")
-    logging.debug(f"min page fetch time: {min(fetch_times)}")
+    logger.info(f"full fetch duration: {time.monotonic() - start_time}")
+    logger.info(f"scraped {no_of_pages} pages")
+    logger.debug(f"avg page fetch time: {sum(fetch_times) / len(fetch_times)}")
+    logger.debug(f"max page fetch time: {max(fetch_times)}")
+    logger.debug(f"min page fetch time: {min(fetch_times)}")
 
     scrape_timer = timer()
     next(scrape_timer)
     all_product_ids = []
     scrape_times = []
 
     def scrape_soup_links(soup: bs4.BeautifulSoup):
         st = time.monotonic()
         divs = soup.select("div[data-asin]")
         product_ids = filter(lambda x: x != "", [div["data-asin"] for div in divs])
         all_product_ids.extend(product_ids)
         scrape_times.append(time.monotonic() - st)
 
-    [scrape_soup_links(soup) for soup in set(soup_pages)]
-
-    logging.info(f"full scrape duration: {next(scrape_timer)}")
-    logging.info(f"scraped {len(all_product_ids)} product id's")
-    logging.info(f"but only {len(set(all_product_ids))} product id's are unique")
-    logging.debug(f"avg page half scrape time: {sum(scrape_times) / len(scrape_times)}")
-    logging.debug(f"max page half scrape time: {max(scrape_times)}")
-    logging.debug(f"min page half scrape time: {min(scrape_times)}")
+    for soup in set(soup_pages):
+        old_no = len(all_product_ids)
+        scrape_soup_links(soup)
+        logger.info(f"found {len(all_product_ids) - old_no} products")
+
+    logger.info(f"full scrape duration: {next(scrape_timer)}")
+    logger.info(f"scraped {len(all_product_ids)} product id's")
+    logger.info(f"but only {len(set(all_product_ids))} product id's are unique")
+    logger.debug(f"avg page half scrape time: {sum(scrape_times) / len(scrape_times)}")
+    logger.debug(f"max page half scrape time: {max(scrape_times)}")
+    logger.debug(f"min page half scrape time: {min(scrape_times)}")
 
     return set(all_product_ids)
 
 
 def product_scraper(fetch_ratings: bool = True, get_others: bool = True):
     """
     Decorator to mark a function as a product scraper.
@@ -155,18 +166,20 @@
 
     def inner_decorator(func):
         @wraps(func)
         def _wrapper(soup: bs4.BeautifulSoup, product_id: str, *args, **kwargs):
             data_func_timer = timer()
             next(data_func_timer)
             data = func(soup, product_id, *args, **kwargs)
-            assert isinstance(data, (dict, None)), "Output should be Dict or None!"
+            assert data is None or isinstance(
+                data, dict
+            ), "Output should be Dict or None!"
 
             if data is None:
-                logging.info(f"page_failed [{product_id}]")
+                logger.info(f"page_failed [{product_id}]")
                 return None
 
             data_func_timer = next(data_func_timer)
             new_phones_to_add = [] if get_others else None
 
             other_phones_fetch_timer = timer()
             next(other_phones_fetch_timer)
@@ -266,15 +279,15 @@
                         for key, value in individual_star_ratings
                     }
                 else:
                     stared_ratings = {f"no of {key} star": 0 for key in range(1, 6)}
             ratings_fetch_timer = next(ratings_fetch_timer)
 
             # log success in fetching thing
-            logging.info(f"fetched_everything [{product_id}]")
+            logger.info(f"fetched_everything [{product_id}]")
 
             return ProductInfo(
                 new_phones_to_add,
                 stared_ratings,
                 data,
                 data_func_timer,
                 ratings_fetch_timer,
@@ -310,15 +323,15 @@
     def fetch_webpage(url):
         response = requests.get(url, headers=headers.req)
         response.raise_for_status()
         return response.content
 
     while len(product_ids_to_scrape) > 0:
         id_to_scrape = product_ids_to_scrape.pop()
-        logging.info(f"Scraping product with ID: {id_to_scrape}")
+        logger.info(f"Scraping product with ID: {id_to_scrape}")
 
         if id_to_scrape in scraped_ids:
             continue
 
         link = f"https://www.amazon.in/dp/{id_to_scrape}"
         soup = bs4.BeautifulSoup(fetch_webpage(link), "lxml")
         output: ProductInfo = function(soup, id_to_scrape)
@@ -333,15 +346,16 @@
             product_ids_to_scrape.update(output.other_products)
 
         if output.ratings is not None:
             product_data.update(output.ratings)
 
         if product_data not in data:
             data.append(product_data)
-            logging.info(f"product_scraped and saved [{id_to_scrape}]")
+            logger.info(f"product_scraped and saved [{id_to_scrape}]")
         else:
-            logging.info(f"product data not new and so not saved [{id_to_scrape}]")
+            logger.info(f"product data not new and so not saved [{id_to_scrape}]")
 
-        logging.info(f"Remaining products to scrape: {len(product_ids_to_scrape)}")
+        logger.info(f"Remaining products to scrape: {len(product_ids_to_scrape)}")
+        logger.info("-------")
 
-    logging.info(f"DONE - TIME TAKEN: {next(code_timer)}")
+    logger.info(f"DONE - TIME TAKEN: {next(code_timer)}")
     return data
```

### Comparing `amazon-scraper-toolkit-0.0.1/amazon_scraper_toolkit.egg-info/PKG-INFO` & `amazon-scraper-toolkit-1.0.0/amazon_scraper_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-scraper-toolkit
-Version: 0.0.1
+Version: 1.0.0
 Summary: Some Helpful Classes and Functions for Scraping Amazon Data
 Author: Tejas
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `amazon-scraper-toolkit-0.0.1/pyproject.toml` & `amazon-scraper-toolkit-1.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amazon-scraper-toolkit"
-version = "0.0.1"
+version = "1.0.0"
 description = "Some Helpful Classes and Functions for Scraping Amazon Data"
 readme = "README.md"
 authors = [{ name = "Tejas" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Natural Language :: English",
     "Intended Audience :: Developers",
@@ -29,8 +29,20 @@
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "pylint", "pep8"]
 
 [project.urls]
-Homepage = "https://github.com/KidCoderT/amazon-scraper"
+Homepage = "https://github.com/KidCoderT/amazon-scraper"
+
+[tool.bumpver]
+current_version = "1.0.0"
+version_pattern = "MAJOR.MINOR.PATCH"
+commit_message = "bump version {old_version} -> {new_version}"
+commit = true
+tag = true
+push = false
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = ['current_version = "{version}"']
+
```

