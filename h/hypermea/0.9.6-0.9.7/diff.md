# Comparing `tmp/hypermea-0.9.6-py3-none-any.whl.zip` & `tmp/hypermea-0.9.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 145402 bytes, number of entries: 108
+Zip file size: 145416 bytes, number of entries: 108
 -rw-rw-rw-  2.0 fat     5354 b- defN 23-Jun-18 15:26 hypermea/__init__.py
 -rw-rw-rw-  2.0 fat      138 b- defN 23-May-09 20:38 hypermea/addins/__init__.py
 -rw-rw-rw-  2.0 fat     2357 b- defN 23-Jun-18 15:28 hypermea/addins/auth.py
 -rw-rw-rw-  2.0 fat     1857 b- defN 23-Jun-18 15:26 hypermea/addins/docker.py
 -rw-rw-rw-  2.0 fat     2621 b- defN 23-Jun-18 15:26 hypermea/addins/git.py
 -rw-rw-rw-  2.0 fat     6331 b- defN 23-Jun-18 15:26 hypermea/addins/serverless.py
 -rw-rw-rw-  2.0 fat     2521 b- defN 23-Jun-18 15:28 hypermea/addins/validation.py
@@ -98,13 +98,13 @@
 -rw-rw-rw-  2.0 fat     4286 b- defN 23-Jan-13 14:25 hypermea/skel/win_service/win_service.ico
 -rw-rw-rw-  2.0 fat     1243 b- defN 23-Jun-18 15:28 hypermea/skel/win_service/win_service.py
 -rw-rw-rw-  2.0 fat       36 b- defN 23-Jan-13 14:25 hypermea/skel/win_service/svc-tools/off.bat
 -rw-rw-rw-  2.0 fat       37 b- defN 23-Jan-13 14:25 hypermea/skel/win_service/svc-tools/on.bat
 -rw-rw-rw-  2.0 fat       35 b- defN 23-Jan-13 14:25 hypermea/skel/win_service/svc-tools/query.bat
 -rw-rw-rw-  2.0 fat      573 b- defN 23-Jan-13 14:25 hypermea/skel/win_service/svc-tools/svc-install.bat
 -rw-rw-rw-  2.0 fat      273 b- defN 23-Jan-13 14:25 hypermea/skel/win_service/svc-tools/svc-uninstall.bat
--rw-rw-rw-  2.0 fat    20433 b- defN 23-Jun-19 03:03 hypermea-0.9.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-19 03:03 hypermea-0.9.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-19 03:03 hypermea-0.9.6.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-19 03:03 hypermea-0.9.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     9958 b- defN 23-Jun-19 03:03 hypermea-0.9.6.dist-info/RECORD
-108 files, 330044 bytes uncompressed, 129370 bytes compressed:  60.8%
+-rw-rw-rw-  2.0 fat    20429 b- defN 23-Jun-19 12:11 hypermea-0.9.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-19 12:11 hypermea-0.9.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-19 12:11 hypermea-0.9.7.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-19 12:11 hypermea-0.9.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     9958 b- defN 23-Jun-19 12:11 hypermea-0.9.7.dist-info/RECORD
+108 files, 330040 bytes uncompressed, 129384 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -303,23 +303,23 @@
 
 Filename: hypermea/skel/win_service/svc-tools/svc-install.bat
 Comment: 
 
 Filename: hypermea/skel/win_service/svc-tools/svc-uninstall.bat
 Comment: 
 
-Filename: hypermea-0.9.6.dist-info/METADATA
+Filename: hypermea-0.9.7.dist-info/METADATA
 Comment: 
 
-Filename: hypermea-0.9.6.dist-info/WHEEL
+Filename: hypermea-0.9.7.dist-info/WHEEL
 Comment: 
 
-Filename: hypermea-0.9.6.dist-info/entry_points.txt
+Filename: hypermea-0.9.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: hypermea-0.9.6.dist-info/top_level.txt
+Filename: hypermea-0.9.7.dist-info/top_level.txt
 Comment: 
 
-Filename: hypermea-0.9.6.dist-info/RECORD
+Filename: hypermea-0.9.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `hypermea-0.9.6.dist-info/METADATA` & `hypermea-0.9.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypermea
-Version: 0.9.6
+Version: 0.9.7
 Summary: Templates and scripts to rapidly spin up a production-ready Eve-based API.
 Home-page: https://github.com/pointw-dev/hypermea
 Author: Michael Ottoson
 Author-email: michael@pointw.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -17,17 +17,17 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Requires-Dist: libcst
 Requires-Dist: inflect
 Requires-Dist: click
 
 # hypermea
-Templates and scripts to rapidly spin up a production-ready Eve-based API.
+A toolkit for creating production-ready hypermedia APIs based on Eve/Flask.
 
-> **Please note**:  although I currently use these tools to create production-ready APIs, the tools themselves are still under development.  Use at your own risk.  This doc is under a heavy rewrite.  Information here is correct, but there are gaps and it's messy.
+> **Please note**:  although we currently use this toolkit to create production-ready APIs, the toolkit is still under development.  Use at your own risk.  This doc is under a heavy rewrite.  Information here is mostly correct, but there are gaps and it's messy.
 
 
 
 ## Introduction
 
 [Eve](https://docs.python-eve.org/en/stable/) is amazing.  The full power of Flask/Python, optimized for an API over mongodb.  Nice.
 
@@ -614,17 +614,17 @@
   90x - integration
   901 - integration already exists
   902 - name required when choosing empty integration
 
  100x - affordances
  1001 - affordance already exists
  1002 - affordance does not exist
+
   
-  
-  
+
 * organized folder structure
   - designed with more than simple api in mind (e.g. scripts)
   - src, doc, etc
   - FAQ why my-api/src/my-api ?
   - domain decomposition
   - hooks
```

## Comparing `hypermea-0.9.6.dist-info/RECORD` & `hypermea-0.9.7.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -97,12 +97,12 @@
 hypermea/skel/win_service/win_service.ico,sha256=LRSGigbw67cpnXU3trYMkwRYvJMJkjugiQYm9CsYnTI,4286
 hypermea/skel/win_service/win_service.py,sha256=-9EGOUJN6rLOYdm51nLGsp9KWnPrCI_Vd7mGy00ilpQ,1243
 hypermea/skel/win_service/svc-tools/off.bat,sha256=rLkN06zJrd-wvr2ZkxtK7ZdGWQyqHoPYN49j2DZKwO4,36
 hypermea/skel/win_service/svc-tools/on.bat,sha256=M42_C-NypskcxmObBSHZxX4ZLDPapC4CiiINI6kvoCM,37
 hypermea/skel/win_service/svc-tools/query.bat,sha256=8Kho3qBB1VOplnQaWkwhFMVpqf9W8dvbDuZDw30tBaQ,35
 hypermea/skel/win_service/svc-tools/svc-install.bat,sha256=5CuefcczanDAjiRjxUSr25KbDd9pTyuwzXnpKEDo0gE,573
 hypermea/skel/win_service/svc-tools/svc-uninstall.bat,sha256=nZr85Son7dzj489dWxciUQoXXXdalc5PF5TGnjmM-2c,273
-hypermea-0.9.6.dist-info/METADATA,sha256=FZYa5HX_Bfu8EZAldFqwYFZv-dJe5dK__JPD3T6uk6Q,20433
-hypermea-0.9.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-hypermea-0.9.6.dist-info/entry_points.txt,sha256=CwKD4WSfHfjX9BhpgzuPDmxYog8q9Z7LOu276BnmjQk,92
-hypermea-0.9.6.dist-info/top_level.txt,sha256=9bzOoz1VUgvzpAkl1_a-mzlZAMlcpfCvoOxIAkdxBPA,9
-hypermea-0.9.6.dist-info/RECORD,,
+hypermea-0.9.7.dist-info/METADATA,sha256=JgOxkHr-4JdxFbCsAxXTs8D47E8xtMosKp6AxVG3W_4,20429
+hypermea-0.9.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+hypermea-0.9.7.dist-info/entry_points.txt,sha256=CwKD4WSfHfjX9BhpgzuPDmxYog8q9Z7LOu276BnmjQk,92
+hypermea-0.9.7.dist-info/top_level.txt,sha256=9bzOoz1VUgvzpAkl1_a-mzlZAMlcpfCvoOxIAkdxBPA,9
+hypermea-0.9.7.dist-info/RECORD,,
```

