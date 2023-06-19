# Comparing `tmp/webscrapex-0.0.5.tar.gz` & `tmp/webscrapex-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscrapex-0.0.5.tar", max compression
+gzip compressed data, was "webscrapex-0.0.7.tar", max compression
```

## Comparing `webscrapex-0.0.5.tar` & `webscrapex-0.0.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      772 2023-06-13 16:25:39.259866 webscrapex-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2234 2023-06-13 16:17:34.369303 webscrapex-0.0.5/README.md
--rw-r--r--   0        0        0       48 2023-06-13 16:25:25.157131 webscrapex-0.0.5/WebScrapeX/__init__.py
--rw-r--r--   0        0        0    14721 2023-06-13 16:06:51.159418 webscrapex-0.0.5/WebScrapeX/WebScrapeX.py
--rw-r--r--   0        0        0     3277 1970-01-01 00:00:00.000000 webscrapex-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      772 2023-06-19 05:19:40.581293 webscrapex-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2406 2023-06-19 05:12:49.699574 webscrapex-0.0.7/README.md
+-rw-r--r--   0        0        0       48 2023-06-19 05:19:29.840530 webscrapex-0.0.7/WebScrapeX/__init__.py
+-rw-r--r--   0        0        0    14722 2023-06-13 17:43:15.245938 webscrapex-0.0.7/WebScrapeX/WebScrapeX.py
+-rw-r--r--   0        0        0     3445 1970-01-01 00:00:00.000000 webscrapex-0.0.7/PKG-INFO
```

### Comparing `webscrapex-0.0.5/pyproject.toml` & `webscrapex-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "WebScrapeX"
-version = "0.0.5"
+version = "0.0.7"
 description = "A unified collection of web data premises eg Apartment for sale, apartment for rent, house for sale, house for rent"
 authors = ["Lisa Yvette INYANGE <linyange@andrew.cmu.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ILisa250/WebScrapeX"
 repository = "https://github.com/ILisa250/WebScrapeX"
 keywords = ["WebScrapeX", "web-data-extraction", "web-scraping", "web data collection",
```

### Comparing `webscrapex-0.0.5/WebScrapeX/WebScrapeX.py` & `webscrapex-0.0.7/WebScrapeX/WebScrapeX.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 # Loop through every house's link
                 for div in soup.findAll('div', {'class': 'item-list'}):
                     # Find the link for the current property
                     link = div.find('a').attrs['href']
                     # Keep the links in the Links list
                     Links.append("https://imali.biz" + link) 
                 # Break the loop after collecting the first 10 page
-                if page == 2:
+                if page == 10:
                     break
             except requests.exceptions.RequestException as e:
                 print(f"An error occurred while fetching data: {e}")
         # Create a DataFrame from the list
         imali_data = pd.DataFrame({f'{filename}_links': Links})
         imali_data.to_csv(f"{filename}_links.csv")
```

### Comparing `webscrapex-0.0.5/PKG-INFO` & `webscrapex-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscrapex
-Version: 0.0.5
+Version: 0.0.7
 Summary: A unified collection of web data premises eg Apartment for sale, apartment for rent, house for sale, house for rent
 Home-page: https://github.com/ILisa250/WebScrapeX
 License: MIT
 Keywords: WebScrapeX,web-data-extraction,web-scraping,web data collection,web data integration,web data aggregation,automated data extraction,Lisa Yvette INYANGE
 Author: Lisa Yvette INYANGE
 Author-email: linyange@andrew.cmu.edu
 Requires-Python: >=3,<4
@@ -66,17 +66,21 @@
     House for Rent: https://imali.biz/category/0/27/search?pg=
     House for Sale: https://imali.biz/category/0/24/search?pg=
 
 #### Usage example
 Here's an example of how to use the WebScrapeX package to scrape, clean, and save real estate data:
 ``` bash
 from WebScrapeX import scrape_clean_save_data
+import os 
 
+env_path = os.path.abspath('.env')
 # Specify the link of the real estate type to scrape
 url = "https://imali.biz/category/1/125/search?pg="
 
 # Specify the name of the file to save the data (in lowercase)
 file_name = "real_estate_data.csv"
 
 # Scrape, clean, and save the data
 scrape_clean_save_data(url, file_name, env_path)
 ```
+
+##### Note: File name should be either "house_sale" or "house_for_rent" or "apartment_for_sale" or "apartment_for_rent".
```

