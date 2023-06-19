# Comparing `tmp/WebtoonScraper-0.1.0.tar.gz` & `tmp/WebtoonScraper-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebtoonScraper-0.1.0.tar", last modified: Mon Jun 19 04:11:05 2023, max compression
+gzip compressed data, was "WebtoonScraper-0.1.0a1.tar", last modified: Mon Jun 19 03:52:40 2023, max compression
```

## Comparing `WebtoonScraper-0.1.0.tar` & `WebtoonScraper-0.1.0a1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 04:11:05.387356 WebtoonScraper-0.1.0/
--rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      140 2023-06-06 01:23:54.000000 WebtoonScraper-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6717 2023-06-19 04:11:05.386764 WebtoonScraper-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5706 2023-06-19 04:09:39.000000 WebtoonScraper-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 04:11:05.361654 WebtoonScraper-0.1.0/WebtoonScraper/
--rw-rw-rw-   0        0        0      516 2023-06-06 00:42:00.000000 WebtoonScraper-0.1.0/WebtoonScraper/BestChallengeScraper.py
--rw-rw-rw-   0        0        0     6142 2023-06-19 03:38:04.000000 WebtoonScraper-0.1.0/WebtoonScraper/BufftoonScraper.py
--rw-rw-rw-   0        0        0     3332 2023-06-07 11:43:11.000000 WebtoonScraper-0.1.0/WebtoonScraper/NaverWebtoonScraper.py
--rw-rw-rw-   0        0        0    16541 2023-06-18 19:19:13.000000 WebtoonScraper-0.1.0/WebtoonScraper/Scraper.py
--rw-rw-rw-   0        0        0     4665 2023-06-17 13:02:43.000000 WebtoonScraper-0.1.0/WebtoonScraper/TelescopeScraper.py
--rw-rw-rw-   0        0        0     3438 2023-06-18 16:33:27.000000 WebtoonScraper-0.1.0/WebtoonScraper/Webtoon.py
--rw-rw-rw-   0        0        0      501 2023-06-06 00:44:55.000000 WebtoonScraper-0.1.0/WebtoonScraper/WebtoonCanvasScraper.py
--rw-rw-rw-   0        0        0     4250 2023-06-17 07:29:55.000000 WebtoonScraper-0.1.0/WebtoonScraper/WebtoonOriginalsScraper.py
--rw-rw-rw-   0        0        0      568 2023-06-18 16:21:17.000000 WebtoonScraper-0.1.0/WebtoonScraper/__init__.py
--rw-rw-rw-   0        0        0     9473 2023-05-17 13:49:27.000000 WebtoonScraper-0.1.0/WebtoonScraper/foldermanagement.py
-drwxrwxrwx   0        0        0        0 2023-06-19 04:11:05.383954 WebtoonScraper-0.1.0/WebtoonScraper.egg-info/
--rw-rw-rw-   0        0        0     6717 2023-06-19 04:11:05.000000 WebtoonScraper-0.1.0/WebtoonScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-06-19 04:11:05.000000 WebtoonScraper-0.1.0/WebtoonScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 04:11:05.000000 WebtoonScraper-0.1.0/WebtoonScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-0.1.0/WebtoonScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       29 2023-06-19 04:11:05.000000 WebtoonScraper-0.1.0/WebtoonScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-19 04:11:05.000000 WebtoonScraper-0.1.0/WebtoonScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    29088 2023-06-06 01:18:53.000000 WebtoonScraper-0.1.0/number_from_manhwakyung.png
--rw-rw-rw-   0        0        0       42 2023-06-19 04:11:05.387356 WebtoonScraper-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1747 2023-06-19 04:10:53.000000 WebtoonScraper-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 04:11:05.384959 WebtoonScraper-0.1.0/test/
--rw-rw-rw-   0        0        0      131 2023-06-18 16:21:20.000000 WebtoonScraper-0.1.0/test/test.py
--rw-rw-rw-   0        0        0   182776 2023-05-29 08:43:24.000000 WebtoonScraper-0.1.0/title_no_from_webtoons.com.png
--rw-rw-rw-   0        0        0    52914 2023-05-15 00:27:14.000000 WebtoonScraper-0.1.0/titleid_from_nw.png
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

### Comparing `WebtoonScraper-0.1.0/LICENSE` & `WebtoonScraper-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0/PKG-INFO` & `WebtoonScraper-0.1.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 0.1.0
+Version: 0.1.0a1
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: Webtoon,Webtoon Scraper,Never Webtoon,Webtoon Downloader,Download Webtoon
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.
 # WebtoonScraper
 
 웹툰을 다운로드하는 프로젝트입니다. 그 외에도 웹툰 모아서 보기 등 몇 가지 편의 기능을 지원합니다.
@@ -115,18 +115,12 @@
 
 우선 작가가 설정한 회차 번호에 맞추는 것은 힘듭니다. 우선 번호가 어디에 있을지 알기 어렵고, 프롤로그가 있을지 없을지 알 수 없으며, 여러 화에 걸쳐 같은 에피소드를 진행하는 경우도 있고, 외전으로 본편의 회차에서 분리된 화를 운영하는 경우가 있어 화에 맞추어서 번호를 정하는 것을 어렵습니다.
 1부터 시작해서 끝까지 일정한 번호를 유지하는 것도 고려해볼 만하나 만약 그렇게 된다면 무결성 체크를 사용하기 어렵게 됩니다.
 따라서 작가가 설정한 회차를 그대로 사용하는 것도 어렵고, 만약 가능하다 할 지라도 무결성 체크를 포기하기 어렵기 때문에 현재는 ID를 회차 번호로 사용하고 있습니다.
 
 ## 전 버전과의 차이
 
-0.1.0: 버프툰 추가, 빠진 부분 재추가
-
 0.0.19.3: merge 속성 추가, get_webtoon 함수로 변경
-
 0.0.19.1: pbar에 표시되는 내용 변경, 내부적 개선
-
 0.0.18: 만화경 지원, 리팩토링됨(Scraper Abstract Base Class 추가)
-
 0.0.17: 웹툰즈 오리지널, 캔버스 지원
-
 0.0.12: 네이버 웹툰, 베스트 도전 지원
```

### Comparing `WebtoonScraper-0.1.0/README.md` & `WebtoonScraper-0.1.0a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -97,18 +97,12 @@
 
 우선 작가가 설정한 회차 번호에 맞추는 것은 힘듭니다. 우선 번호가 어디에 있을지 알기 어렵고, 프롤로그가 있을지 없을지 알 수 없으며, 여러 화에 걸쳐 같은 에피소드를 진행하는 경우도 있고, 외전으로 본편의 회차에서 분리된 화를 운영하는 경우가 있어 화에 맞추어서 번호를 정하는 것을 어렵습니다.
 1부터 시작해서 끝까지 일정한 번호를 유지하는 것도 고려해볼 만하나 만약 그렇게 된다면 무결성 체크를 사용하기 어렵게 됩니다.
 따라서 작가가 설정한 회차를 그대로 사용하는 것도 어렵고, 만약 가능하다 할 지라도 무결성 체크를 포기하기 어렵기 때문에 현재는 ID를 회차 번호로 사용하고 있습니다.
 
 ## 전 버전과의 차이
 
-0.1.0: 버프툰 추가, 빠진 부분 재추가
-
 0.0.19.3: merge 속성 추가, get_webtoon 함수로 변경
-
 0.0.19.1: pbar에 표시되는 내용 변경, 내부적 개선
-
 0.0.18: 만화경 지원, 리팩토링됨(Scraper Abstract Base Class 추가)
-
 0.0.17: 웹툰즈 오리지널, 캔버스 지원
-
 0.0.12: 네이버 웹툰, 베스트 도전 지원
```

### Comparing `WebtoonScraper-0.1.0/WebtoonScraper/BestChallengeScraper.py` & `WebtoonScraper-0.1.0a1/WebtoonScraper/BestChallengeScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0/WebtoonScraper/BufftoonScraper.py` & `WebtoonScraper-0.1.0a1/WebtoonScraper/BufftoonScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0/WebtoonScraper/NaverWebtoonScraper.py` & `WebtoonScraper-0.1.0a1/WebtoonScraper/NaverWebtoonScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0/WebtoonScraper/Scraper.py` & `WebtoonScraper-0.1.0a1/WebtoonScraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0/WebtoonScraper/TelescopeScraper.py` & `WebtoonScraper-0.1.0a1/WebtoonScraper/TelescopeScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0/WebtoonScraper/Webtoon.py` & `WebtoonScraper-0.1.0a1/WebtoonScraper/Webtoon.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0/WebtoonScraper/WebtoonOriginalsScraper.py` & `WebtoonScraper-0.1.0a1/WebtoonScraper/WebtoonOriginalsScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0/WebtoonScraper/__init__.py` & `WebtoonScraper-0.1.0a1/WebtoonScraper/__init__.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0/WebtoonScraper/foldermanagement.py` & `WebtoonScraper-0.1.0a1/WebtoonScraper/foldermanagement.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0/WebtoonScraper.egg-info/PKG-INFO` & `WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 0.1.0
+Version: 0.1.0a1
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: Webtoon,Webtoon Scraper,Never Webtoon,Webtoon Downloader,Download Webtoon
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.
 # WebtoonScraper
 
 웹툰을 다운로드하는 프로젝트입니다. 그 외에도 웹툰 모아서 보기 등 몇 가지 편의 기능을 지원합니다.
@@ -115,18 +115,12 @@
 
 우선 작가가 설정한 회차 번호에 맞추는 것은 힘듭니다. 우선 번호가 어디에 있을지 알기 어렵고, 프롤로그가 있을지 없을지 알 수 없으며, 여러 화에 걸쳐 같은 에피소드를 진행하는 경우도 있고, 외전으로 본편의 회차에서 분리된 화를 운영하는 경우가 있어 화에 맞추어서 번호를 정하는 것을 어렵습니다.
 1부터 시작해서 끝까지 일정한 번호를 유지하는 것도 고려해볼 만하나 만약 그렇게 된다면 무결성 체크를 사용하기 어렵게 됩니다.
 따라서 작가가 설정한 회차를 그대로 사용하는 것도 어렵고, 만약 가능하다 할 지라도 무결성 체크를 포기하기 어렵기 때문에 현재는 ID를 회차 번호로 사용하고 있습니다.
 
 ## 전 버전과의 차이
 
-0.1.0: 버프툰 추가, 빠진 부분 재추가
-
 0.0.19.3: merge 속성 추가, get_webtoon 함수로 변경
-
 0.0.19.1: pbar에 표시되는 내용 변경, 내부적 개선
-
 0.0.18: 만화경 지원, 리팩토링됨(Scraper Abstract Base Class 추가)
-
 0.0.17: 웹툰즈 오리지널, 캔버스 지원
-
 0.0.12: 네이버 웹툰, 베스트 도전 지원
```

### Comparing `WebtoonScraper-0.1.0/WebtoonScraper.egg-info/SOURCES.txt` & `WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0/number_from_manhwakyung.png` & `WebtoonScraper-0.1.0a1/number_from_manhwakyung.png`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0/setup.py` & `WebtoonScraper-0.1.0a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from setuptools import setup, find_packages
 
+# this_directory = Path(__file__).parent
+# long_description = (this_directory / "README.md").read_text()
+
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = '이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.\n'
     long_description += f.read()
     long_description = long_description.replace('titleid_from_nw.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/titleid_from_nw.png')
     long_description = long_description.replace('title_no_from_webtoons.com.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/title_no_from_webtoons.com.png')
     long_description = long_description.replace('number_from_manhwakyung.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/number_from_manhwakyung.png')
 
 setup(
     name='WebtoonScraper',
-    version='0.1.0',
+    version='0.1.0-alpha1',
     description='Scraping webtoons and some utils for it',
     author='ilotoki0804',
     author_email='ilotoki0804@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/ilotoki0804/WebtoonScraper',
     install_requires=['tqdm', 'bs4', 'requests', 'better_abc'],
     packages=find_packages(exclude=[]),
     keywords=['Webtoon', 'Webtoon Scraper', 'Never Webtoon', 'Webtoon Downloader', 'Download Webtoon'],
-    python_requires='>=3.10',
+    python_requires='>=3.8',
     package_data={},
     zip_safe=False,
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
```

### Comparing `WebtoonScraper-0.1.0/title_no_from_webtoons.com.png` & `WebtoonScraper-0.1.0a1/title_no_from_webtoons.com.png`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0/titleid_from_nw.png` & `WebtoonScraper-0.1.0a1/titleid_from_nw.png`

 * *Files identical despite different names*

