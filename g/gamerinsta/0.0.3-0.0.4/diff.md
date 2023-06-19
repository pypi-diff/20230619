# Comparing `tmp/gamerinsta-0.0.3.tar.gz` & `tmp/gamerinsta-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamerinsta-0.0.3.tar", last modified: Sat Jun 17 10:46:42 2023, max compression
+gzip compressed data, was "gamerinsta-0.0.4.tar", last modified: Mon Jun 19 05:00:52 2023, max compression
```

## Comparing `gamerinsta-0.0.3.tar` & `gamerinsta-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 10:46:42.855710 gamerinsta-0.0.3/
--rw-rw-rw-   0        0        0     1062 2023-05-25 19:08:15.000000 gamerinsta-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      617 2023-06-17 10:46:42.855710 gamerinsta-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-17 10:46:42.792712 gamerinsta-0.0.3/gamerinsta/
--rw-rw-rw-   0        0        0    11036 2023-06-17 10:43:23.000000 gamerinsta-0.0.3/gamerinsta/__init__.py
--rw-rw-rw-   0        0        0     6436 2023-06-17 10:28:19.000000 gamerinsta-0.0.3/gamerinsta/tokens.py
-drwxrwxrwx   0        0        0        0 2023-06-17 10:46:42.855710 gamerinsta-0.0.3/gamerinsta.egg-info/
--rw-rw-rw-   0        0        0      617 2023-06-17 10:46:42.000000 gamerinsta-0.0.3/gamerinsta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-06-17 10:46:42.000000 gamerinsta-0.0.3/gamerinsta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 10:46:42.000000 gamerinsta-0.0.3/gamerinsta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-06-17 10:46:42.000000 gamerinsta-0.0.3/gamerinsta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-17 10:46:42.000000 gamerinsta-0.0.3/gamerinsta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 10:46:42.855710 gamerinsta-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      918 2023-06-17 10:43:23.000000 gamerinsta-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:00:52.366630 gamerinsta-0.0.4/
+-rw-rw-rw-   0        0        0     1062 2023-05-25 19:08:15.000000 gamerinsta-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      617 2023-06-19 05:00:52.365336 gamerinsta-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 05:00:52.321596 gamerinsta-0.0.4/gamerinsta/
+-rw-rw-rw-   0        0        0    11037 2023-06-17 10:53:54.000000 gamerinsta-0.0.4/gamerinsta/__init__.py
+-rw-rw-rw-   0        0        0     6450 2023-06-19 04:58:46.000000 gamerinsta-0.0.4/gamerinsta/tokens.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:00:52.357788 gamerinsta-0.0.4/gamerinsta.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-06-19 05:00:52.000000 gamerinsta-0.0.4/gamerinsta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-06-19 05:00:52.000000 gamerinsta-0.0.4/gamerinsta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 05:00:52.000000 gamerinsta-0.0.4/gamerinsta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-06-19 05:00:52.000000 gamerinsta-0.0.4/gamerinsta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 05:00:52.000000 gamerinsta-0.0.4/gamerinsta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 05:00:52.367140 gamerinsta-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      918 2023-06-19 05:00:24.000000 gamerinsta-0.0.4/setup.py
```

### Comparing `gamerinsta-0.0.3/LICENSE` & `gamerinsta-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gamerinsta-0.0.3/PKG-INFO` & `gamerinsta-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamerinsta
-Version: 0.0.3
+Version: 0.0.4
 Summary: Instagram Android Api For Login 
 Author: Gamer
 Author-email: godxgamer0192@gmail.com
 Keywords: Instagram,login
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gamerinsta-0.0.3/gamerinsta/__init__.py` & `gamerinsta-0.0.4/gamerinsta/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
                     'signed_body': 'SIGNATURE.{"two_factor_identifier":"'+self.two_factor_identifier+'","username":"'+self.unnmm+'","guid":"'+self.Deviceid+'","device_id":"'+self.Androidid+'"}',
                 }
 
                 response = httpx.post('https://i.instagram.com/api/v1/accounts/send_two_factor_login_sms/',
                                          headers=self.headers, data=data)
                 if '"status": "ok"' in response.text:
                     value={'Response':'2FA Otp Sent On Your Number'}
-                    print(value)
+                    #print(value)
                     self.Otp=str(input("Enter Otp : "))
                     updict={'x-ig-nav-chain': f'TwoFacLoginVerifyFragment:two_fac:1:button:{round(time())}.{random.randint(111,999)}::,TwoFacLoginHelpSheetFragment:two_fac:2:button:{round(time())}.{random.randint(111,999)}::',}
                     self.headers = {key: updict.get(key, self.headers[key]) for key in self.headers}
                     data = {
                         'signed_body': 'SIGNATURE.{"verification_code":"'+str(self.Otp)+'","phone_id":"'+str(self.FDeviceid)+'","two_factor_identifier":"'+self.two_factor_identifier+'","username":"'+self.unnmm+'","trust_this_device":"1","guid":"'+self.Deviceid+'","device_id":"'+self.Androidid+'","waterfall_id":"'+self.Waterid+'","verification_method":"1"}',
                     }
```

### Comparing `gamerinsta-0.0.3/gamerinsta/tokens.py` & `gamerinsta-0.0.4/gamerinsta/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                                      data=data)
             self.urur = response.headers['ig-set-ig-u-rur'].split(':')[1]
             self.claim = response.headers['x-ig-set-www-claim']
             try:
                 self.shbid = response.headers['ig-set-ig-u-shbid']
                 self.igid = self.shbid.split(',')[0]
                 self.shbi=self.shbid.split(':')[1]
-                self.shbts = response.headers['ig-set-ig-u-shbts']
+                self.shbts = response.headers['ig-set-ig-u-shbts'].split(':')[1]
             except:
                 self.shbid=None
                 self.igid=None
                 self.shbi=None
                 self.shbts=None
```

### Comparing `gamerinsta-0.0.3/gamerinsta.egg-info/PKG-INFO` & `gamerinsta-0.0.4/gamerinsta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamerinsta
-Version: 0.0.3
+Version: 0.0.4
 Summary: Instagram Android Api For Login 
 Author: Gamer
 Author-email: godxgamer0192@gmail.com
 Keywords: Instagram,login
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gamerinsta-0.0.3/setup.py` & `gamerinsta-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Instagram Android Api For Login '
 LONG_DESCRIPTION = 'A python library that helps you to login in instagram do various task and automaiton'
 
 # Setting up
 setup(
     name="gamerinsta",
     version=VERSION,
```

