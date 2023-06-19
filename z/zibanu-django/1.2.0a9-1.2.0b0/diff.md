# Comparing `tmp/zibanu-django-1.2.0a9.tar.gz` & `tmp/zibanu-django-1.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zibanu-django-1.2.0a9.tar", last modified: Tue May 23 17:00:43 2023, max compression
+gzip compressed data, was "zibanu-django-1.2.0b0.tar", last modified: Mon Jun 19 16:44:21 2023, max compression
```

## Comparing `zibanu-django-1.2.0a9.tar` & `zibanu-django-1.2.0b0.tar`

### file list

```diff
@@ -1,163 +1,125 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.593315 zibanu-django-1.2.0a9/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-1.2.0a9/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      304 2023-05-13 16:38:59.000000 zibanu-django-1.2.0a9/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41365 2023-05-23 17:00:43.593315 zibanu-django-1.2.0a9/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      158 2023-01-18 12:15:22.000000 zibanu-django-1.2.0a9/README.md
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      886 2023-05-23 16:56:32.000000 zibanu-django-1.2.0a9/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-05-23 17:00:43.593315 zibanu-django-1.2.0a9/setup.cfg
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.572315 zibanu-django-1.2.0a9/zibanu/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      623 2022-12-10 15:21:05.000000 zibanu-django-1.2.0a9/zibanu/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.573315 zibanu-django-1.2.0a9/zibanu/django/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-11 23:08:20.000000 zibanu-django-1.2.0a9/zibanu/django/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      895 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a9/zibanu/django/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.573315 zibanu-django-1.2.0a9/zibanu/django/auth/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:20:31.000000 zibanu-django-1.2.0a9/zibanu/django/auth/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.573315 zibanu-django-1.2.0a9/zibanu/django/auth/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:25:30.000000 zibanu-django-1.2.0a9/zibanu/django/auth/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.574315 zibanu-django-1.2.0a9/zibanu/django/auth/api/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      648 2023-04-27 14:40:31.000000 zibanu-django-1.2.0a9/zibanu/django/auth/api/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      749 2023-04-27 12:00:18.000000 zibanu-django-1.2.0a9/zibanu/django/auth/api/serializers/profile.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3051 2023-04-27 12:17:39.000000 zibanu-django-1.2.0a9/zibanu/django/auth/api/serializers/token.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3944 2023-05-13 14:19:35.000000 zibanu-django-1.2.0a9/zibanu/django/auth/api/serializers/user.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.574315 zibanu-django-1.2.0a9/zibanu/django/auth/api/services/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      376 2023-04-27 14:42:35.000000 zibanu-django-1.2.0a9/zibanu/django/auth/api/services/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     8259 2023-05-23 16:17:03.000000 zibanu-django-1.2.0a9/zibanu/django/auth/api/services/user.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1245 2023-05-17 01:05:01.000000 zibanu-django-1.2.0a9/zibanu/django/auth/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.575315 zibanu-django-1.2.0a9/zibanu/django/auth/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:32:01.000000 zibanu-django-1.2.0a9/zibanu/django/auth/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.575315 zibanu-django-1.2.0a9/zibanu/django/auth/lib/choices/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:48:01.000000 zibanu-django-1.2.0a9/zibanu/django/auth/lib/choices/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1396 2023-05-17 00:58:35.000000 zibanu-django-1.2.0a9/zibanu/django/auth/lib/signal_events.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      412 2023-05-13 17:53:49.000000 zibanu-django-1.2.0a9/zibanu/django/auth/lib/signals.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1086 2023-05-13 15:23:33.000000 zibanu-django-1.2.0a9/zibanu/django/auth/lib/utils.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.566315 zibanu-django-1.2.0a9/zibanu/django/auth/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.566315 zibanu-django-1.2.0a9/zibanu/django/auth/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.575315 zibanu-django-1.2.0a9/zibanu/django/auth/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      818 2023-04-27 15:20:42.000000 zibanu-django-1.2.0a9/zibanu/django/auth/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1166 2023-04-27 15:20:12.000000 zibanu-django-1.2.0a9/zibanu/django/auth/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.576315 zibanu-django-1.2.0a9/zibanu/django/auth/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    24474 2023-04-11 22:39:55.000000 zibanu-django-1.2.0a9/zibanu/django/auth/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    23375 2023-04-27 14:50:20.000000 zibanu-django-1.2.0a9/zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:31:28.000000 zibanu-django-1.2.0a9/zibanu/django/auth/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1605 2023-04-11 22:39:53.000000 zibanu-django-1.2.0a9/zibanu/django/auth/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.577315 zibanu-django-1.2.0a9/zibanu/django/auth/templates/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      487 2023-05-23 16:11:28.000000 zibanu-django-1.2.0a9/zibanu/django/auth/templates/change_password.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      324 2023-05-22 17:32:26.000000 zibanu-django-1.2.0a9/zibanu/django/auth/templates/change_password.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-05-13 16:44:16.000000 zibanu-django-1.2.0a9/zibanu/django/auth/templates/request-code.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-05-13 16:41:48.000000 zibanu-django-1.2.0a9/zibanu/django/auth/templates/request-code.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      559 2023-05-22 17:30:07.000000 zibanu-django-1.2.0a9/zibanu/django/auth/templates/request_password.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      346 2023-05-13 16:55:01.000000 zibanu-django-1.2.0a9/zibanu/django/auth/templates/request_password.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1067 2023-05-23 00:53:34.000000 zibanu-django-1.2.0a9/zibanu/django/auth/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.580315 zibanu-django-1.2.0a9/zibanu/django/db/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 18:13:01.000000 zibanu-django-1.2.0a9/zibanu/django/db/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.580315 zibanu-django-1.2.0a9/zibanu/django/db/backends/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0a9/zibanu/django/db/backends/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.580315 zibanu-django-1.2.0a9/zibanu/django/db/backends/oracle/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0a9/zibanu/django/db/backends/oracle/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1158 2023-02-07 01:58:51.000000 zibanu-django-1.2.0a9/zibanu/django/db/backends/oracle/base.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.581315 zibanu-django-1.2.0a9/zibanu/django/db/models/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      766 2023-01-17 11:51:34.000000 zibanu-django-1.2.0a9/zibanu/django/db/models/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      931 2023-03-01 18:58:00.000000 zibanu-django-1.2.0a9/zibanu/django/db/models/dated_model.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1458 2023-03-03 23:10:34.000000 zibanu-django-1.2.0a9/zibanu/django/db/models/manager.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      738 2022-12-20 14:58:49.000000 zibanu-django-1.2.0a9/zibanu/django/db/models/model.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.567315 zibanu-django-1.2.0a9/zibanu/django/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.567315 zibanu-django-1.2.0a9/zibanu/django/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.582315 zibanu-django-1.2.0a9/zibanu/django/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2274 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a9/zibanu/django/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3598 2023-04-27 15:33:39.000000 zibanu-django-1.2.0a9/zibanu/django/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.582315 zibanu-django-1.2.0a9/zibanu/django/logging/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-03-16 14:08:34.000000 zibanu-django-1.2.0a9/zibanu/django/logging/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      919 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a9/zibanu/django/logging/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.582315 zibanu-django-1.2.0a9/zibanu/django/logging/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 20:39:57.000000 zibanu-django-1.2.0a9/zibanu/django/logging/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.583315 zibanu-django-1.2.0a9/zibanu/django/logging/lib/events/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a9/zibanu/django/logging/lib/events/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1016 2023-05-13 19:57:25.000000 zibanu-django-1.2.0a9/zibanu/django/logging/lib/events/on_change_password.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1243 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a9/zibanu/django/logging/lib/events/on_login.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      975 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a9/zibanu/django/logging/lib/events/on_send_mail.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.583315 zibanu-django-1.2.0a9/zibanu/django/logging/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:05:35.000000 zibanu-django-1.2.0a9/zibanu/django/logging/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      452 2023-05-13 17:50:17.000000 zibanu-django-1.2.0a9/zibanu/django/logging/lib/signals.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.568315 zibanu-django-1.2.0a9/zibanu/django/logging/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.568315 zibanu-django-1.2.0a9/zibanu/django/logging/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.584315 zibanu-django-1.2.0a9/zibanu/django/logging/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a9/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1185 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a9/zibanu/django/logging/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.584315 zibanu-django-1.2.0a9/zibanu/django/logging/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1501 2023-03-15 21:32:53.000000 zibanu-django-1.2.0a9/zibanu/django/logging/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1143 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a9/zibanu/django/logging/migrations/0002_maillog.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:33:26.000000 zibanu-django-1.2.0a9/zibanu/django/logging/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1946 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a9/zibanu/django/logging/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.585315 zibanu-django-1.2.0a9/zibanu/django/repository/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-03 02:16:47.000000 zibanu-django-1.2.0a9/zibanu/django/repository/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.585315 zibanu-django-1.2.0a9/zibanu/django/repository/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:42:37.000000 zibanu-django-1.2.0a9/zibanu/django/repository/api/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      958 2023-02-03 02:43:10.000000 zibanu-django-1.2.0a9/zibanu/django/repository/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.585315 zibanu-django-1.2.0a9/zibanu/django/repository/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:45:36.000000 zibanu-django-1.2.0a9/zibanu/django/repository/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.586315 zibanu-django-1.2.0a9/zibanu/django/repository/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      566 2023-02-04 20:47:18.000000 zibanu-django-1.2.0a9/zibanu/django/repository/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      740 2023-02-04 21:36:16.000000 zibanu-django-1.2.0a9/zibanu/django/repository/lib/managers/document.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.586315 zibanu-django-1.2.0a9/zibanu/django/repository/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      593 2023-02-04 20:45:36.000000 zibanu-django-1.2.0a9/zibanu/django/repository/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     6973 2023-04-11 22:50:39.000000 zibanu-django-1.2.0a9/zibanu/django/repository/lib/utils/document_generator.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.569315 zibanu-django-1.2.0a9/zibanu/django/repository/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.569315 zibanu-django-1.2.0a9/zibanu/django/repository/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.587315 zibanu-django-1.2.0a9/zibanu/django/repository/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1605 2023-02-09 14:40:51.000000 zibanu-django-1.2.0a9/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2664 2023-04-11 22:52:31.000000 zibanu-django-1.2.0a9/zibanu/django/repository/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.587315 zibanu-django-1.2.0a9/zibanu/django/repository/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1372 2023-02-03 02:43:34.000000 zibanu-django-1.2.0a9/zibanu/django/repository/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      427 2023-02-08 14:23:11.000000 zibanu-django-1.2.0a9/zibanu/django/repository/migrations/0002_document_description.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-02-03 02:23:41.000000 zibanu-django-1.2.0a9/zibanu/django/repository/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1575 2023-02-08 14:23:06.000000 zibanu-django-1.2.0a9/zibanu/django/repository/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.587315 zibanu-django-1.2.0a9/zibanu/django/rest_framework/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 12:39:27.000000 zibanu-django-1.2.0a9/zibanu/django/rest_framework/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1650 2023-04-28 00:41:44.000000 zibanu-django-1.2.0a9/zibanu/django/rest_framework/decorators.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.588315 zibanu-django-1.2.0a9/zibanu/django/rest_framework/exceptions/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      973 2022-12-20 02:49:47.000000 zibanu-django-1.2.0a9/zibanu/django/rest_framework/exceptions/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2039 2023-04-27 15:30:28.000000 zibanu-django-1.2.0a9/zibanu/django/rest_framework/exceptions/api_exception.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.588315 zibanu-django-1.2.0a9/zibanu/django/rest_framework/fields/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a9/zibanu/django/rest_framework/fields/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1142 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a9/zibanu/django/rest_framework/fields/current_user_default.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.589315 zibanu-django-1.2.0a9/zibanu/django/rest_framework/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1560 2022-12-20 10:51:58.000000 zibanu-django-1.2.0a9/zibanu/django/rest_framework/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-02-27 20:11:57.000000 zibanu-django-1.2.0a9/zibanu/django/rest_framework/serializers/fields.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      867 2022-12-14 09:18:30.000000 zibanu-django-1.2.0a9/zibanu/django/rest_framework/serializers/model_serializer.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.589315 zibanu-django-1.2.0a9/zibanu/django/rest_framework/viewsets/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-02-13 14:05:54.000000 zibanu-django-1.2.0a9/zibanu/django/rest_framework/viewsets/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    10487 2023-04-28 00:47:56.000000 zibanu-django-1.2.0a9/zibanu/django/rest_framework/viewsets/model_viewset.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1332 2023-02-13 14:05:54.000000 zibanu-django-1.2.0a9/zibanu/django/rest_framework/viewsets/viewset.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.589315 zibanu-django-1.2.0a9/zibanu/django/template/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-01-28 17:50:45.000000 zibanu-django-1.2.0a9/zibanu/django/template/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      663 2023-01-28 20:32:11.000000 zibanu-django-1.2.0a9/zibanu/django/template/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.590314 zibanu-django-1.2.0a9/zibanu/django/template/context_processors/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-01-29 02:00:01.000000 zibanu-django-1.2.0a9/zibanu/django/template/context_processors/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-01-29 02:00:01.000000 zibanu-django-1.2.0a9/zibanu/django/template/context_processors/full_static_uri.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2023-01-28 20:37:34.000000 zibanu-django-1.2.0a9/zibanu/django/template/context_processors/site.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.570315 zibanu-django-1.2.0a9/zibanu/django/template/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.571315 zibanu-django-1.2.0a9/zibanu/django/template/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.590314 zibanu-django-1.2.0a9/zibanu/django/template/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      519 2023-02-09 14:42:38.000000 zibanu-django-1.2.0a9/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1022 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a9/zibanu/django/template/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.591315 zibanu-django-1.2.0a9/zibanu/django/template/templatetags/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-07 23:57:31.000000 zibanu-django-1.2.0a9/zibanu/django/template/templatetags/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1539 2023-01-29 02:38:53.000000 zibanu-django-1.2.0a9/zibanu/django/template/templatetags/static_uri.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      666 2023-02-08 00:00:29.000000 zibanu-django-1.2.0a9/zibanu/django/template/templatetags/string_concat.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2009 2023-02-16 14:53:50.000000 zibanu-django-1.2.0a9/zibanu/django/template/templatetags/subtotal_dict.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1216 2023-02-08 15:25:53.000000 zibanu-django-1.2.0a9/zibanu/django/template/templatetags/sum_dict.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.592315 zibanu-django-1.2.0a9/zibanu/django/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      863 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a9/zibanu/django/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3332 2023-04-28 21:35:15.000000 zibanu-django-1.2.0a9/zibanu/django/utils/code_generator.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1895 2023-02-26 20:02:32.000000 zibanu-django-1.2.0a9/zibanu/django/utils/date_time.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1163 2023-03-03 13:27:43.000000 zibanu-django-1.2.0a9/zibanu/django/utils/error_messages.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     5768 2023-05-23 00:00:08.000000 zibanu-django-1.2.0a9/zibanu/django/utils/mail.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      562 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a9/zibanu/django/utils/request_utils.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1080 2023-05-13 15:24:32.000000 zibanu-django-1.2.0a9/zibanu/django/utils/user.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      699 2023-03-03 13:27:43.000000 zibanu-django-1.2.0a9/zibanu/django/utils/validate_cache_code.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 17:00:43.593315 zibanu-django-1.2.0a9/zibanu_django.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41365 2023-05-23 17:00:43.000000 zibanu-django-1.2.0a9/zibanu_django.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     4651 2023-05-23 17:00:43.000000 zibanu-django-1.2.0a9/zibanu_django.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-05-23 17:00:43.000000 zibanu-django-1.2.0a9/zibanu_django.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       62 2023-05-23 17:00:43.000000 zibanu-django-1.2.0a9/zibanu_django.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-05-23 17:00:43.000000 zibanu-django-1.2.0a9/zibanu_django.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.821627 zibanu-django-1.2.0b0/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-1.2.0b0/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      208 2023-06-19 16:39:09.000000 zibanu-django-1.2.0b0/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41394 2023-06-19 16:44:21.821627 zibanu-django-1.2.0b0/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      179 2023-06-19 16:22:53.000000 zibanu-django-1.2.0b0/README.md
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      901 2023-06-19 16:40:16.000000 zibanu-django-1.2.0b0/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-06-19 16:44:21.821627 zibanu-django-1.2.0b0/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.804628 zibanu-django-1.2.0b0/zibanu/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      623 2022-12-10 15:21:05.000000 zibanu-django-1.2.0b0/zibanu/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.804628 zibanu-django-1.2.0b0/zibanu/django/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-11 23:08:20.000000 zibanu-django-1.2.0b0/zibanu/django/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      895 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.805628 zibanu-django-1.2.0b0/zibanu/django/db/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 18:13:01.000000 zibanu-django-1.2.0b0/zibanu/django/db/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.805628 zibanu-django-1.2.0b0/zibanu/django/db/backends/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0b0/zibanu/django/db/backends/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.805628 zibanu-django-1.2.0b0/zibanu/django/db/backends/oracle/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0b0/zibanu/django/db/backends/oracle/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1158 2023-02-07 01:58:51.000000 zibanu-django-1.2.0b0/zibanu/django/db/backends/oracle/base.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.806628 zibanu-django-1.2.0b0/zibanu/django/db/models/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      766 2023-01-17 11:51:34.000000 zibanu-django-1.2.0b0/zibanu/django/db/models/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      931 2023-03-01 18:58:00.000000 zibanu-django-1.2.0b0/zibanu/django/db/models/dated_model.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1458 2023-03-03 23:10:34.000000 zibanu-django-1.2.0b0/zibanu/django/db/models/manager.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      738 2022-12-20 14:58:49.000000 zibanu-django-1.2.0b0/zibanu/django/db/models/model.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.800628 zibanu-django-1.2.0b0/zibanu/django/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.800628 zibanu-django-1.2.0b0/zibanu/django/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.806628 zibanu-django-1.2.0b0/zibanu/django/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2274 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3598 2023-04-27 15:33:39.000000 zibanu-django-1.2.0b0/zibanu/django/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.807628 zibanu-django-1.2.0b0/zibanu/django/logging/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-03-16 14:08:34.000000 zibanu-django-1.2.0b0/zibanu/django/logging/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      919 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.807628 zibanu-django-1.2.0b0/zibanu/django/logging/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 20:39:57.000000 zibanu-django-1.2.0b0/zibanu/django/logging/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.808627 zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1016 2023-05-13 19:57:25.000000 zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/on_change_password.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1243 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/on_login.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      975 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/on_send_mail.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.808627 zibanu-django-1.2.0b0/zibanu/django/logging/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:05:35.000000 zibanu-django-1.2.0b0/zibanu/django/logging/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      452 2023-05-13 17:50:17.000000 zibanu-django-1.2.0b0/zibanu/django/logging/lib/signals.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.801628 zibanu-django-1.2.0b0/zibanu/django/logging/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.801628 zibanu-django-1.2.0b0/zibanu/django/logging/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.809628 zibanu-django-1.2.0b0/zibanu/django/logging/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1185 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.809628 zibanu-django-1.2.0b0/zibanu/django/logging/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1501 2023-03-15 21:32:53.000000 zibanu-django-1.2.0b0/zibanu/django/logging/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1143 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/migrations/0002_maillog.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:33:26.000000 zibanu-django-1.2.0b0/zibanu/django/logging/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1946 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/logging/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.810628 zibanu-django-1.2.0b0/zibanu/django/repository/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-03 02:16:47.000000 zibanu-django-1.2.0b0/zibanu/django/repository/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.810628 zibanu-django-1.2.0b0/zibanu/django/repository/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:42:37.000000 zibanu-django-1.2.0b0/zibanu/django/repository/api/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      958 2023-02-03 02:43:10.000000 zibanu-django-1.2.0b0/zibanu/django/repository/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.810628 zibanu-django-1.2.0b0/zibanu/django/repository/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:45:36.000000 zibanu-django-1.2.0b0/zibanu/django/repository/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.811627 zibanu-django-1.2.0b0/zibanu/django/repository/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      566 2023-02-04 20:47:18.000000 zibanu-django-1.2.0b0/zibanu/django/repository/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      740 2023-02-04 21:36:16.000000 zibanu-django-1.2.0b0/zibanu/django/repository/lib/managers/document.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.814628 zibanu-django-1.2.0b0/zibanu/django/repository/lib/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      593 2023-02-04 20:45:36.000000 zibanu-django-1.2.0b0/zibanu/django/repository/lib/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     7366 2023-06-03 20:53:46.000000 zibanu-django-1.2.0b0/zibanu/django/repository/lib/utils/document_generator.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.802628 zibanu-django-1.2.0b0/zibanu/django/repository/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.802628 zibanu-django-1.2.0b0/zibanu/django/repository/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.814628 zibanu-django-1.2.0b0/zibanu/django/repository/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1605 2023-02-09 14:40:51.000000 zibanu-django-1.2.0b0/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2664 2023-04-11 22:52:31.000000 zibanu-django-1.2.0b0/zibanu/django/repository/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.815627 zibanu-django-1.2.0b0/zibanu/django/repository/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1372 2023-02-03 02:43:34.000000 zibanu-django-1.2.0b0/zibanu/django/repository/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      427 2023-02-08 14:23:11.000000 zibanu-django-1.2.0b0/zibanu/django/repository/migrations/0002_document_description.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-02-03 02:23:41.000000 zibanu-django-1.2.0b0/zibanu/django/repository/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1575 2023-02-08 14:23:06.000000 zibanu-django-1.2.0b0/zibanu/django/repository/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.815627 zibanu-django-1.2.0b0/zibanu/django/rest_framework/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 12:39:27.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1650 2023-04-28 00:41:44.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/decorators.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.816627 zibanu-django-1.2.0b0/zibanu/django/rest_framework/exceptions/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      973 2022-12-20 02:49:47.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/exceptions/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2039 2023-04-27 15:30:28.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/exceptions/api_exception.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.816627 zibanu-django-1.2.0b0/zibanu/django/rest_framework/fields/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/fields/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1142 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/fields/current_user_default.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.816627 zibanu-django-1.2.0b0/zibanu/django/rest_framework/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1560 2022-12-20 10:51:58.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-02-27 20:11:57.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/serializers/fields.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      867 2022-12-14 09:18:30.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/serializers/model_serializer.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.817627 zibanu-django-1.2.0b0/zibanu/django/rest_framework/viewsets/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-02-13 14:05:54.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/viewsets/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    10487 2023-04-28 00:47:56.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/viewsets/model_viewset.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1332 2023-02-13 14:05:54.000000 zibanu-django-1.2.0b0/zibanu/django/rest_framework/viewsets/viewset.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.817627 zibanu-django-1.2.0b0/zibanu/django/template/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-01-28 17:50:45.000000 zibanu-django-1.2.0b0/zibanu/django/template/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      663 2023-01-28 20:32:11.000000 zibanu-django-1.2.0b0/zibanu/django/template/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.818627 zibanu-django-1.2.0b0/zibanu/django/template/context_processors/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-01-29 02:00:01.000000 zibanu-django-1.2.0b0/zibanu/django/template/context_processors/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-01-29 02:00:01.000000 zibanu-django-1.2.0b0/zibanu/django/template/context_processors/full_static_uri.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2023-01-28 20:37:34.000000 zibanu-django-1.2.0b0/zibanu/django/template/context_processors/site.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.803628 zibanu-django-1.2.0b0/zibanu/django/template/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.803628 zibanu-django-1.2.0b0/zibanu/django/template/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.818627 zibanu-django-1.2.0b0/zibanu/django/template/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      519 2023-02-09 14:42:38.000000 zibanu-django-1.2.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1022 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.819627 zibanu-django-1.2.0b0/zibanu/django/template/templatetags/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-07 23:57:31.000000 zibanu-django-1.2.0b0/zibanu/django/template/templatetags/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1539 2023-01-29 02:38:53.000000 zibanu-django-1.2.0b0/zibanu/django/template/templatetags/static_uri.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      666 2023-02-08 00:00:29.000000 zibanu-django-1.2.0b0/zibanu/django/template/templatetags/string_concat.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2009 2023-02-16 14:53:50.000000 zibanu-django-1.2.0b0/zibanu/django/template/templatetags/subtotal_dict.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1216 2023-02-08 15:25:53.000000 zibanu-django-1.2.0b0/zibanu/django/template/templatetags/sum_dict.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.820627 zibanu-django-1.2.0b0/zibanu/django/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      863 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3332 2023-04-28 21:35:15.000000 zibanu-django-1.2.0b0/zibanu/django/utils/code_generator.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1895 2023-02-26 20:02:32.000000 zibanu-django-1.2.0b0/zibanu/django/utils/date_time.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1163 2023-03-03 13:27:43.000000 zibanu-django-1.2.0b0/zibanu/django/utils/error_messages.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     5768 2023-05-23 00:00:08.000000 zibanu-django-1.2.0b0/zibanu/django/utils/mail.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      562 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b0/zibanu/django/utils/request_utils.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1080 2023-05-13 15:24:32.000000 zibanu-django-1.2.0b0/zibanu/django/utils/user.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      699 2023-03-03 13:27:43.000000 zibanu-django-1.2.0b0/zibanu/django/utils/validate_cache_code.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:44:21.821627 zibanu-django-1.2.0b0/zibanu_django.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41394 2023-06-19 16:44:21.000000 zibanu-django-1.2.0b0/zibanu_django.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     3506 2023-06-19 16:44:21.000000 zibanu-django-1.2.0b0/zibanu_django.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-06-19 16:44:21.000000 zibanu-django-1.2.0b0/zibanu_django.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       62 2023-06-19 16:44:21.000000 zibanu-django-1.2.0b0/zibanu_django.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-06-19 16:44:21.000000 zibanu-django-1.2.0b0/zibanu_django.egg-info/top_level.txt
```

### Comparing `zibanu-django-1.2.0a9/LICENSE` & `zibanu-django-1.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/PKG-INFO` & `zibanu-django-1.2.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.2.0a9
-Summary: Zibanu library for django projects
+Version: 1.2.0b0
+Summary: Zibanu authentication library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -673,27 +673,27 @@
         
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
-Keywords: django,zibanu,library
+Keywords: django,zibanu,library,auth
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Zibanu Django 
+# Zibanu Django Authentication Module
 
 This package or library contains some functionalities commonly used in django projects and django rest_framework projects. 
 
 ## Django db
```

### Comparing `zibanu-django-1.2.0a9/pyproject.toml` & `zibanu-django-1.2.0b0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,35 +3,36 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "zibanu-django"
-version = "1.2.0-alpha.9"
+version = "1.2.0-beta.0"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
-description = "Zibanu library for django projects"
+description = "Zibanu authentication library for django projects"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3.9",
-    "Development Status :: 5 - Production/Stable",
+    "Development Status :: 3 - Alpha",
     "Framework :: Django",
     "Framework :: Django :: 4.1",
     "Environment :: Web Environment",
     "Operating System :: OS Independent",
     "Topic :: Internet :: WWW/HTTP"
 ]
 dependencies = [
     "Django>=4.1",
     "djangorestframework",
-    "djangorestframework-simplejwt"
+    "djangorestframework-simplejwt",
 ]
 keywords = [
     "django",
     "zibanu",
-    "library"
+    "library",
+    "auth"
 ]
```

### Comparing `zibanu-django-1.2.0a9/zibanu/__init__.py` & `zibanu-django-1.2.0b0/zibanu/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/apps.py` & `zibanu-django-1.2.0b0/zibanu/django/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/auth/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0b0/zibanu/django/logging/locale/es/LC_MESSAGES/django.po`

 * *Files 27% similar despite different names*

```diff
@@ -4,47 +4,59 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-27 10:18-0500\n"
+"POT-Creation-Date: 2023-03-17 14:58-0500\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: apps.py:20
-msgid "Zibanu Auth for Django"
-msgstr "Autenticación Zibanu Django"
+#: apps.py:22
+msgid "Zibanu Logging"
+msgstr ""
+
+#: models.py:20
+msgid "Action"
+msgstr "Acción"
+
+#: models.py:21
+msgid "Sender object method"
+msgstr "Método que envía"
 
 #: models.py:22
-msgid "Time Zone"
-msgstr "Zona Horaria"
+msgid "IP Address"
+msgstr ""
 
 #: models.py:23
-msgid "User Theme"
-msgstr "Tema de Usuario"
+msgid "User"
+msgstr "Usuario"
+
+#: models.py:33
+msgid "Log"
+msgstr ""
 
-#: models.py:24
-msgid "Language"
-msgstr "Lenguaje"
-
-#: models.py:25
-msgid "Avatar"
-msgstr "Avatar"
-
-#: models.py:26
-msgid "Message's Timeout"
-msgstr "Tiempo de espera de mensajes"
-
-#: models.py:27
-msgid "Keep Logged In"
-msgstr "Mantener sesión abierta"
-
-#: models.py:28
-msgid "Custom Application Profile"
-msgstr "Perfil de aplicación"
+#: models.py:34
+msgid "Mail From"
+msgstr "De"
+
+#: models.py:35
+msgid "Mail To"
+msgstr "Para"
+
+#: models.py:36
+msgid "Subject"
+msgstr "Asunto"
+
+#: models.py:37
+msgid "SMTP Code"
+msgstr "Código SMTP"
+
+#: models.py:38
+msgid "SMTP Error"
+msgstr "Error SMTP"
```

### Comparing `zibanu-django-1.2.0a9/zibanu/django/auth/models.py` & `zibanu-django-1.2.0b0/zibanu/django/logging/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 # -*- coding: utf-8 -*-
 
+#  Developed by CQ Inversiones SAS. Copyright ©. 2019 - 2022. All rights reserved.
+#  Desarrollado por CQ Inversiones SAS. Copyright ©. 2019 - 2022. Todos los derechos reservado
+
 # ****************************************************************
 # IDE:          PyCharm
 # Developed by: macercha
-# Date:         10/04/23 13:52
-# Project:      Django Plugins
+# Date:         10/12/22 10:27 AM
+# Project:      CFHL Transactional Backend
 # Module Name:  models
 # Description:
 # ****************************************************************
-import zoneinfo
 from django.contrib.auth import get_user_model
 from django.utils.translation import gettext_lazy as _
 from zibanu.django.db import models
 
 
-class UserProfile(models.Model):
-    user = models.OneToOneField(get_user_model(), on_delete=models.CASCADE, related_name="profile",
-                                related_query_name="user")
-    timezone = models.CharField(max_length=50, null=False, blank=False, default="UTC",
-                                choices=tuple(zip(zoneinfo.available_timezones(), zoneinfo.available_timezones())),
-                                verbose_name=_("Time Zone"))
-    theme = models.CharField(max_length=50, null=True, blank=False, verbose_name=_("User Theme"))
-    lang = models.CharField(max_length=3, null=False, blank=False, default="en", verbose_name=_("Language"))
-    avatar = models.BinaryField(null=True, blank=False, verbose_name=_("Avatar"))
-    messages_timeout = models.IntegerField(default=10, null=False, blank=False, verbose_name=_("Message's Timeout"))
-    keep_logged_in = models.BooleanField(default=False, null=False, blank=False, verbose_name=_("Keep Logged In"))
-    app_profile = models.JSONField(null=True, blank=False, verbose_name=_("Custom Application Profile"))
+class Log(models.DatedModel):
+    action = models.CharField(max_length=100, blank=False, null=False, verbose_name=_("Action"))
+    sender = models.CharField(max_length=100, blank=False, null=False, verbose_name=_("Sender object method"))
+    ip_address = models.GenericIPAddressField(blank=True, null=True, verbose_name=_("IP Address"))
+    user = models.ForeignKey(get_user_model(), null=True, blank=False, verbose_name=_("User"), on_delete=models.CASCADE)
 
     class Meta:
-        db_table = "zb_auth_user_profile"
+        indexes = [
+            models.Index(fields=("user", ), name="IDX_logging_log_user"),
+            models.Index(fields=("action", ), name="IDX_logging_log_action")
+        ]
+
+
+class MailLog(models.Model):
+    log = models.OneToOneField(Log, blank=False, null=False, on_delete=models.PROTECT, verbose_name=_("Log"))
+    mail_from = models.CharField(max_length=250, blank=False, null=False, verbose_name=_("Mail From"))
+    mail_to = models.CharField(max_length=250, blank=False, null=False, verbose_name=_("Mail To"))
+    subject = models.CharField(max_length=250, blank=False, null=False, verbose_name=_("Subject"))
+    smtp_code = models.IntegerField(blank=False, null=False, verbose_name=_("SMTP Code"), default=0)
+    smtp_error = models.CharField(max_length=250, blank=False, null=True, verbose_name=_("SMTP Error"))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zibanu-django-1.2.0a9/zibanu/django/db/backends/oracle/base.py` & `zibanu-django-1.2.0b0/zibanu/django/db/backends/oracle/base.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/db/models/__init__.py` & `zibanu-django-1.2.0b0/zibanu/django/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/db/models/dated_model.py` & `zibanu-django-1.2.0b0/zibanu/django/db/models/dated_model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/db/models/manager.py` & `zibanu-django-1.2.0b0/zibanu/django/db/models/manager.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/db/models/model.py` & `zibanu-django-1.2.0b0/zibanu/django/db/models/model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0b0/zibanu/django/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0b0/zibanu/django/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/logging/apps.py` & `zibanu-django-1.2.0b0/zibanu/django/logging/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/logging/lib/events/__init__.py` & `zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/logging/lib/events/on_change_password.py` & `zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/on_change_password.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/logging/lib/events/on_login.py` & `zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/on_login.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/logging/lib/events/on_send_mail.py` & `zibanu-django-1.2.0b0/zibanu/django/logging/lib/events/on_send_mail.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0b0/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/logging/migrations/0001_initial.py` & `zibanu-django-1.2.0b0/zibanu/django/logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/logging/migrations/0002_maillog.py` & `zibanu-django-1.2.0b0/zibanu/django/logging/migrations/0002_maillog.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/logging/models.py` & `zibanu-django-1.2.0b0/zibanu/django/repository/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 # -*- coding: utf-8 -*-
 
-#  Developed by CQ Inversiones SAS. Copyright ©. 2019 - 2022. All rights reserved.
-#  Desarrollado por CQ Inversiones SAS. Copyright ©. 2019 - 2022. Todos los derechos reservado
+#  Developed by CQ Inversiones SAS. Copyright ©. 2019 - 2023. All rights reserved.
+#  Desarrollado por CQ Inversiones SAS. Copyright ©. 2019 - 2023. Todos los derechos reservado
 
 # ****************************************************************
 # IDE:          PyCharm
 # Developed by: macercha
-# Date:         10/12/22 10:27 AM
+# Date:         2/02/23 16:13
 # Project:      CFHL Transactional Backend
 # Module Name:  models
 # Description:
 # ****************************************************************
+import uuid
 from django.contrib.auth import get_user_model
 from django.utils.translation import gettext_lazy as _
 from zibanu.django.db import models
+from zibanu.django.repository.lib import managers
 
 
-class Log(models.DatedModel):
-    action = models.CharField(max_length=100, blank=False, null=False, verbose_name=_("Action"))
-    sender = models.CharField(max_length=100, blank=False, null=False, verbose_name=_("Sender object method"))
-    ip_address = models.GenericIPAddressField(blank=True, null=True, verbose_name=_("IP Address"))
-    user = models.ForeignKey(get_user_model(), null=True, blank=False, verbose_name=_("User"), on_delete=models.CASCADE)
+class Document(models.Model):
+    """
+    Model class that represent a document entity in database
+    """
+    code = models.CharField(max_length=10, blank=True, null=True, verbose_name=_("Validation Code"))
+    uuid = models.UUIDField(default=uuid.uuid4, verbose_name=_("UUID File"))
+    owner = models.ForeignKey(get_user_model(), verbose_name=_("Owner"), on_delete=models.PROTECT)
+    generated_at = models.DateTimeField(auto_now_add=True, verbose_name=_("Generated At"))
+    description = models.CharField(max_length=150, blank=False, null=False, verbose_name=_("Description"), default="")
+    # Set default Manager
+    objects = managers.Document()
 
     class Meta:
-        indexes = [
-            models.Index(fields=("user", ), name="IDX_logging_log_user"),
-            models.Index(fields=("action", ), name="IDX_logging_log_action")
+        constraints = [
+            models.UniqueConstraint(fields=("code", ), name="UNQ_documents_code"),
+            models.UniqueConstraint(fields=("uuid", ), name="UNQ_documents_uuid")
         ]
 
 
-class MailLog(models.Model):
-    log = models.OneToOneField(Log, blank=False, null=False, on_delete=models.PROTECT, verbose_name=_("Log"))
-    mail_from = models.CharField(max_length=250, blank=False, null=False, verbose_name=_("Mail From"))
-    mail_to = models.CharField(max_length=250, blank=False, null=False, verbose_name=_("Mail To"))
-    subject = models.CharField(max_length=250, blank=False, null=False, verbose_name=_("Subject"))
-    smtp_code = models.IntegerField(blank=False, null=False, verbose_name=_("SMTP Code"), default=0)
-    smtp_error = models.CharField(max_length=250, blank=False, null=True, verbose_name=_("SMTP Error"))
+
```

### Comparing `zibanu-django-1.2.0a9/zibanu/django/repository/apps.py` & `zibanu-django-1.2.0b0/zibanu/django/repository/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/repository/lib/managers/__init__.py` & `zibanu-django-1.2.0b0/zibanu/django/repository/lib/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/repository/lib/managers/document.py` & `zibanu-django-1.2.0b0/zibanu/django/repository/lib/managers/document.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/repository/lib/utils/__init__.py` & `zibanu-django-1.2.0b0/zibanu/django/repository/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/repository/lib/utils/document_generator.py` & `zibanu-django-1.2.0b0/zibanu/django/repository/lib/utils/document_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 # ****************************************************************
 import os
 import uuid
 from datetime import date
 from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
 from django.core.exceptions import ValidationError
-from django.http import HttpRequest
 from django.template.exceptions import TemplateDoesNotExist
 from django.template.exceptions import TemplateSyntaxError
 from django.template.loader import get_template
 from django.utils.translation import gettext_lazy as _
 from xhtml2pdf import pisa
+from zibanu.django.utils import CodeGenerator
 from zibanu.django.repository.models import Document
 
 
 class DocumentGenerator:
     def __init__(self, template_prefix: str, custom_dir: str = None, file_uuid: str = None):
         self.__custom_dir = custom_dir
         self.__template_prefix = template_prefix
@@ -87,47 +87,58 @@
             document_qs = Document.objects.get_by_uuid(kwargs.get("uuid"))
         elif "code" in kwargs:
             document_qs = Document.objects.get_by_code(kwargs.get("code"))
         else:
             raise ValueError(_("Key to get document does not found."))
         return document_qs
 
-    def generate_from_template(self, template_name: str, context: dict, request: HttpRequest, description: str = "",
-                               key: str = "code"):
+    def generate_from_template(self, template_name: str, context: dict, **kwargs):
         """
         Method to generate a pdf based on html django template
         :param template_name: name of template to render
         :param context: context file to render template
-        :param request: request object from HTTP
-        :param description: Description of document
-        :param key: key that contains a validation code, default = "code"
         :return:
         """
         try:
+            # Load vars from kwargs
+            description = kwargs.get("description", "")
+            request = kwargs.get("request", None)
+            key = kwargs.get("key", "code")
+            if request is None:
+                user = kwargs.get("user")
+                if user is None:
+                    raise ValueError(_("Request or user are required"))
+            else:
+                user = request.user
             # Created directory if it does not exist
             directory = self.__get_directory()
             if not os.path.exists(directory):
                 os.makedirs(directory)
 
-            # Set key to get validation code and get it
-            validation_code = context.get(key) if key in context else None
+            # Get validation code from key or create it
+            # Modified by macercha at 2023/06/03
+            if key in context:
+                validation_code = context.get(key)
+            else:
+                code_generator = CodeGenerator(action="rep_doc_generator")
+                validation_code = code_generator.get_alpha_numeric_code(length=10)
             # Set uuid for filename and uuid file
             file_uuid = uuid.uuid4()
             # Set filename with path and uuid and create it
             file_name = os.path.join(self.__get_directory(), file_uuid.hex + ".pdf")
             # TODO: Validate template name
             # Load template and render it
             template_name = self.__template_prefix + template_name
             template = get_template(template_name)
             rendered = template.render(context=context, request=request)
             # Generate pdf
             file_handler = open(file_name, "w+b")
             pisa_status = pisa.CreatePDF(rendered, file_handler)
             if not pisa_status.err:
-                document = Document(code=validation_code, uuid=file_uuid, owner=request.user, description=description)
+                document = Document(code=validation_code, uuid=file_uuid, owner=user, description=description)
                 document.save()
                 file_handler.close()
             else:
                 file_handler.close()
                 os.remove(file_name)
                 raise Exception(_("Error generating pdf file"))
         except OSError:
```

### Comparing `zibanu-django-1.2.0a9/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0b0/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/repository/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0b0/zibanu/django/repository/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/repository/migrations/0001_initial.py` & `zibanu-django-1.2.0b0/zibanu/django/repository/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/rest_framework/decorators.py` & `zibanu-django-1.2.0b0/zibanu/django/rest_framework/decorators.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/rest_framework/exceptions/__init__.py` & `zibanu-django-1.2.0b0/zibanu/django/rest_framework/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/rest_framework/exceptions/api_exception.py` & `zibanu-django-1.2.0b0/zibanu/django/rest_framework/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/rest_framework/fields/__init__.py` & `zibanu-django-1.2.0b0/zibanu/django/rest_framework/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/rest_framework/fields/current_user_default.py` & `zibanu-django-1.2.0b0/zibanu/django/rest_framework/fields/current_user_default.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/rest_framework/serializers/__init__.py` & `zibanu-django-1.2.0b0/zibanu/django/rest_framework/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/rest_framework/serializers/fields.py` & `zibanu-django-1.2.0b0/zibanu/django/rest_framework/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/rest_framework/serializers/model_serializer.py` & `zibanu-django-1.2.0b0/zibanu/django/rest_framework/serializers/model_serializer.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/rest_framework/viewsets/__init__.py` & `zibanu-django-1.2.0b0/zibanu/django/rest_framework/viewsets/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/rest_framework/viewsets/model_viewset.py` & `zibanu-django-1.2.0b0/zibanu/django/rest_framework/viewsets/model_viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/rest_framework/viewsets/viewset.py` & `zibanu-django-1.2.0b0/zibanu/django/rest_framework/viewsets/viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/template/apps.py` & `zibanu-django-1.2.0b0/zibanu/django/template/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/template/context_processors/__init__.py` & `zibanu-django-1.2.0b0/zibanu/django/template/context_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/template/context_processors/full_static_uri.py` & `zibanu-django-1.2.0b0/zibanu/django/template/context_processors/full_static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/template/context_processors/site.py` & `zibanu-django-1.2.0b0/zibanu/django/template/context_processors/site.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/template/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/template/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/template/templatetags/static_uri.py` & `zibanu-django-1.2.0b0/zibanu/django/template/templatetags/static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/template/templatetags/string_concat.py` & `zibanu-django-1.2.0b0/zibanu/django/template/templatetags/string_concat.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/template/templatetags/subtotal_dict.py` & `zibanu-django-1.2.0b0/zibanu/django/template/templatetags/subtotal_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/template/templatetags/sum_dict.py` & `zibanu-django-1.2.0b0/zibanu/django/template/templatetags/sum_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/utils/__init__.py` & `zibanu-django-1.2.0b0/zibanu/django/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/utils/code_generator.py` & `zibanu-django-1.2.0b0/zibanu/django/utils/code_generator.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/utils/date_time.py` & `zibanu-django-1.2.0b0/zibanu/django/utils/date_time.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/utils/error_messages.py` & `zibanu-django-1.2.0b0/zibanu/django/utils/error_messages.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/utils/mail.py` & `zibanu-django-1.2.0b0/zibanu/django/utils/mail.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/utils/request_utils.py` & `zibanu-django-1.2.0b0/zibanu/django/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/utils/user.py` & `zibanu-django-1.2.0b0/zibanu/django/utils/user.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu/django/utils/validate_cache_code.py` & `zibanu-django-1.2.0b0/zibanu/django/utils/validate_cache_code.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a9/zibanu_django.egg-info/PKG-INFO` & `zibanu-django-1.2.0b0/zibanu_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.2.0a9
-Summary: Zibanu library for django projects
+Version: 1.2.0b0
+Summary: Zibanu authentication library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -673,27 +673,27 @@
         
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
-Keywords: django,zibanu,library
+Keywords: django,zibanu,library,auth
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Zibanu Django 
+# Zibanu Django Authentication Module
 
 This package or library contains some functionalities commonly used in django projects and django rest_framework projects. 
 
 ## Django db
```

### Comparing `zibanu-django-1.2.0a9/zibanu_django.egg-info/SOURCES.txt` & `zibanu-django-1.2.0b0/zibanu_django.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 zibanu/__init__.py
 zibanu/django/__init__.py
 zibanu/django/apps.py
-zibanu/django/auth/__init__.py
-zibanu/django/auth/apps.py
-zibanu/django/auth/models.py
-zibanu/django/auth/urls.py
-zibanu/django/auth/api/__init__.py
-zibanu/django/auth/api/serializers/__init__.py
-zibanu/django/auth/api/serializers/profile.py
-zibanu/django/auth/api/serializers/token.py
-zibanu/django/auth/api/serializers/user.py
-zibanu/django/auth/api/services/__init__.py
-zibanu/django/auth/api/services/user.py
-zibanu/django/auth/lib/__init__.py
-zibanu/django/auth/lib/signal_events.py
-zibanu/django/auth/lib/signals.py
-zibanu/django/auth/lib/utils.py
-zibanu/django/auth/lib/choices/__init__.py
-zibanu/django/auth/locale/es/LC_MESSAGES/django.mo
-zibanu/django/auth/locale/es/LC_MESSAGES/django.po
-zibanu/django/auth/migrations/0001_initial.py
-zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py
-zibanu/django/auth/migrations/__init__.py
-zibanu/django/auth/templates/change_password.html
-zibanu/django/auth/templates/change_password.txt
-zibanu/django/auth/templates/request-code.html
-zibanu/django/auth/templates/request-code.txt
-zibanu/django/auth/templates/request_password.html
-zibanu/django/auth/templates/request_password.txt
 zibanu/django/db/__init__.py
 zibanu/django/db/backends/__init__.py
 zibanu/django/db/backends/oracle/__init__.py
 zibanu/django/db/backends/oracle/base.py
 zibanu/django/db/models/__init__.py
 zibanu/django/db/models/dated_model.py
 zibanu/django/db/models/manager.py
```

