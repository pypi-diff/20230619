# Comparing `tmp/kkyukkyuCrawler-1.0.0.tar.gz` & `tmp/kkyukkyuCrawler-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkyukkyuCrawler-1.0.0.tar", last modified: Sun Jun 18 23:21:39 2023, max compression
+gzip compressed data, was "kkyukkyuCrawler-1.0.2.tar", last modified: Mon Jun 19 01:46:55 2023, max compression
```

## Comparing `kkyukkyuCrawler-1.0.0.tar` & `kkyukkyuCrawler-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 23:21:39.595683 kkyukkyuCrawler-1.0.0/
--rw-rw-rw-   0        0        0     1083 2023-06-18 22:37:34.000000 kkyukkyuCrawler-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1988 2023-06-18 23:21:39.594751 kkyukkyuCrawler-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1587 2023-06-18 23:20:44.000000 kkyukkyuCrawler-1.0.0/README.md
--rw-rw-rw-   0        0        0      180 2023-06-18 22:35:22.000000 kkyukkyuCrawler-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 23:21:39.595683 kkyukkyuCrawler-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      818 2023-06-18 22:36:50.000000 kkyukkyuCrawler-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 23:21:39.561796 kkyukkyuCrawler-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 23:21:39.581592 kkyukkyuCrawler-1.0.0/src/kkyukkyuCrawler/
--rw-rw-rw-   0        0        0      133 2023-06-18 22:33:02.000000 kkyukkyuCrawler-1.0.0/src/kkyukkyuCrawler/__init__.py
--rw-rw-rw-   0        0        0    31113 2023-06-18 22:31:28.000000 kkyukkyuCrawler-1.0.0/src/kkyukkyuCrawler/src.py
-drwxrwxrwx   0        0        0        0 2023-06-18 23:21:39.592643 kkyukkyuCrawler-1.0.0/src/kkyukkyuCrawler.egg-info/
--rw-rw-rw-   0        0        0     1988 2023-06-18 23:21:39.000000 kkyukkyuCrawler-1.0.0/src/kkyukkyuCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-06-18 23:21:39.000000 kkyukkyuCrawler-1.0.0/src/kkyukkyuCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 23:21:39.000000 kkyukkyuCrawler-1.0.0/src/kkyukkyuCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-18 23:21:39.000000 kkyukkyuCrawler-1.0.0/src/kkyukkyuCrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-18 23:21:39.000000 kkyukkyuCrawler-1.0.0/src/kkyukkyuCrawler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 01:46:55.789935 kkyukkyuCrawler-1.0.2/
+-rw-rw-rw-   0        0        0     1083 2023-06-18 22:37:34.000000 kkyukkyuCrawler-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    14387 2023-06-19 01:46:55.789935 kkyukkyuCrawler-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    13942 2023-06-19 01:43:35.000000 kkyukkyuCrawler-1.0.2/README.md
+-rw-rw-rw-   0        0        0      180 2023-06-18 22:35:22.000000 kkyukkyuCrawler-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 01:46:55.790935 kkyukkyuCrawler-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      860 2023-06-19 01:46:21.000000 kkyukkyuCrawler-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:46:55.763965 kkyukkyuCrawler-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 01:46:55.778923 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler/
+-rw-rw-rw-   0        0        0      147 2023-06-18 23:56:07.000000 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler/__init__.py
+-rw-rw-rw-   0        0        0    31089 2023-06-19 01:45:18.000000 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler/src.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:46:55.787954 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler.egg-info/
+-rw-rw-rw-   0        0        0    14387 2023-06-19 01:46:55.000000 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-06-19 01:46:55.000000 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 01:46:55.000000 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-19 01:46:55.000000 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-19 01:46:55.000000 kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler.egg-info/top_level.txt
```

### Comparing `kkyukkyuCrawler-1.0.0/LICENSE.txt` & `kkyukkyuCrawler-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kkyukkyuCrawler-1.0.0/setup.py` & `kkyukkyuCrawler-1.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kkyukkyuCrawler",
-    version="1.0.0",
+    version="1.0.2",
     author="eik4862",
     author_email="lkd1962@naver.com",
     description="law case crawling lib",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="",
+    url="https://github.com/eik4862/kkyukkyuCrawler",
     project_urls={},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
```

### Comparing `kkyukkyuCrawler-1.0.0/src/kkyukkyuCrawler/src.py` & `kkyukkyuCrawler-1.0.2/src/kkyukkyuCrawler/src.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     PRIVATE INSTANCE PARAMS
         - _id: Case ID (e.g. 1234다12345)
         - _ref_pg_no: The position (page #) where the case ID appears
         - _title: Case title (e.g. 대법원 2023. 6. 29. 선고 1234다12345 판결)
         - _issues: 판시/결정사항
         - _summaries: 판결/결정요지
         - _results: 주문
-        - _claims: 청구/항소/반소취지 등
+        - _claims: 청구/항소/반소 등 취지
         - _reasons: 이유
         - _src: The URL used for the GET request to obtain case data
     """
     _id: str
     _ref_pg_no: List[int]
     _title: Optional[str]
     _issues: Optional[List[str]]
@@ -231,14 +231,15 @@
                 j: int = 0
                 while j < len(cases):
                     if cases[j].id == _id:
                         if cases[j].ref_pg_no[-1] == pg_no:
                             break
                         else:
                             cases[j].add_ref_pg_no(pg_no)
+                            break
                     j += 1
                 if j == len(cases):
                     cases.append(Case(_id, pg_no))
             if verbose:
                 if len(curr_pg_ids) == 0:
                     Printer.report_w_desc(f'page {pg_no + 1}', 'not found', 1)
                 elif len(curr_pg_ids) > 4:
@@ -572,19 +573,17 @@
         :param soup: The BS object containing the response of the GET request
         :type soup: BeautifulSoup
 
         :return: The parsed title
         :rtype: str
         """
         title: str = soup.select_one('div.cn-case-title > h1').text.strip()
-        trim_pos = title.find('판결')
-        if trim_pos == -1:
-            trim_pos = title.find('결정')
+        trim_pos = title.find('[')
         assert trim_pos != -1
-        return cls._prettify(title[:trim_pos + 2])
+        return cls._prettify(title[:trim_pos - 1])
 
     @classmethod
     def _parse_issues(cls, soup: BeautifulSoup) -> Optional[List[str]]:
         """
         Parse issues from the GET response.
 
         :param soup: The BS object containing the response of the GET request
@@ -623,17 +622,18 @@
         :type soup: BeautifulSoup
 
         :return: The list of parsed results
         :rtype: list of str
         """
         results: List[str] = []
         cand: ResultSet = soup.select_one('div.cn-case-body').find_all('p', recursive=False)
+        print(cand)
         i: int = 0
         while i < len(cand):
-            if re.sub(r'\s{2,}', '', cand[i].text) == '주문':
+            if re.sub(r'\s+', '', cand[i].text) == '주문':
                 break
             i += 1
         assert i + 1 < len(cand)
         i += 1
         while i < len(cand):
             if cand[i]['class'][0] != 'main-sentence':
                 break
```

