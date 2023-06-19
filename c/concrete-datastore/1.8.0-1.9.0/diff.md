# Comparing `tmp/concrete-datastore-1.8.0.tar.gz` & `tmp/concrete-datastore-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/concrete-datastore-1.8.0.tar", last modified: Tue Apr 28 13:58:43 2020, max compression
+gzip compressed data, was "dist/concrete-datastore-1.9.0.tar", last modified: Tue Jun 16 15:42:33 2020, max compression
```

## Comparing `concrete-datastore-1.8.0.tar` & `concrete-datastore-1.9.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/
--rw-r--r--   0 lco        (503) staff       (20)     4616 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/PKG-INFO
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore.egg-info/
--rw-r--r--   0 lco        (503) staff       (20)     4616 2020-04-28 13:58:42.000000 concrete-datastore-1.8.0/concrete_datastore.egg-info/PKG-INFO
--rw-r--r--   0 lco        (503) staff       (20)        1 2020-02-20 23:19:11.000000 concrete-datastore-1.8.0/concrete_datastore.egg-info/not-zip-safe
--rw-r--r--   0 lco        (503) staff       (20)     4100 2020-04-28 13:58:42.000000 concrete-datastore-1.8.0/concrete_datastore.egg-info/SOURCES.txt
--rw-r--r--   0 lco        (503) staff       (20)       95 2020-04-28 13:58:42.000000 concrete-datastore-1.8.0/concrete_datastore.egg-info/entry_points.txt
--rw-r--r--   0 lco        (503) staff       (20)      722 2020-04-28 13:58:42.000000 concrete-datastore-1.8.0/concrete_datastore.egg-info/requires.txt
--rw-r--r--   0 lco        (503) staff       (20)       37 2020-04-28 13:58:42.000000 concrete-datastore-1.8.0/concrete_datastore.egg-info/top_level.txt
--rw-r--r--   0 lco        (503) staff       (20)        1 2020-04-28 13:58:42.000000 concrete-datastore-1.8.0/concrete_datastore.egg-info/dependency_links.txt
--rw-r--r--   0 lco        (503) staff       (20)    35149 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/LICENSE
--rw-r--r--   0 lco        (503) staff       (20)      320 2020-02-21 17:55:37.000000 concrete-datastore-1.8.0/MANIFEST.in
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/settings/
--rw-r--r--   0 lco        (503) staff       (20)       16 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/settings/__init__.py
--rw-r--r--   0 lco        (503) staff       (20)     1533 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/settings/utils.py
--rw-r--r--   0 lco        (503) staff       (20)      748 2020-03-20 14:39:44.000000 concrete-datastore-1.8.0/concrete_datastore/settings/celery.py
--rw-r--r--   0 lco        (503) staff       (20)    14120 2020-04-28 13:58:25.000000 concrete-datastore-1.8.0/concrete_datastore/settings/base.py
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/parsers/
--rw-r--r--   0 lco        (503) staff       (20)     2659 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/parsers/models.py
--rw-r--r--   0 lco        (503) staff       (20)     1334 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/parsers/fields.py
--rw-r--r--   0 lco        (503) staff       (20)      416 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/parsers/validators.py
--rw-r--r--   0 lco        (503) staff       (20)     2445 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/parsers/constants.py
--rw-r--r--   0 lco        (503) staff       (20)     1219 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/parsers/loaders.py
--rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/parsers/__init__.py
--rw-r--r--   0 lco        (503) staff       (20)      255 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/parsers/parsers.py
--rw-r--r--   0 lco        (503) staff       (20)     4949 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/parsers/exceptions.py
--rw-r--r--   0 lco        (503) staff       (20)      322 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/parsers/helpers.py
--rw-r--r--   0 lco        (503) staff       (20)    17951 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/parsers/meta.py
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/migrations/
--rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/migrations/__init__.py
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/locale/
--rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/locale/.gitignore
--rw-r--r--   0 lco        (503) staff       (20)    30942 2020-04-28 13:58:25.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/models.py
--rw-r--r--   0 lco        (503) staff       (20)     1628 2020-03-03 20:02:09.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/constants.py
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/management/
--rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/management/__init__.py
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/management/commands/
--rw-r--r--   0 lco        (503) staff       (20)     4189 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/management/commands/openapispec.py
--rw-r--r--   0 lco        (503) staff       (20)      793 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/management/commands/create_superuser.py
--rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/management/commands/__init__.py
--rw-r--r--   0 lco        (503) staff       (20)     2247 2020-02-20 22:16:52.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/management/commands/create_superuser_with_email.py
--rw-r--r--   0 lco        (503) staff       (20)     1919 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/management/commands/init_app.py
--rw-r--r--   0 lco        (503) staff       (20)       81 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/__init__.py
--rw-r--r--   0 lco        (503) staff       (20)     2236 2020-03-20 09:26:06.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/apps.py
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/templates/
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/templates/admin/
--rw-r--r--   0 lco        (503) staff       (20)     3179 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/templates/admin/mfa-login.html
--rw-r--r--   0 lco        (503) staff       (20)     1611 2020-03-03 20:02:09.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/templates/admin/index.html
--rw-r--r--   0 lco        (503) staff       (20)      595 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/templates/admin/base.html
--rw-r--r--   0 lco        (503) staff       (20)      265 2020-03-03 20:02:09.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/templates/admin/change_list.html
--rw-r--r--   0 lco        (503) staff       (20)      436 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/templates/admin/add_form.html
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/templates/mainApp/
--rw-r--r--   0 lco        (503) staff       (20)     9043 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/templates/mainApp/index.html
--rw-r--r--   0 lco        (503) staff       (20)     1795 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/templates/mainApp/unsubscribe.html
--rw-r--r--   0 lco        (503) staff       (20)     9054 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/templates/mainApp/logged-using-oauth.html
--rw-r--r--   0 lco        (503) staff       (20)      465 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/templates/mainApp/unsubscribe_result.html
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/automation/
--rw-r--r--   0 lco        (503) staff       (20)      105 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/automation/signals.py
--rw-r--r--   0 lco        (503) staff       (20)      513 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/automation/tasks.py
--rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/automation/__init__.py
--rw-r--r--   0 lco        (503) staff       (20)     1271 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/automation/signal_processor.py
--rw-r--r--   0 lco        (503) staff       (20)     6553 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/password.py
--rw-r--r--   0 lco        (503) staff       (20)      827 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/urls.py
--rw-r--r--   0 lco        (503) staff       (20)      564 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/middleware.py
--rw-r--r--   0 lco        (503) staff       (20)     3379 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/views.py
--rw-r--r--   0 lco        (503) staff       (20)     4081 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/concrete/meta.py
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/admin/
--rw-r--r--   0 lco        (503) staff       (20)       16 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/admin/__init__.py
--rw-r--r--   0 lco        (503) staff       (20)     5899 2020-03-10 13:44:34.000000 concrete-datastore-1.8.0/concrete_datastore/admin/admin.py
--rw-r--r--   0 lco        (503) staff       (20)     5130 2020-04-28 13:58:25.000000 concrete-datastore-1.8.0/concrete_datastore/admin/admin_site.py
--rw-r--r--   0 lco        (503) staff       (20)     5706 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/admin/admin_form.py
--rw-r--r--   0 lco        (503) staff       (20)     3417 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/admin/admin_models.py
--rw-r--r--   0 lco        (503) staff       (20)      150 2020-04-28 13:58:35.000000 concrete-datastore-1.8.0/concrete_datastore/__init__.py
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/api/
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1/
--rw-r--r--   0 lco        (503) staff       (20)     2068 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1/signals.py
--rw-r--r--   0 lco        (503) staff       (20)     1959 2020-03-03 20:02:09.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1/validators.py
--rw-r--r--   0 lco        (503) staff       (20)    19781 2020-03-03 20:02:09.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1/serializers.py
--rw-r--r--   0 lco        (503) staff       (20)      181 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1/__init__.py
--rw-r--r--   0 lco        (503) staff       (20)     3102 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1/authentication.py
--rw-r--r--   0 lco        (503) staff       (20)    12161 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1/permissions.py
--rw-r--r--   0 lco        (503) staff       (20)      305 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1/exceptions.py
--rw-r--r--   0 lco        (503) staff       (20)     1366 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1/pagination.py
--rw-r--r--   0 lco        (503) staff       (20)      335 2020-03-30 09:16:09.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1/datetime.py
--rw-r--r--   0 lco        (503) staff       (20)     2361 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1/urls.py
--rw-r--r--   0 lco        (503) staff       (20)    11191 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1/filters.py
--rw-r--r--   0 lco        (503) staff       (20)    71847 2020-03-30 09:16:09.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1/views.py
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1_1/
--rw-r--r--   0 lco        (503) staff       (20)     6984 2020-03-20 09:26:06.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1_1/serializers.py
--rw-r--r--   0 lco        (503) staff       (20)      175 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1_1/__init__.py
--rw-r--r--   0 lco        (503) staff       (20)     2842 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1_1/permissions.py
--rw-r--r--   0 lco        (503) staff       (20)     3564 2020-03-20 09:26:06.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1_1/urls.py
--rw-r--r--   0 lco        (503) staff       (20)    21659 2020-03-20 09:26:06.000000 concrete-datastore-1.8.0/concrete_datastore/api/v1_1/views.py
--rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/api/__init__.py
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/authentication/
--rw-r--r--   0 lco        (503) staff       (20)      984 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/authentication/auth.py
--rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/authentication/__init__.py
--rw-r--r--   0 lco        (503) staff       (20)      794 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/authentication/oauth2_utils.py
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/routes/
--rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/routes/__init__.py
--rw-r--r--   0 lco        (503) staff       (20)     2291 2020-04-28 13:58:25.000000 concrete-datastore-1.8.0/concrete_datastore/routes/urls.py
--rw-r--r--   0 lco        (503) staff       (20)     2324 2020-02-20 22:16:44.000000 concrete-datastore-1.8.0/concrete_datastore/routes/views.py
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/concrete_datastore/interfaces/
--rw-r--r--   0 lco        (503) staff       (20)    21761 2020-02-20 22:16:35.000000 concrete-datastore-1.8.0/concrete_datastore/interfaces/openapi_schema_generator.py
--rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/concrete_datastore/interfaces/__init__.py
--rw-r--r--   0 lco        (503) staff       (20)     1128 2020-03-10 13:44:34.000000 concrete-datastore-1.8.0/concrete_datastore/interfaces/csv.py
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/docs/
--rw-r--r--   0 lco        (503) staff       (20)    12232 2020-02-21 17:42:15.000000 concrete-datastore-1.8.0/docs/authentication.md
--rw-r--r--   0 lco        (503) staff       (20)     7660 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/docs/permissions.md
--rw-r--r--   0 lco        (503) staff       (20)     3355 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/docs/filters.md
--rw-r--r--   0 lco        (503) staff       (20)     4913 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/docs/demo.md
--rw-r--r--   0 lco        (503) staff       (20)     2365 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/docs/roles.md
--rw-r--r--   0 lco        (503) staff       (20)     1201 2020-02-21 17:42:15.000000 concrete-datastore-1.8.0/docs/index.md
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/docs/assets/
--rw-r--r--   0 lco        (503) staff       (20)    33934 2020-03-20 09:26:06.000000 concrete-datastore-1.8.0/docs/assets/mini-term-sample.svg
--rw-r--r--   0 lco        (503) staff       (20)    28449 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/docs/assets/default-graph.png
--rw-r--r--   0 lco        (503) staff       (20)    24303 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/docs/assets/permissions-example.png
--rw-r--r--   0 lco        (503) staff       (20)     3507 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/docs/assets/concrete-permissions.png
--rw-r--r--   0 lco        (503) staff       (20)     2547 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/docs/assets/concrete-roles.png
--rw-r--r--   0 lco        (503) staff       (20)     4119 2020-03-30 09:16:09.000000 concrete-datastore-1.8.0/docs/assets/sample-datamodel.yml
--rw-r--r--   0 lco        (503) staff       (20)     4709 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/docs/datamodel-yml.md
--rw-r--r--   0 lco        (503) staff       (20)    15214 2020-02-21 17:42:15.000000 concrete-datastore-1.8.0/docs/api-routes.md
--rw-r--r--   0 lco        (503) staff       (20)     3155 2020-04-28 13:58:25.000000 concrete-datastore-1.8.0/README.md
--rw-r--r--   0 lco        (503) staff       (20)       54 2020-02-20 22:05:18.000000 concrete-datastore-1.8.0/setup.py
--rw-r--r--   0 lco        (503) staff       (20)     2258 2020-04-28 13:58:43.000000 concrete-datastore-1.8.0/setup.cfg
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/
+-rw-r--r--   0 lco        (503) staff       (20)     4616 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/PKG-INFO
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:32.000000 concrete-datastore-1.9.0/concrete_datastore.egg-info/
+-rw-r--r--   0 lco        (503) staff       (20)     4616 2020-06-16 15:42:32.000000 concrete-datastore-1.9.0/concrete_datastore.egg-info/PKG-INFO
+-rw-r--r--   0 lco        (503) staff       (20)        1 2020-02-20 23:19:11.000000 concrete-datastore-1.9.0/concrete_datastore.egg-info/not-zip-safe
+-rw-r--r--   0 lco        (503) staff       (20)     4100 2020-06-16 15:42:32.000000 concrete-datastore-1.9.0/concrete_datastore.egg-info/SOURCES.txt
+-rw-r--r--   0 lco        (503) staff       (20)       95 2020-06-16 15:42:32.000000 concrete-datastore-1.9.0/concrete_datastore.egg-info/entry_points.txt
+-rw-r--r--   0 lco        (503) staff       (20)      722 2020-06-16 15:42:32.000000 concrete-datastore-1.9.0/concrete_datastore.egg-info/requires.txt
+-rw-r--r--   0 lco        (503) staff       (20)       37 2020-06-16 15:42:32.000000 concrete-datastore-1.9.0/concrete_datastore.egg-info/top_level.txt
+-rw-r--r--   0 lco        (503) staff       (20)        1 2020-06-16 15:42:32.000000 concrete-datastore-1.9.0/concrete_datastore.egg-info/dependency_links.txt
+-rw-r--r--   0 lco        (503) staff       (20)    35149 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/LICENSE
+-rw-r--r--   0 lco        (503) staff       (20)      320 2020-02-21 17:55:37.000000 concrete-datastore-1.9.0/MANIFEST.in
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:32.000000 concrete-datastore-1.9.0/concrete_datastore/
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/concrete_datastore/settings/
+-rw-r--r--   0 lco        (503) staff       (20)       16 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/settings/__init__.py
+-rw-r--r--   0 lco        (503) staff       (20)     1533 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/settings/utils.py
+-rw-r--r--   0 lco        (503) staff       (20)      748 2020-03-20 14:39:44.000000 concrete-datastore-1.9.0/concrete_datastore/settings/celery.py
+-rw-r--r--   0 lco        (503) staff       (20)    14120 2020-04-28 13:58:25.000000 concrete-datastore-1.9.0/concrete_datastore/settings/base.py
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/concrete_datastore/parsers/
+-rw-r--r--   0 lco        (503) staff       (20)     2659 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/parsers/models.py
+-rw-r--r--   0 lco        (503) staff       (20)     1334 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/parsers/fields.py
+-rw-r--r--   0 lco        (503) staff       (20)      416 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/parsers/validators.py
+-rw-r--r--   0 lco        (503) staff       (20)     2445 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/parsers/constants.py
+-rw-r--r--   0 lco        (503) staff       (20)     1219 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/parsers/loaders.py
+-rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/parsers/__init__.py
+-rw-r--r--   0 lco        (503) staff       (20)      255 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/parsers/parsers.py
+-rw-r--r--   0 lco        (503) staff       (20)     4949 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/parsers/exceptions.py
+-rw-r--r--   0 lco        (503) staff       (20)      322 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/parsers/helpers.py
+-rw-r--r--   0 lco        (503) staff       (20)    17951 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/parsers/meta.py
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/migrations/
+-rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/migrations/__init__.py
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/locale/
+-rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/locale/.gitignore
+-rw-r--r--   0 lco        (503) staff       (20)    30942 2020-04-28 13:58:25.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/models.py
+-rw-r--r--   0 lco        (503) staff       (20)     1628 2020-03-03 20:02:09.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/constants.py
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/management/
+-rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/management/__init__.py
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/management/commands/
+-rw-r--r--   0 lco        (503) staff       (20)     4189 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/management/commands/openapispec.py
+-rw-r--r--   0 lco        (503) staff       (20)      793 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/management/commands/create_superuser.py
+-rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/management/commands/__init__.py
+-rw-r--r--   0 lco        (503) staff       (20)     2247 2020-02-20 22:16:52.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/management/commands/create_superuser_with_email.py
+-rw-r--r--   0 lco        (503) staff       (20)     1919 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/management/commands/init_app.py
+-rw-r--r--   0 lco        (503) staff       (20)       81 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/__init__.py
+-rw-r--r--   0 lco        (503) staff       (20)     2236 2020-03-20 09:26:06.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/apps.py
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:32.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/templates/
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/templates/admin/
+-rw-r--r--   0 lco        (503) staff       (20)     3179 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/templates/admin/mfa-login.html
+-rw-r--r--   0 lco        (503) staff       (20)     1611 2020-03-03 20:02:09.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/templates/admin/index.html
+-rw-r--r--   0 lco        (503) staff       (20)      595 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/templates/admin/base.html
+-rw-r--r--   0 lco        (503) staff       (20)      265 2020-03-03 20:02:09.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/templates/admin/change_list.html
+-rw-r--r--   0 lco        (503) staff       (20)      436 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/templates/admin/add_form.html
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/templates/mainApp/
+-rw-r--r--   0 lco        (503) staff       (20)     9043 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/templates/mainApp/index.html
+-rw-r--r--   0 lco        (503) staff       (20)     1795 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/templates/mainApp/unsubscribe.html
+-rw-r--r--   0 lco        (503) staff       (20)     9054 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/templates/mainApp/logged-using-oauth.html
+-rw-r--r--   0 lco        (503) staff       (20)      465 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/templates/mainApp/unsubscribe_result.html
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/automation/
+-rw-r--r--   0 lco        (503) staff       (20)      105 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/automation/signals.py
+-rw-r--r--   0 lco        (503) staff       (20)      513 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/automation/tasks.py
+-rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/automation/__init__.py
+-rw-r--r--   0 lco        (503) staff       (20)     1271 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/automation/signal_processor.py
+-rw-r--r--   0 lco        (503) staff       (20)     6553 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/password.py
+-rw-r--r--   0 lco        (503) staff       (20)      827 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/urls.py
+-rw-r--r--   0 lco        (503) staff       (20)      564 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/middleware.py
+-rw-r--r--   0 lco        (503) staff       (20)     3379 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/views.py
+-rw-r--r--   0 lco        (503) staff       (20)     4081 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/concrete/meta.py
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:32.000000 concrete-datastore-1.9.0/concrete_datastore/admin/
+-rw-r--r--   0 lco        (503) staff       (20)       16 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/admin/__init__.py
+-rw-r--r--   0 lco        (503) staff       (20)     5899 2020-03-10 13:44:34.000000 concrete-datastore-1.9.0/concrete_datastore/admin/admin.py
+-rw-r--r--   0 lco        (503) staff       (20)     5130 2020-04-28 13:58:25.000000 concrete-datastore-1.9.0/concrete_datastore/admin/admin_site.py
+-rw-r--r--   0 lco        (503) staff       (20)     5706 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/admin/admin_form.py
+-rw-r--r--   0 lco        (503) staff       (20)     3417 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/admin/admin_models.py
+-rw-r--r--   0 lco        (503) staff       (20)      150 2020-06-16 15:42:25.000000 concrete-datastore-1.9.0/concrete_datastore/__init__.py
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:32.000000 concrete-datastore-1.9.0/concrete_datastore/api/
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:32.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1/
+-rw-r--r--   0 lco        (503) staff       (20)     2068 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1/signals.py
+-rw-r--r--   0 lco        (503) staff       (20)     1959 2020-03-03 20:02:09.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1/validators.py
+-rw-r--r--   0 lco        (503) staff       (20)    19781 2020-03-03 20:02:09.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1/serializers.py
+-rw-r--r--   0 lco        (503) staff       (20)      181 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1/__init__.py
+-rw-r--r--   0 lco        (503) staff       (20)     3102 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1/authentication.py
+-rw-r--r--   0 lco        (503) staff       (20)    12161 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1/permissions.py
+-rw-r--r--   0 lco        (503) staff       (20)      305 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1/exceptions.py
+-rw-r--r--   0 lco        (503) staff       (20)     1366 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1/pagination.py
+-rw-r--r--   0 lco        (503) staff       (20)      335 2020-03-30 09:16:09.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1/datetime.py
+-rw-r--r--   0 lco        (503) staff       (20)     2361 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1/urls.py
+-rw-r--r--   0 lco        (503) staff       (20)    11191 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1/filters.py
+-rw-r--r--   0 lco        (503) staff       (20)    72706 2020-06-16 15:29:40.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1/views.py
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:32.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1_1/
+-rw-r--r--   0 lco        (503) staff       (20)     6984 2020-03-20 09:26:06.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1_1/serializers.py
+-rw-r--r--   0 lco        (503) staff       (20)      175 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1_1/__init__.py
+-rw-r--r--   0 lco        (503) staff       (20)     2842 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1_1/permissions.py
+-rw-r--r--   0 lco        (503) staff       (20)     3564 2020-03-20 09:26:06.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1_1/urls.py
+-rw-r--r--   0 lco        (503) staff       (20)    21659 2020-03-20 09:26:06.000000 concrete-datastore-1.9.0/concrete_datastore/api/v1_1/views.py
+-rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/api/__init__.py
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:32.000000 concrete-datastore-1.9.0/concrete_datastore/authentication/
+-rw-r--r--   0 lco        (503) staff       (20)      984 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/authentication/auth.py
+-rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/authentication/__init__.py
+-rw-r--r--   0 lco        (503) staff       (20)      794 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/authentication/oauth2_utils.py
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/concrete_datastore/routes/
+-rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/routes/__init__.py
+-rw-r--r--   0 lco        (503) staff       (20)     2291 2020-04-28 13:58:25.000000 concrete-datastore-1.9.0/concrete_datastore/routes/urls.py
+-rw-r--r--   0 lco        (503) staff       (20)     2324 2020-02-20 22:16:44.000000 concrete-datastore-1.9.0/concrete_datastore/routes/views.py
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/concrete_datastore/interfaces/
+-rw-r--r--   0 lco        (503) staff       (20)    21761 2020-02-20 22:16:35.000000 concrete-datastore-1.9.0/concrete_datastore/interfaces/openapi_schema_generator.py
+-rw-r--r--   0 lco        (503) staff       (20)        0 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/concrete_datastore/interfaces/__init__.py
+-rw-r--r--   0 lco        (503) staff       (20)     1128 2020-03-10 13:44:34.000000 concrete-datastore-1.9.0/concrete_datastore/interfaces/csv.py
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/docs/
+-rw-r--r--   0 lco        (503) staff       (20)    11917 2020-06-16 15:29:40.000000 concrete-datastore-1.9.0/docs/authentication.md
+-rw-r--r--   0 lco        (503) staff       (20)     7496 2020-06-16 15:29:40.000000 concrete-datastore-1.9.0/docs/permissions.md
+-rw-r--r--   0 lco        (503) staff       (20)     3355 2020-06-16 15:29:40.000000 concrete-datastore-1.9.0/docs/filters.md
+-rw-r--r--   0 lco        (503) staff       (20)     4901 2020-06-16 15:29:40.000000 concrete-datastore-1.9.0/docs/demo.md
+-rw-r--r--   0 lco        (503) staff       (20)     2369 2020-06-16 15:29:40.000000 concrete-datastore-1.9.0/docs/roles.md
+-rw-r--r--   0 lco        (503) staff       (20)     1201 2020-06-16 15:29:40.000000 concrete-datastore-1.9.0/docs/index.md
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/docs/assets/
+-rw-r--r--   0 lco        (503) staff       (20)    33934 2020-03-20 09:26:06.000000 concrete-datastore-1.9.0/docs/assets/mini-term-sample.svg
+-rw-r--r--   0 lco        (503) staff       (20)    28449 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/docs/assets/default-graph.png
+-rw-r--r--   0 lco        (503) staff       (20)    24303 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/docs/assets/permissions-example.png
+-rw-r--r--   0 lco        (503) staff       (20)     3507 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/docs/assets/concrete-permissions.png
+-rw-r--r--   0 lco        (503) staff       (20)     2547 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/docs/assets/concrete-roles.png
+-rw-r--r--   0 lco        (503) staff       (20)     4119 2020-03-30 09:16:09.000000 concrete-datastore-1.9.0/docs/assets/sample-datamodel.yml
+-rw-r--r--   0 lco        (503) staff       (20)     4709 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/docs/datamodel-yml.md
+-rw-r--r--   0 lco        (503) staff       (20)    15139 2020-06-16 15:29:40.000000 concrete-datastore-1.9.0/docs/api-routes.md
+-rw-r--r--   0 lco        (503) staff       (20)     3155 2020-04-28 13:58:25.000000 concrete-datastore-1.9.0/README.md
+-rw-r--r--   0 lco        (503) staff       (20)       54 2020-02-20 22:05:18.000000 concrete-datastore-1.9.0/setup.py
+-rw-r--r--   0 lco        (503) staff       (20)     2258 2020-06-16 15:42:33.000000 concrete-datastore-1.9.0/setup.cfg
```

### Comparing `concrete-datastore-1.8.0/PKG-INFO` & `concrete-datastore-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concrete-datastore
-Version: 1.8.0
+Version: 1.9.0
 Summary: A highly versatile REST Datastore
 Home-page: https://customer.caas.microservices.rest/
 Author: Netsach
 Author-email: contact@netsach.org
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Project-URL: Bug Tracker, https://github.com/Netsach/concrete-datastore/issues
 Project-URL: Documentation, https://concrete-datastore.netsach.org/en/latest/
```

### Comparing `concrete-datastore-1.8.0/concrete_datastore.egg-info/PKG-INFO` & `concrete-datastore-1.9.0/concrete_datastore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concrete-datastore
-Version: 1.8.0
+Version: 1.9.0
 Summary: A highly versatile REST Datastore
 Home-page: https://customer.caas.microservices.rest/
 Author: Netsach
 Author-email: contact@netsach.org
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Project-URL: Bug Tracker, https://github.com/Netsach/concrete-datastore/issues
 Project-URL: Documentation, https://concrete-datastore.netsach.org/en/latest/
```

### Comparing `concrete-datastore-1.8.0/concrete_datastore.egg-info/SOURCES.txt` & `concrete-datastore-1.9.0/concrete_datastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore.egg-info/requires.txt` & `concrete-datastore-1.9.0/concrete_datastore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/LICENSE` & `concrete-datastore-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/settings/utils.py` & `concrete-datastore-1.9.0/concrete_datastore/settings/utils.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/settings/celery.py` & `concrete-datastore-1.9.0/concrete_datastore/settings/celery.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/settings/base.py` & `concrete-datastore-1.9.0/concrete_datastore/settings/base.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/parsers/models.py` & `concrete-datastore-1.9.0/concrete_datastore/parsers/models.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/parsers/fields.py` & `concrete-datastore-1.9.0/concrete_datastore/parsers/fields.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/parsers/constants.py` & `concrete-datastore-1.9.0/concrete_datastore/parsers/constants.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/parsers/loaders.py` & `concrete-datastore-1.9.0/concrete_datastore/parsers/loaders.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/parsers/exceptions.py` & `concrete-datastore-1.9.0/concrete_datastore/parsers/exceptions.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/parsers/meta.py` & `concrete-datastore-1.9.0/concrete_datastore/parsers/meta.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/models.py` & `concrete-datastore-1.9.0/concrete_datastore/concrete/models.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/constants.py` & `concrete-datastore-1.9.0/concrete_datastore/concrete/constants.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/management/commands/openapispec.py` & `concrete-datastore-1.9.0/concrete_datastore/concrete/management/commands/openapispec.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/management/commands/create_superuser.py` & `concrete-datastore-1.9.0/concrete_datastore/concrete/management/commands/create_superuser.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/management/commands/create_superuser_with_email.py` & `concrete-datastore-1.9.0/concrete_datastore/concrete/management/commands/create_superuser_with_email.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/management/commands/init_app.py` & `concrete-datastore-1.9.0/concrete_datastore/concrete/management/commands/init_app.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/apps.py` & `concrete-datastore-1.9.0/concrete_datastore/concrete/apps.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/templates/admin/mfa-login.html` & `concrete-datastore-1.9.0/concrete_datastore/concrete/templates/admin/mfa-login.html`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/templates/admin/index.html` & `concrete-datastore-1.9.0/concrete_datastore/concrete/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/templates/admin/base.html` & `concrete-datastore-1.9.0/concrete_datastore/concrete/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/templates/mainApp/index.html` & `concrete-datastore-1.9.0/concrete_datastore/concrete/templates/mainApp/index.html`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/templates/mainApp/unsubscribe.html` & `concrete-datastore-1.9.0/concrete_datastore/concrete/templates/mainApp/unsubscribe.html`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/templates/mainApp/logged-using-oauth.html` & `concrete-datastore-1.9.0/concrete_datastore/concrete/templates/mainApp/logged-using-oauth.html`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/automation/tasks.py` & `concrete-datastore-1.9.0/concrete_datastore/concrete/automation/tasks.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/automation/signal_processor.py` & `concrete-datastore-1.9.0/concrete_datastore/concrete/automation/signal_processor.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/password.py` & `concrete-datastore-1.9.0/concrete_datastore/concrete/password.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/urls.py` & `concrete-datastore-1.9.0/concrete_datastore/concrete/urls.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/middleware.py` & `concrete-datastore-1.9.0/concrete_datastore/concrete/middleware.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/views.py` & `concrete-datastore-1.9.0/concrete_datastore/concrete/views.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/concrete/meta.py` & `concrete-datastore-1.9.0/concrete_datastore/concrete/meta.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/admin/admin.py` & `concrete-datastore-1.9.0/concrete_datastore/admin/admin.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/admin/admin_site.py` & `concrete-datastore-1.9.0/concrete_datastore/admin/admin_site.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/admin/admin_form.py` & `concrete-datastore-1.9.0/concrete_datastore/admin/admin_form.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/admin/admin_models.py` & `concrete-datastore-1.9.0/concrete_datastore/admin/admin_models.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/api/v1/signals.py` & `concrete-datastore-1.9.0/concrete_datastore/api/v1/signals.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/api/v1/validators.py` & `concrete-datastore-1.9.0/concrete_datastore/api/v1/validators.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/api/v1/serializers.py` & `concrete-datastore-1.9.0/concrete_datastore/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/api/v1/authentication.py` & `concrete-datastore-1.9.0/concrete_datastore/api/v1/authentication.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/api/v1/permissions.py` & `concrete-datastore-1.9.0/concrete_datastore/api/v1/permissions.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/api/v1/pagination.py` & `concrete-datastore-1.9.0/concrete_datastore/api/v1/pagination.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/api/v1/urls.py` & `concrete-datastore-1.9.0/concrete_datastore/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/api/v1/filters.py` & `concrete-datastore-1.9.0/concrete_datastore/api/v1/filters.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/api/v1/views.py` & `concrete-datastore-1.9.0/concrete_datastore/api/v1/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     HTTP_403_FORBIDDEN,
     HTTP_401_UNAUTHORIZED,
     HTTP_200_OK,
     HTTP_412_PRECONDITION_FAILED,
     HTTP_204_NO_CONTENT,
 )
 from rest_framework import authentication, permissions, generics, viewsets
+from rest_framework.utils.urls import remove_query_param, replace_query_param
 
 from concrete_datastore.concrete.models import (  # pylint:disable=E0611
     AuthToken,
     DeletedModel,
     DIVIDER_MODEL,
     UNDIVIDED_MODEL,
     PasswordChangeToken,
@@ -1212,19 +1213,41 @@
         if request.parser_context["view"].model_class.__name__ == "User":
             validate_request_permissions(request=request)
 
         queryset, timestamp_end = self._get_queryset_filtered_since_timestamp(
             timestamp_start, timestamp_end
         )
 
+        _resp = self.get_paginated_response(self.request.data)
+
         _total = queryset.count()
+
+        _num_pages = _resp.data['num_total_pages']
+
+        dict_pages = dict()
+        url = self.request.build_absolute_uri()
+        for page_number in range(1, _num_pages + 1):
+            if page_number == 1:
+                dict_pages['page{}'.format(page_number)] = remove_query_param(
+                    url, 'page'
+                )
+            else:
+                dict_pages['page{}'.format(page_number)] = replace_query_param(
+                    url, 'page', page_number
+                )
+
         data = {
             'objects_count': _total,
             'timestamp_start': timestamp_start or 0.0,
             'timestamp_end': timestamp_end,
+            'num_total_pages': _num_pages,
+            'max_allowed_objects_per_page': _resp.data[
+                'max_allowed_objects_per_page'
+            ],
+            'page_urls': dict_pages,
         }
         return Response(data)
 
     def _get_queryset_filtered_since_timestamp(
         self, timestamp_start=None, timestamp_end=None
     ):
         queryset = self.filter_queryset(self.get_queryset())
@@ -1588,15 +1611,15 @@
         except WrongEntityUIDError:
             return self.model_class.objects.none()
 
         model_name = self.model_class.__name__
 
         if model_name == DIVIDER_MODEL and divider is None:
             if user.is_anonymous:
-                return self.model_class.objects.none()
+                return self.model_class.objects.filter(public=True)
             elif at_least_admin:
                 return self.model_class.objects.all()
             else:
                 return self.model_class.objects.filter(
                     pk__in=getattr(
                         user, '{}s'.format(DIVIDER_MODEL.lower())
                     ).all()
```

### Comparing `concrete-datastore-1.8.0/concrete_datastore/api/v1_1/serializers.py` & `concrete-datastore-1.9.0/concrete_datastore/api/v1_1/serializers.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/api/v1_1/permissions.py` & `concrete-datastore-1.9.0/concrete_datastore/api/v1_1/permissions.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/api/v1_1/urls.py` & `concrete-datastore-1.9.0/concrete_datastore/api/v1_1/urls.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/api/v1_1/views.py` & `concrete-datastore-1.9.0/concrete_datastore/api/v1_1/views.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/authentication/auth.py` & `concrete-datastore-1.9.0/concrete_datastore/authentication/auth.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/authentication/oauth2_utils.py` & `concrete-datastore-1.9.0/concrete_datastore/authentication/oauth2_utils.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/routes/urls.py` & `concrete-datastore-1.9.0/concrete_datastore/routes/urls.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/routes/views.py` & `concrete-datastore-1.9.0/concrete_datastore/routes/views.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/interfaces/openapi_schema_generator.py` & `concrete-datastore-1.9.0/concrete_datastore/interfaces/openapi_schema_generator.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/concrete_datastore/interfaces/csv.py` & `concrete-datastore-1.9.0/concrete_datastore/interfaces/csv.py`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/docs/authentication.md` & `concrete-datastore-1.9.0/docs/authentication.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,23 +28,23 @@
     "password1": "[password in plain text]",
     "password2": "[repeated password in plain text]",
     "url_format": "[valid url format]",
     "email_format": "[valid email format]"
 }
 ```
 -  `email` is mandatory
--  `password1` is optional (if ALLOW_SEND_EMAIL_ON_REGISTER is enabled in settings) and has a default value generated within the view.
--  `password2` is optional (if ALLOW_SEND_EMAIL_ON_REGISTER is enabled in settings) and has a default value generated within the view.
+-  `password1` is optional (if ALLOW_SEND_EMAIL_ON_REGISTER is enabled in settings) and has a default value generated within the view
+-  `password2` is optional (if ALLOW_SEND_EMAIL_ON_REGISTER is enabled in settings) and has a default value generated within the view
 -  `email_format` is optional and has a default value of DEFAULT_REGISTER_EMAIL_FORMAT (in settings)
 -  `url_format` is optional and has a default value of `"/#/set-password/{token}/{email}/"`
 
 **Use cases** :
 
 -  A user can set `password1` and `password2` in order to register whith his own password.
--  A user can register without setting passwords (if the settings ALLOW_SEND_EMAIL_ON_REGISTER is enabled), and he will recieve a link in an email. This link contains the email adress used to register with and a token used to reset password. He can then reset his password using this token
+-  A user can register without setting passwords (if the setting ALLOW_SEND_EMAIL_ON_REGISTER is enabled), and he will recieve a link in an email. This link contains the email adress used to register with and a token used to reset the password. He can then reset his password using this token.
 
 **Data example**
 
 ```json
 {
     "email": "johndoe@netsach.com",
     "password1": "abcd1234",
@@ -66,15 +66,15 @@
     "token": "e0d15a8547e37ccced180ad590bac5e28cabc71a",
     "first_name": "",
     "last_name": "",
     "level": "simpleuser",
 }
 ```
 
-**IMPORTANT:** if AUTH_CONFIRM_EMAIL_ENABLE is True is settings, you will receiev an email. You will need to confirm your email address by clicking on the link attached to this email.
+**IMPORTANT:** if AUTH_CONFIRM_EMAIL_ENABLE is True is settings, you will receive an email. You will need to confirm your email address by clicking on the link attached to this email.
 
 #### Error Responses
 
 **Condition** : If the email is not allowed to register.
 
 **Code** : `400 BAD REQUEST`
 
@@ -93,51 +93,51 @@
 
 **Code** : `400 BAD REQUEST`
 
 **Content** :
 
 ```json
 {
-    'message': 'Password confimation incorrect'
+    "message": "Password confimation incorrect"
 }
 ```
 
 **Condition** : If the `url_format` has not the right format.
 
 **Code** : `400 BAD REQUEST`
 
 **Content** :
 
 ```json
 {
-    'errors': 'url_format is not a valid format_string'
+    "errors": "url_format is not a valid format_string"
 }
 ```
 
 **Condition** : If the `email_format` has not the right format.
 
 **Code** : `400 BAD REQUEST`
 
 **Content** :
 
 ```json
 {
-    'errors': 'email_format is not a valid format_string'
+    "errors": "email_format is not a valid format_string"
 }
 ```
 
-**Condition** : If a user not authenticated to the plateform (AnonymousUser) attempts to post an email format.
+**Condition** : If a user not authenticated to the platform (AnonymousUser) attempts to post an email format.
 
 **Code** : `400 BAD REQUEST`
 
 **Content** :
 
 ```json
 {
-    'message': 'Only registered users are allowed to set an email_format'
+    "message": "Only registered users are allowed to set an email_format"
 }
 ```
 
 **Condition** : If `password` does not comply with complexity criteria.
 
 **Code** : `400 BAD REQUEST`
 
@@ -261,29 +261,14 @@
     "message": "Email has not been validated",
     "_errors": [
         "EMAIL_NOT_VALIDATED"
     ]
 }
 ```
 
-**Condition** : If the email address has not been validated.
-
-**Code** : `401 UNAUTHORIZED`
-
-**Content** :
-
-```json
-{
-    "message": "Email has not been validated",
-    "_errors": [
-        "EMAIL_NOT_VALIDATED"
-    ]
-}
-```
-
 ### Account information
 
 #### Request
 
 Used to get information about the user.
 
 **URL** : `/api/v1.1/account/me/`
@@ -401,17 +386,17 @@
 **Data constraints**
 ```json
 {
     "email": "[valid email]",
     "url_format": "[valid url_format]"
 }
 ```
-the url_format will be used to send the reset password email with a link to allow the user to reset its own password. it should be a string containing `"{email}"` and `"{token}"`. example: `"/redirection-url/{email}/{token}"`.  
+The url_format will be used to send the reset password email with a link to allow the user to reset his own password. It should be a string containing `"{email}"` and `"{token}"`. Example: `"/redirection-url/{email}/{token}"`.  
 
-default value: `"/#/reset-password/{token}/{email}/"`.
+Default value: `"/#/reset-password/{token}/{email}/"`.
 
 **Data example**
 
 ```json
 {
     "email": "johndoe@netsach.com",
     "url_format": "/redirection-url/{token}/{email}/"
@@ -442,15 +427,15 @@
 }
 ```
 
 ### Change Password
 
 #### Request
 
-Used to change password of a user.
+Used to change the password of a user.
 
 **URL** : `/api/v1.1/auth/change-password/`
 
 **Method** : `POST`
 
 **Auth required** : YES.
 
@@ -463,15 +448,15 @@
     "password_change_token": "[valid token]"
 }
 ```
 
 -  `email` is mandatory
 -  `password1` is mandatory
 -  `password2` is mandatory
--  `password_change_token` is optional. This token is created if the user forgot his password and requests a reset password, or if the current password has expired. If given in data, that means that the user is attemting to change his own password (the request is not authenticated). Otherwise, if the `password_change_token` is not given, the request must be authenticated and the authenticated user must have the permissions to alter another user's password.
+-  `password_change_token` is optional. This token is created if the user forgot his password and requests a reset password, or if the current password has expired. If given in data, that means that the user is attempting to change his own password (the request is not authenticated). Otherwise, if the `password_change_token` is not given, the request must be authenticated and the authenticated user must have the permissions to alter another user's password.
 
 **Data example**
 
 ```json
 {
     "email": "johndoe@netsach.com",
     "password1": "test",
@@ -482,15 +467,15 @@
 
 #### Success Response
 
 **Code** : `200 OK`
 
 **Content example**
 
-if a user attempts to change his own password
+If a user attempts to change his own password
 
 ```json
 {
     "public": true,
     "uid": "49297d80-e924-479a-8fcc-27e15f7a12e7",
     "modification_date": "2018-11-26T15:54:34Z",
     "creation_date": "2018-11-26T15:54:34Z",
@@ -499,15 +484,15 @@
     "last_name": "John",
     "first_name": "Doe",
     "level": "simpleuser",
     "email": "johndoe@netsach.com"
 }
 ```
 
-if a user (with the sufficient permissions) attempts to change another user's password:
+If a user (with the sufficient permissions) attempts to change another user's password:
 
 ```json
 {
     "email": "johndoe@netsach.com",
     "message": "Passwod updated !"
 }
 ```
@@ -526,15 +511,11 @@
 
 **Code** : `400 BAD REQUEST`
 
 **Condition** : If the new password is identical to the old one.
 
 **Code** : `400 BAD REQUEST`
 
-**Condition** : If the given `password_change_token` is invalid.
-
-**Code** : `400 BAD REQUEST`
-
 **Condition** : If the user making the request does not have the permission to change another user's password.
 
 **Code** : `403 FORBIDDEN`
```

### Comparing `concrete-datastore-1.8.0/docs/permissions.md` & `concrete-datastore-1.9.0/docs/permissions.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ## Permissions
 
-Multiple parameters are put together to determine for each user the permissions he was granted:
+Multiple parameters are put together to determine the permissions that were granted for each user:
 
 - Request Type (scoped/unscoped)
 - Model and objects definition
 - Scopes of user
 - User Level
 
-These criterions are ordered by strength (from the strongest criterion to the weakest).
+These criteria are ordered by strength (from the strongest criterion to the weakest).
 
 ### Request Type
 
 When performing a request to the API Concrete (get, post, patch, delete), the scope (`X-ENTITY-UID`) can be added to the headers of the request:
 
-The scope passed in the headers of a request is used to filter the response's objects, and allow access only to the objects having the same scope.
+The scope passed in the headers of a request is used to filter the response's objects, and allows access only to the objects having the same scope.
 
 #### Unscoped Request
 
 ```shell
 curl \
   -X GET \
   -H "Authorization: Token b1cccee29710b53386b964d93847648a526005a8" \
@@ -28,16 +28,14 @@
 ```shell
 curl \
   -X GET \
   -H "Authorization: Token b1cccee29710b53386b964d93847648a526005a8" \
   -H "X-ENTITY-UID: 7508ffd7-2d10-413e-86b6-4adab3767413" \
   "https://<webapp>/api/v1.1/<model-name>/"
 ```
-The scope passed in the headers of a request is used to filter the response's objects, and allow access only to the objects having this same scope.
-
 
 **Example:** given two scopes `scopeA` and `scopeB` and a model `MyModel` accessible through a `url`. Given objects:
 
 - `object1: scope=scopeA`
 - `object2: scope=scopeB`
 - `object3: scope=None`
 - `object4: scope=scopeA`
@@ -48,15 +46,15 @@
 
 - **Scoped Request:** `requests.get(url,headers={"Authorization":"Token {}".format(super_token),"X-ENTITY-UID":scopeA.uid})` returns a list containing only the objects with the scope `scopeA` (i.e only `object1` and `object4`).
 
 ### Model and Object Definition
 
 #### Model Definition
 
-For a model, some constraints on the user level are set to determine whether a given user can perform a given operation (create, delete, retrieve and update) or not:
+For a model, some user level constraints are set to determine whether a given user can perform a given operation (create, delete, retrieve and update) or not:
 
 ```json
 {
   "ext.m_creation_minimum_level": "admin",
   "ext.m_delete_minimum_level": "superuser",
   "ext.m_retrieve_minimum_level": "authenticated",
   "ext.m_update_minimum_level": "manager"
@@ -64,35 +62,35 @@
 ```
 
 #### Object Definition
 
 Objects can have arguments that allow a user (or a group of users) to perform some operations that he can't normally perform:
 
 
-- `can_view_users`, `can_view_groups`: gives retrieve rights to a user or a group of users.
-- `can_admin_users`, `can_admin_groups`: gives retrieve and update rights to a user or a group of users.
-- `public`: a boolean. If `public` is false : a user whose level is `manager` or less can't have access to this object unless he is the owner (`created_by`) or listed in `can_admin_[users/groups]` or `can_view_[users/groups]`.
+- `can_view_users`, `can_view_groups`: gives `Retrieve` rights to a user or a group of users.
+- `can_admin_users`, `can_admin_groups`: gives `Retrieve` and `Update` rights to a user or a group of users.
+- `public`: a boolean. If set to false, a user with level `manager` or less can't have access to this object unless he is the owner (`created_by`) or listed in `can_admin_[users/groups]` or `can_view_[users/groups]`.
 
 ### User levels
 
 There are five user levels with a set of permissions and privileges:
 
 Superuser > Admin > Manager > Simpleuser > Blocked
 
-- The `superuser` and access to everything and has all the rights.
-- The other levels have different create, retrieve permissions depending on the model and the instance created.
+- The `superuser` has access to everything and has all the rights.
+- The other levels have different create and retrieve permissions, depending on the model and the created instance.
 - The `blocked` user has access to nothing.
 
 ### User Scopes
 
-A user can have one or more scopes that are used to determine the range of objects accessible by a user.
+A user can have one or more scopes that are used to determine the range of objects accessible to him.
 
-A user of an `admin` level or higher can access to all the objects independently of his scopes.
+A user of an `admin` level or higher has access to all the objects, independently of his scopes.
 
-For a level `manager` or less if the user has a scope `A`, he can access to all the objects having a scope `A` (and only these objects).
+For a level `manager` or less, if the user has a scope `A`, he can access to all the objects having a scope `A` (and only these objects).
 The possible operations on these objects are those that satisfy the model's definition.
 
 
 ### Example
 
 Given two scopes: `Divider_X` and `Divider_Y`
 
@@ -112,43 +110,43 @@
 
 Given a Divided Model `MyModel` and four instances of this model with the following configuration:
 
 ![](./assets/permissions-example.png)
 
 #### 1st case: For A Scoped Request With The Scope Divider_X:
 
-- **SuperUser :** can access to `instance_1` and `instance_3` and has all the rights.
-- **Admin :** can access to `instance_1` and `instance_3` and has retrieve, create and update rights
-- **Manager :** can access to `instance_3` (because of `can_view_users`) with retrieve rights and `instance_1`(because of `can_admin_users`) with retrieve and update rights
+- **SuperUser:** can access to `instance_1` and `instance_3` and has all the rights.
+- **Admin:** can access to `instance_1` and `instance_3` and has retrieve, create and update rights
+- **Manager:** can access to `instance_3` (because of `can_view_users`) with retrieve rights and `instance_1`(because of `can_admin_users`) with retrieve and update rights
 - **Manager_X**: can access to `instance_1` and `instance_3` (because of scope) and has retrieve and update rights
 - **Manager_Y**: has access only to `instance_3` (because of `can_admin_users`) and has retrieve and update rights.
 - **Manager_XY**: can access to `instance_1` and `instance_3` and has retrieve and update rights
 - **SimpleUser**: has access only to `instance_1` (because of `can_view_users`) and has only retrieve rights
 - **SimpleUser_X**: has access to `instance_1` and `instance_3` (because of scope) and has only retrieve rights
 - **SimpleUser_Y**: has access to nothing
 - **SimpleUser_XY**: has access to `instance_1` and `instance_3` (because of scope) and has only retrieve rights
 
 #### 2nd case: For A Scoped Request With The Scope Divider_Y:
 
-- **SuperUser :** can access to `instance_2` and has all the rights.
-- **Admin :** can access to `instance_2` and has retrieve, create and update rights
-- **Manager :** has access to nothing
+- **SuperUser:** can access to `instance_2` and has all the rights.
+- **Admin:** can access to `instance_2` and has retrieve, create and update rights
+- **Manager:** has access to nothing
 - **Manager_X**: can access to `instance_2` (because of `can_view_users`) and has only retrieve rights
 - **Manager_Y**: has access to `instance_2` (because of scope) and has retrieve and update rights.
 - **Manager_XY**: can access to `instance_2` and has retrieve and update rights
 - **SimpleUser**: has access `instance_2` (because of `can_admin_users`) and has only retrieve rights
 - **SimpleUser_X**: has access to nothing
 - **SimpleUser_Y**: has access to `instance_2` with retrieve rights
 - **SimpleUser_XY**: has access to `instance_2` (because of scope) and has only retrieve rights
 
 #### 3rd case: For A Non-Scoped Request:
 
-- **SuperUser :** can access to everything and has all the rights.
-- **Admin :** can access to everything and has retrieve, create and update rights
-- **Manager :** can access to `instance_3` (because of `can_view_users`) with retrieve rights and `instance_1`(because of `can_admin_users`) with retrieve and update rights
+- **SuperUser:** can access to everything and has all the rights.
+- **Admin:** can access to everything and has retrieve, create and update rights
+- **Manager:** can access to `instance_3` (because of `can_view_users`) with retrieve rights and `instance_1`(because of `can_admin_users`) with retrieve and update rights
 - **Manager_X**: can access to `instance_2` (because of `can_view_users`) with only retrieve rights, and can access to `instance_1` and `instance_3` (because of scope) with retrieve and update rights
 - **Manager_Y**: has access to `instance_2` (because of scope) and to `instance_3` (because of `can_admin_users`) and has retrieve and update rights.
 - **Manager_XY**: can access to everything and has retrieve and update rights
 - **SimpleUser**: has access `instance_2` (because of `can_admin_users`) and `instance_1` (because of `can_view_users`) and has only retrieve rights
 - **SimpleUser_X**: has access to `instance_1` and `instance_3` (because of scope) as well as `instance_4` (because of public) and has only retrieve rights
 - **SimpleUser_Y**: has access to `instance_2` (because of scope) and `instance_4` (because of public) with retrieve rights
 - **SimpleUser_XY**: has access to everything (because of scopes and public) and has only retrieve rights
```

### Comparing `concrete-datastore-1.8.0/docs/filters.md` & `concrete-datastore-1.9.0/docs/filters.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 ## Filters and ordering
 
 ### Filters
 API requests support different types of filters:
 
-- **Filter Supporting Or operation:** by adding the `__in` suffix:
+- **Filter Supporting Or operation:** By adding the `__in` suffix:
 example: `?name__in=project1,project2,project3` returns all objects that the field name has a value of "project1" **OR** "project2" **OR** "project3"
-- **Filter Supporting Empty values:** by adding `__isempty=true`:
+- **Filter Supporting Empty values:** By adding `__isempty=true`:
 example: `?project__isempty=true` returns all objects that do not have a `project`
-- **Filter Supporting Comparison operations:** by adding the suffixes `__gte`, `__gt`, `__lte` and `__lt`
+- **Filter Supporting Comparison operations:** By adding the suffixes `__gte`, `__gt`, `__lte` and `__lt`
 example:
  * `?price__gte=10` (price >= 10)
  * `?price__gt=10` (price > 10)
  * `?price__lte=10` (price <= 10)
  * `?price__lt=10` (price < 10)
-- **Filter Supporting Range:** by adding the suffix `__range`:
+- **Filter Supporting Range:** By adding the suffix `__range`:
 example: `?creation_date__range=2018-01-01,2018-12-31` returns all objects with creation date is between 1st Jan 2018 and 31st Dec 2018
 
 - `c_resp_page_size`: The API also features pagination by the use of the query parameter `c_resp_page_size` that takes an integer representing the number of results per page that sould be returned
 - `c_resp_nested`: If there are relation between objects, by default the API shows the relation completely, it is nested.
-example:
+Example:
 
 ```json
 {
       "global_status": "PENDING",
       "name": "Test Name",
       "other_object": { //Nested here
         "status":"other_object_status",
@@ -48,16 +48,16 @@
 examples:
     - `?timestamp_start=100000&timestamp_end=20000`: Filter objects between timestamp [10000, 20000]
     - `?timestamp_start=10000`: Filter objects between timestamp [10000, now]
     - `?timestamp_end=20000`: Filter objects between timestamp [0, 20000]
 
 
 * **Filter users by level:** You can filter users by level with two filters: `level` and `atleast`
-    * **/user/?level**=[user_level]: Users with an exact level `user_level`. The user_level must be in [**superuser**, **admin**, **manager**, **simpleuser**]
-    * **/user/?atleast**=[user_level]: Users with a level atleast equal to `user_level`. The user_level must be in [**superuser**, **admin**, **manager**, **simpleuser**]
+    - **/user/?level**=[user_level]: Users with an exact level `user_level`. The user_level must be in [**superuser**, **admin**, **manager**, **simpleuser**]
+    - **/user/?atleast**=[user_level]: Users with a level atleast equal to `user_level`. The user_level must be in [**superuser**, **admin**, **manager**, **simpleuser**]
 
     Example: `/user/?atleast=manager` gives users with level manager, admin and superuser
 
 
 
 **Filter examples**:
```

### Comparing `concrete-datastore-1.8.0/docs/demo.md` & `concrete-datastore-1.9.0/docs/demo.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,23 +38,23 @@
   "groups": [],
   "defaultdividers": []
 }
 ```
 The token will be used for further autheticated requests.
 
 #### Login to the API
-In order to login to the plateforme and retrieve your token, you can perform a `POST` request on `/auth/login/` with data containing your user's email and password (used to register):
+In order to login to the platform and retrieve your token, you can perform a `POST` request on `/auth/login/` with data containing your user's email and password (used to register):
 ```shell
 curl \
    -X POST \
    -d "{\"email\":\"johndoe@netsach.com\",\"password\":\"netsach2020\"}" \
    -H "Content-Type: application/json" \
    "https://<webapp>/api/v1.1/auth/login/"
 ```
-And the server will respond with a JSON containing your token along with other user's information:
+The server will respond with a JSON containing your token along with other user information:
 ```json
 {
   "uid": "fe2ad17a-4678-499c-a957-4cd84dd16e08",
   "email": "johndoe@netsach.com",
   "url": "https://localhost:8000/api/v1.1/account/me/",
   "token": "e72e8df2d1ab9ee0d7cb61367958e4bb8620c1e6",
   "first_name": "John",
@@ -74,15 +74,15 @@
     -X POST \
     -H "Content-Type: application/json" \
     -H "Authorization: Token e72e8df2d1ab9ee0d7cb61367958e4bb8620c1e6" \
     -d '{"name":"MyFirstProject","code":"MFP",manager_uid":"fe2ad17a-4678-499c-a957-4cd84dd16e08","start_date":"2020-01-24T10:23:53Z"}' \
     "https://<webapp>/api/v1.1/project/"
 ```
 
-The instance is the created and the server responds with the following JSON:
+The instance is created and the server responds with the following JSON:
 
 ```json
 {
   "uid": "b1546151-3519-415d-8d8d-8cc113dc1408",
   "name": "MyFirstProject",
   "code": "MFP",
   "manager": "c18f9045-b850-47a5-9d48-5ee2a8196bb8",
@@ -104,15 +104,15 @@
 You can also list all instances of model `Project` with a `GET` request on `api/v1.1/project/` with your token:
 ```shell
 curl \
     -X GET \
     -H "Authorization: Token e72e8df2d1ab9ee0d7cb61367958e4bb8620c1e6" \
     "https://<webapp>/api/v1.1/project/"
 ```
-the API responds with the following JSON:
+The API responds with the following JSON:
 ```json
 {
   "objects_count": 1,
   "next": null,
   "previous": null,
   "results": [
     {
```

### Comparing `concrete-datastore-1.8.0/docs/roles.md` & `concrete-datastore-1.9.0/docs/roles.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 ## Concrete Roles and Concrete Permissions
 
 **IMPORTANT:** Concrete Roles and permissions are only enabled if USE_CONCRETE_ROLES is True in settings
 
 ### Concrete Roles
 
-`ConcreteRole` is a concrete datastore model that allows to attribute different permissions for users of the same level. (**admins and superusers don't have their permissions changed by the roles, that only affects simpleusers and managers of the plateform.**)
+`ConcreteRole` is a concrete datastore model that allows to attribute different permissions for users of the same level. (**admins and superusers don't have their permissions changed by the roles, that only affects simpleusers and managers of the platform.**)
 
 Each instance of model ConcreteRole has a role name and a list of users.
 
 ![](./assets/concrete-roles.png)
 
 `ConcreteRole` is associated (M2M) to [`ConcrerePremissions`](#ConcretePermissions) in order to set the permissions rules.
 
 Note that concrete roles and permissions don't give additional permissions to a user, it only restricts his default permissions.
 
 ### <a name="ConcretePermissions"></a>Concrete permission
 
-`ConcretePermission` is a concrete datastore model that allows to specify for each model of the datamdoel definition a set of permissions depending on the roles defined in ConcretRole. These permissions match with the **CRUD** operations (**C**reate, **R**etrieve, **U**pdate, **D**elete)
+`ConcretePermission` is a concrete datastore model that allows to specify a set of permissions for each model of the datamodel definition, depending on the roles defined in ConcretRole. These permissions match with the **CRUD** operations (**C**reate, **R**etrieve, **U**pdate, **D**elete)
 
 ![](./assets/concrete-permissions.png)
 
 For simpleusers and managers, in order to perform a **CRUD** operation, a user must have a role allowed to perform this operation (see example below for more details).
 
 ### Example
 
@@ -40,12 +40,12 @@
     "model_name": "MyModel",
     "create_roles": {
         "roles": ["<Creator_uid>"]
     }
 }
 ```
 
--  With this permission added, the only user than is allowed to create instances of `MyModel` is the `Manager_1` because he belongs to `Creator` role.
+-  With this permission added, the only user that is allowed to create instances of `MyModel` is the `Manager_1` because he belongs to the `Creator` role.
 
 -  Even if `Manager_2` has the minimum required level to create instances, he does not have the required role to do so.
 
 -  The `SimpleUser` has a role of `Creator` that is allowed to create new instances, but he does not have the minimun level required by the model, so he cannot perform a create on this model.
```

### Comparing `concrete-datastore-1.8.0/docs/index.md` & `concrete-datastore-1.9.0/docs/index.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ## Introduction
 
 This document is a user guide to Concrete Datastore and its features.
 
 Concrete Datastore is a Datastore generator that consumes a datamodel file containing a database description, and dynamically generates the corresponding tables.
 
-Concrete Datastore exposes a Restfull API to allow its users to interact with the database by **C**reating, **R**etrieving, **U**pdating and **D**eleting data (**CRUD**).
+Concrete Datastore exposes a RESTful API to allow its users to interact with the database by **C**reating, **R**etrieving, **U**pdating and **D**eleting data (**CRUD**).
 
-In order to gain access or modify the database’s data, each request must be authenticated with a unique token for each user (see [authentication](authentication.md) section). This allows Concrete Datastore to know which user is using the plateform. The desired actions depend on the user’s permissions (see [permissions](permissions.md) and [roles](roles.md) sections).
+In order to gain access or modify the database’s data, each request must be authenticated with a unique token for each user (see [authentication](authentication.md) section). This allows Concrete Datastore to know which user is using the platform. The desired actions depend on the user’s permissions (see [permissions](permissions.md) and [roles](roles.md) sections).
 
-Concrete Datastore also allows its users to have full control on the data requested by enabling a filtering mechanism on the different elements of the database (see [filters](filters.md) section).
+Concrete Datastore also allows its users to have full control over the data requested by enabling a filtering mechanism on the different elements of the database (see [filters](filters.md) section).
 
 ## Table of contents
 
 - [API Authentication](authentication.md)
 - [API Routes](api-routes.md)
 - [API Filters](filters.md)
 - [API Permissions](permissions.md)
```

### Comparing `concrete-datastore-1.8.0/docs/assets/mini-term-sample.svg` & `concrete-datastore-1.9.0/docs/assets/mini-term-sample.svg`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/docs/assets/default-graph.png` & `concrete-datastore-1.9.0/docs/assets/default-graph.png`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/docs/assets/permissions-example.png` & `concrete-datastore-1.9.0/docs/assets/permissions-example.png`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/docs/assets/concrete-permissions.png` & `concrete-datastore-1.9.0/docs/assets/concrete-permissions.png`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/docs/assets/concrete-roles.png` & `concrete-datastore-1.9.0/docs/assets/concrete-roles.png`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/docs/assets/sample-datamodel.yml` & `concrete-datastore-1.9.0/docs/assets/sample-datamodel.yml`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/docs/datamodel-yml.md` & `concrete-datastore-1.9.0/docs/datamodel-yml.md`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/README.md` & `concrete-datastore-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `concrete-datastore-1.8.0/setup.cfg` & `concrete-datastore-1.9.0/setup.cfg`

 * *Files identical despite different names*

