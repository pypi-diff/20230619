# Comparing `tmp/wfuzzserver-3.2.0.tar.gz` & `tmp/wfuzzserver-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wfuzzserver-3.2.0.tar", last modified: Mon Jun 19 04:59:42 2023, max compression
+gzip compressed data, was "wfuzzserver-3.3.0.tar", last modified: Mon Jun 19 05:46:09 2023, max compression
```

## Comparing `wfuzzserver-3.2.0.tar` & `wfuzzserver-3.3.0.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.705182 wfuzzserver-3.2.0/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)    18027 2023-06-19 02:50:09.000000 wfuzzserver-3.2.0/LICENSE
--rw-rw-r--   0 hussam    (1000) hussam    (1000)       49 2023-06-19 02:50:09.000000 wfuzzserver-3.2.0/MANIFEST.in
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     3653 2023-06-19 04:59:42.705182 wfuzzserver-3.2.0/PKG-INFO
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2419 2023-06-19 02:50:09.000000 wfuzzserver-3.2.0/README.md
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.693182 wfuzzserver-3.2.0/docs/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)      602 2023-06-19 02:50:09.000000 wfuzzserver-3.2.0/docs/Makefile
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     5032 2023-06-19 02:50:09.000000 wfuzzserver-3.2.0/docs/conf.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     5503 2023-06-19 02:50:09.000000 wfuzzserver-3.2.0/docs/index.rst
--rw-rw-r--   0 hussam    (1000) hussam    (1000)      809 2023-06-19 02:50:09.000000 wfuzzserver-3.2.0/docs/make.bat
--rw-rw-r--   0 hussam    (1000) hussam    (1000)       38 2023-06-19 04:59:42.705182 wfuzzserver-3.2.0/setup.cfg
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2693 2023-06-19 04:56:46.000000 wfuzzserver-3.2.0/setup.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.689182 wfuzzserver-3.2.0/src/
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.693182 wfuzzserver-3.2.0/src/wfuzzserver/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1667 2023-06-19 04:52:59.000000 wfuzzserver-3.2.0/src/wfuzzserver/__init__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)       32 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/__main__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)      725 2023-06-19 04:42:09.000000 wfuzzserver-3.2.0/src/wfuzzserver/api.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     4251 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/core.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     4718 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/dictionaries.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)      820 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/exception.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.693182 wfuzzserver-3.2.0/src/wfuzzserver/externals/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/externals/__init__.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.693182 wfuzzserver-3.2.0/src/wfuzzserver/externals/moduleman/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/externals/moduleman/__init__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     5152 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/externals/moduleman/loader.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     4797 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/externals/moduleman/modulefilter.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)      552 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/externals/moduleman/plugin.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     4670 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/externals/moduleman/registrant.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.693182 wfuzzserver-3.2.0/src/wfuzzserver/externals/reqresp/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)    15929 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/externals/reqresp/Request.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     7262 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/externals/reqresp/Response.py
--rwxrwxr-x   0 hussam    (1000) hussam    (1000)     4204 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/externals/reqresp/TextParser.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     3685 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/externals/reqresp/Variables.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)       60 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/externals/reqresp/__init__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)      713 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/externals/reqresp/cache.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)      244 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/externals/reqresp/exceptions.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.697182 wfuzzserver-3.2.0/src/wfuzzserver/externals/settings/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/externals/settings/__init__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2680 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/externals/settings/settings.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     3285 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/facade.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.697182 wfuzzserver-3.2.0/src/wfuzzserver/factories/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/factories/__init__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     4015 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/factories/dictfactory.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)      903 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/factories/fuzzfactory.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     4150 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/factories/fuzzresfactory.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1416 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/factories/payman.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1905 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/factories/plugin_factory.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     4019 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/factories/reqresp_factory.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.697182 wfuzzserver-3.2.0/src/wfuzzserver/filters/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/filters/__init__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)    13771 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/filters/ppfilter.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     3567 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/filters/simplefilter.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)    11996 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/fuzzobjects.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)    14220 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/fuzzqueues.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)    11147 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/fuzzrequest.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.697182 wfuzzserver-3.2.0/src/wfuzzserver/helpers/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/helpers/__init__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     4484 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/helpers/file_func.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2161 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/helpers/obj_dic.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2627 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/helpers/obj_dyn.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     4429 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/helpers/obj_factory.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2893 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/helpers/str_func.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)      701 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/helpers/utils.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1481 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/mixins.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     8028 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/myhttp.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     9891 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/myqueues.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)    12920 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/options.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.697182 wfuzzserver-3.2.0/src/wfuzzserver/plugin_api/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugin_api/__init__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     5264 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugin_api/base.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)      344 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugin_api/mixins.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)    12744 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugin_api/payloadtools.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2830 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugin_api/urlutils.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.697182 wfuzzserver-3.2.0/src/wfuzzserver/plugins/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/__init__.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.697182 wfuzzserver-3.2.0/src/wfuzzserver/plugins/encoders/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/encoders/__init__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)    14774 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/encoders/encoders.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.697182 wfuzzserver-3.2.0/src/wfuzzserver/plugins/iterators/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/iterators/__init__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2360 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/iterators/iterations.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.701182 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/__init__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2526 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/autorize.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1311 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/bing.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1022 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/buffer_overflow.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2529 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/burpitem.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     4170 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/burplog.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     8146 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/burpstate.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1513 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/dirwalk.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1930 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/file.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1338 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/guitab.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1660 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/hexrand.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1685 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/hexrange.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1787 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/ipnet.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1741 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/iprange.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1630 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/list.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     3300 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/names.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1733 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/permutation.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1659 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/range.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1626 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/shodanp.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)      768 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/stdin.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2307 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/wfuzzp.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.701182 wfuzzserver-3.2.0/src/wfuzzserver/plugins/printers/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/printers/__init__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)    13490 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/printers/printers.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.701182 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/__init__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2080 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/backups.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1144 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/cookies.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1636 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/cvs_extractor.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     4140 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/errors.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1217 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/grep.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     5102 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/headers.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     5945 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/links.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1803 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/listing.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1692 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/npm_deps.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1824 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/robots.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1410 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/screenshot.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     1230 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/sitemap.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2211 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/svn_extractor.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)      893 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/title.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2508 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/wcdb.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.701182 wfuzzserver-3.2.0/src/wfuzzserver/ui/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/ui/__init__.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.701182 wfuzzserver-3.2.0/src/wfuzzserver/ui/console/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/ui/console/__init__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)    20246 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/ui/console/clparser.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)    15081 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/ui/console/common.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2634 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/ui/console/getch.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)    10791 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/ui/console/mvc.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     6657 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/ui/console/output.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.701182 wfuzzserver-3.2.0/src/wfuzzserver/ui/gui/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/ui/gui/__init__.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     2256 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/ui/gui/controller.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)    10862 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/ui/gui/guicontrols.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     3032 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/ui/gui/model.py
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     6755 2023-06-19 03:18:25.000000 wfuzzserver-3.2.0/src/wfuzzserver/wfuzz.py
-drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 04:59:42.705182 wfuzzserver-3.2.0/wfuzzserver.egg-info/
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     3653 2023-06-19 04:59:42.000000 wfuzzserver-3.2.0/wfuzzserver.egg-info/PKG-INFO
--rw-rw-r--   0 hussam    (1000) hussam    (1000)     4583 2023-06-19 04:59:42.000000 wfuzzserver-3.2.0/wfuzzserver.egg-info/SOURCES.txt
--rw-rw-r--   0 hussam    (1000) hussam    (1000)        1 2023-06-19 04:59:42.000000 wfuzzserver-3.2.0/wfuzzserver.egg-info/dependency_links.txt
--rw-rw-r--   0 hussam    (1000) hussam    (1000)      209 2023-06-19 04:59:42.000000 wfuzzserver-3.2.0/wfuzzserver.egg-info/entry_points.txt
--rw-rw-r--   0 hussam    (1000) hussam    (1000)      275 2023-06-19 04:59:42.000000 wfuzzserver-3.2.0/wfuzzserver.egg-info/requires.txt
--rw-rw-r--   0 hussam    (1000) hussam    (1000)       12 2023-06-19 04:59:42.000000 wfuzzserver-3.2.0/wfuzzserver.egg-info/top_level.txt
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.512912 wfuzzserver-3.3.0/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)    18027 2023-06-19 02:50:09.000000 wfuzzserver-3.3.0/LICENSE
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)       49 2023-06-19 02:50:09.000000 wfuzzserver-3.3.0/MANIFEST.in
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     3653 2023-06-19 05:46:09.512912 wfuzzserver-3.3.0/PKG-INFO
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2419 2023-06-19 02:50:09.000000 wfuzzserver-3.3.0/README.md
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.500912 wfuzzserver-3.3.0/docs/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)      602 2023-06-19 02:50:09.000000 wfuzzserver-3.3.0/docs/Makefile
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     5032 2023-06-19 02:50:09.000000 wfuzzserver-3.3.0/docs/conf.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     5503 2023-06-19 02:50:09.000000 wfuzzserver-3.3.0/docs/index.rst
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)      809 2023-06-19 02:50:09.000000 wfuzzserver-3.3.0/docs/make.bat
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)       38 2023-06-19 05:46:09.512912 wfuzzserver-3.3.0/setup.cfg
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2693 2023-06-19 05:44:41.000000 wfuzzserver-3.3.0/setup.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.496912 wfuzzserver-3.3.0/src/
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.500912 wfuzzserver-3.3.0/src/wfuzzserver/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1667 2023-06-19 05:43:56.000000 wfuzzserver-3.3.0/src/wfuzzserver/__init__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)       38 2023-06-19 05:36:31.000000 wfuzzserver-3.3.0/src/wfuzzserver/__main__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)      731 2023-06-19 05:36:01.000000 wfuzzserver-3.3.0/src/wfuzzserver/api.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     4251 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/core.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     4718 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/dictionaries.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)      820 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/exception.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.500912 wfuzzserver-3.3.0/src/wfuzzserver/externals/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/externals/__init__.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.500912 wfuzzserver-3.3.0/src/wfuzzserver/externals/moduleman/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/externals/moduleman/__init__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     5152 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/externals/moduleman/loader.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     4797 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/externals/moduleman/modulefilter.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)      552 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/externals/moduleman/plugin.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     4670 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/externals/moduleman/registrant.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.504912 wfuzzserver-3.3.0/src/wfuzzserver/externals/reqresp/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)    15929 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/externals/reqresp/Request.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     7262 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/externals/reqresp/Response.py
+-rwxrwxr-x   0 hussam    (1000) hussam    (1000)     4204 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/externals/reqresp/TextParser.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     3685 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/externals/reqresp/Variables.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)       60 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/externals/reqresp/__init__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)      713 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/externals/reqresp/cache.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)      244 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/externals/reqresp/exceptions.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.504912 wfuzzserver-3.3.0/src/wfuzzserver/externals/settings/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/externals/settings/__init__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2680 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/externals/settings/settings.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     3285 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/facade.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.504912 wfuzzserver-3.3.0/src/wfuzzserver/factories/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/factories/__init__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     4015 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/factories/dictfactory.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)      903 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/factories/fuzzfactory.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     4150 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/factories/fuzzresfactory.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1416 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/factories/payman.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1905 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/factories/plugin_factory.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     4019 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/factories/reqresp_factory.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.504912 wfuzzserver-3.3.0/src/wfuzzserver/filters/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/filters/__init__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)    13771 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/filters/ppfilter.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     3567 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/filters/simplefilter.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)    11996 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/fuzzobjects.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)    14220 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/fuzzqueues.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)    11147 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/fuzzrequest.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.504912 wfuzzserver-3.3.0/src/wfuzzserver/helpers/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/helpers/__init__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     4502 2023-06-19 05:35:00.000000 wfuzzserver-3.3.0/src/wfuzzserver/helpers/file_func.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2161 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/helpers/obj_dic.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2627 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/helpers/obj_dyn.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     4429 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/helpers/obj_factory.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2893 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/helpers/str_func.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)      701 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/helpers/utils.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1481 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/mixins.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     8028 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/myhttp.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     9891 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/myqueues.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)    12920 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/options.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.504912 wfuzzserver-3.3.0/src/wfuzzserver/plugin_api/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugin_api/__init__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     5264 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugin_api/base.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)      344 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugin_api/mixins.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)    12750 2023-06-19 05:42:12.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugin_api/payloadtools.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2830 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugin_api/urlutils.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.504912 wfuzzserver-3.3.0/src/wfuzzserver/plugins/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/__init__.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.504912 wfuzzserver-3.3.0/src/wfuzzserver/plugins/encoders/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/encoders/__init__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)    14774 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/encoders/encoders.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.504912 wfuzzserver-3.3.0/src/wfuzzserver/plugins/iterators/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/iterators/__init__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2360 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/iterators/iterations.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.508912 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/__init__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2526 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/autorize.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1311 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/bing.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1022 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/buffer_overflow.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2529 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/burpitem.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     4170 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/burplog.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     8146 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/burpstate.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1513 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/dirwalk.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1930 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/file.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1338 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/guitab.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1660 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/hexrand.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1685 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/hexrange.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1787 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/ipnet.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1741 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/iprange.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1630 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/list.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     3300 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/names.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1733 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/permutation.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1659 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/range.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1626 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/shodanp.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)      768 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/stdin.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2307 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/wfuzzp.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.508912 wfuzzserver-3.3.0/src/wfuzzserver/plugins/printers/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/printers/__init__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)    13490 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/printers/printers.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.508912 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/__init__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2080 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/backups.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1144 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/cookies.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1636 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/cvs_extractor.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     4140 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/errors.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1217 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/grep.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     5102 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/headers.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     5945 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/links.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1803 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/listing.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1692 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/npm_deps.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1824 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/robots.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1410 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/screenshot.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     1230 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/sitemap.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2211 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/svn_extractor.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)      893 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/title.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2508 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/wcdb.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.508912 wfuzzserver-3.3.0/src/wfuzzserver/ui/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/ui/__init__.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.512912 wfuzzserver-3.3.0/src/wfuzzserver/ui/console/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/ui/console/__init__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)    20252 2023-06-19 05:39:52.000000 wfuzzserver-3.3.0/src/wfuzzserver/ui/console/clparser.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)    15087 2023-06-19 05:37:37.000000 wfuzzserver-3.3.0/src/wfuzzserver/ui/console/common.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2634 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/ui/console/getch.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)    10791 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/ui/console/mvc.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     6657 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/ui/console/output.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.512912 wfuzzserver-3.3.0/src/wfuzzserver/ui/gui/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        0 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/ui/gui/__init__.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     2262 2023-06-19 05:40:54.000000 wfuzzserver-3.3.0/src/wfuzzserver/ui/gui/controller.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)    10862 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/ui/gui/guicontrols.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     3032 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/ui/gui/model.py
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     6755 2023-06-19 03:18:25.000000 wfuzzserver-3.3.0/src/wfuzzserver/wfuzz.py
+drwxrwxr-x   0 hussam    (1000) hussam    (1000)        0 2023-06-19 05:46:09.512912 wfuzzserver-3.3.0/wfuzzserver.egg-info/
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     3653 2023-06-19 05:46:09.000000 wfuzzserver-3.3.0/wfuzzserver.egg-info/PKG-INFO
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)     4583 2023-06-19 05:46:09.000000 wfuzzserver-3.3.0/wfuzzserver.egg-info/SOURCES.txt
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)        1 2023-06-19 05:46:09.000000 wfuzzserver-3.3.0/wfuzzserver.egg-info/dependency_links.txt
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)      209 2023-06-19 05:46:09.000000 wfuzzserver-3.3.0/wfuzzserver.egg-info/entry_points.txt
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)      275 2023-06-19 05:46:09.000000 wfuzzserver-3.3.0/wfuzzserver.egg-info/requires.txt
+-rw-rw-r--   0 hussam    (1000) hussam    (1000)       12 2023-06-19 05:46:09.000000 wfuzzserver-3.3.0/wfuzzserver.egg-info/top_level.txt
```

### Comparing `wfuzzserver-3.2.0/LICENSE` & `wfuzzserver-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/PKG-INFO` & `wfuzzserver-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfuzzserver
-Version: 3.2.0
+Version: 3.3.0
 Summary: Wfuzz - The web fuzzer
 Home-page: http://wfuzz.org
 Author: Xavi Mendez (@x4vi_mendez)
 Author-email: xmendez@edge-security.com
 License: GPLv2
 Description: <img src="https://github.com/xmendez/wfuzz/blob/master/docs/_static/logo/wfuzz_letters.svg" width="500">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wfuzzserver Version: 3.2.0 Summary: Wfuzz - The web
+Metadata-Version: 2.1 Name: wfuzzserver Version: 3.3.0 Summary: Wfuzz - The web
 fuzzer Home-page: http://wfuzz.org Author: Xavi Mendez (@x4vi_mendez) Author-
 email: xmendez@edge-security.com License: GPLv2 Description: [https://
 github.com/xmendez/wfuzz/blob/master/docs/_static/logo/wfuzz_letters.svg] [!
 [Build Status](https://travis-ci.org/xmendez/wfuzz.svg?branch=master)](https://
 travis-ci.org/xmendez/wfuzz) [https://img.shields.io/pypi/v/wfuzz.svg] [https:/
 /img.shields.io/pypi/dm/wfuzz] [https://img.shields.io/pypi/pyversions/
 wfuzz.svg] [https://codecov.io/github/xmendez/wfuzz/coverage.svg?branch=master]
```

### Comparing `wfuzzserver-3.2.0/README.md` & `wfuzzserver-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/docs/Makefile` & `wfuzzserver-3.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/docs/conf.py` & `wfuzzserver-3.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/docs/index.rst` & `wfuzzserver-3.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/docs/make.bat` & `wfuzzserver-3.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/setup.py` & `wfuzzserver-3.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                 'wfpayloadserver = wfuzzserver.wfuzz:main_filter',
                 'wfencodeserver = wfuzzserver.wfuzz:main_encoder',
             ],
             'gui_scripts': [
                 'wxfuzzserver = wfuzzserver.wfuzz:main_gui',
             ]
         },
-        version="3.2.0",
+        version="3.3.0",
         description="Wfuzz - The web fuzzer",
         long_description=long_descr,
         long_description_content_type='text/markdown',
         author="Xavi Mendez (@x4vi_mendez)",
         author_email="xmendez@edge-security.com",
         url="http://wfuzz.org",
         license="GPLv2",
```

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/__init__.py` & `wfuzzserver-3.3.0/src/wfuzzserver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __title__ = "wfuzz"
-__version__ = "3.2.0"
+__version__ = "3.3.0"
 __build__ = 0x023000
 __author__ = "Xavier Mendez"
 __license__ = "GPL 2.0"
 __copyright__ = "Copyright 2011-2020 Xavier Mendez"
 
 import logging
 import sys
```

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/api.py` & `wfuzzserver-3.3.0/src/wfuzzserver/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,9 +31,9 @@
 
 
 def payload(**kwargs):
     return FuzzSession(**kwargs).payload()
 
 
 def get_session(cline):
-    cl = ["wfuzz"] + cline.split("####")
+    cl = ["wfuzzserver"] + cline.split("####")
     return FuzzSession(**CLParser(cl).parse_cl())
```

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/core.py` & `wfuzzserver-3.3.0/src/wfuzzserver/core.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/dictionaries.py` & `wfuzzserver-3.3.0/src/wfuzzserver/dictionaries.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/exception.py` & `wfuzzserver-3.3.0/src/wfuzzserver/exception.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/externals/moduleman/loader.py` & `wfuzzserver-3.3.0/src/wfuzzserver/externals/moduleman/loader.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/externals/moduleman/modulefilter.py` & `wfuzzserver-3.3.0/src/wfuzzserver/externals/moduleman/modulefilter.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/externals/moduleman/plugin.py` & `wfuzzserver-3.3.0/src/wfuzzserver/externals/moduleman/plugin.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/externals/moduleman/registrant.py` & `wfuzzserver-3.3.0/src/wfuzzserver/externals/moduleman/registrant.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/externals/reqresp/Request.py` & `wfuzzserver-3.3.0/src/wfuzzserver/externals/reqresp/Request.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/externals/reqresp/Response.py` & `wfuzzserver-3.3.0/src/wfuzzserver/externals/reqresp/Response.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/externals/reqresp/TextParser.py` & `wfuzzserver-3.3.0/src/wfuzzserver/externals/reqresp/TextParser.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/externals/reqresp/Variables.py` & `wfuzzserver-3.3.0/src/wfuzzserver/externals/reqresp/Variables.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/externals/reqresp/cache.py` & `wfuzzserver-3.3.0/src/wfuzzserver/externals/reqresp/cache.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/externals/settings/settings.py` & `wfuzzserver-3.3.0/src/wfuzzserver/externals/settings/settings.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/facade.py` & `wfuzzserver-3.3.0/src/wfuzzserver/facade.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/factories/dictfactory.py` & `wfuzzserver-3.3.0/src/wfuzzserver/factories/dictfactory.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/factories/fuzzfactory.py` & `wfuzzserver-3.3.0/src/wfuzzserver/factories/fuzzfactory.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/factories/fuzzresfactory.py` & `wfuzzserver-3.3.0/src/wfuzzserver/factories/fuzzresfactory.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/factories/payman.py` & `wfuzzserver-3.3.0/src/wfuzzserver/factories/payman.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/factories/plugin_factory.py` & `wfuzzserver-3.3.0/src/wfuzzserver/factories/plugin_factory.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/factories/reqresp_factory.py` & `wfuzzserver-3.3.0/src/wfuzzserver/factories/reqresp_factory.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/filters/ppfilter.py` & `wfuzzserver-3.3.0/src/wfuzzserver/filters/ppfilter.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/filters/simplefilter.py` & `wfuzzserver-3.3.0/src/wfuzzserver/filters/simplefilter.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/fuzzobjects.py` & `wfuzzserver-3.3.0/src/wfuzzserver/fuzzobjects.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/fuzzqueues.py` & `wfuzzserver-3.3.0/src/wfuzzserver/fuzzqueues.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/fuzzrequest.py` & `wfuzzserver-3.3.0/src/wfuzzserver/fuzzrequest.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/helpers/file_func.py` & `wfuzzserver-3.3.0/src/wfuzzserver/helpers/file_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 
 def get_filter_help_file():
     FILTER_HELP_FILE = "advanced.rst"
     FILTER_HELP_DEV_FILE = "../../../docs/user/advanced.rst"
 
     filter_help_text = None
     try:
-        fname = pkg_resources.resource_filename("wfuzz", FILTER_HELP_FILE)
+        fname = pkg_resources.resource_filename("wfuzzserver", FILTER_HELP_FILE)
         filter_help_text = open(fname).read()
     except IOError:
         filter_help_text = open(get_path(FILTER_HELP_DEV_FILE)).read()
 
     return filter_help_text
 
 
 def create_dir(dir_path):
     if not os.path.exists(dir_path):
         os.makedirs(dir_path)
 
 
 def get_home(check=False, directory=None):
-    path = os.path.join(os.path.expanduser("~"), ".wfuzz")
+    path = os.path.join(os.path.expanduser("~"), ".wfuzzserver")
     if check:
         create_dir(path)
 
     return os.path.join(path, directory) if directory else path
 
 
 def get_config_dir(check=False):
     config_dir = os.environ.get("XDG_CONFIG_HOME") or os.path.join(
         os.path.expanduser("~"), ".config"
     )
-    wfuzz_config_dir = os.path.join(config_dir, "wfuzz")
+    wfuzz_config_dir = os.path.join(config_dir, "wfuzzserver")
     if check:
         create_dir(wfuzz_config_dir)
     return wfuzz_config_dir
 
 
 def get_path(directory=None):
     abspath = os.path.abspath(__file__)
```

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/helpers/obj_dic.py` & `wfuzzserver-3.3.0/src/wfuzzserver/helpers/obj_dic.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/helpers/obj_dyn.py` & `wfuzzserver-3.3.0/src/wfuzzserver/helpers/obj_dyn.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/helpers/obj_factory.py` & `wfuzzserver-3.3.0/src/wfuzzserver/helpers/obj_factory.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/helpers/str_func.py` & `wfuzzserver-3.3.0/src/wfuzzserver/helpers/str_func.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/helpers/utils.py` & `wfuzzserver-3.3.0/src/wfuzzserver/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/mixins.py` & `wfuzzserver-3.3.0/src/wfuzzserver/mixins.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/myhttp.py` & `wfuzzserver-3.3.0/src/wfuzzserver/myhttp.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/myqueues.py` & `wfuzzserver-3.3.0/src/wfuzzserver/myqueues.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/options.py` & `wfuzzserver-3.3.0/src/wfuzzserver/options.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugin_api/base.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugin_api/base.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugin_api/payloadtools.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugin_api/payloadtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
             raise FuzzExceptPluginLoadError(
                 "shodan module not imported. Please, install shodan using pip"
             )
 
         key = Facade().sett.get("plugins", "shodan_apikey")
         if not key:
             raise FuzzExceptMissingAPIKey(
-                "A Shodan api key is needed. Please check ~/.wfuzz/wfuzz.ini"
+                "A Shodan api key is needed. Please check ~/.wfuzzserver/wfuzz.ini"
             )
 
         self.api = shodan.Shodan(key)
         self._dork = dork
         self._page = MyCounter(page)
         self._page_limit = self._page() + limit if limit > 0 else -1
```

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugin_api/urlutils.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugin_api/urlutils.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/encoders/encoders.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/encoders/encoders.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/iterators/iterations.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/iterators/iterations.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/autorize.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/autorize.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/bing.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/bing.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/buffer_overflow.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/buffer_overflow.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/burpitem.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/burpitem.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/burplog.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/burplog.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/burpstate.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/burpstate.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/dirwalk.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/dirwalk.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/file.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/file.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/guitab.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/guitab.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/hexrand.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/hexrand.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/hexrange.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/hexrange.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/ipnet.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/ipnet.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/iprange.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/iprange.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/list.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/list.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/names.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/names.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/permutation.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/permutation.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/range.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/range.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/shodanp.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/shodanp.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/stdin.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/stdin.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/payloads/wfuzzp.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/payloads/wfuzzp.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/printers/printers.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/printers/printers.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/backups.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/backups.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/cookies.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/cookies.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/cvs_extractor.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/cvs_extractor.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/errors.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/errors.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/grep.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/grep.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/headers.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/headers.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/links.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/links.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/listing.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/listing.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/npm_deps.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/npm_deps.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/robots.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/robots.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/screenshot.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/screenshot.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/sitemap.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/sitemap.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/svn_extractor.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/svn_extractor.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/title.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/title.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/plugins/scripts/wcdb.py` & `wfuzzserver-3.3.0/src/wfuzzserver/plugins/scripts/wcdb.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/ui/console/clparser.py` & `wfuzzserver-3.3.0/src/wfuzzserver/ui/console/clparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from wfuzzserver.facade import Facade
 from wfuzzserver.options import FuzzSession
 from wfuzzserver.exception import FuzzException, FuzzExceptBadOptions, FuzzExceptBadInstall
 from .common import help_banner, exec_banner
 from .common import usage
 from .common import brief_usage
 from .common import verbose_usage
-from wfuzz import __version__ as version
+from wfuzzserver import __version__ as version
 from .output import table_print
 
 short_opts = "hLAZX:vcb:e:R:D:d:z:r:f:t:w:V:H:m:f:o:s:p:w:u:"
 long_opts = [
     "efield=",
     "no-cache",
     "ee=",
```

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/ui/console/common.py` & `wfuzzserver-3.3.0/src/wfuzzserver/ui/console/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from wfuzz import __version__ as version
+from wfuzzserver import __version__ as version
 import os
 
 if os.name == "nt":
     import colorama
 
     colorama.init()
```

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/ui/console/getch.py` & `wfuzzserver-3.3.0/src/wfuzzserver/ui/console/getch.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/ui/console/mvc.py` & `wfuzzserver-3.3.0/src/wfuzzserver/ui/console/mvc.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/ui/console/output.py` & `wfuzzserver-3.3.0/src/wfuzzserver/ui/console/output.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/ui/gui/controller.py` & `wfuzzserver-3.3.0/src/wfuzzserver/ui/gui/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class WfuzzInterpreter:
     def __init__(self, model):
         self.model = model
 
     def onecmd(self, cmd):
-        if cmd[0] == "wfuzz":
+        if cmd[0] == "wfuzzserver":
             self.do_wfuzz(cmd)
         elif cmd[0] == "clear":
             self.model.Clear()
         elif cmd[0] == "wfilter":
             self.do_wfilter(cmd)
         elif cmd[0] == "newtab":
             self.do_tab(cmd)
```

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/ui/gui/guicontrols.py` & `wfuzzserver-3.3.0/src/wfuzzserver/ui/gui/guicontrols.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/ui/gui/model.py` & `wfuzzserver-3.3.0/src/wfuzzserver/ui/gui/model.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/src/wfuzzserver/wfuzz.py` & `wfuzzserver-3.3.0/src/wfuzzserver/wfuzz.py`

 * *Files identical despite different names*

### Comparing `wfuzzserver-3.2.0/wfuzzserver.egg-info/PKG-INFO` & `wfuzzserver-3.3.0/wfuzzserver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfuzzserver
-Version: 3.2.0
+Version: 3.3.0
 Summary: Wfuzz - The web fuzzer
 Home-page: http://wfuzz.org
 Author: Xavi Mendez (@x4vi_mendez)
 Author-email: xmendez@edge-security.com
 License: GPLv2
 Description: <img src="https://github.com/xmendez/wfuzz/blob/master/docs/_static/logo/wfuzz_letters.svg" width="500">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wfuzzserver Version: 3.2.0 Summary: Wfuzz - The web
+Metadata-Version: 2.1 Name: wfuzzserver Version: 3.3.0 Summary: Wfuzz - The web
 fuzzer Home-page: http://wfuzz.org Author: Xavi Mendez (@x4vi_mendez) Author-
 email: xmendez@edge-security.com License: GPLv2 Description: [https://
 github.com/xmendez/wfuzz/blob/master/docs/_static/logo/wfuzz_letters.svg] [!
 [Build Status](https://travis-ci.org/xmendez/wfuzz.svg?branch=master)](https://
 travis-ci.org/xmendez/wfuzz) [https://img.shields.io/pypi/v/wfuzz.svg] [https:/
 /img.shields.io/pypi/dm/wfuzz] [https://img.shields.io/pypi/pyversions/
 wfuzz.svg] [https://codecov.io/github/xmendez/wfuzz/coverage.svg?branch=master]
```

### Comparing `wfuzzserver-3.2.0/wfuzzserver.egg-info/SOURCES.txt` & `wfuzzserver-3.3.0/wfuzzserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

