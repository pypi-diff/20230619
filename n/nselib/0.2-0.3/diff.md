# Comparing `tmp/nselib-0.2.tar.gz` & `tmp/nselib-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nselib-0.2.tar", last modified: Mon Jun 19 14:41:14 2023, max compression
+gzip compressed data, was "nselib-0.3.tar", last modified: Mon Jun 19 16:51:16 2023, max compression
```

## Comparing `nselib-0.2.tar` & `nselib-0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 14:41:14.600610 nselib-0.2/
--rw-rw-rw-   0        0        0    11558 2023-06-18 02:00:39.000000 nselib-0.2/LICENSE
--rw-rw-rw-   0        0        0        0 2023-06-18 00:57:58.000000 nselib-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3052 2023-06-19 14:41:14.600610 nselib-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2359 2023-06-19 14:00:31.000000 nselib-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 14:41:14.561606 nselib-0.2/nselib/
--rw-rw-rw-   0        0        0        0 2023-06-17 23:08:53.000000 nselib-0.2/nselib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:41:14.582606 nselib-0.2/nselib/capital_market/
--rw-rw-rw-   0        0        0      226 2023-06-19 13:36:13.000000 nselib-0.2/nselib/capital_market/__init__.py
--rw-rw-rw-   0        0        0    15225 2023-06-19 13:36:13.000000 nselib-0.2/nselib/capital_market/capital_market_data.py
--rw-rw-rw-   0        0        0     2115 2023-06-19 08:30:28.000000 nselib-0.2/nselib/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:41:14.586604 nselib-0.2/nselib/debt/
--rw-rw-rw-   0        0        0        0 2023-06-18 00:50:56.000000 nselib-0.2/nselib/debt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:41:14.595610 nselib-0.2/nselib/derivatives/
--rw-rw-rw-   0        0        0      168 2023-06-19 13:36:13.000000 nselib-0.2/nselib/derivatives/__init__.py
--rw-rw-rw-   0        0        0     8971 2023-06-19 12:46:17.000000 nselib-0.2/nselib/derivatives/derivative_data.py
--rw-rw-rw-   0        0        0     2965 2023-06-19 07:56:30.000000 nselib-0.2/nselib/libutil.py
--rw-rw-rw-   0        0        0      438 2023-06-18 06:43:26.000000 nselib-0.2/nselib/logger.py
--rw-rw-rw-   0        0        0       17 2023-06-19 13:23:14.000000 nselib-0.2/nselib/version.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:41:14.575610 nselib-0.2/nselib.egg-info/
--rw-rw-rw-   0        0        0     3052 2023-06-19 14:41:14.000000 nselib-0.2/nselib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-06-19 14:41:14.000000 nselib-0.2/nselib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 14:41:14.000000 nselib-0.2/nselib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-19 14:41:14.000000 nselib-0.2/nselib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-19 14:41:14.000000 nselib-0.2/nselib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-19 14:41:14.602610 nselib-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1011 2023-06-19 13:24:28.000000 nselib-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:51:16.019899 nselib-0.3/
+-rw-rw-rw-   0        0        0    11558 2023-06-18 02:00:39.000000 nselib-0.3/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:57:58.000000 nselib-0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3052 2023-06-19 16:51:16.020407 nselib-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2359 2023-06-19 16:47:39.000000 nselib-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 16:51:15.970229 nselib-0.3/nselib/
+-rw-rw-rw-   0        0        0        0 2023-06-17 23:08:53.000000 nselib-0.3/nselib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:51:15.993213 nselib-0.3/nselib/capital_market/
+-rw-rw-rw-   0        0        0      227 2023-06-19 16:40:39.000000 nselib-0.3/nselib/capital_market/__init__.py
+-rw-rw-rw-   0        0        0    15217 2023-06-19 16:39:21.000000 nselib-0.3/nselib/capital_market/capital_market_data.py
+-rw-rw-rw-   0        0        0     2115 2023-06-19 08:30:28.000000 nselib-0.3/nselib/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:51:15.999211 nselib-0.3/nselib/debt/
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:50:56.000000 nselib-0.3/nselib/debt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:51:16.008366 nselib-0.3/nselib/derivatives/
+-rw-rw-rw-   0        0        0      168 2023-06-19 13:36:13.000000 nselib-0.3/nselib/derivatives/__init__.py
+-rw-rw-rw-   0        0        0     9022 2023-06-19 16:34:43.000000 nselib-0.3/nselib/derivatives/derivative_data.py
+-rw-rw-rw-   0        0        0     3026 2023-06-19 15:56:00.000000 nselib-0.3/nselib/libutil.py
+-rw-rw-rw-   0        0        0      438 2023-06-18 06:43:26.000000 nselib-0.3/nselib/logger.py
+-rw-rw-rw-   0        0        0       17 2023-06-19 16:47:39.000000 nselib-0.3/nselib/version.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:51:15.984768 nselib-0.3/nselib.egg-info/
+-rw-rw-rw-   0        0        0     3052 2023-06-19 16:51:15.000000 nselib-0.3/nselib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2023-06-19 16:51:15.000000 nselib-0.3/nselib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 16:51:15.000000 nselib-0.3/nselib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-19 16:51:15.000000 nselib-0.3/nselib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-19 16:51:15.000000 nselib-0.3/nselib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-19 16:51:16.024431 nselib-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1011 2023-06-19 16:49:37.000000 nselib-0.3/setup.py
```

### Comparing `nselib-0.2/LICENSE` & `nselib-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nselib-0.2/PKG-INFO` & `nselib-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nselib
-Version: 0.2
+Version: 0.3
 Summary: library to get NSE India data
 Home-page: https://github.com/RuchiTanmay/nselib
 Author: RuchiTanmay
 Author-email: ruchitanmay@gmail.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# NSElib 0.2
+# NSElib 0.3
 Python Library to get publicly available data on new NSE india website.
 
 Release Notes
 * Compatible and Tested with Python 3.8 and above 
 * Future release will be done on requirement basic
 
 ## Libraries Required
```

### Comparing `nselib-0.2/README.md` & `nselib-0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# NSElib 0.2
+# NSElib 0.3
 Python Library to get publicly available data on new NSE india website.
 
 Release Notes
 * Compatible and Tested with Python 3.8 and above 
 * Future release will be done on requirement basic
 
 ## Libraries Required
```

### Comparing `nselib-0.2/nselib/capital_market/capital_market_data.py` & `nselib-0.3/nselib/capital_market/capital_market_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,12 +317,12 @@
     elif request_bhav.status_code == 403:
         raise FileNotFoundError(f' Data not found, change the date...')
     bhav_df = bhav_df[['SYMBOL', 'SERIES', 'OPEN', 'HIGH', 'LOW', 'CLOSE', 'LAST', 'PREVCLOSE', 'TOTTRDQTY',
                        'TOTTRDVAL', 'TIMESTAMP', 'TOTALTRADES']]
     return bhav_df
 
 
-# if __name__ == '__main__':
-#     df = bhav_copy(trade_date='01-06-2022')
-#     print(df)
-#     print(df.columns)
+if __name__ == '__main__':
+    df = bhav_copy(trade_date='01-06-2022')
+    print(df)
+    print(df.columns)
```

### Comparing `nselib-0.2/nselib/constants.py` & `nselib-0.3/nselib/constants.py`

 * *Files identical despite different names*

### Comparing `nselib-0.2/nselib/derivatives/derivative_data.py` & `nselib-0.3/nselib/derivatives/derivative_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 import time
 import zipfile
 from io import BytesIO, StringIO
 from nselib.libutil import *
 from nselib.constants import *
 
 
-def future_price_volume_data(symbol:str, instrument:str, from_date:str = None, to_date:str = None, period:str = None):
+def future_price_volume_data(symbol: str, instrument: str, from_date: str = None, to_date: str = None,
+                             period: str = None):
     """
     get contract wise future price volume data set.
-    :param instrument:  FUTIDX/FUTSTD
+    :param instrument:  FUTIDX/FUTSTK
     :param symbol: symbol eg: 'SBIN' / 'BANKNIFTY'
     :param from_date: '17-03-2022' ('dd-mm-YYYY')
     :param to_date: '17-06-2023' ('dd-mm-YYYY')
     :param period: use one {'1D': last day data,
                             '1W': for last 7 days data,
                             '1M': from last month same date,
                             '3M': last 3 month data
                             '6M': last 6 month data}
     :return: pandas.DataFrame
     :raise ValueError if the parameter input is not proper
     """
     validate_date_param(from_date, to_date, period)
 
-    if instrument not in ['FUTIDX', 'FUTSTD']:
+    if instrument not in ['FUTIDX', 'FUTSTK']:
         raise ValueError(f'{instrument} is not a future instrument')
 
     from_date, to_date = derive_from_and_to_date(from_date=from_date, to_date=to_date, period=period)
     nse_df = pd.DataFrame(columns=future_price_volume_data_column)
     from_date = datetime.strptime(from_date, dd_mm_yyyy)
     to_date = datetime.strptime(to_date, dd_mm_yyyy)
     load_days = (to_date - from_date).days
@@ -43,47 +44,48 @@
                                                from_date=start_date, to_date=end_date)
         from_date = from_date + dt.timedelta(91)
         load_days = (to_date - from_date).days
         nse_df = pd.concat([nse_df, data_df], ignore_index=True)
     return nse_df
 
 
-def get_future_price_volume_data(symbol:str, instrument:str, from_date:str, to_date:str):
+def get_future_price_volume_data(symbol: str, instrument: str, from_date: str, to_date: str):
     # print(from_date, to_date)
     data_df = pd.DataFrame()
     url = "https://www.nseindia.com/api/historical/foCPV?"
     payload = f"from={from_date}&to={to_date}&instrumentType={instrument}&symbol={symbol}&csv=true"
     try:
-        data_dict = nse_urlfetch(url+payload).json()
+        data_dict = nse_urlfetch(url + payload).json()
     except Exception as e:
         raise ValueError(" Invalid parameters ")
     data_df = pd.DataFrame(data_dict['data']).drop(columns='TIMESTAMP')
     data_df.columns = cleaning_column_name(data_df.columns)
     return data_df[future_price_volume_data_column]
 
 
-def option_price_volume_data(symbol:str, instrument:str, option_type:str = None, from_date:str = None, to_date:str = None, period:str = None):
+def option_price_volume_data(symbol: str, instrument: str, option_type: str = None, from_date: str = None,
+                             to_date: str = None, period: str = None):
     """
     get contract wise option price volume data set. more than 90 days will take more time to collect data.
     :param option_type: PE/CE
-    :param instrument:  OPTIDX/OPTSTD
+    :param instrument:  OPTIDX/OPTSTK
     :param symbol: symbol eg: 'SBIN' / 'BANKNIFTY'
     :param from_date: '17-03-2022' ('dd-mm-YYYY')
     :param to_date: '17-06-2023' ('dd-mm-YYYY')
     :param period: use one {'1D': last day data,
                             '1W': for last 7 days data,
                             '1M': from last month same date,
                             '3M': last 3 month data
                             '6M': last 6 month data}
     :return: pandas.DataFrame
     :raise ValueError if the parameter input is not proper
     """
     validate_date_param(from_date, to_date, period)
 
-    if instrument not in ['OPTIDX', 'OPTSTD']:
+    if instrument not in ['OPTIDX', 'OPTSTK']:
         raise ValueError(f'{instrument} is not a future instrument')
 
     if option_type and option_type not in ['PE', 'CE']:
         raise ValueError(f'{option_type} is not a valid option type')
 
     option_type = [option_type] if option_type else ['PE', 'CE']
     from_date, to_date = derive_from_and_to_date(from_date=from_date, to_date=to_date, period=period)
@@ -104,85 +106,82 @@
             nse_df = pd.concat([nse_df, data_df], ignore_index=True)
         from_date = from_date + dt.timedelta(91)
         load_days = (to_date - from_date).days
 
     return nse_df
 
 
-def get_option_price_volume_data(symbol:str, instrument:str, option_type:str, from_date:str, to_date:str):
+def get_option_price_volume_data(symbol: str, instrument: str, option_type: str, from_date: str, to_date: str):
     data_df = pd.DataFrame()
     url = "https://www.nseindia.com/api/historical/foCPV?"
     payload = f"from={from_date}&to={to_date}&instrumentType={instrument}&symbol={symbol}" \
               f"&optionType={option_type}&csv=true"
     try:
-        data_dict = nse_urlfetch(url+payload).json()
+        data_dict = nse_urlfetch(url + payload).json()
     except Exception as e:
         raise ValueError(" Invalid parameters ")
     data_df = pd.DataFrame(data_dict['data']).drop(columns='TIMESTAMP')
     data_df.columns = cleaning_column_name(data_df.columns)
-    print(data_df.columns)
+    # print(data_df.columns)
     return data_df[future_price_volume_data_column]
 
 
-def fno_bhav_copy(trade_date:str):
+def fno_bhav_copy(trade_date: str):
     trade_date = datetime.strptime(trade_date, dd_mm_yyyy)
     url = 'https://archives.nseindia.com/content/historical/DERIVATIVES/'
     payload = f"{str(trade_date.strftime('%Y'))}/{str(trade_date.strftime('%b').upper())}/" \
               f"fo{str(trade_date.strftime('%d%b%Y').upper())}bhav.csv.zip"
-    request_bhav = nse_urlfetch(url+payload)
+    request_bhav = nse_urlfetch(url + payload)
     bhav_df = pd.DataFrame()
     if request_bhav.status_code == 200:
         zip_bhav = zipfile.ZipFile(BytesIO(request_bhav.content), 'r')
         for file_name in zip_bhav.filelist:
             if file_name:
                 bhav_df = pd.read_csv(zip_bhav.open(file_name))
     elif request_bhav.status_code == 403:
         raise FileNotFoundError(f' Data not found, change the date...')
     bhav_df = bhav_df[['INSTRUMENT', 'SYMBOL', 'EXPIRY_DT', 'STRIKE_PR', 'OPTION_TYP', 'OPEN', 'HIGH', 'LOW',
                        'CLOSE', 'SETTLE_PR', 'CONTRACTS', 'VAL_INLAKH', 'OPEN_INT', 'CHG_IN_OI', 'TIMESTAMP']]
     return bhav_df
 
 
-def participant_wise_open_interest(trade_date:str):
+def participant_wise_open_interest(trade_date: str):
     trade_date = datetime.strptime(trade_date, dd_mm_yyyy)
     raw_data = pd.DataFrame()
     url = f"https://archives.nseindia.com/content/nsccl/fao_participant_oi_{str(trade_date.strftime('%d%m%Y'))}.csv"
     # payload = f"{str(for_date.strftime('%d%m%Y'))}.csv"
     file_chk = requests.get(url, headers=header)
     if file_chk.status_code != 200:
         raise FileNotFoundError(f" No data available for : {trade_date}")
     try:
         data_df = pd.read_csv(url, engine='python', sep=',', quotechar='"', on_bad_lines='skip', skiprows=1,
-                               skipfooter=1)
+                              skipfooter=1)
     except:
         data_df = pd.read_csv(url, engine='c', sep=',', quotechar='"', on_bad_lines='skip', skiprows=1)
         data_df.drop(data_df.tail(1).index, inplace=True)
         data_df.columns = [name.replace('\t', '') for name in data_df.columns]
     return data_df
 
 
-def participant_wise_trading_volume(trade_date:str):
+def participant_wise_trading_volume(trade_date: str):
     trade_date = datetime.strptime(trade_date, dd_mm_yyyy)
     raw_data = pd.DataFrame()
     url = f"https://archives.nseindia.com/content/nsccl/fao_participant_vol_{str(trade_date.strftime('%d%m%Y'))}.csv"
     # payload = f"{str(for_date.strftime('%d%m%Y'))}.csv"
     file_chk = requests.get(url, headers=header)
     if file_chk.status_code != 200:
         raise FileNotFoundError(f" No data available for : {trade_date}")
     try:
         data_df = pd.read_csv(url, engine='python', sep=',', quotechar='"', on_bad_lines='skip', skiprows=1,
-                               skipfooter=1)
+                              skipfooter=1)
     except Exception:
         data_df = pd.read_csv(url, engine='c', sep=',', quotechar='"', on_bad_lines='skip', skiprows=1)
         data_df.drop(data_df.tail(1).index, inplace=True)
         data_df.columns = [name.replace('\t', '') for name in data_df.columns]
     return data_df
 
 
-
-
-# if __name__ == '__main__':
-#     # df = option_price_volume_data(symbol='BANKNIFTY', instrument='OPTIDX',
-#     #                                   from_date='01-04-2023', to_date='16-06-2023')
-#     df = participant_wise_trading_volume(trade_date='03-04-2023')
-#     print(df)
-#     print(df.columns)
+if __name__ == '__main__':
+    df = future_price_volume_data("BANKNIFTY", "FUTIDX", from_date='17-06-2023', to_date='19-06-2023', period='1D')
+    # df = participant_wise_trading_volume(trade_date='03-04-2023')
+    print(df)
+    print(df[df['EXPIRY_DT']=='27-Jul-2023'])
```

### Comparing `nselib-0.2/nselib/libutil.py` & `nselib-0.3/nselib/libutil.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,16 @@
     value = [today - timedelta(days=1),
              today - timedelta(weeks=1),
              today - relativedelta(months=1),
              today - relativedelta(months=6),
              today - relativedelta(months=12)]
 
     f_date = np.select(conditions,value, default=(today - timedelta(days=1)))
-    from_date = pd.to_datetime(str(f_date))
+    from_date = pd.to_datetime(str(f_date)).strftime(dd_mm_yyyy)
+    today = today.strftime(dd_mm_yyyy)
     return from_date, today
 
 
 def cleaning_column_name(col:list):
     unwanted_str_list = ['FH_']
     new_col=col
     for unwanted in unwanted_str_list:
```

### Comparing `nselib-0.2/nselib.egg-info/PKG-INFO` & `nselib-0.3/nselib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nselib
-Version: 0.2
+Version: 0.3
 Summary: library to get NSE India data
 Home-page: https://github.com/RuchiTanmay/nselib
 Author: RuchiTanmay
 Author-email: ruchitanmay@gmail.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# NSElib 0.2
+# NSElib 0.3
 Python Library to get publicly available data on new NSE india website.
 
 Release Notes
 * Compatible and Tested with Python 3.8 and above 
 * Future release will be done on requirement basic
 
 ## Libraries Required
```

### Comparing `nselib-0.2/setup.py` & `nselib-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='nselib',
     packages=setuptools.find_packages(),
-    version='0.2',
+    version='0.3',
     include_package_data=True,
     description='library to get NSE India data',
     long_description=long_description,
     long_description_content_type="text/markdown", author='RuchiTanmay',
     author_email='ruchitanmay@gmail.com',
     url='https://github.com/RuchiTanmay/nselib',
     install_requires=['requests', 'pandas', 'scipy'],
```

