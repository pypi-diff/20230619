# Comparing `tmp/hkfdb-3.4.3.tar.gz` & `tmp/hkfdb-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-3.4.3.tar", last modified: Mon Jun  5 12:38:05 2023, max compression
+gzip compressed data, was "hkfdb-3.5.1.tar", last modified: Mon Jun 19 02:34:31 2023, max compression
```

## Comparing `hkfdb-3.4.3.tar` & `hkfdb-3.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 12:38:05.811287 hkfdb-3.4.3/
--rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.4.3/LICENSE
--rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-06-05 12:38:05.811020 hkfdb-3.4.3/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.4.3/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 12:38:05.810064 hkfdb-3.4.3/hkfdb/
--rw-rw-rw-   0 cmw        (501) staff       (20)   107897 2023-06-05 12:36:51.000000 hkfdb-3.4.3/hkfdb/Database.py
--rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.4.3/hkfdb/__init__.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 12:38:05.810834 hkfdb-3.4.3/hkfdb.egg-info/
--rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-06-05 12:38:05.000000 hkfdb-3.4.3/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-06-05 12:38:05.000000 hkfdb-3.4.3/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-06-05 12:38:05.000000 hkfdb-3.4.3/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)       44 2023-06-05 12:38:05.000000 hkfdb-3.4.3/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-06-05 12:38:05.000000 hkfdb-3.4.3/hkfdb.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-05 12:38:05.811336 hkfdb-3.4.3/setup.cfg
--rw-rw-rw-   0 cmw        (501) staff       (20)      763 2023-06-05 12:37:22.000000 hkfdb-3.4.3/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-19 02:34:31.379424 hkfdb-3.5.1/
+-rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.5.1/LICENSE
+-rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-06-19 02:34:31.379273 hkfdb-3.5.1/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.5.1/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-19 02:34:31.378342 hkfdb-3.5.1/hkfdb/
+-rw-rw-rw-   0 cmw        (501) staff       (20)   108587 2023-06-19 02:29:22.000000 hkfdb-3.5.1/hkfdb/Database.py
+-rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.5.1/hkfdb/__init__.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-19 02:34:31.379079 hkfdb-3.5.1/hkfdb.egg-info/
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-06-19 02:34:31.000000 hkfdb-3.5.1/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-06-19 02:34:31.000000 hkfdb-3.5.1/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-06-19 02:34:31.000000 hkfdb-3.5.1/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-06-19 02:34:31.000000 hkfdb-3.5.1/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-06-19 02:34:31.000000 hkfdb-3.5.1/hkfdb.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-19 02:34:31.379469 hkfdb-3.5.1/setup.cfg
+-rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-06-19 02:33:24.000000 hkfdb-3.5.1/setup.py
```

### Comparing `hkfdb-3.4.3/LICENSE` & `hkfdb-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-3.4.3/PKG-INFO` & `hkfdb-3.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.4.3
+Version: 3.5.1
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.4.3/README.md` & `hkfdb-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-3.4.3/hkfdb/Database.py` & `hkfdb-3.5.1/hkfdb/Database.py`

 * *Files 0% similar despite different names*

```diff
@@ -810,15 +810,14 @@
             err_msg = 'Error in: '
             for error in check_bool_dict:
                 if check_bool_dict[error] == False:
                     err_msg += error + ','
             print(err_msg)
 
     def get_hk_market_cap_hist_by_code(self, code):
-
         check_bool_dict = self.check_hk_code_args(code)
 
         if False not in list(check_bool_dict.values()):
             link_url = 'http://www.hkfdb.net/data_api?'
             token_str = 'token=' + str(self.authToken)
             database_str = 'database=' + 'hk_market_cap_hist_by_code'
             code_str = 'code=' + str(code)
@@ -843,18 +842,32 @@
 
                 df = df.sort_values(by='date')
                 df = df.reset_index(drop=True)
                 if '-' in df.at[0, 'date']:
                     df['date'] = pd.to_datetime(df['date'], format='%Y-%m-%d')
                 else:
                     df['date'] = pd.to_datetime(df['date'], format='%Y%m%d')
-                df = df[['date','code','issued_share_mil','market_cap_mil','cumulative_market_cap_mil']]
+                df = df[['date', 'code', 'issued_share_mil', 'market_cap_mil', 'cumulative_market_cap_mil']]
                 df = df.set_index('date')
                 df = df[~df.index.duplicated(keep='first')]
 
+                df2 = df[df.index >= '2023-02-20']
+                df = df[df.index < '2023-02-20']
+
+                index_end_date = datetime.datetime.now() + datetime.timedelta(days=1)
+                index_end_year = index_end_date.year
+                date_index = pd.date_range(start='2023-02-20', end=index_end_date.strftime('%Y-%m-%d'), freq='1D')
+                df2 = df2.reindex(date_index)
+                df2 = df2.shift(-1)
+                df = pd.concat([df, df2])
+                df = df.dropna()
+
+                # holiday_list = get_hk_holiday_and_expiry_date(2023, index_end_year, format='dt')['public_holiday']
+                # df = df[~df.index.isin(holiday_list)]
+
                 return df
 
         else:
             err_msg = 'Error in: '
             for error in check_bool_dict:
                 if check_bool_dict[error] == False:
                     err_msg += error + ','
```

### Comparing `hkfdb-3.4.3/hkfdb.egg-info/PKG-INFO` & `hkfdb-3.5.1/hkfdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.4.3
+Version: 3.5.1
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.4.3/setup.py` & `hkfdb-3.5.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="3.4.3",
+    version="3.5.1",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires = [
-        'pandas',
+        'pandas == 1.5.3',
         'requests',
         'beautifulsoup4',
         'pymongo',
         'lxml',
     ]
 )
```

