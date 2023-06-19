# Comparing `tmp/fbn-0.0.4-py3-none-any.whl.zip` & `tmp/fbn-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 8120 bytes, number of entries: 12
--rw-r--r--  2.0 unx       81 b- defN 23-Feb-04 16:04 fbn/__init__.py
--rw-r--r--  2.0 unx       61 b- defN 23-Feb-04 16:04 fbn/__main__.py
--rw-r--r--  2.0 unx     2571 b- defN 23-Feb-04 16:04 fbn/cli.py
--rw-r--r--  2.0 unx       78 b- defN 23-Feb-04 16:04 fbn/constants.py
--rw-r--r--  2.0 unx      406 b- defN 23-Feb-04 16:04 fbn/exceptions.py
--rw-r--r--  2.0 unx     6761 b- defN 23-Feb-04 16:04 fbn/fb.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Feb-04 16:05 fbn-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     4370 b- defN 23-Feb-04 16:05 fbn-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-04 16:05 fbn-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       42 b- defN 23-Feb-04 16:05 fbn-0.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Feb-04 16:05 fbn-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      873 b- defN 23-Feb-04 16:05 fbn-0.0.4.dist-info/RECORD
-12 files, 16404 bytes uncompressed, 6672 bytes compressed:  59.3%
+Zip file size: 8154 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       81 b- defN 23-Jun-19 14:13 fbn/__init__.py
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-19 14:13 fbn/__main__.py
+-rw-r--r--  2.0 unx     2550 b- defN 23-Jun-19 14:13 fbn/cli.py
+-rw-r--r--  2.0 unx       78 b- defN 23-Jun-19 14:13 fbn/constants.py
+-rw-r--r--  2.0 unx      406 b- defN 23-Jun-19 14:13 fbn/exceptions.py
+-rw-r--r--  2.0 unx     6898 b- defN 23-Jun-19 14:13 fbn/fb.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jun-19 14:13 fbn-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4355 b- defN 23-Jun-19 14:13 fbn-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 14:13 fbn-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-19 14:13 fbn-0.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-19 14:13 fbn-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      873 b- defN 23-Jun-19 14:13 fbn-0.0.5.dist-info/RECORD
+12 files, 16505 bytes uncompressed, 6706 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: fbn/exceptions.py
 Comment: 
 
 Filename: fbn/fb.py
 Comment: 
 
-Filename: fbn-0.0.4.dist-info/LICENSE
+Filename: fbn-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: fbn-0.0.4.dist-info/METADATA
+Filename: fbn-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: fbn-0.0.4.dist-info/WHEEL
+Filename: fbn-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: fbn-0.0.4.dist-info/entry_points.txt
+Filename: fbn-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: fbn-0.0.4.dist-info/top_level.txt
+Filename: fbn-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: fbn-0.0.4.dist-info/RECORD
+Filename: fbn-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbn/__init__.py

```diff
@@ -1,3 +1,3 @@
 __author__ = "Visesh Prasad"
 __email__ = "visesh@live.com"
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

## fbn/cli.py

```diff
@@ -68,16 +68,15 @@
     help="Number of posts to sample",
 )
 @click.option(
     "-e",
     "--every",
     "frequency",
     type=str,
-    default="1h",
-    show_default=True,
+    required=False,
     help="Monitor frequency",
 )
 @click.option(
     "-a",
     "--apprise-url",
     type=str,
     required=True,
```

## fbn/fb.py

```diff
@@ -190,16 +190,19 @@
         if username is not None and password is not None:
             kwargs["credentials"] = (username, password)
         else:
             raise NoAuthInfoException(
                 "Please provide your Facebook username/password or a cookies file."
             )
 
-    interval, unit = parse_frequency(frequency)
-    schedule_unit = SCHEDULE_UNIT_MAP[unit]
     logger.debug("Creating schedule...")
-    job = getattr(schedule.every(int(interval)), schedule_unit).do(monitor_fb, **kwargs)
+    if frequency:
+        interval, unit = parse_frequency(frequency)
+        schedule_unit = SCHEDULE_UNIT_MAP[unit]
+        job = getattr(schedule.every(int(interval)), schedule_unit).do(monitor_fb, **kwargs)
+    else:  # randomize as the default
+        job = schedule.every(2).to(4).hours.do(monitor_fb, **kwargs)
     logger.debug(f"Running once...")
     schedule.run_all()
     logger.debug(f"Starting schedule {job}...")
     while True:
         schedule.run_pending()
```

## Comparing `fbn-0.0.4.dist-info/LICENSE` & `fbn-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fbn-0.0.4.dist-info/METADATA` & `fbn-0.0.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbn
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool to monitor fb groups and notify
 Home-page: https://github.com/viseshrp/fbn
 Author: Visesh Prasad
 Author-email: visesh@live.com
 Maintainer: Visesh Prasad
 Maintainer-email: visesh@live.com
 License: MIT license
@@ -62,15 +62,15 @@
   -i, --id TEXT               The Facebook group name or id  [required]
   -u, --username TEXT         Your Facebook username
   -p, --password TEXT         Your Facebook password
   -c, --cookies-file FILE     Path to the Facebook cookies file  [default:
                               facebook.com_cookies.txt]
   -g, --user-agent TEXT       User agent to use for scraping
   -s, --sample-count INTEGER  Number of posts to sample  [default: 10]
-  -e, --every TEXT            Monitor frequency  [default: 1h]
+  -e, --every TEXT            Monitor frequency
   -a, --apprise-url TEXT      The apprise URL to notify  [required]
   -v, --verbose               Enable debug logging.
   -h, --help                  Show this message and exit.
 ```
 
 This uses [facebook-scraper](https://github.com/kevinzg/facebook-scraper) that scrapes the target group for posts.
 If the group is private, authentication is required as you must be a member,
```

