# Comparing `tmp/WebtoonScraper-0.0.9.tar.gz` & `tmp/WebtoonScraper-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebtoonScraper-0.0.9.tar", last modified: Wed May 17 14:22:45 2023, max compression
+gzip compressed data, was "WebtoonScraper-0.1.0a1.tar", last modified: Mon Jun 19 03:52:40 2023, max compression
```

## Comparing `WebtoonScraper-0.0.9.tar` & `WebtoonScraper-0.1.0a1.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 14:22:45.187776 WebtoonScraper-0.0.9/
--rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.0.9/LICENSE
--rw-rw-rw-   0        0        0       56 2023-05-17 13:57:54.000000 WebtoonScraper-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2134 2023-05-17 14:22:45.187776 WebtoonScraper-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2023-05-15 00:37:37.000000 WebtoonScraper-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 14:22:45.166747 WebtoonScraper-0.0.9/WebtoonScraper/
--rw-rw-rw-   0        0        0      165 2023-05-17 14:15:41.000000 WebtoonScraper-0.0.9/WebtoonScraper/__init__.py
--rw-rw-rw-   0        0        0     9473 2023-05-17 13:49:27.000000 WebtoonScraper-0.0.9/WebtoonScraper/foldermanagement.py
--rw-rw-rw-   0        0        0      682 2023-05-17 13:42:15.000000 WebtoonScraper-0.0.9/WebtoonScraper/getsoup.py
--rw-rw-rw-   0        0        0    11337 2023-05-17 14:22:22.000000 WebtoonScraper-0.0.9/WebtoonScraper/scraper.py
-drwxrwxrwx   0        0        0        0 2023-05-17 14:22:45.184400 WebtoonScraper-0.0.9/WebtoonScraper.egg-info/
--rw-rw-rw-   0        0        0     2134 2023-05-17 14:22:45.000000 WebtoonScraper-0.0.9/WebtoonScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-05-17 14:22:45.000000 WebtoonScraper-0.0.9/WebtoonScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 14:22:45.000000 WebtoonScraper-0.0.9/WebtoonScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-0.0.9/WebtoonScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-05-17 14:22:45.000000 WebtoonScraper-0.0.9/WebtoonScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-17 14:22:45.000000 WebtoonScraper-0.0.9/WebtoonScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    52914 2023-05-15 00:27:14.000000 WebtoonScraper-0.0.9/example1.png
--rw-rw-rw-   0        0        0       42 2023-05-17 14:22:45.187776 WebtoonScraper-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1326 2023-05-17 14:22:40.000000 WebtoonScraper-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 14:22:45.186747 WebtoonScraper-0.0.9/tests/
--rw-rw-rw-   0        0        0        0 2023-05-17 09:28:57.000000 WebtoonScraper-0.0.9/tests/__init__.py
--rw-rw-rw-   0        0        0      128 2023-05-16 14:18:05.000000 WebtoonScraper-0.0.9/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:52:40.428008 WebtoonScraper-0.1.0a1/
+-rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.1.0a1/LICENSE
+-rw-rw-rw-   0        0        0      140 2023-06-06 01:23:54.000000 WebtoonScraper-0.1.0a1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6658 2023-06-19 03:52:40.428008 WebtoonScraper-0.1.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0     5646 2023-06-18 13:17:35.000000 WebtoonScraper-0.1.0a1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 03:52:40.413076 WebtoonScraper-0.1.0a1/WebtoonScraper/
+-rw-rw-rw-   0        0        0      516 2023-06-06 00:42:00.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/BestChallengeScraper.py
+-rw-rw-rw-   0        0        0     6142 2023-06-19 03:38:04.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/BufftoonScraper.py
+-rw-rw-rw-   0        0        0     3332 2023-06-07 11:43:11.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/NaverWebtoonScraper.py
+-rw-rw-rw-   0        0        0    16541 2023-06-18 19:19:13.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/Scraper.py
+-rw-rw-rw-   0        0        0     4665 2023-06-17 13:02:43.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/TelescopeScraper.py
+-rw-rw-rw-   0        0        0     3438 2023-06-18 16:33:27.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/Webtoon.py
+-rw-rw-rw-   0        0        0      501 2023-06-06 00:44:55.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/WebtoonCanvasScraper.py
+-rw-rw-rw-   0        0        0     4250 2023-06-17 07:29:55.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/WebtoonOriginalsScraper.py
+-rw-rw-rw-   0        0        0      568 2023-06-18 16:21:17.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/__init__.py
+-rw-rw-rw-   0        0        0     9473 2023-05-17 13:49:27.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/foldermanagement.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:52:40.425804 WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/
+-rw-rw-rw-   0        0        0     6658 2023-06-19 03:52:40.000000 WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-06-19 03:52:40.000000 WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 03:52:40.000000 WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       29 2023-06-19 03:52:40.000000 WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-19 03:52:40.000000 WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    29088 2023-06-06 01:18:53.000000 WebtoonScraper-0.1.0a1/number_from_manhwakyung.png
+-rw-rw-rw-   0        0        0       42 2023-06-19 03:52:40.429009 WebtoonScraper-0.1.0a1/setup.cfg
+-rw-rw-rw-   0        0        0     1862 2023-06-19 03:52:38.000000 WebtoonScraper-0.1.0a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:52:40.426998 WebtoonScraper-0.1.0a1/test/
+-rw-rw-rw-   0        0        0      131 2023-06-18 16:21:20.000000 WebtoonScraper-0.1.0a1/test/test.py
+-rw-rw-rw-   0        0        0   182776 2023-05-29 08:43:24.000000 WebtoonScraper-0.1.0a1/title_no_from_webtoons.com.png
+-rw-rw-rw-   0        0        0    52914 2023-05-15 00:27:14.000000 WebtoonScraper-0.1.0a1/titleid_from_nw.png
```

### Comparing `WebtoonScraper-0.0.9/LICENSE` & `WebtoonScraper-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.9/WebtoonScraper/foldermanagement.py` & `WebtoonScraper-0.1.0a1/WebtoonScraper/foldermanagement.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.9/example1.png` & `WebtoonScraper-0.1.0a1/titleid_from_nw.png`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.9/setup.py` & `WebtoonScraper-0.1.0a1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-from pathlib import Path
 from setuptools import setup, find_packages
 
 # this_directory = Path(__file__).parent
 # long_description = (this_directory / "README.md").read_text()
 
 with open('README.md', 'r', encoding='utf-8') as f:
-    long_description = f.read()
+    long_description = '이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.\n'
+    long_description += f.read()
+    long_description = long_description.replace('titleid_from_nw.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/titleid_from_nw.png')
+    long_description = long_description.replace('title_no_from_webtoons.com.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/title_no_from_webtoons.com.png')
+    long_description = long_description.replace('number_from_manhwakyung.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/number_from_manhwakyung.png')
 
 setup(
     name='WebtoonScraper',
-    version='0.0.9',
+    version='0.1.0-alpha1',
     description='Scraping webtoons and some utils for it',
     author='ilotoki0804',
     author_email='ilotoki0804@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/ilotoki0804/WebtoonScraper',
-    install_requires=['tqdm', 'bs4', 'requests'],
+    install_requires=['tqdm', 'bs4', 'requests', 'better_abc'],
     packages=find_packages(exclude=[]),
     keywords=['Webtoon', 'Webtoon Scraper', 'Never Webtoon', 'Webtoon Downloader', 'Download Webtoon'],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     package_data={},
     zip_safe=False,
     classifiers=[
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

