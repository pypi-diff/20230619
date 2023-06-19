# Comparing `tmp/djangosaml2-1.5.8.tar.gz` & `tmp/djangosaml2-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangosaml2-1.5.8.tar", last modified: Tue May 30 08:44:29 2023, max compression
+gzip compressed data, was "djangosaml2-1.6.0.tar", last modified: Mon Jun 19 17:02:21 2023, max compression
```

## Comparing `djangosaml2-1.5.8.tar` & `djangosaml2-1.6.0.tar`

### file list

```diff
@@ -1,85 +1,1590 @@
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/
--rw-rw-r--   0 wert      (1000) wert      (1000)    13512 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/CHANGES
--rw-rw-r--   0 wert      (1000) wert      (1000)    11358 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/COPYING
--rw-rw-r--   0 wert      (1000) wert      (1000)      164 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/MANIFEST.in
--rw-rw-r--   0 wert      (1000) wert      (1000)     3017 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/PKG-INFO
--rw-rw-r--   0 wert      (1000) wert      (1000)     1681 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/README.md
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)        0 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/__init__.py
--rw-rw-r--   0 wert      (1000) wert      (1000)      190 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/apps.py
--rw-rw-r--   0 wert      (1000) wert      (1000)    14380 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/backends.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     2894 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/cache.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     2568 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/conf.py
--rw-rw-r--   0 wert      (1000) wert      (1000)       51 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/exceptions.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     3511 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/middleware.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1045 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/overrides.py
--rw-rw-r--   0 wert      (1000) wert      (1000)      726 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/signals.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/djangosaml2/templatetags/
--rw-rw-r--   0 wert      (1000) wert      (1000)        0 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templatetags/__init__.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templatetags/idplist.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)    42515 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/__init__.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/djangosaml2/tests/attribute-maps/
--rw-rw-r--   0 wert      (1000) wert      (1000)      555 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/attribute-maps/django_saml_uri.py
--rw-rw-r--   0 wert      (1000) wert      (1000)    11106 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/attribute-maps/saml_uri.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     5095 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/auth_response.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     4177 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/conf.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13780 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3565 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3557 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10380 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2466 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/spcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/utils.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1190 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/urls.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     6333 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/utils.py
--rw-rw-r--   0 wert      (1000) wert      (1000)    33758 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/views.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/djangosaml2.egg-info/
--rw-rw-r--   0 wert      (1000) wert      (1000)     3017 2023-05-30 08:44:29.000000 djangosaml2-1.5.8/djangosaml2.egg-info/PKG-INFO
--rw-rw-r--   0 wert      (1000) wert      (1000)     2042 2023-05-30 08:44:29.000000 djangosaml2-1.5.8/djangosaml2.egg-info/SOURCES.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-05-30 08:44:29.000000 djangosaml2-1.5.8/djangosaml2.egg-info/dependency_links.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-05-30 08:44:29.000000 djangosaml2-1.5.8/djangosaml2.egg-info/not-zip-safe
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-30 08:44:29.000000 djangosaml2-1.5.8/djangosaml2.egg-info/requires.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)       12 2023-05-30 08:44:29.000000 djangosaml2-1.5.8/djangosaml2.egg-info/top_level.txt
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/docs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/docs/source/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/docs/source/_templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/docs/source/_templates/pplnx_template/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1829 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/docs/source/_templates/pplnx_template/footer.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1486 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/docs/source/_templates/pplnx_template/layout.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/lib/python3.10/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   278952 2023-05-30 08:44:24.000000 djangosaml2-1.5.8/env/lib/python3.10/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/jeepney/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/jeepney/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     4575 2023-05-30 08:44:24.000000 djangosaml2-1.5.8/env/lib/python3.10/site-packages/jeepney/tests/secrets_introspect.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   275233 2023-05-30 08:44:11.000000 djangosaml2-1.5.8/env/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2023-05-30 08:44:11.000000 djangosaml2-1.5.8/env/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      439 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/pyproject.toml
--rw-rw-r--   0 wert      (1000) wert      (1000)      197 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/setup.cfg
--rw-rw-r--   0 wert      (1000) wert      (1000)     2436 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/setup.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:01.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      268 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      527 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1200 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      385 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      310 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2339 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3656 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      316 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3043 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      395 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2983 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      370 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1569 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2397 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2312 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2405 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4324 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      330 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      188 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3181 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      437 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1870 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1444 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      553 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      358 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      245 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1020 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1024 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      568 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      346 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1454 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      374 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      671 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2046 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      505 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      669 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      582 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      966 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1333 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1313 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      734 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1824 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1322 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      995 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1747 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1703 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      896 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1682 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1867 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      479 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    16595 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2453 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/technical_404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    17182 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/technical_500.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:32:55.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:01.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:32:55.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:10.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/technical_404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/technical_500.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:06.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:06.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:20.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/technical_404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/technical_500.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:16.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:20.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:16.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/technical_404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/technical_500.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:25.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:25.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.7-django2.2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:39.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      268 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      527 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1200 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      385 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      310 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2339 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3656 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      316 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3043 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      395 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2983 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      370 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1569 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2397 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2312 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2405 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4324 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      330 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      188 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3181 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      437 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1870 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1444 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      553 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      358 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      245 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1020 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1024 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      568 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      346 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1454 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      374 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      671 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2046 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      505 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      669 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      582 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      966 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1333 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1313 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      734 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1824 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1322 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      995 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1747 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1703 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      896 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1682 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1867 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      479 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    16595 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2453 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/technical_404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    17182 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/technical_500.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:35.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:39.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:35.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/technical_404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/technical_500.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:44.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:44.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.1/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:58.000000 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:54.000000 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:54.000000 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13512 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/CHANGES
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11358 2021-01-23 23:44:15.000000 djangosaml2-1.6.0/COPYING
+-rw-rw-r--   0 wert      (1000) wert      (1000)      164 2021-01-23 23:44:15.000000 djangosaml2-1.6.0/MANIFEST.in
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3017 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/PKG-INFO
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1681 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/README.md
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)        0 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/__init__.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)      190 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/apps.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)    14380 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/backends.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2894 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/cache.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2568 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/conf.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)       51 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/exceptions.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3586 2023-06-19 16:48:07.000000 djangosaml2-1.6.0/djangosaml2/middleware.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1045 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/overrides.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)      726 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/signals.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/djangosaml2/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/djangosaml2/templates/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/templates/djangosaml2/login_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/templates/djangosaml2/wayf.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/djangosaml2/templatetags/
+-rw-rw-r--   0 wert      (1000) wert      (1000)        0 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/templatetags/__init__.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/templatetags/idplist.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/djangosaml2/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    43575 2023-06-19 16:48:07.000000 djangosaml2-1.6.0/djangosaml2/tests/__init__.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/djangosaml2/tests/attribute-maps/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      555 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/attribute-maps/django_saml_uri.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11106 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/attribute-maps/saml_uri.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     5095 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/auth_response.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4177 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/conf.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/idpcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/idpcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/idpcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/mycert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/mycert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/mycert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13780 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/remote_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3565 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3557 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    10380 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2466 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/sp_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/spcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/spcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/spcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/utils.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1190 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/urls.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     6333 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/utils.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)    33758 2023-06-19 16:48:07.000000 djangosaml2-1.6.0/djangosaml2/views.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/djangosaml2.egg-info/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3017 2023-06-19 17:02:20.000000 djangosaml2-1.6.0/djangosaml2.egg-info/PKG-INFO
+-rw-rw-r--   0 wert      (1000) wert      (1000)   111057 2023-06-19 17:02:21.000000 djangosaml2-1.6.0/djangosaml2.egg-info/SOURCES.txt
+-rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-06-19 17:02:20.000000 djangosaml2-1.6.0/djangosaml2.egg-info/dependency_links.txt
+-rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-06-19 17:02:20.000000 djangosaml2-1.6.0/djangosaml2.egg-info/not-zip-safe
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-06-19 17:02:20.000000 djangosaml2-1.6.0/djangosaml2.egg-info/requires.txt
+-rw-rw-r--   0 wert      (1000) wert      (1000)       12 2023-06-19 17:02:20.000000 djangosaml2-1.6.0/djangosaml2.egg-info/top_level.txt
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/docs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/docs/build/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/docs/build/html/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/docs/build/html/contents/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    12532 2023-06-19 16:49:08.000000 djangosaml2-1.6.0/docs/build/html/contents/developer.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     8498 2023-06-19 16:49:08.000000 djangosaml2-1.6.0/docs/build/html/contents/faq.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    15228 2023-06-19 16:49:08.000000 djangosaml2-1.6.0/docs/build/html/contents/miscellanea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    69252 2023-06-19 16:50:07.000000 djangosaml2-1.6.0/docs/build/html/contents/setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     8538 2023-06-19 16:49:08.000000 djangosaml2-1.6.0/docs/build/html/contents/usage.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     6153 2023-06-19 16:50:07.000000 djangosaml2-1.6.0/docs/build/html/genindex.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    12704 2023-06-19 16:50:07.000000 djangosaml2-1.6.0/docs/build/html/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     6552 2023-06-19 16:50:07.000000 djangosaml2-1.6.0/docs/build/html/search.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/docs/source/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/docs/source/_templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/docs/source/_templates/pplnx_template/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1829 2021-04-04 22:43:59.000000 djangosaml2-1.6.0/docs/source/_templates/pplnx_template/footer.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1488 2023-06-19 16:54:37.000000 djangosaml2-1.6.0/docs/source/_templates/pplnx_template/layout.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/docs/source/html/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/docs/source/html/contents/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    12532 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/contents/developer.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     8498 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/contents/faq.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    15228 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/contents/miscellanea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    69252 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/contents/setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     8538 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/contents/usage.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     6153 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/genindex.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    12704 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     6552 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/search.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   275233 2023-05-01 09:54:30.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/coverage/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/coverage/htmlfiles/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     5400 2023-05-01 09:54:30.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/coverage/htmlfiles/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     6434 2023-05-01 09:54:30.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/coverage/htmlfiles/pyfile.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      282 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      551 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/500.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1235 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/actions.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      389 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/app_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1716 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/app_list.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      320 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2515 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     6110 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/base.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      448 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/base_site.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3019 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      403 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3290 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1502 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list_results.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      697 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/color_theme_toggle.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      453 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2539 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2241 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2580 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4086 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      395 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/filter.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2200 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      192 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1849 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      447 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1899 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/login.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      486 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2136 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/object_history.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      549 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/pagination.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      327 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/popup_response.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      209 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1257 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/search_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1093 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/submit_line.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      618 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      339 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2096 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      238 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      218 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      425 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/logged_out.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      745 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_change_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2428 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      417 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1366 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      588 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      612 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      869 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      786 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      928 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/auth/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/auth/templates/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/auth/templates/auth/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      196 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      111 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1587 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/openlayers.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/templates/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/templates/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/sitemaps/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      683 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/sitemap.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      360 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       40 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      865 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/div.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/dict/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       49 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/dict/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      137 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/dict/ul.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/list/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       49 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/list/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      119 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/list/ul.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       77 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/div.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       84 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/p.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       88 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/table.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       85 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/ul.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      147 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/label.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      673 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/p.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      814 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/table.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      712 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/ul.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      395 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      365 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      110 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       40 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      874 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/div.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/dict/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/dict/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      137 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/dict/ul.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/list/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/list/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      118 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/list/ul.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       77 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       84 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/div.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       82 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/p.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/table.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       83 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/ul.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      122 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/label.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      684 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/p.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      825 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/table.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      723 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/ul.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      189 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      426 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      117 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      384 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      127 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/views/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/views/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11184 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/views/templates/default_urlconf.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/views/templates/technical_404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    17662 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/views/templates/technical_500.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/docutils-0.19.dist-info/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    26094 2023-05-01 09:54:30.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/docutils-0.19.dist-info/SOURCES.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2023-05-01 09:54:30.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/docutils-0.19.dist-info/dependency_links.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      969 2023-05-01 09:54:30.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/docutils-0.19.dist-info/top_level.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/jeepney/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/jeepney/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4575 2023-05-07 19:41:47.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/jeepney/tests/secrets_introspect.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   275233 2023-05-01 09:54:29.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/saml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/saml2/data/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/saml2/data/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      769 2023-05-01 09:55:04.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/saml2/data/templates/template_enc.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2023-05-01 09:54:28.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      439 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/pyproject.toml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      197 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/setup.cfg
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2436 2023-06-19 16:48:07.000000 djangosaml2-1.6.0/setup.py
```

### Comparing `djangosaml2-1.5.8/CHANGES` & `djangosaml2-1.6.0/CHANGES`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/COPYING` & `djangosaml2-1.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/PKG-INFO` & `djangosaml2-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangosaml2
-Version: 1.5.8
+Version: 1.6.0
 Summary: pysaml2 integration for Django
 Home-page: https://github.com/IdentityPython/djangosaml2
 Download-URL: https://pypi.org/project/djangosaml2/
 Author: Yaco Sistemas and independent contributors
 Author-email: lorenzo.gil.sanchez@gmail.com
 Maintainer: Giuseppe De Marco
 License: Apache 2.0
```

### Comparing `djangosaml2-1.5.8/README.md` & `djangosaml2-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/backends.py` & `djangosaml2-1.6.0/djangosaml2/backends.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/cache.py` & `djangosaml2-1.6.0/djangosaml2/cache.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/conf.py` & `djangosaml2-1.6.0/djangosaml2/conf.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/middleware.py` & `djangosaml2-1.6.0/djangosaml2/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,28 +22,30 @@
 
     def process_response(self, request, response):
         """
         If request.saml_session was modified, or if the configuration is to save the
         session every time, save the changes and set a session cookie or delete
         the session cookie if the session has been emptied.
         """
+        SAMESITE = getattr(settings, "SAML_SESSION_COOKIE_SAMESITE", SAMESITE_NONE)
+
         try:
             accessed = request.saml_session.accessed
             modified = request.saml_session.modified
             empty = request.saml_session.is_empty()
         except AttributeError:
             return response
         # First check if we need to delete this cookie.
         # The session should be deleted only if the session is entirely empty.
         if self.cookie_name in request.COOKIES and empty:
             response.delete_cookie(
                 self.cookie_name,
                 path=settings.SESSION_COOKIE_PATH,
                 domain=settings.SESSION_COOKIE_DOMAIN,
-                samesite=SAMESITE_NONE,
+                samesite=SAMESITE,
             )
             patch_vary_headers(response, ("Cookie",))
         else:
             if accessed:
                 patch_vary_headers(response, ("Cookie",))
             # relies and the global one
             if (modified or settings.SESSION_SAVE_EVERY_REQUEST) and not empty:
@@ -70,10 +72,10 @@
                         request.saml_session.session_key,
                         max_age=max_age,
                         expires=expires,
                         domain=settings.SESSION_COOKIE_DOMAIN,
                         path=settings.SESSION_COOKIE_PATH,
                         secure=settings.SESSION_COOKIE_SECURE or None,
                         httponly=settings.SESSION_COOKIE_HTTPONLY or None,
-                        samesite=SAMESITE_NONE,
+                        samesite=SAMESITE,
                     )
         return response
```

### Comparing `djangosaml2-1.5.8/djangosaml2/overrides.py` & `djangosaml2-1.6.0/djangosaml2/overrides.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/signals.py` & `djangosaml2-1.6.0/djangosaml2/signals.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/auth_error.html` & `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/echo_attributes.html` & `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/logout_error.html` & `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/wayf.html` & `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/templatetags/idplist.py` & `djangosaml2-1.6.0/djangosaml2/templatetags/idplist.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/__init__.py` & `djangosaml2-1.6.0/djangosaml2/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1026,7 +1026,35 @@
             response = middleware.process_response(request, response)
 
             cookie = response.cookies[saml_session_name]
 
             self.assertIsNotNone(cookie["expires"])
             self.assertNotEqual(cookie["expires"], "")
             self.assertNotEqual(cookie["max-age"], "")
+
+    def test_middleware_cookie_samesite(self):
+        with override_settings(SAML_SESSION_COOKIE_SAMESITE="Lax"):
+            session = self.get_session()
+            session.save()
+            self.set_session_cookies(session)
+
+            config_loader_path = "djangosaml2.tests.test_config_loader_with_real_conf"
+            request = RequestFactory().get("/login/")
+            request.user = AnonymousUser()
+            request.session = session
+            middleware = SamlSessionMiddleware(dummy_get_response)
+            middleware.process_request(request)
+
+            saml_session_name = getattr(
+                settings, "SAML_SESSION_COOKIE_NAME", "saml_session"
+            )
+            getattr(request, saml_session_name).save()
+
+            response = views.LoginView.as_view(config_loader_path=config_loader_path)(
+                request
+            )
+
+            response = middleware.process_response(request, response)
+
+            cookie = response.cookies[saml_session_name]
+
+            self.assertEqual(cookie["samesite"], "Lax")
```

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/attribute-maps/django_saml_uri.py` & `djangosaml2-1.6.0/djangosaml2/tests/attribute-maps/django_saml_uri.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/attribute-maps/saml_uri.py` & `djangosaml2-1.6.0/djangosaml2/tests/attribute-maps/saml_uri.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/auth_response.py` & `djangosaml2-1.6.0/djangosaml2/tests/auth_response.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/conf.py` & `djangosaml2-1.6.0/djangosaml2/tests/conf.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/idpcert.csr` & `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/idpcert.key` & `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/idpcert.pem` & `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/mycert.csr` & `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/mycert.key` & `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/mycert.pem` & `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/remote_metadata.xml` & `djangosaml2-1.6.0/djangosaml2/tests/remote_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_one_idp.xml` & `djangosaml2-1.6.0/djangosaml2/tests/remote_metadata_one_idp.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_post_binding.xml` & `djangosaml2-1.6.0/djangosaml2/tests/remote_metadata_post_binding.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_three_idps.xml` & `djangosaml2-1.6.0/djangosaml2/tests/remote_metadata_three_idps.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/sp_metadata.xml` & `djangosaml2-1.6.0/djangosaml2/tests/sp_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/spcert.csr` & `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/spcert.key` & `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/tests/spcert.pem` & `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/urls.py` & `djangosaml2-1.6.0/djangosaml2/urls.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/utils.py` & `djangosaml2-1.6.0/djangosaml2/utils.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2/views.py` & `djangosaml2-1.6.0/djangosaml2/views.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/djangosaml2.egg-info/PKG-INFO` & `djangosaml2-1.6.0/djangosaml2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangosaml2
-Version: 1.5.8
+Version: 1.6.0
 Summary: pysaml2 integration for Django
 Home-page: https://github.com/IdentityPython/djangosaml2
 Download-URL: https://pypi.org/project/djangosaml2/
 Author: Yaco Sistemas and independent contributors
 Author-email: lorenzo.gil.sanchez@gmail.com
 Maintainer: Giuseppe De Marco
 License: Apache 2.0
```

### Comparing `djangosaml2-1.5.8/docs/source/_templates/pplnx_template/footer.html` & `djangosaml2-1.6.0/docs/source/_templates/pplnx_template/footer.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/docs/source/_templates/pplnx_template/layout.html` & `djangosaml2-1.6.0/docs/source/_templates/pplnx_template/layout.html`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 {% block sidebartitle %}
 
 {% if logo %}
     {# Not strictly valid HTML, but it's the only way to display/scale
         it properly, without weird scripting or heaps of work
     #}
-    <a href="{{ pathto(master_doc) }}" id="logo_main"><img src="{{ pathto('_static/' + logo, 1) }}" class="logo" alt="Logo" /></a>
+    <a href="{{ pathto(master_doc) }}" id="logo_main"><img src="{{ pathto('_static/logo.jpg', 1) }}" class="logo" alt="Logo" /></a>
 {% endif %}
 
 {% if logo and theme_logo_only %}
     <a id="title_under_logo" href="{{ pathto(master_doc) }}">
 {% else %}
     <a id="title_under_logo" href="{{ pathto(master_doc) }}"> {{ project }}
 {% endif %}
@@ -41,13 +41,13 @@
 
 
 
 <!-- MOBILE TOP BAR OVERLOAD -->
 {% block mobile_nav %}
     <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
     <a href="{{ pathto(master_doc) }}">
-        <img src="{{ pathto('_static/' + logo, 1) }}" class="logo" alt="Logo"/>
+        <img src="{{ pathto('_static/logo.jpg', 1) }}" class="logo" alt="Logo"/>
         </a>
     <a href="{{ pathto(master_doc) }}">
         {{ project }}
     </a>
 {% endblock %}
```

### Comparing `djangosaml2-1.5.8/env/lib/python3.10/site-packages/certifi/cacert.pem` & `djangosaml2-1.6.0/env/lib/python3.10/site-packages/certifi/cacert.pem`

 * *Files 2% similar despite different names*

```diff
@@ -4521,69 +4521,7 @@
 AASkpW9gAwPDvTH00xecK4R1rOX9PVdu12O/5gSJko6BnOPpR27KkBLIE+Cnnfdl
 dB9sELLo5OnvbYUymUSxXv3MdhDYW72ixvnWQuRXdtyQwjWpS4g8EkdtXP9JTxpK
 ULGjQjBAMB0GA1UdDgQWBBSGHOf+LaVKiwj+KBH6vqNm+GBZLzAOBgNVHQ8BAf8E
 BAMCAQYwDwYDVR0TAQH/BAUwAwEB/zAKBggqhkjOPQQDAwNoADBlAjAVXUI9/Lbu
 9zuxNuie9sRGKEkz0FhDKmMpzE2xtHqiuQ04pV1IKv3LsnNdo4gIxwwCMQDAqy0O
 be0YottT6SXbVQjgUMzfRGEWgqtJsLKB7HOHeLRMsmIbEvoWTSVLY70eN9k=
 -----END CERTIFICATE-----
-
-# Issuer: CN=BJCA Global Root CA1 O=BEIJING CERTIFICATE AUTHORITY
-# Subject: CN=BJCA Global Root CA1 O=BEIJING CERTIFICATE AUTHORITY
-# Label: "BJCA Global Root CA1"
-# Serial: 113562791157148395269083148143378328608
-# MD5 Fingerprint: 42:32:99:76:43:33:36:24:35:07:82:9b:28:f9:d0:90
-# SHA1 Fingerprint: d5:ec:8d:7b:4c:ba:79:f4:e7:e8:cb:9d:6b:ae:77:83:10:03:21:6a
-# SHA256 Fingerprint: f3:89:6f:88:fe:7c:0a:88:27:66:a7:fa:6a:d2:74:9f:b5:7a:7f:3e:98:fb:76:9c:1f:a7:b0:9c:2c:44:d5:ae
------BEGIN CERTIFICATE-----
-MIIFdDCCA1ygAwIBAgIQVW9l47TZkGobCdFsPsBsIDANBgkqhkiG9w0BAQsFADBU
-MQswCQYDVQQGEwJDTjEmMCQGA1UECgwdQkVJSklORyBDRVJUSUZJQ0FURSBBVVRI
-T1JJVFkxHTAbBgNVBAMMFEJKQ0EgR2xvYmFsIFJvb3QgQ0ExMB4XDTE5MTIxOTAz
-MTYxN1oXDTQ0MTIxMjAzMTYxN1owVDELMAkGA1UEBhMCQ04xJjAkBgNVBAoMHUJF
-SUpJTkcgQ0VSVElGSUNBVEUgQVVUSE9SSVRZMR0wGwYDVQQDDBRCSkNBIEdsb2Jh
-bCBSb290IENBMTCCAiIwDQYJKoZIhvcNAQEBBQADggIPADCCAgoCggIBAPFmCL3Z
-xRVhy4QEQaVpN3cdwbB7+sN3SJATcmTRuHyQNZ0YeYjjlwE8R4HyDqKYDZ4/N+AZ
-spDyRhySsTphzvq3Rp4Dhtczbu33RYx2N95ulpH3134rhxfVizXuhJFyV9xgw8O5
-58dnJCNPYwpj9mZ9S1WnP3hkSWkSl+BMDdMJoDIwOvqfwPKcxRIqLhy1BDPapDgR
-at7GGPZHOiJBhyL8xIkoVNiMpTAK+BcWyqw3/XmnkRd4OJmtWO2y3syJfQOcs4ll
-5+M7sSKGjwZteAf9kRJ/sGsciQ35uMt0WwfCyPQ10WRjeulumijWML3mG90Vr4Tq
-nMfK9Q7q8l0ph49pczm+LiRvRSGsxdRpJQaDrXpIhRMsDQa4bHlW/KNnMoH1V6XK
-V0Jp6VwkYe/iMBhORJhVb3rCk9gZtt58R4oRTklH2yiUAguUSiz5EtBP6DF+bHq/
-pj+bOT0CFqMYs2esWz8sgytnOYFcuX6U1WTdno9uruh8W7TXakdI136z1C2OVnZO
-z2nxbkRs1CTqjSShGL+9V/6pmTW12xB3uD1IutbB5/EjPtffhZ0nPNRAvQoMvfXn
-jSXWgXSHRtQpdaJCbPdzied9v3pKH9MiyRVVz99vfFXQpIsHETdfg6YmV6YBW37+
-WGgHqel62bno/1Afq8K0wM7o6v0PvY1NuLxxAgMBAAGjQjBAMB0GA1UdDgQWBBTF
-7+3M2I0hxkjk49cULqcWk+WYATAPBgNVHRMBAf8EBTADAQH/MA4GA1UdDwEB/wQE
-AwIBBjANBgkqhkiG9w0BAQsFAAOCAgEAUoKsITQfI/Ki2Pm4rzc2IInRNwPWaZ+4
-YRC6ojGYWUfo0Q0lHhVBDOAqVdVXUsv45Mdpox1NcQJeXyFFYEhcCY5JEMEE3Kli
-awLwQ8hOnThJdMkycFRtwUf8jrQ2ntScvd0g1lPJGKm1Vrl2i5VnZu69mP6u775u
-+2D2/VnGKhs/I0qUJDAnyIm860Qkmss9vk/Ves6OF8tiwdneHg56/0OGNFK8YT88
-X7vZdrRTvJez/opMEi4r89fO4aL/3Xtw+zuhTaRjAv04l5U/BXCga99igUOLtFkN
-SoxUnMW7gZ/NfaXvCyUeOiDbHPwfmGcCCtRzRBPbUYQaVQNW4AB+dAb/OMRyHdOo
-P2gxXdMJxy6MW2Pg6Nwe0uxhHvLe5e/2mXZgLR6UcnHGCyoyx5JO1UbXHfmpGQrI
-+pXObSOYqgs4rZpWDW+N8TEAiMEXnM0ZNjX+VVOg4DwzX5Ze4jLp3zO7Bkqp2IRz
-znfSxqxx4VyjHQy7Ct9f4qNx2No3WqB4K/TUfet27fJhcKVlmtOJNBir+3I+17Q9
-eVzYH6Eze9mCUAyTF6ps3MKCuwJXNq+YJyo5UOGwifUll35HaBC07HPKs5fRJNz2
-YqAo07WjuGS3iGJCz51TzZm+ZGiPTx4SSPfSKcOYKMryMguTjClPPGAyzQWWYezy
-r/6zcCwupvI=
------END CERTIFICATE-----
-
-# Issuer: CN=BJCA Global Root CA2 O=BEIJING CERTIFICATE AUTHORITY
-# Subject: CN=BJCA Global Root CA2 O=BEIJING CERTIFICATE AUTHORITY
-# Label: "BJCA Global Root CA2"
-# Serial: 58605626836079930195615843123109055211
-# MD5 Fingerprint: 5e:0a:f6:47:5f:a6:14:e8:11:01:95:3f:4d:01:eb:3c
-# SHA1 Fingerprint: f4:27:86:eb:6e:b8:6d:88:31:67:02:fb:ba:66:a4:53:00:aa:7a:a6
-# SHA256 Fingerprint: 57:4d:f6:93:1e:27:80:39:66:7b:72:0a:fd:c1:60:0f:c2:7e:b6:6d:d3:09:29:79:fb:73:85:64:87:21:28:82
------BEGIN CERTIFICATE-----
-MIICJTCCAaugAwIBAgIQLBcIfWQqwP6FGFkGz7RK6zAKBggqhkjOPQQDAzBUMQsw
-CQYDVQQGEwJDTjEmMCQGA1UECgwdQkVJSklORyBDRVJUSUZJQ0FURSBBVVRIT1JJ
-VFkxHTAbBgNVBAMMFEJKQ0EgR2xvYmFsIFJvb3QgQ0EyMB4XDTE5MTIxOTAzMTgy
-MVoXDTQ0MTIxMjAzMTgyMVowVDELMAkGA1UEBhMCQ04xJjAkBgNVBAoMHUJFSUpJ
-TkcgQ0VSVElGSUNBVEUgQVVUSE9SSVRZMR0wGwYDVQQDDBRCSkNBIEdsb2JhbCBS
-b290IENBMjB2MBAGByqGSM49AgEGBSuBBAAiA2IABJ3LgJGNU2e1uVCxA/jlSR9B
-IgmwUVJY1is0j8USRhTFiy8shP8sbqjV8QnjAyEUxEM9fMEsxEtqSs3ph+B99iK+
-+kpRuDCK/eHeGBIK9ke35xe/J4rUQUyWPGCWwf0VHKNCMEAwHQYDVR0OBBYEFNJK
-sVF/BvDRgh9Obl+rg/xI1LCRMA8GA1UdEwEB/wQFMAMBAf8wDgYDVR0PAQH/BAQD
-AgEGMAoGCCqGSM49BAMDA2gAMGUCMBq8W9f+qdJUDkpd0m2xQNz0Q9XSSpkZElaA
-94M04TVOSG0ED1cxMDAtsaqdAzjbBgIxAMvMh1PLet8gUXOQwKhbYdDFUDn9hf7B
-43j4ptZLvZuHjw/l1lOWqzzIQNph91Oj9w==
------END CERTIFICATE-----
```

### Comparing `djangosaml2-1.5.8/env/lib/python3.10/site-packages/jeepney/tests/secrets_introspect.xml` & `djangosaml2-1.6.0/env/lib/python3.10/site-packages/jeepney/tests/secrets_introspect.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/env/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem` & `djangosaml2-1.6.0/env/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/env/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml` & `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.8/setup.py` & `djangosaml2-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     return codecs.open(
         os.path.join(os.path.dirname(__file__), *rnames), encoding="utf-8"
     ).read()
 
 
 setup(
     name="djangosaml2",
-    version="1.5.8",
+    version="1.6.0",
     description="pysaml2 integration for Django",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
```

