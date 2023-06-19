# Comparing `tmp/yeref-0.1.99.tar.gz` & `tmp/yeref-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.99.tar", last modified: Sun Jun 18 12:52:36 2023, max compression
+gzip compressed data, was "yeref-0.2.0.tar", last modified: Mon Jun 19 08:14:49 2023, max compression
```

## Comparing `yeref-0.1.99.tar` & `yeref-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-18 12:52:36.678305 yeref-0.1.99/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-18 12:52:36.678454 yeref-0.1.99/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-18 12:52:36.679039 yeref-0.1.99/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-18 12:52:23.000000 yeref-0.1.99/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-18 12:52:36.669882 yeref-0.1.99/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.99/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   557031 2023-06-18 12:52:19.000000 yeref-0.1.99/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   211025 2023-06-15 14:36:34.000000 yeref-0.1.99/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-18 12:52:36.677867 yeref-0.1.99/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-18 12:52:36.000000 yeref-0.1.99/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-18 12:52:36.000000 yeref-0.1.99/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-18 12:52:36.000000 yeref-0.1.99/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-18 12:52:36.000000 yeref-0.1.99/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-19 08:14:49.723598 yeref-0.2.0/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-19 08:14:49.723859 yeref-0.2.0/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-19 08:14:49.725498 yeref-0.2.0/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-19 08:14:37.000000 yeref-0.2.0/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-19 08:14:49.716182 yeref-0.2.0/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.0/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   557031 2023-06-18 12:52:19.000000 yeref-0.2.0/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   210926 2023-06-19 08:12:39.000000 yeref-0.2.0/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-19 08:14:49.722841 yeref-0.2.0/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-19 08:14:49.000000 yeref-0.2.0/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-19 08:14:49.000000 yeref-0.2.0/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-19 08:14:49.000000 yeref-0.2.0/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-19 08:14:49.000000 yeref-0.2.0/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.99/setup.py` & `yeref-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.99',
+      version='0.2.0',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -43,12 +43,12 @@
 
 # twine upload dist/*
 # freey.sitner.ya
 # cejwez-nosgin-vaVfe7
 
 # python3 -m pip install --upgrade yeref
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.98-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.99-py3-none-any.whl
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.99/yeref/l_.py` & `yeref-0.2.0/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.1.99/yeref/yeref.py` & `yeref-0.2.0/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -3121,37 +3121,34 @@
         offer_id = int(offer_id)
         dic_btns = await check_buttons(bot, None, OFFER_BUTTON, is_counter)
         result = InlineKeyboardBuilder()
         for k, v in dic_btns.items():
             try:
                 if v[0]:
                     if len(tmp) > 0 and tmp[-1] is None:
-                        result.add(*buttons)
+                        result.row(*buttons)
                         if 'ᴵ' in v[0]:
                             buttons = [types.InlineKeyboardButton(text=str(v[0]), switch_inline_query_current_chat='')]
                         elif str(v[1]).startswith("btn_"):
-                            buttons = [
-                                types.InlineKeyboardButton(text=str(v[0]), callback_data=f"btn_{type_}_{offer_id}_{k}")]
+                            buttons = [types.InlineKeyboardButton(text=str(v[0]), callback_data=f"btn_{type_}_{offer_id}_{k}")]
                         else:
                             buttons = [types.InlineKeyboardButton(text=str(v[0]), url=v[1])]
                     else:
                         if 'ᴵ' in v[0]:
-                            buttons.append(
-                                types.InlineKeyboardButton(text=str(v[0]), switch_inline_query_current_chat=''))
+                            buttons.append(types.InlineKeyboardButton(text=str(v[0]), switch_inline_query_current_chat=''))
                         elif str(v[1]).startswith("btn_"):
-                            buttons.append(
-                                types.InlineKeyboardButton(text=str(v[0]), callback_data=f"btn_{type_}_{offer_id}_{k}"))
+                            buttons.append(types.InlineKeyboardButton(text=str(v[0]), callback_data=f"btn_{type_}_{offer_id}_{k}"))
                         else:
                             buttons.append(types.InlineKeyboardButton(text=str(v[0]), url=v[1]))
                 tmp.append(v[0])
             except Exception as e:
                 logger.info(log_ % str(e))
                 pass
         if len(buttons) > 0:
-            result.add(*buttons)
+            result.row(*buttons)
     except Exception as e:
         logger.info(log_ % str(e))
         pass
     finally:
         return result
```

