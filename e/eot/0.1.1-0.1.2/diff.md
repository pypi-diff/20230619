# Comparing `tmp/eot-0.1.1.tar.gz` & `tmp/eot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eot-0.1.1.tar", last modified: Sat Jun  3 19:54:25 2023, max compression
+gzip compressed data, was "eot-0.1.2.tar", last modified: Mon Jun 19 00:24:18 2023, max compression
```

## Comparing `eot-0.1.1.tar` & `eot-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:54:25.131075 eot-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-03 19:54:25.131075 eot-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-03 19:54:04.000000 eot-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:54:25.127075 eot-0.1.1/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:54:25.131075 eot-0.1.1/pkg/eot/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-03 19:54:16.000000 eot-0.1.1/pkg/eot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 19:54:16.000000 eot-0.1.1/pkg/eot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-03 19:54:16.000000 eot-0.1.1/pkg/eot/eot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:54:25.131075 eot-0.1.1/pkg/eot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-03 19:54:25.000000 eot-0.1.1/pkg/eot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-03 19:54:25.000000 eot-0.1.1/pkg/eot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 19:54:25.000000 eot-0.1.1/pkg/eot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-03 19:54:25.000000 eot-0.1.1/pkg/eot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-03 19:54:25.000000 eot-0.1.1/pkg/eot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-03 19:54:16.000000 eot-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-03 19:54:25.135075 eot-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:24:18.264871 eot-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-19 00:24:18.264871 eot-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-19 00:24:00.000000 eot-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:24:18.260871 eot-0.1.2/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:24:18.264871 eot-0.1.2/pkg/eot/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-19 00:24:10.000000 eot-0.1.2/pkg/eot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-19 00:24:10.000000 eot-0.1.2/pkg/eot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-19 00:24:10.000000 eot-0.1.2/pkg/eot/eot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:24:18.264871 eot-0.1.2/pkg/eot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-19 00:24:18.000000 eot-0.1.2/pkg/eot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-19 00:24:18.000000 eot-0.1.2/pkg/eot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 00:24:18.000000 eot-0.1.2/pkg/eot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-19 00:24:18.000000 eot-0.1.2/pkg/eot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-19 00:24:18.000000 eot-0.1.2/pkg/eot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-19 00:24:10.000000 eot-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-19 00:24:18.264871 eot-0.1.2/setup.cfg
```

### Comparing `eot-0.1.1/pkg/eot/eot.py` & `eot-0.1.2/pkg/eot/eot.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 	@staticmethod
 	def GetStardate():
 		now = datetime.utcnow()
 		year = now.year
 		day_of_year = now.timetuple().tm_yday
 		hour = now.hour
 		minute = now.minute
-		second = now.second
+		second = now.microsecond / 1000000
 
 		one_hour = 1 / 24 / 365
 		one_minute = one_hour / 60
 		one_second = one_minute / 60
 
 		exact_day = (day_of_year / 365)
 		exact_hour = hour * one_hour
-		exact_minute = now.minute * one_minute
-		exact_second = now.second * one_second
+		exact_minute = minute * one_minute
+		exact_second = second * one_second
 		exact_decimal = exact_day + exact_hour + exact_minute + exact_second
-		decimal = float('%.8f' % (exact_decimal))
+		decimal = float('%.12f' % (exact_decimal))
 		# error = decimal * 365 - day_of_year - (hour / 24)
 		# error_hours = error * 24
-		stardate = format(year + decimal, '.8f')
+		stardate = format(year + decimal, '.10f')
 
 		# print("stardate for", year, day_of_year, hour)
 		# print("error:", error, "in hours:", error_hours)
 		return stardate
 
 	#Called when executing this as a functor.
 	def __call__(this):
```

