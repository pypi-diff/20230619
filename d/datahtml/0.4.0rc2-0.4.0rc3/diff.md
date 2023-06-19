# Comparing `tmp/datahtml-0.4.0rc2.tar.gz` & `tmp/datahtml-0.4.0rc3.tar.gz`

## Comparing `datahtml-0.4.0rc2.tar` & `datahtml-0.4.0rc3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/.pylintrc
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/Makefile
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/mypy.ini
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/readthedocs.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/__about__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/_utils.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/base.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/crawler.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/defaults.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/errors.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/google.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/google_trends.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/news.py
--rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/parsers.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/rss.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/sitemap.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/types.py
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/web.py
--rw-r--r--   0        0        0    10774 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/youtube.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/apis/__init__.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/apis/youtube.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/Makefile
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/api_reference.rst
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/conf.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/make.bat
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/api/crawler.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/api/sitemap.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/api/types.rst
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/api/web.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/__init__.py
--rw-r--r--   0        0        0   264417 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/google_search.html
--rw-r--r--   0        0        0    29868 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/google_trends_rss.xml
--rw-r--r--   0        0        0   284678 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/lanacion_article.html
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/robots.txt
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/root_carrefour_sitemap.xml
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/test_apis_youtube.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/test_google.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/test_google_trends.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/test_root.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/test_youtube.py
--rw-r--r--   0        0        0   333386 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_channel.html
--rw-r--r--   0        0        0    19929 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_channel_rss.xml
--rw-r--r--   0        0        0   568777 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_search.html
--rw-r--r--   0        0        0    29235 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_search_response.json
--rw-r--r--   0        0        0   597066 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_video.html
--rw-r--r--   0        0        0   295956 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_video.json
--rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_video_multiple_ids.json
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_video_response.json
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/.gitignore
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/LICENSE
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/README.md
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/pyproject.toml
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/.pylintrc
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/Makefile
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/mypy.ini
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/readthedocs.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/__about__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/_utils.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/base.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/crawler.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/defaults.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/errors.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/google.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/google_trends.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/news.py
+-rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/parsers.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/rss.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/sitemap.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/types.py
+-rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/web.py
+-rw-r--r--   0        0        0    10774 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/youtube.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/apis/__init__.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/datahtml/apis/youtube.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/docs/Makefile
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/docs/api_reference.rst
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/docs/conf.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/docs/make.bat
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/docs/api/crawler.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/docs/api/sitemap.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/docs/api/types.rst
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/docs/api/web.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/__init__.py
+-rw-r--r--   0        0        0   264417 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/google_search.html
+-rw-r--r--   0        0        0    29868 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/google_trends_rss.xml
+-rw-r--r--   0        0        0   284678 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/lanacion_article.html
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/robots.txt
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/root_carrefour_sitemap.xml
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/test_apis_youtube.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/test_google.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/test_google_trends.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/test_root.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/test_youtube.py
+-rw-r--r--   0        0        0   333386 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/youtube_channel.html
+-rw-r--r--   0        0        0    19929 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/youtube_channel_rss.xml
+-rw-r--r--   0        0        0   568777 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/youtube_search.html
+-rw-r--r--   0        0        0    29235 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/youtube_search_response.json
+-rw-r--r--   0        0        0   597066 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/youtube_video.html
+-rw-r--r--   0        0        0   295956 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/youtube_video.json
+-rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/youtube_video_multiple_ids.json
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/tests/youtube_video_response.json
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/.gitignore
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/LICENSE
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/README.md
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 datahtml-0.4.0rc3/PKG-INFO
```

### Comparing `datahtml-0.4.0rc2/.pylintrc` & `datahtml-0.4.0rc3/.pylintrc`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/datahtml/base.py` & `datahtml-0.4.0rc3/datahtml/base.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/datahtml/crawler.py` & `datahtml-0.4.0rc3/datahtml/crawler.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/datahtml/defaults.py` & `datahtml-0.4.0rc3/datahtml/defaults.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/datahtml/errors.py` & `datahtml-0.4.0rc3/datahtml/errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,7 +20,15 @@
         super().__init__(msg)
 
 
 class RobotsTxtNotFound(Exception):
     def __init__(self, url):
         msg = f"robots.txt file not found for {url}"
         super().__init__(msg)
+
+
+class CrawlingError(Exception):
+    def __init__(self, url, status):
+        msg = f"Error crawling url {url} with status {status}"
+        super().__init__(msg)
+
+
```

### Comparing `datahtml-0.4.0rc2/datahtml/google.py` & `datahtml-0.4.0rc3/datahtml/google.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/datahtml/google_trends.py` & `datahtml-0.4.0rc3/datahtml/google_trends.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/datahtml/news.py` & `datahtml-0.4.0rc3/datahtml/news.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/datahtml/parsers.py` & `datahtml-0.4.0rc3/datahtml/parsers.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/datahtml/rss.py` & `datahtml-0.4.0rc3/datahtml/rss.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/datahtml/sitemap.py` & `datahtml-0.4.0rc3/datahtml/sitemap.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/datahtml/types.py` & `datahtml-0.4.0rc3/datahtml/types.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/datahtml/web.py` & `datahtml-0.4.0rc3/datahtml/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,28 +107,32 @@
 
 
 def download(
     url: str,
     *,
     crawler: CrawlerSpec,
     is_root=True,
+    raise_when_not_200=True,
 ) -> WebDocument:
     """
     It crawls the url passed.
 
     :param url: url to crawl
     :type url: str
     :param crawler: A class:`CrawlerSpec` implementation.
     :type crawler: CrawlerSpec
     :param is_root: if it's a root site or not.
     :type is_root: bool
     :return: A web object.
     :rtype: WebDocument
     """
     rsp = crawler.get(url)
+    if raise_when_not_200 and rsp.status_code != 200:
+        raise errors.CrawlingError(url=url, status=rsp.status_code)
+
     w = WebDocument(url=url, html_txt=rsp.text, is_root=is_root)
     return w
 
 
 def build_sitemap(
     url: str, *, crawler: CrawlerSpec, filter_dt: int = 1
 ) -> List[sitemap.SitemapLink]:
```

### Comparing `datahtml-0.4.0rc2/datahtml/youtube.py` & `datahtml-0.4.0rc3/datahtml/youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/datahtml/apis/youtube.py` & `datahtml-0.4.0rc3/datahtml/apis/youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/docs/Makefile` & `datahtml-0.4.0rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/docs/conf.py` & `datahtml-0.4.0rc3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/docs/index.rst` & `datahtml-0.4.0rc3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/docs/make.bat` & `datahtml-0.4.0rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/tests/google_search.html` & `datahtml-0.4.0rc3/tests/google_search.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/tests/google_trends_rss.xml` & `datahtml-0.4.0rc3/tests/google_trends_rss.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/tests/lanacion_article.html` & `datahtml-0.4.0rc3/tests/lanacion_article.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/tests/root_carrefour_sitemap.xml` & `datahtml-0.4.0rc3/tests/root_carrefour_sitemap.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/tests/test_apis_youtube.py` & `datahtml-0.4.0rc3/tests/test_apis_youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/tests/test_youtube.py` & `datahtml-0.4.0rc3/tests/test_youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/tests/youtube_channel.html` & `datahtml-0.4.0rc3/tests/youtube_channel.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/tests/youtube_channel_rss.xml` & `datahtml-0.4.0rc3/tests/youtube_channel_rss.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/tests/youtube_search.html` & `datahtml-0.4.0rc3/tests/youtube_search.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/tests/youtube_search_response.json` & `datahtml-0.4.0rc3/tests/youtube_search_response.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/tests/youtube_video.html` & `datahtml-0.4.0rc3/tests/youtube_video.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/tests/youtube_video.json` & `datahtml-0.4.0rc3/tests/youtube_video.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/tests/youtube_video_multiple_ids.json` & `datahtml-0.4.0rc3/tests/youtube_video_multiple_ids.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/tests/youtube_video_response.json` & `datahtml-0.4.0rc3/tests/youtube_video_response.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/.gitignore` & `datahtml-0.4.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/LICENSE` & `datahtml-0.4.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/README.md` & `datahtml-0.4.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/pyproject.toml` & `datahtml-0.4.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc2/PKG-INFO` & `datahtml-0.4.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datahtml
-Version: 0.4.0rc2
+Version: 0.4.0rc3
 Summary: A lib to work with html and web data
 Project-URL: Documentation, https://github.com/algorinfo/datahtml#readme
 Project-URL: Issues, https://github.com/algorinfo/datahtml/issues
 Project-URL: Source, https://github.com/algorinfo/datahtml
 Author-email: Xavier Petit <nuxion@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

