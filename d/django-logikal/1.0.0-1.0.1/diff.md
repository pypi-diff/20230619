# Comparing `tmp/django-logikal-1.0.0.tar.gz` & `tmp/django-logikal-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-logikal-1.0.0.tar", last modified: Sat Jun 17 16:45:49 2023, max compression
+gzip compressed data, was "django-logikal-1.0.1.tar", last modified: Mon Jun 19 17:36:30 2023, max compression
```

## Comparing `django-logikal-1.0.0.tar` & `django-logikal-1.0.1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.332282 django-logikal-1.0.0/
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      674 2023-06-17 15:42:42.000000 django-logikal-1.0.0/.copier-answers.yml
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     1052 2023-06-17 15:42:42.000000 django-logikal-1.0.0/LICENSE.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)       68 2023-06-17 15:42:42.000000 django-logikal-1.0.0/MANIFEST.in
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     2512 2023-06-17 16:45:49.332282 django-logikal-1.0.0/PKG-INFO
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      220 2023-06-17 15:42:42.000000 django-logikal-1.0.0/README.rst
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      730 2023-06-17 15:42:42.000000 django-logikal-1.0.0/compose.yml
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.316282 django-logikal-1.0.0/django_logikal/
--rw-rw-r--   0 gregory   (1000) gregory   (1000)       56 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/__init__.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     2108 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/apps.py
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.316282 django-logikal-1.0.0/django_logikal/babel/
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      242 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/babel/django.ini
--rw-rw-r--   0 gregory   (1000) gregory   (1000)       20 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/babel/djangojs.ini
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     6663 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/bibliography.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     6453 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/email.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      457 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/env.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      193 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/local_data.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     4550 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/logging.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      485 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/manage.py
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.316282 django-logikal-1.0.0/django_logikal/management/
--rw-rw-r--   0 gregory   (1000) gregory   (1000)        0 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/management/__init__.py
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.316282 django-logikal-1.0.0/django_logikal/management/commands/
--rw-rw-r--   0 gregory   (1000) gregory   (1000)        0 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/management/commands/__init__.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      915 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/management/commands/generate.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     3746 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/management/commands/syncdb.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     7637 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/management/commands/translate.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      322 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/middleware.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      716 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/migrations.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      482 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/models.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)        0 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/py.typed
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      247 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/pyproject.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     1327 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/run.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     1469 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/security.py
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.320282 django-logikal-1.0.0/django_logikal/settings/
--rw-rw-r--   0 gregory   (1000) gregory   (1000)        0 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/settings/__init__.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     4421 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/settings/base.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     3031 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/settings/dynamic_site.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     1282 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/settings/production.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      437 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/settings/static_site.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      392 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/settings/testing.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      575 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/sitemap.py
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.316282 django-logikal-1.0.0/django_logikal/static/
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.320282 django-logikal-1.0.0/django_logikal/static/django_logikal/
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.328282 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   600856 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   309728 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   184912 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   622572 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   323344 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   193308 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   639388 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   328412 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   195704 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     4494 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   617492 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Light.ttf
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   310884 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   181500 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff2
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   628640 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   325296 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   192916 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     3517 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-README.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   607720 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   309192 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   182708 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   614256 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   312952 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   184076 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   630852 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   327188 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   195128 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   610876 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   306060 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   180576 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   628352 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   323532 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff
--rw-rw-r--   0 gregory   (1000) gregory   (1000)   191804 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2
--rw-rw-r--   0 gregory   (1000) gregory   (1000)    87008 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf
--rw-rw-r--   0 gregory   (1000) gregory   (1000)    53528 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff
--rw-rw-r--   0 gregory   (1000) gregory   (1000)    40688 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2
--rw-rw-r--   0 gregory   (1000) gregory   (1000)    94148 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-r--   0 gregory   (1000) gregory   (1000)    59380 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff
--rw-rw-r--   0 gregory   (1000) gregory   (1000)    44824 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2
--rw-rw-r--   0 gregory   (1000) gregory   (1000)    93904 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf
--rw-rw-r--   0 gregory   (1000) gregory   (1000)    58800 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff
--rw-rw-r--   0 gregory   (1000) gregory   (1000)    44544 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2
--rw-rw-r--   0 gregory   (1000) gregory   (1000)    11560 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)    86908 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf
--rw-rw-r--   0 gregory   (1000) gregory   (1000)    53252 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff
--rw-rw-r--   0 gregory   (1000) gregory   (1000)    40672 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     3714 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/fonts.css
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      666 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static/django_logikal/validation_error.css
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      598 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/static.py
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.328282 django-logikal-1.0.0/django_logikal/templates/
--rw-rw-r--   0 gregory   (1000) gregory   (1000)       79 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/templates/__init__.py
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.328282 django-logikal-1.0.0/django_logikal/templates/admin/
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      377 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/templates/admin/base.html
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.328282 django-logikal-1.0.0/django_logikal/templates/debug_toolbar/
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      321 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/templates/debug_toolbar/base.html
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.328282 django-logikal-1.0.0/django_logikal/templates/django_logikal/
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      657 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/templates/django_logikal/base.html.j
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.328282 django-logikal-1.0.0/django_logikal/templates/django_logikal/email/
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      248 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/templates/django_logikal/email/base.html.j
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      956 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/templates/django_logikal/validation_error.html.j
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     1630 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/templates/extensions.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     1440 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/templates/filters.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     5339 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/templates/functions.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     3740 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/templates/jinja.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      346 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/templates/processors.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     2718 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/templates/template.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      176 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/templates/tests.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     2765 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/urls.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     2223 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/validation.py
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     1941 2023-06-17 15:42:42.000000 django-logikal-1.0.0/django_logikal/views.py
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.316282 django-logikal-1.0.0/django_logikal.egg-info/
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     2512 2023-06-17 16:45:49.000000 django-logikal-1.0.0/django_logikal.egg-info/PKG-INFO
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     5115 2023-06-17 16:45:49.000000 django-logikal-1.0.0/django_logikal.egg-info/SOURCES.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)        1 2023-06-17 16:45:49.000000 django-logikal-1.0.0/django_logikal.egg-info/dependency_links.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)       84 2023-06-17 16:45:49.000000 django-logikal-1.0.0/django_logikal.egg-info/entry_points.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      473 2023-06-17 16:45:49.000000 django-logikal-1.0.0/django_logikal.egg-info/requires.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)       15 2023-06-17 16:45:49.000000 django-logikal-1.0.0/django_logikal.egg-info/top_level.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     3358 2023-06-17 15:42:42.000000 django-logikal-1.0.0/pyproject.toml
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.328282 django-logikal-1.0.0/requirements/
--rw-rw-r--   0 gregory   (1000) gregory   (1000)       27 2023-06-17 15:42:42.000000 django-logikal-1.0.0/requirements/build.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     1038 2023-06-17 15:42:42.000000 django-logikal-1.0.0/requirements/build.txt.lock
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      414 2023-06-17 16:17:00.000000 django-logikal-1.0.0/requirements/core.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      149 2023-06-17 15:42:42.000000 django-logikal-1.0.0/requirements/dev.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     4425 2023-06-17 16:44:19.000000 django-logikal-1.0.0/requirements/dev.txt.lock
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      137 2023-06-17 16:44:19.000000 django-logikal-1.0.0/requirements/docs.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)     3894 2023-06-17 16:44:19.000000 django-logikal-1.0.0/requirements/docs.txt.lock
-drwxrwxr-x   0 gregory   (1000) gregory   (1000)        0 2023-06-17 16:45:49.332282 django-logikal-1.0.0/requirements/extras/
--rw-rw-r--   0 gregory   (1000) gregory   (1000)       15 2023-06-17 15:42:42.000000 django-logikal-1.0.0/requirements/extras/bibliography.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)      117 2023-06-17 15:42:42.000000 django-logikal-1.0.0/requirements/extras/dynamic.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)       20 2023-06-17 15:42:42.000000 django-logikal-1.0.0/requirements/extras/static.txt
--rw-rw-r--   0 gregory   (1000) gregory   (1000)       38 2023-06-17 16:45:49.332282 django-logikal-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.049968 django-logikal-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-19 17:36:00.000000 django-logikal-1.0.1/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-06-19 17:36:00.000000 django-logikal-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-19 17:36:00.000000 django-logikal-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2512 2023-06-19 17:36:30.049968 django-logikal-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-19 17:36:00.000000 django-logikal-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-06-19 17:36:00.000000 django-logikal-1.0.1/compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.021968 django-logikal-1.0.1/django_logikal/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.025968 django-logikal-1.0.1/django_logikal/babel/
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/babel/django.ini
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/babel/djangojs.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     6663 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/bibliography.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6453 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/email.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/env.py
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/local_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4602 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)      485 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.025968 django-logikal-1.0.1/django_logikal/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.025968 django-logikal-1.0.1/django_logikal/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/management/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3746 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/management/commands/syncdb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7637 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/management/commands/translate.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/security.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.025968 django-logikal-1.0.1/django_logikal/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4421 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3031 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/settings/dynamic_site.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/settings/static_site.py
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/settings/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/sitemap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.017968 django-logikal-1.0.1/django_logikal/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.025968 django-logikal-1.0.1/django_logikal/static/django_logikal/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.045968 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   600856 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   309728 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   184912 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   622572 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   323344 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   193308 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   639388 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   328412 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   195704 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)     4494 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)   617492 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   310884 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Light.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   181500 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Light.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   628640 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   325296 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   192916 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)     3517 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-README.txt
+-rw-r--r--   0 runner    (1001) docker     (122)   607720 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   309192 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   182708 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   614256 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   312952 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   184076 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   630852 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   327188 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   195128 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   610876 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   306060 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Thin.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   180576 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   628352 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   323532 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   191804 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)    87008 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    53528 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    40688 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)    94148 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    59380 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    44824 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)    93904 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    58800 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    44544 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)    11560 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    86908 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    53252 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    40672 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)     3714 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/validation_error.css
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.045968 django-logikal-1.0.1/django_logikal/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.045968 django-logikal-1.0.1/django_logikal/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      377 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/admin/base.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.045968 django-logikal-1.0.1/django_logikal/templates/debug_toolbar/
+-rw-r--r--   0 runner    (1001) docker     (122)      321 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/debug_toolbar/base.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.045968 django-logikal-1.0.1/django_logikal/templates/django_logikal/
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/django_logikal/base.html.j
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.045968 django-logikal-1.0.1/django_logikal/templates/django_logikal/email/
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/django_logikal/email/base.html.j
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/django_logikal/validation_error.html.j
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5460 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/processors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2718 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/template.py
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2223 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1941 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.025968 django-logikal-1.0.1/django_logikal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2512 2023-06-19 17:36:29.000000 django-logikal-1.0.1/django_logikal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5115 2023-06-19 17:36:30.000000 django-logikal-1.0.1/django_logikal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 17:36:29.000000 django-logikal-1.0.1/django_logikal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-19 17:36:29.000000 django-logikal-1.0.1/django_logikal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      473 2023-06-19 17:36:29.000000 django-logikal-1.0.1/django_logikal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-19 17:36:29.000000 django-logikal-1.0.1/django_logikal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3386 2023-06-19 17:36:00.000000 django-logikal-1.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.045968 django-logikal-1.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4425 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.049968 django-logikal-1.0.1/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/extras/bibliography.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/extras/dynamic.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/extras/static.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-19 17:36:30.049968 django-logikal-1.0.1/setup.cfg
```

### Comparing `django-logikal-1.0.0/.copier-answers.yml` & `django-logikal-1.0.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/LICENSE.txt` & `django-logikal-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/PKG-INFO` & `django-logikal-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-logikal
-Version: 1.0.0
+Version: 1.0.1
 Summary: Django utilities used at Logikal
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `django-logikal-1.0.0/compose.yml` & `django-logikal-1.0.1/compose.yml`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/apps.py` & `django-logikal-1.0.1/django_logikal/apps.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 
 from django.apps import AppConfig
 from django.conf import global_settings, settings
 from django.core.checks import Error, register
 from django.db.migrations import writer
 from django.template.loader import get_template
 
-from django_logikal.bibliography import Bibliography
 from django_logikal.migrations import FormattedMigrationWriter
 
 
 class DjangoLogikalConfig(AppConfig):
     name = 'django_logikal'
     verbose_name = 'django-logikal'
 
     def ready(self) -> None:
         # Load bibliographies
         if bibliographies := getattr(settings, 'BIBLIOGRAPHIES', None):
+            from django_logikal.bibliography import (  # pylint: disable=import-outside-toplevel
+                Bibliography,
+            )
+
             Bibliography.add_bibliographies({
                 # Note: both Django and Jinja2 templates have an origin attribute, so this is fine
                 name: get_template(path).origin.name  # type: ignore[attr-defined]
                 for name, path in bibliographies.items()
             })
 
         # Format migrations
```

### Comparing `django-logikal-1.0.0/django_logikal/bibliography.py` & `django-logikal-1.0.1/django_logikal/bibliography.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/email.py` & `django-logikal-1.0.1/django_logikal/email.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/logging.py` & `django-logikal-1.0.1/django_logikal/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import warnings
 from time import localtime, strftime
 from typing import Any, Callable, Mapping, Optional, Type
 
 from django.conf import settings
 from google.cloud import logging as cloud_logging
-from stormware.google.auth import GCPAuth
 from termcolor import colored
 
 
 class ConsoleLogFormatter(logging.Formatter):
     _STYLES: Mapping[str, Any] = {
         'timestamp': {'color': 'magenta'},
         'level': {
@@ -95,14 +94,16 @@
     }
 
     if console:
         config['root']['handlers'].append('console')
         warnings.formatwarning = ConsoleLogFormatter.warning_formatter()
 
     if cloud:
+        from stormware.google.auth import GCPAuth  # pylint: disable=import-outside-toplevel
+
         auth = GCPAuth()
         client = cloud_logging.Client(  # type: ignore[no-untyped-call]
             project=auth.project_id(),
             credentials=auth.credentials(),
         )
         config['handlers']['cloud'] = {
             'class': 'google.cloud.logging.handlers.CloudLoggingHandler',
```

### Comparing `django-logikal-1.0.0/django_logikal/management/commands/generate.py` & `django-logikal-1.0.1/django_logikal/management/commands/generate.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/management/commands/syncdb.py` & `django-logikal-1.0.1/django_logikal/management/commands/syncdb.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/management/commands/translate.py` & `django-logikal-1.0.1/django_logikal/management/commands/translate.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/migrations.py` & `django-logikal-1.0.1/django_logikal/migrations.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/run.py` & `django-logikal-1.0.1/django_logikal/run.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/security.py` & `django-logikal-1.0.1/django_logikal/security.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/settings/base.py` & `django-logikal-1.0.1/django_logikal/settings/base.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/settings/dynamic_site.py` & `django-logikal-1.0.1/django_logikal/settings/dynamic_site.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/settings/production.py` & `django-logikal-1.0.1/django_logikal/settings/production.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/sitemap.py` & `django-logikal-1.0.1/django_logikal/sitemap.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Bold.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Italic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Light.ttf` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Light.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff2` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Light.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-README.txt` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-README.txt`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Regular.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Thin.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/fonts.css` & `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts.css`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static/django_logikal/validation_error.css` & `django-logikal-1.0.1/django_logikal/static/django_logikal/validation_error.css`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/static.py` & `django-logikal-1.0.1/django_logikal/static.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/templates/django_logikal/base.html.j` & `django-logikal-1.0.1/django_logikal/templates/django_logikal/base.html.j`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/templates/django_logikal/validation_error.html.j` & `django-logikal-1.0.1/django_logikal/templates/django_logikal/validation_error.html.j`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/templates/extensions.py` & `django-logikal-1.0.1/django_logikal/templates/extensions.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/templates/filters.py` & `django-logikal-1.0.1/django_logikal/templates/filters.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/templates/functions.py` & `django-logikal-1.0.1/django_logikal/templates/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.safestring import SafeString, mark_safe
 from django.utils.translation import get_language
 from jinja2.runtime import Context
 from jinja2.utils import pass_context
 
-from django_logikal.bibliography import Bibliography
+import django_logikal  # for type checking
 
 
 @pass_context
 def context(context: Context) -> Context:  # pylint: disable=redefined-outer-name
     # noqa: D400, D402, D415
     """
     context()
@@ -152,15 +152,15 @@
 def now() -> datetime:
     """
     Return the current date and time.
     """
     return timezone.now()
 
 
-def bibliography(name: str) -> Bibliography:
+def bibliography(name: str) -> 'django_logikal.bibliography.Bibliography':
     """
     Return a :class:`~django_logikal.bibliography.Bibliography` instance.
 
     Args:
         name: The name of the bibliography configuration to use.
 
     .. note:: Requires the :ref:`bibliography extra <index:Bibliography>`.
@@ -182,8 +182,10 @@
         {% set cite = bib.cite %}
 
         ... {{ cite('entry') }} ...
 
         {{ bib.references() }}
 
     """
+    from django_logikal.bibliography import Bibliography  # pylint: disable=import-outside-toplevel
+
     return Bibliography(name=name)
```

### Comparing `django-logikal-1.0.0/django_logikal/templates/jinja.py` & `django-logikal-1.0.1/django_logikal/templates/jinja.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/templates/template.py` & `django-logikal-1.0.1/django_logikal/templates/template.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/urls.py` & `django-logikal-1.0.1/django_logikal/urls.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/validation.py` & `django-logikal-1.0.1/django_logikal/validation.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal/views.py` & `django-logikal-1.0.1/django_logikal/views.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/django_logikal.egg-info/PKG-INFO` & `django-logikal-1.0.1/django_logikal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-logikal
-Version: 1.0.0
+Version: 1.0.1
 Summary: Django utilities used at Logikal
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `django-logikal-1.0.0/django_logikal.egg-info/SOURCES.txt` & `django-logikal-1.0.1/django_logikal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/pyproject.toml` & `django-logikal-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
   'django_logikal.templates.django_logikal',
   'django_logikal.templates.django_logikal.email',
 ]
 
 [tool.setuptools_scm]
 
 [tool.pytest.ini_options]
+addopts = '--ignore=static'
 filterwarnings = [
   'error',
   # See https://github.com/googleapis/python-crc32c/issues/168
   'ignore:pkg_resources is deprecated as an API:DeprecationWarning',
   # See https://github.com/googleapis/api-common-protos/issues/121
   "ignore:Deprecated call to `pkg_resources.declare_namespace\\('google:DeprecationWarning",
   "ignore:Deprecated call to `pkg_resources.declare_namespace\\('sphinxcontrib:DeprecationWarning",
```

### Comparing `django-logikal-1.0.0/requirements/build.txt.lock` & `django-logikal-1.0.1/requirements/build.txt.lock`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/requirements/dev.txt.lock` & `django-logikal-1.0.1/requirements/dev.txt.lock`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.0/requirements/docs.txt.lock` & `django-logikal-1.0.1/requirements/docs.txt.lock`

 * *Files identical despite different names*

