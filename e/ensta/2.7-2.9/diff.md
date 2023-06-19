# Comparing `tmp/ensta-2.7.tar.gz` & `tmp/ensta-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-2.7.tar", last modified: Sat Jun 17 10:14:03 2023, max compression
+gzip compressed data, was "ensta-2.9.tar", last modified: Mon Jun 19 09:36:05 2023, max compression
```

## Comparing `ensta-2.7.tar` & `ensta-2.9.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:14:03.922889 ensta-2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-17 10:13:54.000000 ensta-2.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-17 10:14:03.922889 ensta-2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-06-17 10:13:54.000000 ensta-2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:14:03.922889 ensta-2.7/ensta/
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-17 10:13:54.000000 ensta-2.7/ensta/Authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-06-17 10:13:54.000000 ensta-2.7/ensta/Guest.py
--rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-06-17 10:13:54.000000 ensta-2.7/ensta/Host.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-17 10:13:54.000000 ensta-2.7/ensta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:14:03.922889 ensta-2.7/ensta/containers/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/FollowPerson.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/FollowedStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/Post.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/PostUser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/Profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/ProfileHost.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/UnfollowedStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:14:03.922889 ensta-2.7/ensta/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-17 10:13:54.000000 ensta-2.7/ensta/lib/Commons.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-17 10:13:54.000000 ensta-2.7/ensta/lib/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-17 10:13:54.000000 ensta-2.7/ensta/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:14:03.922889 ensta-2.7/ensta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-17 10:14:03.000000 ensta-2.7/ensta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-17 10:14:03.000000 ensta-2.7/ensta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 10:14:03.000000 ensta-2.7/ensta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-17 10:14:03.000000 ensta-2.7/ensta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 10:14:03.000000 ensta-2.7/ensta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-17 10:14:03.922889 ensta-2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-17 10:13:54.000000 ensta-2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:36:05.372658 ensta-2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-19 09:35:54.000000 ensta-2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-19 09:36:05.372658 ensta-2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-06-19 09:35:54.000000 ensta-2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:36:05.368657 ensta-2.9/ensta/
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-19 09:35:54.000000 ensta-2.9/ensta/Authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-19 09:35:54.000000 ensta-2.9/ensta/AutoHost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-06-19 09:35:54.000000 ensta-2.9/ensta/Guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-06-19 09:35:54.000000 ensta-2.9/ensta/Host.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-19 09:35:54.000000 ensta-2.9/ensta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:36:05.368657 ensta-2.9/ensta/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 09:35:54.000000 ensta-2.9/ensta/containers/FollowPerson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-19 09:35:54.000000 ensta-2.9/ensta/containers/FollowedStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-19 09:35:54.000000 ensta-2.9/ensta/containers/Liker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-19 09:35:54.000000 ensta-2.9/ensta/containers/Likers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-19 09:35:54.000000 ensta-2.9/ensta/containers/Post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-19 09:35:54.000000 ensta-2.9/ensta/containers/PostUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-19 09:35:54.000000 ensta-2.9/ensta/containers/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-19 09:35:54.000000 ensta-2.9/ensta/containers/ProfileHost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-19 09:35:54.000000 ensta-2.9/ensta/containers/UnfollowedStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-19 09:35:54.000000 ensta-2.9/ensta/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:36:05.372658 ensta-2.9/ensta/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-19 09:35:54.000000 ensta-2.9/ensta/lib/Commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-19 09:35:54.000000 ensta-2.9/ensta/lib/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-19 09:35:54.000000 ensta-2.9/ensta/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:36:05.368657 ensta-2.9/ensta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-19 09:36:05.000000 ensta-2.9/ensta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-19 09:36:05.000000 ensta-2.9/ensta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:36:05.000000 ensta-2.9/ensta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-19 09:36:05.000000 ensta-2.9/ensta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 09:36:05.000000 ensta-2.9/ensta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-19 09:36:05.372658 ensta-2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-19 09:35:54.000000 ensta-2.9/setup.py
```

### Comparing `ensta-2.7/LICENSE.txt` & `ensta-2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-2.7/PKG-INFO` & `ensta-2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 2.7
+Version: 2.9
 Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.7.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.9.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram-client,instagram,api-wrapper,instagram-scraper,instagram-api,instagram-sdk,instagram-photos,instagram-api-python,instabot,instagram-stories,instagram-bot,instapy,instagram-downloader,instagram-account,instagram-crawler,instagram-private-api,igtv,instagram-automation,reels,instagram-feed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -27,16 +27,18 @@
 
 This package lets you use Instagram's Internal Web API through simple functions and classes. Ensta uses Instagram's Original Web API to scrape data which makes it a reliable choice over other third-party scrapers. This library mainly focuses on Simplicity & Reliability.
 
 Two type of classes are supported - ***Guest & Host***.
 
 [<img style="margin-top: 10px" src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="160"/>](https://buymeacoffee.com/diezo)
 
-## 📢 Announcement
-Users can now log in through their **Username** and **Password** to generate SessionId! [See this](https://github.com/diezo/ensta#:~:text=NewSessionID(%22username%22%2C%20%22password%22))
+## 📢 Announcements
+**[#02]** [AutoHost](https://github.com/diezo/ensta/) is released! Authentication update to the *Host Class*.
+
+**[#01]** Users can now log in through their **Username** and **Password** to generate SessionId! [See this](https://github.com/diezo/ensta#:~:text=NewSessionID(%22username%22%2C%20%22password%22))
 
 ## Installation
 To install this package using [Python's PIP](https://pypi.org/project/pip/), run this command in a terminal window:
 ```shell
 $ pip install ensta
 ```
```

### Comparing `ensta-2.7/README.md` & `ensta-2.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 
 This package lets you use Instagram's Internal Web API through simple functions and classes. Ensta uses Instagram's Original Web API to scrape data which makes it a reliable choice over other third-party scrapers. This library mainly focuses on Simplicity & Reliability.
 
 Two type of classes are supported - ***Guest & Host***.
 
 [<img style="margin-top: 10px" src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="160"/>](https://buymeacoffee.com/diezo)
 
-## 📢 Announcement
-Users can now log in through their **Username** and **Password** to generate SessionId! [See this](https://github.com/diezo/ensta#:~:text=NewSessionID(%22username%22%2C%20%22password%22))
+## 📢 Announcements
+**[#02]** [AutoHost](https://github.com/diezo/ensta/) is released! Authentication update to the *Host Class*.
+
+**[#01]** Users can now log in through their **Username** and **Password** to generate SessionId! [See this](https://github.com/diezo/ensta#:~:text=NewSessionID(%22username%22%2C%20%22password%22))
 
 ## Installation
 To install this package using [Python's PIP](https://pypi.org/project/pip/), run this command in a terminal window:
 ```shell
 $ pip install ensta
 ```
```

### Comparing `ensta-2.7/ensta/Authentication.py` & `ensta-2.9/ensta/Authentication.py`

 * *Files identical despite different names*

### Comparing `ensta-2.7/ensta/Guest.py` & `ensta-2.9/ensta/Guest.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     format_username,
     format_uid
 )
 from .lib.Exceptions import APIError
 from .containers.Profile import Profile
 from .containers.ProfileHost import ProfileHost
 import dataclasses
+from fake_useragent import UserAgent
 
 
 class Guest:
     request_session: requests.Session = None
     homepage_source: str = None
     insta_app_id: str = None
     csrf_token: str = None
@@ -39,21 +40,22 @@
         refresh_csrf_token(self)
         body_json = {
             "email": f"{username}@{self.csrf_token}.com",
             "username": username,
             "first_name": username.capitalize(),
             "opt_into_one_tap": False
         }
+        ua = UserAgent().random
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "content-type": "application/x-www-form-urlencoded",
             "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
+            "sec-ch-ua": ua,
+            "sec-ch-ua-full-version-list": ua,
             "sec-ch-ua-mobile": "?0",
             "sec-ch-ua-platform": "\"Windows\"",
             "sec-ch-ua-platform-version": "\"15.0.0\"",
             "sec-fetch-dest": "empty",
             "sec-fetch-mode": "cors",
             "sec-fetch-site": "same-origin",
             "viewport-width": "1475",
@@ -75,20 +77,21 @@
                 return "username" not in response_json["errors"]
         except JSONDecodeError:
             return None
 
     def profile(self, username: str, __session__: requests.Session | None = None) -> Profile | ProfileHost | None:
         username: str = format_username(username)
         refresh_csrf_token(self)
+        ua = UserAgent().random
         request_headers: dict = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
+            "sec-ch-ua": ua,
+            "sec-ch-ua-full-version-list": ua,
             "sec-ch-ua-mobile": "?0",
             "sec-ch-ua-platform": "\"Windows\"",
             "sec-ch-ua-platform-version": "\"15.0.0\"",
             "sec-fetch-dest": "empty",
             "sec-fetch-mode": "cors",
             "sec-fetch-site": "same-origin",
             "viewport-width": "1475",
@@ -103,15 +106,15 @@
 
         try:
             session: requests.Session = __session__
             if __session__ is None: session: requests.Session = self.request_session
 
             http_response: requests.Response = session.get(
                 f"https://www.instagram.com/api/v1/users/web_profile_info/?username={username}",
-                headers=request_headers
+                headers=request_headers,
             )
             response_json: dict = http_response.json()
 
             if "status" in response_json:
                 if response_json["status"] == "ok" and "data" in response_json:
                     if "user" in response_json["data"]:
                         try:
```

### Comparing `ensta-2.7/ensta/Host.py` & `ensta-2.9/ensta/Host.py`

 * *Files identical despite different names*

### Comparing `ensta-2.7/ensta/containers/PostUser.py` & `ensta-2.9/ensta/containers/PostUser.py`

 * *Files identical despite different names*

### Comparing `ensta-2.7/ensta/containers/Profile.py` & `ensta-2.9/ensta/containers/Profile.py`

 * *Files identical despite different names*

### Comparing `ensta-2.7/ensta/lib/Commons.py` & `ensta-2.9/ensta/lib/Commons.py`

 * *Files identical despite different names*

### Comparing `ensta-2.7/ensta/lib/Exceptions.py` & `ensta-2.9/ensta/lib/Exceptions.py`

 * *Files identical despite different names*

### Comparing `ensta-2.7/ensta.egg-info/PKG-INFO` & `ensta-2.9/ensta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 2.7
+Version: 2.9
 Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.7.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.9.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram-client,instagram,api-wrapper,instagram-scraper,instagram-api,instagram-sdk,instagram-photos,instagram-api-python,instabot,instagram-stories,instagram-bot,instapy,instagram-downloader,instagram-account,instagram-crawler,instagram-private-api,igtv,instagram-automation,reels,instagram-feed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -27,16 +27,18 @@
 
 This package lets you use Instagram's Internal Web API through simple functions and classes. Ensta uses Instagram's Original Web API to scrape data which makes it a reliable choice over other third-party scrapers. This library mainly focuses on Simplicity & Reliability.
 
 Two type of classes are supported - ***Guest & Host***.
 
 [<img style="margin-top: 10px" src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="160"/>](https://buymeacoffee.com/diezo)
 
-## 📢 Announcement
-Users can now log in through their **Username** and **Password** to generate SessionId! [See this](https://github.com/diezo/ensta#:~:text=NewSessionID(%22username%22%2C%20%22password%22))
+## 📢 Announcements
+**[#02]** [AutoHost](https://github.com/diezo/ensta/) is released! Authentication update to the *Host Class*.
+
+**[#01]** Users can now log in through their **Username** and **Password** to generate SessionId! [See this](https://github.com/diezo/ensta#:~:text=NewSessionID(%22username%22%2C%20%22password%22))
 
 ## Installation
 To install this package using [Python's PIP](https://pypi.org/project/pip/), run this command in a terminal window:
 ```shell
 $ pip install ensta
 ```
```

### Comparing `ensta-2.7/ensta.egg-info/SOURCES.txt` & `ensta-2.9/ensta.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 LICENSE.txt
 README.md
 setup.cfg
 setup.py
 ensta/Authentication.py
+ensta/AutoHost.py
 ensta/Guest.py
 ensta/Host.py
 ensta/__init__.py
 ensta.egg-info/PKG-INFO
 ensta.egg-info/SOURCES.txt
 ensta.egg-info/dependency_links.txt
 ensta.egg-info/requires.txt
 ensta.egg-info/top_level.txt
 ensta/containers/FollowPerson.py
 ensta/containers/FollowedStatus.py
+ensta/containers/Liker.py
+ensta/containers/Likers.py
 ensta/containers/Post.py
 ensta/containers/PostUser.py
 ensta/containers/Profile.py
 ensta/containers/ProfileHost.py
 ensta/containers/UnfollowedStatus.py
 ensta/containers/__init__.py
 ensta/lib/Commons.py
```

### Comparing `ensta-2.7/setup.py` & `ensta-2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ensta",
     packages=["ensta", "ensta.lib", "ensta.containers"],
-    version="2.7",
+    version="2.9",
     license="MIT",
     description="🔥 Fastest & Simplest Python Package For Instagram Automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
-    download_url="https://github.com/diezo/ensta/archive/refs/tags/v2.7.tar.gz",
+    download_url="https://github.com/diezo/ensta/archive/refs/tags/v2.9.tar.gz",
     keywords=["instagram-client", "instagram", "api-wrapper", "instagram-scraper", "instagram-api", "instagram-sdk", "instagram-photos", "instagram-api-python", "instabot", "instagram-stories", "instagram-bot", "instapy", "instagram-downloader", "instagram-account", "instagram-crawler", "instagram-private-api", "igtv", "instagram-automation", "reels", "instagram-feed"],
-    install_requires=["requests", "selenium"],
+    install_requires=["requests", "selenium", "fake-useragent"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10"
```

