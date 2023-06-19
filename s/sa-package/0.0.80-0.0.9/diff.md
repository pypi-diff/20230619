# Comparing `tmp/sa_package-0.0.80.tar.gz` & `tmp/sa_package-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sa_package-0.0.80.tar", last modified: Mon Jun 19 09:08:57 2023, max compression
+gzip compressed data, was "sa_package-0.0.9.tar", last modified: Sun Nov 20 08:40:08 2022, max compression
```

## Comparing `sa_package-0.0.80.tar` & `sa_package-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 09:08:57.710084 sa_package-0.0.80/
--rw-rw-rw-   0        0        0        0 2022-11-14 08:11:02.000000 sa_package-0.0.80/LICENSE
--rw-rw-rw-   0        0        0      194 2023-06-19 09:08:57.708057 sa_package-0.0.80/PKG-INFO
--rw-rw-rw-   0        0        0       15 2022-11-20 08:50:45.000000 sa_package-0.0.80/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 09:08:57.562364 sa_package-0.0.80/sa_package/
--rw-rw-rw-   0        0        0        0 2023-01-07 03:45:28.000000 sa_package-0.0.80/sa_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:08:57.614150 sa_package-0.0.80/sa_package/calendar/
--rw-rw-rw-   0        0        0        0 2022-11-20 07:19:46.000000 sa_package-0.0.80/sa_package/calendar/__init__.py
--rw-rw-rw-   0        0        0     1406 2023-01-07 05:40:12.000000 sa_package-0.0.80/sa_package/calendar/calculate_date.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:08:57.629182 sa_package-0.0.80/sa_package/convert/
--rw-rw-rw-   0        0        0        0 2022-11-14 08:11:02.000000 sa_package-0.0.80/sa_package/convert/__init__.py
--rw-rw-rw-   0        0        0      816 2023-01-31 01:30:43.000000 sa_package-0.0.80/sa_package/convert/datetime_format.py
--rw-rw-rw-   0        0        0     1595 2023-01-07 06:13:32.000000 sa_package-0.0.80/sa_package/convert/number_format.py
--rw-rw-rw-   0        0        0     1904 2023-02-14 08:40:56.000000 sa_package-0.0.80/sa_package/convert/time_format.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:08:57.646271 sa_package-0.0.80/sa_package/google_api/
--rw-rw-rw-   0        0        0        0 2022-11-14 08:11:02.000000 sa_package-0.0.80/sa_package/google_api/__init__.py
--rw-rw-rw-   0        0        0     2189 2022-11-14 08:11:02.000000 sa_package-0.0.80/sa_package/google_api/my_gmail.py
--rw-rw-rw-   0        0        0    16814 2023-03-07 02:17:40.000000 sa_package-0.0.80/sa_package/google_api/my_gspread.py
--rw-rw-rw-   0        0        0     4298 2023-06-19 09:07:58.000000 sa_package-0.0.80/sa_package/google_api/my_youtube.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:08:57.654122 sa_package-0.0.80/sa_package/my_selenium/
--rw-rw-rw-   0        0        0        0 2022-11-25 08:38:47.000000 sa_package-0.0.80/sa_package/my_selenium/__init__.py
--rw-rw-rw-   0        0        0      569 2022-11-25 08:53:13.000000 sa_package-0.0.80/sa_package/my_selenium/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:08:57.657284 sa_package-0.0.80/sa_package/mydatabase/
--rw-rw-rw-   0        0        0     2360 2023-02-17 07:35:27.000000 sa_package-0.0.80/sa_package/mydatabase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:08:57.703736 sa_package-0.0.80/sa_package/platform/
--rw-rw-rw-   0        0        0        0 2022-11-20 08:34:44.000000 sa_package-0.0.80/sa_package/platform/__init__.py
--rw-rw-rw-   0        0        0    20523 2023-04-21 05:18:43.000000 sa_package-0.0.80/sa_package/platform/afreecatv.py
--rw-rw-rw-   0        0        0     3455 2023-04-03 07:42:12.000000 sa_package-0.0.80/sa_package/platform/google.py
--rw-rw-rw-   0        0        0     1876 2023-01-07 02:49:22.000000 sa_package-0.0.80/sa_package/platform/slack.py
--rw-rw-rw-   0        0        0     6453 2023-01-07 01:42:08.000000 sa_package-0.0.80/sa_package/platform/youtube.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:08:57.608073 sa_package-0.0.80/sa_package.egg-info/
--rw-rw-rw-   0        0        0      194 2023-06-19 09:08:57.000000 sa_package-0.0.80/sa_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      827 2023-06-19 09:08:57.000000 sa_package-0.0.80/sa_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 09:08:57.000000 sa_package-0.0.80/sa_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2023-06-19 09:08:57.000000 sa_package-0.0.80/sa_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 09:08:57.000000 sa_package-0.0.80/sa_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 09:08:57.711085 sa_package-0.0.80/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-19 09:08:25.000000 sa_package-0.0.80/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-20 08:40:08.477459 sa_package-0.0.9/
+-rw-rw-rw-   0        0        0        0 2022-11-14 08:11:02.000000 sa_package-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      261 2022-11-20 08:40:08.475464 sa_package-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2022-11-14 08:11:02.000000 sa_package-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-11-20 08:40:08.438564 sa_package-0.0.9/sa_package/
+-rw-rw-rw-   0        0        0        0 2022-11-20 08:34:44.000000 sa_package-0.0.9/sa_package/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-20 08:40:08.472474 sa_package-0.0.9/sa_package/calendar/
+-rw-rw-rw-   0        0        0        0 2022-11-20 07:19:46.000000 sa_package-0.0.9/sa_package/calendar/__init__.py
+-rw-rw-rw-   0        0        0      842 2022-11-14 08:11:02.000000 sa_package-0.0.9/sa_package/calendar/calculate_date.py
+drwxrwxrwx   0        0        0        0 2022-11-20 08:40:08.464496 sa_package-0.0.9/sa_package.egg-info/
+-rw-rw-rw-   0        0        0      261 2022-11-20 08:40:08.000000 sa_package-0.0.9/sa_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2022-11-20 08:40:08.000000 sa_package-0.0.9/sa_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-20 08:40:08.000000 sa_package-0.0.9/sa_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2022-11-20 08:40:08.000000 sa_package-0.0.9/sa_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-11-20 08:40:08.000000 sa_package-0.0.9/sa_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-11-20 08:40:08.478457 sa_package-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      669 2022-11-20 08:40:04.000000 sa_package-0.0.9/setup.py
```

### Comparing `sa_package-0.0.80/sa_package/calendar/calculate_date.py` & `sa_package-0.0.9/sa_package/calendar/calculate_date.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,23 @@
 import datetime
 
-
-def first_day_of_month(any_day:datetime.date) -> datetime.date:    
+def first_day_of_month(any_day):    
     return any_day.replace(day=1)
 
 
-def last_day_of_month(any_day:datetime.date) -> datetime.date:
+def last_day_of_month(any_day):
     # this will never fail
     # get close to the end of the month for any day, and add 4 days 'over'
     next_month = any_day.replace(day=28) + datetime.timedelta(days=4)
     # subtract the number of remaining 'overage' days to get last day of current month, or said programattically said, the previous day of the first of next month
     return next_month - datetime.timedelta(days=next_month.day)
 
 
-def first_day_of_week(any_day:datetime.date) -> datetime.date:
+def first_day_of_week(any_day):
     return any_day - datetime.timedelta(days=any_day.weekday())
 
 
-def first_day_of_last_month(any_day:datetime.date=None) -> datetime.date:
-    if any_day is None:
-        any_day = datetime.date.today()
-
-    return (any_day.replace(day=1) - datetime.timedelta(days=1)).replace(day=1)
-
-
-def last_day_of_last_month(any_day:datetime.date=None) -> datetime.date:
-    if any_day is None:
-        any_day = datetime.date.today()
-
-    return any_day.replace(day=1) - datetime.timedelta(days=1)
-
-
-def last_day_of_last_week(any_day:datetime.date=None) -> datetime.date:
+def last_day_of_last_week(any_day=None):
     if any_day is None:
         any_day = datetime.date.today()
     
     return any_day - datetime.timedelta(days=any_day.weekday()+1)  # 이전 주 일요일
```

