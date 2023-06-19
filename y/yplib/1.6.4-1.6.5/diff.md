# Comparing `tmp/yplib-1.6.4.tar.gz` & `tmp/yplib-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.6.4.tar", last modified: Mon Jun 19 01:15:10 2023, max compression
+gzip compressed data, was "dist\yplib-1.6.5.tar", last modified: Mon Jun 19 01:34:20 2023, max compression
```

## Comparing `yplib-1.6.4.tar` & `yplib-1.6.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 01:15:10.800145 yplib-1.6.4/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.6.4/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-19 01:15:10.799622 yplib-1.6.4/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.6.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 01:15:10.800145 yplib-1.6.4/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-19 01:15:06.000000 yplib-1.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:15:10.796371 yplib-1.6.4/yplib/
--rw-rw-rw-   0        0        0      355 2023-06-19 01:15:00.000000 yplib-1.6.4/yplib/__init__.py
--rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.6.4/yplib/chart.py
--rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.6.4/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.6.4/yplib/file.py
--rw-rw-rw-   0        0        0     1577 2023-06-19 01:13:34.000000 yplib-1.6.4/yplib/http_util.py
--rw-rw-rw-   0        0        0    24344 2023-06-19 00:55:36.000000 yplib-1.6.4/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:15:10.798639 yplib-1.6.4/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-19 01:15:10.000000 yplib-1.6.4/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-19 01:15:10.000000 yplib-1.6.4/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 01:15:10.000000 yplib-1.6.4/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 01:15:10.000000 yplib-1.6.4/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 01:34:20.162084 yplib-1.6.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.6.5/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-19 01:34:20.161652 yplib-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 01:34:20.162084 yplib-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-19 01:33:47.000000 yplib-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:34:20.158059 yplib-1.6.5/yplib/
+-rw-rw-rw-   0        0        0      355 2023-06-19 01:15:00.000000 yplib-1.6.5/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.6.5/yplib/chart.py
+-rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.6.5/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.6.5/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.6.5/yplib/http_util.py
+-rw-rw-rw-   0        0        0    24344 2023-06-19 00:55:36.000000 yplib-1.6.5/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:34:20.161140 yplib-1.6.5/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-19 01:34:20.000000 yplib-1.6.5/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-19 01:34:20.000000 yplib-1.6.5/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 01:34:20.000000 yplib-1.6.5/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 01:34:20.000000 yplib-1.6.5/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.6.4/LICENSE` & `yplib-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.6.4/setup.py` & `yplib-1.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.6.4",
+  version="1.6.5",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.6.4/yplib/chart.py` & `yplib-1.6.5/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.4/yplib/chart_html.py` & `yplib-1.6.5/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.4/yplib/file.py` & `yplib-1.6.5/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.4/yplib/http_util.py` & `yplib-1.6.5/yplib/http_util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from yplib.index import *
 from bs4 import BeautifulSoup
 import requests
+
+
 # from requests.packages.urllib3.exceptions import InsecureRequestWarning
 
 
 # 有关 http 的工具类
 
 # 解析 html 中的数据
 # file_path :   html 文件的路径
@@ -28,23 +30,72 @@
 #     num = td[0].text
 #     fun_name = td[1].select('a')[0].text
 #     fun_desc = td[1].text.replace(fun_name, '')
 #     print(f'{num} : {fun_name} , {fun_desc}')
 
 
 # get 类型的请求
-# headers :
-# cookie  :
-# auth    :
-# verify  :
+# session : session , 默认 : requests.session()
+# headers : headers
+# cookie  : cookie
+# auth    : auth
+# verify  : verify
+# r_json : 返回的数据是否是一个 json 类型的数据
 def do_get(url=None,
+           session=None,
            headers=None,
            cookie=None,
            auth=None,
            timeout=10,
-           verify=False):
-    # requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
-    response = requests.get(url, headers=headers, auth=auth, timeout=timeout, verify=verify, cookies=cookie)
+           verify=False,
+           r_json=False):
+    if session is None:
+        session = requests.session()
+    requests.packages.urllib3.disable_warnings()
+    response = session.get(url=url, headers=headers, auth=auth, timeout=timeout, verify=verify, cookies=cookie)
     response.encoding = 'utf-8'
-    return response.text.strip()
+    return json.loads(response.text.strip()) if r_json else response.text.strip()
+
+
+# print(do_get('https://www.runoob.com/?s=sorted'))
+# print(do_get('http://10.6.180.156:18000/login/need'))
+# print(do_get('http://10.6.180.156:18000/login/need', r_json=True))
 
-# print(do_get('https://www.runoob.com/?s=sorted'))
+
+# get 类型的请求
+# data         : data post 体中的数据
+# is_form_data : 是否是 form 表单
+# headers : headers
+# cookie  : cookie
+# auth    : auth
+# verify  : verify
+# r_json : 返回的数据是否是一个 json 类型的数据
+def do_post(url=None,
+            data=None,
+            is_form_data=False,
+            session=None,
+            headers=None,
+            cookie=None,
+            auth=None,
+            timeout=10,
+            verify=False,
+            r_json=False):
+    # headers = {'Content-Type': 'application/x-www-form-urlencoded'}
+    # data = {}
+    # data['appkey'] = APP_KEY
+    # data['secretkey'] = SECRET_KEY
+    # data['content'] = content
+    # data['phone'] = obtainMobileIndonesia(mobile)
+    # requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
+    # response = requests.post(URL, headers=headers, verify=False, data=data)
+    # response.encoding = 'utf-8'
+    # text = response.text
+    # text = text.replace('\n', '')
+    # text = text.replace('\r', '')
+    # return text
+    if session is None:
+        session = requests.session()
+    requests.packages.urllib3.disable_warnings()
+    d = data if is_form_data else json.dumps(data)
+    response = session.post(url=url, data=d, headers=headers, auth=auth, timeout=timeout, verify=verify, cookies=cookie)
+    response.encoding = 'utf-8'
+    return json.loads(response.text.strip()) if r_json else response.text.strip()
```

### Comparing `yplib-1.6.4/yplib/index.py` & `yplib-1.6.5/yplib/index.py`

 * *Files identical despite different names*

