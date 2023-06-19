# Comparing `tmp/zibanu-django-1.2.0b0.tar.gz` & `tmp/zibanu-django-1.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zibanu-django-1.2.0b0.tar", last modified: Mon Jun 19 16:44:21 2023, max compression
+gzip compressed data, was "zibanu-django-1.2.0b1.tar", last modified: Mon Jun 19 16:46:45 2023, max compression
```

## Comparing `zibanu-django-1.2.0b0.tar` & `zibanu-django-1.2.0b1.tar`

### file list

```diff
@@ -1,125 +1,102 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.821627 zibanu-django-1.2.0b0/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-1.2.0b0/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      208 2023-06-19 16:39:09.000000 zibanu-django-1.2.0b0/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41394 2023-06-19 16:44:21.821627 zibanu-django-1.2.0b0/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      179 2023-06-19 16:22:53.000000 zibanu-django-1.2.0b0/README.md
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      901 2023-06-19 16:40:16.000000 zibanu-django-1.2.0b0/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-06-19 16:44:21.821627 zibanu-django-1.2.0b0/setup.cfg
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.804628 zibanu-django-1.2.0b0/zibanu/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      623 2022-12-10 15:21:05.000000 zibanu-django-1.2.0b0/zibanu/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.804628 zibanu-django-1.2.0b0/zibanu/django/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-11 23:08:20.000000 zibanu-django-1.2.0b0/zibanu/django/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      895 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.805628 zibanu-django-1.2.0b0/zibanu/django/db/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 18:13:01.000000 zibanu-django-1.2.0b0/zibanu/django/db/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.805628 zibanu-django-1.2.0b0/zibanu/django/db/backends/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0b0/zibanu/django/db/backends/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.805628 zibanu-django-1.2.0b0/zibanu/django/db/backends/oracle/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0b0/zibanu/django/db/backends/oracle/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1158 2023-02-07 01:58:51.000000 zibanu-django-1.2.0b0/zibanu/django/db/backends/oracle/base.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.806628 zibanu-django-1.2.0b0/zibanu/django/db/models/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      766 2023-01-17 11:51:34.000000 zibanu-django-1.2.0b0/zibanu/django/db/models/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      931 2023-03-01 18:58:00.000000 zibanu-django-1.2.0b0/zibanu/django/db/models/dated_model.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1458 2023-03-03 23:10:34.000000 zibanu-django-1.2.0b0/zibanu/django/db/models/manager.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      738 2022-12-20 14:58:49.000000 zibanu-django-1.2.0b0/zibanu/django/db/models/model.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.800628 zibanu-django-1.2.0b0/zibanu/django/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.800628 zibanu-django-1.2.0b0/zibanu/django/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.806628 zibanu-django-1.2.0b0/zibanu/django/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2274 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3598 2023-04-27 15:33:39.000000 zibanu-django-1.2.0b0/zibanu/django/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.807628 zibanu-django-1.2.0b0/zibanu/django/logging/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-03-16 14:08:34.000000 zibanu-django-1.2.0b0/zibanu/django/logging/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      919 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.807628 zibanu-django-1.2.0b0/zibanu/django/logging/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 20:39:57.000000 zibanu-django-1.2.0b0/zibanu/django/logging/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.808627 zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1016 2023-05-13 19:57:25.000000 zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/on_change_password.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1243 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/on_login.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      975 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/on_send_mail.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.808627 zibanu-django-1.2.0b0/zibanu/django/logging/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:05:35.000000 zibanu-django-1.2.0b0/zibanu/django/logging/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      452 2023-05-13 17:50:17.000000 zibanu-django-1.2.0b0/zibanu/django/logging/lib/signals.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.801628 zibanu-django-1.2.0b0/zibanu/django/logging/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.801628 zibanu-django-1.2.0b0/zibanu/django/logging/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.809628 zibanu-django-1.2.0b0/zibanu/django/logging/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1185 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.809628 zibanu-django-1.2.0b0/zibanu/django/logging/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1501 2023-03-15 21:32:53.000000 zibanu-django-1.2.0b0/zibanu/django/logging/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1143 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/migrations/0002_maillog.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:33:26.000000 zibanu-django-1.2.0b0/zibanu/django/logging/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1946 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.810628 zibanu-django-1.2.0b0/zibanu/django/repository/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-03 02:16:47.000000 zibanu-django-1.2.0b0/zibanu/django/repository/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.810628 zibanu-django-1.2.0b0/zibanu/django/repository/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:42:37.000000 zibanu-django-1.2.0b0/zibanu/django/repository/api/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      958 2023-02-03 02:43:10.000000 zibanu-django-1.2.0b0/zibanu/django/repository/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.810628 zibanu-django-1.2.0b0/zibanu/django/repository/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:45:36.000000 zibanu-django-1.2.0b0/zibanu/django/repository/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.811627 zibanu-django-1.2.0b0/zibanu/django/repository/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      566 2023-02-04 20:47:18.000000 zibanu-django-1.2.0b0/zibanu/django/repository/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      740 2023-02-04 21:36:16.000000 zibanu-django-1.2.0b0/zibanu/django/repository/lib/managers/document.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.814628 zibanu-django-1.2.0b0/zibanu/django/repository/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      593 2023-02-04 20:45:36.000000 zibanu-django-1.2.0b0/zibanu/django/repository/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     7366 2023-06-03 20:53:46.000000 zibanu-django-1.2.0b0/zibanu/django/repository/lib/utils/document_generator.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.802628 zibanu-django-1.2.0b0/zibanu/django/repository/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.802628 zibanu-django-1.2.0b0/zibanu/django/repository/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.814628 zibanu-django-1.2.0b0/zibanu/django/repository/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1605 2023-02-09 14:40:51.000000 zibanu-django-1.2.0b0/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2664 2023-04-11 22:52:31.000000 zibanu-django-1.2.0b0/zibanu/django/repository/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.815627 zibanu-django-1.2.0b0/zibanu/django/repository/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1372 2023-02-03 02:43:34.000000 zibanu-django-1.2.0b0/zibanu/django/repository/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      427 2023-02-08 14:23:11.000000 zibanu-django-1.2.0b0/zibanu/django/repository/migrations/0002_document_description.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-02-03 02:23:41.000000 zibanu-django-1.2.0b0/zibanu/django/repository/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1575 2023-02-08 14:23:06.000000 zibanu-django-1.2.0b0/zibanu/django/repository/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.815627 zibanu-django-1.2.0b0/zibanu/django/rest_framework/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 12:39:27.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1650 2023-04-28 00:41:44.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/decorators.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.816627 zibanu-django-1.2.0b0/zibanu/django/rest_framework/exceptions/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      973 2022-12-20 02:49:47.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/exceptions/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2039 2023-04-27 15:30:28.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/exceptions/api_exception.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.816627 zibanu-django-1.2.0b0/zibanu/django/rest_framework/fields/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/fields/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1142 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/fields/current_user_default.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.816627 zibanu-django-1.2.0b0/zibanu/django/rest_framework/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1560 2022-12-20 10:51:58.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-02-27 20:11:57.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/serializers/fields.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      867 2022-12-14 09:18:30.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/serializers/model_serializer.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.817627 zibanu-django-1.2.0b0/zibanu/django/rest_framework/viewsets/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-02-13 14:05:54.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/viewsets/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    10487 2023-04-28 00:47:56.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/viewsets/model_viewset.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1332 2023-02-13 14:05:54.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/viewsets/viewset.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.817627 zibanu-django-1.2.0b0/zibanu/django/template/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-01-28 17:50:45.000000 zibanu-django-1.2.0b0/zibanu/django/template/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      663 2023-01-28 20:32:11.000000 zibanu-django-1.2.0b0/zibanu/django/template/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.818627 zibanu-django-1.2.0b0/zibanu/django/template/context_processors/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-01-29 02:00:01.000000 zibanu-django-1.2.0b0/zibanu/django/template/context_processors/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-01-29 02:00:01.000000 zibanu-django-1.2.0b0/zibanu/django/template/context_processors/full_static_uri.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2023-01-28 20:37:34.000000 zibanu-django-1.2.0b0/zibanu/django/template/context_processors/site.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.803628 zibanu-django-1.2.0b0/zibanu/django/template/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.803628 zibanu-django-1.2.0b0/zibanu/django/template/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.818627 zibanu-django-1.2.0b0/zibanu/django/template/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      519 2023-02-09 14:42:38.000000 zibanu-django-1.2.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1022 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.819627 zibanu-django-1.2.0b0/zibanu/django/template/templatetags/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-07 23:57:31.000000 zibanu-django-1.2.0b0/zibanu/django/template/templatetags/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1539 2023-01-29 02:38:53.000000 zibanu-django-1.2.0b0/zibanu/django/template/templatetags/static_uri.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      666 2023-02-08 00:00:29.000000 zibanu-django-1.2.0b0/zibanu/django/template/templatetags/string_concat.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2009 2023-02-16 14:53:50.000000 zibanu-django-1.2.0b0/zibanu/django/template/templatetags/subtotal_dict.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1216 2023-02-08 15:25:53.000000 zibanu-django-1.2.0b0/zibanu/django/template/templatetags/sum_dict.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.820627 zibanu-django-1.2.0b0/zibanu/django/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      863 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3332 2023-04-28 21:35:15.000000 zibanu-django-1.2.0b0/zibanu/django/utils/code_generator.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1895 2023-02-26 20:02:32.000000 zibanu-django-1.2.0b0/zibanu/django/utils/date_time.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1163 2023-03-03 13:27:43.000000 zibanu-django-1.2.0b0/zibanu/django/utils/error_messages.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     5768 2023-05-23 00:00:08.000000 zibanu-django-1.2.0b0/zibanu/django/utils/mail.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      562 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/utils/request_utils.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1080 2023-05-13 15:24:32.000000 zibanu-django-1.2.0b0/zibanu/django/utils/user.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      699 2023-03-03 13:27:43.000000 zibanu-django-1.2.0b0/zibanu/django/utils/validate_cache_code.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.821627 zibanu-django-1.2.0b0/zibanu_django.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41394 2023-06-19 16:44:21.000000 zibanu-django-1.2.0b0/zibanu_django.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     3506 2023-06-19 16:44:21.000000 zibanu-django-1.2.0b0/zibanu_django.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-06-19 16:44:21.000000 zibanu-django-1.2.0b0/zibanu_django.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       62 2023-06-19 16:44:21.000000 zibanu-django-1.2.0b0/zibanu_django.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-06-19 16:44:21.000000 zibanu-django-1.2.0b0/zibanu_django.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.539692 zibanu-django-1.2.0b1/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-1.2.0b1/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      208 2023-06-19 16:39:09.000000 zibanu-django-1.2.0b1/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41394 2023-06-19 16:46:45.539692 zibanu-django-1.2.0b1/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      179 2023-06-19 16:22:53.000000 zibanu-django-1.2.0b1/README.md
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      901 2023-06-19 16:46:30.000000 zibanu-django-1.2.0b1/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-06-19 16:46:45.539692 zibanu-django-1.2.0b1/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.525692 zibanu-django-1.2.0b1/zibanu/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      623 2022-12-10 15:21:05.000000 zibanu-django-1.2.0b1/zibanu/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.526692 zibanu-django-1.2.0b1/zibanu/django/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-11 23:08:20.000000 zibanu-django-1.2.0b1/zibanu/django/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      895 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.526692 zibanu-django-1.2.0b1/zibanu/django/db/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 18:13:01.000000 zibanu-django-1.2.0b1/zibanu/django/db/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.526692 zibanu-django-1.2.0b1/zibanu/django/db/backends/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0b1/zibanu/django/db/backends/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.527692 zibanu-django-1.2.0b1/zibanu/django/db/backends/oracle/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0b1/zibanu/django/db/backends/oracle/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1158 2023-02-07 01:58:51.000000 zibanu-django-1.2.0b1/zibanu/django/db/backends/oracle/base.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.528692 zibanu-django-1.2.0b1/zibanu/django/db/models/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      766 2023-01-17 11:51:34.000000 zibanu-django-1.2.0b1/zibanu/django/db/models/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      931 2023-03-01 18:58:00.000000 zibanu-django-1.2.0b1/zibanu/django/db/models/dated_model.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1458 2023-03-03 23:10:34.000000 zibanu-django-1.2.0b1/zibanu/django/db/models/manager.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      738 2022-12-20 14:58:49.000000 zibanu-django-1.2.0b1/zibanu/django/db/models/model.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.522692 zibanu-django-1.2.0b1/zibanu/django/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.522692 zibanu-django-1.2.0b1/zibanu/django/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.528692 zibanu-django-1.2.0b1/zibanu/django/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2274 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3598 2023-04-27 15:33:39.000000 zibanu-django-1.2.0b1/zibanu/django/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.529692 zibanu-django-1.2.0b1/zibanu/django/logging/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-03-16 14:08:34.000000 zibanu-django-1.2.0b1/zibanu/django/logging/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      919 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.529692 zibanu-django-1.2.0b1/zibanu/django/logging/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 20:39:57.000000 zibanu-django-1.2.0b1/zibanu/django/logging/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.530692 zibanu-django-1.2.0b1/zibanu/django/logging/lib/events/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/lib/events/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1016 2023-05-13 19:57:25.000000 zibanu-django-1.2.0b1/zibanu/django/logging/lib/events/on_change_password.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1243 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/lib/events/on_login.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      975 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/lib/events/on_send_mail.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.530692 zibanu-django-1.2.0b1/zibanu/django/logging/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:05:35.000000 zibanu-django-1.2.0b1/zibanu/django/logging/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      452 2023-05-13 17:50:17.000000 zibanu-django-1.2.0b1/zibanu/django/logging/lib/signals.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.523692 zibanu-django-1.2.0b1/zibanu/django/logging/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.523692 zibanu-django-1.2.0b1/zibanu/django/logging/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.530692 zibanu-django-1.2.0b1/zibanu/django/logging/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1185 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.531692 zibanu-django-1.2.0b1/zibanu/django/logging/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1501 2023-03-15 21:32:53.000000 zibanu-django-1.2.0b1/zibanu/django/logging/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1143 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/migrations/0002_maillog.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:33:26.000000 zibanu-django-1.2.0b1/zibanu/django/logging/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1946 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.531692 zibanu-django-1.2.0b1/zibanu/django/rest_framework/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 12:39:27.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1650 2023-04-28 00:41:44.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/decorators.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.532692 zibanu-django-1.2.0b1/zibanu/django/rest_framework/exceptions/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      973 2022-12-20 02:49:47.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/exceptions/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2039 2023-04-27 15:30:28.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/exceptions/api_exception.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.532692 zibanu-django-1.2.0b1/zibanu/django/rest_framework/fields/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/fields/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1142 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/fields/current_user_default.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.533692 zibanu-django-1.2.0b1/zibanu/django/rest_framework/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1560 2022-12-20 10:51:58.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-02-27 20:11:57.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/serializers/fields.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      867 2022-12-14 09:18:30.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/serializers/model_serializer.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.533692 zibanu-django-1.2.0b1/zibanu/django/rest_framework/viewsets/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-02-13 14:05:54.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/viewsets/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    10487 2023-04-28 00:47:56.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/viewsets/model_viewset.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1332 2023-02-13 14:05:54.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/viewsets/viewset.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.534692 zibanu-django-1.2.0b1/zibanu/django/template/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-01-28 17:50:45.000000 zibanu-django-1.2.0b1/zibanu/django/template/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      663 2023-01-28 20:32:11.000000 zibanu-django-1.2.0b1/zibanu/django/template/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.534692 zibanu-django-1.2.0b1/zibanu/django/template/context_processors/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-01-29 02:00:01.000000 zibanu-django-1.2.0b1/zibanu/django/template/context_processors/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-01-29 02:00:01.000000 zibanu-django-1.2.0b1/zibanu/django/template/context_processors/full_static_uri.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2023-01-28 20:37:34.000000 zibanu-django-1.2.0b1/zibanu/django/template/context_processors/site.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.524692 zibanu-django-1.2.0b1/zibanu/django/template/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.524692 zibanu-django-1.2.0b1/zibanu/django/template/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.535692 zibanu-django-1.2.0b1/zibanu/django/template/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      519 2023-02-09 14:42:38.000000 zibanu-django-1.2.0b1/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1022 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/template/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.536692 zibanu-django-1.2.0b1/zibanu/django/template/templatetags/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-07 23:57:31.000000 zibanu-django-1.2.0b1/zibanu/django/template/templatetags/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1539 2023-01-29 02:38:53.000000 zibanu-django-1.2.0b1/zibanu/django/template/templatetags/static_uri.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      666 2023-02-08 00:00:29.000000 zibanu-django-1.2.0b1/zibanu/django/template/templatetags/string_concat.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2009 2023-02-16 14:53:50.000000 zibanu-django-1.2.0b1/zibanu/django/template/templatetags/subtotal_dict.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1216 2023-02-08 15:25:53.000000 zibanu-django-1.2.0b1/zibanu/django/template/templatetags/sum_dict.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.537692 zibanu-django-1.2.0b1/zibanu/django/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      863 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3332 2023-04-28 21:35:15.000000 zibanu-django-1.2.0b1/zibanu/django/utils/code_generator.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1895 2023-02-26 20:02:32.000000 zibanu-django-1.2.0b1/zibanu/django/utils/date_time.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1163 2023-03-03 13:27:43.000000 zibanu-django-1.2.0b1/zibanu/django/utils/error_messages.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     5768 2023-05-23 00:00:08.000000 zibanu-django-1.2.0b1/zibanu/django/utils/mail.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      562 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/utils/request_utils.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1080 2023-05-13 15:24:32.000000 zibanu-django-1.2.0b1/zibanu/django/utils/user.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      699 2023-03-03 13:27:43.000000 zibanu-django-1.2.0b1/zibanu/django/utils/validate_cache_code.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.538692 zibanu-django-1.2.0b1/zibanu_django.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41394 2023-06-19 16:46:45.000000 zibanu-django-1.2.0b1/zibanu_django.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2836 2023-06-19 16:46:45.000000 zibanu-django-1.2.0b1/zibanu_django.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-06-19 16:46:45.000000 zibanu-django-1.2.0b1/zibanu_django.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       62 2023-06-19 16:46:45.000000 zibanu-django-1.2.0b1/zibanu_django.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-06-19 16:46:45.000000 zibanu-django-1.2.0b1/zibanu_django.egg-info/top_level.txt
```

### Comparing `zibanu-django-1.2.0b0/LICENSE` & `zibanu-django-1.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/PKG-INFO` & `zibanu-django-1.2.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.2.0b0
+Version: 1.2.0b1
 Summary: Zibanu authentication library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-1.2.0b0/pyproject.toml` & `zibanu-django-1.2.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "zibanu-django"
-version = "1.2.0-beta.0"
+version = "1.2.0-beta.1"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
 description = "Zibanu authentication library for django projects"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
```

### Comparing `zibanu-django-1.2.0b0/zibanu/__init__.py` & `zibanu-django-1.2.0b1/zibanu/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/apps.py` & `zibanu-django-1.2.0b1/zibanu/django/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/db/backends/oracle/base.py` & `zibanu-django-1.2.0b1/zibanu/django/db/backends/oracle/base.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/db/models/__init__.py` & `zibanu-django-1.2.0b1/zibanu/django/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/db/models/dated_model.py` & `zibanu-django-1.2.0b1/zibanu/django/db/models/dated_model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/db/models/manager.py` & `zibanu-django-1.2.0b1/zibanu/django/db/models/manager.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/db/models/model.py` & `zibanu-django-1.2.0b1/zibanu/django/db/models/model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0b1/zibanu/django/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0b1/zibanu/django/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/logging/apps.py` & `zibanu-django-1.2.0b1/zibanu/django/logging/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/__init__.py` & `zibanu-django-1.2.0b1/zibanu/django/logging/lib/events/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/on_change_password.py` & `zibanu-django-1.2.0b1/zibanu/django/logging/lib/events/on_change_password.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/on_login.py` & `zibanu-django-1.2.0b1/zibanu/django/logging/lib/events/on_login.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/on_send_mail.py` & `zibanu-django-1.2.0b1/zibanu/django/logging/lib/events/on_send_mail.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0b1/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/logging/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0b1/zibanu/django/logging/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/logging/migrations/0001_initial.py` & `zibanu-django-1.2.0b1/zibanu/django/logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/logging/migrations/0002_maillog.py` & `zibanu-django-1.2.0b1/zibanu/django/logging/migrations/0002_maillog.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/logging/models.py` & `zibanu-django-1.2.0b1/zibanu/django/logging/models.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/repository/lib/managers/__init__.py` & `zibanu-django-1.2.0b1/zibanu/django/template/templatetags/string_concat.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 
 #  Developed by CQ Inversiones SAS. Copyright ©. 2019 - 2023. All rights reserved.
 #  Desarrollado por CQ Inversiones SAS. Copyright ©. 2019 - 2023. Todos los derechos reservado
 
 # ****************************************************************
 # IDE:          PyCharm
 # Developed by: macercha
-# Date:         4/02/23 15:45
+# Date:         7/02/23 18:56
 # Project:      CFHL Transactional Backend
-# Module Name:  __init__.py
+# Module Name:  string_concat
 # Description:
 # ****************************************************************
-from .document import Document
+from django import template
+
+register = template.Library()
+
+
+@register.simple_tag
+def string_concat(first_string: str, *args):
+    return first_string % args
 
-__all__ = [
-    "Document"
-]
```

### Comparing `zibanu-django-1.2.0b0/zibanu/django/rest_framework/decorators.py` & `zibanu-django-1.2.0b1/zibanu/django/rest_framework/decorators.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/rest_framework/exceptions/__init__.py` & `zibanu-django-1.2.0b1/zibanu/django/rest_framework/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/rest_framework/exceptions/api_exception.py` & `zibanu-django-1.2.0b1/zibanu/django/rest_framework/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/rest_framework/fields/__init__.py` & `zibanu-django-1.2.0b1/zibanu/django/rest_framework/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/rest_framework/fields/current_user_default.py` & `zibanu-django-1.2.0b1/zibanu/django/rest_framework/fields/current_user_default.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/rest_framework/serializers/__init__.py` & `zibanu-django-1.2.0b1/zibanu/django/rest_framework/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/rest_framework/serializers/fields.py` & `zibanu-django-1.2.0b1/zibanu/django/rest_framework/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/rest_framework/serializers/model_serializer.py` & `zibanu-django-1.2.0b1/zibanu/django/rest_framework/serializers/model_serializer.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/rest_framework/viewsets/__init__.py` & `zibanu-django-1.2.0b1/zibanu/django/rest_framework/viewsets/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/rest_framework/viewsets/model_viewset.py` & `zibanu-django-1.2.0b1/zibanu/django/rest_framework/viewsets/model_viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/rest_framework/viewsets/viewset.py` & `zibanu-django-1.2.0b1/zibanu/django/rest_framework/viewsets/viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/template/apps.py` & `zibanu-django-1.2.0b1/zibanu/django/template/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/template/context_processors/__init__.py` & `zibanu-django-1.2.0b1/zibanu/django/template/context_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/template/context_processors/full_static_uri.py` & `zibanu-django-1.2.0b1/zibanu/django/template/context_processors/full_static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/template/context_processors/site.py` & `zibanu-django-1.2.0b1/zibanu/django/template/context_processors/site.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0b1/zibanu/django/template/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0b1/zibanu/django/template/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/template/templatetags/static_uri.py` & `zibanu-django-1.2.0b1/zibanu/django/template/templatetags/static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/template/templatetags/subtotal_dict.py` & `zibanu-django-1.2.0b1/zibanu/django/template/templatetags/subtotal_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/template/templatetags/sum_dict.py` & `zibanu-django-1.2.0b1/zibanu/django/template/templatetags/sum_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/utils/__init__.py` & `zibanu-django-1.2.0b1/zibanu/django/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/utils/code_generator.py` & `zibanu-django-1.2.0b1/zibanu/django/utils/code_generator.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/utils/date_time.py` & `zibanu-django-1.2.0b1/zibanu/django/utils/date_time.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/utils/error_messages.py` & `zibanu-django-1.2.0b1/zibanu/django/utils/error_messages.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/utils/mail.py` & `zibanu-django-1.2.0b1/zibanu/django/utils/mail.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/utils/request_utils.py` & `zibanu-django-1.2.0b1/zibanu/django/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/utils/user.py` & `zibanu-django-1.2.0b1/zibanu/django/utils/user.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu/django/utils/validate_cache_code.py` & `zibanu-django-1.2.0b1/zibanu/django/utils/validate_cache_code.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b0/zibanu_django.egg-info/PKG-INFO` & `zibanu-django-1.2.0b1/zibanu_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.2.0b0
+Version: 1.2.0b1
 Summary: Zibanu authentication library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

