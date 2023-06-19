# Comparing `tmp/MYPACKAGE123dpp-1.3.tar.gz` & `tmp/MYPACKAGE123dpp-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MYPACKAGE123dpp-1.3.tar", last modified: Fri Jun 16 19:21:21 2023, max compression
+gzip compressed data, was "MYPACKAGE123dpp-1.4.tar", last modified: Mon Jun 19 18:15:12 2023, max compression
```

## Comparing `MYPACKAGE123dpp-1.3.tar` & `MYPACKAGE123dpp-1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 19:21:21.024198 MYPACKAGE123dpp-1.3/
-drwxrwxrwx   0        0        0        0 2023-06-16 19:21:21.013198 MYPACKAGE123dpp-1.3/FirstApi/
--rw-rw-rw-   0        0        0     1017 2023-06-16 19:19:39.000000 MYPACKAGE123dpp-1.3/FirstApi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 19:21:21.020235 MYPACKAGE123dpp-1.3/MYPACKAGE123dpp.egg-info/
--rw-rw-rw-   0        0        0      212 2023-06-16 19:21:20.000000 MYPACKAGE123dpp-1.3/MYPACKAGE123dpp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-06-16 19:21:20.000000 MYPACKAGE123dpp-1.3/MYPACKAGE123dpp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 19:21:20.000000 MYPACKAGE123dpp-1.3/MYPACKAGE123dpp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-16 19:21:20.000000 MYPACKAGE123dpp-1.3/MYPACKAGE123dpp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      212 2023-06-16 19:21:21.023199 MYPACKAGE123dpp-1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 19:21:21.022233 MYPACKAGE123dpp-1.3/SecondApi/
--rw-rw-rw-   0        0        0     1069 2023-06-16 19:19:53.000000 MYPACKAGE123dpp-1.3/SecondApi/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-16 19:21:21.024198 MYPACKAGE123dpp-1.3/setup.cfg
--rw-rw-rw-   0        0        0      220 2023-06-16 19:20:22.000000 MYPACKAGE123dpp-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 18:15:12.752461 MYPACKAGE123dpp-1.4/
+drwxrwxrwx   0        0        0        0 2023-06-19 18:15:12.740471 MYPACKAGE123dpp-1.4/ChatAPI/
+-rw-rw-rw-   0        0        0      868 2023-06-16 19:47:00.000000 MYPACKAGE123dpp-1.4/ChatAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 18:15:12.748489 MYPACKAGE123dpp-1.4/MYPACKAGE123dpp.egg-info/
+-rw-rw-rw-   0        0        0      212 2023-06-19 18:15:12.000000 MYPACKAGE123dpp-1.4/MYPACKAGE123dpp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-06-19 18:15:12.000000 MYPACKAGE123dpp-1.4/MYPACKAGE123dpp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 18:15:12.000000 MYPACKAGE123dpp-1.4/MYPACKAGE123dpp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-19 18:15:12.000000 MYPACKAGE123dpp-1.4/MYPACKAGE123dpp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      212 2023-06-19 18:15:12.751459 MYPACKAGE123dpp-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 18:15:12.750459 MYPACKAGE123dpp-1.4/TextTranslatorAPI/
+-rw-rw-rw-   0        0        0      775 2023-06-16 19:47:00.000000 MYPACKAGE123dpp-1.4/TextTranslatorAPI/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 18:15:12.752461 MYPACKAGE123dpp-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      220 2023-06-19 18:14:35.000000 MYPACKAGE123dpp-1.4/setup.py
```

### Comparing `MYPACKAGE123dpp-1.3/FirstApi/__init__.py` & `MYPACKAGE123dpp-1.4/ChatAPI/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,13 +22,10 @@
 
         response = requests.post(self.url, json=payload, headers=self.headers)
         data = response.json()
         content = data["choices"][0]["message"]["content"]
         return content
 
 
-# Example usage
+
 api_key = "d9050d5653msh75d645c395b0db8p19a102jsn44253b504e66"
-chat_api = ChatAPI(api_key)
-user_input = input("User: ")
-response = chat_api.send_message(user_input)
-print("Assistant:", response)
+
```

