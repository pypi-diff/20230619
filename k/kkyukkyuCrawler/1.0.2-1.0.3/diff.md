# Comparing `tmp/kkyukkyuCrawler-1.0.2.tar.gz` & `tmp/kkyukkyuCrawler-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkyukkyuCrawler-1.0.2.tar", last modified: Mon Jun 19 01:46:55 2023, max compression
+gzip compressed data, was "kkyukkyuCrawler-1.0.3.tar", last modified: Mon Jun 19 01:59:11 2023, max compression
```

## Comparing `kkyukkyuCrawler-1.0.2.tar` & `kkyukkyuCrawler-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 01:46:55.789935 kkyukkyuCrawler-1.0.2/
--rw-rw-rw-   0        0        0     1083 2023-06-18 22:37:34.000000 kkyukkyuCrawler-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0    14387 2023-06-19 01:46:55.789935 kkyukkyuCrawler-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    13942 2023-06-19 01:43:35.000000 kkyukkyuCrawler-1.0.2/README.md
--rw-rw-rw-   0        0        0      180 2023-06-18 22:35:22.000000 kkyukkyuCrawler-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 01:46:55.790935 kkyukkyuCrawler-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-06-19 01:46:21.000000 kkyukkyuCrawler-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:46:55.763965 kkyukkyuCrawler-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 01:46:55.778923 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler/
--rw-rw-rw-   0        0        0      147 2023-06-18 23:56:07.000000 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler/__init__.py
--rw-rw-rw-   0        0        0    31089 2023-06-19 01:45:18.000000 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler/src.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:46:55.787954 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler.egg-info/
--rw-rw-rw-   0        0        0    14387 2023-06-19 01:46:55.000000 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-06-19 01:46:55.000000 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 01:46:55.000000 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-19 01:46:55.000000 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-19 01:46:55.000000 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 01:59:11.973127 kkyukkyuCrawler-1.0.3/
+-rw-rw-rw-   0        0        0     1083 2023-06-18 22:37:34.000000 kkyukkyuCrawler-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    14387 2023-06-19 01:59:11.972128 kkyukkyuCrawler-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    13942 2023-06-19 01:43:35.000000 kkyukkyuCrawler-1.0.3/README.md
+-rw-rw-rw-   0        0        0      180 2023-06-18 22:35:22.000000 kkyukkyuCrawler-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 01:59:11.973127 kkyukkyuCrawler-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      860 2023-06-19 01:59:00.000000 kkyukkyuCrawler-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:59:11.950040 kkyukkyuCrawler-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 01:59:11.959451 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler/
+-rw-rw-rw-   0        0        0      147 2023-06-18 23:56:07.000000 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler/__init__.py
+-rw-rw-rw-   0        0        0    31068 2023-06-19 01:52:54.000000 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler/src.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:59:11.971212 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler.egg-info/
+-rw-rw-rw-   0        0        0    14387 2023-06-19 01:59:11.000000 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-06-19 01:59:11.000000 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 01:59:11.000000 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-19 01:59:11.000000 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-19 01:59:11.000000 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler.egg-info/top_level.txt
```

### Comparing `kkyukkyuCrawler-1.0.2/LICENSE.txt` & `kkyukkyuCrawler-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kkyukkyuCrawler-1.0.2/PKG-INFO` & `kkyukkyuCrawler-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kkyukkyuCrawler
-Version: 1.0.2
+Version: 1.0.3
 Summary: law case crawling lib
 Home-page: https://github.com/eik4862/kkyukkyuCrawler
 Author: eik4862
 Author-email: lkd1962@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kkyukkyuCrawler-1.0.2/README.md` & `kkyukkyuCrawler-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `kkyukkyuCrawler-1.0.2/setup.py` & `kkyukkyuCrawler-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kkyukkyuCrawler",
-    version="1.0.2",
+    version="1.0.3",
     author="eik4862",
     author_email="lkd1962@naver.com",
     description="law case crawling lib",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/eik4862/kkyukkyuCrawler",
     project_urls={},
```

### Comparing `kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler/src.py` & `kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler/src.py`

 * *Files 1% similar despite different names*

```diff
@@ -622,15 +622,14 @@
         :type soup: BeautifulSoup
 
         :return: The list of parsed results
         :rtype: list of str
         """
         results: List[str] = []
         cand: ResultSet = soup.select_one('div.cn-case-body').find_all('p', recursive=False)
-        print(cand)
         i: int = 0
         while i < len(cand):
             if re.sub(r'\s+', '', cand[i].text) == '주문':
                 break
             i += 1
         assert i + 1 < len(cand)
         i += 1
```

### Comparing `kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler.egg-info/PKG-INFO` & `kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kkyukkyuCrawler
-Version: 1.0.2
+Version: 1.0.3
 Summary: law case crawling lib
 Home-page: https://github.com/eik4862/kkyukkyuCrawler
 Author: eik4862
 Author-email: lkd1962@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

