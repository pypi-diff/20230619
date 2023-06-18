# Comparing `tmp/django_simple_forms-0.1.4.tar.gz` & `tmp/django_simple_forms-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_simple_forms-0.1.4.tar", last modified: Sun Jun 18 22:51:10 2023, max compression
+gzip compressed data, was "django_simple_forms-0.1.5.tar", last modified: Sun Jun 18 23:18:20 2023, max compression
```

## Comparing `django_simple_forms-0.1.4.tar` & `django_simple_forms-0.1.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.215525 django_simple_forms-0.1.4/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1063 2022-12-24 16:53:50.000000 django_simple_forms-0.1.4/LICENSE
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      132 2020-11-25 20:09:02.000000 django_simple_forms-0.1.4/MANIFEST.in
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6048 2023-06-18 22:51:10.215603 django_simple_forms-0.1.4/PKG-INFO
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     5075 2022-12-03 11:56:53.000000 django_simple_forms-0.1.4/README.rst
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.206537 django_simple_forms-0.1.4/django_simple_forms/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)       55 2020-03-13 19:52:39.000000 django_simple_forms-0.1.4/django_simple_forms/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    28509 2022-10-25 00:07:24.000000 django_simple_forms-0.1.4/django_simple_forms/admin.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      187 2021-05-13 20:01:43.000000 django_simple_forms-0.1.4/django_simple_forms/apps.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     3688 2022-12-03 11:34:51.000000 django_simple_forms-0.1.4/django_simple_forms/forms.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.207749 django_simple_forms-0.1.4/django_simple_forms/management/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2017-08-21 13:49:56.000000 django_simple_forms-0.1.4/django_simple_forms/management/__init__.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.208437 django_simple_forms-0.1.4/django_simple_forms/management/commands/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2017-08-21 13:49:56.000000 django_simple_forms-0.1.4/django_simple_forms/management/commands/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      879 2022-09-13 13:39:05.000000 django_simple_forms-0.1.4/django_simple_forms/management/commands/delete_expired_responses.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      340 2022-09-08 16:57:08.000000 django_simple_forms-0.1.4/django_simple_forms/management/commands/delete_unused_addresses.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      636 2021-01-27 18:01:44.000000 django_simple_forms-0.1.4/django_simple_forms/management/commands/forms_import_sites.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.208922 django_simple_forms-0.1.4/django_simple_forms/migrations/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    15282 2022-12-03 11:20:36.000000 django_simple_forms-0.1.4/django_simple_forms/migrations/0001_initial.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2020-11-16 20:10:59.000000 django_simple_forms-0.1.4/django_simple_forms/migrations/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    26775 2022-12-03 11:33:21.000000 django_simple_forms-0.1.4/django_simple_forms/models.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      381 2020-03-07 20:39:02.000000 django_simple_forms-0.1.4/django_simple_forms/runtests.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.209031 django_simple_forms-0.1.4/django_simple_forms/static/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2022-08-11 18:16:52.000000 django_simple_forms-0.1.4/django_simple_forms/static/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.209267 django_simple_forms-0.1.4/django_simple_forms/static/admin/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-20 21:01:11.000000 django_simple_forms-0.1.4/django_simple_forms/static/admin/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.209814 django_simple_forms-0.1.4/django_simple_forms/static/admin/css/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      113 2022-08-26 11:26:25.000000 django_simple_forms-0.1.4/django_simple_forms/static/admin/css/delete_button.css
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      684 2022-08-26 11:11:09.000000 django_simple_forms-0.1.4/django_simple_forms/static/admin/css/django_simple_forms.css
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.210017 django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     8196 2020-11-25 15:13:25.000000 django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.210268 django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/external/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-25 15:13:21.000000 django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/external/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.210669 django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/external/css/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-25 15:13:30.000000 django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/external/css/.DS_Store
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2507 2022-08-19 10:18:57.000000 django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/external/css/form_style.css
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.210932 django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/internal/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2022-08-11 17:15:02.000000 django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/internal/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.211413 django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/internal/css/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2022-08-11 18:16:52.000000 django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/internal/css/.DS_Store
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1742 2022-08-11 20:10:24.000000 django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/internal/css/post_html.css
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.211707 django_simple_forms-0.1.4/django_simple_forms/templates/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2022-10-13 19:03:38.000000 django_simple_forms-0.1.4/django_simple_forms/templates/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.211960 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2020-11-25 15:18:01.000000 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.212229 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/external/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-25 15:18:06.000000 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/external/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.212693 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/external/pages/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1471 2022-10-11 20:33:41.000000 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/external/pages/form_page.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      393 2021-04-21 22:11:13.000000 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/external/pages/form_submitted.html
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.213226 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2022-08-11 17:13:43.000000 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.213683 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/emails/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2028 2022-10-16 18:37:40.000000 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/emails/form_email.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      319 2022-10-16 18:49:33.000000 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/emails/form_email.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      477 2022-10-13 18:59:37.000000 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/internal_base.html
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.214518 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/pages/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-01-19 16:10:11.000000 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/pages/.DS_Store
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      815 2022-10-13 19:20:58.000000 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/pages/post_form.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2082 2022-10-16 18:38:52.000000 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/pages/post_view.html
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.214742 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/pdfs/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1021 2022-10-16 19:13:03.000000 django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/pdfs/default_pdf.html
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.215314 django_simple_forms-0.1.4/django_simple_forms/tests/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_forms-0.1.4/django_simple_forms/tests/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1811 2022-12-03 11:21:14.000000 django_simple_forms-0.1.4/django_simple_forms/tests/settings.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      274 2022-12-03 11:22:49.000000 django_simple_forms-0.1.4/django_simple_forms/tests/urls.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1699 2022-08-12 21:41:33.000000 django_simple_forms-0.1.4/django_simple_forms/urls.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    21187 2022-12-04 19:19:33.000000 django_simple_forms-0.1.4/django_simple_forms/views.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:51:10.207519 django_simple_forms-0.1.4/django_simple_forms.egg-info/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6048 2023-06-18 22:51:10.000000 django_simple_forms-0.1.4/django_simple_forms.egg-info/PKG-INFO
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2664 2023-06-18 22:51:10.000000 django_simple_forms-0.1.4/django_simple_forms.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2023-06-18 22:51:10.000000 django_simple_forms-0.1.4/django_simple_forms.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      129 2023-06-18 22:51:10.000000 django_simple_forms-0.1.4/django_simple_forms.egg-info/requires.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)       20 2023-06-18 22:51:10.000000 django_simple_forms-0.1.4/django_simple_forms.egg-info/top_level.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2021-04-01 21:42:55.000000 django_simple_forms-0.1.4/django_simple_forms.egg-info/zip-safe
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1092 2023-06-18 22:51:10.215947 django_simple_forms-0.1.4/setup.cfg
--rw-r--r--   0 jonathanrickard   (501) staff       (20)       39 2021-04-01 21:48:14.000000 django_simple_forms-0.1.4/setup.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.376188 django_simple_forms-0.1.5/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1063 2022-12-24 16:53:50.000000 django_simple_forms-0.1.5/LICENSE
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      132 2020-11-25 20:09:02.000000 django_simple_forms-0.1.5/MANIFEST.in
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6048 2023-06-18 23:18:20.376269 django_simple_forms-0.1.5/PKG-INFO
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     5075 2022-12-03 11:56:53.000000 django_simple_forms-0.1.5/README.rst
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.367447 django_simple_forms-0.1.5/django_simple_forms/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)       55 2020-03-13 19:52:39.000000 django_simple_forms-0.1.5/django_simple_forms/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    28509 2022-10-25 00:07:24.000000 django_simple_forms-0.1.5/django_simple_forms/admin.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      187 2021-05-13 20:01:43.000000 django_simple_forms-0.1.5/django_simple_forms/apps.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     3688 2022-12-03 11:34:51.000000 django_simple_forms-0.1.5/django_simple_forms/forms.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.368603 django_simple_forms-0.1.5/django_simple_forms/management/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2017-08-21 13:49:56.000000 django_simple_forms-0.1.5/django_simple_forms/management/__init__.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.369262 django_simple_forms-0.1.5/django_simple_forms/management/commands/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2017-08-21 13:49:56.000000 django_simple_forms-0.1.5/django_simple_forms/management/commands/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      879 2022-09-13 13:39:05.000000 django_simple_forms-0.1.5/django_simple_forms/management/commands/delete_expired_responses.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      340 2022-09-08 16:57:08.000000 django_simple_forms-0.1.5/django_simple_forms/management/commands/delete_unused_addresses.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      636 2021-01-27 18:01:44.000000 django_simple_forms-0.1.5/django_simple_forms/management/commands/forms_import_sites.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.369721 django_simple_forms-0.1.5/django_simple_forms/migrations/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    15282 2022-12-03 11:20:36.000000 django_simple_forms-0.1.5/django_simple_forms/migrations/0001_initial.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2020-11-16 20:10:59.000000 django_simple_forms-0.1.5/django_simple_forms/migrations/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    26775 2022-12-03 11:33:21.000000 django_simple_forms-0.1.5/django_simple_forms/models.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      381 2020-03-07 20:39:02.000000 django_simple_forms-0.1.5/django_simple_forms/runtests.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.369828 django_simple_forms-0.1.5/django_simple_forms/static/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2022-08-11 18:16:52.000000 django_simple_forms-0.1.5/django_simple_forms/static/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.370068 django_simple_forms-0.1.5/django_simple_forms/static/admin/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-20 21:01:11.000000 django_simple_forms-0.1.5/django_simple_forms/static/admin/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.370679 django_simple_forms-0.1.5/django_simple_forms/static/admin/css/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      113 2022-08-26 11:26:25.000000 django_simple_forms-0.1.5/django_simple_forms/static/admin/css/delete_button.css
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      684 2022-08-26 11:11:09.000000 django_simple_forms-0.1.5/django_simple_forms/static/admin/css/django_simple_forms.css
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.370949 django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     8196 2020-11-25 15:13:25.000000 django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.371241 django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/external/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-25 15:13:21.000000 django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/external/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.371703 django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/external/css/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-25 15:13:30.000000 django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/external/css/.DS_Store
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2507 2022-08-19 10:18:57.000000 django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/external/css/form_style.css
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.372008 django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/internal/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2022-08-11 17:15:02.000000 django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/internal/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.372552 django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/internal/css/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2022-08-11 18:16:52.000000 django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/internal/css/.DS_Store
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1742 2022-08-11 20:10:24.000000 django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/internal/css/post_html.css
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.372797 django_simple_forms-0.1.5/django_simple_forms/templates/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2022-10-13 19:03:38.000000 django_simple_forms-0.1.5/django_simple_forms/templates/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.373042 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2020-11-25 15:18:01.000000 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.373206 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/external/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-25 15:18:06.000000 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/external/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.373625 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/external/pages/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1471 2022-10-11 20:33:41.000000 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/external/pages/form_page.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      393 2021-04-21 22:11:13.000000 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/external/pages/form_submitted.html
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.374208 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2022-08-11 17:13:43.000000 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.374685 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/emails/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2028 2022-10-16 18:37:40.000000 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/emails/form_email.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      319 2022-10-16 18:49:33.000000 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/emails/form_email.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      477 2022-10-13 18:59:37.000000 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/internal_base.html
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.375289 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/pages/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-01-19 16:10:11.000000 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/pages/.DS_Store
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      815 2022-10-13 19:20:58.000000 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/pages/post_form.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2082 2022-10-16 18:38:52.000000 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/pages/post_view.html
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.375460 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/pdfs/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1021 2022-10-16 19:13:03.000000 django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/pdfs/default_pdf.html
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.376008 django_simple_forms-0.1.5/django_simple_forms/tests/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_forms-0.1.5/django_simple_forms/tests/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1811 2022-12-03 11:21:14.000000 django_simple_forms-0.1.5/django_simple_forms/tests/settings.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      274 2022-12-03 11:22:49.000000 django_simple_forms-0.1.5/django_simple_forms/tests/urls.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1699 2022-08-12 21:41:33.000000 django_simple_forms-0.1.5/django_simple_forms/urls.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    21187 2022-12-04 19:19:33.000000 django_simple_forms-0.1.5/django_simple_forms/views.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:18:20.368385 django_simple_forms-0.1.5/django_simple_forms.egg-info/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6048 2023-06-18 23:18:20.000000 django_simple_forms-0.1.5/django_simple_forms.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2664 2023-06-18 23:18:20.000000 django_simple_forms-0.1.5/django_simple_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2023-06-18 23:18:20.000000 django_simple_forms-0.1.5/django_simple_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      134 2023-06-18 23:18:20.000000 django_simple_forms-0.1.5/django_simple_forms.egg-info/requires.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)       20 2023-06-18 23:18:20.000000 django_simple_forms-0.1.5/django_simple_forms.egg-info/top_level.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2021-04-01 21:42:55.000000 django_simple_forms-0.1.5/django_simple_forms.egg-info/zip-safe
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1098 2023-06-18 23:18:20.376542 django_simple_forms-0.1.5/setup.cfg
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)       39 2021-04-01 21:48:14.000000 django_simple_forms-0.1.5/setup.py
```

### Comparing `django_simple_forms-0.1.4/LICENSE` & `django_simple_forms-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/PKG-INFO` & `django_simple_forms-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_simple_forms
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Django app for creating forms
 Home-page: https://github.com/jonathanrickard
 Author: Jonathan Rickard
 Author-email: jonathan@jonathanrickard.com
 License: MIT License
 Keywords: django,forms
 Platform: UNKNOWN
```

### Comparing `django_simple_forms-0.1.4/README.rst` & `django_simple_forms-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/admin.py` & `django_simple_forms-0.1.5/django_simple_forms/admin.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/forms.py` & `django_simple_forms-0.1.5/django_simple_forms/forms.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/management/commands/delete_expired_responses.py` & `django_simple_forms-0.1.5/django_simple_forms/management/commands/delete_expired_responses.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/management/commands/forms_import_sites.py` & `django_simple_forms-0.1.5/django_simple_forms/management/commands/forms_import_sites.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/migrations/0001_initial.py` & `django_simple_forms-0.1.5/django_simple_forms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/models.py` & `django_simple_forms-0.1.5/django_simple_forms/models.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/static/.DS_Store` & `django_simple_forms-0.1.5/django_simple_forms/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/static/admin/.DS_Store` & `django_simple_forms-0.1.5/django_simple_forms/static/admin/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/static/admin/css/django_simple_forms.css` & `django_simple_forms-0.1.5/django_simple_forms/static/admin/css/django_simple_forms.css`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/.DS_Store` & `django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/external/.DS_Store` & `django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/external/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/external/css/.DS_Store` & `django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/external/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/external/css/form_style.css` & `django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/external/css/form_style.css`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/internal/.DS_Store` & `django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/internal/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/internal/css/.DS_Store` & `django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/internal/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/static/django_simple_forms/internal/css/post_html.css` & `django_simple_forms-0.1.5/django_simple_forms/static/django_simple_forms/internal/css/post_html.css`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/templates/.DS_Store` & `django_simple_forms-0.1.5/django_simple_forms/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/.DS_Store` & `django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/external/.DS_Store` & `django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/external/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/external/pages/form_page.html` & `django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/external/pages/form_page.html`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/.DS_Store` & `django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/emails/form_email.html` & `django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/emails/form_email.html`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/pages/.DS_Store` & `django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/pages/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/pages/post_form.html` & `django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/pages/post_form.html`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/pages/post_view.html` & `django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/pages/post_view.html`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/templates/django_simple_forms/internal/pdfs/default_pdf.html` & `django_simple_forms-0.1.5/django_simple_forms/templates/django_simple_forms/internal/pdfs/default_pdf.html`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/tests/settings.py` & `django_simple_forms-0.1.5/django_simple_forms/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/urls.py` & `django_simple_forms-0.1.5/django_simple_forms/urls.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms/views.py` & `django_simple_forms-0.1.5/django_simple_forms/views.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/django_simple_forms.egg-info/PKG-INFO` & `django_simple_forms-0.1.5/django_simple_forms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-forms
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Django app for creating forms
 Home-page: https://github.com/jonathanrickard
 Author: Jonathan Rickard
 Author-email: jonathan@jonathanrickard.com
 License: MIT License
 Keywords: django,forms
 Platform: UNKNOWN
```

### Comparing `django_simple_forms-0.1.4/django_simple_forms.egg-info/SOURCES.txt` & `django_simple_forms-0.1.5/django_simple_forms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.4/setup.cfg` & `django_simple_forms-0.1.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_simple_forms
-version = 0.1.4
+version = 0.1.5
 author = Jonathan Rickard
 author_email = jonathan@jonathanrickard.com
 license = MIT License
 description = A Django app for creating forms
 keywords = django, forms
 url = https://github.com/jonathanrickard
 long_description = file: README.rst
@@ -27,15 +27,15 @@
 
 [options]
 packages = find:
 include_package_data = True
 zip_safe = True
 install_requires = 
 	Django >= 3.2, < 5.0
-	django-admin-sortable2 >= 1.0
+	django-admin-sortable2 >= 1.0, <2.0
 	django-ckeditor >= 6.1
 	django-simple-file-handler >= 0.3
 	requests >= 2.28
 	xlsxwriter >= 3.0
 
 [egg_info]
 tag_build =
```

