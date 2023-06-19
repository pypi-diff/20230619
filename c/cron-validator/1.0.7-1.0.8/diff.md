# Comparing `tmp/cron-validator-1.0.7.tar.gz` & `tmp/cron-validator-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cron-validator-1.0.7.tar", last modified: Mon Jun 12 16:54:07 2023, max compression
+gzip compressed data, was "cron-validator-1.0.8.tar", last modified: Mon Jun 19 10:09:29 2023, max compression
```

## Comparing `cron-validator-1.0.7.tar` & `cron-validator-1.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2023-06-12 16:54:07.949175 cron-validator-1.0.7/
--rw-r--r--   0 baodoan    (503) staff       (20)     1068 2021-10-24 03:55:01.000000 cron-validator-1.0.7/LICENSE.txt
--rw-r--r--   0 baodoan    (503) staff       (20)     4047 2023-06-12 16:54:07.949437 cron-validator-1.0.7/PKG-INFO
--rw-r--r--   0 baodoan    (503) staff       (20)     3573 2022-04-04 02:40:10.000000 cron-validator-1.0.7/README.md
-drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2023-06-12 16:54:07.942344 cron-validator-1.0.7/cron_validator/
--rw-r--r--   0 baodoan    (503) staff       (20)      103 2022-04-04 02:37:41.000000 cron-validator-1.0.7/cron_validator/__init__.py
--rw-r--r--   0 baodoan    (503) staff       (20)     9180 2022-04-04 02:37:41.000000 cron-validator-1.0.7/cron_validator/regexes.py
--rw-r--r--   0 baodoan    (503) staff       (20)      799 2022-02-22 01:59:03.000000 cron-validator-1.0.7/cron_validator/scheduler.py
--rw-r--r--   0 baodoan    (503) staff       (20)     1537 2023-06-12 16:48:02.000000 cron-validator-1.0.7/cron_validator/util.py
--rw-r--r--   0 baodoan    (503) staff       (20)     2213 2023-06-12 16:48:02.000000 cron-validator-1.0.7/cron_validator/validator.py
-drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2023-06-12 16:54:07.944826 cron-validator-1.0.7/cron_validator.egg-info/
--rw-r--r--   0 baodoan    (503) staff       (20)     4047 2023-06-12 16:54:07.000000 cron-validator-1.0.7/cron_validator.egg-info/PKG-INFO
--rw-r--r--   0 baodoan    (503) staff       (20)      478 2023-06-12 16:54:07.000000 cron-validator-1.0.7/cron_validator.egg-info/SOURCES.txt
--rw-r--r--   0 baodoan    (503) staff       (20)        1 2023-06-12 16:54:07.000000 cron-validator-1.0.7/cron_validator.egg-info/dependency_links.txt
--rw-r--r--   0 baodoan    (503) staff       (20)       21 2023-06-12 16:54:07.000000 cron-validator-1.0.7/cron_validator.egg-info/requires.txt
--rw-r--r--   0 baodoan    (503) staff       (20)       15 2023-06-12 16:54:07.000000 cron-validator-1.0.7/cron_validator.egg-info/top_level.txt
--rw-r--r--   0 baodoan    (503) staff       (20)       79 2023-06-12 16:54:07.950207 cron-validator-1.0.7/setup.cfg
--rw-r--r--   0 baodoan    (503) staff       (20)      864 2023-06-12 16:49:49.000000 cron-validator-1.0.7/setup.py
-drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2023-06-12 16:54:07.948469 cron-validator-1.0.7/test/
--rw-r--r--   0 baodoan    (503) staff       (20)     3875 2022-02-22 01:59:03.000000 cron-validator-1.0.7/test/test_CronScheduler.py
--rw-r--r--   0 baodoan    (503) staff       (20)     6319 2022-02-22 01:59:03.000000 cron-validator-1.0.7/test/test_execution_time.py
--rw-r--r--   0 baodoan    (503) staff       (20)     4537 2022-04-04 02:37:41.000000 cron-validator-1.0.7/test/test_match.py
--rw-r--r--   0 baodoan    (503) staff       (20)     1458 2023-06-12 16:48:02.000000 cron-validator-1.0.7/test/test_util.py
--rw-r--r--   0 baodoan    (503) staff       (20)     5128 2023-06-12 16:48:02.000000 cron-validator-1.0.7/test/test_valid_regex.py
+drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2023-06-19 10:09:29.360908 cron-validator-1.0.8/
+-rw-r--r--   0 baodoan    (503) staff       (20)     1068 2021-10-24 03:55:01.000000 cron-validator-1.0.8/LICENSE.txt
+-rw-r--r--   0 baodoan    (503) staff       (20)     4047 2023-06-19 10:09:29.361121 cron-validator-1.0.8/PKG-INFO
+-rw-r--r--   0 baodoan    (503) staff       (20)     3573 2022-04-04 02:40:10.000000 cron-validator-1.0.8/README.md
+drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2023-06-19 10:09:29.353426 cron-validator-1.0.8/cron_validator/
+-rw-r--r--   0 baodoan    (503) staff       (20)      103 2022-04-04 02:37:41.000000 cron-validator-1.0.8/cron_validator/__init__.py
+-rw-r--r--   0 baodoan    (503) staff       (20)     9180 2022-04-04 02:37:41.000000 cron-validator-1.0.8/cron_validator/regexes.py
+-rw-r--r--   0 baodoan    (503) staff       (20)      799 2022-02-22 01:59:03.000000 cron-validator-1.0.8/cron_validator/scheduler.py
+-rw-r--r--   0 baodoan    (503) staff       (20)     1603 2023-06-19 10:08:01.000000 cron-validator-1.0.8/cron_validator/util.py
+-rw-r--r--   0 baodoan    (503) staff       (20)     2213 2023-06-12 16:48:02.000000 cron-validator-1.0.8/cron_validator/validator.py
+drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2023-06-19 10:09:29.356618 cron-validator-1.0.8/cron_validator.egg-info/
+-rw-r--r--   0 baodoan    (503) staff       (20)     4047 2023-06-19 10:09:29.000000 cron-validator-1.0.8/cron_validator.egg-info/PKG-INFO
+-rw-r--r--   0 baodoan    (503) staff       (20)      478 2023-06-19 10:09:29.000000 cron-validator-1.0.8/cron_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 baodoan    (503) staff       (20)        1 2023-06-19 10:09:29.000000 cron-validator-1.0.8/cron_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 baodoan    (503) staff       (20)       21 2023-06-19 10:09:29.000000 cron-validator-1.0.8/cron_validator.egg-info/requires.txt
+-rw-r--r--   0 baodoan    (503) staff       (20)       15 2023-06-19 10:09:29.000000 cron-validator-1.0.8/cron_validator.egg-info/top_level.txt
+-rw-r--r--   0 baodoan    (503) staff       (20)       79 2023-06-19 10:09:29.362379 cron-validator-1.0.8/setup.cfg
+-rw-r--r--   0 baodoan    (503) staff       (20)      864 2023-06-19 10:08:20.000000 cron-validator-1.0.8/setup.py
+drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2023-06-19 10:09:29.360206 cron-validator-1.0.8/test/
+-rw-r--r--   0 baodoan    (503) staff       (20)     3875 2022-02-22 01:59:03.000000 cron-validator-1.0.8/test/test_CronScheduler.py
+-rw-r--r--   0 baodoan    (503) staff       (20)     6319 2022-02-22 01:59:03.000000 cron-validator-1.0.8/test/test_execution_time.py
+-rw-r--r--   0 baodoan    (503) staff       (20)     4537 2022-04-04 02:37:41.000000 cron-validator-1.0.8/test/test_match.py
+-rw-r--r--   0 baodoan    (503) staff       (20)     1518 2023-06-19 10:08:01.000000 cron-validator-1.0.8/test/test_util.py
+-rw-r--r--   0 baodoan    (503) staff       (20)     5128 2023-06-12 16:48:02.000000 cron-validator-1.0.8/test/test_valid_regex.py
```

### Comparing `cron-validator-1.0.7/LICENSE.txt` & `cron-validator-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cron-validator-1.0.7/PKG-INFO` & `cron-validator-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cron-validator
-Version: 1.0.7
+Version: 1.0.8
 Summary: Unix cron implementation by Python
 Home-page: https://github.com/vcoder4c/cron-validator
 Author: vcoder
 Author-email: doanngocbao@gmail.com
 License: MIT
-Download-URL: https://github.com/vcoder4c/cron-validator/archive/v1.0.7.tar.gz
+Download-URL: https://github.com/vcoder4c/cron-validator/archive/v1.0.8.tar.gz
 Keywords: cron,python,cron expression validator,cron expression iterator,cron scheduler
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Cron Validator
```

### Comparing `cron-validator-1.0.7/README.md` & `cron-validator-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cron-validator-1.0.7/cron_validator/regexes.py` & `cron-validator-1.0.8/cron_validator/regexes.py`

 * *Files identical despite different names*

### Comparing `cron-validator-1.0.7/cron_validator/scheduler.py` & `cron-validator-1.0.8/cron_validator/scheduler.py`

 * *Files identical despite different names*

### Comparing `cron-validator-1.0.7/cron_validator/util.py` & `cron-validator-1.0.8/cron_validator/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import datetime
 import re
 
 import dateutil.parser
 import pytz
 
+month_names = ["jan", "feb", "mar", "apr", "may", "jun", "jul", "aug", "sep", "oct", "nov", "dec"]
+day_of_week_names = ["sun", "mon", "tue", "wed", "thu", "fri", "sat"]
+month_names_re = re.compile(rf"(?<![\d\/])({'|'.join(month_names)})(?!\d)", re.IGNORECASE)
+day_of_week_names_re = re.compile(rf"(?<![\d\/])({'|'.join(day_of_week_names)})(?!\d)", re.IGNORECASE)
 
 def get_tz(tz_name):
     """
 
     :param str tz_name:
     :return:
     """
@@ -35,22 +39,20 @@
 def replace_names(expression):
     """
 
     :param expression:
     :return:
     """
     parts = expression.split(" ")
-    month_names = ["jan", "feb", "mar", "apr", "may", "jun", "jul", "aug", "sep", "oct", "nov", "dec"]
-    day_of_week_names = ["sun", "mon", "tue", "wed", "thu", "fri", "sat"]
-    month_names_re = re.compile(rf"(?<![\d\/])({'|'.join(month_names)})(?!\d)", re.IGNORECASE)
-    day_of_week_names_re = re.compile(rf"(?<![\d\/])({'|'.join(day_of_week_names)})(?!\d)", re.IGNORECASE)
-    parts[3] = re.sub(
-        month_names_re, 
-        lambda m: str(month_names.index(m.group().lower()) + 1), 
-        parts[3]
-    )
-    parts[4] = re.sub(
-        day_of_week_names_re, 
-        lambda m: str(day_of_week_names.index(m.group().lower())), 
-        parts[4]
-    )
+    if len(parts) > 3:
+        parts[3] = re.sub(
+            month_names_re,
+            lambda m: str(month_names.index(m.group().lower()) + 1),
+            parts[3]
+        )
+    if len(parts) > 4:
+        parts[4] = re.sub(
+            day_of_week_names_re,
+            lambda m: str(day_of_week_names.index(m.group().lower())),
+            parts[4]
+        )
     return " ".join(parts)
```

### Comparing `cron-validator-1.0.7/cron_validator/validator.py` & `cron-validator-1.0.8/cron_validator/validator.py`

 * *Files identical despite different names*

### Comparing `cron-validator-1.0.7/cron_validator.egg-info/PKG-INFO` & `cron-validator-1.0.8/cron_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cron-validator
-Version: 1.0.7
+Version: 1.0.8
 Summary: Unix cron implementation by Python
 Home-page: https://github.com/vcoder4c/cron-validator
 Author: vcoder
 Author-email: doanngocbao@gmail.com
 License: MIT
-Download-URL: https://github.com/vcoder4c/cron-validator/archive/v1.0.7.tar.gz
+Download-URL: https://github.com/vcoder4c/cron-validator/archive/v1.0.8.tar.gz
 Keywords: cron,python,cron expression validator,cron expression iterator,cron scheduler
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Cron Validator
```

### Comparing `cron-validator-1.0.7/setup.py` & `cron-validator-1.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 else:
     with open("README.md", encoding="utf-8") as f:
         long_description = f.read()
 
 setup(
     name="cron-validator",
     packages=["cron_validator"],
-    version="1.0.7",
+    version="1.0.8",
     license="MIT",
     description="Unix cron implementation by Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="vcoder",
     author_email="doanngocbao@gmail.com",
     url="https://github.com/vcoder4c/cron-validator",
     keywords=["cron", "python", "cron expression validator", "cron expression iterator", "cron scheduler"],
-    download_url="https://github.com/vcoder4c/cron-validator/archive/v1.0.7.tar.gz",
+    download_url="https://github.com/vcoder4c/cron-validator/archive/v1.0.8.tar.gz",
     install_requires=["python_dateutil", "pytz"],
 )
```

### Comparing `cron-validator-1.0.7/test/test_CronScheduler.py` & `cron-validator-1.0.8/test/test_CronScheduler.py`

 * *Files identical despite different names*

### Comparing `cron-validator-1.0.7/test/test_execution_time.py` & `cron-validator-1.0.8/test/test_execution_time.py`

 * *Files identical despite different names*

### Comparing `cron-validator-1.0.7/test/test_match.py` & `cron-validator-1.0.8/test/test_match.py`

 * *Files identical despite different names*

### Comparing `cron-validator-1.0.7/test/test_util.py` & `cron-validator-1.0.8/test/test_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,7 +38,9 @@
 def test_replace_names():
     assert replace_names("* * * */2,3 6") == "* * * */2,3 6"
     assert replace_names("* * * may fri") == "* * * 5 5"
     assert replace_names("* * * jan-sep,nov mon/2") == "* * * 1-9,11 1/2"
     assert replace_names("* * * feb,aug,oct tue,WED,sAT") == "* * * 2,8,10 2,3,6"
     assert replace_names("* * * MAR-apr thu-fri") == "* * * 3-4 4-5"
     assert replace_names("* * * mAy,jun,JUL-DEC SUN/3") == "* * * 5,6,7-12 0/3"
+
+    assert replace_names("invalid_cron") == "invalid_cron"
```

### Comparing `cron-validator-1.0.7/test/test_valid_regex.py` & `cron-validator-1.0.8/test/test_valid_regex.py`

 * *Files identical despite different names*

