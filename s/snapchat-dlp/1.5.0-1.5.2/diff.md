# Comparing `tmp/snapchat-dlp-1.5.0.tar.gz` & `tmp/snapchat-dlp-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapchat-dlp-1.5.0.tar", last modified: Mon Jun 19 07:18:58 2023, max compression
+gzip compressed data, was "snapchat-dlp-1.5.2.tar", last modified: Mon Jun 19 09:07:10 2023, max compression
```

## Comparing `snapchat-dlp-1.5.0.tar` & `snapchat-dlp-1.5.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 07:18:58.349232 snapchat-dlp-1.5.0/
--rw-rw-rw-   0        0        0      170 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     1092 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/LICENSE
--rw-rw-rw-   0        0        0      318 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4945 2023-06-19 07:18:58.349232 snapchat-dlp-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3754 2023-06-19 07:07:33.000000 snapchat-dlp-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 07:18:58.275533 snapchat-dlp-1.5.0/docs/
--rw-rw-rw-   0        0        0      633 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/docs/authors.rst
--rw-rw-rw-   0        0        0     5093 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/docs/history.rst
--rw-rw-rw-   0        0        0      345 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/docs/index.rst
--rw-rw-rw-   0        0        0     1222 2023-06-19 07:07:33.000000 snapchat-dlp-1.5.0/docs/installation.rst
--rwxrwxrwx   0        0        0      810 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.0/docs/make.bat
--rw-rw-rw-   0        0        0       79 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.0/docs/modules.rst
--rw-rw-rw-   0        0        0       28 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/docs/readme.rst
--rw-rw-rw-   0        0        0      523 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.0/docs/snapchat_dl.rst
--rw-rw-rw-   0        0        0       93 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.0/docs/usage.rst
--rw-rw-rw-   0        0        0       29 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/requirements.txt
--rw-rw-rw-   0        0        0      364 2023-06-19 07:18:58.355068 snapchat-dlp-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     2084 2023-06-19 07:07:33.000000 snapchat-dlp-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:18:58.290186 snapchat-dlp-1.5.0/snapchat_dlp/
--rw-rw-rw-   0        0        0      200 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.0/snapchat_dlp/__init__.py
--rw-rw-rw-   0        0        0     2834 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.0/snapchat_dlp/app.py
--rw-rw-rw-   0        0        0     3231 2023-06-19 07:07:33.000000 snapchat-dlp-1.5.0/snapchat_dlp/cli.py
--rw-rw-rw-   0        0        0     1566 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.0/snapchat_dlp/downloader.py
--rw-rw-rw-   0        0        0     5103 2023-06-19 07:08:48.000000 snapchat-dlp-1.5.0/snapchat_dlp/snapchat_dlp.py
--rw-rw-rw-   0        0        0     4077 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.0/snapchat_dlp/utils.py
--rw-rw-rw-   0        0        0       23 2023-06-19 07:18:52.000000 snapchat-dlp-1.5.0/snapchat_dlp/version.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:18:58.316613 snapchat-dlp-1.5.0/snapchat_dlp.egg-info/
--rw-rw-rw-   0        0        0     4945 2023-06-19 07:18:57.000000 snapchat-dlp-1.5.0/snapchat_dlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1073 2023-06-19 07:18:58.000000 snapchat-dlp-1.5.0/snapchat_dlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 07:18:57.000000 snapchat-dlp-1.5.0/snapchat_dlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-06-19 07:18:57.000000 snapchat-dlp-1.5.0/snapchat_dlp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 07:17:46.000000 snapchat-dlp-1.5.0/snapchat_dlp.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-06-19 07:18:57.000000 snapchat-dlp-1.5.0/snapchat_dlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-19 07:18:57.000000 snapchat-dlp-1.5.0/snapchat_dlp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 07:18:58.330047 snapchat-dlp-1.5.0/tests/
--rw-rw-rw-   0        0        0       43 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:18:58.338186 snapchat-dlp-1.5.0/tests/mock_data/
-drwxrwxrwx   0        0        0        0 2023-06-19 07:18:58.339200 snapchat-dlp-1.5.0/tests/mock_data/23/
--rw-rw-rw-   0        0        0       75 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/tests/mock_data/23/.gitignore
--rw-rw-rw-   0        0        0    37579 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/tests/mock_data/api-error.html
--rw-rw-rw-   0        0        0       38 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/tests/mock_data/batch_file.txt
--rw-rw-rw-   0        0        0    36109 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/tests/mock_data/invalidusername-nostories.html
--rw-rw-rw-   0        0        0    37580 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/tests/mock_data/invalidusername.html
--rw-rw-rw-   0        0        0     2184 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/tests/mock_data/invalidusername.json
-drwxrwxrwx   0        0        0        0 2023-06-19 07:18:58.341472 snapchat-dlp-1.5.0/tests/mock_data/user.1name/
--rw-rw-rw-   0        0        0       75 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/tests/mock_data/user.1name/.gitignore
-drwxrwxrwx   0        0        0        0 2023-06-19 07:18:58.342491 snapchat-dlp-1.5.0/tests/mock_data/user1/
--rw-rw-rw-   0        0        0       75 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.0/tests/mock_data/user1/.gitignore
--rw-rw-rw-   0        0        0     1238 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.0/tests/test_downlaoder.py
--rw-rw-rw-   0        0        0     2506 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.0/tests/test_snapchat_dl.py
--rw-rw-rw-   0        0        0     1934 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.307494 snapchat-dlp-1.5.2/
+-rw-rw-rw-   0        0        0      170 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1092 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0      318 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4945 2023-06-19 09:07:10.307494 snapchat-dlp-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3754 2023-06-19 07:07:33.000000 snapchat-dlp-1.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.214755 snapchat-dlp-1.5.2/docs/
+-rw-rw-rw-   0        0        0      633 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/docs/authors.rst
+-rw-rw-rw-   0        0        0     5093 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/docs/history.rst
+-rw-rw-rw-   0        0        0      345 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/docs/index.rst
+-rw-rw-rw-   0        0        0     1222 2023-06-19 07:07:33.000000 snapchat-dlp-1.5.2/docs/installation.rst
+-rwxrwxrwx   0        0        0      810 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/docs/make.bat
+-rw-rw-rw-   0        0        0       79 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/docs/modules.rst
+-rw-rw-rw-   0        0        0       28 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/docs/readme.rst
+-rw-rw-rw-   0        0        0      523 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/docs/snapchat_dl.rst
+-rw-rw-rw-   0        0        0       93 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/docs/usage.rst
+-rw-rw-rw-   0        0        0       29 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/requirements.txt
+-rw-rw-rw-   0        0        0      364 2023-06-19 09:07:10.309534 snapchat-dlp-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     2084 2023-06-19 07:07:33.000000 snapchat-dlp-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.228648 snapchat-dlp-1.5.2/snapchat_dlp/
+-rw-rw-rw-   0        0        0      200 2023-06-19 08:48:53.000000 snapchat-dlp-1.5.2/snapchat_dlp/__init__.py
+-rw-rw-rw-   0        0        0     2834 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/snapchat_dlp/app.py
+-rw-rw-rw-   0        0        0     3231 2023-06-19 07:07:33.000000 snapchat-dlp-1.5.2/snapchat_dlp/cli.py
+-rw-rw-rw-   0        0        0     1566 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/snapchat_dlp/downloader.py
+-rw-rw-rw-   0        0        0     5147 2023-06-19 08:05:15.000000 snapchat-dlp-1.5.2/snapchat_dlp/snapchat_dlp.py
+-rw-rw-rw-   0        0        0     4077 2023-06-19 08:04:48.000000 snapchat-dlp-1.5.2/snapchat_dlp/utils.py
+-rw-rw-rw-   0        0        0       23 2023-06-19 09:07:04.000000 snapchat-dlp-1.5.2/snapchat_dlp/version.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.285177 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/
+-rw-rw-rw-   0        0        0     4945 2023-06-19 09:07:09.000000 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1073 2023-06-19 09:07:09.000000 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:07:09.000000 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-19 09:07:09.000000 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 07:17:46.000000 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-06-19 09:07:09.000000 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-19 09:07:09.000000 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.292179 snapchat-dlp-1.5.2/tests/
+-rw-rw-rw-   0        0        0       43 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.301880 snapchat-dlp-1.5.2/tests/mock_data/
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.302957 snapchat-dlp-1.5.2/tests/mock_data/23/
+-rw-rw-rw-   0        0        0       75 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/23/.gitignore
+-rw-rw-rw-   0        0        0    37579 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/api-error.html
+-rw-rw-rw-   0        0        0       38 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/batch_file.txt
+-rw-rw-rw-   0        0        0    36109 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/invalidusername-nostories.html
+-rw-rw-rw-   0        0        0    37580 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/invalidusername.html
+-rw-rw-rw-   0        0        0     2184 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/invalidusername.json
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.303979 snapchat-dlp-1.5.2/tests/mock_data/user.1name/
+-rw-rw-rw-   0        0        0       75 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/user.1name/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.306462 snapchat-dlp-1.5.2/tests/mock_data/user1/
+-rw-rw-rw-   0        0        0       75 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/user1/.gitignore
+-rw-rw-rw-   0        0        0     1238 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/tests/test_downlaoder.py
+-rw-rw-rw-   0        0        0     2506 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/tests/test_snapchat_dl.py
+-rw-rw-rw-   0        0        0     1934 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/tests/test_utils.py
```

### Comparing `snapchat-dlp-1.5.0/LICENSE` & `snapchat-dlp-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/PKG-INFO` & `snapchat-dlp-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapchat-dlp
-Version: 1.5.0
+Version: 1.5.2
 Summary: An update to snapchat-dlp, a Snapchat Public Stories Downloader.
 Home-page: https://github.com/Walmann/snapchat-dlp
 Author: Aakash Gajjar
 Author-email: skyqutip@gmail.com
 Maintainer: Walmann
 License: MIT license
 Project-URL: Original, https://github.com/skyme5/snapchat-dlp
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: snapchat-dlp Version: 1.5.0 Summary: An update to
+Metadata-Version: 2.1 Name: snapchat-dlp Version: 1.5.2 Summary: An update to
 snapchat-dlp, a Snapchat Public Stories Downloader. Home-page: https://
 github.com/Walmann/snapchat-dlp Author: Aakash Gajjar Author-email:
 skyqutip@gmail.com Maintainer: Walmann License: MIT license Project-URL:
 Original, https://github.com/skyme5/snapchat-dlp Project-URL: Source, https://
 github.com/Walmann/snapchat-dlp Keywords: snapchat-dlp Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
```

### Comparing `snapchat-dlp-1.5.0/README.md` & `snapchat-dlp-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/docs/Makefile` & `snapchat-dlp-1.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/docs/conf.py` & `snapchat-dlp-1.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/docs/installation.rst` & `snapchat-dlp-1.5.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/docs/make.bat` & `snapchat-dlp-1.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/docs/snapchat_dl.rst` & `snapchat-dlp-1.5.2/docs/snapchat_dl.rst`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/setup.py` & `snapchat-dlp-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/snapchat_dlp/app.py` & `snapchat-dlp-1.5.2/snapchat_dlp/app.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/snapchat_dlp/cli.py` & `snapchat-dlp-1.5.2/snapchat_dlp/cli.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/snapchat_dlp/downloader.py` & `snapchat-dlp-1.5.2/snapchat_dlp/downloader.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/snapchat_dlp/snapchat_dlp.py` & `snapchat-dlp-1.5.2/snapchat_dlp/snapchat_dlp.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
             def util_web_user_info(content: dict):
                 if "userProfile" in content["props"]["pageProps"]:
                     user_profile = content["props"]["pageProps"]["userProfile"]
                     field_id = user_profile["$case"]
                     return user_profile[field_id]
                 else:
-                    raise UserNotFoundError
+                    raise UserNotFoundError(f"Could not find Snapchat user {username}")
 
             def util_web_story(content: dict):
                 if "story" in content["props"]["pageProps"]:
                     return content["props"]["pageProps"]["story"]["snapList"]
                 return list()
 
             user_info = util_web_user_info(response_json)
```

### Comparing `snapchat-dlp-1.5.0/snapchat_dlp/utils.py` & `snapchat-dlp-1.5.2/snapchat_dlp/utils.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/snapchat_dlp.egg-info/PKG-INFO` & `snapchat-dlp-1.5.2/snapchat_dlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapchat-dlp
-Version: 1.5.0
+Version: 1.5.2
 Summary: An update to snapchat-dlp, a Snapchat Public Stories Downloader.
 Home-page: https://github.com/Walmann/snapchat-dlp
 Author: Aakash Gajjar
 Author-email: skyqutip@gmail.com
 Maintainer: Walmann
 License: MIT license
 Project-URL: Original, https://github.com/skyme5/snapchat-dlp
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: snapchat-dlp Version: 1.5.0 Summary: An update to
+Metadata-Version: 2.1 Name: snapchat-dlp Version: 1.5.2 Summary: An update to
 snapchat-dlp, a Snapchat Public Stories Downloader. Home-page: https://
 github.com/Walmann/snapchat-dlp Author: Aakash Gajjar Author-email:
 skyqutip@gmail.com Maintainer: Walmann License: MIT license Project-URL:
 Original, https://github.com/skyme5/snapchat-dlp Project-URL: Source, https://
 github.com/Walmann/snapchat-dlp Keywords: snapchat-dlp Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
```

### Comparing `snapchat-dlp-1.5.0/snapchat_dlp.egg-info/SOURCES.txt` & `snapchat-dlp-1.5.2/snapchat_dlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/tests/mock_data/api-error.html` & `snapchat-dlp-1.5.2/tests/mock_data/api-error.html`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/tests/mock_data/invalidusername-nostories.html` & `snapchat-dlp-1.5.2/tests/mock_data/invalidusername-nostories.html`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/tests/mock_data/invalidusername.html` & `snapchat-dlp-1.5.2/tests/mock_data/invalidusername.html`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/tests/mock_data/invalidusername.json` & `snapchat-dlp-1.5.2/tests/mock_data/invalidusername.json`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/tests/test_downlaoder.py` & `snapchat-dlp-1.5.2/tests/test_downlaoder.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/tests/test_snapchat_dl.py` & `snapchat-dlp-1.5.2/tests/test_snapchat_dl.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.0/tests/test_utils.py` & `snapchat-dlp-1.5.2/tests/test_utils.py`

 * *Files identical despite different names*

