# Comparing `tmp/django_simple_bulk_emailer-0.2.2.tar.gz` & `tmp/django_simple_bulk_emailer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_simple_bulk_emailer-0.2.2.tar", last modified: Sun Jun 18 22:03:46 2023, max compression
+gzip compressed data, was "django_simple_bulk_emailer-0.2.3.tar", last modified: Sun Jun 18 23:19:47 2023, max compression
```

## Comparing `django_simple_bulk_emailer-0.2.2.tar` & `django_simple_bulk_emailer-0.2.3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.993489 django_simple_bulk_emailer-0.2.2/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1063 2022-12-24 16:53:32.000000 django_simple_bulk_emailer-0.2.2/LICENSE
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      146 2019-02-05 21:19:31.000000 django_simple_bulk_emailer-0.2.2/MANIFEST.in
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    23335 2023-06-18 22:03:46.993620 django_simple_bulk_emailer-0.2.2/PKG-INFO
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    22324 2021-08-25 17:13:53.000000 django_simple_bulk_emailer-0.2.2/README.rst
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.980049 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2021-08-11 17:05:58.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    11544 2021-08-25 16:22:17.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/admin.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      284 2021-05-13 20:01:20.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/apps.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2134 2019-12-10 18:56:05.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/forms.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.981424 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/__init__.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.983154 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/commands/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/commands/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      401 2020-03-07 20:24:25.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/commands/delete_expired_emails.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      835 2021-08-03 14:29:15.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/commands/delete_expired_stats.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      527 2020-03-07 20:24:54.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/commands/delete_unsubscribed_users.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      621 2019-12-09 19:45:53.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/commands/import_sites.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     4696 2022-04-07 19:58:41.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/commands/send_bulk_email.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     4866 2022-04-07 20:26:28.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/commands/sync_mailchimp.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6788 2022-04-07 20:04:04.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/commands/update_email_stats.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.984519 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/migrations/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     9299 2021-07-02 21:15:25.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/migrations/0001_initial.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     4870 2021-08-12 20:36:15.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/migrations/0002_auto_20210812_1535.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1027 2021-08-24 19:06:30.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/migrations/0003_auto_20210824_1148.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      378 2023-06-18 21:52:50.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/migrations/0004_bulkemail_update_datetime.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2020-03-07 21:10:04.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/migrations/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    13663 2022-11-09 17:49:03.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/models.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      381 2020-03-07 20:39:02.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/runtests.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.984733 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/signals/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-09-25 21:02:03.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/signals/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2780 2020-03-03 19:58:58.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/signals/handlers.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.984911 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-02-07 19:17:46.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.976804 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/admin/
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.985066 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/admin/css/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      534 2021-08-12 16:53:21.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/admin/css/django_simple_bulk_emailer.css
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.985352 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-05-28 19:27:20.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.985849 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2607 2022-01-07 11:59:32.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/django_simple_bulk_emailer.css
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      122 2021-08-11 21:19:35.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/django_simple_bulk_emailer_preview.css
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.986366 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-05-28 19:18:58.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/.DS_Store
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2166 2021-05-26 21:55:30.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/file_icon_64x64.png
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.986747 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-04-24 18:58:47.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/.DS_Store
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      582 2021-05-28 19:55:32.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/django_simple_bulk_emailer.js
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.986961 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2021-05-28 18:19:58.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.987201 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-06-06 22:04:10.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.987351 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-05-28 19:18:24.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.987820 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     5347 2022-11-09 17:30:24.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_html.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      843 2022-11-09 17:30:08.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_text.txt
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.988414 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-03-29 13:50:42.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/.DS_Store
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2658 2021-08-24 16:38:59.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/list_view.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     4100 2022-11-09 17:29:10.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/page_view.html
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.988639 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-08-09 18:56:49.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.989061 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      356 2019-03-28 18:47:23.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/bulk_email_send.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      681 2019-03-27 19:36:44.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/subscribe_email_html.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      329 2019-08-22 20:13:23.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/subscribe_email_text.txt
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.990832 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-08-25 17:58:15.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/.DS_Store
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1831 2021-08-13 19:05:49.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/bulk_email_preview.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2314 2021-08-13 19:07:02.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      587 2021-08-13 19:10:22.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions_error.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      488 2021-08-13 19:10:22.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions_success.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      688 2021-08-13 19:10:54.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/quick_unsubscribe.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1882 2021-08-13 19:11:26.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      522 2021-08-13 19:03:43.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe_success.html
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.993339 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/tests/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/tests/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    27447 2023-06-18 21:48:41.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/tests/functions.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1888 2020-03-04 20:25:13.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/tests/settings.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    43095 2022-04-07 20:51:24.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/tests/test_commands.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     4320 2022-04-07 19:10:54.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/tests/test_forms.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    12277 2021-08-24 15:43:34.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/tests/test_models.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    50205 2022-04-07 19:30:56.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/tests/test_views.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      280 2020-01-09 17:21:22.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/tests/urls.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1374 2021-07-13 14:59:06.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/urls.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    19904 2022-04-07 20:13:05.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/views.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 22:03:46.981050 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer.egg-info/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    23335 2023-06-18 22:03:46.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer.egg-info/PKG-INFO
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     4660 2023-06-18 22:03:46.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2023-06-18 22:03:46.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      141 2023-06-18 22:03:46.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer.egg-info/requires.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)       27 2023-06-18 22:03:46.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer.egg-info/top_level.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2021-08-25 18:06:31.000000 django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer.egg-info/zip-safe
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1145 2023-06-18 22:03:46.993938 django_simple_bulk_emailer-0.2.2/setup.cfg
--rw-r--r--   0 jonathanrickard   (501) staff       (20)       39 2021-04-01 21:33:59.000000 django_simple_bulk_emailer-0.2.2/setup.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.401572 django_simple_bulk_emailer-0.2.3/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1063 2022-12-24 16:53:32.000000 django_simple_bulk_emailer-0.2.3/LICENSE
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      146 2019-02-05 21:19:31.000000 django_simple_bulk_emailer-0.2.3/MANIFEST.in
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    23335 2023-06-18 23:19:47.401666 django_simple_bulk_emailer-0.2.3/PKG-INFO
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    22324 2021-08-25 17:13:53.000000 django_simple_bulk_emailer-0.2.3/README.rst
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.387520 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2021-08-11 17:05:58.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    11544 2021-08-25 16:22:17.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/admin.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      284 2021-05-13 20:01:20.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/apps.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2134 2019-12-10 18:56:05.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/forms.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.388707 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/__init__.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.390544 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/commands/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/commands/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      401 2020-03-07 20:24:25.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/commands/delete_expired_emails.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      835 2021-08-03 14:29:15.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/commands/delete_expired_stats.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      527 2020-03-07 20:24:54.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/commands/delete_unsubscribed_users.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      621 2019-12-09 19:45:53.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/commands/import_sites.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     4696 2022-04-07 19:58:41.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/commands/send_bulk_email.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     4866 2022-04-07 20:26:28.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/commands/sync_mailchimp.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6788 2022-04-07 20:04:04.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/commands/update_email_stats.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.391907 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/migrations/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     9299 2021-07-02 21:15:25.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/migrations/0001_initial.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     4870 2021-08-12 20:36:15.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/migrations/0002_auto_20210812_1535.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1027 2021-08-24 19:06:30.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/migrations/0003_auto_20210824_1148.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      378 2023-06-18 21:52:50.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/migrations/0004_bulkemail_update_datetime.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2020-03-07 21:10:04.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/migrations/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    13663 2022-11-09 17:49:03.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/models.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      381 2020-03-07 20:39:02.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/runtests.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.392078 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/signals/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-09-25 21:02:03.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/signals/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2780 2020-03-03 19:58:58.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/signals/handlers.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.392217 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-02-07 19:17:46.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.383505 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/admin/
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.392359 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/admin/css/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      534 2021-08-12 16:53:21.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/admin/css/django_simple_bulk_emailer.css
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.392611 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-05-28 19:27:20.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.393315 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2607 2022-01-07 11:59:32.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/django_simple_bulk_emailer.css
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      122 2021-08-11 21:19:35.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/django_simple_bulk_emailer_preview.css
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.393782 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-05-28 19:18:58.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/.DS_Store
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2166 2021-05-26 21:55:30.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/file_icon_64x64.png
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.394546 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-04-24 18:58:47.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/.DS_Store
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      582 2021-05-28 19:55:32.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/django_simple_bulk_emailer.js
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.394831 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2021-05-28 18:19:58.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.395049 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-06-06 22:04:10.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.395185 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-05-28 19:18:24.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.395645 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     5347 2022-11-09 17:30:24.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_html.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      843 2022-11-09 17:30:08.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_text.txt
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.396223 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-03-29 13:50:42.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/.DS_Store
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2658 2021-08-24 16:38:59.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/list_view.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     4100 2022-11-09 17:29:10.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/page_view.html
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.396533 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-08-09 18:56:49.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.396947 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      356 2019-03-28 18:47:23.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/bulk_email_send.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      681 2019-03-27 19:36:44.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/subscribe_email_html.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      329 2019-08-22 20:13:23.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/subscribe_email_text.txt
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.398776 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-08-25 17:58:15.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/.DS_Store
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1831 2021-08-13 19:05:49.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/bulk_email_preview.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2314 2021-08-13 19:07:02.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      587 2021-08-13 19:10:22.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions_error.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      488 2021-08-13 19:10:22.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions_success.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      688 2021-08-13 19:10:54.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/quick_unsubscribe.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1882 2021-08-13 19:11:26.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      522 2021-08-13 19:03:43.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe_success.html
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.401336 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/tests/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/tests/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    27447 2023-06-18 21:48:41.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/tests/functions.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1888 2020-03-04 20:25:13.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/tests/settings.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    43095 2022-04-07 20:51:24.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/tests/test_commands.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     4320 2022-04-07 19:10:54.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/tests/test_forms.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    12277 2021-08-24 15:43:34.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/tests/test_models.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    50205 2022-04-07 19:30:56.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/tests/test_views.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      280 2020-01-09 17:21:22.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/tests/urls.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1374 2021-07-13 14:59:06.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/urls.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    19904 2022-04-07 20:13:05.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/views.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 23:19:47.388479 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer.egg-info/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    23335 2023-06-18 23:19:47.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     4660 2023-06-18 23:19:47.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2023-06-18 23:19:47.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      146 2023-06-18 23:19:47.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer.egg-info/requires.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)       27 2023-06-18 23:19:47.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer.egg-info/top_level.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2021-08-25 18:06:31.000000 django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer.egg-info/zip-safe
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1151 2023-06-18 23:19:47.401955 django_simple_bulk_emailer-0.2.3/setup.cfg
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)       39 2021-04-01 21:33:59.000000 django_simple_bulk_emailer-0.2.3/setup.py
```

### Comparing `django_simple_bulk_emailer-0.2.2/LICENSE` & `django_simple_bulk_emailer-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/PKG-INFO` & `django_simple_bulk_emailer-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_simple_bulk_emailer
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Django app for sending bulk email
 Home-page: https://github.com/jonathanrickard/django-simple-bulk-emailer
 Author: Jonathan Rickard
 Author-email: jonathan@jonathanrickard.com
 License: MIT License
 Keywords: django,email
 Platform: UNKNOWN
```

### Comparing `django_simple_bulk_emailer-0.2.2/README.rst` & `django_simple_bulk_emailer-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/admin.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/admin.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/forms.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/forms.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/commands/delete_expired_stats.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/commands/delete_expired_stats.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/commands/delete_unsubscribed_users.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/commands/delete_unsubscribed_users.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/commands/import_sites.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/commands/import_sites.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/commands/send_bulk_email.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/commands/send_bulk_email.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/commands/sync_mailchimp.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/commands/sync_mailchimp.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/management/commands/update_email_stats.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/management/commands/update_email_stats.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/migrations/0001_initial.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/migrations/0002_auto_20210812_1535.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/migrations/0002_auto_20210812_1535.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/migrations/0003_auto_20210824_1148.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/migrations/0003_auto_20210824_1148.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/models.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/models.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/signals/handlers.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/.DS_Store` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/admin/css/django_simple_bulk_emailer.css` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/admin/css/django_simple_bulk_emailer.css`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/.DS_Store` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/django_simple_bulk_emailer.css` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/django_simple_bulk_emailer.css`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/.DS_Store` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/file_icon_64x64.png` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/file_icon_64x64.png`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/.DS_Store` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/django_simple_bulk_emailer.js` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/django_simple_bulk_emailer.js`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/.DS_Store` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/.DS_Store` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/.DS_Store` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_html.html` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_html.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_text.txt` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_text.txt`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/.DS_Store` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/list_view.html` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/list_view.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/page_view.html` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/page_view.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/.DS_Store` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/subscribe_email_html.html` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/subscribe_email_html.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/.DS_Store` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/bulk_email_preview.html` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/bulk_email_preview.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions.html` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions_error.html` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions_error.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/quick_unsubscribe.html` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/quick_unsubscribe.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe.html` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe_success.html` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe_success.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/tests/functions.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/tests/functions.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/tests/settings.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/tests/test_commands.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/tests/test_forms.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/tests/test_models.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/tests/test_views.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/urls.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/urls.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer/views.py` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer/views.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer.egg-info/PKG-INFO` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-bulk-emailer
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Django app for sending bulk email
 Home-page: https://github.com/jonathanrickard/django-simple-bulk-emailer
 Author: Jonathan Rickard
 Author-email: jonathan@jonathanrickard.com
 License: MIT License
 Keywords: django,email
 Platform: UNKNOWN
```

### Comparing `django_simple_bulk_emailer-0.2.2/django_simple_bulk_emailer.egg-info/SOURCES.txt` & `django_simple_bulk_emailer-0.2.3/django_simple_bulk_emailer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.2/setup.cfg` & `django_simple_bulk_emailer-0.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_simple_bulk_emailer
-version = 0.2.2
+version = 0.2.3
 author = Jonathan Rickard
 author_email = jonathan@jonathanrickard.com
 license = MIT License
 description = A Django app for sending bulk email
 keywords = django, email
 url = https://github.com/jonathanrickard/django-simple-bulk-emailer
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
 	django-ckeditor >= 6.2
 	django-simple-file-handler >= 0.3
 	mailchimp3 >= 3.0
 	Pillow >= 9.0
 	requests >= 2.27
 
 [egg_info]
```

