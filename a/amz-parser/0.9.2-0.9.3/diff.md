# Comparing `tmp/amz_parser-0.9.2.tar.gz` & `tmp/amz_parser-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amz_parser-0.9.2.tar", last modified: Tue Jan  3 09:09:56 2023, max compression
+gzip compressed data, was "amz_parser-0.9.3.tar", last modified: Mon Jun 19 07:56:14 2023, max compression
```

## Comparing `amz_parser-0.9.2.tar` & `amz_parser-0.9.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-01-03 09:09:56.303545 amz_parser-0.9.2/
--rw-rw-rw-   0        0        0      172 2023-01-03 09:09:56.302559 amz_parser-0.9.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-01-03 09:09:56.295030 amz_parser-0.9.2/amz_parser/
--rw-rw-rw-   0        0        0       84 2022-12-08 05:54:53.000000 amz_parser-0.9.2/amz_parser/__init__.py
--rw-rw-rw-   0        0        0    36032 2023-01-03 09:00:01.000000 amz_parser-0.9.2/amz_parser/listing_parser.py
--rw-rw-rw-   0        0        0     7754 2022-11-04 03:23:05.000000 amz_parser-0.9.2/amz_parser/review_parser.py
-drwxrwxrwx   0        0        0        0 2023-01-03 09:09:56.301545 amz_parser-0.9.2/amz_parser.egg-info/
--rw-rw-rw-   0        0        0      172 2023-01-03 09:09:55.000000 amz_parser-0.9.2/amz_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-01-03 09:09:56.000000 amz_parser-0.9.2/amz_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-03 09:09:55.000000 amz_parser-0.9.2/amz_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-01-03 09:09:56.000000 amz_parser-0.9.2/amz_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-01-03 09:09:56.000000 amz_parser-0.9.2/amz_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-03 09:09:56.303545 amz_parser-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0      325 2023-01-03 09:01:14.000000 amz_parser-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:56:14.436353 amz_parser-0.9.3/
+-rw-rw-rw-   0        0        0      172 2023-06-19 07:56:14.436353 amz_parser-0.9.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 07:56:14.430259 amz_parser-0.9.3/amz_parser/
+-rw-rw-rw-   0        0        0       84 2022-12-08 05:54:53.000000 amz_parser-0.9.3/amz_parser/__init__.py
+-rw-rw-rw-   0        0        0    36032 2023-01-03 09:00:01.000000 amz_parser-0.9.3/amz_parser/listing_parser.py
+-rw-rw-rw-   0        0        0     7622 2023-06-19 07:38:24.000000 amz_parser-0.9.3/amz_parser/review_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:56:14.435099 amz_parser-0.9.3/amz_parser.egg-info/
+-rw-rw-rw-   0        0        0      172 2023-06-19 07:56:13.000000 amz_parser-0.9.3/amz_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-19 07:56:14.000000 amz_parser-0.9.3/amz_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 07:56:13.000000 amz_parser-0.9.3/amz_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-19 07:56:14.000000 amz_parser-0.9.3/amz_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 07:56:14.000000 amz_parser-0.9.3/amz_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 07:56:14.436353 amz_parser-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      325 2023-06-19 07:51:34.000000 amz_parser-0.9.3/setup.py
```

### Comparing `amz_parser-0.9.2/amz_parser/listing_parser.py` & `amz_parser-0.9.3/amz_parser/listing_parser.py`

 * *Files identical despite different names*

### Comparing `amz_parser-0.9.2/amz_parser/review_parser.py` & `amz_parser-0.9.3/amz_parser/review_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,23 +215,21 @@
         if review_text:
             return int(review_text[-1].replace(',', '').replace('.', ''))
 
     def parse_all(self):
         li = []
         for each in self.d('div[id][data-hook="review"]').items():
             comment_id = each.attr('id')
-            title = each('[data-hook="review-title"]').text()
+            title = each('[data-hook="review-title"] > span').text()
             content = each('span[data-hook="review-body"]').text()
             vp = '是' if each('span[data-hook="avp-badge"]') else '否'
             variant = each('a[data-hook="format-strip"]').text()
             asin = re.findall('product-reviews/(.*?)/', each('a[data-hook="format-strip"]').attr('href'))[
                 0] if variant else self.asin
-            rating = re.findall(r'[\d.]',
-                                each('i[data-hook="review-star-rating"],i[data-hook="cmps-review-star-rating"]').attr(
-                                    'class'))[0]
+            rating = each('i[data-hook="review-star-rating"]').text()[0]
             helpful_info = re.findall(r'[\d,.]+', each('span[data-hook="helpful-vote-statement"]').text())
             helpful = helpful_info[0] if helpful_info else 0
             name = each('.a-profile-name').text()
             country, comment_date = self.get_country_and_date(each)
             # 修复因国家没解析出来而导致的评论链接错误
             comment_url = 'https://{}/gp/customer-reviews/{}'.format(self.amazon_host_mapping[country],
                                                                      comment_id) if country != 'N.A.' else ''
```

