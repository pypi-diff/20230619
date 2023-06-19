# Comparing `tmp/design.plone.ioprenoto-1.0.7.tar.gz` & `tmp/design.plone.ioprenoto-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.ioprenoto-1.0.7.tar", last modified: Fri Jun 16 14:02:09 2023, max compression
+gzip compressed data, was "design.plone.ioprenoto-1.0.8.tar", last modified: Mon Jun 19 15:25:22 2023, max compression
```

## Comparing `design.plone.ioprenoto-1.0.7.tar` & `design.plone.ioprenoto-1.0.8.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.100741 design.plone.ioprenoto-1.0.7/
--rw-r--r--   0 folix      (503) staff       (20)      870 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/CHANGES.rst
--rw-r--r--   0 folix      (503) staff       (20)       58 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/CONTRIBUTORS.rst
--rw-r--r--   0 folix      (503) staff       (20)     1338 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/DEVELOP.rst
--rw-r--r--   0 folix      (503) staff       (20)      662 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/LICENSE.rst
--rw-r--r--   0 folix      (503) staff       (20)      116 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/MANIFEST.in
--rw-r--r--   0 folix      (503) staff       (20)     8226 2023-06-16 14:02:09.100992 design.plone.ioprenoto-1.0.7/PKG-INFO
--rw-r--r--   0 folix      (503) staff       (20)     4344 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/README.rst
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.077230 design.plone.ioprenoto-1.0.7/docs/
--rw-r--r--   0 folix      (503) staff       (20)     7986 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/docs/conf.py
--rw-r--r--   0 folix      (503) staff       (20)       89 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/docs/index.rst
--rw-r--r--   0 folix      (503) staff       (20)      340 2023-06-16 14:02:09.101726 design.plone.ioprenoto-1.0.7/setup.cfg
--rw-r--r--   0 folix      (503) staff       (20)     2774 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/setup.py
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.069104 design.plone.ioprenoto-1.0.7/src/
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.077583 design.plone.ioprenoto-1.0.7/src/design/
--rw-r--r--   0 folix      (503) staff       (20)       80 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/__init__.py
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.080777 design.plone.ioprenoto-1.0.7/src/design/plone/
--rw-r--r--   0 folix      (503) staff       (20)       80 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/__init__.py
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.082814 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/
--rw-r--r--   0 folix      (503) staff       (20)      139 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/__init__.py
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.084041 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/adapters/
--rw-r--r--   0 folix      (503) staff       (20)       24 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/adapters/__init__.py
--rw-r--r--   0 folix      (503) staff       (20)      562 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/adapters/configure.zcml
--rw-r--r--   0 folix      (503) staff       (20)     1015 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/adapters/stringinterp.py
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.085085 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/behaviors/
--rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/behaviors/__init__.py
--rw-r--r--   0 folix      (503) staff       (20)     1392 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/behaviors/additional_fields.py
--rw-r--r--   0 folix      (503) staff       (20)      591 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/behaviors/configure.zcml
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.085670 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/browser/
--rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/browser/__init__.py
--rw-r--r--   0 folix      (503) staff       (20)      628 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/browser/configure.zcml
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.085994 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/browser/overrides/
--rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/browser/overrides/.gitkeep
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.086276 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/browser/static/
--rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/browser/static/.gitkeep
--rw-r--r--   0 folix      (503) staff       (20)     1530 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/configure.zcml
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.087282 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/events/
--rw-r--r--   0 folix      (503) staff       (20)       24 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/events/__init__.py
--rw-r--r--   0 folix      (503) staff       (20)      724 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/events/configure.zcml
--rw-r--r--   0 folix      (503) staff       (20)     1463 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/events/on_create.py
--rw-r--r--   0 folix      (503) staff       (20)      270 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/interfaces.py
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.089012 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/
--rw-r--r--   0 folix      (503) staff       (20)      611 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/README.rst
--rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/__init__.py
--rw-r--r--   0 folix      (503) staff       (20)     1520 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.071062 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/en/
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.089404 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/
--rw-r--r--   0 folix      (503) staff       (20)     1395 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.071403 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/it/
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.089892 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/
--rw-r--r--   0 folix      (503) staff       (20)     1395 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po
--rw-r--r--   0 folix      (503) staff       (20)     1754 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/update.py
--rwxr-xr-x   0 folix      (503) staff       (20)      503 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/update.sh
--rw-r--r--   0 folix      (503) staff       (20)      273 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/permissions.zcml
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.072459 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/profiles/
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.091394 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/profiles/default/
--rw-r--r--   0 folix      (503) staff       (20)      191 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/profiles/default/browserlayer.xml
--rw-r--r--   0 folix      (503) staff       (20)      105 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/profiles/default/catalog.xml
--rw-r--r--   0 folix      (503) staff       (20)      191 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/profiles/default/metadata.xml
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.091777 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/profiles/default/registry/
--rw-r--r--   0 folix      (503) staff       (20)      180 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/profiles/default/registry/main.xml
--rw-r--r--   0 folix      (503) staff       (20)      340 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/profiles/default/rolemap.xml
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.092151 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/profiles/default/types/
--rw-r--r--   0 folix      (503) staff       (20)      325 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.092512 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/profiles/uninstall/
--rw-r--r--   0 folix      (503) staff       (20)      132 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.093245 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/
--rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/__init__.py
--rw-r--r--   0 folix      (503) staff       (20)      280 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/configure.zcml
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.093866 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/serializers/
--rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/serializers/__init__.py
--rw-r--r--   0 folix      (503) staff       (20)      166 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/serializers/configure.zcml
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.095296 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/serializers/ovverrides/
--rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
--rw-r--r--   0 folix      (503) staff       (20)      414 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
--rw-r--r--   0 folix      (503) staff       (20)     1685 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
--rw-r--r--   0 folix      (503) staff       (20)     2773 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.095636 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/services/
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.096417 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/services/bookable_list/
--rw-r--r--   0 folix      (503) staff       (20)      478 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
--rw-r--r--   0 folix      (503) staff       (20)     6155 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.097368 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/services/bookings/
--rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/services/bookings/__init__.py
--rw-r--r--   0 folix      (503) staff       (20)      354 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/services/bookings/configure.zcml
--rw-r--r--   0 folix      (503) staff       (20)      653 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/services/bookings/search.py
--rw-r--r--   0 folix      (503) staff       (20)      201 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/services/configure.zcml
--rw-r--r--   0 folix      (503) staff       (20)      794 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/setuphandlers.py
--rw-r--r--   0 folix      (503) staff       (20)     2326 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/testing.py
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.100072 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/
--rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/__init__.py
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.100420 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/robot/
--rw-r--r--   0 folix      (503) staff       (20)     2019 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/robot/test_example.robot
--rw-r--r--   0 folix      (503) staff       (20)     1231 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
--rw-r--r--   0 folix      (503) staff       (20)     2873 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/test_prenotazioni_messages.py
--rw-r--r--   0 folix      (503) staff       (20)     2221 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
--rw-r--r--   0 folix      (503) staff       (20)     2800 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py
--rw-r--r--   0 folix      (503) staff       (20)     7008 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py
--rw-r--r--   0 folix      (503) staff       (20)     2459 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/test_setup.py
--rw-r--r--   0 folix      (503) staff       (20)     4095 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py
-drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 14:02:09.080458 design.plone.ioprenoto-1.0.7/src/design.plone.ioprenoto.egg-info/
--rw-r--r--   0 folix      (503) staff       (20)     8226 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design.plone.ioprenoto.egg-info/PKG-INFO
--rw-r--r--   0 folix      (503) staff       (20)     3800 2023-06-16 14:02:09.000000 design.plone.ioprenoto-1.0.7/src/design.plone.ioprenoto.egg-info/SOURCES.txt
--rw-r--r--   0 folix      (503) staff       (20)        1 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design.plone.ioprenoto.egg-info/dependency_links.txt
--rw-r--r--   0 folix      (503) staff       (20)      147 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design.plone.ioprenoto.egg-info/entry_points.txt
--rw-r--r--   0 folix      (503) staff       (20)       20 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design.plone.ioprenoto.egg-info/namespace_packages.txt
--rw-r--r--   0 folix      (503) staff       (20)        1 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design.plone.ioprenoto.egg-info/not-zip-safe
--rw-r--r--   0 folix      (503) staff       (20)      293 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design.plone.ioprenoto.egg-info/requires.txt
--rw-r--r--   0 folix      (503) staff       (20)        7 2023-06-16 14:02:08.000000 design.plone.ioprenoto-1.0.7/src/design.plone.ioprenoto.egg-info/top_level.txt
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.569674 design.plone.ioprenoto-1.0.8/
+-rw-r--r--   0 roman      (502) staff       (20)      962 2023-06-19 15:25:21.000000 design.plone.ioprenoto-1.0.8/CHANGES.rst
+-rw-r--r--   0 roman      (502) staff       (20)       58 2023-06-19 15:25:21.000000 design.plone.ioprenoto-1.0.8/CONTRIBUTORS.rst
+-rw-r--r--   0 roman      (502) staff       (20)     1338 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/DEVELOP.rst
+-rw-r--r--   0 roman      (502) staff       (20)    18092 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/LICENSE.GPL
+-rw-r--r--   0 roman      (502) staff       (20)      662 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/LICENSE.rst
+-rw-r--r--   0 roman      (502) staff       (20)      116 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/MANIFEST.in
+-rw-r--r--   0 roman      (502) staff       (20)     8374 2023-06-19 15:25:22.569863 design.plone.ioprenoto-1.0.8/PKG-INFO
+-rw-r--r--   0 roman      (502) staff       (20)     4344 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/README.rst
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.552308 design.plone.ioprenoto-1.0.8/docs/
+-rw-r--r--   0 roman      (502) staff       (20)     7986 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/docs/conf.py
+-rw-r--r--   0 roman      (502) staff       (20)       89 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/docs/index.rst
+-rw-r--r--   0 roman      (502) staff       (20)      340 2023-06-19 15:25:22.570382 design.plone.ioprenoto-1.0.8/setup.cfg
+-rw-r--r--   0 roman      (502) staff       (20)     2774 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/setup.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.546064 design.plone.ioprenoto-1.0.8/src/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.552589 design.plone.ioprenoto-1.0.8/src/design/
+-rw-r--r--   0 roman      (502) staff       (20)       80 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/__init__.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.555019 design.plone.ioprenoto-1.0.8/src/design/plone/
+-rw-r--r--   0 roman      (502) staff       (20)       80 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/__init__.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.556735 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/
+-rw-r--r--   0 roman      (502) staff       (20)      139 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/__init__.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.557620 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/adapters/
+-rw-r--r--   0 roman      (502) staff       (20)       24 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/adapters/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      562 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/adapters/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     1015 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/adapters/stringinterp.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.558288 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/behaviors/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/behaviors/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1392 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/behaviors/additional_fields.py
+-rw-r--r--   0 roman      (502) staff       (20)      591 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/behaviors/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.558839 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/browser/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/browser/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      628 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/browser/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.559065 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/browser/overrides/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/browser/overrides/.gitkeep
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.559243 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/browser/static/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/browser/static/.gitkeep
+-rw-r--r--   0 roman      (502) staff       (20)     1530 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.559989 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/events/
+-rw-r--r--   0 roman      (502) staff       (20)       24 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/events/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      724 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/events/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     1592 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/events/on_create.py
+-rw-r--r--   0 roman      (502) staff       (20)      270 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/interfaces.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.561250 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/
+-rw-r--r--   0 roman      (502) staff       (20)      611 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/README.rst
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1520 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.547343 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/en/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.561511 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/
+-rw-r--r--   0 roman      (502) staff       (20)     1395 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.547582 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/it/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.561743 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/
+-rw-r--r--   0 roman      (502) staff       (20)     1395 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po
+-rw-r--r--   0 roman      (502) staff       (20)     1754 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/update.py
+-rwxr-xr-x   0 roman      (502) staff       (20)      503 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/update.sh
+-rw-r--r--   0 roman      (502) staff       (20)      273 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/permissions.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.548238 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/profiles/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.562856 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/profiles/default/
+-rw-r--r--   0 roman      (502) staff       (20)      191 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/profiles/default/browserlayer.xml
+-rw-r--r--   0 roman      (502) staff       (20)      105 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/profiles/default/catalog.xml
+-rw-r--r--   0 roman      (502) staff       (20)      191 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/profiles/default/metadata.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.563117 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/profiles/default/registry/
+-rw-r--r--   0 roman      (502) staff       (20)      180 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/profiles/default/registry/main.xml
+-rw-r--r--   0 roman      (502) staff       (20)      340 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/profiles/default/rolemap.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.563431 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/profiles/default/types/
+-rw-r--r--   0 roman      (502) staff       (20)      325 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.563657 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/profiles/uninstall/
+-rw-r--r--   0 roman      (502) staff       (20)      132 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.564054 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      280 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.564586 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/serializers/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/serializers/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      166 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/serializers/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.565568 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/serializers/ovverrides/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      414 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     1685 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
+-rw-r--r--   0 roman      (502) staff       (20)     2773 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.565837 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/services/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.566418 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/services/bookable_list/
+-rw-r--r--   0 roman      (502) staff       (20)      478 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     6155 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.567064 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/services/bookings/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/services/bookings/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      354 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/services/bookings/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)      653 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/services/bookings/search.py
+-rw-r--r--   0 roman      (502) staff       (20)      201 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/services/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)      794 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/setuphandlers.py
+-rw-r--r--   0 roman      (502) staff       (20)     2326 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/testing.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.569149 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/__init__.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.569404 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/robot/
+-rw-r--r--   0 roman      (502) staff       (20)     2019 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/robot/test_example.robot
+-rw-r--r--   0 roman      (502) staff       (20)     1231 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
+-rw-r--r--   0 roman      (502) staff       (20)     2873 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/test_prenotazioni_messages.py
+-rw-r--r--   0 roman      (502) staff       (20)     2221 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
+-rw-r--r--   0 roman      (502) staff       (20)     2800 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py
+-rw-r--r--   0 roman      (502) staff       (20)     7008 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py
+-rw-r--r--   0 roman      (502) staff       (20)     2459 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/test_setup.py
+-rw-r--r--   0 roman      (502) staff       (20)     4095 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:25:22.554806 design.plone.ioprenoto-1.0.8/src/design.plone.ioprenoto.egg-info/
+-rw-r--r--   0 roman      (502) staff       (20)     8374 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design.plone.ioprenoto.egg-info/PKG-INFO
+-rw-r--r--   0 roman      (502) staff       (20)     3812 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design.plone.ioprenoto.egg-info/SOURCES.txt
+-rw-r--r--   0 roman      (502) staff       (20)        1 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design.plone.ioprenoto.egg-info/dependency_links.txt
+-rw-r--r--   0 roman      (502) staff       (20)      147 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design.plone.ioprenoto.egg-info/entry_points.txt
+-rw-r--r--   0 roman      (502) staff       (20)       20 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design.plone.ioprenoto.egg-info/namespace_packages.txt
+-rw-r--r--   0 roman      (502) staff       (20)        1 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design.plone.ioprenoto.egg-info/not-zip-safe
+-rw-r--r--   0 roman      (502) staff       (20)      293 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design.plone.ioprenoto.egg-info/requires.txt
+-rw-r--r--   0 roman      (502) staff       (20)        7 2023-06-19 15:25:22.000000 design.plone.ioprenoto-1.0.8/src/design.plone.ioprenoto.egg-info/top_level.txt
```

### Comparing `design.plone.ioprenoto-1.0.7/CHANGES.rst` & `design.plone.ioprenoto-1.0.8/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.0.8 (2023-06-19)
+------------------
+
+- Edit prenotazione creation message.
+  [folix-01]
+
+
 1.0.7 (2023-06-16)
 ------------------
 
 - Add title to message created on prenotazione creation(#42314).
   [folix-01]
 
 1.0.6 (2023-06-16)
```

### Comparing `design.plone.ioprenoto-1.0.7/DEVELOP.rst` & `design.plone.ioprenoto-1.0.8/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/LICENSE.rst` & `design.plone.ioprenoto-1.0.8/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/PKG-INFO` & `design.plone.ioprenoto-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.ioprenoto
-Version: 1.0.7
+Version: 1.0.8
 Summary: An add-on for Plone
 Home-page: https://github.com/collective/design.plone.ioprenoto
 Author: RedTurtle
 Author-email: info@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/design.plone.ioprenoto/
 Project-URL: Source, https://github.com/RedTurtle/design.plone.ioprenoto
@@ -177,14 +177,21 @@
         - RedTurtle, info@redturtle.it
         
         
         Changelog
         =========
         
         
+        1.0.8 (2023-06-19)
+        ------------------
+        
+        - Edit prenotazione creation message.
+          [folix-01]
+        
+        
         1.0.7 (2023-06-16)
         ------------------
         
         - Add title to message created on prenotazione creation(#42314).
           [folix-01]
         
         1.0.6 (2023-06-16)
```

### Comparing `design.plone.ioprenoto-1.0.7/README.rst` & `design.plone.ioprenoto-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/docs/conf.py` & `design.plone.ioprenoto-1.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/setup.py` & `design.plone.ioprenoto-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.ioprenoto",
-    version="1.0.7",
+    version="1.0.8",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/adapters/configure.zcml` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/adapters/stringinterp.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/adapters/stringinterp.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/behaviors/additional_fields.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/behaviors/additional_fields.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/behaviors/configure.zcml` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/browser/configure.zcml` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/configure.zcml` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/events/configure.zcml` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/events/on_create.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/events/on_create.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,32 +15,36 @@
     """
     Create message on prenotazione creation
     """
     from design.plone.iocittadino.interfaces.store import (
         IMessageContentStore,
     )
 
+    portal_state = api.content.get_view(
+        name="plone_portal_state",
+        context=api.portal.get(),
+        request=getRequest(),
+    )
     booking_date = str(obj.booking_date and obj.booking_date.date() or "")
     booking_time = str(obj.booking_date and obj.booking_date.time() or "")
-    booking_print_url = "{folder}/@@prenotazione_print?uid={uid}".format(
-        folder=obj.getPrenotazioniFolder().absolute_url(), uid=obj.UID()
+    booking_print_url = "{root}?booking_id={uid}".format(
+        root=portal_state.navigation_root_url(), uid=obj.UID()
     )
 
     message_store = getMultiAdapter(
         (api.portal.get(), getRequest()), IMessageContentStore
     )
 
-    message_text = f"""La prenotazione per il {booking_date} alle {booking_time} è stata creata.
-                      Riceverete una mail di conferma quando la prenotazione verrà confermata definitivamente.
-                      Se non hai salvato o stampato il promemoria, puoi visualizzarlo a questo link: {booking_print_url}
-                    """
+    message_text = f"""La prenotazione per il {booking_date} alle {booking_time} è stata creata.\
+        Riceverete una mail di conferma quando la prenotazione verrà confermata definitivamente.\
+        Se non hai salvato o stampato il promemoria, puoi visualizzarlo a questo link: <a href={booking_print_url}>questo link</a>"""
 
     # message add here
     message_store.add(
         {
             "object_uid": obj.UID(),
-            "title": obj.booking_type,
+            "title": "Prenotazione appuntamento: " + obj.booking_type,
             "message": message_text,
             "state": "sent",
             "notify_on_email": False,
         }
     )
```

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/README.rst` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/locales/update.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/restapi/services/bookings/search.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/restapi/services/bookings/search.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/setuphandlers.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/testing.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/testing.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/robot/test_example.robot` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/test_prenotazioni_messages.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/test_prenotazioni_messages.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/test_setup.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py` & `design.plone.ioprenoto-1.0.8/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.7/src/design.plone.ioprenoto.egg-info/PKG-INFO` & `design.plone.ioprenoto-1.0.8/src/design.plone.ioprenoto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.ioprenoto
-Version: 1.0.7
+Version: 1.0.8
 Summary: An add-on for Plone
 Home-page: https://github.com/collective/design.plone.ioprenoto
 Author: RedTurtle
 Author-email: info@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/design.plone.ioprenoto/
 Project-URL: Source, https://github.com/RedTurtle/design.plone.ioprenoto
@@ -177,14 +177,21 @@
         - RedTurtle, info@redturtle.it
         
         
         Changelog
         =========
         
         
+        1.0.8 (2023-06-19)
+        ------------------
+        
+        - Edit prenotazione creation message.
+          [folix-01]
+        
+        
         1.0.7 (2023-06-16)
         ------------------
         
         - Add title to message created on prenotazione creation(#42314).
           [folix-01]
         
         1.0.6 (2023-06-16)
```

### Comparing `design.plone.ioprenoto-1.0.7/src/design.plone.ioprenoto.egg-info/SOURCES.txt` & `design.plone.ioprenoto-1.0.8/src/design.plone.ioprenoto.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CHANGES.rst
 CONTRIBUTORS.rst
 DEVELOP.rst
+LICENSE.GPL
 LICENSE.rst
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 docs/conf.py
 docs/index.rst
```

