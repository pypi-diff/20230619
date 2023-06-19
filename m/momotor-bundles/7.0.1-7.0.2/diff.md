# Comparing `tmp/momotor-bundles-7.0.1.tar.gz` & `tmp/momotor-bundles-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momotor-bundles-7.0.1.tar", last modified: Mon Nov 21 13:07:14 2022, max compression
+gzip compressed data, was "momotor-bundles-7.0.2.tar", last modified: Mon Jun 19 07:15:39 2023, max compression
```

## Comparing `momotor-bundles-7.0.1.tar` & `momotor-bundles-7.0.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2527 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1468 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2387 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor/bundles/
--rw-rw-rw-   0 root         (0) root         (0)      228 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18402 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor/bundles/binding/
--rw-rw-rw-   0 root         (0) root         (0)     1815 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/binding/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25198 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/binding/momotor_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/binding/xml.py
--rw-rw-rw-   0 root         (0) root         (0)     2858 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/config.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor/bundles/elements/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-21 13:06:40.000000 momotor-bundles-7.0.1/src/momotor/bundles/elements/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7209 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/elements/base.py
--rw-rw-rw-   0 root         (0) root         (0)    15829 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/elements/checklets.py
--rw-rw-rw-   0 root         (0) root         (0)    27589 2022-10-06 08:41:07.000000 momotor-bundles-7.0.1/src/momotor/bundles/elements/content.py
--rw-rw-rw-   0 root         (0) root         (0)    12932 2022-10-06 08:41:07.000000 momotor-bundles-7.0.1/src/momotor/bundles/elements/files.py
--rw-rw-rw-   0 root         (0) root         (0)     9813 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/elements/options.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/elements/properties.py
--rw-rw-rw-   0 root         (0) root         (0)     1477 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/elements/refs.py
--rw-rw-rw-   0 root         (0) root         (0)     5309 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/elements/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     9882 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/elements/result.py
--rw-rw-rw-   0 root         (0) root         (0)     4322 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/elements/results.py
--rw-rw-rw-   0 root         (0) root         (0)    10566 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/elements/steps.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/elements/wildcard.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor/bundles/mixins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-21 13:06:40.000000 momotor-bundles-7.0.1/src/momotor/bundles/mixins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21723 2022-11-21 13:06:40.000000 momotor-bundles-7.0.1/src/momotor/bundles/mixins/attachments.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/mixins/id.py
--rw-rw-rw-   0 root         (0) root         (0)     1823 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/mixins/name.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor/bundles/parsers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-21 13:06:40.000000 momotor-bundles-7.0.1/src/momotor/bundles/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      315 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/parsers/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor/bundles/parsers/handlers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-21 13:06:40.000000 momotor-bundles-7.0.1/src/momotor/bundles/parsers/handlers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/parsers/handlers/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2244 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/parsers/handlers/lxml.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/parsers/handlers/xml.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/parsers/xml.py
--rw-rw-rw-   0 root         (0) root         (0)     3268 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/product.py
--rw-rw-rw-   0 root         (0) root         (0)     6125 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/recipe.py
--rw-rw-rw-   0 root         (0) root         (0)     2782 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/results.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor/bundles/schema/
--rw-rw-rw-   0 root         (0) root         (0)    14077 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/schema/momotor-1.0.xsd
--rw-rw-rw-   0 root         (0) root         (0)     8836 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/schema/xml.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor/bundles/serializers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-21 13:06:40.000000 momotor-bundles-7.0.1/src/momotor/bundles/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/serializers/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor/bundles/serializers/writers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-21 13:06:40.000000 momotor-bundles-7.0.1/src/momotor/bundles/serializers/writers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/serializers/writers/lxml.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/serializers/writers/xml.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/serializers/xml.py
--rw-rw-rw-   0 root         (0) root         (0)     3996 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/testresult.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor/bundles/typing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-21 13:06:40.000000 momotor-bundles-7.0.1/src/momotor/bundles/typing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/typing/element.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-21 13:06:40.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2895 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)      642 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/ascii.py
--rw-rw-rw-   0 root         (0) root         (0)     5284 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/assertion.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/boolean.py
--rw-rw-rw-   0 root         (0) root         (0)     4350 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/detect.py
--rw-rw-rw-   0 root         (0) root         (0)     3434 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/domain.py
--rw-rw-rw-   0 root         (0) root         (0)     4222 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/encoding.py
--rw-rw-rw-   0 root         (0) root         (0)    12914 2022-09-29 07:20:13.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/grouping.py
--rw-rw-rw-   0 root         (0) root         (0)     2198 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/immutable.py
--rw-rw-rw-   0 root         (0) root         (0)     5947 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/keyedtuple.py
--rw-rw-rw-   0 root         (0) root         (0)      997 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/lxml.py
--rw-rw-rw-   0 root         (0) root         (0)     1339 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     4362 2022-09-29 07:20:13.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/rglob.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/text.py
--rw-rw-rw-   0 root         (0) root         (0)     1805 2022-03-24 09:30:06.000000 momotor-bundles-7.0.1/src/momotor/bundles/utils/zipwrapper.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-11-21 13:06:31.000000 momotor-bundles-7.0.1/src/momotor/bundles/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor_bundles.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2527 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor_bundles.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2739 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor_bundles.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor_bundles.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor_bundles.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      253 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor_bundles.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-11-21 13:07:14.000000 momotor-bundles-7.0.1/src/momotor_bundles.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2527 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1468 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor/bundles/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18402 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor/bundles/binding/
+-rw-rw-rw-   0 root         (0) root         (0)     1815 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/binding/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25198 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/binding/momotor_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/binding/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)     2858 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor/bundles/elements/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 07:15:12.000000 momotor-bundles-7.0.2/src/momotor/bundles/elements/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7209 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/elements/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    15829 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/elements/checklets.py
+-rw-rw-rw-   0 root         (0) root         (0)    27589 2022-10-06 08:41:07.000000 momotor-bundles-7.0.2/src/momotor/bundles/elements/content.py
+-rw-rw-rw-   0 root         (0) root         (0)    12920 2023-06-19 07:15:12.000000 momotor-bundles-7.0.2/src/momotor/bundles/elements/files.py
+-rw-rw-rw-   0 root         (0) root         (0)     9813 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/elements/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/elements/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/elements/refs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5309 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/elements/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     9882 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/elements/result.py
+-rw-rw-rw-   0 root         (0) root         (0)     4322 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/elements/results.py
+-rw-rw-rw-   0 root         (0) root         (0)    10566 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/elements/steps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/elements/wildcard.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor/bundles/mixins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 07:15:12.000000 momotor-bundles-7.0.2/src/momotor/bundles/mixins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21723 2023-06-19 07:15:12.000000 momotor-bundles-7.0.2/src/momotor/bundles/mixins/attachments.py
+-rw-rw-rw-   0 root         (0) root         (0)      748 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/mixins/id.py
+-rw-rw-rw-   0 root         (0) root         (0)     1823 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/mixins/name.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor/bundles/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 07:15:12.000000 momotor-bundles-7.0.2/src/momotor/bundles/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      315 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/parsers/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor/bundles/parsers/handlers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 07:15:12.000000 momotor-bundles-7.0.2/src/momotor/bundles/parsers/handlers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       45 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/parsers/handlers/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/parsers/handlers/lxml.py
+-rw-rw-rw-   0 root         (0) root         (0)      648 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/parsers/handlers/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/parsers/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)     3268 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/product.py
+-rw-rw-rw-   0 root         (0) root         (0)     6125 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/recipe.py
+-rw-rw-rw-   0 root         (0) root         (0)     2782 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/results.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor/bundles/schema/
+-rw-rw-rw-   0 root         (0) root         (0)    14077 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/schema/momotor-1.0.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     8836 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/schema/xml.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor/bundles/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 07:15:12.000000 momotor-bundles-7.0.2/src/momotor/bundles/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/serializers/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor/bundles/serializers/writers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 07:15:12.000000 momotor-bundles-7.0.2/src/momotor/bundles/serializers/writers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/serializers/writers/lxml.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/serializers/writers/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/serializers/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)     3996 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/testresult.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor/bundles/typing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 07:15:12.000000 momotor-bundles-7.0.2/src/momotor/bundles/typing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/typing/element.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 07:15:12.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2895 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)      642 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/ascii.py
+-rw-rw-rw-   0 root         (0) root         (0)     5284 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/assertion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/boolean.py
+-rw-rw-rw-   0 root         (0) root         (0)     4350 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/detect.py
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     4222 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/encoding.py
+-rw-rw-rw-   0 root         (0) root         (0)    12914 2022-09-29 07:20:13.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/grouping.py
+-rw-rw-rw-   0 root         (0) root         (0)     2198 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/immutable.py
+-rw-rw-rw-   0 root         (0) root         (0)     5947 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/keyedtuple.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/lxml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4362 2022-09-29 07:20:13.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/rglob.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/text.py
+-rw-rw-rw-   0 root         (0) root         (0)     1805 2022-03-24 09:30:06.000000 momotor-bundles-7.0.2/src/momotor/bundles/utils/zipwrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-19 07:15:04.000000 momotor-bundles-7.0.2/src/momotor/bundles/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor_bundles.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2527 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor_bundles.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor_bundles.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor_bundles.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor_bundles.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      253 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor_bundles.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-19 07:15:39.000000 momotor-bundles-7.0.2/src/momotor_bundles.egg-info/top_level.txt
```

### Comparing `momotor-bundles-7.0.1/LICENSE.txt` & `momotor-bundles-7.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/PKG-INFO` & `momotor-bundles-7.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: momotor-bundles
-Version: 7.0.1
+Version: 7.0.2
 Summary: Momotor bundle reader, writer, tools
 Home-page: https://momotor.org/
 Author: Erik Scheffers
 Author-email: e.t.j.scheffers@tue.nl
-Project-URL: Documentation, https://momotor.org/doc/engine/momotor-bundles/release/7.0.1/
+Project-URL: Documentation, https://momotor.org/doc/engine/momotor-bundles/release/7.0.2/
 Project-URL: Source, https://gitlab.tue.nl/momotor/engine-py3/momotor-bundles/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-bundles/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `momotor-bundles-7.0.1/README.md` & `momotor-bundles-7.0.2/README.md`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/setup.py` & `momotor-bundles-7.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/base.py` & `momotor-bundles-7.0.2/src/momotor/bundles/base.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/binding/__init__.py` & `momotor-bundles-7.0.2/src/momotor/bundles/binding/__init__.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/binding/momotor_1_0.py` & `momotor-bundles-7.0.2/src/momotor/bundles/binding/momotor_1_0.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/config.py` & `momotor-bundles-7.0.2/src/momotor/bundles/config.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/elements/base.py` & `momotor-bundles-7.0.2/src/momotor/bundles/elements/base.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/elements/checklets.py` & `momotor-bundles-7.0.2/src/momotor/bundles/elements/checklets.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/elements/content.py` & `momotor-bundles-7.0.2/src/momotor/bundles/elements/content.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/elements/files.py` & `momotor-bundles-7.0.2/src/momotor/bundles/elements/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
 
     def copy_to(self, destination: Path, *,
                 name: typing.Union[PurePath, str] = None,
                 executable_attribute: bool = False) -> PurePath:
 
         dest_path = super().copy_to(destination, name=name)
 
-        if executable_attribute and self.attr.get('executable'):
+        if executable_attribute and self.executable:
             # Set executable bits
             import stat
             dest_path.chmod(dest_path.stat().st_mode | stat.S_IXUSR | stat.S_IXGRP | stat.S_IXOTH)
 
         return dest_path
```

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/elements/options.py` & `momotor-bundles-7.0.2/src/momotor/bundles/elements/options.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/elements/properties.py` & `momotor-bundles-7.0.2/src/momotor/bundles/elements/properties.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/elements/refs.py` & `momotor-bundles-7.0.2/src/momotor/bundles/elements/refs.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/elements/resources.py` & `momotor-bundles-7.0.2/src/momotor/bundles/elements/resources.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/elements/result.py` & `momotor-bundles-7.0.2/src/momotor/bundles/elements/result.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/elements/results.py` & `momotor-bundles-7.0.2/src/momotor/bundles/elements/results.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/elements/steps.py` & `momotor-bundles-7.0.2/src/momotor/bundles/elements/steps.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/elements/wildcard.py` & `momotor-bundles-7.0.2/src/momotor/bundles/elements/wildcard.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/mixins/attachments.py` & `momotor-bundles-7.0.2/src/momotor/bundles/mixins/attachments.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/mixins/id.py` & `momotor-bundles-7.0.2/src/momotor/bundles/mixins/id.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/mixins/name.py` & `momotor-bundles-7.0.2/src/momotor/bundles/mixins/name.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/parsers/handlers/lxml.py` & `momotor-bundles-7.0.2/src/momotor/bundles/parsers/handlers/lxml.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/parsers/handlers/xml.py` & `momotor-bundles-7.0.2/src/momotor/bundles/parsers/handlers/xml.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/parsers/xml.py` & `momotor-bundles-7.0.2/src/momotor/bundles/parsers/xml.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/product.py` & `momotor-bundles-7.0.2/src/momotor/bundles/product.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/recipe.py` & `momotor-bundles-7.0.2/src/momotor/bundles/recipe.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/results.py` & `momotor-bundles-7.0.2/src/momotor/bundles/results.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/schema/momotor-1.0.xsd` & `momotor-bundles-7.0.2/src/momotor/bundles/schema/momotor-1.0.xsd`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/schema/xml.xsd` & `momotor-bundles-7.0.2/src/momotor/bundles/schema/xml.xsd`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/testresult.py` & `momotor-bundles-7.0.2/src/momotor/bundles/testresult.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/arguments.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/arguments.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/ascii.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/ascii.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/assertion.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/assertion.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/boolean.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/boolean.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/detect.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/detect.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/domain.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/domain.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/encoding.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/filters.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/filters.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/grouping.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/grouping.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/immutable.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/immutable.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/keyedtuple.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/keyedtuple.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/lxml.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/lxml.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/nodes.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/nodes.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/rglob.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/rglob.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/text.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/text.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor/bundles/utils/zipwrapper.py` & `momotor-bundles-7.0.2/src/momotor/bundles/utils/zipwrapper.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-7.0.1/src/momotor_bundles.egg-info/PKG-INFO` & `momotor-bundles-7.0.2/src/momotor_bundles.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: momotor-bundles
-Version: 7.0.1
+Version: 7.0.2
 Summary: Momotor bundle reader, writer, tools
 Home-page: https://momotor.org/
 Author: Erik Scheffers
 Author-email: e.t.j.scheffers@tue.nl
-Project-URL: Documentation, https://momotor.org/doc/engine/momotor-bundles/release/7.0.1/
+Project-URL: Documentation, https://momotor.org/doc/engine/momotor-bundles/release/7.0.2/
 Project-URL: Source, https://gitlab.tue.nl/momotor/engine-py3/momotor-bundles/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-bundles/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `momotor-bundles-7.0.1/src/momotor_bundles.egg-info/SOURCES.txt` & `momotor-bundles-7.0.2/src/momotor_bundles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

