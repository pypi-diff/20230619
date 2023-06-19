# Comparing `tmp/kkyukkyuCrawler-1.0.3.tar.gz` & `tmp/kkyukkyuCrawler-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkyukkyuCrawler-1.0.3.tar", last modified: Mon Jun 19 01:59:11 2023, max compression
+gzip compressed data, was "kkyukkyuCrawler-1.1.0.tar", last modified: Mon Jun 19 03:17:43 2023, max compression
```

## Comparing `kkyukkyuCrawler-1.0.3.tar` & `kkyukkyuCrawler-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 01:59:11.973127 kkyukkyuCrawler-1.0.3/
--rw-rw-rw-   0        0        0     1083 2023-06-18 22:37:34.000000 kkyukkyuCrawler-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0    14387 2023-06-19 01:59:11.972128 kkyukkyuCrawler-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    13942 2023-06-19 01:43:35.000000 kkyukkyuCrawler-1.0.3/README.md
--rw-rw-rw-   0        0        0      180 2023-06-18 22:35:22.000000 kkyukkyuCrawler-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 01:59:11.973127 kkyukkyuCrawler-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-06-19 01:59:00.000000 kkyukkyuCrawler-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:59:11.950040 kkyukkyuCrawler-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 01:59:11.959451 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler/
--rw-rw-rw-   0        0        0      147 2023-06-18 23:56:07.000000 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler/__init__.py
--rw-rw-rw-   0        0        0    31068 2023-06-19 01:52:54.000000 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler/src.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:59:11.971212 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler.egg-info/
--rw-rw-rw-   0        0        0    14387 2023-06-19 01:59:11.000000 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-06-19 01:59:11.000000 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 01:59:11.000000 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-19 01:59:11.000000 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-19 01:59:11.000000 kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 03:17:43.181918 kkyukkyuCrawler-1.1.0/
+-rw-rw-rw-   0        0        0     1083 2023-06-18 22:37:34.000000 kkyukkyuCrawler-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    14673 2023-06-19 03:17:43.180923 kkyukkyuCrawler-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14228 2023-06-19 03:15:49.000000 kkyukkyuCrawler-1.1.0/README.md
+-rw-rw-rw-   0        0        0      180 2023-06-18 22:35:22.000000 kkyukkyuCrawler-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 03:17:43.181918 kkyukkyuCrawler-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      860 2023-06-19 03:16:12.000000 kkyukkyuCrawler-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:17:43.157933 kkyukkyuCrawler-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 03:17:43.170258 kkyukkyuCrawler-1.1.0/src/kkyukkyuCrawler/
+-rw-rw-rw-   0        0        0      147 2023-06-18 23:56:07.000000 kkyukkyuCrawler-1.1.0/src/kkyukkyuCrawler/__init__.py
+-rw-rw-rw-   0        0        0    31068 2023-06-19 01:52:54.000000 kkyukkyuCrawler-1.1.0/src/kkyukkyuCrawler/src.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:17:43.178964 kkyukkyuCrawler-1.1.0/src/kkyukkyuCrawler.egg-info/
+-rw-rw-rw-   0        0        0    14673 2023-06-19 03:17:43.000000 kkyukkyuCrawler-1.1.0/src/kkyukkyuCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-06-19 03:17:43.000000 kkyukkyuCrawler-1.1.0/src/kkyukkyuCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 03:17:43.000000 kkyukkyuCrawler-1.1.0/src/kkyukkyuCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-19 03:17:43.000000 kkyukkyuCrawler-1.1.0/src/kkyukkyuCrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-19 03:17:43.000000 kkyukkyuCrawler-1.1.0/src/kkyukkyuCrawler.egg-info/top_level.txt
```

### Comparing `kkyukkyuCrawler-1.0.3/LICENSE.txt` & `kkyukkyuCrawler-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kkyukkyuCrawler-1.0.3/PKG-INFO` & `kkyukkyuCrawler-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: kkyukkyuCrawler
-Version: 1.0.3
+Version: 1.1.0
 Summary: law case crawling lib
 Home-page: https://github.com/eik4862/kkyukkyuCrawler
 Author: eik4862
 Author-email: lkd1962@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # 뀨뀨 크롤러(kkyukkyuCrawler)
+
 > 강의안에서 판례요지 따기를 손쉽게!
 
 뀨뀨 크롤러는 PDF 강의안의 판례번호(예: 1234다12345)를 자동으로 인식해서 [casenote](https://casenote.kr/)로부터 해당 판례를 검색한 후, 
 판례 정보를 긁어다가 txt 파일로 만들어주는 파이썬 라이브러리입니다.
 
 ## 설치
 ### 의존성
@@ -41,14 +42,17 @@
     git clone https://github.com/eik4862/kkyukkyuCrawler.git
 ```
 
 ## 사용법 - 기초
 `extract_and_export` 메소드에 입력할 PDF의 경로(`in.pdf`)와 출력할 txt의 경로(`out.txt`)를 넘겨주면 끝! 
 당연히 PDF 경로가 유효하지 않으면 에러가 나고, 출력할 경로에 이미 해당 파일이 있는 경우에는 **경고 없이 덮어쓰기가 되니 주의해주세요.**
 
+casenote 서버에 부담을 주지 않기 위해 0.5초에 하나의 판례를 검색하며, 경우에 따라 20초의 검색중단(timeout)이 발생합니다.
+다만, 검색할 판례의 수가 10개 이하이면 고속 모드로 전환하여 빠르게 검색을 마칩니다.
+
 ```python
     import kkyukkyuCrawler as kc
     kc.extract_and_export('in.pdf', 'out.txt')
 ```
 
 > **주의** PDF는 텍스트 형식이어야 하고, 암호화 되어있으면 안됩니다.
 > 즉, PDF의 텍스트 부분을 드래그해서 다른 곳에 복사-붙여넣기가 가능해야 합니다.
```

### Comparing `kkyukkyuCrawler-1.0.3/README.md` & `kkyukkyuCrawler-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # 뀨뀨 크롤러(kkyukkyuCrawler)
+
 > 강의안에서 판례요지 따기를 손쉽게!
 
 뀨뀨 크롤러는 PDF 강의안의 판례번호(예: 1234다12345)를 자동으로 인식해서 [casenote](https://casenote.kr/)로부터 해당 판례를 검색한 후, 
 판례 정보를 긁어다가 txt 파일로 만들어주는 파이썬 라이브러리입니다.
 
 ## 설치
 ### 의존성
@@ -27,14 +28,17 @@
     git clone https://github.com/eik4862/kkyukkyuCrawler.git
 ```
 
 ## 사용법 - 기초
 `extract_and_export` 메소드에 입력할 PDF의 경로(`in.pdf`)와 출력할 txt의 경로(`out.txt`)를 넘겨주면 끝! 
 당연히 PDF 경로가 유효하지 않으면 에러가 나고, 출력할 경로에 이미 해당 파일이 있는 경우에는 **경고 없이 덮어쓰기가 되니 주의해주세요.**
 
+casenote 서버에 부담을 주지 않기 위해 0.5초에 하나의 판례를 검색하며, 경우에 따라 20초의 검색중단(timeout)이 발생합니다.
+다만, 검색할 판례의 수가 10개 이하이면 고속 모드로 전환하여 빠르게 검색을 마칩니다.
+
 ```python
     import kkyukkyuCrawler as kc
     kc.extract_and_export('in.pdf', 'out.txt')
 ```
 
 > **주의** PDF는 텍스트 형식이어야 하고, 암호화 되어있으면 안됩니다.
 > 즉, PDF의 텍스트 부분을 드래그해서 다른 곳에 복사-붙여넣기가 가능해야 합니다.
```

### Comparing `kkyukkyuCrawler-1.0.3/setup.py` & `kkyukkyuCrawler-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kkyukkyuCrawler",
-    version="1.0.3",
+    version="1.1.0",
     author="eik4862",
     author_email="lkd1962@naver.com",
     description="law case crawling lib",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/eik4862/kkyukkyuCrawler",
     project_urls={},
```

### Comparing `kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler/src.py` & `kkyukkyuCrawler-1.1.0/src/kkyukkyuCrawler/src.py`

 * *Files identical despite different names*

### Comparing `kkyukkyuCrawler-1.0.3/src/kkyukkyuCrawler.egg-info/PKG-INFO` & `kkyukkyuCrawler-1.1.0/src/kkyukkyuCrawler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: kkyukkyuCrawler
-Version: 1.0.3
+Version: 1.1.0
 Summary: law case crawling lib
 Home-page: https://github.com/eik4862/kkyukkyuCrawler
 Author: eik4862
 Author-email: lkd1962@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # 뀨뀨 크롤러(kkyukkyuCrawler)
+
 > 강의안에서 판례요지 따기를 손쉽게!
 
 뀨뀨 크롤러는 PDF 강의안의 판례번호(예: 1234다12345)를 자동으로 인식해서 [casenote](https://casenote.kr/)로부터 해당 판례를 검색한 후, 
 판례 정보를 긁어다가 txt 파일로 만들어주는 파이썬 라이브러리입니다.
 
 ## 설치
 ### 의존성
@@ -41,14 +42,17 @@
     git clone https://github.com/eik4862/kkyukkyuCrawler.git
 ```
 
 ## 사용법 - 기초
 `extract_and_export` 메소드에 입력할 PDF의 경로(`in.pdf`)와 출력할 txt의 경로(`out.txt`)를 넘겨주면 끝! 
 당연히 PDF 경로가 유효하지 않으면 에러가 나고, 출력할 경로에 이미 해당 파일이 있는 경우에는 **경고 없이 덮어쓰기가 되니 주의해주세요.**
 
+casenote 서버에 부담을 주지 않기 위해 0.5초에 하나의 판례를 검색하며, 경우에 따라 20초의 검색중단(timeout)이 발생합니다.
+다만, 검색할 판례의 수가 10개 이하이면 고속 모드로 전환하여 빠르게 검색을 마칩니다.
+
 ```python
     import kkyukkyuCrawler as kc
     kc.extract_and_export('in.pdf', 'out.txt')
 ```
 
 > **주의** PDF는 텍스트 형식이어야 하고, 암호화 되어있으면 안됩니다.
 > 즉, PDF의 텍스트 부분을 드래그해서 다른 곳에 복사-붙여넣기가 가능해야 합니다.
```

