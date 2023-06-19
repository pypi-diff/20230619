# Comparing `tmp/iosense_connect-4.0.2.tar.gz` & `tmp/iosense_connect-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-4.0.2.tar", last modified: Thu Jun 15 16:07:59 2023, max compression
+gzip compressed data, was "dist\iosense_connect-4.0.3.tar", last modified: Mon Jun 19 07:39:28 2023, max compression
```

## Comparing `iosense_connect-4.0.2.tar` & `iosense_connect-4.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 16:07:59.768420 iosense_connect-4.0.2/
--rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-4.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-06-15 16:07:59.767119 iosense_connect-4.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-4.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 16:07:59.717167 iosense_connect-4.0.2/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-4.0.2/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    27602 2023-06-15 16:07:42.000000 iosense_connect-4.0.2/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-06-15 16:07:59.764158 iosense_connect-4.0.2/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-06-15 16:07:59.000000 iosense_connect-4.0.2/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-15 16:07:59.000000 iosense_connect-4.0.2/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 16:07:59.000000 iosense_connect-4.0.2/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      268 2023-06-15 16:07:59.000000 iosense_connect-4.0.2/iosense_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-15 16:07:59.000000 iosense_connect-4.0.2/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 16:07:59.769121 iosense_connect-4.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1106 2023-06-15 16:07:42.000000 iosense_connect-4.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:39:28.256207 iosense_connect-4.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-4.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-06-19 07:39:28.255022 iosense_connect-4.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-4.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 07:39:28.201719 iosense_connect-4.0.3/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-4.0.3/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    28130 2023-06-19 07:39:22.000000 iosense_connect-4.0.3/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:39:28.250216 iosense_connect-4.0.3/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-06-19 07:39:27.000000 iosense_connect-4.0.3/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-19 07:39:28.000000 iosense_connect-4.0.3/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 07:39:27.000000 iosense_connect-4.0.3/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      268 2023-06-19 07:39:27.000000 iosense_connect-4.0.3/iosense_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-19 07:39:27.000000 iosense_connect-4.0.3/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 07:39:28.256207 iosense_connect-4.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2023-06-19 07:39:22.000000 iosense_connect-4.0.3/setup.py
```

### Comparing `iosense_connect-4.0.2/LICENSE.txt` & `iosense_connect-4.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-4.0.2/PKG-INFO` & `iosense_connect-4.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect
-Version: 4.0.2
+Version: 4.0.3
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-4.0.2/README.md` & `iosense_connect-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-4.0.2/iosense_connect/data_access.py` & `iosense_connect-4.0.3/iosense_connect/data_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 import sys
+import pytz
 import json
 import fsspec
 import urllib3
 import requests
 import numpy as np
 import pandas as pd
-from concurrent.futures import ThreadPoolExecutor
-from cryptography.fernet import Fernet
 from datetime import timedelta
+from cryptography.fernet import Fernet
 from datetime import datetime, timezone
 from dateutil.relativedelta import relativedelta
+from concurrent.futures import ThreadPoolExecutor
 
 pd.options.mode.chained_assignment = None
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 class DataAccess:
     def __init__(self, userid, url, key):
@@ -502,20 +503,27 @@
                             sys.stdout.flush()
                         results = executor.map(read_one, filenames_list)
                     fetched_df = pd.concat(results, axis=0)
                 else:
                     fetched_df = pd.DataFrame()
                 return fetched_df
             start_time = pd.to_datetime(start_time)
-            end_time = pd.to_datetime(end_time)
             if type(end_time) == str:
                 try:
                     end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S').strftime('%Y-%m-%d %H:%M:%S')
-                except Exception:
-                    end_time = str(end_time) + " 23:59:59" if isinstance(end_time, str) else end_time
+                except ValueError:
+                    try:
+                        end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S.%f').strftime(
+                            '%Y-%m-%d %H:%M:%S')
+                    except Exception:
+                        end_time = str(end_time) + " 23:59:59" if isinstance(end_time, str) else end_time
+            else:
+                india_timezone = pytz.timezone('Asia/Kolkata')
+                end_time = end_time.astimezone(india_timezone)
+                end_time = end_time.strftime('%Y-%m-%d %H:%M:%S')
             df = pd.DataFrame()
             metadata = {}
             connector = None
             container_name = None
             if db is not None:
                 credentials = DataAccess.get_cloud_credentials(self, db)
                 if len(credentials) !=0:
@@ -542,54 +550,52 @@
                     device_list = [blob.split("/")[1] for blob in blobs]
                     if device_id in device_list:
                         blobs = [blob_name.split("/")[2] for blob_name in connector.ls(container_name + str(device_id) + "/")]
                         dates = generate_month_year_dates(start_time, end_time)
                         filenames = list(set(dates).intersection(blobs))
                         filenames = sorted(filenames, key=get_month_year)
                         df = thread_read(filenames)
+                if len(df) != 0:
+                    try:
+                        start_time = datetime.strptime(str(start_time), '%Y-%m-%d %H:%M:%S')
+                        end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S')
+                    except ValueError:
+                        pass
+                    except Exception as e:
+                        print('Message:', e)
+
+                    df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
+                    if len(df) != 0:
+                        if sensors is None:
+                            sensors = list(df.columns)
+                            sensors.remove('time')
+
+                        sensors_filtered = list(set(df.columns).intersection(sensors))
+                        if sensors and len(sensors_filtered) != 0:
+                            sensors_filtered.insert(0, 'time')
+                            df = df[sensors_filtered]
+                        else:
+                            df = pd.DataFrame()
+                        df.sort_values(['time'], inplace=True)
+                        df.reset_index(drop=True, inplace=True)
+                        last_date = df['time'].iloc[-1]
+                        if str(last_date) < str(end_time):
+                            df1 = DataAccess.fetch_data(self, device_id, start_time=last_date, alias=False,
+                                                        end_time=end_time, sensors=sensors, echo=True,
+                                                        onpremise=onpremise, IST=True)
+                            df = pd.concat([df, df1])
+                            df.reset_index(drop=True, inplace=True)
             else:
                 df_devices = DataAccess.get_device_details(self,onpremise=onpremise)
                 device_list = df_devices['devID'].tolist()
                 if device_id in device_list:
                     df = DataAccess.fetch_data(self, device_id, start_time, end_time, alias, sensors=sensors, echo=True,
                                                onpremise=onpremise, IST=IST)
                 else:
                     raise Exception('Message: Device not added in account')
-            if len(df) != 0:
-
-                try:
-                    start_time = datetime.strptime(str(start_time), '%Y-%m-%d %H:%M:%S')
-                    end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S')
-                except ValueError:
-                    pass
-                except Exception as e:
-                    print('Message:', e)
-
-                df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
-                if len(df) != 0:
-                    if sensors is None:
-                        sensors = list(df.columns)
-                        sensors.remove('time')
-
-                    sensors_filtered = list(set(df.columns).intersection(sensors))
-                    if sensors and len(sensors_filtered) != 0:
-                        sensors_filtered.insert(0, 'time')
-                        df = df[sensors_filtered]
-                    else:
-                        df = pd.DataFrame()
-                    df.sort_values(['time'], inplace=True)
-                    df.reset_index(drop=True, inplace=True)
-                    last_date = df['time'].iloc[-1]
-
-                    if str(last_date) < str(end_time):
-                        df1 = DataAccess.fetch_data(self, device_id, start_time=last_date, alias=False,
-                                                    end_time=end_time, sensors=sensors, echo=True,
-                                                    onpremise=onpremise, IST=True)
-                        df = pd.concat([df, df1])
-                        df.reset_index(drop=True, inplace=True)
 
             if len(df) != 0:
                 if str(alias).lower() == "true":
                     df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata, onpremise=onpremise)
 
                 if str(cal).lower() == 'true':
                     df = DataAccess.get_caliberation(self, device_id, metadata, df, onpremise=onpremise)
@@ -597,12 +603,12 @@
                 if bands is not None:
                     df = DataAccess.time_grouping(self, df, bands, compute)
                 df = df.set_index(['time'])
                 df = df.fillna(value=np.nan)
                 df.dropna(axis=0, how='all', inplace=True)
                 df.reset_index(drop=False, inplace=True)
                 df.drop_duplicates(inplace=True)
-                if IST is False:
+                if IST is False and db is not None:
                     df['time'] = pd.to_datetime(df['time']) - timedelta(hours=5, minutes=30)
             return df
         except Exception as e:
             print(e)
```

### Comparing `iosense_connect-4.0.2/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-4.0.3/iosense_connect.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect
-Version: 4.0.2
+Version: 4.0.3
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-4.0.2/setup.py` & `iosense_connect-4.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "4.0.2",
+    version = "4.0.3",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     install_requires=[
```

