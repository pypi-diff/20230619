# Comparing `tmp/capeditor-0.1.8.tar.gz` & `tmp/capeditor-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capeditor-0.1.8.tar", last modified: Thu May 18 07:13:02 2023, max compression
+gzip compressed data, was "capeditor-0.1.9.tar", last modified: Mon Jun 19 12:44:23 2023, max compression
```

## Comparing `capeditor-0.1.8.tar` & `capeditor-0.1.9.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:13:02.521781 capeditor-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-18 07:12:47.000000 capeditor-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-18 07:13:02.521781 capeditor-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-18 07:12:47.000000 capeditor-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:13:02.521781 capeditor-0.1.8/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:13:02.521781 capeditor-0.1.8/capeditor/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23430 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:13:02.517781 capeditor-0.1.8/capeditor/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:13:02.521781 capeditor-0.1.8/capeditor/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/static/css/header.css
--rw-r--r--   0 runner    (1001) docker     (123)    32997 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:13:02.521781 capeditor-0.1.8/capeditor/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/static/js/common.js
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/static/js/hide_attributes.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:13:02.517781 capeditor-0.1.8/capeditor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:13:02.521781 capeditor-0.1.8/capeditor/templates/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/templates/capeditor/alert_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/templates/capeditor/alert_filter_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/templates/capeditor/alert_index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/templates/capeditor/alert_item_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/templates/capeditor/alert_list_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/templates/capeditor/latest_alert_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/templates/capeditor/pagination_include.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:13:02.521781 capeditor-0.1.8/capeditor/templates/capeditor/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/templates/capeditor/widgets/basemap_polygon.html
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/templates/capeditor/widgets/polygon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:13:02.521781 capeditor-0.1.8/capeditor/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/templatetags/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-18 07:12:47.000000 capeditor-0.1.8/capeditor/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:13:02.521781 capeditor-0.1.8/capeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-18 07:13:02.000000 capeditor-0.1.8/capeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-18 07:13:02.000000 capeditor-0.1.8/capeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 07:13:02.000000 capeditor-0.1.8/capeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-18 07:13:02.000000 capeditor-0.1.8/capeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 07:13:02.000000 capeditor-0.1.8/capeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 07:13:02.521781 capeditor-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-18 07:12:47.000000 capeditor-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:44:23.704407 capeditor-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-19 12:44:15.000000 capeditor-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-06-19 12:44:23.704407 capeditor-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-06-19 12:44:15.000000 capeditor-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:44:23.700407 capeditor-0.1.9/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:44:23.704407 capeditor-0.1.9/capeditor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/migrations/0002_alter_alertinfo_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/migrations/0003_alter_alert_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:44:23.700407 capeditor-0.1.9/capeditor/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:44:23.704407 capeditor-0.1.9/capeditor/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/static/css/header.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32997 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:44:23.704407 capeditor-0.1.9/capeditor/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/static/js/common.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/static/js/hide_attributes.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:44:23.700407 capeditor-0.1.9/capeditor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:44:23.704407 capeditor-0.1.9/capeditor/templates/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/templates/capeditor/alert_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/templates/capeditor/alert_filter_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/templates/capeditor/alert_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/templates/capeditor/alert_item_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/templates/capeditor/alert_list_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/templates/capeditor/latest_alert_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/templates/capeditor/pagination_include.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:44:23.704407 capeditor-0.1.9/capeditor/templates/capeditor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/templates/capeditor/widgets/basemap_polygon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/templates/capeditor/widgets/polygon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:44:23.704407 capeditor-0.1.9/capeditor/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/templatetags/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-19 12:44:15.000000 capeditor-0.1.9/capeditor/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:44:23.704407 capeditor-0.1.9/capeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-06-19 12:44:23.000000 capeditor-0.1.9/capeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-19 12:44:23.000000 capeditor-0.1.9/capeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:44:23.000000 capeditor-0.1.9/capeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-19 12:44:23.000000 capeditor-0.1.9/capeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-19 12:44:23.000000 capeditor-0.1.9/capeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 12:44:23.704407 capeditor-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-19 12:44:15.000000 capeditor-0.1.9/setup.py
```

### Comparing `capeditor-0.1.8/PKG-INFO` & `capeditor-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.1.8
+Version: 0.1.9
 Summary: Wagtail CAP Editor can be run as standalone or integrated into website
 Home-page: https://github.com/wmo-raf/cap-editor
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `capeditor-0.1.8/README.md` & `capeditor-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/migrations/0001_initial.py` & `capeditor-0.1.9/capeditor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/models.py` & `capeditor-0.1.9/capeditor/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     template = "capeditor/alert_index.html"
     ajax_template = 'capeditor/alert_list_include.html'
 
     subpage_types = [
         'capeditor.Alert',  # appname.ModelName
     ]
     parent_page_type = [
-        'wagtailcore.Page'  # appname.ModelName
+        # 'wagtailcore.Page'  # appname.ModelName
     ]
     max_count = 1
 
     alerts_per_page = models.PositiveIntegerField(default=6, validators=[
         MinValueValidator(6),
         MaxValueValidator(20),
     ], help_text=_("How many of this products should be visible on the landing page filter section ?"),
@@ -70,15 +70,15 @@
             'Unlikely': _("Unlikely - Not expected to occur (percentage ~ 0)"),
             'Unknown': _("Unknown - Certainty unknown"),
         }
         return {'urgency': URGENCIES, 'severity':SEVERITIES, 'certainty': CERTAINTIES}
 
     @property
     def all_alerts(self):
-        return Alert.objects.live()
+        return Alert.objects.live().exclude(status='Draft').filter(scope='Public').order_by('-alert_info__effective')
 
     def filter_alerts(self, request):
         alerts = self.all_alerts
 
         
         urgency = query_param_to_list(request.GET.get("urgency"), as_int=False)
         severity = query_param_to_list(request.GET.get("severity"), as_int=False)
@@ -152,15 +152,15 @@
     )
 
   
     identifier = models.UUIDField(default=uuid.uuid4, editable=False,
                                   help_text=_("Unique ID. Auto generated on creation."), verbose_name=_("Identifier"))
     sender = models.EmailField(max_length=255,
                               help_text=_(" Identifies the originator of an alert. "
-                                        "This can be an email of the institution for example"), default='grace@gmail.com', verbose_name=_("Sender"))
+                                        "This can be an email of the institution for example"), verbose_name=_("Sender"))
     sent = models.DateTimeField(help_text=_("Time and date of origination of the alert"), default=timezone.now, verbose_name=_("Sent"))
     status = models.CharField(max_length=50, choices=STATUS_CHOICES,
                               help_text=_("The code denoting the appropriate handling of the alert"), default='Actual', verbose_name=_("Status"))
     msgType = models.CharField(max_length=100, choices=MESSAGE_TYPE_CHOICES,
                                     help_text=_("The code denoting the nature of the alert message"),  default='Alert', verbose_name=_("Message Type"))
     scope = models.CharField(max_length=100,
                              choices=SCOPE_CHOICES,
@@ -241,14 +241,18 @@
     def __str__(self):
         return self.title
 
 class AlertInfo(ClusterableModel):
 
     LANGUAGE_CHOICES = (
         ('en', _("English")),
+        ('fr', _("French")),
+        ('ar', _("Arabic")),
+        ('am', _("Amharic")),
+        ('sw', _("Swahili")),
     )
 
     CATEGORY_CHOICES = (
         ('Geo', _("Geophysical")),
         ('Met', _("Meteorological")),
         ('Safety', _("General emergency and public safety")),
         ('Security', _("Law enforcement, military, homeland and local/private security")),
```

### Comparing `capeditor-0.1.8/capeditor/renderers.py` & `capeditor-0.1.9/capeditor/renderers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/serializers.py` & `capeditor-0.1.9/capeditor/serializers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/static/css/header.css` & `capeditor-0.1.9/capeditor/static/css/header.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/static/css/style.css` & `capeditor-0.1.9/capeditor/static/css/style.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/static/js/common.js` & `capeditor-0.1.9/capeditor/static/js/common.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/static/js/hide_attributes.js` & `capeditor-0.1.9/capeditor/static/js/hide_attributes.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/templates/capeditor/alert_detail.html` & `capeditor-0.1.9/capeditor/templates/capeditor/alert_detail.html`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,16 @@
 {% load wagtailcore_tags static %}
 
 {% block extra_css %}
 {{ block.super }}
 
 <link href='https://unpkg.com/maplibre-gl@2.4.0/dist/maplibre-gl.css' rel='stylesheet' />
 <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@0.9.4/css/bulma.min.css">
-<link rel="stylesheet" type="text/css" href="{% static 'css/header.css' %}">
 <link rel="stylesheet" type="text/css" href="{% static 'css/style.css' %}">
 
-
-
 <style>
   .tabs li a {
     color: rgb(239, 239, 239);
   }
   .tabs.is-active {
     color: #333;
   }
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
 {% extends 'base.html' %} {% load wagtailcore_tags static %} {% block extra_css
 %} {{ block.super }}
 
 
-
  {% endblock %} {% block content %}
 {% comment %}
 ***** Latest Alert *****
 {% endcomment %} {% include 'capeditor/alert_item_include.html' with
 item_title=page.title item_url=page.url item_info=page.alert_info.all
 item_identifier=page.identifier %}
   {% endblock content %}
```

### Comparing `capeditor-0.1.8/capeditor/templates/capeditor/alert_filter_include.html` & `capeditor-0.1.9/capeditor/templates/capeditor/alert_filter_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/templates/capeditor/alert_index.html` & `capeditor-0.1.9/capeditor/templates/capeditor/alert_index.html`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 
 {% block content %}
 <main class="is-index">
 
 {% if latest_alert %}
       <section class="featured-event-section">
           <div class="container">
-              <h2 class="section-title center">Latest Alert</h2>
+              <h2 class="section-title center">{{page.title}}</h2>
+
+              <h3 class="section-title center">Latest Alert</h3>
               {% include 'capeditor/latest_alert_include.html' with item_title=latest_alert.title item_url=latest_alert.url item_info=latest_alert.alert_info.all item_identifier=latest_alert.identifier%}
           </div>
       </section>
   {% endif %}
 
   <section class="listing-section">
     <h2 id="results" class="section-title has-text-centered">Browse CAP Alerts</h2>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 {% extends 'base.html' %} {% load wagtailcore_tags static %} {% block extra_css
 %} {{ block.super }}
 
 
  {% endblock %} {% block extra_js %} {{ block.super }}
  {% endblock %} {% block content %}  {% if latest_alert %}
-***** Latest Alert *****
+***** {{page.title}} *****
+**** Latest Alert ****
 {% include 'capeditor/latest_alert_include.html' with
 item_title=latest_alert.title item_url=latest_alert.url
 item_info=latest_alert.alert_info.all item_identifier=latest_alert.identifier%}
  {% endif %}
 ***** Browse CAP Alerts *****
 {% include 'capeditor/alert_filter_include.html' with filters=page.filters %}
 {% include 'capeditor/alert_list_include.html' with alerts=alerts %}
```

### Comparing `capeditor-0.1.8/capeditor/templates/capeditor/alert_item_include.html` & `capeditor-0.1.9/capeditor/templates/capeditor/alert_item_include.html`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,16 @@
       </div>
 
     </div>
   </div>
 </div>
 
 {% block extra_js %}
+<script src="https://code.jquery.com/jquery-3.6.3.min.js"
+        integrity="sha256-pvPw+upLPUjgMXY0G+8O0xUf+/Im1MZjXxxgOcBQBXU=" crossorigin="anonymous"></script>
 <script src="https://kit.fontawesome.com/db8ac3c257.js" crossorigin="anonymous"></script>
 <script src="https://cdn.maptiler.com/maplibre-gl-js/v2.4.0/maplibre-gl.js"></script>
 <script src="https://unpkg.com/@turf/turf@6.5.0/turf.min.js"></script>
 <script>
   const detail_map = new maplibregl.Map({
     container: "alert-map", // container ID
     style: "https://api.maptiler.com/maps/basic-v2/style.json?key=uYCBTRo5fyHCkPvoa5Io", // style URL
```

### Comparing `capeditor-0.1.8/capeditor/templates/capeditor/alert_list_include.html` & `capeditor-0.1.9/capeditor/templates/capeditor/alert_list_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/templates/capeditor/latest_alert_include.html` & `capeditor-0.1.9/capeditor/templates/capeditor/latest_alert_include.html`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,16 @@
           </div>
       </div>
       
   </div>
 </div>
 
 {% block extra_js %}
+<script src="https://code.jquery.com/jquery-3.6.3.min.js"
+        integrity="sha256-pvPw+upLPUjgMXY0G+8O0xUf+/Im1MZjXxxgOcBQBXU=" crossorigin="anonymous"></script>
 <script src="https://kit.fontawesome.com/db8ac3c257.js" crossorigin="anonymous"></script>
 <script src="https://cdn.maptiler.com/maplibre-gl-js/v2.4.0/maplibre-gl.js"></script>
 <script src="https://unpkg.com/@turf/turf@6.5.0/turf.min.js"></script>
 <script>
     const latest_map = new maplibregl.Map({
         container: "alert-map", // container ID
         style: "https://api.maptiler.com/maps/basic-v2/style.json?key=uYCBTRo5fyHCkPvoa5Io", // style URL
```

### Comparing `capeditor-0.1.8/capeditor/templates/capeditor/pagination_include.html` & `capeditor-0.1.9/capeditor/templates/capeditor/pagination_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/templates/capeditor/widgets/polygon.html` & `capeditor-0.1.9/capeditor/templates/capeditor/widgets/polygon.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/templatetags/pagination.py` & `capeditor-0.1.9/capeditor/templatetags/pagination.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/utils.py` & `capeditor-0.1.9/capeditor/utils.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/views.py` & `capeditor-0.1.9/capeditor/views.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/wagtail_hooks.py` & `capeditor-0.1.9/capeditor/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor/widgets.py` & `capeditor-0.1.9/capeditor/widgets.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.8/capeditor.egg-info/PKG-INFO` & `capeditor-0.1.9/capeditor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.1.8
+Version: 0.1.9
 Summary: Wagtail CAP Editor can be run as standalone or integrated into website
 Home-page: https://github.com/wmo-raf/cap-editor
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `capeditor-0.1.8/capeditor.egg-info/SOURCES.txt` & `capeditor-0.1.9/capeditor.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 capeditor/widgets.py
 capeditor.egg-info/PKG-INFO
 capeditor.egg-info/SOURCES.txt
 capeditor.egg-info/dependency_links.txt
 capeditor.egg-info/requires.txt
 capeditor.egg-info/top_level.txt
 capeditor/migrations/0001_initial.py
+capeditor/migrations/0002_alter_alertinfo_language.py
+capeditor/migrations/0003_alter_alert_sender.py
 capeditor/migrations/__init__.py
 capeditor/static/css/header.css
 capeditor/static/css/style.css
 capeditor/static/js/common.js
 capeditor/static/js/hide_attributes.js
 capeditor/templates/capeditor/alert_detail.html
 capeditor/templates/capeditor/alert_filter_include.html
```

### Comparing `capeditor-0.1.8/setup.py` & `capeditor-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 install_requirements = parse_requirements(os.path.join(PROJECT_ROOT, 'requirements.txt'), session=uuid.uuid1())
 
 # e.g. ['django', 'google-api-python-client']
 requirements = [getattr(ir, 'requirement', str(getattr(ir, 'req', None))) for ir in install_requirements]
 
 setup(
     name='capeditor',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     install_requires=requirements,
     include_package_data=True,
     license='MIT License',
     description='Wagtail CAP Editor can be run as standalone or integrated into website',
     long_description=README,
     long_description_content_type='text/markdown',
```

