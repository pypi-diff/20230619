# Comparing `tmp/forecastmanager-0.0.2.tar.gz` & `tmp/forecastmanager-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastmanager-0.0.2.tar", last modified: Sun Jun 18 18:36:58 2023, max compression
+gzip compressed data, was "forecastmanager-0.0.3.tar", last modified: Mon Jun 19 08:57:00 2023, max compression
```

## Comparing `forecastmanager-0.0.2.tar` & `forecastmanager-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/forecastmanager/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/forecastmanager/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/management/commands/generate_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/forecastmanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/site_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/forecastmanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/forecastmanager/templates/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/templates/forecastmanager/create_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/templates/forecastmanager/forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/templates/forecastmanager/query_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/forecastmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-18 18:36:58.000000 forecastmanager-0.0.2/forecastmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-18 18:36:58.000000 forecastmanager-0.0.2/forecastmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:36:58.000000 forecastmanager-0.0.2/forecastmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-18 18:36:58.000000 forecastmanager-0.0.2/forecastmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 18:36:58.000000 forecastmanager-0.0.2/forecastmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.778028 forecastmanager-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-19 08:57:00.778028 forecastmanager-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.774028 forecastmanager-0.0.3/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.774028 forecastmanager-0.0.3/forecastmanager/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.778028 forecastmanager-0.0.3/forecastmanager/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/management/commands/generate_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.778028 forecastmanager-0.0.3/forecastmanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/site_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.774028 forecastmanager-0.0.3/forecastmanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.778028 forecastmanager-0.0.3/forecastmanager/templates/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/templates/forecastmanager/create_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/templates/forecastmanager/forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/templates/forecastmanager/query_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.774028 forecastmanager-0.0.3/forecastmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-19 08:57:00.000000 forecastmanager-0.0.3/forecastmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-19 08:57:00.000000 forecastmanager-0.0.3/forecastmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:57:00.000000 forecastmanager-0.0.3/forecastmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-19 08:57:00.000000 forecastmanager-0.0.3/forecastmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 08:57:00.000000 forecastmanager-0.0.3/forecastmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-19 08:57:00.778028 forecastmanager-0.0.3/setup.cfg
```

### Comparing `forecastmanager-0.0.2/PKG-INFO` & `forecastmanager-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.0.2
+Version: 0.0.3
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.0.2/forecastmanager/management/commands/generate_forecast.py` & `forecastmanager-0.0.3/forecastmanager/management/commands/generate_forecast.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.2/forecastmanager/migrations/0001_initial.py` & `forecastmanager-0.0.3/forecastmanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.2/forecastmanager/models.py` & `forecastmanager-0.0.3/forecastmanager/models.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.2/forecastmanager/site_settings.py` & `forecastmanager-0.0.3/forecastmanager/site_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 from wagtail.admin.panels import (
     FieldPanel,
     TabbedInterface,
     ObjectList,
 )
-# @register_setting
+@register_setting
 class Setting(BaseSiteSetting):
     enable_auto_forecast = models.BooleanField(
         default=True,
         verbose_name=_('Enable automated forecasts')
     )
 
     TEMPERATURE_UNITS = (
```

### Comparing `forecastmanager-0.0.2/forecastmanager/templates/forecastmanager/create_forecast.html` & `forecastmanager-0.0.3/forecastmanager/templates/forecastmanager/create_forecast.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.2/forecastmanager/templates/forecastmanager/forecast.html` & `forecastmanager-0.0.3/forecastmanager/templates/forecastmanager/forecast.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.2/forecastmanager/templates/forecastmanager/query_forecast.html` & `forecastmanager-0.0.3/forecastmanager/templates/forecastmanager/query_forecast.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.2/forecastmanager/views.py` & `forecastmanager-0.0.3/forecastmanager/views.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.2/forecastmanager/wagtail_hooks.py` & `forecastmanager-0.0.3/forecastmanager/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.2/forecastmanager.egg-info/PKG-INFO` & `forecastmanager-0.0.3/forecastmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.0.2
+Version: 0.0.3
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.0.2/forecastmanager.egg-info/SOURCES.txt` & `forecastmanager-0.0.3/forecastmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.2/setup.cfg` & `forecastmanager-0.0.3/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = forecastmanager
-version = 0.0.2
+version = 0.0.3
 description = Integration of Weather City Forecasts Manager in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/forecastmanager
 author = Grace Amondi
 author_email = miswa.grace@gmail.com
 license = MIT
```

