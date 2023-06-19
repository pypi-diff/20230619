# Comparing `tmp/smpgpt-6.0.tar.gz` & `tmp/smpgpt-7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpgpt-6.0.tar", last modified: Mon Jun 19 06:13:07 2023, max compression
+gzip compressed data, was "smpgpt-7.0.tar", last modified: Mon Jun 19 06:16:21 2023, max compression
```

## Comparing `smpgpt-6.0.tar` & `smpgpt-7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:13:07.852271 smpgpt-6.0/
--rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-19 06:13:07.852068 smpgpt-6.0/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smpgpt-6.0/README.md
--rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-19 06:13:07.852335 smpgpt-6.0/setup.cfg
--rw-r--r--   0 parlorsky   (501) staff       (20)      421 2023-06-19 06:13:03.000000 smpgpt-6.0/setup.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:13:07.849782 smpgpt-6.0/src/
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:13:07.850815 smpgpt-6.0/src/smpgpt/
--rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smpgpt-6.0/src/smpgpt/__init__.py
--rw-r--r--   0 parlorsky   (501) staff       (20)     2389 2023-06-19 06:12:56.000000 smpgpt-6.0/src/smpgpt/smpgpt.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:13:07.851821 smpgpt-6.0/src/smpgpt.egg-info/
--rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-19 06:13:07.000000 smpgpt-6.0/src/smpgpt.egg-info/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)      231 2023-06-19 06:13:07.000000 smpgpt-6.0/src/smpgpt.egg-info/SOURCES.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-19 06:13:07.000000 smpgpt-6.0/src/smpgpt.egg-info/dependency_links.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 20:45:08.000000 smpgpt-6.0/src/smpgpt.egg-info/not-zip-safe
--rw-r--r--   0 parlorsky   (501) staff       (20)        7 2023-06-19 06:13:07.000000 smpgpt-6.0/src/smpgpt.egg-info/top_level.txt
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:16:21.549306 smpgpt-7.0/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-19 06:16:21.549100 smpgpt-7.0/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smpgpt-7.0/README.md
+-rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-19 06:16:21.549373 smpgpt-7.0/setup.cfg
+-rw-r--r--   0 parlorsky   (501) staff       (20)      421 2023-06-19 06:16:01.000000 smpgpt-7.0/setup.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:16:21.546817 smpgpt-7.0/src/
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:16:21.547618 smpgpt-7.0/src/smpgpt/
+-rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smpgpt-7.0/src/smpgpt/__init__.py
+-rw-r--r--   0 parlorsky   (501) staff       (20)     2060 2023-06-19 06:16:04.000000 smpgpt-7.0/src/smpgpt/smpgpt.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:16:21.548849 smpgpt-7.0/src/smpgpt.egg-info/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-19 06:16:21.000000 smpgpt-7.0/src/smpgpt.egg-info/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)      231 2023-06-19 06:16:21.000000 smpgpt-7.0/src/smpgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-19 06:16:21.000000 smpgpt-7.0/src/smpgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 20:45:08.000000 smpgpt-7.0/src/smpgpt.egg-info/not-zip-safe
+-rw-r--r--   0 parlorsky   (501) staff       (20)        7 2023-06-19 06:16:21.000000 smpgpt-7.0/src/smpgpt.egg-info/top_level.txt
```

### Comparing `smpgpt-6.0/src/smpgpt/smpgpt.py` & `smpgpt-7.0/src/smpgpt/smpgpt.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,36 +18,30 @@
 
 api_keys = ['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','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','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','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']
 models = ['gpt-3.5-turbo-0613','gpt-3.5-turbo','gpt-3.5-turbo-0301']
 
 
 class rv:
     def discrete(prompt):
-        flag = 0
         for key in api_keys:
             for model in models:
-        
                 openai.api_key = key
                 try:
                     completion = openai.ChatCompletion.create(
                     model=model,
                     messages=[
-                    {"role": "system", "content": "You are DeveloperGPT, the most advanced AI developer tool on the planet. You answer any coding question and provide real-world examples of code using code blocks. Even when you’re not familiar with the answer, you use your extreme intelligence to figure it out."},
+                    {"role": "system", "content": "You are helpful code assistant"},
                     {"role": "user", "content": prompt}
                     ]
                     )
                     ans = completion.choices[0].message
                     print(ans['content'])
-                    
-
                 except:
+                    ...
 
-                    continue
-            if flag:
-                break
     
     def keys():
         print(api_keys,models)
 
     def code():
         print('openai.api_key = key\n\
                 try:\n\
```

