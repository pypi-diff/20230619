# Comparing `tmp/nobinobi-staff-0.1.6.8.tar.gz` & `tmp/nobinobi-staff-0.1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nobinobi-staff-0.1.6.8.tar", last modified: Thu Dec 23 10:39:28 2021, max compression
+gzip compressed data, was "nobinobi-staff-0.1.6.9.tar", last modified: Wed Jun 14 13:04:41 2023, max compression
```

## Comparing `nobinobi-staff-0.1.6.8.tar` & `nobinobi-staff-0.1.6.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/
--rw-rw-rw-   0        0        0      153 2020-10-29 12:35:37.000000 nobinobi-staff-0.1.6.8/AUTHORS.rst
--rw-rw-rw-   0        0        0     3373 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     2543 2021-12-23 10:38:19.000000 nobinobi-staff-0.1.6.8/HISTORY.rst
--rw-rw-rw-   0        0        0    31774 2020-10-29 12:40:58.000000 nobinobi-staff-0.1.6.8/LICENSE
--rw-rw-rw-   0        0        0      248 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6914 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     2053 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/README.rst
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/
--rw-rw-rw-   0        0        0      684 2021-12-23 10:38:19.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/__init__.py
--rw-rw-rw-   0        0        0    10581 2021-12-23 10:38:17.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/admin.py
--rw-rw-rw-   0        0        0     1905 2021-09-17 09:46:04.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/apps.py
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/fixtures/
--rw-rw-rw-   0        0        0     1981 2020-09-01 10:41:02.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/fixtures/staff_absence_type_en-US.json
--rw-rw-rw-   0        0        0     2138 2021-03-12 09:31:05.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/fixtures/staff_absence_type_fr-CH.json
--rw-rw-rw-   0        0        0     3742 2021-12-14 10:57:24.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/forms.py
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/de/
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0      442 2021-03-12 09:31:05.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/de/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/en/
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0      399 2021-03-12 09:31:05.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/en/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr/
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     5594 2021-09-17 09:46:04.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr_CH/
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr_CH/LC_MESSAGES/
--rw-rw-rw-   0        0        0     5357 2021-09-17 10:45:02.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr_CH/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/it/
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/it/LC_MESSAGES/
--rw-rw-rw-   0        0        0      442 2021-03-12 09:31:05.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/it/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/management/
--rw-rw-rw-   0        0        0      748 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/management/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/management/commands/
--rw-rw-rw-   0        0        0      748 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/management/commands/__init__.py
--rw-rw-rw-   0        0        0     3241 2021-09-29 10:43:25.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/management/commands/generate_training.py
--rw-rw-rw-   0        0        0     4647 2021-09-29 10:43:25.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/management/commands/update_training.py
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/
--rw-rw-rw-   0        0        0     5934 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     4150 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0002_auto_20181019_1017.py
--rw-rw-rw-   0        0        0     1602 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0003_auto_20181022_1101.py
--rw-rw-rw-   0        0        0     1201 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0004_team_order.py
--rw-rw-rw-   0        0        0     1553 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0005_auto_20181116_0815.py
--rw-rw-rw-   0        0        0     1194 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0006_staff_working_base.py
--rw-rw-rw-   0        0        0     3775 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0007_auto_20200221_1138.py
--rw-rw-rw-   0        0        0     1349 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0008_add_partial_disability.py
--rw-rw-rw-   0        0        0     1374 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0009_auto_20200805_1143.py
--rw-rw-rw-   0        0        0     2794 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0010_auto_20201029_1500.py
--rw-rw-rw-   0        0        0      593 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/__init__.py
--rw-rw-rw-   0        0        0    12677 2021-12-14 10:57:24.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/models.py
--rw-rw-rw-   0        0        0     1067 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/serializers.py
--rw-rw-rw-   0        0        0     4305 2021-12-23 10:38:17.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/signals.py
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/static/
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/static/css/
--rw-rw-rw-   0        0        0      761 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/static/css/nobinobi_staff.css
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/static/js/
--rw-rw-rw-   0        0        0      761 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/static/js/nobinobi_staff.js
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/templates/
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/templates/staff/
--rw-rw-rw-   0        0        0     1530 2020-09-01 10:41:03.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/templates/staff/staff_list_readonly.html
--rw-rw-rw-   0        0        0      777 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/tests.py
--rw-rw-rw-   0        0        0     1784 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/urls.py
--rw-rw-rw-   0        0        0     1796 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/views.py
-drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/
--rw-rw-rw-   0        0        0     6914 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1864 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      331 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      344 2021-12-22 14:21:19.000000 nobinobi-staff-0.1.6.8/requirements.txt
--rw-rw-rw-   0        0        0      789 2021-12-14 10:57:24.000000 nobinobi-staff-0.1.6.8/requirements_dev.txt
--rw-rw-rw-   0        0        0      132 2021-12-14 10:57:24.000000 nobinobi-staff-0.1.6.8/requirements_test.txt
--rw-rw-rw-   0        0        0      281 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/setup.cfg
--rw-rw-rw-   0        0        0     2282 2021-04-13 08:49:29.000000 nobinobi-staff-0.1.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.621169 nobinobi-staff-0.1.6.9/
+-rw-rw-rw-   0        0        0      166 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3373 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     2616 2023-06-14 13:04:15.000000 nobinobi-staff-0.1.6.9/HISTORY.rst
+-rw-rw-rw-   0        0        0    31960 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/LICENSE
+-rw-rw-rw-   0        0        0      248 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5371 2023-06-14 13:04:41.621689 nobinobi-staff-0.1.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2053 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.591944 nobinobi-staff-0.1.6.9/nobinobi_staff/
+-rw-rw-rw-   0        0        0      684 2023-06-14 13:04:15.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/__init__.py
+-rw-rw-rw-   0        0        0    10581 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/admin.py
+-rw-rw-rw-   0        0        0     1905 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.599075 nobinobi-staff-0.1.6.9/nobinobi_staff/fixtures/
+-rw-rw-rw-   0        0        0     2095 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/fixtures/staff_absence_type_en-us.json
+-rw-rw-rw-   0        0        0     2138 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/fixtures/staff_absence_type_fr-CH.json
+-rw-rw-rw-   0        0        0     3742 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/forms.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.573491 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.571449 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/de/
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.599075 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      442 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/de/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.572472 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/en/
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.600615 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      399 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/en/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.572472 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.601135 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     5594 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/fr/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.573491 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/fr_CH/
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.603263 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/fr_CH/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     5357 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/fr_CH/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.573491 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/it/
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.604284 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      442 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/locale/it/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.605308 nobinobi-staff-0.1.6.9/nobinobi_staff/management/
+-rw-rw-rw-   0        0        0      748 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.607343 nobinobi-staff-0.1.6.9/nobinobi_staff/management/commands/
+-rw-rw-rw-   0        0        0      748 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     3241 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/management/commands/generate_training.py
+-rw-rw-rw-   0        0        0     4647 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/management/commands/update_training.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.617628 nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/
+-rw-rw-rw-   0        0        0     5934 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     4150 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0002_auto_20181019_1017.py
+-rw-rw-rw-   0        0        0     1602 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0003_auto_20181022_1101.py
+-rw-rw-rw-   0        0        0     1201 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0004_team_order.py
+-rw-rw-rw-   0        0        0     1553 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0005_auto_20181116_0815.py
+-rw-rw-rw-   0        0        0     1194 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0006_staff_working_base.py
+-rw-rw-rw-   0        0        0     3775 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0007_auto_20200221_1138.py
+-rw-rw-rw-   0        0        0     1349 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0008_add_partial_disability.py
+-rw-rw-rw-   0        0        0     1374 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0009_auto_20200805_1143.py
+-rw-rw-rw-   0        0        0     2794 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0010_auto_20201029_1500.py
+-rw-rw-rw-   0        0        0      593 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/__init__.py
+-rw-rw-rw-   0        0        0    12677 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/models.py
+-rw-rw-rw-   0        0        0     1067 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/serializers.py
+-rw-rw-rw-   0        0        0     4305 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/signals.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.575530 nobinobi-staff-0.1.6.9/nobinobi_staff/static/
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.618635 nobinobi-staff-0.1.6.9/nobinobi_staff/static/css/
+-rw-rw-rw-   0        0        0      761 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/static/css/nobinobi_staff.css
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.619655 nobinobi-staff-0.1.6.9/nobinobi_staff/static/js/
+-rw-rw-rw-   0        0        0      761 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/static/js/nobinobi_staff.js
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.575530 nobinobi-staff-0.1.6.9/nobinobi_staff/templates/
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.620662 nobinobi-staff-0.1.6.9/nobinobi_staff/templates/staff/
+-rw-rw-rw-   0        0        0     1579 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/templates/staff/staff_list_readonly.html
+-rw-rw-rw-   0        0        0      777 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/tests.py
+-rw-rw-rw-   0        0        0     1784 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/urls.py
+-rw-rw-rw-   0        0        0     1796 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/nobinobi_staff/views.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:04:41.597039 nobinobi-staff-0.1.6.9/nobinobi_staff.egg-info/
+-rw-rw-rw-   0        0        0     5371 2023-06-14 13:04:41.000000 nobinobi-staff-0.1.6.9/nobinobi_staff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1864 2023-06-14 13:04:41.000000 nobinobi-staff-0.1.6.9/nobinobi_staff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 13:04:41.000000 nobinobi-staff-0.1.6.9/nobinobi_staff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 13:04:41.000000 nobinobi-staff-0.1.6.9/nobinobi_staff.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      404 2023-06-14 13:04:41.000000 nobinobi-staff-0.1.6.9/nobinobi_staff.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-14 13:04:41.000000 nobinobi-staff-0.1.6.9/nobinobi_staff.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      936 2023-06-14 12:53:53.000000 nobinobi-staff-0.1.6.9/requirements.txt
+-rw-rw-rw-   0        0        0      769 2023-06-14 12:58:50.000000 nobinobi-staff-0.1.6.9/requirements_dev.txt
+-rw-rw-rw-   0        0        0      125 2023-06-14 12:58:04.000000 nobinobi-staff-0.1.6.9/requirements_test.txt
+-rw-rw-rw-   0        0        0      281 2023-06-14 13:04:41.622714 nobinobi-staff-0.1.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     2282 2023-06-14 10:52:26.000000 nobinobi-staff-0.1.6.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nobinobi-staff-0.1.6.8/CONTRIBUTING.rst` & `nobinobi-staff-0.1.6.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/HISTORY.rst` & `nobinobi-staff-0.1.6.9/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. :changelog:
 
 History
 -------
 
+0.1.6.9 (2023-06-14)
+++++++++++++++++++++++
+
+* Update requirements
+
 0.1.6.8 (2021-12-23)
 ++++++++++++++++++++++
 
 * 879490a - filter on choice staff absence only active staff
 * d04ba24 - Fix bug when save staff for training
 
 0.1.6.7 (2021-12-22)
```

### Comparing `nobinobi-staff-0.1.6.8/LICENSE` & `nobinobi-staff-0.1.6.9/LICENSE`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-GNU AFFERO GENERAL PUBLIC LICENSE
-
-Version 3, 19 November 2007
-
-Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org/>
-Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
-Preamble
-
-The GNU Affero General Public License is a free, copyleft license for software and other kinds of works, specifically designed to ensure cooperation with the community in the case of network server software.
-
-The licenses for most software and other practical works are designed to take away your freedom to share and change the works. By contrast, our General Public Licenses are intended to guarantee your freedom to share and change all versions of a program--to make sure it remains free software for all its users.
-
-When we speak of free software, we are referring to freedom, not price. Our General Public Licenses are designed to make sure that you have the freedom to distribute copies of free software (and charge for them if you wish), that you receive source code or can get it if you want it, that you can change the software or use pieces of it in new free programs, and that you know you can do these things.
-
-Developers that use our General Public Licenses protect your rights with two steps: (1) assert copyright on the software, and (2) offer you this License which gives you legal permission to copy, distribute and/or modify the software.
-
-A secondary benefit of defending all users' freedom is that improvements made in alternate versions of the program, if they receive widespread use, become available for other developers to incorporate. Many developers of free software are heartened and encouraged by the resulting cooperation. However, in the case of software used on network servers, this result may fail to come about. The GNU General Public License permits making a modified version and letting the public access it on a server without ever releasing its source code to the public.
-
-The GNU Affero General Public License is designed specifically to ensure that, in such cases, the modified source code becomes available to the community. It requires the operator of a network server to provide the source code of the modified version running there to the users of that server. Therefore, public use of a modified version, on a publicly accessible server, gives the public access to the source code of the modified version.
-
-An older license, called the Affero General Public License and published by Affero, was designed to accomplish similar goals. This is a different license, not a version of the Affero GPL, but Affero has released a new version of the Affero GPL which permits relicensing under this license.
-
-The precise terms and conditions for copying, distribution and modification follow.
-TERMS AND CONDITIONS
-0. Definitions.
-
-"This License" refers to version 3 of the GNU Affero General Public License.
-
-"Copyright" also means copyright-like laws that apply to other kinds of works, such as semiconductor masks.
-
-"The Program" refers to any copyrightable work licensed under this License. Each licensee is addressed as "you". "Licensees" and "recipients" may be individuals or organizations.
-
-To "modify" a work means to copy from or adapt all or part of the work in a fashion requiring copyright permission, other than the making of an exact copy. The resulting work is called a "modified version" of the earlier work or a work "based on" the earlier work.
-
-A "covered work" means either the unmodified Program or a work based on the Program.
-
-To "propagate" a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.
-
-To "convey" a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.
-
-An interactive user interface displays "Appropriate Legal Notices" to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.
-1. Source Code.
-
-The "source code" for a work means the preferred form of the work for making modifications to it. "Object code" means any non-source form of a work.
-
-A "Standard Interface" means an interface that either is an official standard defined by a recognized standards body, or, in the case of interfaces specified for a particular programming language, one that is widely used among developers working in that language.
-
-The "System Libraries" of an executable work include anything, other than the work as a whole, that (a) is included in the normal form of packaging a Major Component, but which is not part of that Major Component, and (b) serves only to enable use of the work with that Major Component, or to implement a Standard Interface for which an implementation is available to the public in source code form. A "Major Component", in this context, means a major essential component (kernel, window system, and so on) of the specific operating system (if any) on which the executable work runs, or a compiler used to produce the work, or an object code interpreter used to run it.
-
-The "Corresponding Source" for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities. However, it does not include the work's System Libraries, or general-purpose tools or generally available free programs which are used unmodified in performing those activities but which are not part of the work. For example, Corresponding Source includes interface definition files associated with source files for the work, and the source code for shared libraries and dynamically linked subprograms that the work is specifically designed to require, such as by intimate data communication or control flow between those subprograms and other parts of the work.
-
-The Corresponding Source need not include anything that users can regenerate automatically from other parts of the Corresponding Source.
-
-The Corresponding Source for a work in source code form is that same work.
-2. Basic Permissions.
-
-All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met. This License explicitly affirms your unlimited permission to run the unmodified Program. The output from running a covered work is covered by this License only if the output, given its content, constitutes a covered work. This License acknowledges your rights of fair use or other equivalent, as provided by copyright law.
-
-You may make, run and propagate covered works that you do not convey, without conditions so long as your license otherwise remains in force. You may convey covered works to others for the sole purpose of having them make modifications exclusively for you, or provide you with facilities for running those works, provided that you comply with the terms of this License in conveying all material for which you do not control copyright. Those thus making or running the covered works for you must do so exclusively on your behalf, under your direction and control, on terms that prohibit them from making any copies of your copyrighted material outside their relationship with you.
-
-Conveying under any other circumstances is permitted solely under the conditions stated below. Sublicensing is not allowed; section 10 makes it unnecessary.
-3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-No covered work shall be deemed part of an effective technological measure under any applicable law fulfilling obligations under article 11 of the WIPO copyright treaty adopted on 20 December 1996, or similar laws prohibiting or restricting circumvention of such measures.
-
-When you convey a covered work, you waive any legal power to forbid circumvention of technological measures to the extent such circumvention is effected by exercising rights under this License with respect to the covered work, and you disclaim any intention to limit operation or modification of the work as a means of enforcing, against the work's users, your or third parties' legal rights to forbid circumvention of technological measures.
-4. Conveying Verbatim Copies.
-
-You may convey verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice; keep intact all notices stating that this License and any non-permissive terms added in accord with section 7 apply to the code; keep intact all notices of the absence of any warranty; and give all recipients a copy of this License along with the Program.
-
-You may charge any price or no price for each copy that you convey, and you may offer support or warranty protection for a fee.
-5. Conveying Modified Source Versions.
-
-You may convey a work based on the Program, or the modifications to produce it from the Program, in the form of source code under the terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified it, and giving a relevant date.
-    b) The work must carry prominent notices stating that it is released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to "keep intact all notices".
-    c) You must license the entire work, as a whole, under this License to anyone who comes into possession of a copy. This License will therefore apply, along with any applicable section 7 additional terms, to the whole of the work, and all its parts, regardless of how they are packaged. This License gives no permission to license the work in any other way, but it does not invalidate such permission if you have separately received it.
-    d) If the work has interactive user interfaces, each must display Appropriate Legal Notices; however, if the Program has interactive interfaces that do not display Appropriate Legal Notices, your work need not make them do so.
-
-A compilation of a covered work with other separate and independent works, which are not by their nature extensions of the covered work, and which are not combined with it such as to form a larger program, in or on a volume of a storage or distribution medium, is called an "aggregate" if the compilation and its resulting copyright are not used to limit the access or legal rights of the compilation's users beyond what the individual works permit. Inclusion of a covered work in an aggregate does not cause this License to apply to the other parts of the aggregate.
-6. Conveying Non-Source Forms.
-
-You may convey a covered work in object code form under the terms of sections 4 and 5, provided that you also convey the machine-readable Corresponding Source under the terms of this License, in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by the Corresponding Source fixed on a durable physical medium customarily used for software interchange.
-    b) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by a written offer, valid for at least three years and valid for as long as you offer spare parts or customer support for that product model, to give anyone who possesses the object code either (1) a copy of the Corresponding Source for all the software in the product that is covered by this License, on a durable physical medium customarily used for software interchange, for a price no more than your reasonable cost of physically performing this conveying of source, or (2) access to copy the Corresponding Source from a network server at no charge.
-    c) Convey individual copies of the object code with a copy of the written offer to provide the Corresponding Source. This alternative is allowed only occasionally and noncommercially, and only if you received the object code with such an offer, in accord with subsection 6b.
-    d) Convey the object code by offering access from a designated place (gratis or for a charge), and offer equivalent access to the Corresponding Source in the same way through the same place at no further charge. You need not require recipients to copy the Corresponding Source along with the object code. If the place to copy the object code is a network server, the Corresponding Source may be on a different server (operated by you or a third party) that supports equivalent copying facilities, provided you maintain clear directions next to the object code saying where to find the Corresponding Source. Regardless of what server hosts the Corresponding Source, you remain obligated to ensure that it is available for as long as needed to satisfy these requirements.
-    e) Convey the object code using peer-to-peer transmission, provided you inform other peers where the object code and Corresponding Source of the work are being offered to the general public at no charge under subsection 6d.
-
-A separable portion of the object code, whose source code is excluded from the Corresponding Source as a System Library, need not be included in conveying the object code work.
-
-A "User Product" is either (1) a "consumer product", which means any tangible personal property which is normally used for personal, family, or household purposes, or (2) anything designed or sold for incorporation into a dwelling. In determining whether a product is a consumer product, doubtful cases shall be resolved in favor of coverage. For a particular product received by a particular user, "normally used" refers to a typical or common use of that class of product, regardless of the status of the particular user or of the way in which the particular user actually uses, or expects or is expected to use, the product. A product is a consumer product regardless of whether the product has substantial commercial, industrial or non-consumer uses, unless such uses represent the only significant mode of use of the product.
-
-"Installation Information" for a User Product means any methods, procedures, authorization keys, or other information required to install and execute modified versions of a covered work in that User Product from a modified version of its Corresponding Source. The information must suffice to ensure that the continued functioning of the modified object code is in no case prevented or interfered with solely because modification has been made.
-
-If you convey an object code work under this section in, or with, or specifically for use in, a User Product, and the conveying occurs as part of a transaction in which the right of possession and use of the User Product is transferred to the recipient in perpetuity or for a fixed term (regardless of how the transaction is characterized), the Corresponding Source conveyed under this section must be accompanied by the Installation Information. But this requirement does not apply if neither you nor any third party retains the ability to install modified object code on the User Product (for example, the work has been installed in ROM).
-
-The requirement to provide Installation Information does not include a requirement to continue to provide support service, warranty, or updates for a work that has been modified or installed by the recipient, or for the User Product in which it has been modified or installed. Access to a network may be denied when the modification itself materially and adversely affects the operation of the network or violates the rules and protocols for communication across the network.
-
-Corresponding Source conveyed, and Installation Information provided, in accord with this section must be in a format that is publicly documented (and with an implementation available to the public in source code form), and must require no special password or key for unpacking, reading or copying.
-7. Additional Terms.
-
-"Additional permissions" are terms that supplement the terms of this License by making exceptions from one or more of its conditions. Additional permissions that are applicable to the entire Program shall be treated as though they were included in this License, to the extent that they are valid under applicable law. If additional permissions apply only to part of the Program, that part may be used separately under those permissions, but the entire Program remains governed by this License without regard to the additional permissions.
-
-When you convey a copy of a covered work, you may at your option remove any additional permissions from that copy, or from any part of it. (Additional permissions may be written to require their own removal in certain cases when you modify the work.) You may place additional permissions on material, added by you to a covered work, for which you have or can give appropriate copyright permission.
-
-Notwithstanding any other provision of this License, for material you add to a covered work, you may (if authorized by the copyright holders of that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the terms of sections 15 and 16 of this License; or
-    b) Requiring preservation of specified reasonable legal notices or author attributions in that material or in the Appropriate Legal Notices displayed by works containing it; or
-    c) Prohibiting misrepresentation of the origin of that material, or requiring that modified versions of such material be marked in reasonable ways as different from the original version; or
-    d) Limiting the use for publicity purposes of names of licensors or authors of the material; or
-    e) Declining to grant rights under trademark law for use of some trade names, trademarks, or service marks; or
-    f) Requiring indemnification of licensors and authors of that material by anyone who conveys the material (or modified versions of it) with contractual assumptions of liability to the recipient, for any liability that these contractual assumptions directly impose on those licensors and authors.
-
-All other non-permissive additional terms are considered "further restrictions" within the meaning of section 10. If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term. If a license document contains a further restriction but permits relicensing or conveying under this License, you may add to a covered work material governed by the terms of that license document, provided that the further restriction does not survive such relicensing or conveying.
-
-If you add terms to a covered work in accord with this section, you must place, in the relevant source files, a statement of the additional terms that apply to those files, or a notice indicating where to find the applicable terms.
-
-Additional terms, permissive or non-permissive, may be stated in the form of a separately written license, or stated as exceptions; the above requirements apply either way.
-8. Termination.
-
-You may not propagate or modify a covered work except as expressly provided under this License. Any attempt otherwise to propagate or modify it is void, and will automatically terminate your rights under this License (including any patent licenses granted under the third paragraph of section 11).
-
-However, if you cease all violation of this License, then your license from a particular copyright holder is reinstated (a) provisionally, unless and until the copyright holder explicitly and finally terminates your license, and (b) permanently, if the copyright holder fails to notify you of the violation by some reasonable means prior to 60 days after the cessation.
-
-Moreover, your license from a particular copyright holder is reinstated permanently if the copyright holder notifies you of the violation by some reasonable means, this is the first time you have received notice of violation of this License (for any work) from that copyright holder, and you cure the violation prior to 30 days after your receipt of the notice.
-
-Termination of your rights under this section does not terminate the licenses of parties who have received copies or rights from you under this License. If your rights have been terminated and not permanently reinstated, you do not qualify to receive new licenses for the same material under section 10.
-9. Acceptance Not Required for Having Copies.
-
-You are not required to accept this License in order to receive or run a copy of the Program. Ancillary propagation of a covered work occurring solely as a consequence of using peer-to-peer transmission to receive a copy likewise does not require acceptance. However, nothing other than this License grants you permission to propagate or modify any covered work. These actions infringe copyright if you do not accept this License. Therefore, by modifying or propagating a covered work, you indicate your acceptance of this License to do so.
-10. Automatic Licensing of Downstream Recipients.
-
-Each time you convey a covered work, the recipient automatically receives a license from the original licensors, to run, modify and propagate that work, subject to this License. You are not responsible for enforcing compliance by third parties with this License.
-
-An "entity transaction" is a transaction transferring control of an organization, or substantially all assets of one, or subdividing an organization, or merging organizations. If propagation of a covered work results from an entity transaction, each party to that transaction who receives a copy of the work also receives whatever licenses to the work the party's predecessor in interest had or could give under the previous paragraph, plus a right to possession of the Corresponding Source of the work from the predecessor in interest, if the predecessor has it or can get it with reasonable efforts.
-
-You may not impose any further restrictions on the exercise of the rights granted or affirmed under this License. For example, you may not impose a license fee, royalty, or other charge for exercise of rights granted under this License, and you may not initiate litigation (including a cross-claim or counterclaim in a lawsuit) alleging that any patent claim is infringed by making, using, selling, offering for sale, or importing the Program or any portion of it.
-11. Patents.
-
-A "contributor" is a copyright holder who authorizes use under this License of the Program or a work on which the Program is based. The work thus licensed is called the contributor's "contributor version".
-
-A contributor's "essential patent claims" are all patent claims owned or controlled by the contributor, whether already acquired or hereafter acquired, that would be infringed by some manner, permitted by this License, of making, using, or selling its contributor version, but do not include claims that would be infringed only as a consequence of further modification of the contributor version. For purposes of this definition, "control" includes the right to grant patent sublicenses in a manner consistent with the requirements of this License.
-
-Each contributor grants you a non-exclusive, worldwide, royalty-free patent license under the contributor's essential patent claims, to make, use, sell, offer for sale, import and otherwise run, modify and propagate the contents of its contributor version.
-
-In the following three paragraphs, a "patent license" is any express agreement or commitment, however denominated, not to enforce a patent (such as an express permission to practice a patent or covenant not to sue for patent infringement). To "grant" such a patent license to a party means to make such an agreement or commitment not to enforce a patent against the party.
-
-If you convey a covered work, knowingly relying on a patent license, and the Corresponding Source of the work is not available for anyone to copy, free of charge and under the terms of this License, through a publicly available network server or other readily accessible means, then you must either (1) cause the Corresponding Source to be so available, or (2) arrange to deprive yourself of the benefit of the patent license for this particular work, or (3) arrange, in a manner consistent with the requirements of this License, to extend the patent license to downstream recipients. "Knowingly relying" means you have actual knowledge that, but for the patent license, your conveying the covered work in a country, or your recipient's use of the covered work in a country, would infringe one or more identifiable patents in that country that you have reason to believe are valid.
-
-If, pursuant to or in connection with a single transaction or arrangement, you convey, or propagate by procuring conveyance of, a covered work, and grant a patent license to some of the parties receiving the covered work authorizing them to use, propagate, modify or convey a specific copy of the covered work, then the patent license you grant is automatically extended to all recipients of the covered work and works based on it.
-
-A patent license is "discriminatory" if it does not include within the scope of its coverage, prohibits the exercise of, or is conditioned on the non-exercise of one or more of the rights that are specifically granted under this License. You may not convey a covered work if you are a party to an arrangement with a third party that is in the business of distributing software, under which you make payment to the third party based on the extent of your activity of conveying the work, and under which the third party grants, to any of the parties who would receive the covered work from you, a discriminatory patent license (a) in connection with copies of the covered work conveyed by you (or copies made from those copies), or (b) primarily for and in connection with specific products or compilations that contain the covered work, unless you entered into that arrangement, or that patent license was granted, prior to 28 March 2007.
-
-Nothing in this License shall be construed as excluding or limiting any implied license or other defenses to infringement that may otherwise be available to you under applicable patent law.
-12. No Surrender of Others' Freedom.
-
-If conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot convey a covered work so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not convey it at all. For example, if you agree to terms that obligate you to collect a royalty for further conveying from those to whom you convey the Program, the only way you could satisfy both those terms and this License would be to refrain entirely from conveying the Program.
-13. Remote Network Interaction; Use with the GNU General Public License.
-
-Notwithstanding any other provision of this License, if you modify the Program, your modified version must prominently offer all users interacting with it remotely through a computer network (if your version supports such interaction) an opportunity to receive the Corresponding Source of your version by providing access to the Corresponding Source from a network server at no charge, through some standard or customary means of facilitating copying of software. This Corresponding Source shall include the Corresponding Source for any work covered by version 3 of the GNU General Public License that is incorporated pursuant to the following paragraph.
-
-Notwithstanding any other provision of this License, you have permission to link or combine any covered work with a work licensed under version 3 of the GNU General Public License into a single combined work, and to convey the resulting work. The terms of this License will continue to apply to the part which is the covered work, but the work with which it is combined will remain governed by version 3 of the GNU General Public License.
-14. Revised Versions of this License.
-
-The Free Software Foundation may publish revised and/or new versions of the GNU Affero General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number. If the Program specifies that a certain numbered version of the GNU Affero General Public License "or any later version" applies to it, you have the option of following the terms and conditions either of that numbered version or of any later version published by the Free Software Foundation. If the Program does not specify a version number of the GNU Affero General Public License, you may choose any version ever published by the Free Software Foundation.
-
-If the Program specifies that a proxy can decide which future versions of the GNU Affero General Public License can be used, that proxy's public statement of acceptance of a version permanently authorizes you to choose that version for the Program.
-
-Later license versions may give you additional or different permissions. However, no additional obligations are imposed on any author or copyright holder as a result of your choosing to follow a later version.
-15. Disclaimer of Warranty.
-
-THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-16. Limitation of Liability.
-
-IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
-17. Interpretation of Sections 15 and 16.
-
-If the disclaimer of warranty and limitation of liability provided above cannot be given local legal effect according to their terms, reviewing courts shall apply local law that most closely approximates an absolute waiver of all civil liability in connection with the Program, unless a warranty or assumption of liability accompanies a copy of the Program in return for a fee.
-
-END OF TERMS AND CONDITIONS
+GNU AFFERO GENERAL PUBLIC LICENSE
+
+Version 3, 19 November 2007
+
+Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org/>
+Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
+Preamble
+
+The GNU Affero General Public License is a free, copyleft license for software and other kinds of works, specifically designed to ensure cooperation with the community in the case of network server software.
+
+The licenses for most software and other practical works are designed to take away your freedom to share and change the works. By contrast, our General Public Licenses are intended to guarantee your freedom to share and change all versions of a program--to make sure it remains free software for all its users.
+
+When we speak of free software, we are referring to freedom, not price. Our General Public Licenses are designed to make sure that you have the freedom to distribute copies of free software (and charge for them if you wish), that you receive source code or can get it if you want it, that you can change the software or use pieces of it in new free programs, and that you know you can do these things.
+
+Developers that use our General Public Licenses protect your rights with two steps: (1) assert copyright on the software, and (2) offer you this License which gives you legal permission to copy, distribute and/or modify the software.
+
+A secondary benefit of defending all users' freedom is that improvements made in alternate versions of the program, if they receive widespread use, become available for other developers to incorporate. Many developers of free software are heartened and encouraged by the resulting cooperation. However, in the case of software used on network servers, this result may fail to come about. The GNU General Public License permits making a modified version and letting the public access it on a server without ever releasing its source code to the public.
+
+The GNU Affero General Public License is designed specifically to ensure that, in such cases, the modified source code becomes available to the community. It requires the operator of a network server to provide the source code of the modified version running there to the users of that server. Therefore, public use of a modified version, on a publicly accessible server, gives the public access to the source code of the modified version.
+
+An older license, called the Affero General Public License and published by Affero, was designed to accomplish similar goals. This is a different license, not a version of the Affero GPL, but Affero has released a new version of the Affero GPL which permits relicensing under this license.
+
+The precise terms and conditions for copying, distribution and modification follow.
+TERMS AND CONDITIONS
+0. Definitions.
+
+"This License" refers to version 3 of the GNU Affero General Public License.
+
+"Copyright" also means copyright-like laws that apply to other kinds of works, such as semiconductor masks.
+
+"The Program" refers to any copyrightable work licensed under this License. Each licensee is addressed as "you". "Licensees" and "recipients" may be individuals or organizations.
+
+To "modify" a work means to copy from or adapt all or part of the work in a fashion requiring copyright permission, other than the making of an exact copy. The resulting work is called a "modified version" of the earlier work or a work "based on" the earlier work.
+
+A "covered work" means either the unmodified Program or a work based on the Program.
+
+To "propagate" a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.
+
+To "convey" a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.
+
+An interactive user interface displays "Appropriate Legal Notices" to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.
+1. Source Code.
+
+The "source code" for a work means the preferred form of the work for making modifications to it. "Object code" means any non-source form of a work.
+
+A "Standard Interface" means an interface that either is an official standard defined by a recognized standards body, or, in the case of interfaces specified for a particular programming language, one that is widely used among developers working in that language.
+
+The "System Libraries" of an executable work include anything, other than the work as a whole, that (a) is included in the normal form of packaging a Major Component, but which is not part of that Major Component, and (b) serves only to enable use of the work with that Major Component, or to implement a Standard Interface for which an implementation is available to the public in source code form. A "Major Component", in this context, means a major essential component (kernel, window system, and so on) of the specific operating system (if any) on which the executable work runs, or a compiler used to produce the work, or an object code interpreter used to run it.
+
+The "Corresponding Source" for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities. However, it does not include the work's System Libraries, or general-purpose tools or generally available free programs which are used unmodified in performing those activities but which are not part of the work. For example, Corresponding Source includes interface definition files associated with source files for the work, and the source code for shared libraries and dynamically linked subprograms that the work is specifically designed to require, such as by intimate data communication or control flow between those subprograms and other parts of the work.
+
+The Corresponding Source need not include anything that users can regenerate automatically from other parts of the Corresponding Source.
+
+The Corresponding Source for a work in source code form is that same work.
+2. Basic Permissions.
+
+All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met. This License explicitly affirms your unlimited permission to run the unmodified Program. The output from running a covered work is covered by this License only if the output, given its content, constitutes a covered work. This License acknowledges your rights of fair use or other equivalent, as provided by copyright law.
+
+You may make, run and propagate covered works that you do not convey, without conditions so long as your license otherwise remains in force. You may convey covered works to others for the sole purpose of having them make modifications exclusively for you, or provide you with facilities for running those works, provided that you comply with the terms of this License in conveying all material for which you do not control copyright. Those thus making or running the covered works for you must do so exclusively on your behalf, under your direction and control, on terms that prohibit them from making any copies of your copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under the conditions stated below. Sublicensing is not allowed; section 10 makes it unnecessary.
+3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+No covered work shall be deemed part of an effective technological measure under any applicable law fulfilling obligations under article 11 of the WIPO copyright treaty adopted on 20 December 1996, or similar laws prohibiting or restricting circumvention of such measures.
+
+When you convey a covered work, you waive any legal power to forbid circumvention of technological measures to the extent such circumvention is effected by exercising rights under this License with respect to the covered work, and you disclaim any intention to limit operation or modification of the work as a means of enforcing, against the work's users, your or third parties' legal rights to forbid circumvention of technological measures.
+4. Conveying Verbatim Copies.
+
+You may convey verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice; keep intact all notices stating that this License and any non-permissive terms added in accord with section 7 apply to the code; keep intact all notices of the absence of any warranty; and give all recipients a copy of this License along with the Program.
+
+You may charge any price or no price for each copy that you convey, and you may offer support or warranty protection for a fee.
+5. Conveying Modified Source Versions.
+
+You may convey a work based on the Program, or the modifications to produce it from the Program, in the form of source code under the terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified it, and giving a relevant date.
+    b) The work must carry prominent notices stating that it is released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to "keep intact all notices".
+    c) You must license the entire work, as a whole, under this License to anyone who comes into possession of a copy. This License will therefore apply, along with any applicable section 7 additional terms, to the whole of the work, and all its parts, regardless of how they are packaged. This License gives no permission to license the work in any other way, but it does not invalidate such permission if you have separately received it.
+    d) If the work has interactive user interfaces, each must display Appropriate Legal Notices; however, if the Program has interactive interfaces that do not display Appropriate Legal Notices, your work need not make them do so.
+
+A compilation of a covered work with other separate and independent works, which are not by their nature extensions of the covered work, and which are not combined with it such as to form a larger program, in or on a volume of a storage or distribution medium, is called an "aggregate" if the compilation and its resulting copyright are not used to limit the access or legal rights of the compilation's users beyond what the individual works permit. Inclusion of a covered work in an aggregate does not cause this License to apply to the other parts of the aggregate.
+6. Conveying Non-Source Forms.
+
+You may convey a covered work in object code form under the terms of sections 4 and 5, provided that you also convey the machine-readable Corresponding Source under the terms of this License, in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by the Corresponding Source fixed on a durable physical medium customarily used for software interchange.
+    b) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by a written offer, valid for at least three years and valid for as long as you offer spare parts or customer support for that product model, to give anyone who possesses the object code either (1) a copy of the Corresponding Source for all the software in the product that is covered by this License, on a durable physical medium customarily used for software interchange, for a price no more than your reasonable cost of physically performing this conveying of source, or (2) access to copy the Corresponding Source from a network server at no charge.
+    c) Convey individual copies of the object code with a copy of the written offer to provide the Corresponding Source. This alternative is allowed only occasionally and noncommercially, and only if you received the object code with such an offer, in accord with subsection 6b.
+    d) Convey the object code by offering access from a designated place (gratis or for a charge), and offer equivalent access to the Corresponding Source in the same way through the same place at no further charge. You need not require recipients to copy the Corresponding Source along with the object code. If the place to copy the object code is a network server, the Corresponding Source may be on a different server (operated by you or a third party) that supports equivalent copying facilities, provided you maintain clear directions next to the object code saying where to find the Corresponding Source. Regardless of what server hosts the Corresponding Source, you remain obligated to ensure that it is available for as long as needed to satisfy these requirements.
+    e) Convey the object code using peer-to-peer transmission, provided you inform other peers where the object code and Corresponding Source of the work are being offered to the general public at no charge under subsection 6d.
+
+A separable portion of the object code, whose source code is excluded from the Corresponding Source as a System Library, need not be included in conveying the object code work.
+
+A "User Product" is either (1) a "consumer product", which means any tangible personal property which is normally used for personal, family, or household purposes, or (2) anything designed or sold for incorporation into a dwelling. In determining whether a product is a consumer product, doubtful cases shall be resolved in favor of coverage. For a particular product received by a particular user, "normally used" refers to a typical or common use of that class of product, regardless of the status of the particular user or of the way in which the particular user actually uses, or expects or is expected to use, the product. A product is a consumer product regardless of whether the product has substantial commercial, industrial or non-consumer uses, unless such uses represent the only significant mode of use of the product.
+
+"Installation Information" for a User Product means any methods, procedures, authorization keys, or other information required to install and execute modified versions of a covered work in that User Product from a modified version of its Corresponding Source. The information must suffice to ensure that the continued functioning of the modified object code is in no case prevented or interfered with solely because modification has been made.
+
+If you convey an object code work under this section in, or with, or specifically for use in, a User Product, and the conveying occurs as part of a transaction in which the right of possession and use of the User Product is transferred to the recipient in perpetuity or for a fixed term (regardless of how the transaction is characterized), the Corresponding Source conveyed under this section must be accompanied by the Installation Information. But this requirement does not apply if neither you nor any third party retains the ability to install modified object code on the User Product (for example, the work has been installed in ROM).
+
+The requirement to provide Installation Information does not include a requirement to continue to provide support service, warranty, or updates for a work that has been modified or installed by the recipient, or for the User Product in which it has been modified or installed. Access to a network may be denied when the modification itself materially and adversely affects the operation of the network or violates the rules and protocols for communication across the network.
+
+Corresponding Source conveyed, and Installation Information provided, in accord with this section must be in a format that is publicly documented (and with an implementation available to the public in source code form), and must require no special password or key for unpacking, reading or copying.
+7. Additional Terms.
+
+"Additional permissions" are terms that supplement the terms of this License by making exceptions from one or more of its conditions. Additional permissions that are applicable to the entire Program shall be treated as though they were included in this License, to the extent that they are valid under applicable law. If additional permissions apply only to part of the Program, that part may be used separately under those permissions, but the entire Program remains governed by this License without regard to the additional permissions.
+
+When you convey a copy of a covered work, you may at your option remove any additional permissions from that copy, or from any part of it. (Additional permissions may be written to require their own removal in certain cases when you modify the work.) You may place additional permissions on material, added by you to a covered work, for which you have or can give appropriate copyright permission.
+
+Notwithstanding any other provision of this License, for material you add to a covered work, you may (if authorized by the copyright holders of that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the terms of sections 15 and 16 of this License; or
+    b) Requiring preservation of specified reasonable legal notices or author attributions in that material or in the Appropriate Legal Notices displayed by works containing it; or
+    c) Prohibiting misrepresentation of the origin of that material, or requiring that modified versions of such material be marked in reasonable ways as different from the original version; or
+    d) Limiting the use for publicity purposes of names of licensors or authors of the material; or
+    e) Declining to grant rights under trademark law for use of some trade names, trademarks, or service marks; or
+    f) Requiring indemnification of licensors and authors of that material by anyone who conveys the material (or modified versions of it) with contractual assumptions of liability to the recipient, for any liability that these contractual assumptions directly impose on those licensors and authors.
+
+All other non-permissive additional terms are considered "further restrictions" within the meaning of section 10. If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term. If a license document contains a further restriction but permits relicensing or conveying under this License, you may add to a covered work material governed by the terms of that license document, provided that the further restriction does not survive such relicensing or conveying.
+
+If you add terms to a covered work in accord with this section, you must place, in the relevant source files, a statement of the additional terms that apply to those files, or a notice indicating where to find the applicable terms.
+
+Additional terms, permissive or non-permissive, may be stated in the form of a separately written license, or stated as exceptions; the above requirements apply either way.
+8. Termination.
+
+You may not propagate or modify a covered work except as expressly provided under this License. Any attempt otherwise to propagate or modify it is void, and will automatically terminate your rights under this License (including any patent licenses granted under the third paragraph of section 11).
+
+However, if you cease all violation of this License, then your license from a particular copyright holder is reinstated (a) provisionally, unless and until the copyright holder explicitly and finally terminates your license, and (b) permanently, if the copyright holder fails to notify you of the violation by some reasonable means prior to 60 days after the cessation.
+
+Moreover, your license from a particular copyright holder is reinstated permanently if the copyright holder notifies you of the violation by some reasonable means, this is the first time you have received notice of violation of this License (for any work) from that copyright holder, and you cure the violation prior to 30 days after your receipt of the notice.
+
+Termination of your rights under this section does not terminate the licenses of parties who have received copies or rights from you under this License. If your rights have been terminated and not permanently reinstated, you do not qualify to receive new licenses for the same material under section 10.
+9. Acceptance Not Required for Having Copies.
+
+You are not required to accept this License in order to receive or run a copy of the Program. Ancillary propagation of a covered work occurring solely as a consequence of using peer-to-peer transmission to receive a copy likewise does not require acceptance. However, nothing other than this License grants you permission to propagate or modify any covered work. These actions infringe copyright if you do not accept this License. Therefore, by modifying or propagating a covered work, you indicate your acceptance of this License to do so.
+10. Automatic Licensing of Downstream Recipients.
+
+Each time you convey a covered work, the recipient automatically receives a license from the original licensors, to run, modify and propagate that work, subject to this License. You are not responsible for enforcing compliance by third parties with this License.
+
+An "entity transaction" is a transaction transferring control of an organization, or substantially all assets of one, or subdividing an organization, or merging organizations. If propagation of a covered work results from an entity transaction, each party to that transaction who receives a copy of the work also receives whatever licenses to the work the party's predecessor in interest had or could give under the previous paragraph, plus a right to possession of the Corresponding Source of the work from the predecessor in interest, if the predecessor has it or can get it with reasonable efforts.
+
+You may not impose any further restrictions on the exercise of the rights granted or affirmed under this License. For example, you may not impose a license fee, royalty, or other charge for exercise of rights granted under this License, and you may not initiate litigation (including a cross-claim or counterclaim in a lawsuit) alleging that any patent claim is infringed by making, using, selling, offering for sale, or importing the Program or any portion of it.
+11. Patents.
+
+A "contributor" is a copyright holder who authorizes use under this License of the Program or a work on which the Program is based. The work thus licensed is called the contributor's "contributor version".
+
+A contributor's "essential patent claims" are all patent claims owned or controlled by the contributor, whether already acquired or hereafter acquired, that would be infringed by some manner, permitted by this License, of making, using, or selling its contributor version, but do not include claims that would be infringed only as a consequence of further modification of the contributor version. For purposes of this definition, "control" includes the right to grant patent sublicenses in a manner consistent with the requirements of this License.
+
+Each contributor grants you a non-exclusive, worldwide, royalty-free patent license under the contributor's essential patent claims, to make, use, sell, offer for sale, import and otherwise run, modify and propagate the contents of its contributor version.
+
+In the following three paragraphs, a "patent license" is any express agreement or commitment, however denominated, not to enforce a patent (such as an express permission to practice a patent or covenant not to sue for patent infringement). To "grant" such a patent license to a party means to make such an agreement or commitment not to enforce a patent against the party.
+
+If you convey a covered work, knowingly relying on a patent license, and the Corresponding Source of the work is not available for anyone to copy, free of charge and under the terms of this License, through a publicly available network server or other readily accessible means, then you must either (1) cause the Corresponding Source to be so available, or (2) arrange to deprive yourself of the benefit of the patent license for this particular work, or (3) arrange, in a manner consistent with the requirements of this License, to extend the patent license to downstream recipients. "Knowingly relying" means you have actual knowledge that, but for the patent license, your conveying the covered work in a country, or your recipient's use of the covered work in a country, would infringe one or more identifiable patents in that country that you have reason to believe are valid.
+
+If, pursuant to or in connection with a single transaction or arrangement, you convey, or propagate by procuring conveyance of, a covered work, and grant a patent license to some of the parties receiving the covered work authorizing them to use, propagate, modify or convey a specific copy of the covered work, then the patent license you grant is automatically extended to all recipients of the covered work and works based on it.
+
+A patent license is "discriminatory" if it does not include within the scope of its coverage, prohibits the exercise of, or is conditioned on the non-exercise of one or more of the rights that are specifically granted under this License. You may not convey a covered work if you are a party to an arrangement with a third party that is in the business of distributing software, under which you make payment to the third party based on the extent of your activity of conveying the work, and under which the third party grants, to any of the parties who would receive the covered work from you, a discriminatory patent license (a) in connection with copies of the covered work conveyed by you (or copies made from those copies), or (b) primarily for and in connection with specific products or compilations that contain the covered work, unless you entered into that arrangement, or that patent license was granted, prior to 28 March 2007.
+
+Nothing in this License shall be construed as excluding or limiting any implied license or other defenses to infringement that may otherwise be available to you under applicable patent law.
+12. No Surrender of Others' Freedom.
+
+If conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot convey a covered work so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not convey it at all. For example, if you agree to terms that obligate you to collect a royalty for further conveying from those to whom you convey the Program, the only way you could satisfy both those terms and this License would be to refrain entirely from conveying the Program.
+13. Remote Network Interaction; Use with the GNU General Public License.
+
+Notwithstanding any other provision of this License, if you modify the Program, your modified version must prominently offer all users interacting with it remotely through a computer network (if your version supports such interaction) an opportunity to receive the Corresponding Source of your version by providing access to the Corresponding Source from a network server at no charge, through some standard or customary means of facilitating copying of software. This Corresponding Source shall include the Corresponding Source for any work covered by version 3 of the GNU General Public License that is incorporated pursuant to the following paragraph.
+
+Notwithstanding any other provision of this License, you have permission to link or combine any covered work with a work licensed under version 3 of the GNU General Public License into a single combined work, and to convey the resulting work. The terms of this License will continue to apply to the part which is the covered work, but the work with which it is combined will remain governed by version 3 of the GNU General Public License.
+14. Revised Versions of this License.
+
+The Free Software Foundation may publish revised and/or new versions of the GNU Affero General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Program specifies that a certain numbered version of the GNU Affero General Public License "or any later version" applies to it, you have the option of following the terms and conditions either of that numbered version or of any later version published by the Free Software Foundation. If the Program does not specify a version number of the GNU Affero General Public License, you may choose any version ever published by the Free Software Foundation.
+
+If the Program specifies that a proxy can decide which future versions of the GNU Affero General Public License can be used, that proxy's public statement of acceptance of a version permanently authorizes you to choose that version for the Program.
+
+Later license versions may give you additional or different permissions. However, no additional obligations are imposed on any author or copyright holder as a result of your choosing to follow a later version.
+15. Disclaimer of Warranty.
+
+THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+16. Limitation of Liability.
+
+IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
+17. Interpretation of Sections 15 and 16.
+
+If the disclaimer of warranty and limitation of liability provided above cannot be given local legal effect according to their terms, reviewing courts shall apply local law that most closely approximates an absolute waiver of all civil liability in connection with the Program, unless a warranty or assumption of liability accompanies a copy of the Program in return for a fee.
+
+END OF TERMS AND CONDITIONS
```

### Comparing `nobinobi-staff-0.1.6.8/README.rst` & `nobinobi-staff-0.1.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/__init__.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,9 +5,9 @@
 #  License, or (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Affero General Public License for more details.
 
-__version__ = "0.1.6.8"
+__version__ = "0.1.6.9"
 default_app_config = 'nobinobi_staff.apps.NobinobiStaffConfig'
```

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/admin.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/admin.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/apps.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/apps.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/fixtures/staff_absence_type_fr-CH.json` & `nobinobi-staff-0.1.6.9/nobinobi_staff/fixtures/staff_absence_type_fr-CH.json`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/forms.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/forms.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr/LC_MESSAGES/django.mo` & `nobinobi-staff-0.1.6.9/nobinobi_staff/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr_CH/LC_MESSAGES/django.mo` & `nobinobi-staff-0.1.6.9/nobinobi_staff/locale/fr_CH/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/management/__init__.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/management/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/management/commands/__init__.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/management/commands/generate_training.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/management/commands/generate_training.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/management/commands/update_training.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/management/commands/update_training.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0001_initial.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0002_auto_20181019_1017.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0002_auto_20181019_1017.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0003_auto_20181022_1101.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0003_auto_20181022_1101.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0004_team_order.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0004_team_order.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0005_auto_20181116_0815.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0005_auto_20181116_0815.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0006_staff_working_base.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0006_staff_working_base.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0007_auto_20200221_1138.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0007_auto_20200221_1138.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0008_add_partial_disability.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0008_add_partial_disability.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0009_auto_20200805_1143.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0009_auto_20200805_1143.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0010_auto_20201029_1500.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/0010_auto_20201029_1500.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/__init__.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/models.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/models.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/serializers.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/serializers.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/signals.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/signals.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/static/css/nobinobi_staff.css` & `nobinobi-staff-0.1.6.9/nobinobi_staff/static/css/nobinobi_staff.css`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/static/js/nobinobi_staff.js` & `nobinobi-staff-0.1.6.9/nobinobi_staff/static/js/nobinobi_staff.js`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/tests.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/tests.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/urls.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/urls.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff/views.py` & `nobinobi-staff-0.1.6.9/nobinobi_staff/views.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/SOURCES.txt` & `nobinobi-staff-0.1.6.9/nobinobi_staff.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 nobinobi_staff/views.py
 nobinobi_staff.egg-info/PKG-INFO
 nobinobi_staff.egg-info/SOURCES.txt
 nobinobi_staff.egg-info/dependency_links.txt
 nobinobi_staff.egg-info/not-zip-safe
 nobinobi_staff.egg-info/requires.txt
 nobinobi_staff.egg-info/top_level.txt
-nobinobi_staff/fixtures/staff_absence_type_en-US.json
+nobinobi_staff/fixtures/staff_absence_type_en-us.json
 nobinobi_staff/fixtures/staff_absence_type_fr-CH.json
 nobinobi_staff/locale/de/LC_MESSAGES/django.mo
 nobinobi_staff/locale/en/LC_MESSAGES/django.mo
 nobinobi_staff/locale/fr/LC_MESSAGES/django.mo
 nobinobi_staff/locale/fr_CH/LC_MESSAGES/django.mo
 nobinobi_staff/locale/it/LC_MESSAGES/django.mo
 nobinobi_staff/management/__init__.py
```

### Comparing `nobinobi-staff-0.1.6.8/requirements_dev.txt` & `nobinobi-staff-0.1.6.9/requirements_dev.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-invoke==1.6.0
-twine==3.7.1
-zest.releaser==6.22.2
-
-wheel==0.37.0
-django-model-utils==4.2.0
-
-Werkzeug==2.0.2  # https://github.com/pallets/werkzeug
-ipdb==0.13.9  # https://github.com/gotcha/ipdb
-
-# Code quality
-# ------------------------------------------------------------------------------
-flake8==4.0.1  # https://github.com/PyCQA/flake8
-coverage==5.5  # https://github.com/nedbat/coveragepy
-
-# Django
-# ------------------------------------------------------------------------------
-factory-boy==3.2.0  # https://github.com/FactoryBoy/factory_boy
-django-test-plus==2.2.0  # https://github.com/revsys/django-test-plus
-
-django-debug-toolbar==3.2.2  # https://github.com/jazzband/django-debug-toolbar
-pytest-django==4.4.0  # https://github.com/pytest-dev/pytest-django
+invoke==2.1.2
+twine==4.0.2
+zest.releaser==8.0.0
+
+wheel==0.40.0
+django-model-utils==4.3.1
+
+Werkzeug==2.3.6  # https://github.com/pallets/werkzeug
+ipdb==0.13.13  # https://github.com/gotcha/ipdb
+
+# Code quality
+# ------------------------------------------------------------------------------
+flake8==6.0.0  # https://github.com/PyCQA/flake8
+coverage==7.2.7  # https://github.com/nedbat/coveragepy
+
+# Django
+# ------------------------------------------------------------------------------
+factory-boy==3.2.1  # https://github.com/FactoryBoy/factory_boy
+django-test-plus==2.2.1  # https://github.com/revsys/django-test-plus
+
+django-debug-toolbar==4.1.0  # https://github.com/jazzband/django-debug-toolbar
+pytest-django==4.5.2  # https://github.com/pytest-dev/pytest-django
```

### Comparing `nobinobi-staff-0.1.6.8/setup.py` & `nobinobi-staff-0.1.6.9/setup.py`

 * *Files identical despite different names*

