# Comparing `tmp/fbn-0.0.5-py3-none-any.whl.zip` & `tmp/fbn-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 8154 bytes, number of entries: 12
--rw-r--r--  2.0 unx       81 b- defN 23-Jun-19 14:13 fbn/__init__.py
--rw-r--r--  2.0 unx       61 b- defN 23-Jun-19 14:13 fbn/__main__.py
--rw-r--r--  2.0 unx     2550 b- defN 23-Jun-19 14:13 fbn/cli.py
--rw-r--r--  2.0 unx       78 b- defN 23-Jun-19 14:13 fbn/constants.py
--rw-r--r--  2.0 unx      406 b- defN 23-Jun-19 14:13 fbn/exceptions.py
--rw-r--r--  2.0 unx     6898 b- defN 23-Jun-19 14:13 fbn/fb.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Jun-19 14:13 fbn-0.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     4355 b- defN 23-Jun-19 14:13 fbn-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 14:13 fbn-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       42 b- defN 23-Jun-19 14:13 fbn-0.0.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Jun-19 14:13 fbn-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      873 b- defN 23-Jun-19 14:13 fbn-0.0.5.dist-info/RECORD
-12 files, 16505 bytes uncompressed, 6706 bytes compressed:  59.4%
+Zip file size: 8112 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       81 b- defN 23-Jun-19 15:36 fbn/__init__.py
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-19 15:36 fbn/__main__.py
+-rw-r--r--  2.0 unx     2550 b- defN 23-Jun-19 15:36 fbn/cli.py
+-rw-r--r--  2.0 unx       78 b- defN 23-Jun-19 15:36 fbn/constants.py
+-rw-r--r--  2.0 unx      406 b- defN 23-Jun-19 15:36 fbn/exceptions.py
+-rw-r--r--  2.0 unx     6789 b- defN 23-Jun-19 15:36 fbn/fb.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jun-19 15:37 fbn-0.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4355 b- defN 23-Jun-19 15:37 fbn-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 15:37 fbn-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-19 15:37 fbn-0.0.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-19 15:37 fbn-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      873 b- defN 23-Jun-19 15:37 fbn-0.0.6.dist-info/RECORD
+12 files, 16396 bytes uncompressed, 6664 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: fbn/exceptions.py
 Comment: 
 
 Filename: fbn/fb.py
 Comment: 
 
-Filename: fbn-0.0.5.dist-info/LICENSE
+Filename: fbn-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: fbn-0.0.5.dist-info/METADATA
+Filename: fbn-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: fbn-0.0.5.dist-info/WHEEL
+Filename: fbn-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: fbn-0.0.5.dist-info/entry_points.txt
+Filename: fbn-0.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: fbn-0.0.5.dist-info/top_level.txt
+Filename: fbn-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: fbn-0.0.5.dist-info/RECORD
+Filename: fbn-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbn/__init__.py

```diff
@@ -1,3 +1,3 @@
 __author__ = "Visesh Prasad"
 __email__ = "visesh@live.com"
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

## fbn/fb.py

```diff
@@ -45,15 +45,14 @@
     wait=wait_chain(wait_fixed(600), wait_fixed(700), wait_fixed(800)),
     reraise=True,
     before=before_log(logger, logging.DEBUG),
     after=after_log(logger, logging.DEBUG),
 )
 def get_latest_posts(**kwargs):
     sample_count = kwargs.pop("sample_count")
-    ban_count = 0
     posts = {}
     try:
         for post in get_posts(**kwargs):
             post_id = post["post_id"]
             posts[post_id] = {
                 "text": post["text"],
                 "post_text": post["post_text"],
@@ -63,17 +62,15 @@
                 "username": post["username"],
             }
             logger.debug(f"Obtained post {post_id}")
             if len(posts) == sample_count:
                 logger.debug(f"Stopping with {sample_count} posts...")
                 break
     except (TemporarilyBanned, AccountDisabled) as e:
-        ban_count += 1
         raise e
-    logger.debug(f"You were banned {ban_count} times temporarily.")
     return posts
 
 
 def notify(apprise_url, title, body):
     app_obj = apprise.Apprise()
     app_obj.add(apprise_url)
     app_obj.notify(
```

## Comparing `fbn-0.0.5.dist-info/LICENSE` & `fbn-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fbn-0.0.5.dist-info/METADATA` & `fbn-0.0.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbn
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tool to monitor fb groups and notify
 Home-page: https://github.com/viseshrp/fbn
 Author: Visesh Prasad
 Author-email: visesh@live.com
 Maintainer: Visesh Prasad
 Maintainer-email: visesh@live.com
 License: MIT license
```

## Comparing `fbn-0.0.5.dist-info/RECORD` & `fbn-0.0.6.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-fbn/__init__.py,sha256=DGCsuKEHr6eK5XHJ6LWRc39_Vml46ksl3EFkRA20nz8,81
+fbn/__init__.py,sha256=EC4HyVHS-jdvoWCetXzqOIAk4DkJsJEdDqkLrNT8jK4,81
 fbn/__main__.py,sha256=MSmt_5Xg84uHqzTN38JwgseJK8rsJn_11A8WD99VtEo,61
 fbn/cli.py,sha256=7jjZTa6ZYPMWoAEs54XEHkttfxbE7UnqLe-SH6Zo-Y4,2550
 fbn/constants.py,sha256=cMQzDOJVV3vm3P1UqY1DKpB5OfhLdT5fbLEM6tAu6l8,78
 fbn/exceptions.py,sha256=8yan1cmPUJEbiTW12adRoyWF48zb3L2SCKEW1trobyA,406
-fbn/fb.py,sha256=PvzbjAbRFYpi1LDVNWd097gm1wtoSakAQKYdyPyeja8,6898
-fbn-0.0.5.dist-info/LICENSE,sha256=25qEHPeTSJTu_3MheLT2jl_taHxPcxlaORhLfxGDbTU,1065
-fbn-0.0.5.dist-info/METADATA,sha256=af07dPmhqVPZ_vHJGjcc2BKsF1Xjo4vBxbgz214d7F4,4355
-fbn-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fbn-0.0.5.dist-info/entry_points.txt,sha256=PjZFFzJbekNwM2i-9gSHHb6eQsIP6NRMgcoF98ysoZM,42
-fbn-0.0.5.dist-info/top_level.txt,sha256=Cekq2PfsBF7azxMgcSBWbU_elQ_WUTGuY37h4zY5Cu8,4
-fbn-0.0.5.dist-info/RECORD,,
+fbn/fb.py,sha256=JKurcWL8q8Ok1XMiXAO-Y64VSacXInBZN86teuYnFAU,6789
+fbn-0.0.6.dist-info/LICENSE,sha256=25qEHPeTSJTu_3MheLT2jl_taHxPcxlaORhLfxGDbTU,1065
+fbn-0.0.6.dist-info/METADATA,sha256=J3n_XHwbPFKu_mWkNJSu7QLi095_bu4tgNJiar6QW6M,4355
+fbn-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fbn-0.0.6.dist-info/entry_points.txt,sha256=PjZFFzJbekNwM2i-9gSHHb6eQsIP6NRMgcoF98ysoZM,42
+fbn-0.0.6.dist-info/top_level.txt,sha256=Cekq2PfsBF7azxMgcSBWbU_elQ_WUTGuY37h4zY5Cu8,4
+fbn-0.0.6.dist-info/RECORD,,
```

